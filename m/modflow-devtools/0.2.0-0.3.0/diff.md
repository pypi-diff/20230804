# Comparing `tmp/modflow-devtools-0.2.0.tar.gz` & `tmp/modflow-devtools-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modflow-devtools-0.2.0.tar", last modified: Wed Jul 26 22:03:12 2023, max compression
+gzip compressed data, was "modflow-devtools-0.3.0.tar", last modified: Fri Aug  4 01:32:00 2023, max compression
```

## Comparing `modflow-devtools-0.2.0.tar` & `modflow-devtools-0.3.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 wes        (501) staff       (20)        0 2023-07-26 22:03:12.090946 modflow-devtools-0.2.0/
--rwxr-xr-x   0 wes        (501) staff       (20)     1627 2023-07-26 18:09:37.000000 modflow-devtools-0.2.0/LICENSE.md
--rw-r--r--   0 wes        (501) staff       (20)      163 2023-07-26 21:57:48.000000 modflow-devtools-0.2.0/MANIFEST.in
--rw-r--r--   0 wes        (501) staff       (20)     5069 2023-07-26 22:03:12.089895 modflow-devtools-0.2.0/PKG-INFO
--rw-r--r--   0 wes        (501) staff       (20)     3856 2023-07-26 21:57:48.000000 modflow-devtools-0.2.0/README.md
-drwxr-xr-x   0 wes        (501) staff       (20)        0 2023-07-26 22:03:12.074693 modflow-devtools-0.2.0/modflow_devtools/
--rw-r--r--   0 wes        (501) staff       (20)      248 2023-07-26 21:57:48.000000 modflow-devtools-0.2.0/modflow_devtools/__init__.py
--rw-r--r--   0 wes        (501) staff       (20)      984 2023-07-26 18:09:37.000000 modflow-devtools-0.2.0/modflow_devtools/build.py
--rw-r--r--   0 wes        (501) staff       (20)     1029 2023-07-26 18:09:37.000000 modflow-devtools-0.2.0/modflow_devtools/case.py
--rw-r--r--   0 wes        (501) staff       (20)     7352 2023-07-26 21:57:48.000000 modflow-devtools-0.2.0/modflow_devtools/context.py
--rw-r--r--   0 wes        (501) staff       (20)    17531 2023-07-26 21:57:48.000000 modflow-devtools-0.2.0/modflow_devtools/download.py
--rw-r--r--   0 wes        (501) staff       (20)     2487 2023-07-26 21:57:48.000000 modflow-devtools-0.2.0/modflow_devtools/executables.py
--rw-r--r--   0 wes        (501) staff       (20)    11854 2023-07-26 21:57:48.000000 modflow-devtools-0.2.0/modflow_devtools/fixtures.py
--rw-r--r--   0 wes        (501) staff       (20)     1732 2023-07-26 18:09:37.000000 modflow-devtools-0.2.0/modflow_devtools/markers.py
--rw-r--r--   0 wes        (501) staff       (20)    11069 2023-07-26 21:57:48.000000 modflow-devtools-0.2.0/modflow_devtools/misc.py
-drwxr-xr-x   0 wes        (501) staff       (20)        0 2023-07-26 22:03:12.089158 modflow-devtools-0.2.0/modflow_devtools/test/
--rw-r--r--   0 wes        (501) staff       (20)        0 2023-07-26 18:09:37.000000 modflow-devtools-0.2.0/modflow_devtools/test/__init__.py
--rw-r--r--   0 wes        (501) staff       (20)     1163 2023-07-26 18:09:37.000000 modflow-devtools-0.2.0/modflow_devtools/test/test_build.py
--rw-r--r--   0 wes        (501) staff       (20)     1788 2023-07-26 18:09:37.000000 modflow-devtools-0.2.0/modflow_devtools/test/test_case.py
--rw-r--r--   0 wes        (501) staff       (20)     3606 2023-07-26 21:57:48.000000 modflow-devtools-0.2.0/modflow_devtools/test/test_download.py
--rw-r--r--   0 wes        (501) staff       (20)     1148 2023-07-26 18:09:37.000000 modflow-devtools-0.2.0/modflow_devtools/test/test_executables.py
--rw-r--r--   0 wes        (501) staff       (20)     8043 2023-07-26 21:57:48.000000 modflow-devtools-0.2.0/modflow_devtools/test/test_fixtures.py
--rw-r--r--   0 wes        (501) staff       (20)      904 2023-07-26 18:09:37.000000 modflow-devtools-0.2.0/modflow_devtools/test/test_markers.py
--rw-r--r--   0 wes        (501) staff       (20)     8476 2023-07-26 21:57:48.000000 modflow-devtools-0.2.0/modflow_devtools/test/test_misc.py
--rw-r--r--   0 wes        (501) staff       (20)     2663 2023-07-26 21:57:48.000000 modflow-devtools-0.2.0/modflow_devtools/test/test_zip.py
--rw-r--r--   0 wes        (501) staff       (20)     5708 2023-07-26 21:57:48.000000 modflow-devtools-0.2.0/modflow_devtools/zip.py
-drwxr-xr-x   0 wes        (501) staff       (20)        0 2023-07-26 22:03:12.079378 modflow-devtools-0.2.0/modflow_devtools.egg-info/
--rw-r--r--   0 wes        (501) staff       (20)     5069 2023-07-26 22:03:12.000000 modflow-devtools-0.2.0/modflow_devtools.egg-info/PKG-INFO
--rw-r--r--   0 wes        (501) staff       (20)      913 2023-07-26 22:03:12.000000 modflow-devtools-0.2.0/modflow_devtools.egg-info/SOURCES.txt
--rw-r--r--   0 wes        (501) staff       (20)        1 2023-07-26 22:03:12.000000 modflow-devtools-0.2.0/modflow_devtools.egg-info/dependency_links.txt
--rw-r--r--   0 wes        (501) staff       (20)        1 2022-07-22 15:19:26.000000 modflow-devtools-0.2.0/modflow_devtools.egg-info/not-zip-safe
--rw-r--r--   0 wes        (501) staff       (20)      235 2023-07-26 22:03:12.000000 modflow-devtools-0.2.0/modflow_devtools.egg-info/requires.txt
--rw-r--r--   0 wes        (501) staff       (20)       17 2023-07-26 22:03:12.000000 modflow-devtools-0.2.0/modflow_devtools.egg-info/top_level.txt
--rw-r--r--   0 wes        (501) staff       (20)     2182 2023-07-26 21:57:48.000000 modflow-devtools-0.2.0/pyproject.toml
--rw-r--r--   0 wes        (501) staff       (20)       38 2023-07-26 22:03:12.091570 modflow-devtools-0.2.0/setup.cfg
--rwxr-xr-x   0 wes        (501) staff       (20)       61 2023-07-26 21:57:48.000000 modflow-devtools-0.2.0/setup.py
--rw-r--r--   0 wes        (501) staff       (20)        5 2023-07-26 21:57:48.000000 modflow-devtools-0.2.0/version.txt
+drwxr-xr-x   0 wes        (501) staff       (20)        0 2023-08-04 01:32:00.455114 modflow-devtools-0.3.0/
+-rwxr-xr-x   0 wes        (501) staff       (20)     1627 2023-07-26 18:09:37.000000 modflow-devtools-0.3.0/LICENSE.md
+-rw-r--r--   0 wes        (501) staff       (20)      163 2023-07-26 21:57:48.000000 modflow-devtools-0.3.0/MANIFEST.in
+-rw-r--r--   0 wes        (501) staff       (20)     4768 2023-08-04 01:32:00.454710 modflow-devtools-0.3.0/PKG-INFO
+-rw-r--r--   0 wes        (501) staff       (20)     3555 2023-08-04 01:30:58.000000 modflow-devtools-0.3.0/README.md
+drwxr-xr-x   0 wes        (501) staff       (20)        0 2023-08-04 01:32:00.403262 modflow-devtools-0.3.0/modflow_devtools/
+-rw-r--r--   0 wes        (501) staff       (20)      248 2023-08-04 01:31:17.000000 modflow-devtools-0.3.0/modflow_devtools/__init__.py
+-rw-r--r--   0 wes        (501) staff       (20)      984 2023-07-26 18:09:37.000000 modflow-devtools-0.3.0/modflow_devtools/build.py
+-rw-r--r--   0 wes        (501) staff       (20)     1029 2023-07-26 18:09:37.000000 modflow-devtools-0.3.0/modflow_devtools/case.py
+-rw-r--r--   0 wes        (501) staff       (20)     7352 2023-07-26 21:57:48.000000 modflow-devtools-0.3.0/modflow_devtools/context.py
+-rw-r--r--   0 wes        (501) staff       (20)    17656 2023-08-04 01:30:58.000000 modflow-devtools-0.3.0/modflow_devtools/download.py
+-rw-r--r--   0 wes        (501) staff       (20)     2487 2023-07-26 21:57:48.000000 modflow-devtools-0.3.0/modflow_devtools/executables.py
+-rw-r--r--   0 wes        (501) staff       (20)    11854 2023-07-26 21:57:48.000000 modflow-devtools-0.3.0/modflow_devtools/fixtures.py
+-rw-r--r--   0 wes        (501) staff       (20)     1732 2023-07-26 18:09:37.000000 modflow-devtools-0.3.0/modflow_devtools/markers.py
+-rw-r--r--   0 wes        (501) staff       (20)    11069 2023-07-26 21:57:48.000000 modflow-devtools-0.3.0/modflow_devtools/misc.py
+drwxr-xr-x   0 wes        (501) staff       (20)        0 2023-08-04 01:32:00.453747 modflow-devtools-0.3.0/modflow_devtools/test/
+-rw-r--r--   0 wes        (501) staff       (20)        0 2023-07-26 18:09:37.000000 modflow-devtools-0.3.0/modflow_devtools/test/__init__.py
+-rw-r--r--   0 wes        (501) staff       (20)     1163 2023-07-26 18:09:37.000000 modflow-devtools-0.3.0/modflow_devtools/test/test_build.py
+-rw-r--r--   0 wes        (501) staff       (20)     1788 2023-07-26 18:09:37.000000 modflow-devtools-0.3.0/modflow_devtools/test/test_case.py
+-rw-r--r--   0 wes        (501) staff       (20)     3606 2023-07-26 21:57:48.000000 modflow-devtools-0.3.0/modflow_devtools/test/test_download.py
+-rw-r--r--   0 wes        (501) staff       (20)     1148 2023-07-26 18:09:37.000000 modflow-devtools-0.3.0/modflow_devtools/test/test_executables.py
+-rw-r--r--   0 wes        (501) staff       (20)     8043 2023-07-26 21:57:48.000000 modflow-devtools-0.3.0/modflow_devtools/test/test_fixtures.py
+-rw-r--r--   0 wes        (501) staff       (20)      904 2023-07-26 18:09:37.000000 modflow-devtools-0.3.0/modflow_devtools/test/test_markers.py
+-rw-r--r--   0 wes        (501) staff       (20)     8476 2023-07-26 21:57:48.000000 modflow-devtools-0.3.0/modflow_devtools/test/test_misc.py
+-rw-r--r--   0 wes        (501) staff       (20)     2663 2023-07-26 21:57:48.000000 modflow-devtools-0.3.0/modflow_devtools/test/test_zip.py
+-rw-r--r--   0 wes        (501) staff       (20)     5708 2023-07-26 21:57:48.000000 modflow-devtools-0.3.0/modflow_devtools/zip.py
+drwxr-xr-x   0 wes        (501) staff       (20)        0 2023-08-04 01:32:00.436144 modflow-devtools-0.3.0/modflow_devtools.egg-info/
+-rw-r--r--   0 wes        (501) staff       (20)     4768 2023-08-04 01:32:00.000000 modflow-devtools-0.3.0/modflow_devtools.egg-info/PKG-INFO
+-rw-r--r--   0 wes        (501) staff       (20)      913 2023-08-04 01:32:00.000000 modflow-devtools-0.3.0/modflow_devtools.egg-info/SOURCES.txt
+-rw-r--r--   0 wes        (501) staff       (20)        1 2023-08-04 01:32:00.000000 modflow-devtools-0.3.0/modflow_devtools.egg-info/dependency_links.txt
+-rw-r--r--   0 wes        (501) staff       (20)        1 2022-07-22 15:19:26.000000 modflow-devtools-0.3.0/modflow_devtools.egg-info/not-zip-safe
+-rw-r--r--   0 wes        (501) staff       (20)      235 2023-08-04 01:32:00.000000 modflow-devtools-0.3.0/modflow_devtools.egg-info/requires.txt
+-rw-r--r--   0 wes        (501) staff       (20)       17 2023-08-04 01:32:00.000000 modflow-devtools-0.3.0/modflow_devtools.egg-info/top_level.txt
+-rw-r--r--   0 wes        (501) staff       (20)     2164 2023-08-04 01:30:58.000000 modflow-devtools-0.3.0/pyproject.toml
+-rw-r--r--   0 wes        (501) staff       (20)       38 2023-08-04 01:32:00.455233 modflow-devtools-0.3.0/setup.cfg
+-rwxr-xr-x   0 wes        (501) staff       (20)       61 2023-07-26 21:57:48.000000 modflow-devtools-0.3.0/setup.py
+-rw-r--r--   0 wes        (501) staff       (20)        5 2023-08-04 01:31:17.000000 modflow-devtools-0.3.0/version.txt
```

### Comparing `modflow-devtools-0.2.0/LICENSE.md` & `modflow-devtools-0.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `modflow-devtools-0.2.0/PKG-INFO` & `modflow-devtools-0.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modflow-devtools
-Version: 0.2.0
+Version: 0.3.0
 Summary: Python tools for MODFLOW development
 Author-email: "Joseph D. Hughes" <modflow@usgs.gov>
 Maintainer-email: "Joseph D. Hughes" <modflow@usgs.gov>
 License: CC0
 Project-URL: Documentation, https://modflow-devtools.readthedocs.io/en/latest/
 Project-URL: Bug Tracker, https://github.com/MODFLOW-USGS/modflow-devtools/issues
 Project-URL: Source Code, https://github.com/MODFLOW-USGS/modflow-devtools
@@ -31,85 +31,75 @@
 [![GitHub tag](https://img.shields.io/github/tag/MODFLOW-USGS/modflow-devtools.svg)](https://github.com/MODFLOW-USGS/modflow-devtools/tags/latest)
 [![PyPI Version](https://img.shields.io/pypi/v/modflow-devtools.png)](https://pypi.python.org/pypi/modflow-devtools)
 [![PyPI Versions](https://img.shields.io/pypi/pyversions/modflow-devtools.png)](https://pypi.python.org/pypi/modflow-devtools)
 [![PyPI Status](https://img.shields.io/pypi/status/modflow-devtools.png)](https://pypi.python.org/pypi/modflow-devtools)
 [![CI](https://github.com/MODFLOW-USGS/modflow-devtools/actions/workflows/ci.yml/badge.svg)](https://github.com/MODFLOW-USGS/modflow-devtools/actions/workflows/ci.yml)
 [![Documentation Status](https://readthedocs.org/projects/modflow-devtools/badge/?version=latest)](https://modflow-devtools.readthedocs.io/en/latest/?badge=latest)
 
-Python tools for MODFLOW development and testing.
+Python development tools for MODFLOW 6.
 
 <!-- START doctoc generated TOC please keep comment here to allow auto update -->
 <!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->
 
+
+- [Use cases](#use-cases)
 - [Requirements](#requirements)
 - [Installation](#installation)
-- [Use cases](#use-cases)
-- [Quickstart](#quickstart)
 - [Documentation](#documentation)
-- [MODFLOW Resources](#modflow-resources)
 
 <!-- END doctoc generated TOC please keep comment here to allow auto update -->
 
+## Use cases
+
+This is a small toolkit for developing MODFLOW 6, FloPy, and related projects. It includes standalone utilities and optional [Pytest](https://github.com/pytest-dev/pytest) extensions.
+
+Standalone utilities include a very minimal GitHub API client, mainly for retrieving release information and downloading assets, and a `ZipFile` subclass that [preserves file permissions](https://stackoverflow.com/questions/39296101/python-zipfile-removes-execute-permissions-from-binaries) (workaround for [Python #15795](https://bugs.python.org/issue15795))
+
+Pytest features include:
+
+- `--keep <path>` tempdir fixtures for [each scope](https://docs.pytest.org/en/stable/how-to/fixtures.html#scope-sharing-fixtures-across-classes-modules-packages-or-session)
+- a [`--smoke` test](https://en.wikipedia.org/wiki/Smoke_testing_(software)) (abbrev. `-S`) CLI option shortcut
+- markers to skip test cases conditional on
+  - operating system
+  - Python packages installed
+  - executables available on the PATH
+- test fixtures for example / test models in
+  - `MODFLOW-USGS/modflow6-examples`
+  - `MODFLOW-USGS/modflow6-testmodels`
+  - `MODFLOW-USGS/modflow6-largetestmodels`
+
 ## Requirements
 
-This project requires Python3.8+. Its only core dependencies are `numpy` and `pytest`.
+Python3.8+, dependency-free, but pairs well with `pytest` and select plugins, e.g.
+
+- [`pytest-dotenv`](https://github.com/quiqua/pytest-dotenv)
+- [`pytest-xdist`](https://github.com/pytest-dev/pytest-xdist)
 
 ## Installation
 
 `modflow-devtools` is available on PyPI and can be installed with pip:
 
 ```shell
 pip install modflow-devtools
 ```
 
-This package pairs well with a few pytest plugins:
-
-- `pytest-cases`
-- `pytest-dotenv`
-- `pytest-xdist`
-
-These and a few other optional dependencies can be installed with:
+Pytest, pytest plugins, and other optional dependencies can be installed with:
 
 ```shell
 pip install "modflow-devtools[test]"
 ```
 
 To install from source and set up a development environment please see the [developer documentation](DEVELOPER.md).
 
-## Use cases
-
-This package contains shared tools for developing and testing MODFLOW 6 and FloPy, including standalone utilities as well as `pytest` fixtures, CLI options, and test cases:
-
-- utilities for retrieving release information and downloading assets from the GitHub API
-- a `ZipFile` subclass that [preserves file permissions](https://stackoverflow.com/questions/39296101/python-zipfile-removes-execute-permissions-from-binaries) (workaround for [Python #15795](https://bugs.python.org/issue15795))
-- a `pytest` CLI option for smoke testing (running a fast subset of cases)
-- a minimal `pytest-cases` framework for reusing test functions and data
-- a set of keepable `pytest` temporary directory fixtures for each scope
-- a set of fixtures to parametrize tests with models from external repos
-  - `MODFLOW-USGS/modflow6-examples`
-  - `MODFLOW-USGS/modflow6-testmodels`
-  - `MODFLOW-USGS/modflow6-largetestmodels`
-- a set of `pytest` markers to conditionally skip test cases based on
-  - operating system
-  - Python packages installed
-  - executables available on the path
-
-## Quickstart
-
 To import `pytest` fixtures in a project consuming `modflow-devtools`, add the following to a `conftest.py` file:
 
 ```python
 pytest_plugins = [ "modflow_devtools.fixtures" ]
 ```
 
-**Note**: `pytest` requires this to be a top-level `conftest.py` file. Nested `conftest.py` files may override or extend this package's fixtures.
+**Note**: this must be a top-level `conftest.py`, which nested `conftest.py` files may then override or extend.
 
 ## Documentation
 
-Usage documentation is available at [modflow-devtools.readthedocs.io](https://modflow-devtools.readthedocs.io/en/latest/).
-
-## MODFLOW Resources
+Docs are available at [modflow-devtools.readthedocs.io](https://modflow-devtools.readthedocs.io/en/latest/).
 
-+ [MODFLOW and Related Programs](https://water.usgs.gov/ogw/modflow/)
-+ [Online guide for MODFLOW-2000](https://water.usgs.gov/nrp/gwsoftware/modflow2000/Guide/)
-+ [Online guide for MODFLOW-2005](https://water.usgs.gov/ogw/modflow/MODFLOW-2005-Guide/)
-+ [Online guide for MODFLOW-NWT](https://water.usgs.gov/ogw/modflow-nwt/MODFLOW-NWT-Guide/)
+For more info on MODFLOW 6 see [the USGS overview](https://water.usgs.gov/ogw/modflow/).
```

### Comparing `modflow-devtools-0.2.0/README.md` & `modflow-devtools-0.3.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -3,85 +3,75 @@
 [![GitHub tag](https://img.shields.io/github/tag/MODFLOW-USGS/modflow-devtools.svg)](https://github.com/MODFLOW-USGS/modflow-devtools/tags/latest)
 [![PyPI Version](https://img.shields.io/pypi/v/modflow-devtools.png)](https://pypi.python.org/pypi/modflow-devtools)
 [![PyPI Versions](https://img.shields.io/pypi/pyversions/modflow-devtools.png)](https://pypi.python.org/pypi/modflow-devtools)
 [![PyPI Status](https://img.shields.io/pypi/status/modflow-devtools.png)](https://pypi.python.org/pypi/modflow-devtools)
 [![CI](https://github.com/MODFLOW-USGS/modflow-devtools/actions/workflows/ci.yml/badge.svg)](https://github.com/MODFLOW-USGS/modflow-devtools/actions/workflows/ci.yml)
 [![Documentation Status](https://readthedocs.org/projects/modflow-devtools/badge/?version=latest)](https://modflow-devtools.readthedocs.io/en/latest/?badge=latest)
 
-Python tools for MODFLOW development and testing.
+Python development tools for MODFLOW 6.
 
 <!-- START doctoc generated TOC please keep comment here to allow auto update -->
 <!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->
 
+
+- [Use cases](#use-cases)
 - [Requirements](#requirements)
 - [Installation](#installation)
-- [Use cases](#use-cases)
-- [Quickstart](#quickstart)
 - [Documentation](#documentation)
-- [MODFLOW Resources](#modflow-resources)
 
 <!-- END doctoc generated TOC please keep comment here to allow auto update -->
 
+## Use cases
+
+This is a small toolkit for developing MODFLOW 6, FloPy, and related projects. It includes standalone utilities and optional [Pytest](https://github.com/pytest-dev/pytest) extensions.
+
+Standalone utilities include a very minimal GitHub API client, mainly for retrieving release information and downloading assets, and a `ZipFile` subclass that [preserves file permissions](https://stackoverflow.com/questions/39296101/python-zipfile-removes-execute-permissions-from-binaries) (workaround for [Python #15795](https://bugs.python.org/issue15795))
+
+Pytest features include:
+
+- `--keep <path>` tempdir fixtures for [each scope](https://docs.pytest.org/en/stable/how-to/fixtures.html#scope-sharing-fixtures-across-classes-modules-packages-or-session)
+- a [`--smoke` test](https://en.wikipedia.org/wiki/Smoke_testing_(software)) (abbrev. `-S`) CLI option shortcut
+- markers to skip test cases conditional on
+  - operating system
+  - Python packages installed
+  - executables available on the PATH
+- test fixtures for example / test models in
+  - `MODFLOW-USGS/modflow6-examples`
+  - `MODFLOW-USGS/modflow6-testmodels`
+  - `MODFLOW-USGS/modflow6-largetestmodels`
+
 ## Requirements
 
-This project requires Python3.8+. Its only core dependencies are `numpy` and `pytest`.
+Python3.8+, dependency-free, but pairs well with `pytest` and select plugins, e.g.
+
+- [`pytest-dotenv`](https://github.com/quiqua/pytest-dotenv)
+- [`pytest-xdist`](https://github.com/pytest-dev/pytest-xdist)
 
 ## Installation
 
 `modflow-devtools` is available on PyPI and can be installed with pip:
 
 ```shell
 pip install modflow-devtools
 ```
 
-This package pairs well with a few pytest plugins:
-
-- `pytest-cases`
-- `pytest-dotenv`
-- `pytest-xdist`
-
-These and a few other optional dependencies can be installed with:
+Pytest, pytest plugins, and other optional dependencies can be installed with:
 
 ```shell
 pip install "modflow-devtools[test]"
 ```
 
 To install from source and set up a development environment please see the [developer documentation](DEVELOPER.md).
 
-## Use cases
-
-This package contains shared tools for developing and testing MODFLOW 6 and FloPy, including standalone utilities as well as `pytest` fixtures, CLI options, and test cases:
-
-- utilities for retrieving release information and downloading assets from the GitHub API
-- a `ZipFile` subclass that [preserves file permissions](https://stackoverflow.com/questions/39296101/python-zipfile-removes-execute-permissions-from-binaries) (workaround for [Python #15795](https://bugs.python.org/issue15795))
-- a `pytest` CLI option for smoke testing (running a fast subset of cases)
-- a minimal `pytest-cases` framework for reusing test functions and data
-- a set of keepable `pytest` temporary directory fixtures for each scope
-- a set of fixtures to parametrize tests with models from external repos
-  - `MODFLOW-USGS/modflow6-examples`
-  - `MODFLOW-USGS/modflow6-testmodels`
-  - `MODFLOW-USGS/modflow6-largetestmodels`
-- a set of `pytest` markers to conditionally skip test cases based on
-  - operating system
-  - Python packages installed
-  - executables available on the path
-
-## Quickstart
-
 To import `pytest` fixtures in a project consuming `modflow-devtools`, add the following to a `conftest.py` file:
 
 ```python
 pytest_plugins = [ "modflow_devtools.fixtures" ]
 ```
 
-**Note**: `pytest` requires this to be a top-level `conftest.py` file. Nested `conftest.py` files may override or extend this package's fixtures.
+**Note**: this must be a top-level `conftest.py`, which nested `conftest.py` files may then override or extend.
 
 ## Documentation
 
-Usage documentation is available at [modflow-devtools.readthedocs.io](https://modflow-devtools.readthedocs.io/en/latest/).
-
-## MODFLOW Resources
+Docs are available at [modflow-devtools.readthedocs.io](https://modflow-devtools.readthedocs.io/en/latest/).
 
-+ [MODFLOW and Related Programs](https://water.usgs.gov/ogw/modflow/)
-+ [Online guide for MODFLOW-2000](https://water.usgs.gov/nrp/gwsoftware/modflow2000/Guide/)
-+ [Online guide for MODFLOW-2005](https://water.usgs.gov/ogw/modflow/MODFLOW-2005-Guide/)
-+ [Online guide for MODFLOW-NWT](https://water.usgs.gov/ogw/modflow-nwt/MODFLOW-NWT-Guide/)
+For more info on MODFLOW 6 see [the USGS overview](https://water.usgs.gov/ogw/modflow/).
```

### Comparing `modflow-devtools-0.2.0/modflow_devtools/build.py` & `modflow-devtools-0.3.0/modflow_devtools/build.py`

 * *Files identical despite different names*

### Comparing `modflow-devtools-0.2.0/modflow_devtools/case.py` & `modflow-devtools-0.3.0/modflow_devtools/case.py`

 * *Files identical despite different names*

### Comparing `modflow-devtools-0.2.0/modflow_devtools/context.py` & `modflow-devtools-0.3.0/modflow_devtools/context.py`

 * *Files identical despite different names*

### Comparing `modflow-devtools-0.2.0/modflow_devtools/download.py` & `modflow-devtools-0.3.0/modflow_devtools/download.py`

 * *Files 1% similar despite different names*

```diff
@@ -434,15 +434,15 @@
 
 def download_and_unzip(
     url: str,
     path: Optional[PathLike] = None,
     delete_zip=True,
     retries=3,
     verbose=False,
-):
+) -> Path:
     """
     Download and unzip a zip file from a URL.
     The filename must be the last element in the URL.
 
     Parameters
     ----------
     url : str
@@ -451,14 +451,19 @@
         Path where the zip file will be saved (default is current path)
     delete_zip : bool
         Whether the zip file should be deleted after it is unzipped (default is True)
     retries : int
         The maximum number of retries for each request
     verbose : bool
         Whether to show verbose output
+
+    Returns
+    -------
+    Path
+        The path to the directory where the zip file was unzipped
     """
 
     path = Path(path if path else os.getcwd())
     path.mkdir(exist_ok=True)
 
     if verbose:
         print(f"Downloading {url}")
@@ -540,7 +545,9 @@
         if delete_zip:
             if verbose:
                 print(f"Deleting zipfile {file_path}")
             file_path.unlink()
 
     if verbose:
         print(f"Done downloading and extracting {file_path.name} to {path}")
+
+    return path
```

### Comparing `modflow-devtools-0.2.0/modflow_devtools/executables.py` & `modflow-devtools-0.3.0/modflow_devtools/executables.py`

 * *Files identical despite different names*

### Comparing `modflow-devtools-0.2.0/modflow_devtools/fixtures.py` & `modflow-devtools-0.3.0/modflow_devtools/fixtures.py`

 * *Files identical despite different names*

### Comparing `modflow-devtools-0.2.0/modflow_devtools/markers.py` & `modflow-devtools-0.3.0/modflow_devtools/markers.py`

 * *Files identical despite different names*

### Comparing `modflow-devtools-0.2.0/modflow_devtools/misc.py` & `modflow-devtools-0.3.0/modflow_devtools/misc.py`

 * *Files identical despite different names*

### Comparing `modflow-devtools-0.2.0/modflow_devtools/test/test_build.py` & `modflow-devtools-0.3.0/modflow_devtools/test/test_build.py`

 * *Files identical despite different names*

### Comparing `modflow-devtools-0.2.0/modflow_devtools/test/test_case.py` & `modflow-devtools-0.3.0/modflow_devtools/test/test_case.py`

 * *Files identical despite different names*

### Comparing `modflow-devtools-0.2.0/modflow_devtools/test/test_download.py` & `modflow-devtools-0.3.0/modflow_devtools/test/test_download.py`

 * *Files identical despite different names*

### Comparing `modflow-devtools-0.2.0/modflow_devtools/test/test_executables.py` & `modflow-devtools-0.3.0/modflow_devtools/test/test_executables.py`

 * *Files identical despite different names*

### Comparing `modflow-devtools-0.2.0/modflow_devtools/test/test_fixtures.py` & `modflow-devtools-0.3.0/modflow_devtools/test/test_fixtures.py`

 * *Files identical despite different names*

### Comparing `modflow-devtools-0.2.0/modflow_devtools/test/test_markers.py` & `modflow-devtools-0.3.0/modflow_devtools/test/test_markers.py`

 * *Files identical despite different names*

### Comparing `modflow-devtools-0.2.0/modflow_devtools/test/test_misc.py` & `modflow-devtools-0.3.0/modflow_devtools/test/test_misc.py`

 * *Files identical despite different names*

### Comparing `modflow-devtools-0.2.0/modflow_devtools/test/test_zip.py` & `modflow-devtools-0.3.0/modflow_devtools/test/test_zip.py`

 * *Files identical despite different names*

### Comparing `modflow-devtools-0.2.0/modflow_devtools/zip.py` & `modflow-devtools-0.3.0/modflow_devtools/zip.py`

 * *Files identical despite different names*

### Comparing `modflow-devtools-0.2.0/modflow_devtools.egg-info/PKG-INFO` & `modflow-devtools-0.3.0/modflow_devtools.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modflow-devtools
-Version: 0.2.0
+Version: 0.3.0
 Summary: Python tools for MODFLOW development
 Author-email: "Joseph D. Hughes" <modflow@usgs.gov>
 Maintainer-email: "Joseph D. Hughes" <modflow@usgs.gov>
 License: CC0
 Project-URL: Documentation, https://modflow-devtools.readthedocs.io/en/latest/
 Project-URL: Bug Tracker, https://github.com/MODFLOW-USGS/modflow-devtools/issues
 Project-URL: Source Code, https://github.com/MODFLOW-USGS/modflow-devtools
@@ -31,85 +31,75 @@
 [![GitHub tag](https://img.shields.io/github/tag/MODFLOW-USGS/modflow-devtools.svg)](https://github.com/MODFLOW-USGS/modflow-devtools/tags/latest)
 [![PyPI Version](https://img.shields.io/pypi/v/modflow-devtools.png)](https://pypi.python.org/pypi/modflow-devtools)
 [![PyPI Versions](https://img.shields.io/pypi/pyversions/modflow-devtools.png)](https://pypi.python.org/pypi/modflow-devtools)
 [![PyPI Status](https://img.shields.io/pypi/status/modflow-devtools.png)](https://pypi.python.org/pypi/modflow-devtools)
 [![CI](https://github.com/MODFLOW-USGS/modflow-devtools/actions/workflows/ci.yml/badge.svg)](https://github.com/MODFLOW-USGS/modflow-devtools/actions/workflows/ci.yml)
 [![Documentation Status](https://readthedocs.org/projects/modflow-devtools/badge/?version=latest)](https://modflow-devtools.readthedocs.io/en/latest/?badge=latest)
 
-Python tools for MODFLOW development and testing.
+Python development tools for MODFLOW 6.
 
 <!-- START doctoc generated TOC please keep comment here to allow auto update -->
 <!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->
 
+
+- [Use cases](#use-cases)
 - [Requirements](#requirements)
 - [Installation](#installation)
-- [Use cases](#use-cases)
-- [Quickstart](#quickstart)
 - [Documentation](#documentation)
-- [MODFLOW Resources](#modflow-resources)
 
 <!-- END doctoc generated TOC please keep comment here to allow auto update -->
 
+## Use cases
+
+This is a small toolkit for developing MODFLOW 6, FloPy, and related projects. It includes standalone utilities and optional [Pytest](https://github.com/pytest-dev/pytest) extensions.
+
+Standalone utilities include a very minimal GitHub API client, mainly for retrieving release information and downloading assets, and a `ZipFile` subclass that [preserves file permissions](https://stackoverflow.com/questions/39296101/python-zipfile-removes-execute-permissions-from-binaries) (workaround for [Python #15795](https://bugs.python.org/issue15795))
+
+Pytest features include:
+
+- `--keep <path>` tempdir fixtures for [each scope](https://docs.pytest.org/en/stable/how-to/fixtures.html#scope-sharing-fixtures-across-classes-modules-packages-or-session)
+- a [`--smoke` test](https://en.wikipedia.org/wiki/Smoke_testing_(software)) (abbrev. `-S`) CLI option shortcut
+- markers to skip test cases conditional on
+  - operating system
+  - Python packages installed
+  - executables available on the PATH
+- test fixtures for example / test models in
+  - `MODFLOW-USGS/modflow6-examples`
+  - `MODFLOW-USGS/modflow6-testmodels`
+  - `MODFLOW-USGS/modflow6-largetestmodels`
+
 ## Requirements
 
-This project requires Python3.8+. Its only core dependencies are `numpy` and `pytest`.
+Python3.8+, dependency-free, but pairs well with `pytest` and select plugins, e.g.
+
+- [`pytest-dotenv`](https://github.com/quiqua/pytest-dotenv)
+- [`pytest-xdist`](https://github.com/pytest-dev/pytest-xdist)
 
 ## Installation
 
 `modflow-devtools` is available on PyPI and can be installed with pip:
 
 ```shell
 pip install modflow-devtools
 ```
 
-This package pairs well with a few pytest plugins:
-
-- `pytest-cases`
-- `pytest-dotenv`
-- `pytest-xdist`
-
-These and a few other optional dependencies can be installed with:
+Pytest, pytest plugins, and other optional dependencies can be installed with:
 
 ```shell
 pip install "modflow-devtools[test]"
 ```
 
 To install from source and set up a development environment please see the [developer documentation](DEVELOPER.md).
 
-## Use cases
-
-This package contains shared tools for developing and testing MODFLOW 6 and FloPy, including standalone utilities as well as `pytest` fixtures, CLI options, and test cases:
-
-- utilities for retrieving release information and downloading assets from the GitHub API
-- a `ZipFile` subclass that [preserves file permissions](https://stackoverflow.com/questions/39296101/python-zipfile-removes-execute-permissions-from-binaries) (workaround for [Python #15795](https://bugs.python.org/issue15795))
-- a `pytest` CLI option for smoke testing (running a fast subset of cases)
-- a minimal `pytest-cases` framework for reusing test functions and data
-- a set of keepable `pytest` temporary directory fixtures for each scope
-- a set of fixtures to parametrize tests with models from external repos
-  - `MODFLOW-USGS/modflow6-examples`
-  - `MODFLOW-USGS/modflow6-testmodels`
-  - `MODFLOW-USGS/modflow6-largetestmodels`
-- a set of `pytest` markers to conditionally skip test cases based on
-  - operating system
-  - Python packages installed
-  - executables available on the path
-
-## Quickstart
-
 To import `pytest` fixtures in a project consuming `modflow-devtools`, add the following to a `conftest.py` file:
 
 ```python
 pytest_plugins = [ "modflow_devtools.fixtures" ]
 ```
 
-**Note**: `pytest` requires this to be a top-level `conftest.py` file. Nested `conftest.py` files may override or extend this package's fixtures.
+**Note**: this must be a top-level `conftest.py`, which nested `conftest.py` files may then override or extend.
 
 ## Documentation
 
-Usage documentation is available at [modflow-devtools.readthedocs.io](https://modflow-devtools.readthedocs.io/en/latest/).
-
-## MODFLOW Resources
+Docs are available at [modflow-devtools.readthedocs.io](https://modflow-devtools.readthedocs.io/en/latest/).
 
-+ [MODFLOW and Related Programs](https://water.usgs.gov/ogw/modflow/)
-+ [Online guide for MODFLOW-2000](https://water.usgs.gov/nrp/gwsoftware/modflow2000/Guide/)
-+ [Online guide for MODFLOW-2005](https://water.usgs.gov/ogw/modflow/MODFLOW-2005-Guide/)
-+ [Online guide for MODFLOW-NWT](https://water.usgs.gov/ogw/modflow-nwt/MODFLOW-NWT-Guide/)
+For more info on MODFLOW 6 see [the USGS overview](https://water.usgs.gov/ogw/modflow/).
```

### Comparing `modflow-devtools-0.2.0/modflow_devtools.egg-info/SOURCES.txt` & `modflow-devtools-0.3.0/modflow_devtools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `modflow-devtools-0.2.0/pyproject.toml` & `modflow-devtools-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -32,18 +32,14 @@
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Scientific/Engineering :: Hydrology"
 ]
 requires-python = ">=3.8"
-dependencies = [
-    "numpy",
-    "pytest"
-]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 lint = [
     "black",
     "cffconvert",
     "flake8",
@@ -53,14 +49,16 @@
 test = [
     "modflow-devtools[lint]",
     "coverage",
     "flaky",
     "filelock",
     "meson!=0.63.0",
     "ninja",
+    "numpy",
+    "pytest",
     "pytest-cases",
     "pytest-cov",
     "pytest-dotenv",
     "pytest-xdist",
     "PyYaml"
 ]
 docs = [
```

