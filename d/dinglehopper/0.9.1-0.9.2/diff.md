# Comparing `tmp/dinglehopper-0.9.1.tar.gz` & `tmp/dinglehopper-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dinglehopper-0.9.1.tar", last modified: Fri Aug  4 17:48:04 2023, max compression
+gzip compressed data, was "dinglehopper-0.9.2.tar", last modified: Fri Aug  4 18:37:50 2023, max compression
```

## Comparing `dinglehopper-0.9.1.tar` & `dinglehopper-0.9.2.tar`

### file list

```diff
@@ -1,58 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 17:48:04.905192 dinglehopper-0.9.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11337 2023-08-04 17:47:48.000000 dinglehopper-0.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6438 2023-08-04 17:48:04.905192 dinglehopper-0.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5495 2023-08-04 17:47:48.000000 dinglehopper-0.9.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-08-04 17:47:48.000000 dinglehopper-0.9.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-08-04 17:47:48.000000 dinglehopper-0.9.1/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-08-04 17:47:48.000000 dinglehopper-0.9.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 17:48:04.905192 dinglehopper-0.9.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 17:48:04.897191 dinglehopper-0.9.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 17:48:04.897191 dinglehopper-0.9.1/src/dinglehopper/
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-08-04 17:47:48.000000 dinglehopper-0.9.1/src/dinglehopper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-08-04 17:47:48.000000 dinglehopper-0.9.1/src/dinglehopper/align.py
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-08-04 17:47:48.000000 dinglehopper-0.9.1/src/dinglehopper/character_error_rate.py
--rw-r--r--   0 runner    (1001) docker     (123)     8411 2023-08-04 17:47:48.000000 dinglehopper-0.9.1/src/dinglehopper/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-08-04 17:47:48.000000 dinglehopper-0.9.1/src/dinglehopper/cli_extract.py
--rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-08-04 17:47:48.000000 dinglehopper-0.9.1/src/dinglehopper/cli_line_dirs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-08-04 17:47:48.000000 dinglehopper-0.9.1/src/dinglehopper/cli_summarize.py
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-04 17:47:48.000000 dinglehopper-0.9.1/src/dinglehopper/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-08-04 17:47:48.000000 dinglehopper-0.9.1/src/dinglehopper/edit_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     9888 2023-08-04 17:47:48.000000 dinglehopper-0.9.1/src/dinglehopper/extracted_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     6075 2023-08-04 17:47:48.000000 dinglehopper-0.9.1/src/dinglehopper/ocr_files.py
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-08-04 17:47:48.000000 dinglehopper-0.9.1/src/dinglehopper/ocrd-tool.json
--rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-08-04 17:47:48.000000 dinglehopper-0.9.1/src/dinglehopper/ocrd_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 17:48:04.901191 dinglehopper-0.9.1/src/dinglehopper/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-08-04 17:47:48.000000 dinglehopper-0.9.1/src/dinglehopper/templates/report.html.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-08-04 17:47:48.000000 dinglehopper-0.9.1/src/dinglehopper/templates/report.html.js
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-08-04 17:47:48.000000 dinglehopper-0.9.1/src/dinglehopper/templates/report.json.j2
--rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-08-04 17:47:48.000000 dinglehopper-0.9.1/src/dinglehopper/templates/summary.html.j2
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-08-04 17:47:48.000000 dinglehopper-0.9.1/src/dinglehopper/templates/summary.json.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 17:48:04.905192 dinglehopper-0.9.1/src/dinglehopper/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 17:47:48.000000 dinglehopper-0.9.1/src/dinglehopper/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4536 2023-08-04 17:47:48.000000 dinglehopper-0.9.1/src/dinglehopper/tests/extracted_text_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4865 2023-08-04 17:47:48.000000 dinglehopper-0.9.1/src/dinglehopper/tests/test_align.py
--rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-08-04 17:47:48.000000 dinglehopper-0.9.1/src/dinglehopper/tests/test_character_error_rate.py
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-08-04 17:47:48.000000 dinglehopper-0.9.1/src/dinglehopper/tests/test_edit_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-08-04 17:47:48.000000 dinglehopper-0.9.1/src/dinglehopper/tests/test_editops.py
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-08-04 17:47:48.000000 dinglehopper-0.9.1/src/dinglehopper/tests/test_integ_align.py
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-08-04 17:47:48.000000 dinglehopper-0.9.1/src/dinglehopper/tests/test_integ_bigger_texts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-08-04 17:47:48.000000 dinglehopper-0.9.1/src/dinglehopper/tests/test_integ_character_error_rate_ocr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-08-04 17:47:48.000000 dinglehopper-0.9.1/src/dinglehopper/tests/test_integ_cli_dir.py
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-08-04 17:47:48.000000 dinglehopper-0.9.1/src/dinglehopper/tests/test_integ_cli_valid_json.py
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-08-04 17:47:48.000000 dinglehopper-0.9.1/src/dinglehopper/tests/test_integ_differences.py
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-08-04 17:47:48.000000 dinglehopper-0.9.1/src/dinglehopper/tests/test_integ_edit_distance_ocr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-08-04 17:47:48.000000 dinglehopper-0.9.1/src/dinglehopper/tests/test_integ_ocrd_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-08-04 17:47:48.000000 dinglehopper-0.9.1/src/dinglehopper/tests/test_integ_summarize.py
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-08-04 17:47:48.000000 dinglehopper-0.9.1/src/dinglehopper/tests/test_integ_table_extraction.py
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-08-04 17:47:48.000000 dinglehopper-0.9.1/src/dinglehopper/tests/test_integ_word_error_rate_ocr.py
--rw-r--r--   0 runner    (1001) docker     (123)     6530 2023-08-04 17:47:48.000000 dinglehopper-0.9.1/src/dinglehopper/tests/test_ocr_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-08-04 17:47:48.000000 dinglehopper-0.9.1/src/dinglehopper/tests/test_word_error_rate.py
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-08-04 17:47:48.000000 dinglehopper-0.9.1/src/dinglehopper/tests/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-08-04 17:47:48.000000 dinglehopper-0.9.1/src/dinglehopper/word_error_rate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 17:48:04.901191 dinglehopper-0.9.1/src/dinglehopper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6438 2023-08-04 17:48:04.000000 dinglehopper-0.9.1/src/dinglehopper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-08-04 17:48:04.000000 dinglehopper-0.9.1/src/dinglehopper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 17:48:04.000000 dinglehopper-0.9.1/src/dinglehopper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-08-04 17:48:04.000000 dinglehopper-0.9.1/src/dinglehopper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-08-04 17:48:04.000000 dinglehopper-0.9.1/src/dinglehopper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-04 17:48:04.000000 dinglehopper-0.9.1/src/dinglehopper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:37:50.673294 dinglehopper-0.9.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11337 2023-08-04 18:37:33.000000 dinglehopper-0.9.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-08-04 18:37:33.000000 dinglehopper-0.9.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6438 2023-08-04 18:37:50.673294 dinglehopper-0.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5495 2023-08-04 18:37:33.000000 dinglehopper-0.9.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-08-04 18:37:33.000000 dinglehopper-0.9.2/ocrd-tool.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-08-04 18:37:33.000000 dinglehopper-0.9.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-08-04 18:37:33.000000 dinglehopper-0.9.2/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-08-04 18:37:33.000000 dinglehopper-0.9.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 18:37:50.673294 dinglehopper-0.9.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:37:50.661293 dinglehopper-0.9.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:37:50.665294 dinglehopper-0.9.2/src/dinglehopper/
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-08-04 18:37:33.000000 dinglehopper-0.9.2/src/dinglehopper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-08-04 18:37:33.000000 dinglehopper-0.9.2/src/dinglehopper/align.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-08-04 18:37:33.000000 dinglehopper-0.9.2/src/dinglehopper/character_error_rate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8411 2023-08-04 18:37:33.000000 dinglehopper-0.9.2/src/dinglehopper/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-08-04 18:37:33.000000 dinglehopper-0.9.2/src/dinglehopper/cli_extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-08-04 18:37:33.000000 dinglehopper-0.9.2/src/dinglehopper/cli_line_dirs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-08-04 18:37:33.000000 dinglehopper-0.9.2/src/dinglehopper/cli_summarize.py
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-04 18:37:33.000000 dinglehopper-0.9.2/src/dinglehopper/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-08-04 18:37:33.000000 dinglehopper-0.9.2/src/dinglehopper/edit_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9888 2023-08-04 18:37:33.000000 dinglehopper-0.9.2/src/dinglehopper/extracted_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6075 2023-08-04 18:37:33.000000 dinglehopper-0.9.2/src/dinglehopper/ocr_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-08-04 18:37:33.000000 dinglehopper-0.9.2/src/dinglehopper/ocrd-tool.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-08-04 18:37:33.000000 dinglehopper-0.9.2/src/dinglehopper/ocrd_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:37:50.665294 dinglehopper-0.9.2/src/dinglehopper/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-08-04 18:37:33.000000 dinglehopper-0.9.2/src/dinglehopper/templates/report.html.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-08-04 18:37:33.000000 dinglehopper-0.9.2/src/dinglehopper/templates/report.html.js
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-08-04 18:37:33.000000 dinglehopper-0.9.2/src/dinglehopper/templates/report.json.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-08-04 18:37:33.000000 dinglehopper-0.9.2/src/dinglehopper/templates/summary.html.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-08-04 18:37:33.000000 dinglehopper-0.9.2/src/dinglehopper/templates/summary.json.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:37:50.673294 dinglehopper-0.9.2/src/dinglehopper/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 18:37:33.000000 dinglehopper-0.9.2/src/dinglehopper/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4536 2023-08-04 18:37:33.000000 dinglehopper-0.9.2/src/dinglehopper/tests/extracted_text_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4865 2023-08-04 18:37:33.000000 dinglehopper-0.9.2/src/dinglehopper/tests/test_align.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-08-04 18:37:33.000000 dinglehopper-0.9.2/src/dinglehopper/tests/test_character_error_rate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-08-04 18:37:33.000000 dinglehopper-0.9.2/src/dinglehopper/tests/test_edit_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-08-04 18:37:33.000000 dinglehopper-0.9.2/src/dinglehopper/tests/test_editops.py
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-08-04 18:37:33.000000 dinglehopper-0.9.2/src/dinglehopper/tests/test_integ_align.py
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-08-04 18:37:33.000000 dinglehopper-0.9.2/src/dinglehopper/tests/test_integ_bigger_texts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-08-04 18:37:33.000000 dinglehopper-0.9.2/src/dinglehopper/tests/test_integ_character_error_rate_ocr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-08-04 18:37:33.000000 dinglehopper-0.9.2/src/dinglehopper/tests/test_integ_cli_dir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-08-04 18:37:33.000000 dinglehopper-0.9.2/src/dinglehopper/tests/test_integ_cli_valid_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-08-04 18:37:33.000000 dinglehopper-0.9.2/src/dinglehopper/tests/test_integ_differences.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-08-04 18:37:33.000000 dinglehopper-0.9.2/src/dinglehopper/tests/test_integ_edit_distance_ocr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-08-04 18:37:33.000000 dinglehopper-0.9.2/src/dinglehopper/tests/test_integ_ocrd_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-08-04 18:37:33.000000 dinglehopper-0.9.2/src/dinglehopper/tests/test_integ_summarize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-08-04 18:37:33.000000 dinglehopper-0.9.2/src/dinglehopper/tests/test_integ_table_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-08-04 18:37:33.000000 dinglehopper-0.9.2/src/dinglehopper/tests/test_integ_word_error_rate_ocr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6530 2023-08-04 18:37:33.000000 dinglehopper-0.9.2/src/dinglehopper/tests/test_ocr_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-08-04 18:37:33.000000 dinglehopper-0.9.2/src/dinglehopper/tests/test_word_error_rate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-08-04 18:37:33.000000 dinglehopper-0.9.2/src/dinglehopper/tests/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-08-04 18:37:33.000000 dinglehopper-0.9.2/src/dinglehopper/word_error_rate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:37:50.665294 dinglehopper-0.9.2/src/dinglehopper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6438 2023-08-04 18:37:50.000000 dinglehopper-0.9.2/src/dinglehopper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-08-04 18:37:50.000000 dinglehopper-0.9.2/src/dinglehopper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 18:37:50.000000 dinglehopper-0.9.2/src/dinglehopper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-08-04 18:37:50.000000 dinglehopper-0.9.2/src/dinglehopper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-08-04 18:37:50.000000 dinglehopper-0.9.2/src/dinglehopper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-04 18:37:50.000000 dinglehopper-0.9.2/src/dinglehopper.egg-info/top_level.txt
```

### Comparing `dinglehopper-0.9.1/LICENSE` & `dinglehopper-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dinglehopper-0.9.1/PKG-INFO` & `dinglehopper-0.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dinglehopper
-Version: 0.9.1
+Version: 0.9.2
 Summary: The OCR evaluation tool
 Author-email: Mike Gerber <mike.gerber@sbb.spk-berlin.de>, The QURATOR SPK Team <qurator@sbb.spk-berlin.de>
 Project-URL: Homepage, https://github.com/qurator-spk/dinglehopper
 Project-URL: Repository, https://github.com/qurator-spk/dinglehopper.git
 Keywords: qurator,ocr,evaluation,ocr-d
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `dinglehopper-0.9.1/README.md` & `dinglehopper-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `dinglehopper-0.9.1/pyproject.toml` & `dinglehopper-0.9.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dinglehopper-0.9.1/src/dinglehopper/__init__.py` & `dinglehopper-0.9.2/src/dinglehopper/__init__.py`

 * *Files identical despite different names*

### Comparing `dinglehopper-0.9.1/src/dinglehopper/align.py` & `dinglehopper-0.9.2/src/dinglehopper/align.py`

 * *Files identical despite different names*

### Comparing `dinglehopper-0.9.1/src/dinglehopper/character_error_rate.py` & `dinglehopper-0.9.2/src/dinglehopper/character_error_rate.py`

 * *Files identical despite different names*

### Comparing `dinglehopper-0.9.1/src/dinglehopper/cli.py` & `dinglehopper-0.9.2/src/dinglehopper/cli.py`

 * *Files identical despite different names*

### Comparing `dinglehopper-0.9.1/src/dinglehopper/cli_extract.py` & `dinglehopper-0.9.2/src/dinglehopper/cli_extract.py`

 * *Files identical despite different names*

### Comparing `dinglehopper-0.9.1/src/dinglehopper/cli_line_dirs.py` & `dinglehopper-0.9.2/src/dinglehopper/cli_line_dirs.py`

 * *Files identical despite different names*

### Comparing `dinglehopper-0.9.1/src/dinglehopper/cli_summarize.py` & `dinglehopper-0.9.2/src/dinglehopper/cli_summarize.py`

 * *Files identical despite different names*

### Comparing `dinglehopper-0.9.1/src/dinglehopper/edit_distance.py` & `dinglehopper-0.9.2/src/dinglehopper/edit_distance.py`

 * *Files identical despite different names*

### Comparing `dinglehopper-0.9.1/src/dinglehopper/extracted_text.py` & `dinglehopper-0.9.2/src/dinglehopper/extracted_text.py`

 * *Files identical despite different names*

### Comparing `dinglehopper-0.9.1/src/dinglehopper/ocr_files.py` & `dinglehopper-0.9.2/src/dinglehopper/ocr_files.py`

 * *Files identical despite different names*

### Comparing `dinglehopper-0.9.1/src/dinglehopper/ocrd-tool.json` & `dinglehopper-0.9.2/ocrd-tool.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8333333333333334%*

 * *Differences: {"'version'": "'0.9.2'"}*

```diff
@@ -31,9 +31,9 @@
                 }
             },
             "steps": [
                 "recognition/text-recognition"
             ]
         }
     },
-    "version": "0.9.1"
+    "version": "0.9.2"
 }
```

### Comparing `dinglehopper-0.9.1/src/dinglehopper/ocrd_cli.py` & `dinglehopper-0.9.2/src/dinglehopper/ocrd_cli.py`

 * *Files identical despite different names*

### Comparing `dinglehopper-0.9.1/src/dinglehopper/templates/report.html.j2` & `dinglehopper-0.9.2/src/dinglehopper/templates/report.html.j2`

 * *Files identical despite different names*

### Comparing `dinglehopper-0.9.1/src/dinglehopper/templates/report.html.js` & `dinglehopper-0.9.2/src/dinglehopper/templates/report.html.js`

 * *Files identical despite different names*

### Comparing `dinglehopper-0.9.1/src/dinglehopper/templates/summary.html.j2` & `dinglehopper-0.9.2/src/dinglehopper/templates/summary.html.j2`

 * *Files identical despite different names*

### Comparing `dinglehopper-0.9.1/src/dinglehopper/tests/extracted_text_test.py` & `dinglehopper-0.9.2/src/dinglehopper/tests/extracted_text_test.py`

 * *Files identical despite different names*

### Comparing `dinglehopper-0.9.1/src/dinglehopper/tests/test_align.py` & `dinglehopper-0.9.2/src/dinglehopper/tests/test_align.py`

 * *Files identical despite different names*

### Comparing `dinglehopper-0.9.1/src/dinglehopper/tests/test_character_error_rate.py` & `dinglehopper-0.9.2/src/dinglehopper/tests/test_character_error_rate.py`

 * *Files identical despite different names*

### Comparing `dinglehopper-0.9.1/src/dinglehopper/tests/test_edit_distance.py` & `dinglehopper-0.9.2/src/dinglehopper/tests/test_edit_distance.py`

 * *Files identical despite different names*

### Comparing `dinglehopper-0.9.1/src/dinglehopper/tests/test_editops.py` & `dinglehopper-0.9.2/src/dinglehopper/tests/test_editops.py`

 * *Files identical despite different names*

### Comparing `dinglehopper-0.9.1/src/dinglehopper/tests/test_integ_align.py` & `dinglehopper-0.9.2/src/dinglehopper/tests/test_integ_align.py`

 * *Files identical despite different names*

### Comparing `dinglehopper-0.9.1/src/dinglehopper/tests/test_integ_bigger_texts.py` & `dinglehopper-0.9.2/src/dinglehopper/tests/test_integ_bigger_texts.py`

 * *Files identical despite different names*

### Comparing `dinglehopper-0.9.1/src/dinglehopper/tests/test_integ_character_error_rate_ocr.py` & `dinglehopper-0.9.2/src/dinglehopper/tests/test_integ_character_error_rate_ocr.py`

 * *Files identical despite different names*

### Comparing `dinglehopper-0.9.1/src/dinglehopper/tests/test_integ_cli_dir.py` & `dinglehopper-0.9.2/src/dinglehopper/tests/test_integ_cli_dir.py`

 * *Files identical despite different names*

### Comparing `dinglehopper-0.9.1/src/dinglehopper/tests/test_integ_cli_valid_json.py` & `dinglehopper-0.9.2/src/dinglehopper/tests/test_integ_cli_valid_json.py`

 * *Files identical despite different names*

### Comparing `dinglehopper-0.9.1/src/dinglehopper/tests/test_integ_differences.py` & `dinglehopper-0.9.2/src/dinglehopper/tests/test_integ_differences.py`

 * *Files identical despite different names*

### Comparing `dinglehopper-0.9.1/src/dinglehopper/tests/test_integ_edit_distance_ocr.py` & `dinglehopper-0.9.2/src/dinglehopper/tests/test_integ_edit_distance_ocr.py`

 * *Files identical despite different names*

### Comparing `dinglehopper-0.9.1/src/dinglehopper/tests/test_integ_ocrd_cli.py` & `dinglehopper-0.9.2/src/dinglehopper/tests/test_integ_ocrd_cli.py`

 * *Files identical despite different names*

### Comparing `dinglehopper-0.9.1/src/dinglehopper/tests/test_integ_summarize.py` & `dinglehopper-0.9.2/src/dinglehopper/tests/test_integ_summarize.py`

 * *Files identical despite different names*

### Comparing `dinglehopper-0.9.1/src/dinglehopper/tests/test_integ_table_extraction.py` & `dinglehopper-0.9.2/src/dinglehopper/tests/test_integ_table_extraction.py`

 * *Files identical despite different names*

### Comparing `dinglehopper-0.9.1/src/dinglehopper/tests/test_integ_word_error_rate_ocr.py` & `dinglehopper-0.9.2/src/dinglehopper/tests/test_integ_word_error_rate_ocr.py`

 * *Files identical despite different names*

### Comparing `dinglehopper-0.9.1/src/dinglehopper/tests/test_ocr_files.py` & `dinglehopper-0.9.2/src/dinglehopper/tests/test_ocr_files.py`

 * *Files identical despite different names*

### Comparing `dinglehopper-0.9.1/src/dinglehopper/tests/test_word_error_rate.py` & `dinglehopper-0.9.2/src/dinglehopper/tests/test_word_error_rate.py`

 * *Files identical despite different names*

### Comparing `dinglehopper-0.9.1/src/dinglehopper/tests/util.py` & `dinglehopper-0.9.2/src/dinglehopper/tests/util.py`

 * *Files identical despite different names*

### Comparing `dinglehopper-0.9.1/src/dinglehopper/word_error_rate.py` & `dinglehopper-0.9.2/src/dinglehopper/word_error_rate.py`

 * *Files identical despite different names*

### Comparing `dinglehopper-0.9.1/src/dinglehopper.egg-info/PKG-INFO` & `dinglehopper-0.9.2/src/dinglehopper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dinglehopper
-Version: 0.9.1
+Version: 0.9.2
 Summary: The OCR evaluation tool
 Author-email: Mike Gerber <mike.gerber@sbb.spk-berlin.de>, The QURATOR SPK Team <qurator@sbb.spk-berlin.de>
 Project-URL: Homepage, https://github.com/qurator-spk/dinglehopper
 Project-URL: Repository, https://github.com/qurator-spk/dinglehopper.git
 Keywords: qurator,ocr,evaluation,ocr-d
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `dinglehopper-0.9.1/src/dinglehopper.egg-info/SOURCES.txt` & `dinglehopper-0.9.2/src/dinglehopper.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 LICENSE
+MANIFEST.in
 README.md
+ocrd-tool.json
 pyproject.toml
 requirements-dev.txt
 requirements.txt
 setup.cfg
 src/dinglehopper/__init__.py
 src/dinglehopper/align.py
 src/dinglehopper/character_error_rate.py
```

