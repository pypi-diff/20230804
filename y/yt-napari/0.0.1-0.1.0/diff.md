# Comparing `tmp/yt_napari-0.0.1.tar.gz` & `tmp/yt_napari-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yt_napari-0.0.1.tar", last modified: Mon May  2 22:26:59 2022, max compression
+gzip compressed data, was "yt_napari-0.1.0.tar", last modified: Fri Aug  4 15:18:38 2023, max compression
```

## Comparing `yt_napari-0.0.1.tar` & `yt_napari-0.1.0.tar`

### file list

```diff
@@ -1,50 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-02 22:26:59.073082 yt_napari-0.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-02 22:26:59.069081 yt_napari-0.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-02 22:26:59.073082 yt_napari-0.0.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      952 2022-05-02 22:26:49.000000 yt_napari-0.0.1/.github/ISSUE_TEMPLATE/bug-report.md
--rw-r--r--   0 runner    (1001) docker     (121)      264 2022-05-02 22:26:49.000000 yt_napari-0.0.1/.github/ISSUE_TEMPLATE/feedback-and-discussion.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-02 22:26:59.073082 yt_napari-0.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      510 2022-05-02 22:26:49.000000 yt_napari-0.0.1/.github/workflows/check_build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      524 2022-05-02 22:26:49.000000 yt_napari-0.0.1/.github/workflows/check_manifest.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1729 2022-05-02 22:26:49.000000 yt_napari-0.0.1/.github/workflows/style_checks.yml
--rw-r--r--   0 runner    (1001) docker     (121)     3148 2022-05-02 22:26:49.000000 yt_napari-0.0.1/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1011 2022-05-02 22:26:49.000000 yt_napari-0.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1480 2022-05-02 22:26:49.000000 yt_napari-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      439 2022-05-02 22:26:49.000000 yt_napari-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    12249 2022-05-02 22:26:59.073082 yt_napari-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    10985 2022-05-02 22:26:49.000000 yt_napari-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      251 2022-05-02 22:26:49.000000 yt_napari-0.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1510 2022-05-02 22:26:59.073082 yt_napari-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      201 2022-05-02 22:26:49.000000 yt_napari-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-02 22:26:59.069081 yt_napari-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-02 22:26:59.073082 yt_napari-0.0.1/src/yt_napari/
--rw-r--r--   0 runner    (1001) docker     (121)      156 2022-05-02 22:26:49.000000 yt_napari-0.0.1/src/yt_napari/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2095 2022-05-02 22:26:49.000000 yt_napari-0.0.1/src/yt_napari/_data_model.py
--rw-r--r--   0 runner    (1001) docker     (121)     9199 2022-05-02 22:26:49.000000 yt_napari-0.0.1/src/yt_napari/_gui_utilities.py
--rw-r--r--   0 runner    (1001) docker     (121)    12907 2022-05-02 22:26:49.000000 yt_napari-0.0.1/src/yt_napari/_model_ingestor.py
--rw-r--r--   0 runner    (1001) docker     (121)     3214 2022-05-02 22:26:49.000000 yt_napari-0.0.1/src/yt_napari/_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-02 22:26:59.073082 yt_napari-0.0.1/src/yt_napari/_tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-02 22:26:49.000000 yt_napari-0.0.1/src/yt_napari/_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      823 2022-05-02 22:26:49.000000 yt_napari-0.0.1/src/yt_napari/_tests/_test_json.json
--rw-r--r--   0 runner    (1001) docker     (121)      708 2022-05-02 22:26:49.000000 yt_napari-0.0.1/src/yt_napari/_tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)     3439 2022-05-02 22:26:49.000000 yt_napari-0.0.1/src/yt_napari/_tests/test_gui_utilities.py
--rw-r--r--   0 runner    (1001) docker     (121)     7593 2022-05-02 22:26:49.000000 yt_napari-0.0.1/src/yt_napari/_tests/test_model_ingestor.py
--rw-r--r--   0 runner    (1001) docker     (121)     3770 2022-05-02 22:26:49.000000 yt_napari-0.0.1/src/yt_napari/_tests/test_reader.py
--rw-r--r--   0 runner    (1001) docker     (121)     3470 2022-05-02 22:26:49.000000 yt_napari-0.0.1/src/yt_napari/_tests/test_schema_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)     4523 2022-05-02 22:26:49.000000 yt_napari-0.0.1/src/yt_napari/_tests/test_viewer.py
--rw-r--r--   0 runner    (1001) docker     (121)     1714 2022-05-02 22:26:49.000000 yt_napari-0.0.1/src/yt_napari/_tests/test_widget_reader.py
--rw-r--r--   0 runner    (1001) docker     (121)      142 2022-05-02 22:26:58.000000 yt_napari-0.0.1/src/yt_napari/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)     2355 2022-05-02 22:26:49.000000 yt_napari-0.0.1/src/yt_napari/_widget_reader.py
--rw-r--r--   0 runner    (1001) docker     (121)      527 2022-05-02 22:26:49.000000 yt_napari-0.0.1/src/yt_napari/napari.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-02 22:26:59.073082 yt_napari-0.0.1/src/yt_napari/schemas/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-02 22:26:49.000000 yt_napari-0.0.1/src/yt_napari/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6867 2022-05-02 22:26:49.000000 yt_napari-0.0.1/src/yt_napari/schemas/_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)     3556 2022-05-02 22:26:49.000000 yt_napari-0.0.1/src/yt_napari/schemas/yt-napari_0.0.1.json
--rw-r--r--   0 runner    (1001) docker     (121)    13088 2022-05-02 22:26:49.000000 yt_napari-0.0.1/src/yt_napari/viewer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-02 22:26:59.073082 yt_napari-0.0.1/src/yt_napari.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    12249 2022-05-02 22:26:58.000000 yt_napari-0.0.1/src/yt_napari.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1244 2022-05-02 22:26:59.000000 yt_napari-0.0.1/src/yt_napari.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-02 22:26:58.000000 yt_napari-0.0.1/src/yt_napari.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       52 2022-05-02 22:26:58.000000 yt_napari-0.0.1/src/yt_napari.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       61 2022-05-02 22:26:58.000000 yt_napari-0.0.1/src/yt_napari.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-05-02 22:26:58.000000 yt_napari-0.0.1/src/yt_napari.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:18:38.342951 yt_napari-0.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:18:38.334951 yt_napari-0.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:18:38.338951 yt_napari-0.1.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-08-04 15:18:28.000000 yt_napari-0.1.0/.github/ISSUE_TEMPLATE/bug-report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-08-04 15:18:28.000000 yt_napari-0.1.0/.github/ISSUE_TEMPLATE/feedback-and-discussion.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:18:38.338951 yt_napari-0.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-08-04 15:18:28.000000 yt_napari-0.1.0/.github/workflows/check_build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-08-04 15:18:28.000000 yt_napari-0.1.0/.github/workflows/check_manifest.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-08-04 15:18:28.000000 yt_napari-0.1.0/.github/workflows/style_checks.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2981 2023-08-04 15:18:28.000000 yt_napari-0.1.0/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-08-04 15:18:28.000000 yt_napari-0.1.0/.github/workflows/weekly_build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-08-04 15:18:28.000000 yt_napari-0.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-08-04 15:18:28.000000 yt_napari-0.1.0/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-08-04 15:18:28.000000 yt_napari-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-08-04 15:18:28.000000 yt_napari-0.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    12926 2023-08-04 15:18:38.342951 yt_napari-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11732 2023-08-04 15:18:28.000000 yt_napari-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-08-04 15:18:28.000000 yt_napari-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-08-04 15:18:28.000000 yt_napari-0.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-08-04 15:18:38.342951 yt_napari-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-08-04 15:18:28.000000 yt_napari-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:18:38.334951 yt_napari-0.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:18:38.338951 yt_napari-0.1.0/src/yt_napari/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-08-04 15:18:28.000000 yt_napari-0.1.0/src/yt_napari/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4122 2023-08-04 15:18:28.000000 yt_napari-0.1.0/src/yt_napari/_data_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-08-04 15:18:28.000000 yt_napari-0.1.0/src/yt_napari/_ds_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10617 2023-08-04 15:18:28.000000 yt_napari-0.1.0/src/yt_napari/_gui_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19733 2023-08-04 15:18:28.000000 yt_napari-0.1.0/src/yt_napari/_model_ingestor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-08-04 15:18:28.000000 yt_napari-0.1.0/src/yt_napari/_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-08-04 15:18:28.000000 yt_napari-0.1.0/src/yt_napari/_special_loaders.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:18:38.342951 yt_napari-0.1.0/src/yt_napari/_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 15:18:28.000000 yt_napari-0.1.0/src/yt_napari/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-08-04 15:18:28.000000 yt_napari-0.1.0/src/yt_napari/_tests/_test_json.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-08-04 15:18:28.000000 yt_napari-0.1.0/src/yt_napari/_tests/_test_json_slice.json
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-08-04 15:18:28.000000 yt_napari-0.1.0/src/yt_napari/_tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-08-04 15:18:28.000000 yt_napari-0.1.0/src/yt_napari/_tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-08-04 15:18:28.000000 yt_napari-0.1.0/src/yt_napari/_tests/test_ds_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4789 2023-08-04 15:18:28.000000 yt_napari-0.1.0/src/yt_napari/_tests/test_gui_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-08-04 15:18:28.000000 yt_napari-0.1.0/src/yt_napari/_tests/test_model_ingestor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-08-04 15:18:28.000000 yt_napari-0.1.0/src/yt_napari/_tests/test_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3511 2023-08-04 15:18:28.000000 yt_napari-0.1.0/src/yt_napari/_tests/test_schema_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-08-04 15:18:28.000000 yt_napari-0.1.0/src/yt_napari/_tests/test_schema_version_comparisons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-08-04 15:18:28.000000 yt_napari-0.1.0/src/yt_napari/_tests/test_slices_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-08-04 15:18:28.000000 yt_napari-0.1.0/src/yt_napari/_tests/test_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3460 2023-08-04 15:18:28.000000 yt_napari-0.1.0/src/yt_napari/_tests/test_widget_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-08-04 15:18:38.000000 yt_napari-0.1.0/src/yt_napari/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7776 2023-08-04 15:18:28.000000 yt_napari-0.1.0/src/yt_napari/_widget_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-08-04 15:18:28.000000 yt_napari-0.1.0/src/yt_napari/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-08-04 15:18:28.000000 yt_napari-0.1.0/src/yt_napari/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-08-04 15:18:28.000000 yt_napari-0.1.0/src/yt_napari/napari.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:18:38.342951 yt_napari-0.1.0/src/yt_napari/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 15:18:28.000000 yt_napari-0.1.0/src/yt_napari/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6998 2023-08-04 15:18:28.000000 yt_napari-0.1.0/src/yt_napari/schemas/_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-08-04 15:18:28.000000 yt_napari-0.1.0/src/yt_napari/schemas/_version_comparison.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-08-04 15:18:28.000000 yt_napari-0.1.0/src/yt_napari/schemas/yt-napari_0.0.1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8002 2023-08-04 15:18:28.000000 yt_napari-0.1.0/src/yt_napari/schemas/yt-napari_0.1.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)    17339 2023-08-04 15:18:28.000000 yt_napari-0.1.0/src/yt_napari/viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:18:38.338951 yt_napari-0.1.0/src/yt_napari.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12926 2023-08-04 15:18:38.000000 yt_napari-0.1.0/src/yt_napari.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-08-04 15:18:38.000000 yt_napari-0.1.0/src/yt_napari.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 15:18:38.000000 yt_napari-0.1.0/src/yt_napari.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 15:18:38.000000 yt_napari-0.1.0/src/yt_napari.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-04 15:18:38.000000 yt_napari-0.1.0/src/yt_napari.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-04 15:18:38.000000 yt_napari-0.1.0/src/yt_napari.egg-info/top_level.txt
```

### Comparing `yt_napari-0.0.1/.github/ISSUE_TEMPLATE/bug-report.md` & `yt_napari-0.1.0/.github/ISSUE_TEMPLATE/bug-report.md`

 * *Files identical despite different names*

### Comparing `yt_napari-0.0.1/.github/workflows/check_manifest.yml` & `yt_napari-0.1.0/.github/workflows/check_manifest.yml`

 * *Files identical despite different names*

### Comparing `yt_napari-0.0.1/.github/workflows/style_checks.yml` & `yt_napari-0.1.0/.github/workflows/style_checks.yml`

 * *Files identical despite different names*

### Comparing `yt_napari-0.0.1/.github/workflows/test_and_deploy.yml` & `yt_napari-0.1.0/.github/workflows/test_and_deploy.yml`

 * *Files 9% similar despite different names*

```diff
@@ -19,46 +19,45 @@
 jobs:
   test:
     name: ${{ matrix.platform }} py${{ matrix.python-version }}
     runs-on: ${{ matrix.platform }}
     strategy:
       matrix:
         platform: [ubuntu-latest, windows-latest, macos-latest]
-        python-version: [3.7, 3.8, 3.9]
+        python-version: ['3.8', '3.9', '3.10']
 
     steps:
       - uses: actions/checkout@v2
 
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v2
         with:
           python-version: ${{ matrix.python-version }}
 
-      # these libraries enable testing on Qt on linux
-      - name: Install Linux libraries
-        if: runner.os == 'Linux'
-        run: |
-          sudo apt-get install -y libdbus-1-3 libxkbcommon-x11-0 libxcb-icccm4 \
-            libxcb-image0 libxcb-keysyms1 libxcb-randr0 libxcb-render-util0 \
-            libxcb-xinerama0 libxcb-xinput0 libxcb-xfixes0
+      # install libraries that enable testing on Qt on linux
+      - name: Install QT libraries for Linux
+        uses:  tlambert03/setup-qt-libs@v1
 
       # strategy borrowed from vispy for installing opengl libs on windows
       - name: Install Windows OpenGL
         if: runner.os == 'Windows'
         run: |
           git clone --depth 1 https://github.com/pyvista/gl-ci-helpers.git
           powershell gl-ci-helpers/appveyor/install_opengl.ps1
 
       # note: if you need dependencies from conda, considering using
       # setup-miniconda: https://github.com/conda-incubator/setup-miniconda
       # and
       # tox-conda: https://github.com/tox-dev/tox-conda
+      - name: Upgrade pip
+        run: |
+          python -m pip install --upgrade pip
+
       - name: Install dependencies
         run: |
-          python -m pip install --upgrade "pip < 22"
           python -m pip install setuptools tox tox-gh-actions
 
       # this runs the platform-specific tests declared in tox.ini
       - name: Test with tox
         uses: GabrielBB/xvfb-action@v1
         with:
           # run tox using the version of Python in `PATH`
```

### Comparing `yt_napari-0.0.1/.gitignore` & `yt_napari-0.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `yt_napari-0.0.1/LICENSE` & `yt_napari-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `yt_napari-0.0.1/PKG-INFO` & `yt_napari-0.1.0/src/yt_napari.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,32 @@
 Metadata-Version: 2.1
-Name: yt_napari
-Version: 0.0.1
+Name: yt-napari
+Version: 0.1.0
 Summary: A napari plugin for loading data from yt
 Home-page: https://github.com/data-exp-lab/yt-napari
 Author: Chris Havlin
 Author-email: chris.havlin@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/data-exp-lab/yt-napari/issues
 Project-URL: Documentation, https://github.com/data-exp-lab/yt-napari#README.md
 Project-URL: Source Code, https://github.com/data-exp-lab/yt-napari
 Project-URL: User Support, https://github.com/data-exp-lab/yt-napari/issues
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: napari
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Testing
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # yt-napari
 
 [![License](https://img.shields.io/pypi/l/yt-napari.svg?color=green)](https://github.com/data-exp-lab/yt-napari/raw/main/LICENSE)
 [![PyPI](https://img.shields.io/pypi/v/yt-napari.svg?color=green)](https://pypi.org/project/yt-napari)
@@ -100,62 +98,62 @@
 ds = yt.load("IsolatedGalaxy/galaxy0030/galaxy0030")
 yt_scene = Scene()
 
 left_edge = ds.domain_center - ds.arr([40, 40, 40], 'kpc')
 right_edge = ds.domain_center + ds.arr([40, 40, 40], 'kpc')
 res = (600, 600, 600)
 
-yt_scene.add_to_viewer(viewer,
-                       ds,
-                       ("enzo", "Temperature"),
-                       left_edge = left_edge,
-                       right_edge = right_edge,
-                       resolution = res)
-
-yt_scene.add_to_viewer(viewer,
-                       ds,
-                       ("enzo", "Density"),
-                       left_edge = left_edge,
-                       right_edge = right_edge,
-                       resolution = res)
+yt_scene.add_region(viewer,
+                    ds,
+                    ("enzo", "Temperature"),
+                    left_edge=left_edge,
+                    right_edge=right_edge,
+                    resolution=res)
+
+yt_scene.add_region(viewer,
+                    ds,
+                    ("enzo", "Density"),
+                    left_edge=left_edge,
+                    right_edge=right_edge,
+                    resolution=res)
 
 nbscreenshot(viewer)
 ```
 
  ![Loading a subset of a yt dataset in napari from a Jupyter notebook](./assets/images/readme_ex_001.png)
 
-`yt_scene.add_to_viewer` accepts any of the keyword arguments allowed by `viewer.add_image`. See the full documentation (!!!NEED LINK!!!) for more examples, including additional helper methods for linking layer appearance.
+`yt_scene.add_to_viewer` accepts any of the keyword arguments allowed by `viewer.add_image`. See the full documentation (https://yt-napari.readthedocs.io/en/stable/) for more examples, including additional helper methods for linking layer appearance.
 
 ### loading a selection from a yt dataset interactively
 
-`yt-napari` provides a two ways to sample a yt dataset and load in an image layer into a Napari viewer: the yt Reader plugin and json file specification.
+`yt-napari` provides two ways to sample a yt dataset and load in an image layer into a Napari viewer: the yt Reader plugin and json file specification.
 
 #### using the yt Reader plugin
 
-To use the yt Reader plugin, click on `Plugins -> yt-napari: yt Reader`. Select a file, specify a field type and field, set the region to sample and then simply click "Load":
+To use the yt Reader plugin, click on `Plugins -> yt-napari: yt Reader`. From there, add a region or slice selector then specify a field type and field and bounds to sample  between and then simply click "Load":
 
 ![Loading a subset of a yt dataset from the napari viewer](./assets/images/readme_ex_003_gui_reader.gif)
 
-To load a different field or section, adjust the values and click "Load" again.
+You can add multiple selections and load them all at once or adjust values and click "Load" again.
 
 #### using a json file and schema
 
 `yt-napari` also provides the ability to load json that contain specifications for loading a file. Properly formatted files can be loaded from the napari GUI as you would load any image file (`File->Open`). The json file describes the selection process for a dataset as described by a json-schema. The following json file results in similar layers as the above examples:
 
 
 ```json
 {"$schema": "https://raw.githubusercontent.com/data-exp-lab/yt-napari/main/src/yt_napari/schemas/yt-napari_0.0.1.json",
  "data": [{"filename": "IsolatedGalaxy/galaxy0030/galaxy0030",
-           "selections": [{
+           "selections": {"regions": [{
                             "fields": [{"field_name": "Temperature", "field_type": "enzo", "take_log": true},
                                        {"field_name": "Density", "field_type": "enzo", "take_log": true}],
                             "left_edge": [460.0, 460.0, 460.0],
                             "right_edge": [560.0, 560.0, 560.0],
                             "resolution": [600, 600, 600]
-                          }],
+                          }]},
            "edge_units": "kpc"
          }]
 }
 ```
 
 To help in filling out a json file, it is recommended that you use an editor capable of parsing a json schema and displaying hints. For example, in vscode, you will see field suggestions after specifying the `yt-napari` schema:
 
@@ -202,38 +200,60 @@
 This will update the `rst` files in `docs/source/` with the latest docstrings in `yt_napari`. Next, build the html documentation with
 
     make html
 
 
 ### updating the pydantic models and schema
 
-Updates to the pydantic models should be accompanied by updates to the json schema. There are a number of utilities to help automate the management of schema.
+The schema versioning follows a `major.minor.micro` versioning pattern that matches the yt-napari versioning. Each yt-napari release should have an accompanying updated schema file, even if the  contents of the schema file have not changed. On-disk schema are stored in  `src/yt_napari/schemas/`, with copies in the documentation at `docs/_static`.
 
-The schema versioning follows a `major.minor.micro` versioning pattern and yt-napari schema are stored in `src/yt_napari/schemas/`. When changing the model, you can store a new schema from a python shell with:
+There are a number of utilities to help automate the management of schema in `repo_utilities/`. The easiest way to use these utitities is with `taskipy` from the command line. To list available scripts:
 
+```commandline
+task --list
+```
+
+Before a release, run
+
+```commandline
+task validate_release vX.X.X
+```
 
-    from yt_napari._data_model import _store_schema
-    _store_schema()
+where `vX.X.X` is the version of the upcoming release. This script will run through some checks that ensure:
+* the on-disk schema matches the schema generated by the pydantic model
+* the schema files in the documentation match the schema files in the package
 
-And the current version of the primary pydantic model, `yt_napari._data_model.InputModel`, will be exported to a new json schema file. By default, the micro version number will be incremented. To increment the major or minor version number, you can supply any of the keyword arguments described in the `write_new_schema` method of the `yt_napari.schemas._mananager.Manager` class.
+If any of the checks fail, you will be advised to update the schema using `update_schema_docs`. If you
+run without providing a version:
 
-After updating or adding a new schema, the docs also need to be updated. To do that, run
+```commandline
+task update_schema_docs
+```
 
-    python repo_utilities/update_schema_docs.py
-    make clean && make html
+It will simply copy over the existing on-disk schema files to the documentation. If you run with a version:
+
+```commandline
+task update_schema_docs vX.X.X
+```
+It will write a schema file for the current pydantic model, overwriting any on-disk schema files for
+the provided version.
 
 ## License
 
 Distributed under the terms of the [BSD-3] license,
 "yt-napari" is free and open source software
 
 ## Issues
 
 If you encounter any problems, please [file an issue] along with a detailed description.
 
+## Funding
+
+The yt-napari plugin project was funded with support from the Chan Zuckerberg Initiative through the napari Plugin Accelerator Grants project, [Enabling Access To Multi-resolution Data](https://chanzuckerberg.com/science/programs-resources/imaging/napari/enabling-access-to-multi-resolution-data/).
+
 ----------------------------------
 
 This [napari] plugin was generated with [Cookiecutter] using [@napari]'s [cookiecutter-napari-plugin] template.
 
 <!--
 Don't miss the full getting started guide to set up your new package:
 https://github.com/napari/cookiecutter-napari-plugin#getting-started
@@ -257,9 +277,7 @@
 [file an issue]: https://github.com/data-exp-lab/yt-napari/issues
 
 [napari]: https://github.com/napari/napari
 [tox]: https://tox.readthedocs.io/en/latest/
 [pip]: https://pypi.org/project/pip/
 [PyPI]: https://pypi.org/
 [yt]: https://yt-project.org/
-
-
```

### Comparing `yt_napari-0.0.1/README.md` & `yt_napari-0.1.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -70,62 +70,62 @@
 ds = yt.load("IsolatedGalaxy/galaxy0030/galaxy0030")
 yt_scene = Scene()
 
 left_edge = ds.domain_center - ds.arr([40, 40, 40], 'kpc')
 right_edge = ds.domain_center + ds.arr([40, 40, 40], 'kpc')
 res = (600, 600, 600)
 
-yt_scene.add_to_viewer(viewer,
-                       ds,
-                       ("enzo", "Temperature"),
-                       left_edge = left_edge,
-                       right_edge = right_edge,
-                       resolution = res)
-
-yt_scene.add_to_viewer(viewer,
-                       ds,
-                       ("enzo", "Density"),
-                       left_edge = left_edge,
-                       right_edge = right_edge,
-                       resolution = res)
+yt_scene.add_region(viewer,
+                    ds,
+                    ("enzo", "Temperature"),
+                    left_edge=left_edge,
+                    right_edge=right_edge,
+                    resolution=res)
+
+yt_scene.add_region(viewer,
+                    ds,
+                    ("enzo", "Density"),
+                    left_edge=left_edge,
+                    right_edge=right_edge,
+                    resolution=res)
 
 nbscreenshot(viewer)
 ```
 
  ![Loading a subset of a yt dataset in napari from a Jupyter notebook](./assets/images/readme_ex_001.png)
 
-`yt_scene.add_to_viewer` accepts any of the keyword arguments allowed by `viewer.add_image`. See the full documentation (!!!NEED LINK!!!) for more examples, including additional helper methods for linking layer appearance.
+`yt_scene.add_to_viewer` accepts any of the keyword arguments allowed by `viewer.add_image`. See the full documentation (https://yt-napari.readthedocs.io/en/stable/) for more examples, including additional helper methods for linking layer appearance.
 
 ### loading a selection from a yt dataset interactively
 
-`yt-napari` provides a two ways to sample a yt dataset and load in an image layer into a Napari viewer: the yt Reader plugin and json file specification.
+`yt-napari` provides two ways to sample a yt dataset and load in an image layer into a Napari viewer: the yt Reader plugin and json file specification.
 
 #### using the yt Reader plugin
 
-To use the yt Reader plugin, click on `Plugins -> yt-napari: yt Reader`. Select a file, specify a field type and field, set the region to sample and then simply click "Load":
+To use the yt Reader plugin, click on `Plugins -> yt-napari: yt Reader`. From there, add a region or slice selector then specify a field type and field and bounds to sample  between and then simply click "Load":
 
 ![Loading a subset of a yt dataset from the napari viewer](./assets/images/readme_ex_003_gui_reader.gif)
 
-To load a different field or section, adjust the values and click "Load" again.
+You can add multiple selections and load them all at once or adjust values and click "Load" again.
 
 #### using a json file and schema
 
 `yt-napari` also provides the ability to load json that contain specifications for loading a file. Properly formatted files can be loaded from the napari GUI as you would load any image file (`File->Open`). The json file describes the selection process for a dataset as described by a json-schema. The following json file results in similar layers as the above examples:
 
 
 ```json
 {"$schema": "https://raw.githubusercontent.com/data-exp-lab/yt-napari/main/src/yt_napari/schemas/yt-napari_0.0.1.json",
  "data": [{"filename": "IsolatedGalaxy/galaxy0030/galaxy0030",
-           "selections": [{
+           "selections": {"regions": [{
                             "fields": [{"field_name": "Temperature", "field_type": "enzo", "take_log": true},
                                        {"field_name": "Density", "field_type": "enzo", "take_log": true}],
                             "left_edge": [460.0, 460.0, 460.0],
                             "right_edge": [560.0, 560.0, 560.0],
                             "resolution": [600, 600, 600]
-                          }],
+                          }]},
            "edge_units": "kpc"
          }]
 }
 ```
 
 To help in filling out a json file, it is recommended that you use an editor capable of parsing a json schema and displaying hints. For example, in vscode, you will see field suggestions after specifying the `yt-napari` schema:
 
@@ -172,38 +172,60 @@
 This will update the `rst` files in `docs/source/` with the latest docstrings in `yt_napari`. Next, build the html documentation with
 
     make html
 
 
 ### updating the pydantic models and schema
 
-Updates to the pydantic models should be accompanied by updates to the json schema. There are a number of utilities to help automate the management of schema.
+The schema versioning follows a `major.minor.micro` versioning pattern that matches the yt-napari versioning. Each yt-napari release should have an accompanying updated schema file, even if the  contents of the schema file have not changed. On-disk schema are stored in  `src/yt_napari/schemas/`, with copies in the documentation at `docs/_static`.
 
-The schema versioning follows a `major.minor.micro` versioning pattern and yt-napari schema are stored in `src/yt_napari/schemas/`. When changing the model, you can store a new schema from a python shell with:
+There are a number of utilities to help automate the management of schema in `repo_utilities/`. The easiest way to use these utitities is with `taskipy` from the command line. To list available scripts:
 
+```commandline
+task --list
+```
+
+Before a release, run
 
-    from yt_napari._data_model import _store_schema
-    _store_schema()
+```commandline
+task validate_release vX.X.X
+```
 
-And the current version of the primary pydantic model, `yt_napari._data_model.InputModel`, will be exported to a new json schema file. By default, the micro version number will be incremented. To increment the major or minor version number, you can supply any of the keyword arguments described in the `write_new_schema` method of the `yt_napari.schemas._mananager.Manager` class.
+where `vX.X.X` is the version of the upcoming release. This script will run through some checks that ensure:
+* the on-disk schema matches the schema generated by the pydantic model
+* the schema files in the documentation match the schema files in the package
 
-After updating or adding a new schema, the docs also need to be updated. To do that, run
+If any of the checks fail, you will be advised to update the schema using `update_schema_docs`. If you
+run without providing a version:
+
+```commandline
+task update_schema_docs
+```
 
-    python repo_utilities/update_schema_docs.py
-    make clean && make html
+It will simply copy over the existing on-disk schema files to the documentation. If you run with a version:
+
+```commandline
+task update_schema_docs vX.X.X
+```
+It will write a schema file for the current pydantic model, overwriting any on-disk schema files for
+the provided version.
 
 ## License
 
 Distributed under the terms of the [BSD-3] license,
 "yt-napari" is free and open source software
 
 ## Issues
 
 If you encounter any problems, please [file an issue] along with a detailed description.
 
+## Funding
+
+The yt-napari plugin project was funded with support from the Chan Zuckerberg Initiative through the napari Plugin Accelerator Grants project, [Enabling Access To Multi-resolution Data](https://chanzuckerberg.com/science/programs-resources/imaging/napari/enabling-access-to-multi-resolution-data/).
+
 ----------------------------------
 
 This [napari] plugin was generated with [Cookiecutter] using [@napari]'s [cookiecutter-napari-plugin] template.
 
 <!--
 Don't miss the full getting started guide to set up your new package:
 https://github.com/napari/cookiecutter-napari-plugin#getting-started
```

### Comparing `yt_napari-0.0.1/setup.cfg` & `yt_napari-0.1.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -13,36 +13,35 @@
 	Framework :: napari
 	Intended Audience :: Developers
 	License :: OSI Approved :: BSD License
 	Operating System :: OS Independent
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Topic :: Software Development :: Testing
 include_package_data = True
 project_urls = 
 	Bug Tracker = https://github.com/data-exp-lab/yt-napari/issues
 	Documentation = https://github.com/data-exp-lab/yt-napari#README.md
 	Source Code = https://github.com/data-exp-lab/yt-napari
 	User Support = https://github.com/data-exp-lab/yt-napari/issues
 
 [options]
 packages = find:
 install_requires = 
-	magicgui>=0.4.0
+	magicgui>=0.6.1
 	napari>=0.4.13
 	npe2
 	numpy
 	pydantic
 	yt>=4.0.1
-python_requires = >=3.7
+python_requires = >=3.8
 package_dir = 
 	=src
 setup_requires = 
 	setuptools-scm
 
 [options.packages.find]
 where = src
```

### Comparing `yt_napari-0.0.1/src/yt_napari/_gui_utilities.py` & `yt_napari-0.1.0/src/yt_napari/_gui_utilities.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-import warnings
 from collections import defaultdict
-from typing import Callable, Optional, Union
+from typing import Callable, List, Optional, Union
 
 import pydantic
 from magicgui import type_map, widgets
 
 from yt_napari import _data_model
+from yt_napari.logging import ytnapari_log
 
 
 def set_default(variable, default):
     if variable is None:
         return default
     return variable
 
@@ -102,18 +102,27 @@
             func, args, kwargs = self.registry[pydantic_model][field]["pydantic"]
             return func(widget_instance, *args, **kwargs)
 
     def add_pydantic_to_container(
         self,
         py_model: Union[pydantic.BaseModel, pydantic.main.ModelMetaclass],
         container: widgets.Container,
+        ignore_attrs: Optional[Union[str, List[str]]] = None,
     ):
         # recursively traverse a pydantic model adding widgets to a container.
         # When a nested pydantic model is encountered, add a new container
+
+        if not isinstance(ignore_attrs, list):
+            ignore_attrs = [
+                ignore_attrs,
+            ]
+
         for field, field_def in py_model.__fields__.items():
+            if field in ignore_attrs:
+                continue
             ftype = field_def.type_
             if isinstance(ftype, pydantic.BaseModel) or isinstance(
                 ftype, pydantic.main.ModelMetaclass
             ):
                 # the field is a pydantic class, add a container for it and fill it
                 new_widget_cls = widgets.Container
                 new_widget = new_widget_cls(name=field_def.name)
@@ -121,25 +130,35 @@
             elif self.is_registered(py_model, field):
                 new_widget = self.get_widget_instance(py_model, field)
             else:
                 new_widget = get_magicguidefault(field_def)
                 if isinstance(new_widget, widgets.EmptyWidget):
                     msg = "magicgui could not identify a widget for "
                     msg += f" {py_model}.{field}, which has type {ftype}"
-                    warnings.warn(message=msg)
+                    ytnapari_log.warning(msg)
             container.append(new_widget)
 
     def get_pydantic_kwargs(
-        self, container: widgets.Container, py_model, pydantic_kwargs: dict
+        self,
+        container: widgets.Container,
+        py_model,
+        pydantic_kwargs: dict,
+        ignore_attrs: Optional[Union[str, List[str]]] = None,
     ):
         # given a container that was instantiated from a pydantic model, get
         # the arguments needed to instantiate that pydantic model
+        if not isinstance(ignore_attrs, list):
+            ignore_attrs = [
+                ignore_attrs,
+            ]
 
         # traverse model fields, pull out values from container
         for field, field_def in py_model.__fields__.items():
+            if field in ignore_attrs:
+                continue
             ftype = field_def.type_
             if isinstance(ftype, pydantic.BaseModel) or isinstance(
                 ftype, pydantic.main.ModelMetaclass
             ):
                 new_kwargs = {}  # new dictionary for the new nest level
                 # any pydantic class will be a container, so pull that out to pass
                 # to the recursive call
@@ -180,14 +199,15 @@
 def get_magicguidefault(field_def: pydantic.fields.ModelField):
     # returns an instance of the default widget selected by magicgui
     ftype = field_def.type_
     new_widget_cls, ops = type_map.get_widget_class(
         None,
         ftype,
         dict(name=field_def.name, value=field_def.default, annotation=ftype),
+        raise_on_unknown=False,
     )
     if field_def.default is None:
         # for some widgets, explicitly passing None as a default will error
         _ = ops.pop("value", None)
 
     return new_widget_cls(**ops)
 
@@ -198,44 +218,70 @@
     return returnval
 
 
 def _get_pydantic_model_field(py_model, field: str) -> pydantic.fields.ModelField:
     return py_model.__fields__[field]
 
 
+# the following model-field tuples will be embedded in containers
+_models_to_embed_in_list = (
+    (_data_model.Slice, "fields"),
+    (_data_model.Region, "fields"),
+    (_data_model.DataContainer, "selections"),
+    (_data_model.SelectionObject, "regions"),
+    (_data_model.SelectionObject, "slices"),
+)
+
+
 def _register_yt_data_model(translator: MagicPydanticRegistry):
     # registers some special cases for pydantic fields.
     translator.register(
         _data_model.DataContainer,
         "filename",
         magicgui_factory=get_file_widget,
         magicgui_kwargs={"name": "filename"},
         pydantic_attr_factory=get_filename,
     )
 
-    py_model, field = _data_model.SelectionObject, "fields"
-    translator.register(
-        py_model,
-        field,
-        magicgui_factory=get_magicguidefault,
-        magicgui_args=(py_model.__fields__[field]),
-        pydantic_attr_factory=embed_in_list,
-    )
-
-    py_model, field = _data_model.DataContainer, "selections"
-    translator.register(
-        py_model,
-        field,
-        magicgui_factory=get_magicguidefault,
-        magicgui_args=(py_model.__fields__[field]),
-        pydantic_attr_factory=embed_in_list,
-    )
+    for py_model, field in _models_to_embed_in_list:
+        translator.register(
+            py_model,
+            field,
+            magicgui_factory=get_magicguidefault,
+            magicgui_args=(py_model.__fields__[field]),
+            pydantic_attr_factory=embed_in_list,
+        )
 
 
 translator = MagicPydanticRegistry()
 _register_yt_data_model(translator)
 
 
-def get_yt_data_container():
+def get_yt_data_container(
+    ignore_attrs: Optional[Union[str, List[str]]] = None
+) -> widgets.Container:
     data_container = widgets.Container()
-    translator.add_pydantic_to_container(_data_model.DataContainer, data_container)
+    translator.add_pydantic_to_container(
+        _data_model.DataContainer,
+        data_container,
+        ignore_attrs=ignore_attrs,
+    )
     return data_container
+
+
+_valid_selections = ("Region", "Slice")
+
+
+def get_yt_selection_container(selection_type: str, return_native: bool = False):
+    # return a container for a single selection
+    if selection_type not in _valid_selections:
+        raise ValueError(
+            f"selection_type must be one of {_valid_selections}, "
+            f"found {selection_type}"
+        )
+
+    selection_container = widgets.Container()
+    pydantic_model = getattr(_data_model, selection_type)
+    translator.add_pydantic_to_container(pydantic_model, selection_container)
+    if return_native:
+        return selection_container.native
+    return selection_container
```

### Comparing `yt_napari-0.0.1/src/yt_napari/_model_ingestor.py` & `yt_napari-0.1.0/src/yt_napari/_model_ingestor.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,45 +1,95 @@
 from typing import List, Optional, Tuple, Union
 
 import numpy as np
-import yt
-from unyt import unit_object, unit_registry, unyt_array
+from unyt import unit_object, unit_registry, unyt_array, unyt_quantity
 
-from yt_napari._data_model import InputModel
+from yt_napari._data_model import DataContainer, InputModel
+from yt_napari._ds_cache import dataset_cache
 
 
 def _le_re_to_cen_wid(
     left_edge: unyt_array, right_edge: unyt_array
 ) -> Tuple[unyt_array, unyt_array]:
     # return the center and width from a left and right edge
     center = (right_edge + left_edge) / 2.0
     width = right_edge - left_edge
     return center, width
 
 
 class LayerDomain:
     # container for domain info for a single layer
+    # left_edge, right_edge, resolution, n_d are all self explanatory.
+    # other parameters:
+    #
+    # new_dim_value: optional unyt_quantity.
+    #   If n_d == 2, and upgrade_to_3D is subsequently called, then this value
+    #   will be used for the new
+    # new_dim_axis: optional int.
+    #   the index position to add the new_dim_position, default is last
     def __init__(
-        self, left_edge: unyt_array, right_edge: unyt_array, resolution: tuple
+        self,
+        left_edge: unyt_array,
+        right_edge: unyt_array,
+        resolution: tuple,
+        n_d: Optional[int] = 3,
+        new_dim_value: Optional[unyt_quantity] = None,
+        new_dim_axis: Optional[int] = 2,
     ):
 
         if len(left_edge) != len(right_edge):
             raise ValueError("length of edge arrays must match")
 
         if len(resolution) != len(left_edge):
             if len(resolution) == 1:
-                resolution = resolution * 3  # assume same in every dim
+                resolution = resolution * n_d  # assume same in every dim
             else:
-                raise ValueError("length of resolution does not match edge arrays")
+                msg = f"{len(resolution)}:{len(left_edge)}"
+                raise ValueError(
+                    f"length of resolution does not match edge arrays {msg}"
+                )
 
         self.left_edge = left_edge
         self.right_edge = right_edge
         self.center, self.width = _le_re_to_cen_wid(left_edge, right_edge)
         self.resolution = unyt_array(resolution)
         self.grid_width = self.width / self.resolution
+        self.aspect_ratio = self.width / self.width[0]
+        self.requires_scale = np.any(self.aspect_ratio != unyt_array(1.0, ""))
+        self.n_d = n_d
+        if new_dim_value is None:
+            new_dim_value = unyt_quantity(0.0, left_edge.units)
+        self.new_dim_value = new_dim_value
+        self.new_dim_axis = new_dim_axis
+
+    def upgrade_to_3D(self):
+        # note: this is not (yet) used when loading planes in 3d scenes.
+        if self.n_d == 3:
+            return  # already 3D, nothing to do
+
+        if self.n_d == 2:
+            new_l_r = self.new_dim_value
+            axid = self.new_dim_axis
+            self.left_edge = _insert_to_unyt_array(self.left_edge, new_l_r, axid)
+            self.right_edge = _insert_to_unyt_array(self.right_edge, new_l_r, axid)
+            self.resolution = _insert_to_unyt_array(self.right_edge, 1, axid)
+            self.grid_width = _insert_to_unyt_array(self.grid_width, 0, axid)
+            self.aspect_ratio = _insert_to_unyt_array(self.aspect_ratio, 1.0, axid)
+            self.n_d = 3
+
+
+def _insert_to_unyt_array(
+    x: unyt_array, new_value: Union[float, unyt_array], position: int
+) -> unyt_array:
+    # just for scalars
+    if isinstance(new_value, unyt_array):
+        # reminder: unyt_quantity is instance of unyt_array
+        new_value = new_value.to(x.units).d
+
+    return unyt_array(np.insert(x.d, position, new_value), x.units)
 
 
 # define types for the napari layer tuples
 Layer = Tuple[np.ndarray, dict, str]
 SpatialLayer = Tuple[np.ndarray, dict, str, LayerDomain]
 
 
@@ -52,23 +102,32 @@
         # copy over standard layer attributes
         self.left_edge = ref_layer_domain.left_edge
         self.right_edge = ref_layer_domain.right_edge
         self.center = ref_layer_domain.center
         self.width = ref_layer_domain.width
         self.resolution = ref_layer_domain.resolution
         self.grid_width = ref_layer_domain.grid_width
+        self.aspect_ratio = ref_layer_domain.aspect_ratio
+
+        # and store the full domain
+        self.layer_domain = ref_layer_domain
 
     def calculate_scale(self, other_layer: LayerDomain) -> unyt_array:
         # calculate the pixel scale for a layer relative to the reference
 
         # the scale accounts for different grid resolutions and is calculated
         # relative to the minimum grid resolution in each direction across
         # layers. scale > 1 will take a small number of pixels and stretch them
         # to cover more pixels. scale < 1 will shrink them.
-        return other_layer.grid_width / self.grid_width
+        sc = other_layer.grid_width / self.grid_width
+        sc[sc == 0] = 1.0
+
+        # we also need to multiply by the initial reference layer aspect ratio
+        # to account for any initial distortion.
+        return sc * self.aspect_ratio
 
     def calculate_translation(self, other_layer: LayerDomain) -> unyt_array:
         # get the translation vector for another layer relative to the left edge
         # of the reference layer
 
         # the translation vector is in PIXELS, so get a translation vector in
         # physical units and then normalize by the reference grid width to get
@@ -80,14 +139,20 @@
     def align_sanitize_layer(self, layer: SpatialLayer) -> Layer:
         # align and scale a single SpatialLayer relative to the reference layer,
         # return a standard Layer tuple
 
         # pull out the elements of the SpatialLayer tuple
         im_arr, im_kwargs, layer_type, domain = layer
 
+        # bypass if adding a 2d layer
+        if domain.n_d == 2 and self.layer_domain.n_d == 3:
+            # when mixing 2d and 3d selections, cannot guarantee alignment
+            # or scaling, simply return with no adjustment
+            return (im_arr, im_kwargs, layer_type)
+
         # calculate scale and translation
         scale = self.calculate_scale(domain)
         translate = self.calculate_translation(domain)
 
         # store these in the image layer keyword arguments only if they are used
         if np.any(scale != 1.0):
             im_kwargs["scale"] = scale.tolist()
@@ -110,15 +175,15 @@
 
 
 def create_metadata_dict(
     data: np.ndarray,
     layer_domain: LayerDomain,
     is_log: bool,
     reference_layer: Optional[ReferenceLayer] = None,
-    **kwargs
+    **kwargs,
 ) -> dict:
     """
     returns a metadata dict with some consistent keys for helping yt-napari
     functionality
 
     Parameters
     ----------
@@ -274,55 +339,167 @@
 
     def update_width_and_center(self):
         # set the domain center and width based on current edges
         center_wid = _le_re_to_cen_wid(self.left_edge, self.right_edge)
         self.center, self.width = center_wid
 
 
+def _load_3D_regions(ds, m_data: DataContainer, layer_list: list) -> list:
+
+    for sel in m_data.selections.regions:
+        # get the left, right edge as a unitful array, initialize the layer
+        # domain tracking for this layer and update the global domain extent
+        if sel.left_edge is None:
+            LE = ds.domain_left_edge
+        else:
+            LE = ds.arr(sel.left_edge.value, sel.left_edge.unit)
+
+        if sel.right_edge is None:
+            RE = ds.domain_right_edge
+        else:
+            RE = ds.arr(sel.right_edge.value, sel.right_edge.unit)
+        res = sel.resolution
+        layer_domain = LayerDomain(left_edge=LE, right_edge=RE, resolution=res)
+
+        # create the fixed resolution buffer
+        frb = ds.r[
+            LE[0] : RE[0] : complex(0, res[0]),  # noqa: E203
+            LE[1] : RE[1] : complex(0, res[1]),  # noqa: E203
+            LE[2] : RE[2] : complex(0, res[2]),  # noqa: E203
+        ]
+
+        for field_container in sel.fields:
+            field = (field_container.field_type, field_container.field_name)
+
+            data = frb[field]  # extract the field (the slow part)
+            if field_container.take_log:
+                data = np.log10(data)
+
+            # create a metadata dict and set a name
+            fieldname = ":".join(field)
+            md = create_metadata_dict(data, layer_domain, field_container.take_log)
+            add_kwargs = {"name": fieldname, "metadata": md}
+            layer_type = "image"
+
+            layer_list.append((data, add_kwargs, layer_type, layer_domain))
+
+    return layer_list
+
+
+def _process_slice(
+    ds,
+    normal: Union[str, int],
+    center: Optional[unyt_array] = None,
+    width: Optional[unyt_quantity] = None,
+    height: Optional[unyt_quantity] = None,
+    resolution: Optional[Tuple[int, int]] = (400, 400),
+    periodic: Optional[bool] = False,
+) -> tuple:
+    # returns a slice frb and a LayerDomain for a slice
+    axis_id = ds.coordinates.axis_id
+    normal_ax = axis_id[normal]
+    x_axis = axis_id[ds.coordinates.image_axis_name[normal][0]]
+    y_axis = axis_id[ds.coordinates.image_axis_name[normal][1]]
+
+    if center is None:
+        center = ds.domain_center
+    if width is None:
+        width = ds.domain_width[x_axis]
+    if height is None:
+        height = ds.domain_width[y_axis]
+
+    LE = ds.arr([0.0, 0.0], "code_length")
+    RE = ds.arr([0.0, 0.0], "code_length")
+    LE[0] = center[x_axis] - width / 2.0
+    RE[0] = center[x_axis] + width / 2.0
+    LE[1] = center[y_axis] - height / 2.0
+    RE[1] = center[y_axis] + height / 2.0
+
+    slc = ds.slice(normal_ax, center[normal_ax])
+    frb = slc.to_frb(
+        width=width,
+        height=height,
+        center=center,
+        resolution=resolution,
+        periodic=periodic,
+    )
+
+    layer_domain = LayerDomain(
+        left_edge=LE,
+        right_edge=RE,
+        resolution=resolution,
+        n_d=2,
+        new_dim_axis=2,
+        new_dim_value=0.0,
+    )
+
+    return frb, layer_domain
+
+
+def _load_2D_slices(ds, m_data: DataContainer, layer_list: list) -> list:
+
+    for slice in m_data.selections.slices:
+
+        if slice.center is None:
+            c = None
+        else:
+            c = ds.arr(slice.center.value, slice.center.unit)
+
+        if slice.slice_width is None:
+            w = None
+        else:
+            w = ds.quan(slice.slice_width.value, slice.slice_width.unit)
+
+        if slice.slice_height is None:
+            h = None
+        else:
+            h = ds.quan(slice.slice_height.value, slice.slice_height.unit)
+
+        frb, layer_domain = _process_slice(
+            ds,
+            slice.normal,
+            center=c,
+            width=w,
+            height=h,
+            resolution=slice.resolution,
+            periodic=slice.periodic,
+        )
+
+        for field_container in slice.fields:
+            field = (field_container.field_type, field_container.field_name)
+
+            data = frb[field]  # extract the field (the slow part)
+            if field_container.take_log:
+                data = np.log10(data)
+
+            # create a metadata dict and set a name
+            fieldname = ":".join(field)
+            md = create_metadata_dict(data, layer_domain, field_container.take_log)
+            add_kwargs = {"name": fieldname, "metadata": md}
+            layer_type = "image"
+
+            layer_list.append((data, add_kwargs, layer_type, layer_domain))
+
+    return layer_list
+
+
 def _process_validated_model(model: InputModel) -> List[SpatialLayer]:
     # return a list of layer tuples with domain information
 
     layer_list = []
-
     # our model is already validated, so we can assume the field exist with
     # their correct types. This is all the yt-specific code required to load a
     # dataset and return a plain numpy array
     for m_data in model.data:
 
-        ds = yt.load(m_data.filename)
-
-        for sel in m_data.selections:
-            # get the left, right edge as a unitful array, initialize the layer
-            # domain tracking for this layer and update the global domain extent
-            LE = ds.arr(sel.left_edge, m_data.edge_units)
-            RE = ds.arr(sel.right_edge, m_data.edge_units)
-            res = sel.resolution
-            layer_domain = LayerDomain(left_edge=LE, right_edge=RE, resolution=res)
-
-            # create the fixed resolution buffer
-            frb = ds.r[
-                LE[0] : RE[0] : complex(0, res[0]),  # noqa: E203
-                LE[1] : RE[1] : complex(0, res[1]),  # noqa: E203
-                LE[2] : RE[2] : complex(0, res[2]),  # noqa: E203
-            ]
-
-            for field_container in sel.fields:
-                field = (field_container.field_type, field_container.field_name)
-
-                data = frb[field]  # extract the field (the slow part)
-                if field_container.take_log:
-                    data = np.log10(data)
-
-                # create a metadata dict and set a name
-                fieldname = ":".join(field)
-                md = create_metadata_dict(data, layer_domain, field_container.take_log)
-                add_kwargs = {"name": fieldname, "metadata": md}
-                layer_type = "image"
-
-                layer_list.append((data, add_kwargs, layer_type, layer_domain))
+        ds = dataset_cache.check_then_load(m_data.filename)
+        if m_data.selections.regions is not None:
+            layer_list = _load_3D_regions(ds, m_data, layer_list)
+        if m_data.selections.slices is not None:
+            layer_list = _load_2D_slices(ds, m_data, layer_list)
 
     return layer_list
 
 
 def load_from_json(json_paths: List[str]) -> List[Layer]:
 
     layer_lists = []  # we will concatenate layers across json paths
@@ -335,12 +512,35 @@
         # to execute the code that will return our array for the image
         layer_lists += _process_validated_model(model)
 
     # now we need to align all our layers!
     # choose a reference layer -- using the first in the list at present, could
     # make this user configurable and/or use the layer with highest pixel density
     # as the reference so that high density layers do not lose resolution
-    layer_0 = layer_lists[0][3]
-    ref_layer = ReferenceLayer(layer_0)
+    ref_layer = _choose_ref_layer(layer_lists)
     layer_lists = ref_layer.align_sanitize_layers(layer_lists)
 
     return layer_lists
+
+
+def _choose_ref_layer(
+    layer_list: List[SpatialLayer], method: Optional[str] = "first_in_list"
+) -> ReferenceLayer:
+    # decides on which layer to use as the reference
+    if method == "first_in_list":
+        ref_layer_id = 0
+    elif method == "smallest_volume":
+        min_vol = None
+        for layer_id, layer in enumerate(layer_list):
+            ld = layer[3]  # the layer domain
+            layer_vol = np.prod(ld.width)
+            if min_vol is None:
+                min_vol = layer_vol
+                ref_layer_id = layer_id
+            elif layer_vol < min_vol:
+                min_vol = layer_vol
+                ref_layer_id = layer_id
+    else:
+        vmeths = ("first_in_list", "smallest_volume")
+        raise ValueError(f"method must be one of {vmeths}, found {method}")
+
+    return ReferenceLayer(layer_list[ref_layer_id][3])
```

### Comparing `yt_napari-0.0.1/src/yt_napari/_reader.py` & `yt_napari-0.1.0/src/yt_napari/_reader.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 https://napari.org/plugins/stable/npe2_manifest_specification.html
 
 Replace code below accordingly.  For complete documentation see:
 https://napari.org/docs/dev/plugins/index.html
 """
 import json
 
-from yt_napari._data_model import InputModel
+from yt_napari.logging import ytnapari_log
+from yt_napari.schemas._version_comparison import schema_version_is_valid
 
 
 def napari_get_reader(path):
     """A basic implementation of a Reader contribution.
 
     Parameters
     ----------
@@ -45,21 +46,15 @@
         return False
 
     # check the schema
     with open(path) as jhandle:
         schema_raw = json.load(jhandle)
         schema_version = schema_raw.get("$schema", None)
 
-    pfx = InputModel._schema_prefix
-    if schema_version is None or pfx not in schema_version:
-        # To Do: check schema against a list of valid schemas rather than a
-        # single schema.
-        # the schema does not match a known schema for this plugin
-        return False
-    return True
+    return schema_version_is_valid(schema_version)
 
 
 def reader_function(path):
     """Take a path or list of paths and return a list of LayerData tuples.
 
     Readers are expected to return data as a list of tuples, where each tuple
     is (data, [add_kwargs, [layer_type]]), "add_kwargs" and "layer_type" are
@@ -82,14 +77,14 @@
     """
     from yt_napari._model_ingestor import load_from_json
 
     # handle both a string and a list of strings
     if isinstance(path, list):
         path_list = [p for p in path if path_is_valid(p)]
         if len(path) != len(path_list):
-            raise RuntimeWarning(
+            ytnapari_log.warning(
                 "Some of the provided paths are not valid yt-napari json files"
             )
     else:
         path_list = [path]
 
     return load_from_json(path_list)
```

### Comparing `yt_napari-0.0.1/src/yt_napari/_tests/conftest.py` & `yt_napari-0.1.0/src/yt_napari/_tests/conftest.py`

 * *Files identical despite different names*

### Comparing `yt_napari-0.0.1/src/yt_napari/_tests/test_model_ingestor.py` & `yt_napari-0.1.0/src/yt_napari/_tests/test_model_ingestor.py`

 * *Files 24% similar despite different names*

```diff
@@ -79,24 +79,80 @@
 def test_layer_domain(domains_to_test):
     for d in domains_to_test.domain_sets:
         layer_domain = _mi.LayerDomain(d.left_edge, d.right_edge, d.resolution)
         assert np.all(layer_domain.center == d.center)
         assert np.all(layer_domain.width == d.width)
 
     # check some instantiation things
-    with pytest.raises(ValueError):
+    with pytest.raises(ValueError, match="length of edge arrays must match"):
         _ = _mi.LayerDomain(d.left_edge, unyt.unyt_array([1, 2], "m"), d.resolution)
 
-    with pytest.raises(ValueError):
+    with pytest.raises(ValueError, match="length of resolution does not"):
         _ = _mi.LayerDomain(d.left_edge, d.right_edge, (10, 12))
 
     ld = _mi.LayerDomain(d.left_edge, d.right_edge, (10,))
     assert len(ld.resolution) == 3
 
 
+def test_layer_domain_dimensionality():
+    # note: the code being tested here could be used to help orient the slices
+    # in 3D but is not currently used.
+    # sets of left_edge, right_edge, center, width, res
+    le = unyt.unyt_array([1.0, 1.0], "km")
+    re = unyt.unyt_array([2000.0, 2000.0], "m")
+    res = (10, 20)
+    ld = _mi.LayerDomain(le, re, res, n_d=2)
+    assert ld.n_d == 2
+
+    ld.upgrade_to_3D()
+    assert ld.n_d == 3
+    assert len(ld.left_edge) == 3
+    assert ld.left_edge[-1] == 0.0
+    ld.upgrade_to_3D()  # nothing should happen
+
+    ld = _mi.LayerDomain(le, re, res, n_d=2, new_dim_value=0.5)
+    ld.upgrade_to_3D()
+    assert ld.left_edge[2] == unyt.unyt_quantity(0.5, le.units)
+
+    new_val = unyt.unyt_quantity(0.5, "km")
+    ld = _mi.LayerDomain(le, re, res, n_d=2, new_dim_value=new_val)
+    ld.upgrade_to_3D()
+    assert ld.left_edge[2].to("km") == new_val
+
+    ld = _mi.LayerDomain(le, re, res, n_d=2, new_dim_value=new_val, new_dim_axis=0)
+    ld.upgrade_to_3D()
+    assert ld.left_edge[0].to("km") == new_val
+
+
+_test_cases_insert = [
+    (
+        unyt.unyt_array([1.0, 1.0], "km"),
+        unyt.unyt_array(
+            [
+                1000.0,
+            ],
+            "m",
+        ),
+        unyt.unyt_array([1.0, 1.0, 1.0], "km"),
+    ),
+    (
+        unyt.unyt_array([1.0, 1.0], "km"),
+        unyt.unyt_quantity(1000.0, "m"),
+        unyt.unyt_array([1.0, 1.0, 1.0], "km"),
+    ),
+    (unyt.unyt_array([1.0, 1.0], "km"), 0.5, unyt.unyt_array([1.0, 1.0, 0.5], "km")),
+]
+
+
+@pytest.mark.parametrize("x,x2,expected", _test_cases_insert)
+def test_insert_to_unyt_array(x, x2, expected):
+    result = _mi._insert_to_unyt_array(x, x2, 2)
+    assert np.all(result == expected)
+
+
 def test_domain_tracking(domains_to_test):
 
     full_domain = _mi.PhysicalDomainTracker()
     full_domain.update_unit_info(unit="m")
 
     full_domain.update_from_layer(domains_to_test.domain_sets[0])
     for d in domains_to_test.domain_sets[1:]:
@@ -204,7 +260,58 @@
 def test_metadata():
     left_edge = unyt.unyt_array([0, 0, 0], "m")
     right_edge = unyt.unyt_array([1, 1, 1], "m")
     layer_domain = _mi.LayerDomain(left_edge, right_edge, (100, 100, 100))
     fake_data = np.ones((10, 10))
     md = _mi.create_metadata_dict(fake_data, layer_domain, True, a="a")
     assert isinstance(md, dict)
+
+
+def test_ref_layer_selection(domains_to_test):
+    # assemble some fake layer tuples
+    im_type = "image"
+
+    spatial_layer_list = []
+    for d in domains_to_test.domain_sets:
+        layer_domain = _mi.LayerDomain(d.left_edge, d.right_edge, d.resolution)
+        im = np.random.random(d.resolution)
+        spatial_layer_list.append((im, {}, im_type, layer_domain))
+
+    # add another small volume layer
+    le = unyt.unyt_array([0.1, 0.1, 0.1], "m")
+    re = unyt.unyt_array([0.2, 0.2, 0.2], "m")
+    res = (3, 4, 5)
+    small_vol_domain = _mi.LayerDomain(le, re, resolution=res)
+    im = np.random.random(res)
+    spatial_layer_list.append((im, {}, im_type, small_vol_domain))
+
+    first_ref = _mi._choose_ref_layer(spatial_layer_list, method="first_in_list")
+    expected_ref = spatial_layer_list[0][3]
+    assert np.all(first_ref.left_edge == expected_ref.left_edge)
+    assert np.all(first_ref.right_edge == expected_ref.right_edge)
+
+    smal_ref = _mi._choose_ref_layer(spatial_layer_list, method="smallest_volume")
+    assert np.all(small_vol_domain.left_edge == smal_ref.left_edge)
+    assert np.all(small_vol_domain.right_edge == smal_ref.right_edge)
+
+    with pytest.raises(ValueError, match="method must be one of"):
+        _ = _mi._choose_ref_layer(spatial_layer_list, method="not_a_method")
+
+
+def test_2d_3d_mix():
+
+    le = unyt.unyt_array([1.0, 1.0, 1.0], "km")
+    re = unyt.unyt_array([2000.0, 2000.0, 2000.0], "m")
+    res = (10, 20, 15)
+    layer_3d = _mi.LayerDomain(le, re, res)
+    ref = _mi.ReferenceLayer(layer_3d)
+
+    le = unyt.unyt_array([1, 1], "km")
+    re = unyt.unyt_array([2000.0, 2000.0], "m")
+    res = (10, 20)
+    layer_2d = _mi.LayerDomain(
+        le, re, res, n_d=2, new_dim_value=unyt.unyt_quantity(1, "km")
+    )
+
+    sp_layer = (np.random.random(res), {}, "testname", layer_2d)
+    new_layer_2d = ref.align_sanitize_layer(sp_layer)
+    assert "scale" not in new_layer_2d[1]  # no scale when it is all 1
```

### Comparing `yt_napari-0.0.1/src/yt_napari/_tests/test_reader.py` & `yt_napari-0.1.0/src/yt_napari/_tests/test_reader.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,39 +2,38 @@
 
 import numpy as np
 import pytest
 import yt
 
 from yt_napari import napari_get_reader
 
-# the following should be a valid json, need to add some functionality to
-# test infrastructure for loading an actual dataset... as is, this requires
-# the IsolatedGalaxy file so will only pass locally.
 valid_jdict = {
-    "$schema": "yt-napari_0.0.1.json",
+    "$schema": "yt-napari_0.1.0.json",
     "data": [
         {
             "filename": None,
-            "selections": [
-                {
-                    "fields": [
-                        {
-                            "field_type": "gas",
-                            "field_name": "density",
-                            "take_log": False,
-                        },
-                        {
-                            "field_type": "gas",
-                            "field_name": "temperature",
-                            "take_log": True,
-                        },
-                    ],
-                    "resolution": [50, 50, 50],
-                }
-            ],
+            "selections": {
+                "regions": [
+                    {
+                        "fields": [
+                            {
+                                "field_type": "gas",
+                                "field_name": "density",
+                                "take_log": False,
+                            },
+                            {
+                                "field_type": "gas",
+                                "field_name": "temperature",
+                                "take_log": True,
+                            },
+                        ],
+                        "resolution": [50, 50, 50],
+                    }
+                ]
+            },
             "edge_units": "Mpc",
         }
     ],
 }
 
 
 @pytest.fixture
@@ -89,15 +88,15 @@
     assert "temperature" in layer_data_list[1][1]["name"]
 
     layer_data_list_2 = reader([json_file_fixture])
     layer_tuple_2 = layer_data_list_2[0]
     assert np.all(layer_tuple_2[0] == layer_tuple[0])
 
 
-def test_invalid_schema(tmp_path, json_file_fixture):
+def test_invalid_schema(tmp_path, json_file_fixture, caplog):
 
     # test invalid schema
     with open(json_file_fixture) as jhandle:
         jdict = json.load(jhandle)
 
     # check that invlaid schema does not return a reader
     jdict["$schema"] = "unsupported_schema.json"
@@ -106,14 +105,14 @@
         json.dump(jdict, fp)
     reader = napari_get_reader(json_file)
     assert reader is None
 
     # test that including one invalid raises a warning
     jpaths = [json_file_fixture, json_file]
     reader = napari_get_reader(jpaths)  # should succeed
-    with pytest.raises(RuntimeWarning):
-        _ = reader(jpaths)
+    _ = reader(jpaths)
+    assert "Some of the provided paths" in caplog.text
 
 
 def test_get_reader_pass():
     reader = napari_get_reader("fake.file")
     assert reader is None
```

### Comparing `yt_napari-0.0.1/src/yt_napari/_tests/test_schema_manager.py` & `yt_napari-0.1.0/src/yt_napari/_tests/test_schema_manager.py`

 * *Files 11% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
     # test explicity version
     expected_file = get_expected(pfx, "2.0.0")
     m.write_new_schema("any old string", version="2.0.0")
     assert expected_file.is_file()
 
     # should error without override
-    with pytest.raises(Exception):
+    with pytest.raises(FileExistsError, match="provide overwrite_version"):
         m.write_new_schema("any old string", version="2.0.0")
 
     # provide override, should have new text
     new_text = "different string"
     m.write_new_schema(new_text, version="2.0.0", overwrite_version=True)
     with open(expected_file) as f:
         assert "different string" in f.read()
```

### Comparing `yt_napari-0.0.1/src/yt_napari/_tests/test_viewer.py` & `yt_napari-0.1.0/src/yt_napari/_tests/test_viewer.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,68 +1,67 @@
 import numpy as np
 import pytest
-import yt
 from napari.layers import Layer
 from napari.layers.utils._link_layers import get_linked_layers
+from yt import testing as yt_testing
 
 from yt_napari.viewer import Scene
 
 
 @pytest.fixture
 def yt_ds():
-    return yt.testing.fake_amr_ds(fields=("density", "mass"), units=("kg/m**3", "kg"))
+    return yt_testing.fake_amr_ds(fields=("density", "mass"), units=("kg/m**3", "kg"))
 
 
-def test_viewer(make_napari_viewer, yt_ds):
+def test_viewer(make_napari_viewer, yt_ds, caplog):
 
     # make_napari_viewer is a pytest fixture. It takes any keyword arguments
     # that napari.Viewer() takes. The fixture takes care of teardown, do **not**
     # explicitly close it!
     viewer = make_napari_viewer()
 
     # also note that building the viewer takes a few seconds so all tests here
     # are in a single function.
 
     ####################
     # test add_to_viewer
     sc = Scene()
     res = (10, 10, 10)
-    sc.add_to_viewer(viewer, yt_ds, ("gas", "density"), resolution=res)
+    sc.add_region(viewer, yt_ds, ("gas", "density"), resolution=res)
 
     expected_layers = 1
     assert len(viewer.layers) == expected_layers
 
-    with pytest.warns(RuntimeWarning):
-        sc.add_to_viewer(
-            viewer, yt_ds, ("gas", "density"), translate=10, resolution=res
-        )
-    with pytest.warns(RuntimeWarning):
-        sc.add_to_viewer(viewer, yt_ds, ("gas", "density"), scale=10, resolution=res)
+    sc.add_region(viewer, yt_ds, ("gas", "density"), translate=10, resolution=res)
+    assert "translate is calculated internally" in caplog.text
+    sc.add_region(viewer, yt_ds, ("gas", "density"), scale=10, resolution=res)
+    assert "scale is calculated internally" in caplog.text
+
     expected_layers += 2  # the above will add layers!
     assert len(viewer.layers) == expected_layers
 
-    sc.add_to_viewer(viewer, yt_ds, ("gas", "density"), resolution=res)
+    sc.add_region(viewer, yt_ds, ("gas", "density"), resolution=res)
     expected_layers += 1
     assert len(viewer.layers) == expected_layers
 
     # build a new scene so it builds from prior
     sc = Scene()
-    sc.add_to_viewer(viewer, yt_ds, ("gas", "density"), resolution=res)
+    sc.add_region(viewer, yt_ds, ("gas", "density"))
     expected_layers += 1
     assert len(viewer.layers) == expected_layers
 
 
 def test_sanitize_layers(make_napari_viewer, yt_ds):
 
     viewer = make_napari_viewer()
 
     sc = Scene()
     res = (10, 10, 10)
-    sc.add_to_viewer(viewer, yt_ds, ("gas", "density"), name="layer0", resolution=res)
-    sc.add_to_viewer(viewer, yt_ds, ("gas", "mass"), name="layer1", resolution=res)
+    sc.add_region(viewer, yt_ds, ("gas", "density"), name="layer0", resolution=res)
+    sc.add_region(viewer, yt_ds, ("gas", "mass"), name="layer1", resolution=res)
 
     clean_layers = sc._sanitize_layers(["layer0", "layer1"], viewer.layers)
     assert len(clean_layers) == 2
     assert all([isinstance(i, Layer) for i in clean_layers])
 
     clean_layers = sc._sanitize_layers([viewer.layers["layer1"]])
     assert len(clean_layers) == 1
@@ -87,16 +86,16 @@
 
 def test_get_data_range(make_napari_viewer, yt_ds):
 
     viewer = make_napari_viewer()
 
     sc = Scene()
     res = (10, 10, 10)
-    sc.add_to_viewer(viewer, yt_ds, ("gas", "density"), name="layer0", resolution=res)
-    sc.add_to_viewer(viewer, yt_ds, ("gas", "density"), name="layer1", resolution=res)
+    sc.add_region(viewer, yt_ds, ("gas", "density"), name="layer0", resolution=res)
+    sc.add_region(viewer, yt_ds, ("gas", "density"), name="layer1", resolution=res)
     expected = (viewer.layers[0].data.min(), viewer.layers[0].data.max())
     actual = sc.get_data_range(viewer.layers)
     assert np.allclose(actual, expected)
 
     # check that a non yt-napari layer gets picked up too
     expected = (expected[0], expected[1] + 100.0)
     viewer.add_image(np.full((10, 10, 10), expected[1]))
@@ -106,28 +105,48 @@
 
 def test_cross_layer_features(make_napari_viewer, yt_ds):
 
     viewer = make_napari_viewer()
 
     sc = Scene()
     res = (10, 10, 10)
-    sc.add_to_viewer(viewer, yt_ds, ("gas", "density"), name="layer0", resolution=res)
-    sc.add_to_viewer(viewer, yt_ds, ("gas", "density"), name="layer1", resolution=res)
+    sc.add_region(viewer, yt_ds, ("gas", "density"), name="layer0", resolution=res)
+    sc.add_region(viewer, yt_ds, ("gas", "density"), name="layer1", resolution=res)
 
     sc.set_across_layers(viewer.layers, "colormap", "viridis")
     assert all([layer.colormap == "viridis"] for layer in viewer.layers)
 
     expected = (viewer.layers[0].data.min(), viewer.layers[0].data.max())
     sc.normalize_color_limits(viewer.layers)
     for layer in viewer.layers:
         assert np.allclose(layer.contrast_limits, expected)
 
-    sc.add_to_viewer(
+    sc.add_region(
         viewer,
         yt_ds,
         ("gas", "density"),
         name="layer2",
         link_to="layer1",
         resolution=res,
     )
     linked = get_linked_layers(viewer.layers["layer2"])
     assert viewer.layers["layer1"] in linked
+
+
+def test_viewer_deprecations(make_napari_viewer, yt_ds):
+    viewer = make_napari_viewer()
+
+    sc = Scene()
+    res = (10, 10, 10)
+
+    # remove in v0.2.0 or higher
+    with pytest.deprecated_call():
+        sc.add_to_viewer(viewer, yt_ds, ("gas", "density"), resolution=res)
+
+
+def test_viewer_slices(make_napari_viewer, yt_ds):
+    viewer = make_napari_viewer()
+    sc = Scene()
+    res = (50, 50)
+    sc.add_slice(viewer, yt_ds, "x", ("gas", "density"), resolution=res)
+
+    assert len(viewer.layers) == 1
```

### Comparing `yt_napari-0.0.1/src/yt_napari/napari.yaml` & `yt_napari-0.1.0/src/yt_napari/napari.yaml`

 * *Files identical despite different names*

### Comparing `yt_napari-0.0.1/src/yt_napari/schemas/_manager.py` & `yt_napari-0.1.0/src/yt_napari/schemas/_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 from collections import defaultdict
 from os import PathLike
 from pathlib import PosixPath
 from typing import DefaultDict, Optional, Set, Union
 
 from packaging.version import Version
 
+from yt_napari.logging import ytnapari_log
+
 
 class Manager:
     # This is a simple on-disk schema version management class meant for
     # tracking development of new schema files.
     default_schema_prefix = "yt-napari"
 
     def __init__(self, schema_db: Union[str, PosixPath]):
@@ -112,15 +114,15 @@
             and overwrite_version is False
         ):
             raise FileExistsError(
                 f"provide overwrite_version=True to overwrite {filename}"
             )
 
         # write out json to filename
-        print(f"writing new schema {filename}")
+        ytnapari_log.info(f"writing new schema {filename}")
         with open(filename, "w") as f:
             f.write(schema_json)
 
     def update_docs(
         self, source: Union[str, PathLike], schema_prefix: Optional[str] = None
     ):
         """
@@ -143,14 +145,15 @@
         >>> m.update_docs(source_dir)
 
         """
 
         schema_prefix = self._validate_prefix(schema_prefix)
         source_dir = PosixPath(source)
         source_static = source_dir.joinpath("_static")
+        ytnapari_log.info(f"Updating the schema files in {source_static}")
 
         # copy all json files to docs/_static/
         copied_files = []
         for fi in self.schema_files:
             if schema_prefix in fi.name:
                 target = source_static.joinpath(fi.name)
                 shutil.copy2(fi, target)
```

### Comparing `yt_napari-0.0.1/src/yt_napari/schemas/yt-napari_0.0.1.json` & `yt_napari-0.1.0/src/yt_napari/schemas/yt-napari_0.0.1.json`

 * *Files identical despite different names*

### Comparing `yt_napari-0.0.1/src/yt_napari/viewer.py` & `yt_napari-0.1.0/src/yt_napari/viewer.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,32 +2,39 @@
 from typing import Any, List, Optional, Set, Tuple, Union
 
 import numpy as np
 from napari import Viewer
 from napari.components.layerlist import LayerList
 from napari.layers import Layer
 from napari.layers.utils._link_layers import get_linked_layers
-from unyt import unyt_array
+from unyt import unyt_array, unyt_quantity
 
 import yt_napari._model_ingestor as _mi
+from yt_napari.logging import ytnapari_log
+
+
+def _check_for_reference_layer(
+    napari_layer_list: LayerList,
+) -> Optional[_mi.ReferenceLayer]:
+    # check the napari viewer layer list for an existing reference layer
+    for layer in napari_layer_list:
+        if "_yt_napari_layer" in layer.metadata:
+            if layer.metadata["_reference_layer"] is not None:
+                return layer.metadata["_reference_layer"]
+    return None
 
 
 class Scene:
     def __init__(self, reference_layer: Optional[_mi.ReferenceLayer] = None):
         self._reference_layer = reference_layer
 
     def _check_for_reference_layer(
         self, current_layers: list
     ) -> Optional[_mi.ReferenceLayer]:
-        # check the napari viewer layer list for an existing reference layer
-        for layer in current_layers:
-            if "_yt_napari_layer" in layer.metadata:
-                if layer.metadata["_reference_layer"] is not None:
-                    return layer.metadata["_reference_layer"]
-        return None
+        return _check_for_reference_layer(current_layers)
 
     def _get_reference_layer(
         self,
         layer_list: List[Layer],
         default_if_missing: Optional[_mi.LayerDomain] = None,
     ):
         if len(layer_list) == 0:
@@ -40,29 +47,85 @@
             if ref_layer is None:
                 # still None, use this layer:
                 layer_domain = default_if_missing
                 ref_layer = _mi.ReferenceLayer(layer_domain)
             self._reference_layer = ref_layer
         return self._reference_layer
 
-    def add_to_viewer(
+    def _add_to_scene(
+        self,
+        viewer: Viewer,
+        data,
+        layer_domain,
+        field,
+        take_log,
+        colormap=None,
+        link_to=None,
+        **kwargs,
+    ):
+        # adds any new data to the viewer
+
+        if colormap is None:
+            colormap = "viridis"
+
+        # initialize the spatial layer then sanitize it
+        splayer = (data, {}, "image", layer_domain)
+        ref_layer = self._get_reference_layer(
+            viewer.layers, default_if_missing=layer_domain
+        )
+        _, im_kwargs, _ = ref_layer.align_sanitize_layer(splayer)
+
+        # extract the translate and scale values
+        tr = im_kwargs.get("translate", None)
+        sc = im_kwargs.get("scale", None)
+        # check that the user has not supplied translate or scale separately
+        for attr in ["translate", "scale"]:
+            if attr in kwargs:
+                msg = f"{attr} is calculated internally, ignoring provided value"
+                ytnapari_log.warning(msg)
+                _ = kwargs.pop(attr)
+
+        # set the display name
+        if "name" in kwargs:
+            fname = kwargs.pop("name")
+        else:
+            fname = f"{field[0]}_{field[1]}"
+
+        md = _mi.create_metadata_dict(
+            data, layer_domain, take_log, reference_layer=ref_layer
+        )
+        viewer.add_image(
+            data,
+            name=fname,
+            translate=tr,
+            scale=sc,
+            metadata=md,
+            colormap=colormap,
+            **kwargs,
+        )
+
+        if link_to is not None:
+            # link the one we just added with the provided layer
+            viewer.layers.link_layers([link_to, viewer.layers[-1]])
+
+    def add_region(
         self,
         viewer: Viewer,
         ds,
         field: Tuple[str, str],
         resolution: Optional[Tuple[int, int, int]] = None,
         left_edge: Optional[unyt_array] = None,
         right_edge: Optional[unyt_array] = None,
         take_log: Optional[bool] = None,
         colormap: Optional[str] = None,
         link_to: Optional[Union[str, Layer]] = None,
         **kwargs,
     ):
         """
-        create a uniform sampling of ds and add it to the napari viewer
+        uniformly sample a region from a yt dataset and add it to a viewer
 
         Parameters
         ----------
         viewer: napari.Viewer
             the active napari viewer
         ds
             the yt dataset to sample
@@ -89,86 +152,174 @@
 
         >>> import napari
         >>> import yt
         >>> from yt_napari.viewer import Scene
         >>> viewer = napari.Viewer()
         >>> ds = yt.load_sample("IsolatedGalaxy")
         >>> yt_scene = Scene()
-        >>> yt_scene.add_to_viewer(viewer, ds, ("enzo", "Temperature"))
+        >>> yt_scene.add_region(viewer, ds, ("enzo", "Temperature"))
 
         """
 
         # set defaults
         if left_edge is None:
             left_edge = ds.domain_left_edge
         if right_edge is None:
             right_edge = ds.domain_right_edge
         if resolution is None:
             resolution = (400, 400, 400)
         if take_log is None:
             take_log = ds._get_field_info(field).take_log
-        if colormap is None:
-            # TO DO: make this a per-field default based on yt info?
-            # or use ytcfg.get("yt", "default_colormap") ?
-            # would need to check against available cmaps in napari
-            colormap = "viridis"
 
         # add the bounds of this new layer
         layer_domain = _mi.LayerDomain(left_edge, right_edge, resolution)
-        ref_layer = self._get_reference_layer(
-            viewer.layers, default_if_missing=layer_domain
-        )
 
         # create the fixed resolution buffer
         frb = ds.r[
             left_edge[0] : right_edge[0] : complex(0, resolution[0]),  # noqa: E203
             left_edge[1] : right_edge[1] : complex(0, resolution[1]),  # noqa: E203
             left_edge[2] : right_edge[2] : complex(0, resolution[2]),  # noqa: E203
         ]
         data = frb[field]
         if take_log:
             data = np.log10(data)
 
-        # initialize the spatial layer then sanitize it
-        splayer = (data, {}, "image", layer_domain)
-        _, im_kwargs, _ = ref_layer.align_sanitize_layer(splayer)
+        self._add_to_scene(
+            viewer,
+            data,
+            layer_domain,
+            field,
+            take_log,
+            colormap=colormap,
+            link_to=link_to,
+            **kwargs,
+        )
 
-        # extract the translate and scale values
-        tr = im_kwargs.get("translate", None)
-        sc = im_kwargs.get("scale", None)
-        # check that the user has not supplied translate or scale separately
-        for attr in ["translate", "scale"]:
-            if attr in kwargs:
-                msg = f"{attr} is calculated internally, ignoring provided value"
-                warnings.warn(msg, RuntimeWarning)
-                _ = kwargs.pop(attr)
+    def add_to_viewer(
+        self,
+        viewer: Viewer,
+        ds,
+        field: Tuple[str, str],
+        resolution: Optional[Tuple[int, int, int]] = None,
+        left_edge: Optional[unyt_array] = None,
+        right_edge: Optional[unyt_array] = None,
+        take_log: Optional[bool] = None,
+        colormap: Optional[str] = None,
+        link_to: Optional[Union[str, Layer]] = None,
+        **kwargs,
+    ):
+        """deprecated, will be removed in v>0.1.0. use add_region"""
+        msg = (
+            "add_to_viewer has been deprecated, use add_region "
+            "instead. add_to_viewer will be removed in v>0.1.0"
+        )
+        warnings.warn(msg, DeprecationWarning, stacklevel=2)
+        self.add_region(
+            viewer,
+            ds,
+            field,
+            resolution=resolution,
+            left_edge=left_edge,
+            right_edge=right_edge,
+            take_log=take_log,
+            colormap=colormap,
+            link_to=link_to,
+            **kwargs,
+        )
 
-        # set the display name
-        if "name" in kwargs:
-            fname = kwargs.pop("name")
-        else:
-            fname = f"{field[0]}_{field[1]}"
+    def add_slice(
+        self,
+        viewer: Viewer,
+        ds,
+        normal: Union[str, int],
+        field: Tuple[str, str],
+        center: Optional[unyt_array] = None,
+        resolution: Optional[Tuple[int, int]] = (400, 400),
+        width: Optional[unyt_quantity] = None,
+        height: Optional[unyt_quantity] = None,
+        take_log: Optional[bool] = None,
+        periodic: Optional[bool] = False,
+        colormap: Optional[str] = None,
+        link_to: Optional[Union[str, Layer]] = None,
+        **kwargs,
+    ):
+        """
+        sample an orthogonal slice from a yt dataset and add it to a viewer
 
-        md = _mi.create_metadata_dict(
-            data, layer_domain, take_log, reference_layer=ref_layer
+        Parameters
+        ----------
+        viewer: napari.Viewer
+            the active napari viewer
+        ds
+            the yt dataset to sample
+        normal: str, int
+            the normal axis of the slice, either an axis name or number
+        field: Tuple[str, str]
+            the field tuple to sample  e.g., ('enzo', 'Density')
+        center: unyt_array
+            the center of the slice (3D)
+        width: unyt_quantity
+            the width of the slice
+        height: unyt_quantity
+            the height of the slice
+        resolution: Tuple[int, int]
+            the sampling resolution in each dimension, e.g., (400, 400)
+        take_log : Optional[bool]
+            if True, will take the log of the extracted data. Defaults to the
+            default behavior for the field set by ds.
+        periodic: Optional[bool]
+            use periodic bounds for the slice, default False
+        colormap : Optional[str]
+            the color map to use, default is "viridis"
+        link_to : Optional[Union[str, Layer]]
+            specify a layer to which the new layer should link
+        **kwargs :
+            any keyword argument accepted by Viewer.add_image()
+
+        Examples
+        --------
+
+        >>> import napari
+        >>> import yt
+        >>> from yt_napari.viewer import Scene
+        >>> viewer = napari.Viewer()
+        >>> ds = yt.load_sample("IsolatedGalaxy")
+        >>> yt_scene = Scene()
+        >>> yt_scene.add_slice(viewer, ds, "x", ("enzo", "Temperature"))
+
+        """
+
+        if take_log is None:
+            take_log = ds._get_field_info(field).take_log
+
+        frb, layer_domain = _mi._process_slice(
+            ds,
+            normal,
+            center=center,
+            width=width,
+            height=height,
+            resolution=resolution,
+            periodic=periodic,
         )
-        viewer.add_image(
+
+        data = frb[field]
+        if take_log:
+            data = np.log10(data)
+
+        self._add_to_scene(
+            viewer,
             data,
-            name=fname,
-            translate=tr,
-            scale=sc,
-            metadata=md,
+            layer_domain,
+            field,
+            take_log,
             colormap=colormap,
+            link_to=link_to,
             **kwargs,
         )
 
-        if link_to is not None:
-            # link the one we just added with the provided layer
-            viewer.layers.link_layers([link_to, viewer.layers[-1]])
-
     def normalize_color_limits(
         self,
         layers: List[Union[str, Layer]],
         layer_list: Optional[LayerList] = None,
         check_linked: Optional[bool] = True,
     ):
         """
@@ -199,24 +350,24 @@
         >>> import yt
         >>> from yt_napari.viewer import Scene
         >>> viewer = napari.Viewer()
         >>> ds = yt.load_sample("IsolatedGalaxy")
         >>> yt_scene = Scene()
         >>> le = ds.domain_center - ds.arr([10, 10, 10], 'kpc')
         >>> re = ds.domain_center + ds.arr([10, 10, 10], 'kpc')
-        >>> yt_scene.add_to_viewer(viewer,
+        >>> yt_scene.add_region(viewer,
         >>>                        ds,
         >>>                        ("enzo", "Density"),
         >>>                        left_edge = le,
         >>>                        right_edge = re,
         >>>                        resolution=(600, 600, 600),
         >>>                        name="Density_1")
         >>> le = ds.domain_center + ds.arr([10, 10, 10], 'kpc')
         >>> re = le + ds.arr([20, 20, 20], 'kpc')
-        >>> yt_scene.add_to_viewer(viewer,
+        >>> yt_scene.add_region(viewer,
         >>>                        ds,
         >>>                        ("enzo", "Density"),
         >>>                        left_edge = le,
         >>>                        right_edge = re,
         >>>                        resolution=(300, 300, 300),
         >>>                        name="Density_2")
         >>> yt_scene.normalize_color_limits(["Density_2", "Density_1"], viewer.layers)
@@ -345,15 +496,15 @@
 
         >>> import napari
         >>> import yt
         >>> from yt_napari.viewer import Scene
         >>> viewer = napari.Viewer()
         >>> ds = yt.load_sample("IsolatedGalaxy")
         >>> yt_scene = Scene()
-        >>> yt_scene.add_to_viewer(viewer, ds, ("enzo", "Temperature"))
+        >>> yt_scene.add_region(viewer, ds, ("enzo", "Temperature"))
         >>> yt_scene.get_data_range(viewer.layers)
         (3.2446250040130398, 5.003147905498429)
 
         """
 
         clean_layers = self._sanitize_layers(layers, layer_list, check_linked)
```

### Comparing `yt_napari-0.0.1/src/yt_napari.egg-info/PKG-INFO` & `yt_napari-0.1.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,32 @@
 Metadata-Version: 2.1
-Name: yt-napari
-Version: 0.0.1
+Name: yt_napari
+Version: 0.1.0
 Summary: A napari plugin for loading data from yt
 Home-page: https://github.com/data-exp-lab/yt-napari
 Author: Chris Havlin
 Author-email: chris.havlin@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/data-exp-lab/yt-napari/issues
 Project-URL: Documentation, https://github.com/data-exp-lab/yt-napari#README.md
 Project-URL: Source Code, https://github.com/data-exp-lab/yt-napari
 Project-URL: User Support, https://github.com/data-exp-lab/yt-napari/issues
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: napari
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Testing
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # yt-napari
 
 [![License](https://img.shields.io/pypi/l/yt-napari.svg?color=green)](https://github.com/data-exp-lab/yt-napari/raw/main/LICENSE)
 [![PyPI](https://img.shields.io/pypi/v/yt-napari.svg?color=green)](https://pypi.org/project/yt-napari)
@@ -100,62 +98,62 @@
 ds = yt.load("IsolatedGalaxy/galaxy0030/galaxy0030")
 yt_scene = Scene()
 
 left_edge = ds.domain_center - ds.arr([40, 40, 40], 'kpc')
 right_edge = ds.domain_center + ds.arr([40, 40, 40], 'kpc')
 res = (600, 600, 600)
 
-yt_scene.add_to_viewer(viewer,
-                       ds,
-                       ("enzo", "Temperature"),
-                       left_edge = left_edge,
-                       right_edge = right_edge,
-                       resolution = res)
-
-yt_scene.add_to_viewer(viewer,
-                       ds,
-                       ("enzo", "Density"),
-                       left_edge = left_edge,
-                       right_edge = right_edge,
-                       resolution = res)
+yt_scene.add_region(viewer,
+                    ds,
+                    ("enzo", "Temperature"),
+                    left_edge=left_edge,
+                    right_edge=right_edge,
+                    resolution=res)
+
+yt_scene.add_region(viewer,
+                    ds,
+                    ("enzo", "Density"),
+                    left_edge=left_edge,
+                    right_edge=right_edge,
+                    resolution=res)
 
 nbscreenshot(viewer)
 ```
 
  ![Loading a subset of a yt dataset in napari from a Jupyter notebook](./assets/images/readme_ex_001.png)
 
-`yt_scene.add_to_viewer` accepts any of the keyword arguments allowed by `viewer.add_image`. See the full documentation (!!!NEED LINK!!!) for more examples, including additional helper methods for linking layer appearance.
+`yt_scene.add_to_viewer` accepts any of the keyword arguments allowed by `viewer.add_image`. See the full documentation (https://yt-napari.readthedocs.io/en/stable/) for more examples, including additional helper methods for linking layer appearance.
 
 ### loading a selection from a yt dataset interactively
 
-`yt-napari` provides a two ways to sample a yt dataset and load in an image layer into a Napari viewer: the yt Reader plugin and json file specification.
+`yt-napari` provides two ways to sample a yt dataset and load in an image layer into a Napari viewer: the yt Reader plugin and json file specification.
 
 #### using the yt Reader plugin
 
-To use the yt Reader plugin, click on `Plugins -> yt-napari: yt Reader`. Select a file, specify a field type and field, set the region to sample and then simply click "Load":
+To use the yt Reader plugin, click on `Plugins -> yt-napari: yt Reader`. From there, add a region or slice selector then specify a field type and field and bounds to sample  between and then simply click "Load":
 
 ![Loading a subset of a yt dataset from the napari viewer](./assets/images/readme_ex_003_gui_reader.gif)
 
-To load a different field or section, adjust the values and click "Load" again.
+You can add multiple selections and load them all at once or adjust values and click "Load" again.
 
 #### using a json file and schema
 
 `yt-napari` also provides the ability to load json that contain specifications for loading a file. Properly formatted files can be loaded from the napari GUI as you would load any image file (`File->Open`). The json file describes the selection process for a dataset as described by a json-schema. The following json file results in similar layers as the above examples:
 
 
 ```json
 {"$schema": "https://raw.githubusercontent.com/data-exp-lab/yt-napari/main/src/yt_napari/schemas/yt-napari_0.0.1.json",
  "data": [{"filename": "IsolatedGalaxy/galaxy0030/galaxy0030",
-           "selections": [{
+           "selections": {"regions": [{
                             "fields": [{"field_name": "Temperature", "field_type": "enzo", "take_log": true},
                                        {"field_name": "Density", "field_type": "enzo", "take_log": true}],
                             "left_edge": [460.0, 460.0, 460.0],
                             "right_edge": [560.0, 560.0, 560.0],
                             "resolution": [600, 600, 600]
-                          }],
+                          }]},
            "edge_units": "kpc"
          }]
 }
 ```
 
 To help in filling out a json file, it is recommended that you use an editor capable of parsing a json schema and displaying hints. For example, in vscode, you will see field suggestions after specifying the `yt-napari` schema:
 
@@ -202,38 +200,60 @@
 This will update the `rst` files in `docs/source/` with the latest docstrings in `yt_napari`. Next, build the html documentation with
 
     make html
 
 
 ### updating the pydantic models and schema
 
-Updates to the pydantic models should be accompanied by updates to the json schema. There are a number of utilities to help automate the management of schema.
+The schema versioning follows a `major.minor.micro` versioning pattern that matches the yt-napari versioning. Each yt-napari release should have an accompanying updated schema file, even if the  contents of the schema file have not changed. On-disk schema are stored in  `src/yt_napari/schemas/`, with copies in the documentation at `docs/_static`.
 
-The schema versioning follows a `major.minor.micro` versioning pattern and yt-napari schema are stored in `src/yt_napari/schemas/`. When changing the model, you can store a new schema from a python shell with:
+There are a number of utilities to help automate the management of schema in `repo_utilities/`. The easiest way to use these utitities is with `taskipy` from the command line. To list available scripts:
 
+```commandline
+task --list
+```
+
+Before a release, run
+
+```commandline
+task validate_release vX.X.X
+```
 
-    from yt_napari._data_model import _store_schema
-    _store_schema()
+where `vX.X.X` is the version of the upcoming release. This script will run through some checks that ensure:
+* the on-disk schema matches the schema generated by the pydantic model
+* the schema files in the documentation match the schema files in the package
 
-And the current version of the primary pydantic model, `yt_napari._data_model.InputModel`, will be exported to a new json schema file. By default, the micro version number will be incremented. To increment the major or minor version number, you can supply any of the keyword arguments described in the `write_new_schema` method of the `yt_napari.schemas._mananager.Manager` class.
+If any of the checks fail, you will be advised to update the schema using `update_schema_docs`. If you
+run without providing a version:
 
-After updating or adding a new schema, the docs also need to be updated. To do that, run
+```commandline
+task update_schema_docs
+```
 
-    python repo_utilities/update_schema_docs.py
-    make clean && make html
+It will simply copy over the existing on-disk schema files to the documentation. If you run with a version:
+
+```commandline
+task update_schema_docs vX.X.X
+```
+It will write a schema file for the current pydantic model, overwriting any on-disk schema files for
+the provided version.
 
 ## License
 
 Distributed under the terms of the [BSD-3] license,
 "yt-napari" is free and open source software
 
 ## Issues
 
 If you encounter any problems, please [file an issue] along with a detailed description.
 
+## Funding
+
+The yt-napari plugin project was funded with support from the Chan Zuckerberg Initiative through the napari Plugin Accelerator Grants project, [Enabling Access To Multi-resolution Data](https://chanzuckerberg.com/science/programs-resources/imaging/napari/enabling-access-to-multi-resolution-data/).
+
 ----------------------------------
 
 This [napari] plugin was generated with [Cookiecutter] using [@napari]'s [cookiecutter-napari-plugin] template.
 
 <!--
 Don't miss the full getting started guide to set up your new package:
 https://github.com/napari/cookiecutter-napari-plugin#getting-started
@@ -257,9 +277,7 @@
 [file an issue]: https://github.com/data-exp-lab/yt-napari/issues
 
 [napari]: https://github.com/napari/napari
 [tox]: https://tox.readthedocs.io/en/latest/
 [pip]: https://pypi.org/project/pip/
 [PyPI]: https://pypi.org/
 [yt]: https://yt-project.org/
-
-
```

### Comparing `yt_napari-0.0.1/src/yt_napari.egg-info/SOURCES.txt` & `yt_napari-0.1.0/src/yt_napari.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -1,40 +1,54 @@
 .gitignore
+HISTORY.md
 LICENSE
 MANIFEST.in
 README.md
+pyproject.toml
 requirements.txt
 setup.cfg
 setup.py
 .github/ISSUE_TEMPLATE/bug-report.md
 .github/ISSUE_TEMPLATE/feedback-and-discussion.md
 .github/workflows/check_build.yml
 .github/workflows/check_manifest.yml
 .github/workflows/style_checks.yml
 .github/workflows/test_and_deploy.yml
+.github/workflows/weekly_build.yml
 src/yt_napari/__init__.py
 src/yt_napari/_data_model.py
+src/yt_napari/_ds_cache.py
 src/yt_napari/_gui_utilities.py
 src/yt_napari/_model_ingestor.py
 src/yt_napari/_reader.py
+src/yt_napari/_special_loaders.py
 src/yt_napari/_version.py
 src/yt_napari/_widget_reader.py
+src/yt_napari/config.py
+src/yt_napari/logging.py
 src/yt_napari/napari.yaml
 src/yt_napari/viewer.py
 src/yt_napari.egg-info/PKG-INFO
 src/yt_napari.egg-info/SOURCES.txt
 src/yt_napari.egg-info/dependency_links.txt
 src/yt_napari.egg-info/entry_points.txt
 src/yt_napari.egg-info/requires.txt
 src/yt_napari.egg-info/top_level.txt
 src/yt_napari/_tests/__init__.py
 src/yt_napari/_tests/_test_json.json
+src/yt_napari/_tests/_test_json_slice.json
 src/yt_napari/_tests/conftest.py
+src/yt_napari/_tests/test_config.py
+src/yt_napari/_tests/test_ds_cache.py
 src/yt_napari/_tests/test_gui_utilities.py
 src/yt_napari/_tests/test_model_ingestor.py
 src/yt_napari/_tests/test_reader.py
 src/yt_napari/_tests/test_schema_manager.py
+src/yt_napari/_tests/test_schema_version_comparisons.py
+src/yt_napari/_tests/test_slices_json.py
 src/yt_napari/_tests/test_viewer.py
 src/yt_napari/_tests/test_widget_reader.py
 src/yt_napari/schemas/__init__.py
 src/yt_napari/schemas/_manager.py
-src/yt_napari/schemas/yt-napari_0.0.1.json
+src/yt_napari/schemas/_version_comparison.py
+src/yt_napari/schemas/yt-napari_0.0.1.json
+src/yt_napari/schemas/yt-napari_0.1.0.json
```

