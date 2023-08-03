# Comparing `tmp/pz-rail-astro-tools-0.0.2.tar.gz` & `tmp/pz-rail-astro-tools-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pz-rail-astro-tools-0.0.2.tar", last modified: Tue Jun 13 19:46:32 2023, max compression
+gzip compressed data, was "pz-rail-astro-tools-0.0.3.tar", last modified: Thu Aug  3 23:28:35 2023, max compression
```

## Comparing `pz-rail-astro-tools-0.0.2.tar` & `pz-rail-astro-tools-0.0.3.tar`

### file list

```diff
@@ -1,51 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:46:32.240157 pz-rail-astro-tools-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-13 19:46:14.000000 pz-rail-astro-tools-0.0.2/.copier-answers.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:46:32.216155 pz-rail-astro-tools-0.0.2/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     3329 2023-06-13 19:46:14.000000 pz-rail-astro-tools-0.0.2/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:46:32.216155 pz-rail-astro-tools-0.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-06-13 19:46:14.000000 pz-rail-astro-tools-0.0.2/.github/workflows/add-issue-to-project-tracker.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-06-13 19:46:14.000000 pz-rail-astro-tools-0.0.2/.github/workflows/linting.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-13 19:46:14.000000 pz-rail-astro-tools-0.0.2/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-06-13 19:46:14.000000 pz-rail-astro-tools-0.0.2/.github/workflows/smoke-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-06-13 19:46:14.000000 pz-rail-astro-tools-0.0.2/.github/workflows/testing-and-coverage.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-06-13 19:46:14.000000 pz-rail-astro-tools-0.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-06-13 19:46:14.000000 pz-rail-astro-tools-0.0.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-13 19:46:14.000000 pz-rail-astro-tools-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-06-13 19:46:32.240157 pz-rail-astro-tools-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-06-13 19:46:14.000000 pz-rail-astro-tools-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-06-13 19:46:14.000000 pz-rail-astro-tools-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 19:46:32.240157 pz-rail-astro-tools-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-13 19:46:14.000000 pz-rail-astro-tools-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:46:32.212155 pz-rail-astro-tools-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:46:32.216155 pz-rail-astro-tools-0.0.2/src/pz_rail_astro_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-06-13 19:46:32.000000 pz-rail-astro-tools-0.0.2/src/pz_rail_astro_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-06-13 19:46:32.000000 pz-rail-astro-tools-0.0.2/src/pz_rail_astro_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 19:46:32.000000 pz-rail-astro-tools-0.0.2/src/pz_rail_astro_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-13 19:46:32.000000 pz-rail-astro-tools-0.0.2/src/pz_rail_astro_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-13 19:46:32.000000 pz-rail-astro-tools-0.0.2/src/pz_rail_astro_tools.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:46:32.212155 pz-rail-astro-tools-0.0.2/src/rail/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:46:32.216155 pz-rail-astro-tools-0.0.2/src/rail/astro_tools/
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-13 19:46:14.000000 pz-rail-astro-tools-0.0.2/src/rail/astro_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-13 19:46:31.000000 pz-rail-astro-tools-0.0.2/src/rail/astro_tools/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:46:32.212155 pz-rail-astro-tools-0.0.2/src/rail/creation/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:46:32.216155 pz-rail-astro-tools-0.0.2/src/rail/creation/degradation/
--rw-r--r--   0 runner    (1001) docker     (123)    11974 2023-06-13 19:46:14.000000 pz-rail-astro-tools-0.0.2/src/rail/creation/degradation/grid_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)    15697 2023-06-13 19:46:14.000000 pz-rail-astro-tools-0.0.2/src/rail/creation/degradation/observing_condition_degrader.py
--rw-r--r--   0 runner    (1001) docker     (123)     4935 2023-06-13 19:46:14.000000 pz-rail-astro-tools-0.0.2/src/rail/creation/degradation/spectroscopic_degraders.py
--rw-r--r--   0 runner    (1001) docker     (123)    22251 2023-06-13 19:46:14.000000 pz-rail-astro-tools-0.0.2/src/rail/creation/degradation/spectroscopic_selections.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:46:32.212155 pz-rail-astro-tools-0.0.2/src/rail/examples_data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:46:32.212155 pz-rail-astro-tools-0.0.2/src/rail/examples_data/creation_data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:46:32.216155 pz-rail-astro-tools-0.0.2/src/rail/examples_data/creation_data/data/
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-13 19:46:14.000000 pz-rail-astro-tools-0.0.2/src/rail/examples_data/creation_data/data/HSC_grid_settings.pkl
--rw-r--r--   0 runner    (1001) docker     (123) 13823712 2023-06-13 19:46:14.000000 pz-rail-astro-tools-0.0.2/src/rail/examples_data/creation_data/data/hsc_ratios_and_specz.hdf5
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:46:32.240157 pz-rail-astro-tools-0.0.2/src/rail/examples_data/creation_data/data/survey_conditions/
--rw-r--r--   0 runner    (1001) docker     (123)  1581120 2023-06-13 19:46:14.000000 pz-rail-astro-tools-0.0.2/src/rail/examples_data/creation_data/data/survey_conditions/DC2-dr6-galcounts-i20-i25.3-nside-128.fits
--rw-r--r--   0 runner    (1001) docker     (123)  1581120 2023-06-13 19:46:14.000000 pz-rail-astro-tools-0.0.2/src/rail/examples_data/creation_data/data/survey_conditions/DC2-mask-neg-nside-128.fits
--rw-r--r--   0 runner    (1001) docker     (123)  1581120 2023-06-13 19:46:14.000000 pz-rail-astro-tools-0.0.2/src/rail/examples_data/creation_data/data/survey_conditions/minion_1016_dc2_Median_airmass_i_and_nightlt1825_HEAL.fits
--rw-r--r--   0 runner    (1001) docker     (123)  1581120 2023-06-13 19:46:14.000000 pz-rail-astro-tools-0.0.2/src/rail/examples_data/creation_data/data/survey_conditions/minion_1016_dc2_Median_fiveSigmaDepth_i_and_nightlt1825_HEAL.fits
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:46:32.240157 pz-rail-astro-tools-0.0.2/src/rail/tools/
--rw-r--r--   0 runner    (1001) docker     (123)    17806 2023-06-13 19:46:14.000000 pz-rail-astro-tools-0.0.2/src/rail/tools/utilPhotometry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:46:32.212155 pz-rail-astro-tools-0.0.2/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:46:32.240157 pz-rail-astro-tools-0.0.2/tests/astro_tools/
--rw-r--r--   0 runner    (1001) docker     (123)     7268 2023-06-13 19:46:14.000000 pz-rail-astro-tools-0.0.2/tests/astro_tools/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     8262 2023-06-13 19:46:14.000000 pz-rail-astro-tools-0.0.2/tests/astro_tools/test_degraders.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 23:28:35.424539 pz-rail-astro-tools-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-08-03 23:28:22.000000 pz-rail-astro-tools-0.0.3/.copier-answers.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 23:28:35.400539 pz-rail-astro-tools-0.0.3/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     3329 2023-08-03 23:28:22.000000 pz-rail-astro-tools-0.0.3/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 23:28:35.400539 pz-rail-astro-tools-0.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-08-03 23:28:22.000000 pz-rail-astro-tools-0.0.3/.github/workflows/add-issue-to-project-tracker.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-08-03 23:28:22.000000 pz-rail-astro-tools-0.0.3/.github/workflows/linting.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-08-03 23:28:22.000000 pz-rail-astro-tools-0.0.3/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-08-03 23:28:22.000000 pz-rail-astro-tools-0.0.3/.github/workflows/smoke-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-08-03 23:28:22.000000 pz-rail-astro-tools-0.0.3/.github/workflows/testing-and-coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-08-03 23:28:22.000000 pz-rail-astro-tools-0.0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-08-03 23:28:22.000000 pz-rail-astro-tools-0.0.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-08-03 23:28:22.000000 pz-rail-astro-tools-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-08-03 23:28:35.424539 pz-rail-astro-tools-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-08-03 23:28:22.000000 pz-rail-astro-tools-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-08-03 23:28:22.000000 pz-rail-astro-tools-0.0.3/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-08-03 23:28:22.000000 pz-rail-astro-tools-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 23:28:35.424539 pz-rail-astro-tools-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-08-03 23:28:22.000000 pz-rail-astro-tools-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 23:28:35.396538 pz-rail-astro-tools-0.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 23:28:35.400539 pz-rail-astro-tools-0.0.3/src/pz_rail_astro_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-08-03 23:28:35.000000 pz-rail-astro-tools-0.0.3/src/pz_rail_astro_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-08-03 23:28:35.000000 pz-rail-astro-tools-0.0.3/src/pz_rail_astro_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 23:28:35.000000 pz-rail-astro-tools-0.0.3/src/pz_rail_astro_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-08-03 23:28:35.000000 pz-rail-astro-tools-0.0.3/src/pz_rail_astro_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-03 23:28:35.000000 pz-rail-astro-tools-0.0.3/src/pz_rail_astro_tools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 23:28:35.396538 pz-rail-astro-tools-0.0.3/src/rail/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 23:28:35.400539 pz-rail-astro-tools-0.0.3/src/rail/astro_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-08-03 23:28:22.000000 pz-rail-astro-tools-0.0.3/src/rail/astro_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-08-03 23:28:35.000000 pz-rail-astro-tools-0.0.3/src/rail/astro_tools/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 23:28:35.396538 pz-rail-astro-tools-0.0.3/src/rail/creation/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 23:28:35.400539 pz-rail-astro-tools-0.0.3/src/rail/creation/degradation/
+-rw-r--r--   0 runner    (1001) docker     (123)    11974 2023-08-03 23:28:22.000000 pz-rail-astro-tools-0.0.3/src/rail/creation/degradation/grid_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-08-03 23:28:22.000000 pz-rail-astro-tools-0.0.3/src/rail/creation/degradation/lsst_error_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15697 2023-08-03 23:28:22.000000 pz-rail-astro-tools-0.0.3/src/rail/creation/degradation/observing_condition_degrader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4935 2023-08-03 23:28:22.000000 pz-rail-astro-tools-0.0.3/src/rail/creation/degradation/spectroscopic_degraders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22251 2023-08-03 23:28:22.000000 pz-rail-astro-tools-0.0.3/src/rail/creation/degradation/spectroscopic_selections.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 23:28:35.396538 pz-rail-astro-tools-0.0.3/src/rail/examples_data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 23:28:35.396538 pz-rail-astro-tools-0.0.3/src/rail/examples_data/creation_data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 23:28:35.400539 pz-rail-astro-tools-0.0.3/src/rail/examples_data/creation_data/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-08-03 23:28:22.000000 pz-rail-astro-tools-0.0.3/src/rail/examples_data/creation_data/data/HSC_grid_settings.pkl
+-rw-r--r--   0 runner    (1001) docker     (123) 13823712 2023-08-03 23:28:22.000000 pz-rail-astro-tools-0.0.3/src/rail/examples_data/creation_data/data/hsc_ratios_and_specz.hdf5
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 23:28:35.420539 pz-rail-astro-tools-0.0.3/src/rail/examples_data/creation_data/data/survey_conditions/
+-rw-r--r--   0 runner    (1001) docker     (123)  1581120 2023-08-03 23:28:22.000000 pz-rail-astro-tools-0.0.3/src/rail/examples_data/creation_data/data/survey_conditions/DC2-dr6-galcounts-i20-i25.3-nside-128.fits
+-rw-r--r--   0 runner    (1001) docker     (123)  1581120 2023-08-03 23:28:22.000000 pz-rail-astro-tools-0.0.3/src/rail/examples_data/creation_data/data/survey_conditions/DC2-mask-neg-nside-128.fits
+-rw-r--r--   0 runner    (1001) docker     (123)  1581120 2023-08-03 23:28:22.000000 pz-rail-astro-tools-0.0.3/src/rail/examples_data/creation_data/data/survey_conditions/minion_1016_dc2_Median_airmass_i_and_nightlt1825_HEAL.fits
+-rw-r--r--   0 runner    (1001) docker     (123)  1581120 2023-08-03 23:28:22.000000 pz-rail-astro-tools-0.0.3/src/rail/examples_data/creation_data/data/survey_conditions/minion_1016_dc2_Median_fiveSigmaDepth_i_and_nightlt1825_HEAL.fits
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 23:28:35.424539 pz-rail-astro-tools-0.0.3/src/rail/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)    17806 2023-08-03 23:28:22.000000 pz-rail-astro-tools-0.0.3/src/rail/tools/utilPhotometry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 23:28:35.396538 pz-rail-astro-tools-0.0.3/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 23:28:35.424539 pz-rail-astro-tools-0.0.3/tests/astro_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)     7268 2023-08-03 23:28:22.000000 pz-rail-astro-tools-0.0.3/tests/astro_tools/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8969 2023-08-03 23:28:22.000000 pz-rail-astro-tools-0.0.3/tests/astro_tools/test_degraders.py
```

### Comparing `pz-rail-astro-tools-0.0.2/.github/pull_request_template.md` & `pz-rail-astro-tools-0.0.3/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `pz-rail-astro-tools-0.0.2/.github/workflows/linting.yml` & `pz-rail-astro-tools-0.0.3/.github/workflows/linting.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-astro-tools-0.0.2/.github/workflows/publish-to-pypi.yml` & `pz-rail-astro-tools-0.0.3/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-astro-tools-0.0.2/.github/workflows/smoke-test.yml` & `pz-rail-astro-tools-0.0.3/.github/workflows/smoke-test.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-astro-tools-0.0.2/.github/workflows/testing-and-coverage.yml` & `pz-rail-astro-tools-0.0.3/.github/workflows/testing-and-coverage.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-astro-tools-0.0.2/.gitignore` & `pz-rail-astro-tools-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `pz-rail-astro-tools-0.0.2/.pre-commit-config.yaml` & `pz-rail-astro-tools-0.0.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pz-rail-astro-tools-0.0.2/LICENSE` & `pz-rail-astro-tools-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pz-rail-astro-tools-0.0.2/PKG-INFO` & `pz-rail-astro-tools-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pz-rail-astro-tools
-Version: 0.0.2
+Version: 0.0.3
 Author-email: "LSST Dark Energy Science Collaboration (DESC)" <later@later.com>
 License: MIT License
         
         Copyright (c) 2023 LSST Dark Energy Science Collaboration (DESC)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `pz-rail-astro-tools-0.0.2/README.md` & `pz-rail-astro-tools-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pz-rail-astro-tools-0.0.2/pyproject.toml` & `pz-rail-astro-tools-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pz-rail-astro-tools-0.0.2/src/pz_rail_astro_tools.egg-info/PKG-INFO` & `pz-rail-astro-tools-0.0.3/src/pz_rail_astro_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pz-rail-astro-tools
-Version: 0.0.2
+Version: 0.0.3
 Author-email: "LSST Dark Energy Science Collaboration (DESC)" <later@later.com>
 License: MIT License
         
         Copyright (c) 2023 LSST Dark Energy Science Collaboration (DESC)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `pz-rail-astro-tools-0.0.2/src/pz_rail_astro_tools.egg-info/SOURCES.txt` & `pz-rail-astro-tools-0.0.3/src/pz_rail_astro_tools.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 .copier-answers.yml
 .gitignore
 .pre-commit-config.yaml
 LICENSE
 README.md
+environment.yml
 pyproject.toml
 setup.py
 .github/pull_request_template.md
 .github/workflows/add-issue-to-project-tracker.yml
 .github/workflows/linting.yml
 .github/workflows/publish-to-pypi.yml
 .github/workflows/smoke-test.yml
@@ -15,14 +16,15 @@
 src/pz_rail_astro_tools.egg-info/SOURCES.txt
 src/pz_rail_astro_tools.egg-info/dependency_links.txt
 src/pz_rail_astro_tools.egg-info/requires.txt
 src/pz_rail_astro_tools.egg-info/top_level.txt
 src/rail/astro_tools/__init__.py
 src/rail/astro_tools/_version.py
 src/rail/creation/degradation/grid_selection.py
+src/rail/creation/degradation/lsst_error_model.py
 src/rail/creation/degradation/observing_condition_degrader.py
 src/rail/creation/degradation/spectroscopic_degraders.py
 src/rail/creation/degradation/spectroscopic_selections.py
 src/rail/examples_data/creation_data/data/HSC_grid_settings.pkl
 src/rail/examples_data/creation_data/data/hsc_ratios_and_specz.hdf5
 src/rail/examples_data/creation_data/data/survey_conditions/DC2-dr6-galcounts-i20-i25.3-nside-128.fits
 src/rail/examples_data/creation_data/data/survey_conditions/DC2-mask-neg-nside-128.fits
```

### Comparing `pz-rail-astro-tools-0.0.2/src/rail/creation/degradation/grid_selection.py` & `pz-rail-astro-tools-0.0.3/src/rail/creation/degradation/grid_selection.py`

 * *Files identical despite different names*

### Comparing `pz-rail-astro-tools-0.0.2/src/rail/creation/degradation/observing_condition_degrader.py` & `pz-rail-astro-tools-0.0.3/src/rail/creation/degradation/observing_condition_degrader.py`

 * *Files identical despite different names*

### Comparing `pz-rail-astro-tools-0.0.2/src/rail/creation/degradation/spectroscopic_degraders.py` & `pz-rail-astro-tools-0.0.3/src/rail/creation/degradation/spectroscopic_degraders.py`

 * *Files identical despite different names*

### Comparing `pz-rail-astro-tools-0.0.2/src/rail/creation/degradation/spectroscopic_selections.py` & `pz-rail-astro-tools-0.0.3/src/rail/creation/degradation/spectroscopic_selections.py`

 * *Files identical despite different names*

### Comparing `pz-rail-astro-tools-0.0.2/src/rail/examples_data/creation_data/data/hsc_ratios_and_specz.hdf5` & `pz-rail-astro-tools-0.0.3/src/rail/examples_data/creation_data/data/hsc_ratios_and_specz.hdf5`

 * *Files identical despite different names*

### Comparing `pz-rail-astro-tools-0.0.2/src/rail/examples_data/creation_data/data/survey_conditions/DC2-dr6-galcounts-i20-i25.3-nside-128.fits` & `pz-rail-astro-tools-0.0.3/src/rail/examples_data/creation_data/data/survey_conditions/DC2-dr6-galcounts-i20-i25.3-nside-128.fits`

 * *Files identical despite different names*

### Comparing `pz-rail-astro-tools-0.0.2/src/rail/examples_data/creation_data/data/survey_conditions/DC2-mask-neg-nside-128.fits` & `pz-rail-astro-tools-0.0.3/src/rail/examples_data/creation_data/data/survey_conditions/DC2-mask-neg-nside-128.fits`

 * *Files identical despite different names*

### Comparing `pz-rail-astro-tools-0.0.2/src/rail/examples_data/creation_data/data/survey_conditions/minion_1016_dc2_Median_airmass_i_and_nightlt1825_HEAL.fits` & `pz-rail-astro-tools-0.0.3/src/rail/examples_data/creation_data/data/survey_conditions/minion_1016_dc2_Median_airmass_i_and_nightlt1825_HEAL.fits`

 * *Files identical despite different names*

### Comparing `pz-rail-astro-tools-0.0.2/src/rail/examples_data/creation_data/data/survey_conditions/minion_1016_dc2_Median_fiveSigmaDepth_i_and_nightlt1825_HEAL.fits` & `pz-rail-astro-tools-0.0.3/src/rail/examples_data/creation_data/data/survey_conditions/minion_1016_dc2_Median_fiveSigmaDepth_i_and_nightlt1825_HEAL.fits`

 * *Files identical despite different names*

### Comparing `pz-rail-astro-tools-0.0.2/src/rail/tools/utilPhotometry.py` & `pz-rail-astro-tools-0.0.3/src/rail/tools/utilPhotometry.py`

 * *Files identical despite different names*

### Comparing `pz-rail-astro-tools-0.0.2/tests/astro_tools/test_core.py` & `pz-rail-astro-tools-0.0.3/tests/astro_tools/test_core.py`

 * *Files identical despite different names*

### Comparing `pz-rail-astro-tools-0.0.2/tests/astro_tools/test_degraders.py` & `pz-rail-astro-tools-0.0.3/tests/astro_tools/test_degraders.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import os
 from typing import Type
 
 import numpy as np
 import pandas as pd
 import pytest
-from photerr import LsstErrorModel
+from photerr import LsstErrorModel as PhoterrErrorModel
 
 from rail.core.data import DATA_STORE, TableHandle
 from rail.core.utils import find_rail_file
 from rail.core.utilStages import ColumnMapper
 from rail.creation.degradation.spectroscopic_degraders import InvRedshiftIncompleteness, LineConfusion
 from rail.creation.degradation.spectroscopic_selections import *
 from rail.creation.degradation.observing_condition_degrader import ObsCondition
 from rail.creation.degradation.grid_selection import GridSelection
+from rail.creation.degradation.lsst_error_model import LSSTErrorModel
 
 
 @pytest.fixture
 def data():
     """Some dummy data to use below."""
 
     DS = DATA_STORE()
@@ -229,15 +230,33 @@
 
     os.remove(degrader_ext.get_output(degrader_ext.get_aliased_tag("output"), final_name=True))
 
 
 def test_ObsCondition_empty_map_dict(data):
     """Test control with random seeds."""
     degrader1 = ObsCondition.make_stage(random_seed=0, map_dict={})
-    degrader2 = LsstErrorModel()
+    degrader2 = PhoterrErrorModel()
 
     # make sure setting the same seeds yields the same output
     degraded_data1 = degrader1(data).data
     degraded_data2 = degrader2(data.data, random_state=0)
     assert degraded_data1.equals(degraded_data2)
 
     os.remove(degrader1.get_output(degrader1.get_aliased_tag("output"), final_name=True))
+
+
+def test_LSSTErrorModel_returns_correct_columns(data):
+    # Setup the stage
+    degrader = LSSTErrorModel.make_stage()
+
+    # Apply the degrader and get the data out
+    degraded_data = degrader(data).data
+
+    # Check that we still have the same number of rows, and added an extra
+    # column for each band
+    assert degraded_data.shape == (data.data.shape[0], 2 * data.data.shape[1] - 1)
+    for band in "ugrizy":
+        assert band in degraded_data.columns
+        assert f"{band}_err" in degraded_data.columns
+    os.remove(degrader.get_output(degrader.get_aliased_tag("output"), final_name=True))
+
+
```

