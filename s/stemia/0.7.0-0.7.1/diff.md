# Comparing `tmp/stemia-0.7.0.tar.gz` & `tmp/stemia-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stemia-0.7.0.tar", last modified: Fri Aug  4 15:11:36 2023, max compression
+gzip compressed data, was "stemia-0.7.1.tar", last modified: Fri Aug  4 15:26:35 2023, max compression
```

## Comparing `stemia-0.7.0.tar` & `stemia-0.7.1.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:11:36.933989 stemia-0.7.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:11:36.925989 stemia-0.7.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:11:36.925989 stemia-0.7.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-08-04 15:11:18.000000 stemia-0.7.0/.github/workflows/deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-04 15:11:18.000000 stemia-0.7.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-08-04 15:11:18.000000 stemia-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13839 2023-08-04 15:11:36.933989 stemia-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13350 2023-08-04 15:11:18.000000 stemia-0.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:11:36.925989 stemia-0.7.0/docs/
--rwxr-xr-x   0 runner    (1001) docker     (123)      568 2023-08-04 15:11:18.000000 stemia-0.7.0/docs/generate_readme.py
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-08-04 15:11:18.000000 stemia-0.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-08-04 15:11:36.933989 stemia-0.7.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:11:36.925989 stemia-0.7.0/stemia/
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-08-04 15:11:18.000000 stemia-0.7.0/stemia/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-08-04 15:11:36.000000 stemia-0.7.0/stemia/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:11:36.929988 stemia-0.7.0/stemia/aretomo/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-04 15:11:18.000000 stemia-0.7.0/stemia/aretomo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-08-04 15:11:18.000000 stemia-0.7.0/stemia/aretomo/aln2xf.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      343 2023-08-04 15:11:18.000000 stemia-0.7.0/stemia/aretomo/batch.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:11:36.929988 stemia-0.7.0/stemia/aretomo/batch_warp/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-04 15:11:18.000000 stemia-0.7.0/stemia/aretomo/batch_warp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4743 2023-08-04 15:11:18.000000 stemia-0.7.0/stemia/aretomo/batch_warp/aretomo.py
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-08-04 15:11:18.000000 stemia-0.7.0/stemia/aretomo/batch_warp/fix.py
--rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-08-04 15:11:18.000000 stemia-0.7.0/stemia/aretomo/batch_warp/fix_mdoc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8816 2023-08-04 15:11:18.000000 stemia-0.7.0/stemia/aretomo/batch_warp/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     4225 2023-08-04 15:11:18.000000 stemia-0.7.0/stemia/aretomo/batch_warp/parse.py
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-08-04 15:11:18.000000 stemia-0.7.0/stemia/aretomo/batch_warp/stack.py
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-08-04 15:11:18.000000 stemia-0.7.0/stemia/aretomo/batch_warp/threaded.py
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-08-04 15:11:18.000000 stemia-0.7.0/stemia/aretomo/batch_warp/topaz.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:11:36.929988 stemia-0.7.0/stemia/cryosparc/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-04 15:11:18.000000 stemia-0.7.0/stemia/cryosparc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:11:36.929988 stemia-0.7.0/stemia/cryosparc/csplot/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-04 15:11:18.000000 stemia-0.7.0/stemia/cryosparc/csplot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-08-04 15:11:18.000000 stemia-0.7.0/stemia/cryosparc/csplot/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     6768 2023-08-04 15:11:18.000000 stemia-0.7.0/stemia/cryosparc/csplot/parse.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-08-04 15:11:18.000000 stemia-0.7.0/stemia/cryosparc/csplot/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-08-04 15:11:18.000000 stemia-0.7.0/stemia/cryosparc/fix_filament_ids.py
--rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-08-04 15:11:18.000000 stemia-0.7.0/stemia/cryosparc/generate_tilt_angles.py
--rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-08-04 15:11:18.000000 stemia-0.7.0/stemia/cryosparc/merge_defects_gainref.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:11:36.929988 stemia-0.7.0/stemia/image/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-08-04 15:11:18.000000 stemia-0.7.0/stemia/image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:11:36.929988 stemia-0.7.0/stemia/image/center_filament/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-04 15:11:18.000000 stemia-0.7.0/stemia/image/center_filament/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2696 2023-08-04 15:11:18.000000 stemia-0.7.0/stemia/image/center_filament/center_filament.py
--rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-08-04 15:11:18.000000 stemia-0.7.0/stemia/image/center_filament/funcs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3103 2023-08-04 15:11:18.000000 stemia-0.7.0/stemia/image/classify_densities.py
--rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-08-04 15:11:18.000000 stemia-0.7.0/stemia/image/create_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-08-04 15:11:18.000000 stemia-0.7.0/stemia/image/extract_z_snapshots.py
--rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-08-04 15:11:18.000000 stemia-0.7.0/stemia/image/flip_z.py
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-08-04 15:11:18.000000 stemia-0.7.0/stemia/image/fourier_crop.py
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-08-04 15:11:18.000000 stemia-0.7.0/stemia/image/rescale.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:11:36.929988 stemia-0.7.0/stemia/imod/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-08-04 15:11:18.000000 stemia-0.7.0/stemia/imod/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-08-04 15:11:18.000000 stemia-0.7.0/stemia/imod/find_NAD_params.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:11:36.929988 stemia-0.7.0/stemia/relion/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-08-04 15:11:18.000000 stemia-0.7.0/stemia/relion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-08-04 15:11:18.000000 stemia-0.7.0/stemia/relion/align_filament_particles.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:11:36.933989 stemia-0.7.0/stemia/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 15:11:18.000000 stemia-0.7.0/stemia/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3236 2023-08-04 15:11:18.000000 stemia-0.7.0/stemia/utils/click.py
--rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-08-04 15:11:18.000000 stemia-0.7.0/stemia/utils/image_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-08-04 15:11:18.000000 stemia-0.7.0/stemia/utils/io_.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:11:36.933989 stemia-0.7.0/stemia/warp/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-08-04 15:11:18.000000 stemia-0.7.0/stemia/warp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-08-04 15:11:18.000000 stemia-0.7.0/stemia/warp/fix_mdoc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-08-04 15:11:18.000000 stemia-0.7.0/stemia/warp/offset_angle.py
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-08-04 15:11:18.000000 stemia-0.7.0/stemia/warp/parse_xml.py
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-08-04 15:11:18.000000 stemia-0.7.0/stemia/warp/prepare_isonet.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1252 2023-08-04 15:11:18.000000 stemia-0.7.0/stemia/warp/preprocess_serialem.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-08-04 15:11:18.000000 stemia-0.7.0/stemia/warp/spoof_mdoc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-08-04 15:11:18.000000 stemia-0.7.0/stemia/warp/summarize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:11:36.929988 stemia-0.7.0/stemia.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13839 2023-08-04 15:11:36.000000 stemia-0.7.0/stemia.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-08-04 15:11:36.000000 stemia-0.7.0/stemia.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 15:11:36.000000 stemia-0.7.0/stemia.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 15:11:36.000000 stemia-0.7.0/stemia.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 15:11:36.000000 stemia-0.7.0/stemia.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-08-04 15:11:36.000000 stemia-0.7.0/stemia.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-04 15:11:36.000000 stemia-0.7.0/stemia.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:26:35.681819 stemia-0.7.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:26:35.673819 stemia-0.7.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:26:35.673819 stemia-0.7.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-08-04 15:26:18.000000 stemia-0.7.1/.github/workflows/deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-04 15:26:18.000000 stemia-0.7.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-08-04 15:26:18.000000 stemia-0.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13839 2023-08-04 15:26:35.681819 stemia-0.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13350 2023-08-04 15:26:18.000000 stemia-0.7.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:26:35.673819 stemia-0.7.1/docs/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      568 2023-08-04 15:26:18.000000 stemia-0.7.1/docs/generate_readme.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-08-04 15:26:18.000000 stemia-0.7.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-08-04 15:26:35.681819 stemia-0.7.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:26:35.673819 stemia-0.7.1/stemia/
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-08-04 15:26:18.000000 stemia-0.7.1/stemia/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-08-04 15:26:35.000000 stemia-0.7.1/stemia/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:26:35.677819 stemia-0.7.1/stemia/aretomo/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-04 15:26:18.000000 stemia-0.7.1/stemia/aretomo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-08-04 15:26:18.000000 stemia-0.7.1/stemia/aretomo/aln2xf.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      343 2023-08-04 15:26:18.000000 stemia-0.7.1/stemia/aretomo/batch.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:26:35.677819 stemia-0.7.1/stemia/aretomo/batch_warp/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-04 15:26:18.000000 stemia-0.7.1/stemia/aretomo/batch_warp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4743 2023-08-04 15:26:18.000000 stemia-0.7.1/stemia/aretomo/batch_warp/aretomo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-08-04 15:26:18.000000 stemia-0.7.1/stemia/aretomo/batch_warp/fix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-08-04 15:26:18.000000 stemia-0.7.1/stemia/aretomo/batch_warp/fix_mdoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8816 2023-08-04 15:26:18.000000 stemia-0.7.1/stemia/aretomo/batch_warp/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4225 2023-08-04 15:26:18.000000 stemia-0.7.1/stemia/aretomo/batch_warp/parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-08-04 15:26:18.000000 stemia-0.7.1/stemia/aretomo/batch_warp/stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-08-04 15:26:18.000000 stemia-0.7.1/stemia/aretomo/batch_warp/threaded.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-08-04 15:26:18.000000 stemia-0.7.1/stemia/aretomo/batch_warp/topaz.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:26:35.677819 stemia-0.7.1/stemia/cryosparc/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-04 15:26:18.000000 stemia-0.7.1/stemia/cryosparc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:26:35.677819 stemia-0.7.1/stemia/cryosparc/csplot/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-04 15:26:18.000000 stemia-0.7.1/stemia/cryosparc/csplot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-08-04 15:26:18.000000 stemia-0.7.1/stemia/cryosparc/csplot/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6768 2023-08-04 15:26:18.000000 stemia-0.7.1/stemia/cryosparc/csplot/parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-08-04 15:26:18.000000 stemia-0.7.1/stemia/cryosparc/csplot/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-08-04 15:26:18.000000 stemia-0.7.1/stemia/cryosparc/fix_filament_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-08-04 15:26:18.000000 stemia-0.7.1/stemia/cryosparc/generate_tilt_angles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-08-04 15:26:18.000000 stemia-0.7.1/stemia/cryosparc/merge_defects_gainref.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:26:35.677819 stemia-0.7.1/stemia/image/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-08-04 15:26:18.000000 stemia-0.7.1/stemia/image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:26:35.677819 stemia-0.7.1/stemia/image/center_filament/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-04 15:26:18.000000 stemia-0.7.1/stemia/image/center_filament/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2696 2023-08-04 15:26:18.000000 stemia-0.7.1/stemia/image/center_filament/center_filament.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-08-04 15:26:18.000000 stemia-0.7.1/stemia/image/center_filament/funcs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3164 2023-08-04 15:26:18.000000 stemia-0.7.1/stemia/image/classify_densities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-08-04 15:26:18.000000 stemia-0.7.1/stemia/image/create_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-08-04 15:26:18.000000 stemia-0.7.1/stemia/image/extract_z_snapshots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-08-04 15:26:18.000000 stemia-0.7.1/stemia/image/flip_z.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-08-04 15:26:18.000000 stemia-0.7.1/stemia/image/fourier_crop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-08-04 15:26:18.000000 stemia-0.7.1/stemia/image/rescale.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:26:35.677819 stemia-0.7.1/stemia/imod/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-08-04 15:26:18.000000 stemia-0.7.1/stemia/imod/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-08-04 15:26:18.000000 stemia-0.7.1/stemia/imod/find_NAD_params.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:26:35.677819 stemia-0.7.1/stemia/relion/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-08-04 15:26:18.000000 stemia-0.7.1/stemia/relion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-08-04 15:26:18.000000 stemia-0.7.1/stemia/relion/align_filament_particles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:26:35.681819 stemia-0.7.1/stemia/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 15:26:18.000000 stemia-0.7.1/stemia/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3236 2023-08-04 15:26:18.000000 stemia-0.7.1/stemia/utils/click.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-08-04 15:26:18.000000 stemia-0.7.1/stemia/utils/image_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-08-04 15:26:18.000000 stemia-0.7.1/stemia/utils/io_.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:26:35.681819 stemia-0.7.1/stemia/warp/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-08-04 15:26:18.000000 stemia-0.7.1/stemia/warp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-08-04 15:26:18.000000 stemia-0.7.1/stemia/warp/fix_mdoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-08-04 15:26:18.000000 stemia-0.7.1/stemia/warp/offset_angle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-08-04 15:26:18.000000 stemia-0.7.1/stemia/warp/parse_xml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-08-04 15:26:18.000000 stemia-0.7.1/stemia/warp/prepare_isonet.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1252 2023-08-04 15:26:18.000000 stemia-0.7.1/stemia/warp/preprocess_serialem.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-08-04 15:26:18.000000 stemia-0.7.1/stemia/warp/spoof_mdoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-08-04 15:26:18.000000 stemia-0.7.1/stemia/warp/summarize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:26:35.673819 stemia-0.7.1/stemia.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13839 2023-08-04 15:26:35.000000 stemia-0.7.1/stemia.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-08-04 15:26:35.000000 stemia-0.7.1/stemia.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 15:26:35.000000 stemia-0.7.1/stemia.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 15:26:35.000000 stemia-0.7.1/stemia.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 15:26:35.000000 stemia-0.7.1/stemia.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-08-04 15:26:35.000000 stemia-0.7.1/stemia.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-04 15:26:35.000000 stemia-0.7.1/stemia.egg-info/top_level.txt
```

### Comparing `stemia-0.7.0/.github/workflows/deploy.yml` & `stemia-0.7.1/.github/workflows/deploy.yml`

 * *Files identical despite different names*

### Comparing `stemia-0.7.0/LICENSE` & `stemia-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `stemia-0.7.0/PKG-INFO` & `stemia-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stemia
-Version: 0.7.0
+Version: 0.7.1
 Summary: Scripts and Tools for Electron Microscopy Analysis.
 Home-page: https://github.com/brisvag/stemia/
 Author: Lorenzo Gaifas
 Author-email: brisvag@gmail.com
 License: GNU General Public License v3 (GPLv3)
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `stemia-0.7.0/README.md` & `stemia-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `stemia-0.7.0/docs/generate_readme.py` & `stemia-0.7.1/docs/generate_readme.py`

 * *Files identical despite different names*

### Comparing `stemia-0.7.0/setup.cfg` & `stemia-0.7.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `stemia-0.7.0/stemia/__init__.py` & `stemia-0.7.1/stemia/__init__.py`

 * *Files identical despite different names*

### Comparing `stemia-0.7.0/stemia/aretomo/aln2xf.py` & `stemia-0.7.1/stemia/aretomo/aln2xf.py`

 * *Files identical despite different names*

### Comparing `stemia-0.7.0/stemia/aretomo/batch_warp/aretomo.py` & `stemia-0.7.1/stemia/aretomo/batch_warp/aretomo.py`

 * *Files identical despite different names*

### Comparing `stemia-0.7.0/stemia/aretomo/batch_warp/fix.py` & `stemia-0.7.1/stemia/aretomo/batch_warp/fix.py`

 * *Files identical despite different names*

### Comparing `stemia-0.7.0/stemia/aretomo/batch_warp/fix_mdoc.py` & `stemia-0.7.1/stemia/aretomo/batch_warp/fix_mdoc.py`

 * *Files identical despite different names*

### Comparing `stemia-0.7.0/stemia/aretomo/batch_warp/main.py` & `stemia-0.7.1/stemia/aretomo/batch_warp/main.py`

 * *Files identical despite different names*

### Comparing `stemia-0.7.0/stemia/aretomo/batch_warp/parse.py` & `stemia-0.7.1/stemia/aretomo/batch_warp/parse.py`

 * *Files identical despite different names*

### Comparing `stemia-0.7.0/stemia/aretomo/batch_warp/stack.py` & `stemia-0.7.1/stemia/aretomo/batch_warp/stack.py`

 * *Files identical despite different names*

### Comparing `stemia-0.7.0/stemia/aretomo/batch_warp/threaded.py` & `stemia-0.7.1/stemia/aretomo/batch_warp/threaded.py`

 * *Files identical despite different names*

### Comparing `stemia-0.7.0/stemia/aretomo/batch_warp/topaz.py` & `stemia-0.7.1/stemia/aretomo/batch_warp/topaz.py`

 * *Files identical despite different names*

### Comparing `stemia-0.7.0/stemia/cryosparc/csplot/main.py` & `stemia-0.7.1/stemia/cryosparc/csplot/main.py`

 * *Files identical despite different names*

### Comparing `stemia-0.7.0/stemia/cryosparc/csplot/parse.py` & `stemia-0.7.1/stemia/cryosparc/csplot/parse.py`

 * *Files identical despite different names*

### Comparing `stemia-0.7.0/stemia/cryosparc/csplot/plot.py` & `stemia-0.7.1/stemia/cryosparc/csplot/plot.py`

 * *Files identical despite different names*

### Comparing `stemia-0.7.0/stemia/cryosparc/fix_filament_ids.py` & `stemia-0.7.1/stemia/cryosparc/fix_filament_ids.py`

 * *Files identical despite different names*

### Comparing `stemia-0.7.0/stemia/cryosparc/generate_tilt_angles.py` & `stemia-0.7.1/stemia/cryosparc/generate_tilt_angles.py`

 * *Files identical despite different names*

### Comparing `stemia-0.7.0/stemia/cryosparc/merge_defects_gainref.py` & `stemia-0.7.1/stemia/cryosparc/merge_defects_gainref.py`

 * *Files identical despite different names*

### Comparing `stemia-0.7.0/stemia/image/center_filament/center_filament.py` & `stemia-0.7.1/stemia/image/center_filament/center_filament.py`

 * *Files identical despite different names*

### Comparing `stemia-0.7.0/stemia/image/center_filament/funcs.py` & `stemia-0.7.1/stemia/image/center_filament/funcs.py`

 * *Files identical despite different names*

### Comparing `stemia-0.7.0/stemia/image/classify_densities.py` & `stemia-0.7.1/stemia/image/classify_densities.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         padding=radius * 0.8,
     )
 
     field_squared = dist_field**2
 
     images = {}
 
-    print('Running with {max_classes} classes.')
+    print(f'Running with {max_classes} classes.')
 
     df = pd.DataFrame(columns=['total_density', 'radius_of_gyration'])
     df.index.name = 'image'
     with Progress() as progress:
         for st in progress.track(stacks, description='Reading data...'):
             data = mrcfile.read(st)
             images[Path(st).stem] = data
@@ -75,15 +75,16 @@
         df['name'] = df.index
 
         fig = px.scatter(df, x='total_density', y='radius_of_gyration', color='class', hover_name='name')
         fig.show()
         progress.update(proc_task, advance=1)
 
         for cl, df_cl in progress.track(df.groupby('class'), description='Splitting classes...'):
-            stacked = []
+            stacked = {}
             for img in df_cl.index:
                 *img_name, idx = img.split('_')
                 img_name = '_'.join(img_name)
                 idx = int(idx)
-                stacked.append(images[img_name][idx])
-            mrc = mrcfile.new(f'{img_name}_class_{cl:04}.mrc', np.stack(stacked), overwrite=True)
-            mrc.close()
+                stacked[img_name] = images[img_name][idx]
+            for img_name, data in stacked.items():
+                mrc = mrcfile.new(f'{img_name}_class_{cl:04}.mrc', np.stack(data), overwrite=True)
+                mrc.close()
```

### Comparing `stemia-0.7.0/stemia/image/create_mask.py` & `stemia-0.7.1/stemia/image/create_mask.py`

 * *Files identical despite different names*

### Comparing `stemia-0.7.0/stemia/image/extract_z_snapshots.py` & `stemia-0.7.1/stemia/image/extract_z_snapshots.py`

 * *Files identical despite different names*

### Comparing `stemia-0.7.0/stemia/image/flip_z.py` & `stemia-0.7.1/stemia/image/flip_z.py`

 * *Files identical despite different names*

### Comparing `stemia-0.7.0/stemia/image/fourier_crop.py` & `stemia-0.7.1/stemia/image/fourier_crop.py`

 * *Files identical despite different names*

### Comparing `stemia-0.7.0/stemia/image/rescale.py` & `stemia-0.7.1/stemia/image/rescale.py`

 * *Files identical despite different names*

### Comparing `stemia-0.7.0/stemia/imod/find_NAD_params.py` & `stemia-0.7.1/stemia/imod/find_NAD_params.py`

 * *Files identical despite different names*

### Comparing `stemia-0.7.0/stemia/relion/align_filament_particles.py` & `stemia-0.7.1/stemia/relion/align_filament_particles.py`

 * *Files identical despite different names*

### Comparing `stemia-0.7.0/stemia/utils/click.py` & `stemia-0.7.1/stemia/utils/click.py`

 * *Files identical despite different names*

### Comparing `stemia-0.7.0/stemia/utils/image_processing.py` & `stemia-0.7.1/stemia/utils/image_processing.py`

 * *Files identical despite different names*

### Comparing `stemia-0.7.0/stemia/utils/io_.py` & `stemia-0.7.1/stemia/utils/io_.py`

 * *Files identical despite different names*

### Comparing `stemia-0.7.0/stemia/warp/fix_mdoc.py` & `stemia-0.7.1/stemia/warp/fix_mdoc.py`

 * *Files identical despite different names*

### Comparing `stemia-0.7.0/stemia/warp/offset_angle.py` & `stemia-0.7.1/stemia/warp/offset_angle.py`

 * *Files identical despite different names*

### Comparing `stemia-0.7.0/stemia/warp/prepare_isonet.py` & `stemia-0.7.1/stemia/warp/prepare_isonet.py`

 * *Files identical despite different names*

### Comparing `stemia-0.7.0/stemia/warp/preprocess_serialem.sh` & `stemia-0.7.1/stemia/warp/preprocess_serialem.sh`

 * *Files identical despite different names*

### Comparing `stemia-0.7.0/stemia/warp/spoof_mdoc.py` & `stemia-0.7.1/stemia/warp/spoof_mdoc.py`

 * *Files identical despite different names*

### Comparing `stemia-0.7.0/stemia/warp/summarize.py` & `stemia-0.7.1/stemia/warp/summarize.py`

 * *Files identical despite different names*

### Comparing `stemia-0.7.0/stemia.egg-info/PKG-INFO` & `stemia-0.7.1/stemia.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stemia
-Version: 0.7.0
+Version: 0.7.1
 Summary: Scripts and Tools for Electron Microscopy Analysis.
 Home-page: https://github.com/brisvag/stemia/
 Author: Lorenzo Gaifas
 Author-email: brisvag@gmail.com
 License: GNU General Public License v3 (GPLv3)
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `stemia-0.7.0/stemia.egg-info/SOURCES.txt` & `stemia-0.7.1/stemia.egg-info/SOURCES.txt`

 * *Files identical despite different names*

