# Comparing `tmp/werk24-1.6.0.tar.gz` & `tmp/werk24-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/werk24-1.6.0.tar", last modified: Mon Jul 24 13:11:18 2023, max compression
+gzip compressed data, was "dist/werk24-1.6.1.tar", last modified: Fri Aug  4 10:52:54 2023, max compression
```

## Comparing `werk24-1.6.0.tar` & `werk24-1.6.1.tar`

### file list

```diff
@@ -1,108 +1,108 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:11:18.000000 werk24-1.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-24 13:10:49.000000 werk24-1.6.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-24 13:10:49.000000 werk24-1.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-24 13:10:49.000000 werk24-1.6.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     5074 2023-07-24 13:11:18.000000 werk24-1.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-07-24 13:10:49.000000 werk24-1.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 13:11:18.000000 werk24-1.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-07-24 13:10:49.000000 werk24-1.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:11:18.000000 werk24-1.6.0/werk24/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:11:18.000000 werk24-1.6.0/werk24/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:11:18.000000 werk24-1.6.0/werk24/assets/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)   366380 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/assets/fonts/STIX2Text-Regular.otf
--rw-r--r--   0 runner    (1001) docker     (123)   238007 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/assets/fonts/STIX_2.0.2_license.pdf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:11:18.000000 werk24-1.6.0/werk24/assets/images/
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/assets/images/favicon-16x16.png
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/assets/images/favicon-24x24.png
--rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/assets/images/favicon-256x256.png
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/assets/images/favicon-32x32.png
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/assets/images/favicon-48x48.png
--rw-r--r--   0 runner    (1001) docker     (123)     5598 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/assets/images/logo-625.png
--rw-r--r--   0 runner    (1001) docker     (123)     7748 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/auth_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:11:18.000000 werk24-1.6.0/werk24/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/cli/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/cli/support.py
--rw-r--r--   0 runner    (1001) docker     (123)     9939 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/cli/techread.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/cli/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4901 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/cli/w24cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:11:18.000000 werk24-1.6.0/werk24/gui/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/gui/event_feed.py
--rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/gui/event_illustrator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/gui/gdt_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/gui/json_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/gui/measure_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/gui/style.py
--rw-r--r--   0 runner    (1001) docker     (123)    23860 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/gui/w24gui.py
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/gui/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:11:18.000000 werk24-1.6.0/werk24/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/models/angle.py
--rw-r--r--   0 runner    (1001) docker     (123)    28765 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/models/ask.py
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/models/base_feature.py
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/models/chamfer.py
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/models/date.py
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/models/depth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:11:18.000000 werk24-1.6.0/werk24/models/feature/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/models/feature/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/models/feature/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/models/feature/chamfer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/models/feature/knurl.py
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/models/file_format.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/models/fraction.py
--rw-r--r--   0 runner    (1001) docker     (123)     9122 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/models/gdt.py
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/models/gender.py
--rw-r--r--   0 runner    (1001) docker     (123)     5910 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/models/general_tolerances.py
--rw-r--r--   0 runner    (1001) docker     (123)     4809 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/models/geometric_shape.py
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/models/helpdesk.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/models/language.py
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/models/leader.py
--rw-r--r--   0 runner    (1001) docker     (123)     6891 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/models/location.py
--rw-r--r--   0 runner    (1001) docker     (123)    13588 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/models/material.py
--rw-r--r--   0 runner    (1001) docker     (123)     6388 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/models/measure.py
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/models/note.py
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/models/paper_size.py
--rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/models/part_family.py
--rw-r--r--   0 runner    (1001) docker     (123)     9224 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/models/physical_quantity.py
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/models/process.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:11:18.000000 werk24-1.6.0/werk24/models/property/
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/models/property/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/models/property/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/models/property/cleanness.py
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/models/property/color.py
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/models/property/corrosion_resistance.py
--rw-r--r--   0 runner    (1001) docker     (123)     4285 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/models/property/hardness.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/models/property/material.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/models/property/surface_area.py
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/models/property/weight.py
--rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/models/radius.py
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/models/revision_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     9531 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/models/roughness.py
--rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/models/size.py
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/models/standard.py
--rw-r--r--   0 runner    (1001) docker     (123)     9614 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/models/techread.py
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/models/test_dimension.py
--rw-r--r--   0 runner    (1001) docker     (123)    12306 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/models/thread.py
--rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/models/thread_element.py
--rw-r--r--   0 runner    (1001) docker     (123)     7550 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/models/title_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     6548 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/models/tolerance.py
--rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/models/typed_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/models/unit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/models/value.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/models/view.py
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/models/weight.py
--rw-r--r--   0 runner    (1001) docker     (123)    32337 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/techread_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15169 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/techread_client_https.py
--rw-r--r--   0 runner    (1001) docker     (123)     7198 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/techread_client_wss.py
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-07-24 13:10:49.000000 werk24-1.6.0/werk24/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:11:18.000000 werk24-1.6.0/werk24.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5074 2023-07-24 13:11:17.000000 werk24-1.6.0/werk24.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-07-24 13:11:18.000000 werk24-1.6.0/werk24.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 13:11:17.000000 werk24-1.6.0/werk24.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-24 13:11:17.000000 werk24-1.6.0/werk24.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-24 13:11:17.000000 werk24-1.6.0/werk24.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-24 13:11:17.000000 werk24-1.6.0/werk24.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:52:54.000000 werk24-1.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-08-04 10:52:41.000000 werk24-1.6.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-08-04 10:52:41.000000 werk24-1.6.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-08-04 10:52:41.000000 werk24-1.6.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     5074 2023-08-04 10:52:54.000000 werk24-1.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-08-04 10:52:41.000000 werk24-1.6.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 10:52:54.000000 werk24-1.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-08-04 10:52:41.000000 werk24-1.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:52:54.000000 werk24-1.6.1/werk24/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-08-04 10:52:41.000000 werk24-1.6.1/werk24/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-04 10:52:41.000000 werk24-1.6.1/werk24/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:52:54.000000 werk24-1.6.1/werk24/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:52:54.000000 werk24-1.6.1/werk24/assets/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)   366380 2023-08-04 10:52:41.000000 werk24-1.6.1/werk24/assets/fonts/STIX2Text-Regular.otf
+-rw-r--r--   0 runner    (1001) docker     (123)   238007 2023-08-04 10:52:41.000000 werk24-1.6.1/werk24/assets/fonts/STIX_2.0.2_license.pdf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:52:54.000000 werk24-1.6.1/werk24/assets/images/
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-08-04 10:52:41.000000 werk24-1.6.1/werk24/assets/images/favicon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-08-04 10:52:41.000000 werk24-1.6.1/werk24/assets/images/favicon-24x24.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-08-04 10:52:41.000000 werk24-1.6.1/werk24/assets/images/favicon-256x256.png
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-08-04 10:52:41.000000 werk24-1.6.1/werk24/assets/images/favicon-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-08-04 10:52:41.000000 werk24-1.6.1/werk24/assets/images/favicon-48x48.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5598 2023-08-04 10:52:41.000000 werk24-1.6.1/werk24/assets/images/logo-625.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7748 2023-08-04 10:52:41.000000 werk24-1.6.1/werk24/auth_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:52:54.000000 werk24-1.6.1/werk24/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 10:52:41.000000 werk24-1.6.1/werk24/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-08-04 10:52:41.000000 werk24-1.6.1/werk24/cli/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-08-04 10:52:41.000000 werk24-1.6.1/werk24/cli/support.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9939 2023-08-04 10:52:41.000000 werk24-1.6.1/werk24/cli/techread.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-08-04 10:52:41.000000 werk24-1.6.1/werk24/cli/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4901 2023-08-04 10:52:41.000000 werk24-1.6.1/werk24/cli/w24cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-08-04 10:52:41.000000 werk24-1.6.1/werk24/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:52:54.000000 werk24-1.6.1/werk24/gui/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 10:52:41.000000 werk24-1.6.1/werk24/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-08-04 10:52:41.000000 werk24-1.6.1/werk24/gui/event_feed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-08-04 10:52:41.000000 werk24-1.6.1/werk24/gui/event_illustrator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-08-04 10:52:41.000000 werk24-1.6.1/werk24/gui/gdt_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-08-04 10:52:41.000000 werk24-1.6.1/werk24/gui/json_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-08-04 10:52:41.000000 werk24-1.6.1/werk24/gui/measure_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-08-04 10:52:41.000000 werk24-1.6.1/werk24/gui/style.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23860 2023-08-04 10:52:41.000000 werk24-1.6.1/werk24/gui/w24gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-08-04 10:52:41.000000 werk24-1.6.1/werk24/gui/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:52:54.000000 werk24-1.6.1/werk24/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 10:52:41.000000 werk24-1.6.1/werk24/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-08-04 10:52:41.000000 werk24-1.6.1/werk24/models/angle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28765 2023-08-04 10:52:41.000000 werk24-1.6.1/werk24/models/ask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-08-04 10:52:41.000000 werk24-1.6.1/werk24/models/base_feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-08-04 10:52:41.000000 werk24-1.6.1/werk24/models/chamfer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-08-04 10:52:41.000000 werk24-1.6.1/werk24/models/date.py
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-08-04 10:52:41.000000 werk24-1.6.1/werk24/models/depth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:52:54.000000 werk24-1.6.1/werk24/models/feature/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 10:52:41.000000 werk24-1.6.1/werk24/models/feature/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-08-04 10:52:41.000000 werk24-1.6.1/werk24/models/feature/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-08-04 10:52:41.000000 werk24-1.6.1/werk24/models/feature/chamfer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-08-04 10:52:41.000000 werk24-1.6.1/werk24/models/feature/knurl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-08-04 10:52:41.000000 werk24-1.6.1/werk24/models/file_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-08-04 10:52:41.000000 werk24-1.6.1/werk24/models/fraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9122 2023-08-04 10:52:41.000000 werk24-1.6.1/werk24/models/gdt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-08-04 10:52:41.000000 werk24-1.6.1/werk24/models/gender.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5910 2023-08-04 10:52:41.000000 werk24-1.6.1/werk24/models/general_tolerances.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4809 2023-08-04 10:52:41.000000 werk24-1.6.1/werk24/models/geometric_shape.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-08-04 10:52:41.000000 werk24-1.6.1/werk24/models/helpdesk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-08-04 10:52:41.000000 werk24-1.6.1/werk24/models/language.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-08-04 10:52:41.000000 werk24-1.6.1/werk24/models/leader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6891 2023-08-04 10:52:41.000000 werk24-1.6.1/werk24/models/location.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13870 2023-08-04 10:52:41.000000 werk24-1.6.1/werk24/models/material.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6388 2023-08-04 10:52:41.000000 werk24-1.6.1/werk24/models/measure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-08-04 10:52:41.000000 werk24-1.6.1/werk24/models/note.py
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-08-04 10:52:41.000000 werk24-1.6.1/werk24/models/paper_size.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-08-04 10:52:41.000000 werk24-1.6.1/werk24/models/part_family.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9224 2023-08-04 10:52:41.000000 werk24-1.6.1/werk24/models/physical_quantity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-08-04 10:52:41.000000 werk24-1.6.1/werk24/models/process.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:52:54.000000 werk24-1.6.1/werk24/models/property/
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-08-04 10:52:41.000000 werk24-1.6.1/werk24/models/property/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-08-04 10:52:41.000000 werk24-1.6.1/werk24/models/property/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-08-04 10:52:41.000000 werk24-1.6.1/werk24/models/property/cleanness.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-08-04 10:52:41.000000 werk24-1.6.1/werk24/models/property/color.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-08-04 10:52:41.000000 werk24-1.6.1/werk24/models/property/corrosion_resistance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4285 2023-08-04 10:52:41.000000 werk24-1.6.1/werk24/models/property/hardness.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-08-04 10:52:41.000000 werk24-1.6.1/werk24/models/property/material.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-08-04 10:52:41.000000 werk24-1.6.1/werk24/models/property/surface_area.py
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-08-04 10:52:41.000000 werk24-1.6.1/werk24/models/property/weight.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-08-04 10:52:41.000000 werk24-1.6.1/werk24/models/radius.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-08-04 10:52:41.000000 werk24-1.6.1/werk24/models/revision_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9531 2023-08-04 10:52:41.000000 werk24-1.6.1/werk24/models/roughness.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-08-04 10:52:41.000000 werk24-1.6.1/werk24/models/size.py
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-08-04 10:52:41.000000 werk24-1.6.1/werk24/models/standard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9614 2023-08-04 10:52:41.000000 werk24-1.6.1/werk24/models/techread.py
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-08-04 10:52:41.000000 werk24-1.6.1/werk24/models/test_dimension.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12306 2023-08-04 10:52:41.000000 werk24-1.6.1/werk24/models/thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-08-04 10:52:41.000000 werk24-1.6.1/werk24/models/thread_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7550 2023-08-04 10:52:41.000000 werk24-1.6.1/werk24/models/title_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6548 2023-08-04 10:52:41.000000 werk24-1.6.1/werk24/models/tolerance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-08-04 10:52:41.000000 werk24-1.6.1/werk24/models/typed_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-08-04 10:52:41.000000 werk24-1.6.1/werk24/models/unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-08-04 10:52:41.000000 werk24-1.6.1/werk24/models/value.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-08-04 10:52:41.000000 werk24-1.6.1/werk24/models/view.py
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-08-04 10:52:41.000000 werk24-1.6.1/werk24/models/weight.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32337 2023-08-04 10:52:41.000000 werk24-1.6.1/werk24/techread_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15169 2023-08-04 10:52:41.000000 werk24-1.6.1/werk24/techread_client_https.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7198 2023-08-04 10:52:41.000000 werk24-1.6.1/werk24/techread_client_wss.py
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-08-04 10:52:41.000000 werk24-1.6.1/werk24/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:52:54.000000 werk24-1.6.1/werk24.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5074 2023-08-04 10:52:53.000000 werk24-1.6.1/werk24.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-08-04 10:52:54.000000 werk24-1.6.1/werk24.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 10:52:53.000000 werk24-1.6.1/werk24.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-08-04 10:52:53.000000 werk24-1.6.1/werk24.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-08-04 10:52:53.000000 werk24-1.6.1/werk24.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-04 10:52:53.000000 werk24-1.6.1/werk24.egg-info/top_level.txt
```

### Comparing `werk24-1.6.0/PKG-INFO` & `werk24-1.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: werk24
-Version: 1.6.0
+Version: 1.6.1
 Summary: Werk24 Client to read PDF- and Image-based Technical Drawings / Engineering Drawings
 Home-page: https://werk24.io
 Author: W24 Service GmbH
 Author-email: info@werk24.io
 License: commercial
 Project-URL: Documentation, https://docs.werk24.io/
 Description: # Werk24 Client
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: werk24 Version: 1.6.0 Summary: Werk24 Client to
+Metadata-Version: 2.1 Name: werk24 Version: 1.6.1 Summary: Werk24 Client to
 read PDF- and Image-based Technical Drawings / Engineering Drawings Home-page:
 https://werk24.io Author: W24 Service GmbH Author-email: info@werk24.io
 License: commercial Project-URL: Documentation, https://docs.werk24.io/
 Description: # Werk24 Client
                                    [Werk24]
 [![pypi](https://img.shields.io/pypi/v/werk24.svg)](https://pypi.python.org/
 pypi/werk24) [![Tests | cpython 3.8, 3.9, 3.10](https://github.com/W24-Service-
```

### Comparing `werk24-1.6.0/README.md` & `werk24-1.6.1/README.md`

 * *Files identical despite different names*

### Comparing `werk24-1.6.0/setup.py` & `werk24-1.6.1/setup.py`

 * *Files identical despite different names*

### Comparing `werk24-1.6.0/werk24/assets/fonts/STIX2Text-Regular.otf` & `werk24-1.6.1/werk24/assets/fonts/STIX2Text-Regular.otf`

 * *Files identical despite different names*

### Comparing `werk24-1.6.0/werk24/assets/fonts/STIX_2.0.2_license.pdf` & `werk24-1.6.1/werk24/assets/fonts/STIX_2.0.2_license.pdf`

 * *Files identical despite different names*

### Comparing `werk24-1.6.0/werk24/assets/images/favicon-256x256.png` & `werk24-1.6.1/werk24/assets/images/favicon-256x256.png`

 * *Files identical despite different names*

### Comparing `werk24-1.6.0/werk24/assets/images/favicon-32x32.png` & `werk24-1.6.1/werk24/assets/images/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `werk24-1.6.0/werk24/assets/images/favicon-48x48.png` & `werk24-1.6.1/werk24/assets/images/favicon-48x48.png`

 * *Files identical despite different names*

### Comparing `werk24-1.6.0/werk24/assets/images/logo-625.png` & `werk24-1.6.1/werk24/assets/images/logo-625.png`

 * *Files identical despite different names*

### Comparing `werk24-1.6.0/werk24/auth_client.py` & `werk24-1.6.1/werk24/auth_client.py`

 * *Files identical despite different names*

### Comparing `werk24-1.6.0/werk24/cli/auth.py` & `werk24-1.6.1/werk24/cli/auth.py`

 * *Files identical despite different names*

### Comparing `werk24-1.6.0/werk24/cli/support.py` & `werk24-1.6.1/werk24/cli/support.py`

 * *Files identical despite different names*

### Comparing `werk24-1.6.0/werk24/cli/techread.py` & `werk24-1.6.1/werk24/cli/techread.py`

 * *Files identical despite different names*

### Comparing `werk24-1.6.0/werk24/cli/utils.py` & `werk24-1.6.1/werk24/cli/utils.py`

 * *Files identical despite different names*

### Comparing `werk24-1.6.0/werk24/cli/w24cli.py` & `werk24-1.6.1/werk24/cli/w24cli.py`

 * *Files identical despite different names*

### Comparing `werk24-1.6.0/werk24/exceptions.py` & `werk24-1.6.1/werk24/exceptions.py`

 * *Files identical despite different names*

### Comparing `werk24-1.6.0/werk24/gui/event_feed.py` & `werk24-1.6.1/werk24/gui/event_feed.py`

 * *Files identical despite different names*

### Comparing `werk24-1.6.0/werk24/gui/event_illustrator.py` & `werk24-1.6.1/werk24/gui/event_illustrator.py`

 * *Files identical despite different names*

### Comparing `werk24-1.6.0/werk24/gui/gdt_table.py` & `werk24-1.6.1/werk24/gui/gdt_table.py`

 * *Files identical despite different names*

### Comparing `werk24-1.6.0/werk24/gui/measure_table.py` & `werk24-1.6.1/werk24/gui/measure_table.py`

 * *Files identical despite different names*

### Comparing `werk24-1.6.0/werk24/gui/w24gui.py` & `werk24-1.6.1/werk24/gui/w24gui.py`

 * *Files identical despite different names*

### Comparing `werk24-1.6.0/werk24/gui/worker.py` & `werk24-1.6.1/werk24/gui/worker.py`

 * *Files identical despite different names*

### Comparing `werk24-1.6.0/werk24/models/angle.py` & `werk24-1.6.1/werk24/models/angle.py`

 * *Files identical despite different names*

### Comparing `werk24-1.6.0/werk24/models/ask.py` & `werk24-1.6.1/werk24/models/ask.py`

 * *Files identical despite different names*

### Comparing `werk24-1.6.0/werk24/models/base_feature.py` & `werk24-1.6.1/werk24/models/base_feature.py`

 * *Files identical despite different names*

### Comparing `werk24-1.6.0/werk24/models/chamfer.py` & `werk24-1.6.1/werk24/models/chamfer.py`

 * *Files identical despite different names*

### Comparing `werk24-1.6.0/werk24/models/depth.py` & `werk24-1.6.1/werk24/models/depth.py`

 * *Files identical despite different names*

### Comparing `werk24-1.6.0/werk24/models/feature/base.py` & `werk24-1.6.1/werk24/models/feature/base.py`

 * *Files identical despite different names*

### Comparing `werk24-1.6.0/werk24/models/feature/knurl.py` & `werk24-1.6.1/werk24/models/feature/knurl.py`

 * *Files identical despite different names*

### Comparing `werk24-1.6.0/werk24/models/file_format.py` & `werk24-1.6.1/werk24/models/file_format.py`

 * *Files identical despite different names*

### Comparing `werk24-1.6.0/werk24/models/gdt.py` & `werk24-1.6.1/werk24/models/gdt.py`

 * *Files identical despite different names*

### Comparing `werk24-1.6.0/werk24/models/general_tolerances.py` & `werk24-1.6.1/werk24/models/general_tolerances.py`

 * *Files identical despite different names*

### Comparing `werk24-1.6.0/werk24/models/geometric_shape.py` & `werk24-1.6.1/werk24/models/geometric_shape.py`

 * *Files identical despite different names*

### Comparing `werk24-1.6.0/werk24/models/helpdesk.py` & `werk24-1.6.1/werk24/models/helpdesk.py`

 * *Files identical despite different names*

### Comparing `werk24-1.6.0/werk24/models/leader.py` & `werk24-1.6.1/werk24/models/leader.py`

 * *Files identical despite different names*

### Comparing `werk24-1.6.0/werk24/models/location.py` & `werk24-1.6.1/werk24/models/location.py`

 * *Files identical despite different names*

### Comparing `werk24-1.6.0/werk24/models/material.py` & `werk24-1.6.1/werk24/models/material.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,14 @@
     POLYMER = "POLYMER"
     CERAMIC = "CERAMIC"
     COMPOSITE = "COMPOSITE"
     ORGANIC = "ORGANIC"
 
 
 class W24MaterialCategory2(str, Enum):
-
     # FERROUS ALLOYS
     STEEL = "STEEL"
     IRON = "IRON"
     MAGNETIC_OR_ELECTRICAL_MATERIAL = "MAGNETIC_OR_ELECTRICAL_MATERIAL"
     SINTERED_POWDEDERD_METAL = "SINTERED_POWDEDERD_METAL"
     WELDING_FILLER_MATERIAL = "WELDING_FILLER_MATERIAL"
 
@@ -69,15 +68,14 @@
     REINFORCEMENT = "REINFORCEMENT"
 
     # ORGANIC
     WOOD = "WOOD"
 
 
 class W24MaterialCategory3(str, Enum):
-
     # FERROUS_ALLOY / STEEL
     STRUCTURAL_OR_CONSTRUCTIONAL_STEEL = "STRUCTURAL_OR_CONSTRUCTIONAL_STEEL"
     STAINLESS_STEEL = "STAINLESS_STEEL"
     TOOL_STEEL = "TOOL_STEEL"
     CAST_STEEL = "CAST_STEEL"
 
     # FERROUS_ALLOY / IRON
@@ -503,29 +501,37 @@
     text on the canvas.
 
     Attributes:
         blurb: Material Name for human consumption.
             This will typically include the designation
             and the standard.
 
+        raw_ocr_blurb: Material Name as it was indicated
+            on the drawing. This contains more information
+            than the blurb and is also present when the
+            material was not found in the internal
+            material database.
+
         standard: Material Standard indicated
             on the technical drawing. This used to be
             an enum - but we now have over 100 supported
             material standards and the number is increasing
             weekly. So a string seems to be more appropriate.
 
         designation: Name of the material in accordance
             with the material standard. An alternative name
             would be material_designation.
 
         material_category: Categorization of the material
             following W24MaterialCategoryX Tree.
 
     """
+
     blurb: str
+    raw_ocr_blurb: str = ""
     standard: str
     designation: str
     material_category: Tuple[
         Optional[W24MaterialCategory1],
         Optional[W24MaterialCategory2],
         Optional[W24MaterialCategory3],
     ]
```

### Comparing `werk24-1.6.0/werk24/models/measure.py` & `werk24-1.6.1/werk24/models/measure.py`

 * *Files identical despite different names*

### Comparing `werk24-1.6.0/werk24/models/note.py` & `werk24-1.6.1/werk24/models/note.py`

 * *Files identical despite different names*

### Comparing `werk24-1.6.0/werk24/models/paper_size.py` & `werk24-1.6.1/werk24/models/paper_size.py`

 * *Files identical despite different names*

### Comparing `werk24-1.6.0/werk24/models/part_family.py` & `werk24-1.6.1/werk24/models/part_family.py`

 * *Files identical despite different names*

### Comparing `werk24-1.6.0/werk24/models/physical_quantity.py` & `werk24-1.6.1/werk24/models/physical_quantity.py`

 * *Files identical despite different names*

### Comparing `werk24-1.6.0/werk24/models/property/cleanness.py` & `werk24-1.6.1/werk24/models/property/cleanness.py`

 * *Files identical despite different names*

### Comparing `werk24-1.6.0/werk24/models/property/color.py` & `werk24-1.6.1/werk24/models/property/color.py`

 * *Files identical despite different names*

### Comparing `werk24-1.6.0/werk24/models/property/corrosion_resistance.py` & `werk24-1.6.1/werk24/models/property/corrosion_resistance.py`

 * *Files identical despite different names*

### Comparing `werk24-1.6.0/werk24/models/property/hardness.py` & `werk24-1.6.1/werk24/models/property/hardness.py`

 * *Files identical despite different names*

### Comparing `werk24-1.6.0/werk24/models/property/material.py` & `werk24-1.6.1/werk24/models/property/material.py`

 * *Files identical despite different names*

### Comparing `werk24-1.6.0/werk24/models/property/surface_area.py` & `werk24-1.6.1/werk24/models/property/surface_area.py`

 * *Files identical despite different names*

### Comparing `werk24-1.6.0/werk24/models/property/weight.py` & `werk24-1.6.1/werk24/models/property/weight.py`

 * *Files identical despite different names*

### Comparing `werk24-1.6.0/werk24/models/radius.py` & `werk24-1.6.1/werk24/models/radius.py`

 * *Files identical despite different names*

### Comparing `werk24-1.6.0/werk24/models/revision_table.py` & `werk24-1.6.1/werk24/models/revision_table.py`

 * *Files identical despite different names*

### Comparing `werk24-1.6.0/werk24/models/roughness.py` & `werk24-1.6.1/werk24/models/roughness.py`

 * *Files identical despite different names*

### Comparing `werk24-1.6.0/werk24/models/size.py` & `werk24-1.6.1/werk24/models/size.py`

 * *Files identical despite different names*

### Comparing `werk24-1.6.0/werk24/models/techread.py` & `werk24-1.6.1/werk24/models/techread.py`

 * *Files identical despite different names*

### Comparing `werk24-1.6.0/werk24/models/test_dimension.py` & `werk24-1.6.1/werk24/models/test_dimension.py`

 * *Files identical despite different names*

### Comparing `werk24-1.6.0/werk24/models/thread.py` & `werk24-1.6.1/werk24/models/thread.py`

 * *Files identical despite different names*

### Comparing `werk24-1.6.0/werk24/models/thread_element.py` & `werk24-1.6.1/werk24/models/thread_element.py`

 * *Files identical despite different names*

### Comparing `werk24-1.6.0/werk24/models/title_block.py` & `werk24-1.6.1/werk24/models/title_block.py`

 * *Files identical despite different names*

### Comparing `werk24-1.6.0/werk24/models/tolerance.py` & `werk24-1.6.1/werk24/models/tolerance.py`

 * *Files identical despite different names*

### Comparing `werk24-1.6.0/werk24/models/typed_model.py` & `werk24-1.6.1/werk24/models/typed_model.py`

 * *Files identical despite different names*

### Comparing `werk24-1.6.0/werk24/models/unit.py` & `werk24-1.6.1/werk24/models/unit.py`

 * *Files identical despite different names*

### Comparing `werk24-1.6.0/werk24/models/value.py` & `werk24-1.6.1/werk24/models/value.py`

 * *Files identical despite different names*

### Comparing `werk24-1.6.0/werk24/models/view.py` & `werk24-1.6.1/werk24/models/view.py`

 * *Files identical despite different names*

### Comparing `werk24-1.6.0/werk24/models/weight.py` & `werk24-1.6.1/werk24/models/weight.py`

 * *Files identical despite different names*

### Comparing `werk24-1.6.0/werk24/techread_client.py` & `werk24-1.6.1/werk24/techread_client.py`

 * *Files identical despite different names*

### Comparing `werk24-1.6.0/werk24/techread_client_https.py` & `werk24-1.6.1/werk24/techread_client_https.py`

 * *Files identical despite different names*

### Comparing `werk24-1.6.0/werk24/techread_client_wss.py` & `werk24-1.6.1/werk24/techread_client_wss.py`

 * *Files identical despite different names*

### Comparing `werk24-1.6.0/werk24/utils.py` & `werk24-1.6.1/werk24/utils.py`

 * *Files identical despite different names*

### Comparing `werk24-1.6.0/werk24.egg-info/PKG-INFO` & `werk24-1.6.1/werk24.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: werk24
-Version: 1.6.0
+Version: 1.6.1
 Summary: Werk24 Client to read PDF- and Image-based Technical Drawings / Engineering Drawings
 Home-page: https://werk24.io
 Author: W24 Service GmbH
 Author-email: info@werk24.io
 License: commercial
 Project-URL: Documentation, https://docs.werk24.io/
 Description: # Werk24 Client
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: werk24 Version: 1.6.0 Summary: Werk24 Client to
+Metadata-Version: 2.1 Name: werk24 Version: 1.6.1 Summary: Werk24 Client to
 read PDF- and Image-based Technical Drawings / Engineering Drawings Home-page:
 https://werk24.io Author: W24 Service GmbH Author-email: info@werk24.io
 License: commercial Project-URL: Documentation, https://docs.werk24.io/
 Description: # Werk24 Client
                                    [Werk24]
 [![pypi](https://img.shields.io/pypi/v/werk24.svg)](https://pypi.python.org/
 pypi/werk24) [![Tests | cpython 3.8, 3.9, 3.10](https://github.com/W24-Service-
```

### Comparing `werk24-1.6.0/werk24.egg-info/SOURCES.txt` & `werk24-1.6.1/werk24.egg-info/SOURCES.txt`

 * *Files identical despite different names*

