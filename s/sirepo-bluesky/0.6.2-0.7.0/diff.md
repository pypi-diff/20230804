# Comparing `tmp/sirepo-bluesky-0.6.2.tar.gz` & `tmp/sirepo-bluesky-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sirepo-bluesky-0.6.2.tar", last modified: Fri Jun  9 16:49:00 2023, max compression
+gzip compressed data, was "sirepo-bluesky-0.7.0.tar", last modified: Fri Aug  4 20:56:39 2023, max compression
```

## Comparing `sirepo-bluesky-0.6.2.tar` & `sirepo-bluesky-0.7.0.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:49:00.634703 sirepo-bluesky-0.6.2/
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-06-09 16:48:49.000000 sirepo-bluesky-0.6.2/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3099 2023-06-09 16:48:49.000000 sirepo-bluesky-0.6.2/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-06-09 16:48:49.000000 sirepo-bluesky-0.6.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-09 16:48:49.000000 sirepo-bluesky-0.6.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-06-09 16:49:00.634703 sirepo-bluesky-0.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-06-09 16:48:49.000000 sirepo-bluesky-0.6.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:49:00.626703 sirepo-bluesky-0.6.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-06-09 16:48:49.000000 sirepo-bluesky-0.6.2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-06-09 16:48:49.000000 sirepo-bluesky-0.6.2/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:49:00.626703 sirepo-bluesky-0.6.2/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)     6149 2023-06-09 16:48:49.000000 sirepo-bluesky-0.6.2/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-09 16:48:49.000000 sirepo-bluesky-0.6.2/docs/source/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-06-09 16:48:49.000000 sirepo-bluesky-0.6.2/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-06-09 16:48:49.000000 sirepo-bluesky-0.6.2/docs/source/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8378 2023-06-09 16:48:49.000000 sirepo-bluesky-0.6.2/docs/source/release-history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-06-09 16:48:49.000000 sirepo-bluesky-0.6.2/docs/source/simulations.rst
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-09 16:48:50.000000 sirepo-bluesky-0.6.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-09 16:48:50.000000 sirepo-bluesky-0.6.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-09 16:49:00.634703 sirepo-bluesky-0.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-06-09 16:48:50.000000 sirepo-bluesky-0.6.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:49:00.634703 sirepo-bluesky-0.6.2/sirepo_bluesky/
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-06-09 16:48:50.000000 sirepo-bluesky-0.6.2/sirepo_bluesky/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-09 16:49:00.634703 sirepo-bluesky-0.6.2/sirepo_bluesky/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4199 2023-06-09 16:48:50.000000 sirepo-bluesky-0.6.2/sirepo_bluesky/madx_flyer.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-09 16:48:50.000000 sirepo-bluesky-0.6.2/sirepo_bluesky/madx_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    13429 2023-06-09 16:48:50.000000 sirepo-bluesky-0.6.2/sirepo_bluesky/shadow_detector.py
--rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-06-09 16:48:50.000000 sirepo-bluesky-0.6.2/sirepo_bluesky/shadow_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     8409 2023-06-09 16:48:50.000000 sirepo-bluesky-0.6.2/sirepo_bluesky/sirepo_bluesky.py
--rw-r--r--   0 runner    (1001) docker     (123)    15800 2023-06-09 16:48:50.000000 sirepo-bluesky-0.6.2/sirepo_bluesky/sirepo_flyer.py
--rw-r--r--   0 runner    (1001) docker     (123)    15176 2023-06-09 16:48:50.000000 sirepo-bluesky-0.6.2/sirepo_bluesky/sirepo_ophyd.py
--rw-r--r--   0 runner    (1001) docker     (123)    12002 2023-06-09 16:48:50.000000 sirepo-bluesky-0.6.2/sirepo_bluesky/srw_detector.py
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-06-09 16:48:50.000000 sirepo-bluesky-0.6.2/sirepo_bluesky/srw_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:49:00.630703 sirepo-bluesky-0.6.2/sirepo_bluesky/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 16:48:50.000000 sirepo-bluesky-0.6.2/sirepo_bluesky/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-06-09 16:48:50.000000 sirepo-bluesky-0.6.2/sirepo_bluesky/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    15535 2023-06-09 16:48:50.000000 sirepo-bluesky-0.6.2/sirepo_bluesky/tests/test_bl_elements_as_ophyd_objs.py
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-09 16:48:50.000000 sirepo-bluesky-0.6.2/sirepo_bluesky/tests/test_entrypoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-06-09 16:48:50.000000 sirepo-bluesky-0.6.2/sirepo_bluesky/tests/test_shadow_det.py
--rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-06-09 16:48:50.000000 sirepo-bluesky-0.6.2/sirepo_bluesky/tests/test_sirepo_flyer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-06-09 16:48:50.000000 sirepo-bluesky-0.6.2/sirepo_bluesky/tests/test_srw_det.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:49:00.630703 sirepo-bluesky-0.6.2/sirepo_bluesky.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-06-09 16:49:00.000000 sirepo-bluesky-0.6.2/sirepo_bluesky.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-06-09 16:49:00.000000 sirepo-bluesky-0.6.2/sirepo_bluesky.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 16:49:00.000000 sirepo-bluesky-0.6.2/sirepo_bluesky.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-09 16:49:00.000000 sirepo-bluesky-0.6.2/sirepo_bluesky.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-09 16:49:00.000000 sirepo-bluesky-0.6.2/sirepo_bluesky.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    68503 2023-06-09 16:48:50.000000 sirepo-bluesky-0.6.2/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 20:56:39.111695 sirepo-bluesky-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-08-04 20:56:34.000000 sirepo-bluesky-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-08-04 20:56:34.000000 sirepo-bluesky-0.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-08-04 20:56:39.111695 sirepo-bluesky-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-08-04 20:56:34.000000 sirepo-bluesky-0.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 20:56:39.111695 sirepo-bluesky-0.7.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-08-04 20:56:34.000000 sirepo-bluesky-0.7.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-08-04 20:56:34.000000 sirepo-bluesky-0.7.0/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 20:56:39.111695 sirepo-bluesky-0.7.0/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     6149 2023-08-04 20:56:34.000000 sirepo-bluesky-0.7.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-08-04 20:56:34.000000 sirepo-bluesky-0.7.0/docs/source/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-08-04 20:56:34.000000 sirepo-bluesky-0.7.0/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-08-04 20:56:34.000000 sirepo-bluesky-0.7.0/docs/source/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9538 2023-08-04 20:56:34.000000 sirepo-bluesky-0.7.0/docs/source/release-history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-08-04 20:56:34.000000 sirepo-bluesky-0.7.0/docs/source/simulations.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-08-04 20:56:34.000000 sirepo-bluesky-0.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-08-04 20:56:34.000000 sirepo-bluesky-0.7.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-08-04 20:56:39.111695 sirepo-bluesky-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-08-04 20:56:34.000000 sirepo-bluesky-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 20:56:39.111695 sirepo-bluesky-0.7.0/sirepo_bluesky/
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-08-04 20:56:34.000000 sirepo-bluesky-0.7.0/sirepo_bluesky/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-08-04 20:56:39.111695 sirepo-bluesky-0.7.0/sirepo_bluesky/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4199 2023-08-04 20:56:34.000000 sirepo-bluesky-0.7.0/sirepo_bluesky/madx_flyer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-08-04 20:56:34.000000 sirepo-bluesky-0.7.0/sirepo_bluesky/madx_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4088 2023-08-04 20:56:34.000000 sirepo-bluesky-0.7.0/sirepo_bluesky/shadow_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11514 2023-08-04 20:56:34.000000 sirepo-bluesky-0.7.0/sirepo_bluesky/sirepo_bluesky.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15800 2023-08-04 20:56:34.000000 sirepo-bluesky-0.7.0/sirepo_bluesky/sirepo_flyer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20422 2023-08-04 20:56:34.000000 sirepo-bluesky-0.7.0/sirepo_bluesky/sirepo_ophyd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-08-04 20:56:34.000000 sirepo-bluesky-0.7.0/sirepo_bluesky/srw_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 20:56:39.111695 sirepo-bluesky-0.7.0/sirepo_bluesky/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 20:56:34.000000 sirepo-bluesky-0.7.0/sirepo_bluesky/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3967 2023-08-04 20:56:34.000000 sirepo-bluesky-0.7.0/sirepo_bluesky/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20025 2023-08-04 20:56:34.000000 sirepo-bluesky-0.7.0/sirepo_bluesky/tests/test_bl_elements_as_ophyd_objs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-08-04 20:56:34.000000 sirepo-bluesky-0.7.0/sirepo_bluesky/tests/test_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-08-04 20:56:34.000000 sirepo-bluesky-0.7.0/sirepo_bluesky/tests/test_entrypoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-08-04 20:56:34.000000 sirepo-bluesky-0.7.0/sirepo_bluesky/tests/test_sirepo_flyer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11958 2023-08-04 20:56:34.000000 sirepo-bluesky-0.7.0/sirepo_bluesky/tests/test_stateless_compute.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 20:56:39.111695 sirepo-bluesky-0.7.0/sirepo_bluesky/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-08-04 20:56:34.000000 sirepo-bluesky-0.7.0/sirepo_bluesky/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4214 2023-08-04 20:56:34.000000 sirepo-bluesky-0.7.0/sirepo_bluesky/utils/json_yaml_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 20:56:39.111695 sirepo-bluesky-0.7.0/sirepo_bluesky.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-08-04 20:56:39.000000 sirepo-bluesky-0.7.0/sirepo_bluesky.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-08-04 20:56:39.000000 sirepo-bluesky-0.7.0/sirepo_bluesky.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 20:56:39.000000 sirepo-bluesky-0.7.0/sirepo_bluesky.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-08-04 20:56:39.000000 sirepo-bluesky-0.7.0/sirepo_bluesky.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-08-04 20:56:39.000000 sirepo-bluesky-0.7.0/sirepo_bluesky.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-04 20:56:39.000000 sirepo-bluesky-0.7.0/sirepo_bluesky.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    68503 2023-08-04 20:56:34.000000 sirepo-bluesky-0.7.0/versioneer.py
```

### Comparing `sirepo-bluesky-0.6.2/LICENSE` & `sirepo-bluesky-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sirepo-bluesky-0.6.2/PKG-INFO` & `sirepo-bluesky-0.7.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,46 +1,43 @@
-Metadata-Version: 2.1
-Name: sirepo-bluesky
-Version: 0.6.2
-Summary: Sirepo-Bluesky interface
-Home-page: https://github.com/NSLS-II/sirepo-bluesky
-Author: Brookhaven National Laboratory
-Author-email: mrakitin@bnl.gov
-License: BSD (3-clause)
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.8
-License-File: LICENSE
-License-File: AUTHORS.rst
-
-==============
-sirepo-bluesky
-==============
-
-.. image:: https://zenodo.org/badge/243052461.svg
-   :target: https://zenodo.org/badge/latestdoi/243052461
-
-.. image:: https://github.com/NSLS-II/sirepo-bluesky/actions/workflows/testing.yml/badge.svg
-   :target: https://github.com/NSLS-II/sirepo-bluesky/actions/workflows/testing.yml
-
-.. image:: https://img.shields.io/pypi/v/sirepo-bluesky.svg?logo=pypi&logoColor=white&label=PyPI
-   :target: https://pypi.python.org/pypi/sirepo-bluesky
-
-.. image:: https://img.shields.io/conda/vn/conda-forge/sirepo-bluesky.svg?logo=conda-forge&logoColor=white
-   :target: https://anaconda.org/conda-forge/sirepo-bluesky
-
-
-This is a Sirepo-Bluesky interface library that allows using the `Bluesky data
-acquisition framework <https://blueskyproject.io>`_ to run `Sirepo
-<https://github.com/radiasoft/sirepo>`_ simulations (SRW, Shadow3, etc.)
-
-* Free software: 3-clause BSD license
-* Citation:
-
-     Maksim S. Rakitin, Abigail Giles, Kaleb Swartz, Joshua Lynch, Paul Moeller, Robert Nagler,
-     Daniel B. Allan, Thomas A. Caswell, Lutz Wiegart, Oleg Chubar, and Yonghua Du
-     "Introduction of the Sirepo-Bluesky interface and its application to the optimization problems",
-     Proc. SPIE 11493, Advances in Computational Methods for X-Ray Optics V, 1149311 (21 August 2020);
-     https://doi.org/10.1117/12.2569000
+# Sirepo-Bluesky
 
-* Documentation: https://nsls-ii.github.io/sirepo-bluesky
+[![Zenodo](https://zenodo.org/badge/243052461.svg)](https://zenodo.org/badge/latestdoi/243052461)
+[![Test](https://github.com/NSLS-II/sirepo-bluesky/actions/workflows/testing.yml/badge.svg)](https://github.com/NSLS-II/sirepo-bluesky/actions/workflows/testing.yml)
+[![PyPI](https://img.shields.io/pypi/v/sirepo-bluesky.svg?logo=pypi&logoColor=white&label=PyPI)](https://pypi.python.org/pypi/sirepo-bluesky)
+[![Conda](https://img.shields.io/conda/vn/conda-forge/sirepo-bluesky.svg?logo=conda-forge&logoColor=white)](https://anaconda.org/conda-forge/sirepo-bluesky)
+
+This is a Sirepo-Bluesky interface library that allows using the [Bluesky data
+acquisition framework](https://blueskyproject.io) to run [Sirepo](https://github.com/radiasoft/sirepo) simulations (SRW, Shadow3, etc.)
+
+* Free software: BSD-3-Clause license
+
+
+## Documentation
+
+Please check our documentation at https://nsls-ii.github.io/sirepo-bluesky for
+installation instructions and examples using SRW, Shadow3, and MAD-X apps of
+Sirepo.
+
+
+## Citation
+
+> M. Rakitin, A. Giles, K. Swartz, J. Lynch, P. Moeller, R. Nagler, D.B. Allan, T.A. Caswell, L. Wiegart, O. Chubar, and Y. Du _"Introduction of the Sirepo-Bluesky interface and its application to the optimization problems"_, Proc. SPIE 11493, Advances in Computational Methods for X-Ray Optics V, 1149311 (21 August 2020); https://doi.org/10.1117/12.2569000
+
+BibTeX:
+```
+@InProceedings{2020.08-01:Rakitin,
+  author       = {Rakitin, Maksim S. and Giles, Abigail and Swartz, Kaleb and Lynch, Joshua and Moeller, Paul and Nagler, Robert and Allan, Daniel B. and Caswell, Thomas A. and Wiegart, Lutz and Chubar, Oleg and Du, Yonghua},
+  booktitle    = {Advances in Computational Methods for X-Ray Optics V},
+  title        = {{Introduction of the Sirepo-Bluesky interface and its application to the optimization problems}},
+  year         = {2020},
+  editor       = {Oleg Chubar and Kawal Sawhney},
+  month        = aug,
+  organization = {International Society for Optics and Photonics},
+  pages        = {209--226},
+  publisher    = {SPIE},
+  volume       = {11493},
+  doi          = {10.1117/12.2569000},
+  file         = {:papers/2020.08-01_Rakitin.pdf:PDF},
+  keywords     = {Sirepo, SRW, Bluesky, Databroker, Ophyd, optimization, simulations},
+  url          = {https://doi.org/10.1117/12.2569000},
+}
+```
```

### Comparing `sirepo-bluesky-0.6.2/docs/Makefile` & `sirepo-bluesky-0.7.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `sirepo-bluesky-0.6.2/docs/make.bat` & `sirepo-bluesky-0.7.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `sirepo-bluesky-0.6.2/docs/source/conf.py` & `sirepo-bluesky-0.7.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `sirepo-bluesky-0.6.2/docs/source/installation.rst` & `sirepo-bluesky-0.7.0/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `sirepo-bluesky-0.6.2/docs/source/release-history.rst` & `sirepo-bluesky-0.7.0/docs/source/release-history.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,47 @@
 ===============
 Release History
 ===============
 
+v0.7.0 (2023-08-04)
+-------------------
+
+New features
+............
+- Created ``.json`` and ``.yaml`` CLI exporters and added relevant tests.
+
+API
+...
+- Added ``stateless-compute`` support for CRL, Crystal, and Undulator objects in
+  the Sirepo/SRW app.
+- Implemented Ophyd support for Propagation parameters in the Sirepo/SRW app.
+- Converted integer Sirepo parameters to floats to fix the ``failed to format
+  row`` error in Bluesky's ``LiveTable``.
+- Added a lightweight method that computes the beam position and FWHM before it
+  is turned into a document for SRW and Shadow apps. The beam stats show up in
+  Bluesky's ``BestEffortCallback``.
+- Removed old API support and relevant tests.
+
+Documentation
+.............
+- Suppress Shadow3 code's stdout in notebooks/code.
+- Converted project's `README.rst` to `README.md` for better rendering on PyPI.
+
+Examples
+........
+- Added an empty beamline simulation (``sim_id="emptysim"``) to the list of
+  predefined examples.
+- Fixed MAD-X app's configuration to correctly display the UI components
+  (disabled React frontend).
+
+Linting/styling
+................
+- Added ``black`` formatter for Jupyter notebooks.
+
+
 v0.6.2 (2023-06-09)
 -------------------
 This is a maintenance release with small API, tests, packaging, and documentation updates.
 
 API
 ...
 - Fixed the ``BeamStatisticsReport``'s default values which cannot be a
```

### Comparing `sirepo-bluesky-0.6.2/docs/source/simulations.rst` & `sirepo-bluesky-0.7.0/docs/source/simulations.rst`

 * *Files identical despite different names*

### Comparing `sirepo-bluesky-0.6.2/setup.py` & `sirepo-bluesky-0.7.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -23,36 +23,38 @@
 """.format(
         *(sys.version_info[:2] + min_version)
     )
     sys.exit(error)
 
 here = path.abspath(path.dirname(__file__))
 
-with open(path.join(here, "README.rst"), encoding="utf-8") as readme_file:
+with open(path.join(here, "README.md"), encoding="utf-8") as readme_file:
     readme = readme_file.read()
 
 with open(path.join(here, "requirements.txt")) as requirements_file:
     # Parse requirements.txt, ignoring any commented-out lines.
     requirements = [line for line in requirements_file.read().splitlines() if not line.startswith("#")]
 
 
 setup(
     name="sirepo-bluesky",
     version=versioneer.get_version(),
     cmdclass=versioneer.get_cmdclass(),
     description="Sirepo-Bluesky interface",
     long_description=readme,
+    long_description_content_type="text/markdown",
     author="Brookhaven National Laboratory",
     author_email="mrakitin@bnl.gov",
     url="https://github.com/NSLS-II/sirepo-bluesky",
     python_requires=">={}".format(".".join(str(n) for n in min_version)),
     packages=find_packages(exclude=["docs", "tests"]),
     entry_points={
         "console_scripts": [
             # 'command = some.module:some_function',
+            "json-yaml-converter = sirepo_bluesky.utils.json_yaml_converter:cli_converter"
         ],
     },
     include_package_data=True,
     package_data={
         "sirepo_bluesky": [
             # When adding files here, remember to update MANIFEST.in as well,
             # or else they will not be included in the distribution on PyPI!
```

### Comparing `sirepo-bluesky-0.6.2/sirepo_bluesky/__init__.py` & `sirepo-bluesky-0.7.0/sirepo_bluesky/__init__.py`

 * *Files identical despite different names*

### Comparing `sirepo-bluesky-0.6.2/sirepo_bluesky/madx_flyer.py` & `sirepo-bluesky-0.7.0/sirepo_bluesky/madx_flyer.py`

 * *Files identical despite different names*

### Comparing `sirepo-bluesky-0.6.2/sirepo_bluesky/shadow_handler.py` & `sirepo-bluesky-0.7.0/sirepo_bluesky/shadow_handler.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,16 @@
+import contextlib
+import os
+
 import numpy as np
 import Shadow.ShadowLibExtensions as sd
 import Shadow.ShadowTools
 
+from . import utils
+
 
 def read_shadow_file_col(filename, parameter=30):
     """Read specified parameter from the Shadow3 output binary file.
 
     Parameters
     ----------
     filename : str
@@ -45,15 +50,17 @@
           28   K = 2 pi / lambda * col5 [A^-1]
           29   K = 2 pi / lambda * col6 [A^-1]
           30   S0-stokes = |Es|^2 + |Ep|^2
           31   S1-stokes = |Es|^2 - |Ep|^2
           32   S2-stokes = 2 |Es| |Ep| cos(phase_s-phase_p)
           33   S3-stokes = 2 |Es| |Ep| sin(phase_s-phase_p)
     """
-    data = Shadow.ShadowTools.getshcol(filename, col=parameter)
+    with open(os.devnull, "w") as devnull:
+        with contextlib.redirect_stdout(devnull):
+            data = Shadow.ShadowTools.getshcol(filename, col=parameter)
 
     mean_value = np.mean(data)
 
     return {
         "data": data,
         "shape": data.shape,
         "mean": mean_value,
@@ -69,32 +76,43 @@
     if histogram_bins is None:
         raise ValueError("'histogram_bins' kwarg should be specified.")
 
     beam = sd.Beam()
     beam.load(filename)
 
     # 1=X spatial coordinate; 3=Z spatial coordinate
-    data_dict = beam.histo2(1, 3, nolost=1, nbins=histogram_bins)
-    data = data_dict["histogram"]
+    with open(os.devnull, "w") as devnull:
+        with contextlib.redirect_stdout(devnull):
+            data_dict = beam.histo2(1, 3, nolost=1, nbins=histogram_bins)
 
-    # This returns a list of N values (N=number of rays)
-    photon_energy_list = Shadow.ShadowTools.getshcol(filename, col=11)  # 11=Energy [eV]
+            # This returns a list of N values (N=number of rays)
+            photon_energy_list = Shadow.ShadowTools.getshcol(filename, col=11)  # 11=Energy [eV]
+
+    data = data_dict["histogram"]
     photon_energy = np.mean(photon_energy_list)
 
-    return {
+    # convert to um
+    horizontal_extent = 1e3 * np.array(data_dict["xrange"][:2])
+    vertical_extent = 1e3 * np.array(data_dict["yrange"][:2])
+
+    ret = {
         "data": data,
         "shape": data.shape,
-        "mean": np.mean(data),
+        "flux": data.sum(),
+        "mean": data.mean(),
         "photon_energy": photon_energy,
-        "horizontal_extent": data_dict["xrange"][:2],
-        "vertical_extent": data_dict["yrange"][:2],
-        # 'labels': labels,
-        # 'units': units,
+        "horizontal_extent": horizontal_extent,
+        "vertical_extent": vertical_extent,
+        "units": "um",
     }
 
+    ret.update(utils.get_beam_stats(data, horizontal_extent, vertical_extent))
+
+    return ret
+
 
 class ShadowFileHandler:
     specs = {"shadow"}
 
     def __init__(self, filename, histogram_bins, **kwargs):
         self._name = filename
         self._histogram_bins = histogram_bins
```

### Comparing `sirepo-bluesky-0.6.2/sirepo_bluesky/sirepo_bluesky.py` & `sirepo-bluesky-0.7.0/sirepo_bluesky/sirepo_bluesky.py`

 * *Files 19% similar despite different names*

```diff
@@ -115,14 +115,57 @@
                 "simulationType": self.sim_type,
             },
         )
         if not res["state"] == "ok":
             raise SirepoBlueskyClientException(f"Could not delete simulation: {res}")
         self.sim_id = None
 
+    def compute_crl_characteristics(self, crl_element):
+        res = self._post_json(
+            "stateless-compute",
+            {
+                "method": "crl_characteristics",
+                "optical_element": crl_element,
+                "photon_energy": self.data["models"]["simulation"]["photonEnergy"],
+                "simulationId": self.sim_id,
+                "simulationType": self.sim_type,
+            },
+        )
+
+        return res
+
+    def compute_crystal_init(self, crystal_element):
+        res = self._post_json(
+            "stateless-compute",
+            {
+                "method": "crystal_init",
+                "optical_element": crystal_element,
+                "simulationId": self.sim_id,
+                "simulationType": self.sim_type,
+            },
+        )
+        return res
+
+    def compute_crystal_orientation(self, crystal_element):
+        res_init = self.compute_crystal_init(crystal_element)
+        if res_init.pop("state") != "completed":
+            raise SirepoBlueskyClientException("crystal_init returned error state")
+        res = self._post_json(
+            "stateless-compute",
+            {
+                "method": "crystal_orientation",
+                "optical_element": dict(res_init),
+                "photon_energy": self.data["models"]["simulation"]["photonEnergy"],
+                "simulationId": self.sim_id,
+                "simulationType": self.sim_type,
+            },
+        )
+
+        return res
+
     def compute_grazing_orientation(self, optical_element):
         res = self._post_json(
             "stateless-compute",
             {
                 "method": "compute_grazing_orientation",
                 "optical_element": optical_element,
                 "simulationId": self.sim_id,
@@ -156,14 +199,48 @@
         if not hasattr(self, "cookies"):
             raise Exception("must call auth() before get_datafile()")
         url = f"download-data-file/{self.sim_type}/{self.sim_id}/{self.data['report']}/{file_index}"
         response = requests.get(f"{self.server}/{url}", cookies=self.cookies)
         self._assert_success(response, url)
         return response.content
 
+    def process_beam_parameters(self):
+        res = self._post_json(
+            "stateless-compute",
+            {
+                "ebeam": self.data["models"]["electronBeam"],
+                "ebeam_position": self.data["models"]["electronBeamPosition"],
+                "method": "process_beam_parameters",
+                "simulationId": self.sim_id,
+                "simulationType": self.sim_type,
+                "source_type": self.data["models"]["simulation"]["sourceType"],
+                "undulator_length": self.data["models"]["undulator"]["length"],
+                "undulator_period": self.data["models"]["undulator"]["period"] / 1000.0,
+                "undulator_type": self.data["models"]["tabulatedUndulator"]["undulatorType"],
+            },
+        )
+        return res
+
+    def process_undulator_definition(self):
+        res = self._post_json(
+            "stateless-compute",
+            {
+                "amplitude": self.data["models"]["undulator"]["verticalAmplitude"],
+                "method": "process_undulator_definition",
+                "methodSignature": "process_undulator_definitionverticalDeflectingParameter",
+                "simulationId": self.sim_id,
+                "simulationType": self.sim_type,
+                # Could not locate undulator_definition in source code, using "B" as a placeholder
+                "undulator_definition": "B",
+                "undulator_parameter": self.data["models"]["undulator"]["horizontalDeflectingParameter"],
+                "undulator_period": self.data["models"]["undulator"]["period"] / 1000.0,
+            },
+        )
+        return res
+
     def simulation_list(self):
         """Returns a list of simulations for the authenticated user."""
         return self._post_json("simulation-list", dict(simulationType=self.sim_type))
 
     @staticmethod
     def update_grazing_vectors(data_to_update, grazing_vectors_params):
         """Update grazing angle vectors"""
```

### Comparing `sirepo-bluesky-0.6.2/sirepo_bluesky/sirepo_flyer.py` & `sirepo-bluesky-0.7.0/sirepo_bluesky/sirepo_flyer.py`

 * *Files identical despite different names*

### Comparing `sirepo-bluesky-0.6.2/sirepo_bluesky/sirepo_ophyd.py` & `sirepo-bluesky-0.7.0/sirepo_bluesky/sirepo_ophyd.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import copy
 import datetime
 import hashlib
 import json
 import logging
 import time
-from collections import deque, namedtuple
+from collections import OrderedDict, deque, namedtuple
 from pathlib import Path
 
 import inflection
 from event_model import compose_resource
 from ophyd import Component as Cpt
 from ophyd import Device, Signal
 from ophyd.sim import NullStatus, new_uid
@@ -73,15 +73,20 @@
 
         return NullStatus()
 
 
 class SirepoWatchpoint(DeviceWithJSONData):
     image = Cpt(ExternalFileReference, kind="normal")
     shape = Cpt(Signal)
-    mean = Cpt(Signal, kind="hinted")
+    flux = Cpt(Signal, kind="hinted")
+    mean = Cpt(Signal, kind="normal")
+    x = Cpt(Signal, kind="normal")
+    y = Cpt(Signal, kind="normal")
+    fwhm_x = Cpt(Signal, kind="normal")
+    fwhm_y = Cpt(Signal, kind="normal")
     photon_energy = Cpt(Signal, kind="normal")
     horizontal_extent = Cpt(Signal)
     vertical_extent = Cpt(Signal)
 
     def __init__(
         self,
         *args,
@@ -148,15 +153,20 @@
         elif sim_type == "shadow":
             nbins = conn_data["models"][conn_data["report"]]["histogramBins"]
             ret = read_shadow_file(sim_result_file, histogram_bins=nbins)
             self._resource_document["resource_kwargs"]["histogram_bins"] = nbins
 
         def update_components(_data):
             self.shape.put(_data["shape"])
+            self.flux.put(_data["flux"])
             self.mean.put(_data["mean"])
+            self.x.put(_data["x"])
+            self.y.put(_data["y"])
+            self.fwhm_x.put(_data["fwhm_x"])
+            self.fwhm_y.put(_data["fwhm_y"])
             self.photon_energy.put(_data["photon_energy"])
             self.horizontal_extent.put(_data["horizontal_extent"])
             self.vertical_extent.put(_data["vertical_extent"])
 
         update_components(ret)
 
         datum_document = self._datum_factory(datum_kwargs={})
@@ -229,15 +239,20 @@
         if sim_type == "srw":
             ndim = 1
             ret = read_srw_file(sim_result_file, ndim=ndim)
             self._resource_document["resource_kwargs"]["ndim"] = ndim
 
         def update_components(_data):
             self.shape.put(_data["shape"])
+            self.flux.put(_data["flux"])
             self.mean.put(_data["mean"])
+            self.x.put(_data["x"])
+            self.y.put(_data["y"])
+            self.fwhm_x.put(_data["fwhm_x"])
+            self.fwhm_y.put(_data["fwhm_y"])
             self.photon_energy.put(_data["photon_energy"])
             self.horizontal_extent.put(_data["horizontal_extent"])
             self.vertical_extent.put(_data["vertical_extent"])
 
         update_components(ret)
 
         datum_document = self._datum_factory(datum_kwargs={})
@@ -307,18 +322,82 @@
             "tangentialVectorX",
             "tangentialVectorY",
         ]:
             getattr(self.parent, cpt).put(ret[cpt])
         return NullStatus()
 
 
-def create_classes(sirepo_data, connection, create_objects=True, extra_model_fields=[]):
+class SirepoSignalCRL(SirepoSignal):
+    def set(self, value):
+        super().set(value)
+        ret = self.parent.connection.compute_crl_characteristics(self._sirepo_dict)
+        # State is added to the ret dict from compute_crl_characteristics and we
+        # want to make sure the crl element is updated properly when parameters are changed.
+        ret.pop("state")
+        # Update crl element
+        for cpt in ["absoluteFocusPosition", "focalDistance"]:
+            getattr(self.parent, cpt).put(ret[cpt])
+        return NullStatus()
+
+
+class SirepoSignalCrystal(SirepoSignal):
+    def set(self, value):
+        super().set(value)
+        ret = self.parent.connection.compute_crystal_orientation(self._sirepo_dict)
+        # State is added to the ret dict from compute_crystal_orientation and we
+        # want to make sure the crystal element is updated properly when parameters are changed.
+        ret.pop("state")
+        # Update crystal element
+        for cpt in [
+            "dSpacing",
+            "grazingAngle",
+            "nvx",
+            "nvy",
+            "nvz",
+            "outframevx",
+            "outframevy",
+            "outoptvx",
+            "outoptvy",
+            "outoptvz",
+            "psi0i",
+            "psi0r",
+            "psiHBi",
+            "psiHBr",
+            "psiHi",
+            "psiHr",
+            "tvx",
+            "tvy",
+        ]:
+            getattr(self.parent, cpt).put(ret[cpt])
+        return NullStatus()
+
+
+SimplePropagationConfig = namedtuple(
+    "PropagationConfig",
+    "resize_before resize_after precision propagator_type "
+    + "fourier_resize hrange_mod hres_mod vrange_mod vres_mod",
+)
+
+
+class PropagationConfig(SimplePropagationConfig):
+    read_attrs = list(SimplePropagationConfig._fields)
+    component_names = SimplePropagationConfig._fields
+
+    def read(self):
+        read_attrs = self.read_attrs
+        propagation_read = OrderedDict()
+        for field in read_attrs:
+            propagation_read[field] = getattr(self, field).read()
+        return propagation_read
+
+
+def create_classes(connection, create_objects=True, extra_model_fields=[]):
     classes = {}
     objects = {}
-    data = copy.deepcopy(sirepo_data)
+    data = copy.deepcopy(connection.data)
 
     sim_type = connection.sim_type
 
     SimTypeConfig = namedtuple("SimTypeConfig", "element_location class_name_field")
 
     srw_config = SimTypeConfig("beamline", "title")
     shadow_config = SimTypeConfig("beamline", "title")
@@ -384,28 +463,56 @@
             for k, v in el.items():
                 if (
                     "type" in el
                     and el["type"] in ["sphericalMirror", "toroidalMirror", "ellipsoidMirror"]
                     and k == "grazingAngle"
                 ):
                     cpt_class = SirepoSignalGrazingAngle
+                elif "type" in el and el["type"] == "crl" and k not in ["absoluteFocusPosition", "focalDistance"]:
+                    cpt_class = SirepoSignalCRL
+                elif (
+                    "type" in el
+                    and el["type"] == "crystal"
+                    and k
+                    not in [
+                        "dSpacing",
+                        "grazingAngle",
+                        "nvx",
+                        "nvy",
+                        "nvz",
+                        "outframevx",
+                        "outframevy",
+                        "outoptvx",
+                        "outoptvy",
+                        "outoptvz",
+                        "psi0i",
+                        "psi0r",
+                        "psiHBi",
+                        "psiHBr",
+                        "psiHi",
+                        "psiHr",
+                        "tvx",
+                        "tvy",
+                    ]
+                ):
+                    cpt_class = SirepoSignalCrystal
                 else:
                     # TODO: Cover the cases for mirror and crystal grazing angles
                     cpt_class = SirepoSignal
 
                 if "type" in el and el["type"] not in ["undulator", "intensityReport"]:
-                    sirepo_dict = sirepo_data["models"][model_field][i]
+                    sirepo_dict = connection.data["models"][model_field][i]
                 elif sim_type == "madx" and model_field in ["rpnVariables", "commands"]:
-                    sirepo_dict = sirepo_data["models"][model_field][i]
+                    sirepo_dict = connection.data["models"][model_field][i]
                 else:
-                    sirepo_dict = sirepo_data["models"][model_field]
+                    sirepo_dict = connection.data["models"][model_field]
 
                 components[k] = Cpt(
                     cpt_class,
-                    value=v,
+                    value=(float(v) if type(v) is int else v),
                     sirepo_dict=sirepo_dict,
                     sirepo_param=k,
                 )
             components.update(**extra_kwargs)
 
             cls = type(
                 class_name,
@@ -413,8 +520,41 @@
                 components,
             )
 
             classes[object_name] = cls
             if create_objects:
                 objects[object_name] = cls(name=object_name)
 
+            if sim_type == "srw" and model_field == "beamline":
+                prop_params = connection.data["models"]["propagation"][str(el["id"])][0]
+                sirepo_propagation = []
+                object_name += "_propagation"
+                for i in range(9):
+                    sirepo_propagation.append(
+                        SirepoSignal(
+                            name=f"{object_name}_{SimplePropagationConfig._fields[i]}",
+                            value=float(prop_params[i]),
+                            sirepo_dict=prop_params,
+                            sirepo_param=i,
+                        )
+                    )
+                if create_objects:
+                    objects[object_name] = PropagationConfig(*sirepo_propagation[:])
+
+        if sim_type == "srw":
+            post_prop_params = connection.data["models"]["postPropagation"]
+            sirepo_propagation = []
+            object_name = "post_propagation"
+            for i in range(9):
+                sirepo_propagation.append(
+                    SirepoSignal(
+                        name=f"{object_name}_{SimplePropagationConfig._fields[i]}",
+                        value=float(post_prop_params[i]),
+                        sirepo_dict=post_prop_params,
+                        sirepo_param=i,
+                    )
+                )
+            classes["propagation_parameters"] = PropagationConfig
+            if create_objects:
+                objects[object_name] = PropagationConfig(*sirepo_propagation[:])
+
     return classes, objects
```

### Comparing `sirepo-bluesky-0.6.2/sirepo_bluesky/srw_handler.py` & `sirepo-bluesky-0.7.0/sirepo_bluesky/srw_handler.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,46 @@
 import numpy as np
 import srwpy.uti_plot_com as srw_io
 
+from . import utils
+
 
 def read_srw_file(filename, ndim=2):
     data, mode, ranges, labels, units = srw_io.file_load(filename)
     data = np.array(data)
     if ndim == 2:
         data = data.reshape((ranges[8], ranges[5]), order="C")
         photon_energy = ranges[0]
     elif ndim == 1:
         photon_energy = np.linspace(*ranges[:3])
     else:
         raise ValueError(f"The value ndim={ndim} is not supported.")
 
-    return {
+    horizontal_extent = np.array(ranges[3:5])
+    vertical_extent = np.array(ranges[6:8])
+
+    ret = {
         "data": data,
         "shape": data.shape,
-        "mean": np.mean(data),
+        "flux": data.sum(),
+        "mean": data.mean(),
         "photon_energy": photon_energy,
-        "horizontal_extent": ranges[3:5],
-        "vertical_extent": ranges[6:8],
-        # 'mode': mode,
+        "horizontal_extent": horizontal_extent,
+        "vertical_extent": vertical_extent,
         "labels": labels,
         "units": units,
     }
 
+    if ndim == 1:
+        ret.update({key: np.nan for key in ["x", "y", "fwhm_x", "fwhm_y"]})
+    if ndim == 2:
+        ret.update(utils.get_beam_stats(data, horizontal_extent, vertical_extent))
+
+    return ret
+
 
 class SRWFileHandler:
     specs = {"srw"}
 
     def __init__(self, filename, ndim=2):
         self._name = filename
         self._ndim = ndim
```

### Comparing `sirepo-bluesky-0.6.2/sirepo_bluesky/tests/conftest.py` & `sirepo-bluesky-0.7.0/sirepo_bluesky/tests/conftest.py`

 * *Files 10% similar despite different names*

```diff
@@ -62,14 +62,21 @@
 @pytest.fixture(scope="function")
 def make_dirs():
     root_dir = "/tmp/sirepo-bluesky-data"
     _ = make_dir_tree(datetime.datetime.now().year, base_path=root_dir)
 
 
 @pytest.fixture(scope="function")
+def srw_empty_simulation(make_dirs):
+    connection = SirepoBluesky("http://localhost:8000")
+    data, _ = connection.auth("srw", "emptysim")
+    return connection
+
+
+@pytest.fixture(scope="function")
 def srw_youngs_double_slit_simulation(make_dirs):
     connection = SirepoBluesky("http://localhost:8000")
     data, _ = connection.auth("srw", "00000000")
     return connection
 
 
 @pytest.fixture(scope="function")
@@ -90,14 +97,21 @@
 def srw_ari_simulation(make_dirs):
     connection = SirepoBluesky("http://localhost:8000")
     data, _ = connection.auth("srw", "00000003")
     return connection
 
 
 @pytest.fixture(scope="function")
+def srw_chx_simulation(make_dirs):
+    connection = SirepoBluesky("http://localhost:8000")
+    data, _ = connection.auth("srw", "HXV1JQ5c")
+    return connection
+
+
+@pytest.fixture(scope="function")
 def shadow_basic_simulation(make_dirs):
     connection = SirepoBluesky("http://localhost:8000")
     data, _ = connection.auth("shadow", "00000001")
     return connection
 
 
 @pytest.fixture(scope="function")
```

### Comparing `sirepo-bluesky-0.6.2/sirepo_bluesky/tests/test_bl_elements_as_ophyd_objs.py` & `sirepo-bluesky-0.7.0/sirepo_bluesky/tests/test_bl_elements_as_ophyd_objs.py`

 * *Files 27% similar despite different names*

```diff
@@ -13,31 +13,41 @@
 import tfs
 
 from sirepo_bluesky.madx_flyer import MADXFlyer
 from sirepo_bluesky.sirepo_ophyd import BeamStatisticsReport, create_classes
 
 
 def test_beamline_elements_as_ophyd_objects(srw_tes_simulation):
-    classes, objects = create_classes(srw_tes_simulation.data, connection=srw_tes_simulation)
+    classes, objects = create_classes(connection=srw_tes_simulation)
 
     for name, obj in objects.items():
         pprint.pprint(obj.read())
 
     globals().update(**objects)
 
     print(mono_crystal1.summary())  # noqa
     pprint.pprint(mono_crystal1.read())  # noqa
 
 
+def test_empty_simulation(srw_empty_simulation):
+    classes, objects = create_classes(connection=srw_empty_simulation)
+    globals().update(**objects)
+
+    assert not srw_empty_simulation.data["models"]["beamline"]
+    objects.pop("post_propagation")
+    assert not objects
+
+
 @pytest.mark.parametrize("method", ["set", "put"])
 def test_beamline_elements_set_put(srw_tes_simulation, method):
-    classes, objects = create_classes(srw_tes_simulation.data, connection=srw_tes_simulation)
+    classes, objects = create_classes(connection=srw_tes_simulation)
     globals().update(**objects)
 
-    for i, (k, v) in enumerate(objects.items()):
+    i = 0
+    for k, v in objects.items():
         if "element_position" in v.component_names:
             old_value = v.element_position.get()
             old_sirepo_value = srw_tes_simulation.data["models"]["beamline"][i]["position"]
 
             getattr(v.element_position, method)(old_value + 100)
 
             new_value = v.element_position.get()
@@ -47,19 +57,110 @@
                 f"\n  Changed: {old_value} -> {new_value}\n   Sirepo: {old_sirepo_value} -> {new_sirepo_value}\n"
             )
 
             assert old_value == old_sirepo_value
             assert new_value == new_sirepo_value
             assert new_value != old_value
             assert abs(new_value - (old_value + 100)) < 1e-8
+            i += 1
+
+
+@pytest.mark.parametrize("method", ["set", "put"])
+def test_crl_calculation(srw_chx_simulation, method):
+    classes, objects = create_classes(connection=srw_chx_simulation)
+    globals().update(**objects)
+
+    params_before = copy.deepcopy(crl1.tipRadius._sirepo_dict)  # noqa F821
+    params_before.pop("tipRadius")
+
+    getattr(crl1.tipRadius, method)(2000)  # noqa F821
+
+    params_after = copy.deepcopy(crl1.tipRadius._sirepo_dict)  # noqa F821
+    params_after.pop("tipRadius")
+
+    params_diff = list(dictdiffer.diff(params_before, params_after))
+    assert len(params_diff) > 0  # should not be empty
+
+    expected_values = {
+        "absoluteFocusPosition": -6.195573642892285,
+        "focalDistance": 237.666984823537,
+    }
+
+    actual_values = {
+        "absoluteFocusPosition": crl1.absoluteFocusPosition.get(),  # noqa F821
+        "focalDistance": crl1.focalDistance.get(),  # noqa F821
+    }
+
+    assert not list(dictdiffer.diff(expected_values, actual_values))
+
+
+@pytest.mark.parametrize("method", ["set", "put"])
+def test_crystal_calculation(srw_tes_simulation, method):
+    classes, objects = create_classes(connection=srw_tes_simulation)
+    globals().update(**objects)
+
+    params_before = copy.deepcopy(mono_crystal1.energy._sirepo_dict)  # noqa F821
+    params_before.pop("energy")
+
+    getattr(mono_crystal1.energy, method)(2000)  # noqa F821
+
+    params_after = copy.deepcopy(mono_crystal1.energy._sirepo_dict)  # noqa F821
+    params_after.pop("energy")
+
+    params_diff = list(dictdiffer.diff(params_before, params_after))
+    assert len(params_diff) > 0  # should not be empty
+
+    expected_values = {
+        "dSpacing": 3.1355713563754857,
+        "grazingAngle": 1419.9107955732711,
+        "nvx": 0,
+        "nvy": 0.15031366142760424,
+        "nvz": -0.9886383581412506,
+        "outframevx": 1.0,
+        "outframevy": 0.0,
+        "outoptvx": 0.0,
+        "outoptvy": 0.29721170287997256,
+        "outoptvz": -0.9548116063764552,
+        "psi0i": 6.530421915581681e-05,
+        "psi0r": -0.00020558072555357544,
+        "psiHBi": 4.559368494529194e-05,
+        "psiHBr": -0.00010207663788071082,
+        "psiHi": 4.559368494529194e-05,
+        "psiHr": -0.00010207663788071082,
+        "tvx": 0,
+        "tvy": 0.9886383581412506,
+    }
+
+    actual_values = {
+        "dSpacing": mono_crystal1.dSpacing.get(),  # noqa F821
+        "grazingAngle": mono_crystal1.grazingAngle.get(),  # noqa F821
+        "nvx": mono_crystal1.nvx.get(),  # noqa F821
+        "nvy": mono_crystal1.nvy.get(),  # noqa F821
+        "nvz": mono_crystal1.nvz.get(),  # noqa F821
+        "outframevx": mono_crystal1.outframevx.get(),  # noqa F821
+        "outframevy": mono_crystal1.outframevy.get(),  # noqa F821
+        "outoptvx": mono_crystal1.outoptvx.get(),  # noqa F821
+        "outoptvy": mono_crystal1.outoptvy.get(),  # noqa F821
+        "outoptvz": mono_crystal1.outoptvz.get(),  # noqa F821
+        "psi0i": mono_crystal1.psi0i.get(),  # noqa F821
+        "psi0r": mono_crystal1.psi0r.get(),  # noqa F821
+        "psiHBi": mono_crystal1.psiHBi.get(),  # noqa F821
+        "psiHBr": mono_crystal1.psiHBr.get(),  # noqa F821
+        "psiHi": mono_crystal1.psiHi.get(),  # noqa F821
+        "psiHr": mono_crystal1.psiHr.get(),  # noqa F821
+        "tvx": mono_crystal1.tvx.get(),  # noqa F821
+        "tvy": mono_crystal1.tvy.get(),  # noqa F821
+    }
+
+    assert not list(dictdiffer.diff(expected_values, actual_values))
 
 
 @pytest.mark.parametrize("method", ["set", "put"])
 def test_grazing_angle_calculation(srw_tes_simulation, method):
-    classes, objects = create_classes(srw_tes_simulation.data, connection=srw_tes_simulation)
+    classes, objects = create_classes(connection=srw_tes_simulation)
     globals().update(**objects)
 
     params_before = copy.deepcopy(toroid.grazingAngle._sirepo_dict)  # noqa F821
     params_before.pop("grazingAngle")
 
     getattr(toroid.grazingAngle, method)(10)  # noqa F821
 
@@ -85,28 +186,27 @@
         "tvy": toroid.tangentialVectorY.get(),  # noqa F821
     }
 
     assert not list(dictdiffer.diff(expected_vector_values, actual_vector_values))
 
 
 def test_beamline_elements_simple_connection(srw_basic_simulation):
-    classes, objects = create_classes(srw_basic_simulation.data, connection=srw_basic_simulation)
+    classes, objects = create_classes(connection=srw_basic_simulation)
 
     for name, obj in objects.items():
         pprint.pprint(obj.read())
 
     globals().update(**objects)
 
     print(watchpoint.summary())  # noqa F821
     pprint.pprint(watchpoint.read())  # noqa F821
 
 
 def test_srw_source_with_run_engine(RE, db, srw_ari_simulation, num_steps=5):
     classes, objects = create_classes(
-        srw_ari_simulation.data,
         connection=srw_ari_simulation,
         extra_model_fields=["undulator", "intensityReport"],
     )
     globals().update(**objects)
 
     undulator.verticalAmplitude.kind = "hinted"  # noqa F821
 
@@ -153,16 +253,41 @@
     ax.grid()
     ax.legend()
     ax.set_title("Single-Electron Spectrum vs. Vertical Magnetic Field")
     fig.savefig("ses-vs-ampl.png")
     # plt.show()
 
 
+def test_srw_propagation_with_run_engine(RE, db, srw_chx_simulation, num_steps=5):
+    classes, objects = create_classes(connection=srw_chx_simulation)
+    globals().update(**objects)
+
+    post_propagation.hrange_mod.kind = "hinted"  # noqa F821
+
+    (uid,) = RE(bp.scan([sample], post_propagation.hrange_mod, 0.1, 0.3, num_steps))  # noqa F821
+    hdr = db[uid]
+    tbl = hdr.table(fill=True)
+    print(tbl)
+
+    # Check that the duration for each step in the simulation is positive:
+    sim_durations = np.array(tbl["sample_duration"])
+    assert (sim_durations > 0.0).all(), "Simulation steps did not properly run."
+
+    sample_image = []
+    for i in range(num_steps):
+        sample_image.append(np.array(list(hdr.data("sample_image"))[i]))
+
+    # Check the shape of the image data is right and that hrange_mod was properly changed:
+    for i, hrange_mod in enumerate(np.linspace(0.1, 0.3, num_steps)):
+        assert json.loads(tbl["sample_sirepo_data_json"][i + 1])["models"]["postPropagation"][5] == hrange_mod
+        assert sample_image[i].shape == (294, int(hrange_mod * 1760))
+
+
 def test_shadow_with_run_engine(RE, db, shadow_tes_simulation, num_steps=5):
-    classes, objects = create_classes(shadow_tes_simulation.data, connection=shadow_tes_simulation)
+    classes, objects = create_classes(connection=shadow_tes_simulation)
     globals().update(**objects)
 
     aperture.horizontalSize.kind = "hinted"  # noqa F821
 
     (uid,) = RE(bp.scan([w9], aperture.horizontalSize, 0, 2, num_steps))  # noqa F821
     hdr = db[uid]
     tbl = hdr.table(fill=True)
@@ -199,15 +324,15 @@
             resource_files.append(os.path.basename(doc["resource_path"]))
 
     # Check that all resource files are unique:
     assert len(set(resource_files)) == num_steps
 
 
 def test_beam_statistics_report_only(RE, db, shadow_tes_simulation):
-    classes, objects = create_classes(shadow_tes_simulation.data, connection=shadow_tes_simulation)
+    classes, objects = create_classes(connection=shadow_tes_simulation)
     globals().update(**objects)
 
     bsr = BeamStatisticsReport(name="bsr", connection=shadow_tes_simulation)
 
     toroid.r_maj.kind = "hinted"  # noqa F821
 
     scan_range = (10_000, 50_000, 21)
@@ -239,15 +364,15 @@
     )
     ax.set_title(title)
     fig.savefig("TES-Shadow-timing.png")
     # plt.show()
 
 
 def test_beam_statistics_report_and_watchpoint(RE, db, shadow_tes_simulation):
-    classes, objects = create_classes(shadow_tes_simulation.data, connection=shadow_tes_simulation)
+    classes, objects = create_classes(connection=shadow_tes_simulation)
     globals().update(**objects)
 
     bsr = BeamStatisticsReport(name="bsr", connection=shadow_tes_simulation)
 
     toroid.r_maj.kind = "hinted"  # noqa F821
 
     (uid,) = RE(bp.scan([bsr, w9], toroid.r_maj, 10000, 50000, 5))  # noqa F821
@@ -274,15 +399,15 @@
     ]
 
 
 @pytest.mark.parametrize("method", ["set", "put"])
 def test_mad_x_elements_set_put(madx_resr_storage_ring_simulation, method):
     connection = madx_resr_storage_ring_simulation
     data = connection.data
-    classes, objects = create_classes(data, connection=connection)
+    classes, objects = create_classes(connection=connection)
     globals().update(**objects)
 
     for i, (k, v) in enumerate(objects.items()):
         old_value = v.l.get()  # l is length
         old_sirepo_value = data["models"]["elements"][i]["l"]
 
         getattr(v.l, method)(old_value + 10)
@@ -296,29 +421,27 @@
         assert new_value == new_sirepo_value
         assert new_value != old_value
         assert abs(new_value - (old_value + 10)) < 1e-8
 
 
 def test_mad_x_elements_simple_connection(madx_bl2_triplet_tdc_simulation):
     connection = madx_bl2_triplet_tdc_simulation
-    data = connection.data
-    classes, objects = create_classes(data, connection=connection)
+    classes, objects = create_classes(connection=connection)
     for name, obj in objects.items():
         pprint.pprint(obj.read())
 
     globals().update(**objects)
 
     print(bpm5.summary())  # noqa
     pprint.pprint(bpm5.read())  # noqa
 
 
 def test_madx_with_run_engine(RE, db, madx_bl2_triplet_tdc_simulation):
     connection = madx_bl2_triplet_tdc_simulation
-    data = connection.data
-    classes, objects = create_classes(data, connection=connection)
+    classes, objects = create_classes(connection=connection)
     globals().update(**objects)
 
     madx_flyer = MADXFlyer(
         connection=connection,
         root_dir="/tmp/sirepo-bluesky-data",
         report="elementAnimation250-20",
     )
@@ -347,15 +470,14 @@
             )
 
 
 def test_madx_variables_with_run_engine(RE, db, madx_bl2_triplet_tdc_simulation):
     connection = madx_bl2_triplet_tdc_simulation
     data = connection.data
     classes, objects = create_classes(
-        data,
         connection=connection,
         extra_model_fields=["rpnVariables"],
     )
 
     globals().update(**objects)
 
     assert len(objects) == len(data["models"]["elements"]) + len(data["models"]["rpnVariables"])
@@ -382,15 +504,14 @@
     assert len(tbl["madx_flyer_BETY"]) == expected_data_len
 
 
 def test_madx_commands_with_run_engine(RE, db, madx_bl2_triplet_tdc_simulation):
     connection = madx_bl2_triplet_tdc_simulation
     data = connection.data
     classes, objects = create_classes(
-        data,
         connection=connection,
         extra_model_fields=["commands"],
     )
 
     globals().update(**objects)
     pprint.pprint(classes, sort_dicts=False)
 
@@ -418,15 +539,14 @@
     assert len(tbl["madx_flyer_BETY"]) == expected_data_len
 
 
 def test_madx_variables_and_commands_with_run_engine(RE, db, madx_bl2_triplet_tdc_simulation):
     connection = madx_bl2_triplet_tdc_simulation
     data = connection.data
     classes, objects = create_classes(
-        data,
         connection=connection,
         extra_model_fields=["rpnVariables", "commands"],
     )
 
     globals().update(**objects)
 
     assert len(objects) == len(data["models"]["elements"]) + len(data["models"]["rpnVariables"]) + len(
```

### Comparing `sirepo-bluesky-0.6.2/sirepo_bluesky/tests/test_sirepo_flyer.py` & `sirepo-bluesky-0.7.0/sirepo_bluesky/tests/test_sirepo_flyer.py`

 * *Files identical despite different names*

### Comparing `sirepo-bluesky-0.6.2/sirepo_bluesky.egg-info/SOURCES.txt` & `sirepo-bluesky-0.7.0/sirepo_bluesky.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,10 @@
-AUTHORS.rst
-CONTRIBUTING.rst
 LICENSE
 MANIFEST.in
-README.rst
+README.md
 pyproject.toml
 requirements.txt
 setup.cfg
 setup.py
 versioneer.py
 docs/Makefile
 docs/make.bat
@@ -16,26 +14,27 @@
 docs/source/installation.rst
 docs/source/release-history.rst
 docs/source/simulations.rst
 sirepo_bluesky/__init__.py
 sirepo_bluesky/_version.py
 sirepo_bluesky/madx_flyer.py
 sirepo_bluesky/madx_handler.py
-sirepo_bluesky/shadow_detector.py
 sirepo_bluesky/shadow_handler.py
 sirepo_bluesky/sirepo_bluesky.py
 sirepo_bluesky/sirepo_flyer.py
 sirepo_bluesky/sirepo_ophyd.py
-sirepo_bluesky/srw_detector.py
 sirepo_bluesky/srw_handler.py
 sirepo_bluesky.egg-info/PKG-INFO
 sirepo_bluesky.egg-info/SOURCES.txt
 sirepo_bluesky.egg-info/dependency_links.txt
+sirepo_bluesky.egg-info/entry_points.txt
 sirepo_bluesky.egg-info/requires.txt
 sirepo_bluesky.egg-info/top_level.txt
 sirepo_bluesky/tests/__init__.py
 sirepo_bluesky/tests/conftest.py
 sirepo_bluesky/tests/test_bl_elements_as_ophyd_objs.py
+sirepo_bluesky/tests/test_converter.py
 sirepo_bluesky/tests/test_entrypoint.py
-sirepo_bluesky/tests/test_shadow_det.py
 sirepo_bluesky/tests/test_sirepo_flyer.py
-sirepo_bluesky/tests/test_srw_det.py
+sirepo_bluesky/tests/test_stateless_compute.py
+sirepo_bluesky/utils/__init__.py
+sirepo_bluesky/utils/json_yaml_converter.py
```

### Comparing `sirepo-bluesky-0.6.2/versioneer.py` & `sirepo-bluesky-0.7.0/versioneer.py`

 * *Files identical despite different names*

