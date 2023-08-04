# Comparing `tmp/patch-denoise-1.4.0.tar.gz` & `tmp/patch-denoise-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "patch-denoise-1.4.0.tar", last modified: Mon May 22 08:29:23 2023, max compression
+gzip compressed data, was "patch-denoise-1.4.1.tar", last modified: Fri Aug  4 12:09:14 2023, max compression
```

## Comparing `patch-denoise-1.4.0.tar` & `patch-denoise-1.4.1.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:29:23.533400 patch-denoise-1.4.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:29:23.525400 patch-denoise-1.4.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:29:23.525400 patch-denoise-1.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-05-22 08:28:42.000000 patch-denoise-1.4.0/.github/workflows/master-cd.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-05-22 08:28:42.000000 patch-denoise-1.4.0/.github/workflows/tags-release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-05-22 08:28:42.000000 patch-denoise-1.4.0/.github/workflows/test-ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-22 08:28:42.000000 patch-denoise-1.4.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-22 08:28:42.000000 patch-denoise-1.4.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5988 2023-05-22 08:29:23.533400 patch-denoise-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-05-22 08:28:42.000000 patch-denoise-1.4.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:29:23.525400 patch-denoise-1.4.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-22 08:28:42.000000 patch-denoise-1.4.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:29:23.525400 patch-denoise-1.4.0/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-05-22 08:28:42.000000 patch-denoise-1.4.0/docs/_templates/custom-class-template.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-05-22 08:28:42.000000 patch-denoise-1.4.0/docs/_templates/custom-module-template.rst
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-22 08:28:42.000000 patch-denoise-1.4.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-05-22 08:28:42.000000 patch-denoise-1.4.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     6440 2023-05-22 08:28:42.000000 patch-denoise-1.4.0/docs/denoisers.rst
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-22 08:28:42.000000 patch-denoise-1.4.0/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:29:23.529400 patch-denoise-1.4.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-22 08:28:42.000000 patch-denoise-1.4.0/examples/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-22 08:28:42.000000 patch-denoise-1.4.0/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-05-22 08:28:42.000000 patch-denoise-1.4.0/examples/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-05-22 08:28:42.000000 patch-denoise-1.4.0/examples/example_experimental_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-05-22 08:28:42.000000 patch-denoise-1.4.0/examples/example_visualisation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-05-22 08:28:42.000000 patch-denoise-1.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 08:29:23.533400 patch-denoise-1.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:29:23.525400 patch-denoise-1.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:29:23.529400 patch-denoise-1.4.0/src/patch_denoise/
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-05-22 08:28:42.000000 patch-denoise-1.4.0/src/patch_denoise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-05-22 08:28:42.000000 patch-denoise-1.4.0/src/patch_denoise/_docs.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-22 08:29:23.000000 patch-denoise-1.4.0/src/patch_denoise/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:29:23.529400 patch-denoise-1.4.0/src/patch_denoise/bindings/
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-22 08:28:42.000000 patch-denoise-1.4.0/src/patch_denoise/bindings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4784 2023-05-22 08:28:42.000000 patch-denoise-1.4.0/src/patch_denoise/bindings/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-05-22 08:28:42.000000 patch-denoise-1.4.0/src/patch_denoise/bindings/modopt.py
--rw-r--r--   0 runner    (1001) docker     (123)     6898 2023-05-22 08:28:42.000000 patch-denoise-1.4.0/src/patch_denoise/bindings/nipype.py
--rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-05-22 08:28:42.000000 patch-denoise-1.4.0/src/patch_denoise/bindings/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7565 2023-05-22 08:28:42.000000 patch-denoise-1.4.0/src/patch_denoise/denoise.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:29:23.529400 patch-denoise-1.4.0/src/patch_denoise/simulation/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-22 08:28:42.000000 patch-denoise-1.4.0/src/patch_denoise/simulation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-22 08:28:42.000000 patch-denoise-1.4.0/src/patch_denoise/simulation/activations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-05-22 08:28:42.000000 patch-denoise-1.4.0/src/patch_denoise/simulation/noise.py
--rw-r--r--   0 runner    (1001) docker     (123)     9132 2023-05-22 08:28:42.000000 patch-denoise-1.4.0/src/patch_denoise/simulation/phantom.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:29:23.529400 patch-denoise-1.4.0/src/patch_denoise/space_time/
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-22 08:28:42.000000 patch-denoise-1.4.0/src/patch_denoise/space_time/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6237 2023-05-22 08:28:42.000000 patch-denoise-1.4.0/src/patch_denoise/space_time/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    17807 2023-05-22 08:28:42.000000 patch-denoise-1.4.0/src/patch_denoise/space_time/lowrank.py
--rw-r--r--   0 runner    (1001) docker     (123)     6303 2023-05-22 08:28:42.000000 patch-denoise-1.4.0/src/patch_denoise/space_time/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:29:23.529400 patch-denoise-1.4.0/src/patch_denoise/viz/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-22 08:28:42.000000 patch-denoise-1.4.0/src/patch_denoise/viz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-05-22 08:28:42.000000 patch-denoise-1.4.0/src/patch_denoise/viz/plots.py
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-05-22 08:28:42.000000 patch-denoise-1.4.0/src/patch_denoise/viz/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:29:23.529400 patch-denoise-1.4.0/src/patch_denoise.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5988 2023-05-22 08:29:23.000000 patch-denoise-1.4.0/src/patch_denoise.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-05-22 08:29:23.000000 patch-denoise-1.4.0/src/patch_denoise.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 08:29:23.000000 patch-denoise-1.4.0/src/patch_denoise.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-22 08:29:23.000000 patch-denoise-1.4.0/src/patch_denoise.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-22 08:29:23.000000 patch-denoise-1.4.0/src/patch_denoise.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-22 08:29:23.000000 patch-denoise-1.4.0/src/patch_denoise.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:29:23.529400 patch-denoise-1.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:28:42.000000 patch-denoise-1.4.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-05-22 08:28:42.000000 patch-denoise-1.4.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3501 2023-05-22 08:28:42.000000 patch-denoise-1.4.0/tests/test_bindings.py
--rw-r--r--   0 runner    (1001) docker     (123)     5266 2023-05-22 08:28:42.000000 patch-denoise-1.4.0/tests/test_denoiser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2961 2023-05-22 08:28:42.000000 patch-denoise-1.4.0/tests/test_spacetime_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-05-22 08:28:42.000000 patch-denoise-1.4.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:09:14.862670 patch-denoise-1.4.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:09:14.850670 patch-denoise-1.4.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:09:14.854670 patch-denoise-1.4.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-08-04 12:08:37.000000 patch-denoise-1.4.1/.github/workflows/master-cd.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-08-04 12:08:37.000000 patch-denoise-1.4.1/.github/workflows/tags-release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-08-04 12:08:37.000000 patch-denoise-1.4.1/.github/workflows/test-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-08-04 12:08:37.000000 patch-denoise-1.4.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-08-04 12:08:37.000000 patch-denoise-1.4.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5988 2023-08-04 12:09:14.862670 patch-denoise-1.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-08-04 12:08:37.000000 patch-denoise-1.4.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:09:14.854670 patch-denoise-1.4.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-08-04 12:08:37.000000 patch-denoise-1.4.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:09:14.854670 patch-denoise-1.4.1/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-08-04 12:08:37.000000 patch-denoise-1.4.1/docs/_templates/custom-class-template.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-08-04 12:08:37.000000 patch-denoise-1.4.1/docs/_templates/custom-module-template.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-08-04 12:08:37.000000 patch-denoise-1.4.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-08-04 12:08:37.000000 patch-denoise-1.4.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6440 2023-08-04 12:08:37.000000 patch-denoise-1.4.1/docs/denoisers.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-08-04 12:08:37.000000 patch-denoise-1.4.1/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:09:14.854670 patch-denoise-1.4.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-08-04 12:08:37.000000 patch-denoise-1.4.1/examples/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-08-04 12:08:37.000000 patch-denoise-1.4.1/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-08-04 12:08:37.000000 patch-denoise-1.4.1/examples/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-08-04 12:08:37.000000 patch-denoise-1.4.1/examples/example_experimental_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-08-04 12:08:37.000000 patch-denoise-1.4.1/examples/example_visualisation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-08-04 12:08:37.000000 patch-denoise-1.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:09:14.862670 patch-denoise-1.4.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:09:14.850670 patch-denoise-1.4.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:09:14.854670 patch-denoise-1.4.1/src/patch_denoise/
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-08-04 12:08:37.000000 patch-denoise-1.4.1/src/patch_denoise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-08-04 12:08:37.000000 patch-denoise-1.4.1/src/patch_denoise/_docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-08-04 12:09:14.000000 patch-denoise-1.4.1/src/patch_denoise/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:09:14.858670 patch-denoise-1.4.1/src/patch_denoise/bindings/
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-08-04 12:08:37.000000 patch-denoise-1.4.1/src/patch_denoise/bindings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5285 2023-08-04 12:08:37.000000 patch-denoise-1.4.1/src/patch_denoise/bindings/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-08-04 12:08:37.000000 patch-denoise-1.4.1/src/patch_denoise/bindings/modopt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6898 2023-08-04 12:08:37.000000 patch-denoise-1.4.1/src/patch_denoise/bindings/nipype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-08-04 12:08:37.000000 patch-denoise-1.4.1/src/patch_denoise/bindings/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7565 2023-08-04 12:08:37.000000 patch-denoise-1.4.1/src/patch_denoise/denoise.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:09:14.858670 patch-denoise-1.4.1/src/patch_denoise/simulation/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-08-04 12:08:37.000000 patch-denoise-1.4.1/src/patch_denoise/simulation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-08-04 12:08:37.000000 patch-denoise-1.4.1/src/patch_denoise/simulation/activations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-08-04 12:08:37.000000 patch-denoise-1.4.1/src/patch_denoise/simulation/noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9132 2023-08-04 12:08:37.000000 patch-denoise-1.4.1/src/patch_denoise/simulation/phantom.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:09:14.858670 patch-denoise-1.4.1/src/patch_denoise/space_time/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-08-04 12:08:37.000000 patch-denoise-1.4.1/src/patch_denoise/space_time/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6237 2023-08-04 12:08:37.000000 patch-denoise-1.4.1/src/patch_denoise/space_time/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17807 2023-08-04 12:08:37.000000 patch-denoise-1.4.1/src/patch_denoise/space_time/lowrank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6303 2023-08-04 12:08:37.000000 patch-denoise-1.4.1/src/patch_denoise/space_time/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:09:14.862670 patch-denoise-1.4.1/src/patch_denoise/viz/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-08-04 12:08:37.000000 patch-denoise-1.4.1/src/patch_denoise/viz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-08-04 12:08:37.000000 patch-denoise-1.4.1/src/patch_denoise/viz/plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-08-04 12:08:37.000000 patch-denoise-1.4.1/src/patch_denoise/viz/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:09:14.858670 patch-denoise-1.4.1/src/patch_denoise.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5988 2023-08-04 12:09:14.000000 patch-denoise-1.4.1/src/patch_denoise.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-08-04 12:09:14.000000 patch-denoise-1.4.1/src/patch_denoise.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:09:14.000000 patch-denoise-1.4.1/src/patch_denoise.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-08-04 12:09:14.000000 patch-denoise-1.4.1/src/patch_denoise.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-08-04 12:09:14.000000 patch-denoise-1.4.1/src/patch_denoise.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-04 12:09:14.000000 patch-denoise-1.4.1/src/patch_denoise.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:09:14.862670 patch-denoise-1.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 12:08:37.000000 patch-denoise-1.4.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-08-04 12:08:37.000000 patch-denoise-1.4.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3501 2023-08-04 12:08:37.000000 patch-denoise-1.4.1/tests/test_bindings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5266 2023-08-04 12:08:37.000000 patch-denoise-1.4.1/tests/test_denoiser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2961 2023-08-04 12:08:37.000000 patch-denoise-1.4.1/tests/test_spacetime_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-08-04 12:08:37.000000 patch-denoise-1.4.1/tests/test_utils.py
```

### Comparing `patch-denoise-1.4.0/.github/workflows/master-cd.yml` & `patch-denoise-1.4.1/.github/workflows/master-cd.yml`

 * *Files identical despite different names*

### Comparing `patch-denoise-1.4.0/.github/workflows/tags-release.yml` & `patch-denoise-1.4.1/.github/workflows/tags-release.yml`

 * *Files identical despite different names*

### Comparing `patch-denoise-1.4.0/.github/workflows/test-ci.yml` & `patch-denoise-1.4.1/.github/workflows/test-ci.yml`

 * *Files identical despite different names*

### Comparing `patch-denoise-1.4.0/LICENSE.txt` & `patch-denoise-1.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `patch-denoise-1.4.0/PKG-INFO` & `patch-denoise-1.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: patch-denoise
-Version: 1.4.0
+Version: 1.4.1
 Summary: Denoising method for sequence of images or volumes. Primarly targeting fMRI data.
 Author-email: Pierre-antoine Comby <pierre-antoine.comby@crans.org>
 License: MIT License
         
         Copyright (c) 2023 Pierre-Antoine Comby
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `patch-denoise-1.4.0/README.rst` & `patch-denoise-1.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `patch-denoise-1.4.0/docs/Makefile` & `patch-denoise-1.4.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `patch-denoise-1.4.0/docs/_templates/custom-class-template.rst` & `patch-denoise-1.4.1/docs/_templates/custom-class-template.rst`

 * *Files identical despite different names*

### Comparing `patch-denoise-1.4.0/docs/_templates/custom-module-template.rst` & `patch-denoise-1.4.1/docs/_templates/custom-module-template.rst`

 * *Files identical despite different names*

### Comparing `patch-denoise-1.4.0/docs/conf.py` & `patch-denoise-1.4.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `patch-denoise-1.4.0/docs/denoisers.rst` & `patch-denoise-1.4.1/docs/denoisers.rst`

 * *Files identical despite different names*

### Comparing `patch-denoise-1.4.0/examples/conftest.py` & `patch-denoise-1.4.1/examples/conftest.py`

 * *Files identical despite different names*

### Comparing `patch-denoise-1.4.0/examples/example_experimental_data.py` & `patch-denoise-1.4.1/examples/example_experimental_data.py`

 * *Files identical despite different names*

### Comparing `patch-denoise-1.4.0/examples/example_visualisation.py` & `patch-denoise-1.4.1/examples/example_visualisation.py`

 * *Files identical despite different names*

### Comparing `patch-denoise-1.4.0/pyproject.toml` & `patch-denoise-1.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `patch-denoise-1.4.0/src/patch_denoise/__init__.py` & `patch-denoise-1.4.1/src/patch_denoise/__init__.py`

 * *Files identical despite different names*

### Comparing `patch-denoise-1.4.0/src/patch_denoise/_docs.py` & `patch-denoise-1.4.1/src/patch_denoise/_docs.py`

 * *Files identical despite different names*

### Comparing `patch-denoise-1.4.0/src/patch_denoise/bindings/cli.py` & `patch-denoise-1.4.1/src/patch_denoise/bindings/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -58,14 +58,20 @@
     )
     parser.add_argument(
         "--extra",
         default=None,
         nargs="*",
         help="extra key=value arguments.",
     )
+    parser.add_argument(
+        "--nan-to-num",
+        default=None,
+        type=float,
+        help="Replace NaN by the provided value.",
+    )
 
     args = parser.parse_args()
 
     # default value for output.
     if args.output_file is None:
         input_path = args.input_file.split("/")
         args.output_file = "/".join(input_path)[:-1] + "/d" + input_path[-1]
@@ -115,14 +121,25 @@
 
 def main():
     """Command line entry point."""
     args = parse_args()
     print(args)
 
     input_data, affine = load_as_array(args.input_file)
+
+    if args.nan_to_num is not None:
+        input_data = np.nan_to_num(input_data, nan=args.nan_to_num)
+    n_nans = np.isnan(input_data).sum()
+    if n_nans > 0:
+        warnings.warn(
+            f"{n_nans}/{np.prod(input_data.shape)} voxels are NaN."
+            " You might want to use --nan-to-num=<value>",
+            stacklevel=0,
+        )
+
     if args.mask == "auto":
         mask = compute_mask(input_data)
         affine_mask = None
     else:
         mask, affine_mask = load_as_array(args.mask)
     noise_map, affine_noise_map = load_as_array(args.noise_map)
 
@@ -131,14 +148,15 @@
             warnings.warn(
                 "Affine matrix of input and mask does not match", stacklevel=2
             )
         if affine_noise_map is not None and np.allclose(affine, affine_noise_map):
             warnings.warn(
                 "Affine matrix of input and noise map does not match", stacklevel=2
             )
+
     d_par = DenoiseParameters.from_str(args.conf)
     print(d_par)
     denoise_func = DENOISER_MAP[d_par.method]
     extra_kwargs = dict()
 
     if d_par.method in [
         "nordic",
@@ -153,15 +171,15 @@
         input_data,
         patch_shape=d_par.patch_shape,
         patch_overlap=d_par.patch_overlap,
         mask=mask,
         mask_threshold=d_par.mask_threshold,
         recombination=d_par.recombination,
         **extra_kwargs,
-        **args.extra
+        **args.extra,
     )
 
     save_array(denoised_data, affine, args.output_file)
     save_array(noise_std_map, affine, args.output_noise_map)
 
 
 if __name__ == "__main__":
```

### Comparing `patch-denoise-1.4.0/src/patch_denoise/bindings/modopt.py` & `patch-denoise-1.4.1/src/patch_denoise/bindings/modopt.py`

 * *Files identical despite different names*

### Comparing `patch-denoise-1.4.0/src/patch_denoise/bindings/nipype.py` & `patch-denoise-1.4.1/src/patch_denoise/bindings/nipype.py`

 * *Files identical despite different names*

### Comparing `patch-denoise-1.4.0/src/patch_denoise/bindings/utils.py` & `patch-denoise-1.4.1/src/patch_denoise/bindings/utils.py`

 * *Files identical despite different names*

### Comparing `patch-denoise-1.4.0/src/patch_denoise/denoise.py` & `patch-denoise-1.4.1/src/patch_denoise/denoise.py`

 * *Files identical despite different names*

### Comparing `patch-denoise-1.4.0/src/patch_denoise/simulation/noise.py` & `patch-denoise-1.4.1/src/patch_denoise/simulation/noise.py`

 * *Files identical despite different names*

### Comparing `patch-denoise-1.4.0/src/patch_denoise/simulation/phantom.py` & `patch-denoise-1.4.1/src/patch_denoise/simulation/phantom.py`

 * *Files identical despite different names*

### Comparing `patch-denoise-1.4.0/src/patch_denoise/space_time/base.py` & `patch-denoise-1.4.1/src/patch_denoise/space_time/base.py`

 * *Files identical despite different names*

### Comparing `patch-denoise-1.4.0/src/patch_denoise/space_time/lowrank.py` & `patch-denoise-1.4.1/src/patch_denoise/space_time/lowrank.py`

 * *Files identical despite different names*

### Comparing `patch-denoise-1.4.0/src/patch_denoise/space_time/utils.py` & `patch-denoise-1.4.1/src/patch_denoise/space_time/utils.py`

 * *Files identical despite different names*

### Comparing `patch-denoise-1.4.0/src/patch_denoise/viz/plots.py` & `patch-denoise-1.4.1/src/patch_denoise/viz/plots.py`

 * *Files identical despite different names*

### Comparing `patch-denoise-1.4.0/src/patch_denoise/viz/utils.py` & `patch-denoise-1.4.1/src/patch_denoise/viz/utils.py`

 * *Files identical despite different names*

### Comparing `patch-denoise-1.4.0/src/patch_denoise.egg-info/PKG-INFO` & `patch-denoise-1.4.1/src/patch_denoise.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: patch-denoise
-Version: 1.4.0
+Version: 1.4.1
 Summary: Denoising method for sequence of images or volumes. Primarly targeting fMRI data.
 Author-email: Pierre-antoine Comby <pierre-antoine.comby@crans.org>
 License: MIT License
         
         Copyright (c) 2023 Pierre-Antoine Comby
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `patch-denoise-1.4.0/src/patch_denoise.egg-info/SOURCES.txt` & `patch-denoise-1.4.1/src/patch_denoise.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `patch-denoise-1.4.0/tests/conftest.py` & `patch-denoise-1.4.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `patch-denoise-1.4.0/tests/test_bindings.py` & `patch-denoise-1.4.1/tests/test_bindings.py`

 * *Files identical despite different names*

### Comparing `patch-denoise-1.4.0/tests/test_denoiser.py` & `patch-denoise-1.4.1/tests/test_denoiser.py`

 * *Files identical despite different names*

### Comparing `patch-denoise-1.4.0/tests/test_spacetime_utils.py` & `patch-denoise-1.4.1/tests/test_spacetime_utils.py`

 * *Files identical despite different names*

