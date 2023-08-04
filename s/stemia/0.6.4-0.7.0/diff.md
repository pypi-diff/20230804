# Comparing `tmp/stemia-0.6.4.tar.gz` & `tmp/stemia-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stemia-0.6.4.tar", last modified: Thu Aug  3 09:37:45 2023, max compression
+gzip compressed data, was "stemia-0.7.0.tar", last modified: Fri Aug  4 15:11:36 2023, max compression
```

## Comparing `stemia-0.6.4.tar` & `stemia-0.7.0.tar`

### file list

```diff
@@ -1,78 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:37:45.747343 stemia-0.6.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:37:45.731342 stemia-0.6.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:37:45.735343 stemia-0.6.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-08-03 09:37:26.000000 stemia-0.6.4/.github/workflows/deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-03 09:37:26.000000 stemia-0.6.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-08-03 09:37:26.000000 stemia-0.6.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13839 2023-08-03 09:37:45.747343 stemia-0.6.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13350 2023-08-03 09:37:26.000000 stemia-0.6.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:37:45.735343 stemia-0.6.4/docs/
--rwxr-xr-x   0 runner    (1001) docker     (123)      568 2023-08-03 09:37:26.000000 stemia-0.6.4/docs/generate_readme.py
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-08-03 09:37:26.000000 stemia-0.6.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-03 09:37:45.747343 stemia-0.6.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:37:45.735343 stemia-0.6.4/stemia/
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-08-03 09:37:26.000000 stemia-0.6.4/stemia/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-08-03 09:37:45.000000 stemia-0.6.4/stemia/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:37:45.739343 stemia-0.6.4/stemia/aretomo/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-03 09:37:26.000000 stemia-0.6.4/stemia/aretomo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-08-03 09:37:26.000000 stemia-0.6.4/stemia/aretomo/aln2xf.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      343 2023-08-03 09:37:26.000000 stemia-0.6.4/stemia/aretomo/batch.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:37:45.739343 stemia-0.6.4/stemia/aretomo/batch_warp/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-03 09:37:26.000000 stemia-0.6.4/stemia/aretomo/batch_warp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4743 2023-08-03 09:37:26.000000 stemia-0.6.4/stemia/aretomo/batch_warp/aretomo.py
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-08-03 09:37:26.000000 stemia-0.6.4/stemia/aretomo/batch_warp/fix.py
--rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-08-03 09:37:26.000000 stemia-0.6.4/stemia/aretomo/batch_warp/fix_mdoc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8816 2023-08-03 09:37:26.000000 stemia-0.6.4/stemia/aretomo/batch_warp/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     4225 2023-08-03 09:37:26.000000 stemia-0.6.4/stemia/aretomo/batch_warp/parse.py
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-08-03 09:37:26.000000 stemia-0.6.4/stemia/aretomo/batch_warp/stack.py
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-08-03 09:37:26.000000 stemia-0.6.4/stemia/aretomo/batch_warp/threaded.py
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-08-03 09:37:26.000000 stemia-0.6.4/stemia/aretomo/batch_warp/topaz.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:37:45.739343 stemia-0.6.4/stemia/cryosparc/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-03 09:37:26.000000 stemia-0.6.4/stemia/cryosparc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:37:45.743343 stemia-0.6.4/stemia/cryosparc/csplot/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-03 09:37:26.000000 stemia-0.6.4/stemia/cryosparc/csplot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-08-03 09:37:26.000000 stemia-0.6.4/stemia/cryosparc/csplot/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     6768 2023-08-03 09:37:26.000000 stemia-0.6.4/stemia/cryosparc/csplot/parse.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-08-03 09:37:26.000000 stemia-0.6.4/stemia/cryosparc/csplot/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-08-03 09:37:26.000000 stemia-0.6.4/stemia/cryosparc/fix_filament_ids.py
--rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-08-03 09:37:26.000000 stemia-0.6.4/stemia/cryosparc/generate_tilt_angles.py
--rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-08-03 09:37:26.000000 stemia-0.6.4/stemia/cryosparc/merge_defects_gainref.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:37:45.743343 stemia-0.6.4/stemia/image/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-08-03 09:37:26.000000 stemia-0.6.4/stemia/image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:37:45.743343 stemia-0.6.4/stemia/image/center_filament/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-03 09:37:26.000000 stemia-0.6.4/stemia/image/center_filament/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2696 2023-08-03 09:37:26.000000 stemia-0.6.4/stemia/image/center_filament/center_filament.py
--rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-08-03 09:37:26.000000 stemia-0.6.4/stemia/image/center_filament/funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-08-03 09:37:26.000000 stemia-0.6.4/stemia/image/create_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-08-03 09:37:26.000000 stemia-0.6.4/stemia/image/extract_z_snapshots.py
--rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-08-03 09:37:26.000000 stemia-0.6.4/stemia/image/flip_z.py
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-08-03 09:37:26.000000 stemia-0.6.4/stemia/image/fourier_crop.py
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-08-03 09:37:26.000000 stemia-0.6.4/stemia/image/rescale.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:37:45.743343 stemia-0.6.4/stemia/imod/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 09:37:26.000000 stemia-0.6.4/stemia/imod/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-08-03 09:37:26.000000 stemia-0.6.4/stemia/imod/find_NAD_params.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:37:45.743343 stemia-0.6.4/stemia/relion/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-08-03 09:37:26.000000 stemia-0.6.4/stemia/relion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-08-03 09:37:26.000000 stemia-0.6.4/stemia/relion/align_filament_particles.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:37:45.743343 stemia-0.6.4/stemia/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 09:37:26.000000 stemia-0.6.4/stemia/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-08-03 09:37:26.000000 stemia-0.6.4/stemia/utils/click.py
--rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-08-03 09:37:26.000000 stemia-0.6.4/stemia/utils/image_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-08-03 09:37:26.000000 stemia-0.6.4/stemia/utils/io_.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:37:45.747343 stemia-0.6.4/stemia/warp/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-08-03 09:37:26.000000 stemia-0.6.4/stemia/warp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-08-03 09:37:26.000000 stemia-0.6.4/stemia/warp/fix_mdoc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-08-03 09:37:26.000000 stemia-0.6.4/stemia/warp/offset_angle.py
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-08-03 09:37:26.000000 stemia-0.6.4/stemia/warp/parse_xml.py
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-08-03 09:37:26.000000 stemia-0.6.4/stemia/warp/prepare_isonet.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1252 2023-08-03 09:37:26.000000 stemia-0.6.4/stemia/warp/preprocess_serialem.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-08-03 09:37:26.000000 stemia-0.6.4/stemia/warp/spoof_mdoc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-08-03 09:37:26.000000 stemia-0.6.4/stemia/warp/summarize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:37:45.739343 stemia-0.6.4/stemia.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13839 2023-08-03 09:37:45.000000 stemia-0.6.4/stemia.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-08-03 09:37:45.000000 stemia-0.6.4/stemia.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 09:37:45.000000 stemia-0.6.4/stemia.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 09:37:45.000000 stemia-0.6.4/stemia.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 09:37:45.000000 stemia-0.6.4/stemia.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-08-03 09:37:45.000000 stemia-0.6.4/stemia.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-03 09:37:45.000000 stemia-0.6.4/stemia.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:11:36.933989 stemia-0.7.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:11:36.925989 stemia-0.7.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:11:36.925989 stemia-0.7.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-08-04 15:11:18.000000 stemia-0.7.0/.github/workflows/deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-04 15:11:18.000000 stemia-0.7.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-08-04 15:11:18.000000 stemia-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13839 2023-08-04 15:11:36.933989 stemia-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13350 2023-08-04 15:11:18.000000 stemia-0.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:11:36.925989 stemia-0.7.0/docs/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      568 2023-08-04 15:11:18.000000 stemia-0.7.0/docs/generate_readme.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-08-04 15:11:18.000000 stemia-0.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-08-04 15:11:36.933989 stemia-0.7.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:11:36.925989 stemia-0.7.0/stemia/
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-08-04 15:11:18.000000 stemia-0.7.0/stemia/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-08-04 15:11:36.000000 stemia-0.7.0/stemia/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:11:36.929988 stemia-0.7.0/stemia/aretomo/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-04 15:11:18.000000 stemia-0.7.0/stemia/aretomo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-08-04 15:11:18.000000 stemia-0.7.0/stemia/aretomo/aln2xf.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      343 2023-08-04 15:11:18.000000 stemia-0.7.0/stemia/aretomo/batch.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:11:36.929988 stemia-0.7.0/stemia/aretomo/batch_warp/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-04 15:11:18.000000 stemia-0.7.0/stemia/aretomo/batch_warp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4743 2023-08-04 15:11:18.000000 stemia-0.7.0/stemia/aretomo/batch_warp/aretomo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-08-04 15:11:18.000000 stemia-0.7.0/stemia/aretomo/batch_warp/fix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-08-04 15:11:18.000000 stemia-0.7.0/stemia/aretomo/batch_warp/fix_mdoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8816 2023-08-04 15:11:18.000000 stemia-0.7.0/stemia/aretomo/batch_warp/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4225 2023-08-04 15:11:18.000000 stemia-0.7.0/stemia/aretomo/batch_warp/parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-08-04 15:11:18.000000 stemia-0.7.0/stemia/aretomo/batch_warp/stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-08-04 15:11:18.000000 stemia-0.7.0/stemia/aretomo/batch_warp/threaded.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-08-04 15:11:18.000000 stemia-0.7.0/stemia/aretomo/batch_warp/topaz.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:11:36.929988 stemia-0.7.0/stemia/cryosparc/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-04 15:11:18.000000 stemia-0.7.0/stemia/cryosparc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:11:36.929988 stemia-0.7.0/stemia/cryosparc/csplot/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-04 15:11:18.000000 stemia-0.7.0/stemia/cryosparc/csplot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-08-04 15:11:18.000000 stemia-0.7.0/stemia/cryosparc/csplot/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6768 2023-08-04 15:11:18.000000 stemia-0.7.0/stemia/cryosparc/csplot/parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-08-04 15:11:18.000000 stemia-0.7.0/stemia/cryosparc/csplot/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-08-04 15:11:18.000000 stemia-0.7.0/stemia/cryosparc/fix_filament_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-08-04 15:11:18.000000 stemia-0.7.0/stemia/cryosparc/generate_tilt_angles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-08-04 15:11:18.000000 stemia-0.7.0/stemia/cryosparc/merge_defects_gainref.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:11:36.929988 stemia-0.7.0/stemia/image/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-08-04 15:11:18.000000 stemia-0.7.0/stemia/image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:11:36.929988 stemia-0.7.0/stemia/image/center_filament/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-04 15:11:18.000000 stemia-0.7.0/stemia/image/center_filament/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2696 2023-08-04 15:11:18.000000 stemia-0.7.0/stemia/image/center_filament/center_filament.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-08-04 15:11:18.000000 stemia-0.7.0/stemia/image/center_filament/funcs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3103 2023-08-04 15:11:18.000000 stemia-0.7.0/stemia/image/classify_densities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-08-04 15:11:18.000000 stemia-0.7.0/stemia/image/create_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-08-04 15:11:18.000000 stemia-0.7.0/stemia/image/extract_z_snapshots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-08-04 15:11:18.000000 stemia-0.7.0/stemia/image/flip_z.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-08-04 15:11:18.000000 stemia-0.7.0/stemia/image/fourier_crop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-08-04 15:11:18.000000 stemia-0.7.0/stemia/image/rescale.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:11:36.929988 stemia-0.7.0/stemia/imod/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-08-04 15:11:18.000000 stemia-0.7.0/stemia/imod/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-08-04 15:11:18.000000 stemia-0.7.0/stemia/imod/find_NAD_params.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:11:36.929988 stemia-0.7.0/stemia/relion/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-08-04 15:11:18.000000 stemia-0.7.0/stemia/relion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-08-04 15:11:18.000000 stemia-0.7.0/stemia/relion/align_filament_particles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:11:36.933989 stemia-0.7.0/stemia/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 15:11:18.000000 stemia-0.7.0/stemia/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3236 2023-08-04 15:11:18.000000 stemia-0.7.0/stemia/utils/click.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-08-04 15:11:18.000000 stemia-0.7.0/stemia/utils/image_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-08-04 15:11:18.000000 stemia-0.7.0/stemia/utils/io_.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:11:36.933989 stemia-0.7.0/stemia/warp/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-08-04 15:11:18.000000 stemia-0.7.0/stemia/warp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-08-04 15:11:18.000000 stemia-0.7.0/stemia/warp/fix_mdoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-08-04 15:11:18.000000 stemia-0.7.0/stemia/warp/offset_angle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-08-04 15:11:18.000000 stemia-0.7.0/stemia/warp/parse_xml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-08-04 15:11:18.000000 stemia-0.7.0/stemia/warp/prepare_isonet.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1252 2023-08-04 15:11:18.000000 stemia-0.7.0/stemia/warp/preprocess_serialem.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-08-04 15:11:18.000000 stemia-0.7.0/stemia/warp/spoof_mdoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-08-04 15:11:18.000000 stemia-0.7.0/stemia/warp/summarize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:11:36.929988 stemia-0.7.0/stemia.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13839 2023-08-04 15:11:36.000000 stemia-0.7.0/stemia.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-08-04 15:11:36.000000 stemia-0.7.0/stemia.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 15:11:36.000000 stemia-0.7.0/stemia.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 15:11:36.000000 stemia-0.7.0/stemia.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 15:11:36.000000 stemia-0.7.0/stemia.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-08-04 15:11:36.000000 stemia-0.7.0/stemia.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-04 15:11:36.000000 stemia-0.7.0/stemia.egg-info/top_level.txt
```

### Comparing `stemia-0.6.4/.github/workflows/deploy.yml` & `stemia-0.7.0/.github/workflows/deploy.yml`

 * *Files identical despite different names*

### Comparing `stemia-0.6.4/LICENSE` & `stemia-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `stemia-0.6.4/PKG-INFO` & `stemia-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stemia
-Version: 0.6.4
+Version: 0.7.0
 Summary: Scripts and Tools for Electron Microscopy Analysis.
 Home-page: https://github.com/brisvag/stemia/
 Author: Lorenzo Gaifas
 Author-email: brisvag@gmail.com
 License: GNU General Public License v3 (GPLv3)
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `stemia-0.6.4/README.md` & `stemia-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `stemia-0.6.4/docs/generate_readme.py` & `stemia-0.7.0/docs/generate_readme.py`

 * *Files identical despite different names*

### Comparing `stemia-0.6.4/setup.cfg` & `stemia-0.7.0/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 	mdocfile
 	rich
 	topaz-em
 	tabulate
 	cryohub
 	napari
 	sh
+	matplotlib
 
 [options.entry_points]
 console_scripts = 
 	stemia = stemia:cli
 
 [options.package_data]
 * = *.txt, *.md
```

### Comparing `stemia-0.6.4/stemia/aretomo/aln2xf.py` & `stemia-0.7.0/stemia/aretomo/aln2xf.py`

 * *Files identical despite different names*

### Comparing `stemia-0.6.4/stemia/aretomo/batch_warp/aretomo.py` & `stemia-0.7.0/stemia/aretomo/batch_warp/aretomo.py`

 * *Files identical despite different names*

### Comparing `stemia-0.6.4/stemia/aretomo/batch_warp/fix.py` & `stemia-0.7.0/stemia/aretomo/batch_warp/fix.py`

 * *Files identical despite different names*

### Comparing `stemia-0.6.4/stemia/aretomo/batch_warp/fix_mdoc.py` & `stemia-0.7.0/stemia/aretomo/batch_warp/fix_mdoc.py`

 * *Files identical despite different names*

### Comparing `stemia-0.6.4/stemia/aretomo/batch_warp/main.py` & `stemia-0.7.0/stemia/aretomo/batch_warp/main.py`

 * *Files identical despite different names*

### Comparing `stemia-0.6.4/stemia/aretomo/batch_warp/parse.py` & `stemia-0.7.0/stemia/aretomo/batch_warp/parse.py`

 * *Files identical despite different names*

### Comparing `stemia-0.6.4/stemia/aretomo/batch_warp/stack.py` & `stemia-0.7.0/stemia/aretomo/batch_warp/stack.py`

 * *Files identical despite different names*

### Comparing `stemia-0.6.4/stemia/aretomo/batch_warp/threaded.py` & `stemia-0.7.0/stemia/aretomo/batch_warp/threaded.py`

 * *Files identical despite different names*

### Comparing `stemia-0.6.4/stemia/aretomo/batch_warp/topaz.py` & `stemia-0.7.0/stemia/aretomo/batch_warp/topaz.py`

 * *Files identical despite different names*

### Comparing `stemia-0.6.4/stemia/cryosparc/csplot/main.py` & `stemia-0.7.0/stemia/cryosparc/csplot/main.py`

 * *Files identical despite different names*

### Comparing `stemia-0.6.4/stemia/cryosparc/csplot/parse.py` & `stemia-0.7.0/stemia/cryosparc/csplot/parse.py`

 * *Files identical despite different names*

### Comparing `stemia-0.6.4/stemia/cryosparc/csplot/plot.py` & `stemia-0.7.0/stemia/cryosparc/csplot/plot.py`

 * *Files identical despite different names*

### Comparing `stemia-0.6.4/stemia/cryosparc/fix_filament_ids.py` & `stemia-0.7.0/stemia/cryosparc/fix_filament_ids.py`

 * *Files identical despite different names*

### Comparing `stemia-0.6.4/stemia/cryosparc/generate_tilt_angles.py` & `stemia-0.7.0/stemia/cryosparc/generate_tilt_angles.py`

 * *Files identical despite different names*

### Comparing `stemia-0.6.4/stemia/cryosparc/merge_defects_gainref.py` & `stemia-0.7.0/stemia/cryosparc/merge_defects_gainref.py`

 * *Files identical despite different names*

### Comparing `stemia-0.6.4/stemia/image/center_filament/center_filament.py` & `stemia-0.7.0/stemia/image/center_filament/center_filament.py`

 * *Files identical despite different names*

### Comparing `stemia-0.6.4/stemia/image/center_filament/funcs.py` & `stemia-0.7.0/stemia/image/center_filament/funcs.py`

 * *Files identical despite different names*

### Comparing `stemia-0.6.4/stemia/image/create_mask.py` & `stemia-0.7.0/stemia/image/create_mask.py`

 * *Files 22% similar despite different names*

```diff
@@ -27,53 +27,13 @@
         raise click.UsageError(f'{output} exists but "-f" flag was not passed')
 
     with mrcfile.open(input, header_only=True, permissive=True) as mrc:
         cell = mrc.header.cella
         shape = mrc.header[['nx', 'ny', 'nz']].item()
         px_size = mrc.voxel_size.item()[0]
 
-    if center is None:
-        center = np.array(shape) / 2
     if ang:
         radius *= px_size
         padding *= px_size
 
-    indices = np.stack(
-        np.meshgrid(
-            np.arange(0, shape[0]),
-            np.arange(0, shape[1]),
-            np.arange(0, shape[2]),
-            indexing='ij'
-        ),
-        axis=-1
-    ) + 0.5
-
-    if mask_type == 'sphere':
-        dists = np.linalg.norm(indices - center, axis=-1)
-    elif mask_type == 'cylinder':
-        line = np.full((shape[axis], 3), center)
-        line[:, axis] = np.arange(shape[axis])
-        new_shape = [1 for _ in shape] + [3]
-        new_shape[axis] = -1
-        line = line.reshape(new_shape)
-        dists = np.linalg.norm(indices - line, axis=-1)
-    elif mask_type == 'threshold':
-        import edt
-        with mrcfile.open(input, permissive=True) as mrc:
-            data = mrc.data
-        binarized = data > threshold
-        dists = -edt.sdf(binarized)
-
-    def smoothstep_normalized(arr, min_val, max_val):
-        rng = max_val - min_val
-        normalized = (arr - min_val) / rng
-        smooth = np.where(normalized < 0, 0, np.where(normalized <= 1, 3 * normalized**2 - 2 * normalized**3, 1))
-        return 1 - smooth
-
-    mask = smoothstep_normalized(dists, radius, radius + padding)
-
-    if inner_radius is not None:
-        inner_mask = smoothstep_normalized(dists, inner_radius, inner_radius + padding)
-        mask -= inner_mask
-
     with mrcfile.new(output, mask.astype(np.float32), overwrite=overwrite) as mrc:
         mrc.header.cella = cell
```

### Comparing `stemia-0.6.4/stemia/image/extract_z_snapshots.py` & `stemia-0.7.0/stemia/image/extract_z_snapshots.py`

 * *Files identical despite different names*

### Comparing `stemia-0.6.4/stemia/image/flip_z.py` & `stemia-0.7.0/stemia/image/flip_z.py`

 * *Files identical despite different names*

### Comparing `stemia-0.6.4/stemia/image/fourier_crop.py` & `stemia-0.7.0/stemia/image/fourier_crop.py`

 * *Files identical despite different names*

### Comparing `stemia-0.6.4/stemia/image/rescale.py` & `stemia-0.7.0/stemia/image/rescale.py`

 * *Files identical despite different names*

### Comparing `stemia-0.6.4/stemia/imod/find_NAD_params.py` & `stemia-0.7.0/stemia/imod/find_NAD_params.py`

 * *Files identical despite different names*

### Comparing `stemia-0.6.4/stemia/relion/align_filament_particles.py` & `stemia-0.7.0/stemia/relion/align_filament_particles.py`

 * *Files identical despite different names*

### Comparing `stemia-0.6.4/stemia/utils/click.py` & `stemia-0.7.0/stemia/utils/click.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import subprocess
 import pkgutil
 import importlib
 from pathlib import Path
+from rich import print
 
 import click
 
 
 def make_command(file):
     """
     Generate a click command from a simple shell script.
@@ -60,25 +61,45 @@
     has_subcommands = False
     # loop through all the submodules
     for loader, name, is_pkg in pkgutil.walk_packages([str(source)]):
         full_name = base_package + '.' + name
         module = importlib.import_module(full_name)
         # get the cli if it exists
         if hasattr(module, 'cli'):
+            module.cli.name = name
             cli.add_command(module.cli, name=name)
             has_subcommands = True
         # go deeper if needed
         elif is_pkg:
             def subcli():
                 pass
             subcli.__doc__ = module.__doc__
             subcli = click.group()(subcli)
             has_subcommands = add_subcommands(subcli, source / name, full_name)
             if has_subcommands:
+                subcli.name = name
                 cli.add_command(subcli, name=name)
 
     # add shell scripts
     for file in source.glob('*.sh'):
-        cli.add_command(make_command(file), name=file.stem)
+        subcli = make_command(file)
+        subcli.name = file.stem
+        cli.add_command(subcli, name=file.stem)
         has_subcommands = True
 
     return has_subcommands
+
+
+def print_command_tree(cli, prefix='', last=True):
+    # top of three, put a dot
+    if not prefix:
+        print(f'.[bold]{cli.name}[/]')
+    subs = getattr(cli, 'commands', {})
+    for i, sub in enumerate(subs.values()):
+        last_sub = len(subs) - i == 1
+        end_prefix = '└──' if last_sub else '├──'
+        print(
+            f'[white]{prefix + end_prefix} [/][bold]{sub.name}[/]:  '
+            f'[italic white]{(sub.__doc__ or "-").strip().splitlines()[0]}[/]'
+        )
+        sub_prefix = '    ' if last_sub else '│   '
+        print_command_tree(sub, prefix=prefix + sub_prefix, last=last_sub)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `stemia-0.6.4/stemia/utils/io_.py` & `stemia-0.7.0/stemia/utils/io_.py`

 * *Files identical despite different names*

### Comparing `stemia-0.6.4/stemia/warp/fix_mdoc.py` & `stemia-0.7.0/stemia/warp/fix_mdoc.py`

 * *Files identical despite different names*

### Comparing `stemia-0.6.4/stemia/warp/offset_angle.py` & `stemia-0.7.0/stemia/warp/offset_angle.py`

 * *Files identical despite different names*

### Comparing `stemia-0.6.4/stemia/warp/prepare_isonet.py` & `stemia-0.7.0/stemia/warp/prepare_isonet.py`

 * *Files identical despite different names*

### Comparing `stemia-0.6.4/stemia/warp/preprocess_serialem.sh` & `stemia-0.7.0/stemia/warp/preprocess_serialem.sh`

 * *Files identical despite different names*

### Comparing `stemia-0.6.4/stemia/warp/spoof_mdoc.py` & `stemia-0.7.0/stemia/warp/spoof_mdoc.py`

 * *Files identical despite different names*

### Comparing `stemia-0.6.4/stemia/warp/summarize.py` & `stemia-0.7.0/stemia/warp/summarize.py`

 * *Files identical despite different names*

### Comparing `stemia-0.6.4/stemia.egg-info/PKG-INFO` & `stemia-0.7.0/stemia.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stemia
-Version: 0.6.4
+Version: 0.7.0
 Summary: Scripts and Tools for Electron Microscopy Analysis.
 Home-page: https://github.com/brisvag/stemia/
 Author: Lorenzo Gaifas
 Author-email: brisvag@gmail.com
 License: GNU General Public License v3 (GPLv3)
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `stemia-0.6.4/stemia.egg-info/SOURCES.txt` & `stemia-0.7.0/stemia.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 stemia/cryosparc/generate_tilt_angles.py
 stemia/cryosparc/merge_defects_gainref.py
 stemia/cryosparc/csplot/__init__.py
 stemia/cryosparc/csplot/main.py
 stemia/cryosparc/csplot/parse.py
 stemia/cryosparc/csplot/plot.py
 stemia/image/__init__.py
+stemia/image/classify_densities.py
 stemia/image/create_mask.py
 stemia/image/extract_z_snapshots.py
 stemia/image/flip_z.py
 stemia/image/fourier_crop.py
 stemia/image/rescale.py
 stemia/image/center_filament/__init__.py
 stemia/image/center_filament/center_filament.py
```

