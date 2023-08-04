# Comparing `tmp/gwdetchar-2.1.1.tar.gz` & `tmp/gwdetchar-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gwdetchar-2.1.1.tar", last modified: Mon Jun 19 18:13:48 2023, max compression
+gzip compressed data, was "gwdetchar-2.1.2.tar", last modified: Fri Aug  4 18:21:26 2023, max compression
```

## Comparing `gwdetchar-2.1.1.tar` & `gwdetchar-2.1.2.tar`

### file list

```diff
@@ -1,141 +1,141 @@
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-19 18:13:48.480367 gwdetchar-2.1.1/
--rw-r--r--   0 egoetz     (501) staff       (20)      184 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/.codecov.yml
--rw-r--r--   0 egoetz     (501) staff       (20)      134 2023-06-16 22:43:20.000000 gwdetchar-2.1.1/.flake8
--rw-r--r--   0 egoetz     (501) staff       (20)       35 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/.gitattributes
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-19 18:13:48.401522 gwdetchar-2.1.1/.github/
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-19 18:13:48.416593 gwdetchar-2.1.1/.github/workflows/
--rw-r--r--   0 egoetz     (501) staff       (20)     2885 2023-06-16 22:43:20.000000 gwdetchar-2.1.1/.github/workflows/build.yml
--rw-r--r--   0 egoetz     (501) staff       (20)     1334 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/.github/workflows/docs.yml
--rw-r--r--   0 egoetz     (501) staff       (20)     1084 2023-06-16 22:43:20.000000 gwdetchar-2.1.1/.github/workflows/lint.yml
--rw-r--r--   0 egoetz     (501) staff       (20)      617 2023-06-16 22:43:20.000000 gwdetchar-2.1.1/.gitignore
--rw-r--r--   0 egoetz     (501) staff       (20)      577 2023-06-16 22:43:20.000000 gwdetchar-2.1.1/.readthedocs.yml
--rw-r--r--   0 egoetz     (501) staff       (20)     2638 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/CONTRIBUTING.md
--rw-r--r--   0 egoetz     (501) staff       (20)    35147 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/LICENSE
--rw-r--r--   0 egoetz     (501) staff       (20)       69 2023-06-16 22:43:20.000000 gwdetchar-2.1.1/MANIFEST.in
--rw-r--r--   0 egoetz     (501) staff       (20)     3726 2023-06-19 18:13:48.479852 gwdetchar-2.1.1/PKG-INFO
--rw-r--r--   0 egoetz     (501) staff       (20)     2328 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/README.rst
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-19 18:13:48.417203 gwdetchar-2.1.1/ci/
--rw-r--r--   0 egoetz     (501) staff       (20)     1135 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/ci/test-cli.sh
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-19 18:13:48.419003 gwdetchar-2.1.1/docs/
--rw-r--r--   0 egoetz     (501) staff       (20)     6857 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/docs/Makefile
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-19 18:13:48.402153 gwdetchar-2.1.1/docs/_static/
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-19 18:13:48.419826 gwdetchar-2.1.1/docs/_static/css/
--rw-r--r--   0 egoetz     (501) staff       (20)     4997 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/docs/_static/css/custom.css
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-19 18:13:48.420299 gwdetchar-2.1.1/docs/api/
--rw-r--r--   0 egoetz     (501) staff       (20)       54 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/docs/api/index.rst
--rw-r--r--   0 egoetz     (501) staff       (20)    10994 2023-06-16 22:43:20.000000 gwdetchar-2.1.1/docs/conf.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-19 18:13:48.420707 gwdetchar-2.1.1/docs/conlog/
--rw-r--r--   0 egoetz     (501) staff       (20)      964 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/docs/conlog/index.rst
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-19 18:13:48.421671 gwdetchar-2.1.1/docs/daq/
--rw-r--r--   0 egoetz     (501) staff       (20)     1807 2023-06-16 22:43:20.000000 gwdetchar-2.1.1/docs/daq/index.rst
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-19 18:13:48.422276 gwdetchar-2.1.1/docs/data/
--rw-r--r--   0 egoetz     (501) staff       (20)      863 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/docs/data/index.rst
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-19 18:13:48.422862 gwdetchar-2.1.1/docs/html/
--rw-r--r--   0 egoetz     (501) staff       (20)     1488 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/docs/html/index.rst
--rw-r--r--   0 egoetz     (501) staff       (20)     2968 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/docs/index.rst
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-19 18:13:48.423373 gwdetchar-2.1.1/docs/lasso/
--rw-r--r--   0 egoetz     (501) staff       (20)     1439 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/docs/lasso/index.rst
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-19 18:13:48.424052 gwdetchar-2.1.1/docs/nagios/
--rw-r--r--   0 egoetz     (501) staff       (20)      941 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/docs/nagios/index.rst
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-19 18:13:48.424814 gwdetchar-2.1.1/docs/omega/
--rw-r--r--   0 egoetz     (501) staff       (20)     3035 2023-06-16 22:43:20.000000 gwdetchar-2.1.1/docs/omega/index.rst
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-19 18:13:48.425524 gwdetchar-2.1.1/docs/saturation/
--rw-r--r--   0 egoetz     (501) staff       (20)     1638 2023-06-16 22:43:20.000000 gwdetchar-2.1.1/docs/saturation/index.rst
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-19 18:13:48.426276 gwdetchar-2.1.1/docs/scattering/
--rw-r--r--   0 egoetz     (501) staff       (20)     2926 2023-06-16 22:43:20.000000 gwdetchar-2.1.1/docs/scattering/index.rst
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-19 18:13:48.436457 gwdetchar-2.1.1/gwdetchar/
--rw-r--r--   0 egoetz     (501) staff       (20)     1408 2023-06-16 22:43:20.000000 gwdetchar-2.1.1/gwdetchar/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)      160 2023-06-19 18:13:48.000000 gwdetchar-2.1.1/gwdetchar/_version.py
--rw-r--r--   0 egoetz     (501) staff       (20)     3732 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/gwdetchar/cds.py
--rw-r--r--   0 egoetz     (501) staff       (20)     4738 2023-05-16 23:56:26.000000 gwdetchar-2.1.1/gwdetchar/cli.py
--rw-r--r--   0 egoetz     (501) staff       (20)     2773 2023-04-25 15:49:41.000000 gwdetchar-2.1.1/gwdetchar/condor.py
--rw-r--r--   0 egoetz     (501) staff       (20)     2703 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/gwdetchar/conftest.py
--rw-r--r--   0 egoetz     (501) staff       (20)     7363 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/gwdetchar/conlog.py
--rw-r--r--   0 egoetz     (501) staff       (20)     2997 2023-05-17 00:05:55.000000 gwdetchar-2.1.1/gwdetchar/const.py
--rw-r--r--   0 egoetz     (501) staff       (20)     7440 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/gwdetchar/daq.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-19 18:13:48.440990 gwdetchar-2.1.1/gwdetchar/io/
--rw-r--r--   0 egoetz     (501) staff       (20)      835 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/gwdetchar/io/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)     7584 2023-06-19 18:12:55.000000 gwdetchar-2.1.1/gwdetchar/io/datafind.py
--rw-r--r--   0 egoetz     (501) staff       (20)    41413 2023-06-16 22:43:20.000000 gwdetchar-2.1.1/gwdetchar/io/html.py
--rw-r--r--   0 egoetz     (501) staff       (20)     3764 2023-06-19 18:12:55.000000 gwdetchar-2.1.1/gwdetchar/io/ligolw.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-19 18:13:48.443060 gwdetchar-2.1.1/gwdetchar/io/tests/
--rw-r--r--   0 egoetz     (501) staff       (20)      827 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/gwdetchar/io/tests/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)     4834 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/gwdetchar/io/tests/test_datafind.py
--rw-r--r--   0 egoetz     (501) staff       (20)    24146 2023-06-16 22:43:20.000000 gwdetchar-2.1.1/gwdetchar/io/tests/test_html.py
--rw-r--r--   0 egoetz     (501) staff       (20)     2451 2023-06-19 18:12:55.000000 gwdetchar-2.1.1/gwdetchar/io/tests/test_ligolw.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-19 18:13:48.447783 gwdetchar-2.1.1/gwdetchar/lasso/
--rw-r--r--   0 egoetz     (501) staff       (20)     1063 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/gwdetchar/lasso/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)    35568 2023-06-16 22:43:20.000000 gwdetchar-2.1.1/gwdetchar/lasso/__main__.py
--rw-r--r--   0 egoetz     (501) staff       (20)     6652 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/gwdetchar/lasso/core.py
--rw-r--r--   0 egoetz     (501) staff       (20)    20595 2022-10-03 17:36:21.000000 gwdetchar-2.1.1/gwdetchar/lasso/old.py
--rw-r--r--   0 egoetz     (501) staff       (20)     4946 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/gwdetchar/lasso/plot.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-19 18:13:48.450190 gwdetchar-2.1.1/gwdetchar/lasso/tests/
--rw-r--r--   0 egoetz     (501) staff       (20)      830 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/gwdetchar/lasso/tests/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)     3984 2023-04-27 00:53:55.000000 gwdetchar-2.1.1/gwdetchar/lasso/tests/test_core.py
--rw-r--r--   0 egoetz     (501) staff       (20)     1549 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/gwdetchar/lasso/tests/test_main.py
--rw-r--r--   0 egoetz     (501) staff       (20)     2142 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/gwdetchar/lasso/tests/test_plot.py
--rw-r--r--   0 egoetz     (501) staff       (20)     6744 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/gwdetchar/mct.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-19 18:13:48.451375 gwdetchar-2.1.1/gwdetchar/nagios/
--rw-r--r--   0 egoetz     (501) staff       (20)      887 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/gwdetchar/nagios/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)     2959 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/gwdetchar/nagios/__main__.py
--rw-r--r--   0 egoetz     (501) staff       (20)     2166 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/gwdetchar/nagios/core.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-19 18:13:48.452159 gwdetchar-2.1.1/gwdetchar/nagios/tests/
--rw-r--r--   0 egoetz     (501) staff       (20)      826 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/gwdetchar/nagios/tests/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)     2131 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/gwdetchar/nagios/tests/test_main.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-19 18:13:48.456175 gwdetchar-2.1.1/gwdetchar/omega/
--rw-r--r--   0 egoetz     (501) staff       (20)     1188 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/gwdetchar/omega/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)    13880 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/gwdetchar/omega/__main__.py
--rw-r--r--   0 egoetz     (501) staff       (20)    12682 2023-05-16 23:56:26.000000 gwdetchar-2.1.1/gwdetchar/omega/batch.py
--rw-r--r--   0 egoetz     (501) staff       (20)    15875 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/gwdetchar/omega/config.py
--rw-r--r--   0 egoetz     (501) staff       (20)    10365 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/gwdetchar/omega/core.py
--rw-r--r--   0 egoetz     (501) staff       (20)    20699 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/gwdetchar/omega/html.py
--rw-r--r--   0 egoetz     (501) staff       (20)     8871 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/gwdetchar/omega/plot.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-19 18:13:48.460717 gwdetchar-2.1.1/gwdetchar/omega/tests/
--rw-r--r--   0 egoetz     (501) staff       (20)      830 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/gwdetchar/omega/tests/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)     3689 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/gwdetchar/omega/tests/test_batch.py
--rw-r--r--   0 egoetz     (501) staff       (20)     6970 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/gwdetchar/omega/tests/test_config.py
--rw-r--r--   0 egoetz     (501) staff       (20)     5493 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/gwdetchar/omega/tests/test_core.py
--rw-r--r--   0 egoetz     (501) staff       (20)    13502 2023-06-16 22:43:20.000000 gwdetchar-2.1.1/gwdetchar/omega/tests/test_html.py
--rw-r--r--   0 egoetz     (501) staff       (20)     9824 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/gwdetchar/omega/tests/test_main.py
--rw-r--r--   0 egoetz     (501) staff       (20)     2702 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/gwdetchar/omega/tests/test_plot.py
--rw-r--r--   0 egoetz     (501) staff       (20)    17732 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/gwdetchar/overflow.py
--rw-r--r--   0 egoetz     (501) staff       (20)     2244 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/gwdetchar/plot.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-19 18:13:48.463657 gwdetchar-2.1.1/gwdetchar/saturation/
--rw-r--r--   0 egoetz     (501) staff       (20)     1039 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/gwdetchar/saturation/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)    13870 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/gwdetchar/saturation/__main__.py
--rw-r--r--   0 egoetz     (501) staff       (20)     7654 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/gwdetchar/saturation/core.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-19 18:13:48.465177 gwdetchar-2.1.1/gwdetchar/saturation/tests/
--rw-r--r--   0 egoetz     (501) staff       (20)      835 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/gwdetchar/saturation/tests/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)     3510 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/gwdetchar/saturation/tests/test_saturation.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-19 18:13:48.468893 gwdetchar-2.1.1/gwdetchar/scattering/
--rw-r--r--   0 egoetz     (501) staff       (20)     1983 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/gwdetchar/scattering/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)    32277 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/gwdetchar/scattering/__main__.py
--rw-r--r--   0 egoetz     (501) staff       (20)     6413 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/gwdetchar/scattering/core.py
--rw-r--r--   0 egoetz     (501) staff       (20)     5282 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/gwdetchar/scattering/plot.py
--rw-r--r--   0 egoetz     (501) staff       (20)     8523 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/gwdetchar/scattering/simple.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-19 18:13:48.472746 gwdetchar-2.1.1/gwdetchar/scattering/tests/
--rw-r--r--   0 egoetz     (501) staff       (20)      835 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/gwdetchar/scattering/tests/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)     2238 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/gwdetchar/scattering/tests/test_core.py
--rw-r--r--   0 egoetz     (501) staff       (20)     5520 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/gwdetchar/scattering/tests/test_main.py
--rw-r--r--   0 egoetz     (501) staff       (20)     1831 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/gwdetchar/scattering/tests/test_plot.py
--rw-r--r--   0 egoetz     (501) staff       (20)     3156 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/gwdetchar/scattering/tests/test_simple.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-19 18:13:48.478957 gwdetchar-2.1.1/gwdetchar/tests/
--rw-r--r--   0 egoetz     (501) staff       (20)      826 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/gwdetchar/tests/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)     3276 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/gwdetchar/tests/test_cds.py
--rw-r--r--   0 egoetz     (501) staff       (20)     3181 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/gwdetchar/tests/test_cli.py
--rw-r--r--   0 egoetz     (501) staff       (20)     1918 2023-04-25 15:49:41.000000 gwdetchar-2.1.1/gwdetchar/tests/test_condor.py
--rw-r--r--   0 egoetz     (501) staff       (20)     4819 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/gwdetchar/tests/test_conlog.py
--rw-r--r--   0 egoetz     (501) staff       (20)     1928 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/gwdetchar/tests/test_const.py
--rw-r--r--   0 egoetz     (501) staff       (20)     3306 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/gwdetchar/tests/test_daq.py
--rw-r--r--   0 egoetz     (501) staff       (20)     2077 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/gwdetchar/tests/test_plot.py
--rw-r--r--   0 egoetz     (501) staff       (20)     2831 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/gwdetchar/tests/test_utils.py
--rw-r--r--   0 egoetz     (501) staff       (20)     4531 2022-08-23 18:11:03.000000 gwdetchar-2.1.1/gwdetchar/utils.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-19 18:13:48.439235 gwdetchar-2.1.1/gwdetchar.egg-info/
--rw-r--r--   0 egoetz     (501) staff       (20)     3726 2023-06-19 18:13:48.000000 gwdetchar-2.1.1/gwdetchar.egg-info/PKG-INFO
--rw-r--r--   0 egoetz     (501) staff       (20)     2832 2023-06-19 18:13:48.000000 gwdetchar-2.1.1/gwdetchar.egg-info/SOURCES.txt
--rw-r--r--   0 egoetz     (501) staff       (20)        1 2023-06-19 18:13:48.000000 gwdetchar-2.1.1/gwdetchar.egg-info/dependency_links.txt
--rw-r--r--   0 egoetz     (501) staff       (20)      591 2023-06-19 18:13:48.000000 gwdetchar-2.1.1/gwdetchar.egg-info/entry_points.txt
--rw-r--r--   0 egoetz     (501) staff       (20)      348 2023-06-19 18:13:48.000000 gwdetchar-2.1.1/gwdetchar.egg-info/requires.txt
--rw-r--r--   0 egoetz     (501) staff       (20)       10 2023-06-19 18:13:48.000000 gwdetchar-2.1.1/gwdetchar.egg-info/top_level.txt
--rw-r--r--   0 egoetz     (501) staff       (20)     3457 2023-06-19 18:12:55.000000 gwdetchar-2.1.1/pyproject.toml
--rw-r--r--   0 egoetz     (501) staff       (20)       38 2023-06-19 18:13:48.480508 gwdetchar-2.1.1/setup.cfg
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-04 18:21:26.024246 gwdetchar-2.1.2/
+-rw-r--r--   0 egoetz     (501) staff       (20)      184 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/.codecov.yml
+-rw-r--r--   0 egoetz     (501) staff       (20)      134 2023-06-16 22:43:20.000000 gwdetchar-2.1.2/.flake8
+-rw-r--r--   0 egoetz     (501) staff       (20)       35 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/.gitattributes
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-04 18:21:25.946317 gwdetchar-2.1.2/.github/
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-04 18:21:25.961251 gwdetchar-2.1.2/.github/workflows/
+-rw-r--r--   0 egoetz     (501) staff       (20)     2885 2023-06-16 22:43:20.000000 gwdetchar-2.1.2/.github/workflows/build.yml
+-rw-r--r--   0 egoetz     (501) staff       (20)     1334 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/.github/workflows/docs.yml
+-rw-r--r--   0 egoetz     (501) staff       (20)     1377 2023-06-28 17:53:22.000000 gwdetchar-2.1.2/.github/workflows/lint.yml
+-rw-r--r--   0 egoetz     (501) staff       (20)      617 2023-06-16 22:43:20.000000 gwdetchar-2.1.2/.gitignore
+-rw-r--r--   0 egoetz     (501) staff       (20)      525 2023-06-28 17:53:22.000000 gwdetchar-2.1.2/.readthedocs.yml
+-rw-r--r--   0 egoetz     (501) staff       (20)     2638 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/CONTRIBUTING.md
+-rw-r--r--   0 egoetz     (501) staff       (20)    35147 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/LICENSE
+-rw-r--r--   0 egoetz     (501) staff       (20)       69 2023-06-16 22:43:20.000000 gwdetchar-2.1.2/MANIFEST.in
+-rw-r--r--   0 egoetz     (501) staff       (20)     3726 2023-08-04 18:21:26.023736 gwdetchar-2.1.2/PKG-INFO
+-rw-r--r--   0 egoetz     (501) staff       (20)     2328 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/README.rst
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-04 18:21:25.961965 gwdetchar-2.1.2/ci/
+-rw-r--r--   0 egoetz     (501) staff       (20)     1135 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/ci/test-cli.sh
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-04 18:21:25.964130 gwdetchar-2.1.2/docs/
+-rw-r--r--   0 egoetz     (501) staff       (20)     6857 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/docs/Makefile
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-04 18:21:25.946886 gwdetchar-2.1.2/docs/_static/
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-04 18:21:25.964870 gwdetchar-2.1.2/docs/_static/css/
+-rw-r--r--   0 egoetz     (501) staff       (20)     4997 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/docs/_static/css/custom.css
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-04 18:21:25.965452 gwdetchar-2.1.2/docs/api/
+-rw-r--r--   0 egoetz     (501) staff       (20)       54 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/docs/api/index.rst
+-rw-r--r--   0 egoetz     (501) staff       (20)    10994 2023-06-16 22:43:20.000000 gwdetchar-2.1.2/docs/conf.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-04 18:21:25.966035 gwdetchar-2.1.2/docs/conlog/
+-rw-r--r--   0 egoetz     (501) staff       (20)      964 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/docs/conlog/index.rst
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-04 18:21:25.966874 gwdetchar-2.1.2/docs/daq/
+-rw-r--r--   0 egoetz     (501) staff       (20)     1807 2023-06-16 22:43:20.000000 gwdetchar-2.1.2/docs/daq/index.rst
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-04 18:21:25.967657 gwdetchar-2.1.2/docs/data/
+-rw-r--r--   0 egoetz     (501) staff       (20)      863 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/docs/data/index.rst
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-04 18:21:25.968366 gwdetchar-2.1.2/docs/html/
+-rw-r--r--   0 egoetz     (501) staff       (20)     1488 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/docs/html/index.rst
+-rw-r--r--   0 egoetz     (501) staff       (20)     2968 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/docs/index.rst
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-04 18:21:25.969025 gwdetchar-2.1.2/docs/lasso/
+-rw-r--r--   0 egoetz     (501) staff       (20)     1439 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/docs/lasso/index.rst
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-04 18:21:25.969601 gwdetchar-2.1.2/docs/nagios/
+-rw-r--r--   0 egoetz     (501) staff       (20)      941 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/docs/nagios/index.rst
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-04 18:21:25.970204 gwdetchar-2.1.2/docs/omega/
+-rw-r--r--   0 egoetz     (501) staff       (20)     3035 2023-06-16 22:43:20.000000 gwdetchar-2.1.2/docs/omega/index.rst
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-04 18:21:25.970992 gwdetchar-2.1.2/docs/saturation/
+-rw-r--r--   0 egoetz     (501) staff       (20)     1638 2023-06-16 22:43:20.000000 gwdetchar-2.1.2/docs/saturation/index.rst
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-04 18:21:25.971668 gwdetchar-2.1.2/docs/scattering/
+-rw-r--r--   0 egoetz     (501) staff       (20)     2926 2023-06-16 22:43:20.000000 gwdetchar-2.1.2/docs/scattering/index.rst
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-04 18:21:25.980805 gwdetchar-2.1.2/gwdetchar/
+-rw-r--r--   0 egoetz     (501) staff       (20)     1408 2023-06-16 22:43:20.000000 gwdetchar-2.1.2/gwdetchar/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)      160 2023-08-04 18:21:25.000000 gwdetchar-2.1.2/gwdetchar/_version.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     3732 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/gwdetchar/cds.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     4738 2023-05-16 23:56:26.000000 gwdetchar-2.1.2/gwdetchar/cli.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     2773 2023-04-25 15:49:41.000000 gwdetchar-2.1.2/gwdetchar/condor.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     2703 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/gwdetchar/conftest.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     7363 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/gwdetchar/conlog.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     2997 2023-05-17 00:05:55.000000 gwdetchar-2.1.2/gwdetchar/const.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     7440 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/gwdetchar/daq.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-04 18:21:25.986868 gwdetchar-2.1.2/gwdetchar/io/
+-rw-r--r--   0 egoetz     (501) staff       (20)      835 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/gwdetchar/io/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     7584 2023-06-19 18:12:55.000000 gwdetchar-2.1.2/gwdetchar/io/datafind.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    41413 2023-06-16 22:43:20.000000 gwdetchar-2.1.2/gwdetchar/io/html.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     3764 2023-06-19 18:12:55.000000 gwdetchar-2.1.2/gwdetchar/io/ligolw.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-04 18:21:25.990483 gwdetchar-2.1.2/gwdetchar/io/tests/
+-rw-r--r--   0 egoetz     (501) staff       (20)      827 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/gwdetchar/io/tests/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     4834 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/gwdetchar/io/tests/test_datafind.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    24146 2023-06-16 22:43:20.000000 gwdetchar-2.1.2/gwdetchar/io/tests/test_html.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     2451 2023-06-19 18:12:55.000000 gwdetchar-2.1.2/gwdetchar/io/tests/test_ligolw.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-04 18:21:25.994512 gwdetchar-2.1.2/gwdetchar/lasso/
+-rw-r--r--   0 egoetz     (501) staff       (20)     1063 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/gwdetchar/lasso/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    50279 2023-08-04 18:20:44.000000 gwdetchar-2.1.2/gwdetchar/lasso/__main__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     6652 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/gwdetchar/lasso/core.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    20595 2022-10-03 17:36:21.000000 gwdetchar-2.1.2/gwdetchar/lasso/old.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     4946 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/gwdetchar/lasso/plot.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-04 18:21:25.997247 gwdetchar-2.1.2/gwdetchar/lasso/tests/
+-rw-r--r--   0 egoetz     (501) staff       (20)      830 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/gwdetchar/lasso/tests/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     3984 2023-04-27 00:53:55.000000 gwdetchar-2.1.2/gwdetchar/lasso/tests/test_core.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     1549 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/gwdetchar/lasso/tests/test_main.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     2142 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/gwdetchar/lasso/tests/test_plot.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     6744 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/gwdetchar/mct.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-04 18:21:25.998922 gwdetchar-2.1.2/gwdetchar/nagios/
+-rw-r--r--   0 egoetz     (501) staff       (20)      887 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/gwdetchar/nagios/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     2959 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/gwdetchar/nagios/__main__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     2166 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/gwdetchar/nagios/core.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-04 18:21:25.999883 gwdetchar-2.1.2/gwdetchar/nagios/tests/
+-rw-r--r--   0 egoetz     (501) staff       (20)      826 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/gwdetchar/nagios/tests/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     2131 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/gwdetchar/nagios/tests/test_main.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-04 18:21:26.004146 gwdetchar-2.1.2/gwdetchar/omega/
+-rw-r--r--   0 egoetz     (501) staff       (20)     1188 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/gwdetchar/omega/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    14012 2023-08-04 18:20:44.000000 gwdetchar-2.1.2/gwdetchar/omega/__main__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    12682 2023-05-16 23:56:26.000000 gwdetchar-2.1.2/gwdetchar/omega/batch.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    15875 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/gwdetchar/omega/config.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    10365 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/gwdetchar/omega/core.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    20699 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/gwdetchar/omega/html.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     8871 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/gwdetchar/omega/plot.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-04 18:21:26.008335 gwdetchar-2.1.2/gwdetchar/omega/tests/
+-rw-r--r--   0 egoetz     (501) staff       (20)      830 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/gwdetchar/omega/tests/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     3689 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/gwdetchar/omega/tests/test_batch.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     6970 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/gwdetchar/omega/tests/test_config.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     5493 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/gwdetchar/omega/tests/test_core.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    13502 2023-06-16 22:43:20.000000 gwdetchar-2.1.2/gwdetchar/omega/tests/test_html.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     9824 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/gwdetchar/omega/tests/test_main.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     2702 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/gwdetchar/omega/tests/test_plot.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    17732 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/gwdetchar/overflow.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     2244 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/gwdetchar/plot.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-04 18:21:26.010323 gwdetchar-2.1.2/gwdetchar/saturation/
+-rw-r--r--   0 egoetz     (501) staff       (20)     1039 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/gwdetchar/saturation/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    13870 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/gwdetchar/saturation/__main__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     7654 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/gwdetchar/saturation/core.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-04 18:21:26.011479 gwdetchar-2.1.2/gwdetchar/saturation/tests/
+-rw-r--r--   0 egoetz     (501) staff       (20)      835 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/gwdetchar/saturation/tests/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     3510 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/gwdetchar/saturation/tests/test_saturation.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-04 18:21:26.014534 gwdetchar-2.1.2/gwdetchar/scattering/
+-rw-r--r--   0 egoetz     (501) staff       (20)     1983 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/gwdetchar/scattering/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    32277 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/gwdetchar/scattering/__main__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     6413 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/gwdetchar/scattering/core.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     5282 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/gwdetchar/scattering/plot.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     8523 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/gwdetchar/scattering/simple.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-04 18:21:26.017710 gwdetchar-2.1.2/gwdetchar/scattering/tests/
+-rw-r--r--   0 egoetz     (501) staff       (20)      835 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/gwdetchar/scattering/tests/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     2238 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/gwdetchar/scattering/tests/test_core.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     5520 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/gwdetchar/scattering/tests/test_main.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     1831 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/gwdetchar/scattering/tests/test_plot.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     3156 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/gwdetchar/scattering/tests/test_simple.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-04 18:21:26.022945 gwdetchar-2.1.2/gwdetchar/tests/
+-rw-r--r--   0 egoetz     (501) staff       (20)      826 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/gwdetchar/tests/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     3276 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/gwdetchar/tests/test_cds.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     3181 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/gwdetchar/tests/test_cli.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     1918 2023-04-25 15:49:41.000000 gwdetchar-2.1.2/gwdetchar/tests/test_condor.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     4819 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/gwdetchar/tests/test_conlog.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     1928 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/gwdetchar/tests/test_const.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     3306 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/gwdetchar/tests/test_daq.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     2077 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/gwdetchar/tests/test_plot.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     2831 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/gwdetchar/tests/test_utils.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     4531 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/gwdetchar/utils.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-04 18:21:25.984146 gwdetchar-2.1.2/gwdetchar.egg-info/
+-rw-r--r--   0 egoetz     (501) staff       (20)     3726 2023-08-04 18:21:25.000000 gwdetchar-2.1.2/gwdetchar.egg-info/PKG-INFO
+-rw-r--r--   0 egoetz     (501) staff       (20)     2832 2023-08-04 18:21:25.000000 gwdetchar-2.1.2/gwdetchar.egg-info/SOURCES.txt
+-rw-r--r--   0 egoetz     (501) staff       (20)        1 2023-08-04 18:21:25.000000 gwdetchar-2.1.2/gwdetchar.egg-info/dependency_links.txt
+-rw-r--r--   0 egoetz     (501) staff       (20)      591 2023-08-04 18:21:25.000000 gwdetchar-2.1.2/gwdetchar.egg-info/entry_points.txt
+-rw-r--r--   0 egoetz     (501) staff       (20)      348 2023-08-04 18:21:25.000000 gwdetchar-2.1.2/gwdetchar.egg-info/requires.txt
+-rw-r--r--   0 egoetz     (501) staff       (20)       10 2023-08-04 18:21:25.000000 gwdetchar-2.1.2/gwdetchar.egg-info/top_level.txt
+-rw-r--r--   0 egoetz     (501) staff       (20)     3457 2023-06-19 18:12:55.000000 gwdetchar-2.1.2/pyproject.toml
+-rw-r--r--   0 egoetz     (501) staff       (20)       38 2023-08-04 18:21:26.024377 gwdetchar-2.1.2/setup.cfg
```

### Comparing `gwdetchar-2.1.1/.github/workflows/build.yml` & `gwdetchar-2.1.2/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.1/.github/workflows/docs.yml` & `gwdetchar-2.1.2/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.1/.github/workflows/lint.yml` & `gwdetchar-2.1.2/.github/workflows/lint.yml`

 * *Files 26% similar despite different names*

```diff
@@ -12,14 +12,18 @@
       - main
       - master
   pull_request:
     branches:
       - main
       - master
 
+concurrency:
+  group: ${{ github.workflow }}-${{ github.ref }}
+  cancel-in-progress: true
+
 jobs:
   flake8:
     name: Flake8
     runs-on: ubuntu-latest
     steps:
     - uses: actions/checkout@v2
     - name: Set up Python
@@ -42,11 +46,19 @@
       uses: actions/setup-python@v2
       with:
         python-version: '3.x'
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         python -m pip install \
-            "rstcheck[sphinx,toml]>=6.0.0" \
+            "rstcheck[sphinx]>=6.0.0" \
         ;
+    - name: List packages
+      run: python -m pip list installed
     - name: Lint with rstcheck
-      run: rstcheck . --recursive
+      run: |
+        rstcheck . \
+            --config pyproject.toml \
+            --log-level DEBUG \
+            --recursive \
+            --report-level error \
+        ;
```

### Comparing `gwdetchar-2.1.1/.gitignore` & `gwdetchar-2.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.1/CONTRIBUTING.md` & `gwdetchar-2.1.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.1/LICENSE` & `gwdetchar-2.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.1/PKG-INFO` & `gwdetchar-2.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gwdetchar
-Version: 2.1.1
+Version: 2.1.2
 Summary: A python package for gravitational-wave detector characterisation
 Author-email: Alex Urban <alex.urban@ligo.org>, Duncan Macleod <duncan.macleod@ligo.org>
 Maintainer-email: Evan Goetz <evan.goetz@ligo.org>
 License: GPL-3.0-or-later
 Project-URL: Documentation, https://gwdetchar.readthedocs.io
 Project-URL: Source Code, https://github.com/gwdetchar/gwdetchar
 Project-URL: Bug Tracker, https://github.com/gwdetchar/gwdetchar/issues
```

### Comparing `gwdetchar-2.1.1/README.rst` & `gwdetchar-2.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.1/ci/test-cli.sh` & `gwdetchar-2.1.2/ci/test-cli.sh`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.1/docs/Makefile` & `gwdetchar-2.1.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.1/docs/_static/css/custom.css` & `gwdetchar-2.1.2/docs/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.1/docs/conf.py` & `gwdetchar-2.1.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.1/docs/conlog/index.rst` & `gwdetchar-2.1.2/docs/conlog/index.rst`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.1/docs/daq/index.rst` & `gwdetchar-2.1.2/docs/daq/index.rst`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.1/docs/data/index.rst` & `gwdetchar-2.1.2/docs/data/index.rst`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.1/docs/html/index.rst` & `gwdetchar-2.1.2/docs/html/index.rst`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.1/docs/index.rst` & `gwdetchar-2.1.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.1/docs/lasso/index.rst` & `gwdetchar-2.1.2/docs/lasso/index.rst`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.1/docs/nagios/index.rst` & `gwdetchar-2.1.2/docs/nagios/index.rst`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.1/docs/omega/index.rst` & `gwdetchar-2.1.2/docs/omega/index.rst`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.1/docs/saturation/index.rst` & `gwdetchar-2.1.2/docs/saturation/index.rst`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.1/docs/scattering/index.rst` & `gwdetchar-2.1.2/docs/scattering/index.rst`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.1/gwdetchar/__init__.py` & `gwdetchar-2.1.2/gwdetchar/__init__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.1/gwdetchar/cds.py` & `gwdetchar-2.1.2/gwdetchar/cds.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.1/gwdetchar/cli.py` & `gwdetchar-2.1.2/gwdetchar/cli.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.1/gwdetchar/condor.py` & `gwdetchar-2.1.2/gwdetchar/condor.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.1/gwdetchar/conftest.py` & `gwdetchar-2.1.2/gwdetchar/conftest.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.1/gwdetchar/conlog.py` & `gwdetchar-2.1.2/gwdetchar/conlog.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.1/gwdetchar/const.py` & `gwdetchar-2.1.2/gwdetchar/const.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.1/gwdetchar/daq.py` & `gwdetchar-2.1.2/gwdetchar/daq.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.1/gwdetchar/io/__init__.py` & `gwdetchar-2.1.2/gwdetchar/io/__init__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.1/gwdetchar/io/datafind.py` & `gwdetchar-2.1.2/gwdetchar/io/datafind.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.1/gwdetchar/io/html.py` & `gwdetchar-2.1.2/gwdetchar/io/html.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.1/gwdetchar/io/ligolw.py` & `gwdetchar-2.1.2/gwdetchar/io/ligolw.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.1/gwdetchar/io/tests/__init__.py` & `gwdetchar-2.1.2/gwdetchar/io/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.1/gwdetchar/io/tests/test_datafind.py` & `gwdetchar-2.1.2/gwdetchar/io/tests/test_datafind.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.1/gwdetchar/io/tests/test_html.py` & `gwdetchar-2.1.2/gwdetchar/io/tests/test_html.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.1/gwdetchar/io/tests/test_ligolw.py` & `gwdetchar-2.1.2/gwdetchar/io/tests/test_ligolw.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.1/gwdetchar/lasso/__init__.py` & `gwdetchar-2.1.2/gwdetchar/lasso/__init__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.1/gwdetchar/lasso/__main__.py` & `gwdetchar-2.1.2/gwdetchar/lasso/__main__.py`

 * *Files 20% similar despite different names*

```diff
@@ -12,33 +12,39 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with GW DetChar.  If not, see <http://www.gnu.org/licenses/>.
 
+import fnmatch
 import multiprocessing
 import os
 import re
 import sys
-
-from gwpy.timeseries import TimeSeries
+from getpass import getuser
 
 import numpy
 
 from MarkupPy import markup
 
 from astropy.table import Table
 
 from sklearn import linear_model
 from sklearn.preprocessing import StandardScaler, scale
 
 from pandas import set_option
-from gwpy.detector import ChannelList
-from gwpy.io import nds2 as io_nds2
+from gwpy.io.datafind import find_urls
+from gwpy.io.gwf import get_channel_names
+from gwpy.segments import (
+    SegmentList,
+    DataQualityFlag,
+)
+from gwpy.time import tconvert
+from gwpy.timeseries import TimeSeries
 
 from .. import (cli, lasso as gwlasso)
 from ..io.datafind import get_data
 from ..io import html as htmlio
 
 from matplotlib import (use, rcParams)
 use('Agg')
@@ -134,18 +140,19 @@
                         texify(cluster[i][3]), cluster[i][2])),
                 )
 
             ax.margins(x=0)
             ax.set_ylabel('Scaled amplitude [arbitrary units]')
             ax.set_title('Highly Correlated Channels')
             ax.legend(loc='center left', bbox_to_anchor=(1.05, 0.5))
-            plot7 = gwplot.save_figure(fig, '%s_CLUSTER-%s.png' % (
-                re_delim.sub('_', str(currentchan))
-                        .replace('_', '-', 1),
-                gpsstub), bbox_inches='tight')
+            plot7 = gwplot.save_figure(
+                fig,
+                os.path.join('%s_CLUSTER-%s.png' % (
+                    re_delim.sub('_', str(currentchan)).replace('_', '-', 1),
+                    gpsstub)), bbox_inches='tight')
 
     with counter.get_lock():
         counter.value += 1
         pc = 100 * counter.value / len(nonzerodata)
         LOGGER.info("Completed [%d/%d] %3d%% %-50s"
                     % (counter.value, len(nonzerodata), pc,
                        '(%s)' % str(currentchan)))
@@ -201,15 +208,16 @@
         else:
             ax1.set_ylabel('Primary channel units')
         ax2.set_ylabel('Channel units')
         for ax in fig.axes:
             ax.legend(loc='best')
         channelstub = re_delim.sub('_', str(chan)).replace('_', '-', 1)
         plot4 = gwplot.save_figure(
-            fig, '%s_TRENDS-%s.png' % (channelstub, gpsstub),
+            fig,
+            f'{channelstub}_TRENDS-{gpsstub}.png',
             bbox_inches='tight')
 
         # create scaled, sign-corrected, and overlayed timeseries
         tsscaled = scale(ts.value)
         if lassocoef < 0:
             tsscaled = numpy.negative(tsscaled)
         fig = Plot(figsize=(12, 4))
@@ -224,15 +232,16 @@
                 linewidth=line_size_aux)
         if range_is_primary:
             ax.set_ylabel('Sensitive range [Mpc]')
         else:
             ax.set_ylabel('Primary Channel Units')
         ax.legend(loc='best')
         plot5 = gwplot.save_figure(
-            fig, '%s_COMPARISON-%s.png' % (channelstub, gpsstub),
+            fig,
+            f'{channelstub}_COMPARISON-{gpsstub}.png',
             bbox_inches='tight')
 
         # scatter plot
         tsCopy = ts.value.reshape(-1, 1)
         primarytsCopy = primaryts.value.reshape(-1, 1)
         primaryReg = linear_model.LinearRegression()
         primaryReg.fit(tsCopy, primarytsCopy)
@@ -254,15 +263,16 @@
                 transform=ax.transAxes, color='black', size=20,
                 bbox=dict(boxstyle='square', facecolor='white', alpha=.75,
                           edgecolor='black'))
         ax.scatter(ts.value, primaryts.value, color='red')
         ax.plot(ts.value, primaryFit, color='black')
         ax.autoscale_view(tight=False, scalex=True, scaley=True)
         plot6 = gwplot.save_figure(
-            fig, '%s_SCATTER-%s.png' % (channelstub, gpsstub),
+            fig,
+            f'{channelstub}_SCATTER-{gpsstub}.png',
             bbox_inches='tight')
 
     # increment counter and print status
     with counter.get_lock():
         counter.value += 1
         pc = 100 * counter.value / len(nonzerodata)
         LOGGER.info("Completed [%d/%d] %3d%% %-50s"
@@ -297,14 +307,15 @@
     parser = cli.create_parser(
         prog=PROG,
         description=__doc__,
         formatter_class=cli.argparse.ArgumentDefaultsHelpFormatter,
     )
     psig = parser.add_argument_group('Signal processing options')
     lsig = parser.add_argument_group('Lasso options')
+    segm = parser.add_argument_group('Segment processing options')
 
     # required arguments
     cli.add_gps_start_stop_arguments(parser)
     cli.add_ifo_option(parser)
 
     # optional arguments
     cli.add_nproc_option(parser, default=1)
@@ -320,14 +331,21 @@
         '-o',
         '--output-dir',
         default=os.curdir,
         type=os.path.abspath,
         help='output directory for plots',
     )
     parser.add_argument(
+        '-s',
+        '--summary-dir',
+        default=os.curdir,
+        type=os.path.abspath,
+        help='output directory for html summary pages'
+    )
+    parser.add_argument(
         '-f',
         '--channel-file',
         type=os.path.abspath,
         help='path for channel file',
     )
     parser.add_argument(
         '-T',
@@ -377,14 +395,20 @@
     parser.add_argument(
         '-t',
         '--threshold',
         type=float,
         default=0.0001,
         help='threshold for making a plot',
     )
+    parser.add_argument(
+        '--remove-bad-chans',
+        action='store_true',
+        default=False,
+        help='remove flat/bad channels',
+    )
 
     # signal processing arguments
     psig.add_argument(
         '-b',
         '--band-pass',
         type=float,
         nargs=2,
@@ -433,14 +457,35 @@
         '-l',
         '--line-size-aux',
         default=0.75,
         type=float,
         help='line width of auxilary channel',
     )
 
+    # segment options
+    segm.add_argument(
+        '--low-noise-state-flag',
+        action='store_true',
+        default=False,
+        help='use low noise data quality flag for segments'
+    )
+    segm.add_argument(
+        '--segment-padding',
+        type=int,
+        default=1200,
+        help=('padding of time on either side of a data-quality segment to '
+              'remove')
+    )
+    segm.add_argument(
+        '--segment-min-length',
+        default=10800,
+        type=int,
+        help='data-quality segments must be at least this many seconds'
+    )
+
     # return the argument parser
     return parser
 
 
 # -- main code block ----------------------------------------------------------
 
 def main(args=None):
@@ -460,512 +505,809 @@
     if args.remove_outliers_pf:
         if args.remove_outliers_pf >= 1 or args.remove_outliers_pf <= 0:
             raise ValueError('Percent outlier limit must be between 0 and 1')
 
     # get run params
     start = int(args.gpsstart)
     end = int(args.gpsend)
-    pad = args.filter_padding
 
     # set pertinent global variables
     cluster_threshold = args.cluster_coefficient
     line_size_aux = args.line_size_aux
     line_size_primary = args.line_size_primary
     threshold = args.threshold
     trend_type = args.trend_type
 
     # let's go
-    LOGGER.info('{} Lasso correlations {}-{}'.format(args.ifo, start, end))
+    LOGGER.info(f'{args.ifo} Lasso correlations {start}-{end}')
 
     # get primary channel frametype
     primary = args.primary_channel.format(ifo=args.ifo)
     range_is_primary = 'EFFECTIVE_RANGE_MPC' in args.primary_channel
     if args.primary_cache is not None:
         LOGGER.info("Using custom primary cache file")
     elif args.primary_frametype is None and args.primary_file is None:
         try:
             args.primary_frametype = DEFAULT_FRAMETYPE[
                 primary.split(':')[1]].format(ifo=args.ifo)
         except KeyError as exc:
             raise type(exc)("Could not determine primary channel's frametype, "
                             "please specify with --primary-frametype")
 
+    # Get auxiliary frametype
+    if args.trend_type == 'minute':
+        aux_frametype = f'{args.ifo}_M'  # for minute trends
+    else:
+        aux_frametype = f'{args.ifo}_T'  # for second trends
+
+    # Remove channels regexp
+    to_remove = ['.*\.n$', '.*.min$', '.*.max$', '.*.rms$']  # noqa: W605
+    if range_is_primary:
+        to_remove.extend([
+            'OAF-RANGE', 'SENSEMON', 'SENSMON',
+            'CAL-CS_DARM', ':SUS-.*TM.*MODE[0-9]',
+            'SQZ-DCPD_', 'CAL-CS_TDEP_*', 'PCAL*COHERENCE',
+            'ASC-ADS*'])
+    remove_regex = re.compile("({})".format("|".join(to_remove)))
+
     # create output directory
-    if not os.path.isdir(args.output_dir):
-        os.makedirs(args.output_dir)
-    os.chdir(args.output_dir)
+    os.makedirs(args.output_dir, exist_ok=True)
 
     # multiprocessing for plots
     nprocplot = (args.nproc_plot or args.nproc) if USETEX else 1
 
-    # bandpass primary
-    if args.band_pass:
-        try:
-            flower, fupper = args.band_pass
-        except TypeError:
-            flower, fupper = None
-
-        LOGGER.info("-- Loading primary channel data")
-        bandts = get_primary_ts(filepath=args.primary_file, channel=primary,
-                                start=start-pad, end=end+pad,
-                                frametype=args.primary_frametype,
-                                cache=args.primary_cache, nproc=args.nproc)
-        if flower < 0 or fupper >= float((bandts.sample_rate/2.).value):
-            raise ValueError(
-                "bandpass frequency is out of range for this "
-                "channel, band (Hz): {0}, sample rate: {1}".format(
-                    args.band_pass, bandts.sample_rate))
-
-        # get darm BLRMS
-        LOGGER.debug("-- Filtering data")
-        if trend_type == 'minute':
-            stride = 60
-        else:
-            stride = 1
-        if flower:
-            darmbl = (
-                bandts.highpass(flower/2., fstop=flower/4.,
-                                filtfilt=False, ftype='butter')
-                .notch(60, filtfilt=False)
-                .bandpass(flower, fupper, fstop=[flower/2., fupper*1.5],
-                          filtfilt=False, ftype='butter')
-                .crop(start, end))
-            darmblrms = darmbl.rms(stride)
-            darmblrms.name = '%s %s-%s Hz BLRMS' % (primary, flower, fupper)
-        else:
-            darmbl = bandts.notch(60).crop(start, end)
-            darmblrms = darmbl.rms(stride)
-            darmblrms.name = '%s RMS' % primary
-
-        primaryts = darmblrms
-
-        bandts_asd = bandts.asd(4, 2, method='median')
-        darmbl_asd = darmbl.asd(4, 2, method='median')
-
-        spectrum_plots = gwplot.make_spectrum_plots(
-            start, end, flower, fupper, primary,
-            bandts_asd, darmbl_asd)
-        spectrum_plot_zoomed_out = spectrum_plots[0]
-        spectrum_plot_zoomed_in = spectrum_plots[1]
-
+    # Get segments
+    if args.low_noise_state_flag:
+        state_flag = f'{args.ifo}:DMT-GRD_ISC_LOCK_NOMINAL:1'
+        state_is_observing = False
+        state_name = 'Locked'
     else:
-        # load primary channel data
-        LOGGER.info("-- Loading primary channel data")
-        primaryts = get_primary_ts(filepath=args.primary_file, channel=primary,
-                                   start=start, end=end,
-                                   frametype=args.primary_frametype,
-                                   cache=args.primary_cache,
-                                   nproc=args.nproc).crop(start, end)
-
-    if args.remove_outliers:
-        LOGGER.debug(
-            "-- Removing outliers above %f sigma" % args.remove_outliers)
-        gwlasso.remove_outliers(primaryts, args.remove_outliers)
-    elif args.remove_outliers_pf:
-        LOGGER.debug("-- Removing outliers in the bottom {} percent "
-                     "of data".format(args.remove_outliers_pf*100))
-        gwlasso.remove_outliers(
-            primaryts, args.remove_outliers_pf, method='pf')
-        start = int(primaryts.span[0])
-        end = int(primaryts.span[1])
-
-    primary_mean = numpy.mean(primaryts.value)
-    primary_std = numpy.std(primaryts.value)
-
-    # get aux data
-    LOGGER.info("-- Loading auxiliary channel data")
-    if args.channel_file is None:
-        host, port = io_nds2.host_resolution_order(args.ifo)[0]
-        channels = ChannelList.query_nds2('*.mean', host=host, port=port,
-                                          type='m-trend')
-    else:
-        with open(args.channel_file, 'r') as f:
-            channels = [name.rstrip('\n') for name in f]
-    nchan = len(channels)
-    LOGGER.debug("Identified %d channels" % nchan)
-
-    if trend_type == 'minute':
-        frametype = '%s_M' % args.ifo  # for minute trends
-    else:
-        frametype = '%s_T' % args.ifo  # for second trends
+        state_flag = f'{args.ifo}:DMT-ANALYSIS_READY:1'
+        state_is_observing = True
+        state_name = 'Observing'
+    state = DataQualityFlag.query(state_flag, start, end)
+    state.name = state_name
+    segs = state.active.coalesce()
+
+    # Loop over segments to create the "lasso segments", a perhaps slightly
+    # reduced length of segments because of the segment_padding argument and
+    # minimum length required
+    lasso_segs = SegmentList([])
+    for i, seg in enumerate(segs):
+        if abs(seg) >= args.segment_min_length:
+            padded_seg = seg.contract(args.segment_padding)
+            lasso_segs.append(padded_seg)
+
+    # Loop over lasso segments
+    files = []
+    gpsstubs = []
+    gpsblocks = []
+    subdirs = []
+    for i, seg in enumerate(lasso_segs):
+        gpsstub = f'{int(seg[0])}-{int(seg[1]-seg[0])}'
+        gpsblock = f'{int(seg[0])}-{int(seg[1])}'
+        subdir = os.path.join(args.output_dir, gpsblock)
+        gpsstubs.append(gpsstub)
+        gpsblocks.append(gpsblock)
+        subdirs.append(subdir)
+
+        os.makedirs(subdir, exist_ok=True)
+        os.chdir(subdir)
+
+        # Get auxiliary frames if there was no channel list provided
+        # Get the channels of interest, removing repeats
+        # Remove channels that are "bad" or "flat"
+        # Save channels used
+        if args.channel_file is None:
+            cache = find_urls(args.ifo[0], aux_frametype, seg[0], seg[1])
+            aux_channels = get_channel_names(cache[0])
+            aux_channels = list(filter(
+                lambda x: not remove_regex.search(x),
+                aux_channels,
+            ))
+            if args.remove_bad_chans:
+                LOGGER.debug(
+                    f"Removing flat/bad channels in segment {gpsblock}")
+                data = get_data(aux_channels, int(seg[0]), int(seg[0]) + 600,
+                                frametype=aux_frametype, nproc=args.nproc,
+                                pad=0)
+                data = gwlasso.remove_flat(data)
+                data = gwlasso.remove_bad(data)
+                aux_channels = list(data.keys())
+                filename = os.path.join(
+                    subdir, f'{args.ifo}-CHANNELS-{gpsstub}.txt')
+                files.append(filename)
+                numpy.savetxt(filename, aux_channels, fmt='%s')
+        else:
+            with open(args.channel_file, 'r') as f:
+                aux_channels = [name.rstrip('\n') for name in f]
 
-    # read aux channels
-    auxdata = get_data(
-        channels, start, end, verbose='Reading:'.rjust(30),
-        frametype=frametype, nproc=args.nproc, pad=0).crop(start, end)
-
-    # re-order aux channels to the same order as channel list
-
-    [auxdata.move_to_end(key=ch) for ch in channels if ch]
-
-    # -- removes flat data to be re-introdused later
-
-    LOGGER.info('-- Pre-processing auxiliary channel data')
-    auxdata = gwlasso.remove_flat(auxdata)
-    flatable = Table(data=(list(set(channels) - set(auxdata.keys())),),
-                     names=('Channels',))
-    LOGGER.debug('Removed {0} channels with flat data'.format(len(flatable)))
-    LOGGER.debug('{0} channels remaining'.format(len(auxdata)))
-
-    # -- remove bad data
-
-    LOGGER.info("Removing any channels with bad data...")
-    nbefore = len(auxdata)
-    auxdata = gwlasso.remove_bad(auxdata)
-    nafter = len(auxdata)
-    LOGGER.debug('Removed {0} channels with bad data'.format(nbefore - nafter))
-    LOGGER.debug('{0} channels remaining'.format(nafter))
-    data = numpy.array([ts.value for ts in auxdata.values()]).T
-    scaler = StandardScaler()
-    data = scaler.fit_transform(data)
-
-    # -- perform lasso regression -------------------
-
-    # create model
-    LOGGER.info('-- Fitting data to target')
-    target = scale(primaryts.value)
-    model = gwlasso.fit(data, target, alpha=args.alpha)
-    LOGGER.info('Alpha: {}'.format(model.alpha))
-
-    # restructure results for convenience
-    allresults = Table(
-        data=(list(auxdata.keys()), model.coef_, numpy.abs(model.coef_)),
-        names=('Channel', 'Lasso coefficient', 'rank'))
-    allresults.sort('rank')
-    allresults.reverse()
-    useful = allresults['rank'] > 0
-    allresults.remove_column('rank')
-    results = allresults[useful]  # non-zero coefficient
-    zeroed = allresults[numpy.invert(useful)]  # zero coefficient
-
-    # extract data for useful channels
-    nonzerodata = {name: auxdata[name] for name in results['Channel']}
-    nonzerocoef = {name: coeff for name, coeff in results.as_array()}
-
-    # print results
-    LOGGER.info('Found {} channels with |Lasso coefficient| >= {}:\n\n'.format(
-                len(results), threshold))
-    print(results)
-    print('\n\n')
+        """ Run lasso over segment """
 
-    # convert to pandas
-    set_option('max_colwidth', None)
-    df = results.to_pandas()
-    df.index += 1
-
-    # write results to files
-    gpsstub = '%d-%d' % (start, end-start)
-    resultsfile = '%s-LASSO_RESULTS-%s.csv' % (args.ifo, gpsstub)
-    results.write(resultsfile, format='csv', overwrite=True)
-    zerofile = '%s-ZERO_COEFFICIENT_CHANNELS-%s.csv' % (args.ifo, gpsstub)
-    zeroed.write(zerofile, format='csv', overwrite=True)
-    flatfile = '%s-FLAT_CHANNELS-%s.csv' % (args.ifo, gpsstub)
-    flatable.write(flatfile, format='csv', overwrite=True)
-
-    # -- generate lasso plots
-
-    modelFit = model.predict(data)
-
-    re_delim = re.compile(r'[:_-]')
-    p1 = (.1, .15, .9, .9)  # global plot defaults for plot1, lasso model
-
-    times = primaryts.times.value
-    xlim = primaryts.span
-    cmap = get_cmap('tab20')
-    colors = [cmap(i) for i in numpy.linspace(0, 1, len(nonzerodata)+1)]
-
-    plot = Plot(figsize=(12, 4))
-    plot.subplots_adjust(*p1)
-    ax = plot.gca()
-    ax.set_xscale('auto-gps')
-    ax.set_epoch(start)
-    ax.set_xlim(xlim)
-    ax.plot(times, _descaler(target), label=texify(primary),
-            color='black', linewidth=line_size_primary)
-    ax.plot(times, _descaler(modelFit), label='Lasso model',
-            linewidth=line_size_aux)
-    if range_is_primary:
-        ax.set_ylabel('Sensitive range [Mpc]')
-        ax.set_title('Lasso Model of Range')
-    else:
-        ax.set_ylabel('Primary Channel Units')
-        ax.set_title('Lasso Model of Primary Channel')
-    ax.legend(loc='best')
-    plot1 = gwplot.save_figure(
-         plot, '%s-LASSO_MODEL-%s.png' % (args.ifo, gpsstub),
-         bbox_inches='tight')
-
-    # summed contributions
-    plot = Plot(figsize=(12, 4))
-    plot.subplots_adjust(*p1)
-    ax = plot.gca()
-    ax.set_xscale('auto-gps')
-    ax.set_epoch(start)
-    ax.set_xlim(xlim)
-    ax.plot(times, _descaler(target), label=texify(primary),
-            color='black', linewidth=line_size_primary)
-    summed = 0
-    for i, name in enumerate(results['Channel']):
-        summed += scale(nonzerodata[name].value) * nonzerocoef[name]
-        if i:
-            label = 'Channels 1-{0}'.format(i+1)
+        # Get primary data and optionally bandpass
+        if args.band_pass:
+            try:
+                flower, fupper = args.band_pass
+            except TypeError:
+                flower, fupper = None
+
+            LOGGER.info("-- Loading primary channel data")
+            bandts = get_primary_ts(channel=primary,
+                                    start=int(seg[0]-args.filter_padding),
+                                    end=int(seg[1]+args.filter_padding),
+                                    filepath=args.primary_file,
+                                    frametype=args.primary_frametype,
+                                    cache=args.primary_cache,
+                                    nproc=args.nproc)
+            if flower < 0 or fupper >= float((bandts.sample_rate/2.).value):
+                raise ValueError(
+                    "bandpass frequency is out of range for this "
+                    f"channel, band (Hz): {args.band_pass}, sample rate: "
+                    f"{bandts.sample_rate}")
+
+            # get darm BLRMS
+            LOGGER.debug("-- Filtering data")
+            if trend_type == 'minute':
+                stride = 60
+            else:
+                stride = 1
+            if flower:
+                darmbl = (
+                    bandts.highpass(flower/2., fstop=flower/4.,
+                                    filtfilt=False, ftype='butter')
+                    .notch(60, filtfilt=False)
+                    .bandpass(flower, fupper, fstop=[flower/2., fupper*1.5],
+                              filtfilt=False, ftype='butter')
+                    .crop(int(seg[0]), int(seg[1])))
+                darmblrms = darmbl.rms(stride)
+                darmblrms.name = f'{primary} {flower}-{fupper} Hz BLRMS'
+            else:
+                darmbl = bandts.notch(60).crop(int(seg[0]), int(seg[1]))
+                darmblrms = darmbl.rms(stride)
+                darmblrms.name = f'{primary} RMS'
+
+            primaryts = darmblrms
+
+            bandts_asd = bandts.asd(4, 2, method='median')
+            darmbl_asd = darmbl.asd(4, 2, method='median')
+
+            spectrum_plots = gwplot.make_spectrum_plots(
+                int(seg[0]), int(seg[1]), flower, fupper, primary,
+                bandts_asd, darmbl_asd)
+            spectrum_plot_zoomed_out = spectrum_plots[0]
+            spectrum_plot_zoomed_in = spectrum_plots[1]
         else:
-            label = 'Channel 1'
-        ax.plot(times, _descaler(summed), label=label, color=colors[i],
+            # load primary channel data
+            LOGGER.info("-- Loading primary channel data")
+            primaryts = get_primary_ts(
+                channel=primary,
+                start=int(seg[0]),
+                end=int(seg[1]),
+                filepath=args.primary_file,
+                frametype=args.primary_frametype,
+                cache=args.primary_cache,
+                nproc=args.nproc)
+
+        if args.remove_outliers:
+            LOGGER.debug(
+                f"-- Removing outliers above {args.remove_outliers} sigma")
+            gwlasso.remove_outliers(primaryts, args.remove_outliers)
+        elif args.remove_outliers_pf:
+            LOGGER.debug("-- Removing outliers in the bottom "
+                         f"{args.remove_outliers_pf*100} percent of data")
+            gwlasso.remove_outliers(
+                primaryts, args.remove_outliers_pf, method='pf')
+            start = int(primaryts.span[0])
+            end = int(primaryts.span[1])
+
+        primary_mean = numpy.mean(primaryts.value)
+        primary_std = numpy.std(primaryts.value)
+
+        # -- get aux data
+        LOGGER.info("-- Loading auxiliary channel data")
+        nchan = len(aux_channels)
+        LOGGER.debug(f"Identified {nchan} channels")
+
+        # read aux channels
+        auxdata = get_data(
+            aux_channels,
+            int(seg[0]), int(seg[1]),
+            verbose='Reading:'.rjust(30),
+            frametype=aux_frametype,
+            nproc=args.nproc,
+            pad=0)
+
+        # re-order aux channels to the same order as channel list
+
+        [auxdata.move_to_end(key=ch) for ch in aux_channels if ch]
+
+        # -- removes flat data to be re-introdused later
+
+        LOGGER.info('-- Pre-processing auxiliary channel data')
+        auxdata = gwlasso.remove_flat(auxdata)
+        flatable = Table(data=(list(set(aux_channels) - set(auxdata.keys())),),
+                         names=('Channels',))
+        LOGGER.debug(f'Removed {len(flatable)} channels with flat data')
+        LOGGER.debug(f'{len(auxdata)} channels remaining')
+
+        # -- remove bad data
+
+        LOGGER.info("Removing any channels with bad data...")
+        nbefore = len(auxdata)
+        auxdata = gwlasso.remove_bad(auxdata)
+        nafter = len(auxdata)
+        LOGGER.debug(f'Removed {nbefore - nafter} channels with bad data')
+        LOGGER.debug(f'{nafter} channels remaining'.format())
+        data = numpy.array([ts.value for ts in auxdata.values()]).T
+        scaler = StandardScaler()
+        data = scaler.fit_transform(data)
+
+        # -- perform lasso regression -------------------
+
+        # create model
+        LOGGER.info('-- Fitting data to target')
+        target = scale(primaryts.value)
+        model = gwlasso.fit(data, target, alpha=args.alpha)
+        LOGGER.info(f'Alpha: {model.alpha}')
+
+        # restructure results for convenience
+        allresults = Table(
+            data=(list(auxdata.keys()), model.coef_, numpy.abs(model.coef_)),
+            names=('Channel', 'Lasso coefficient', 'rank'))
+        allresults.sort('rank')
+        allresults.reverse()
+        useful = allresults['rank'] > 0
+        allresults.remove_column('rank')
+        results = allresults[useful]  # non-zero coefficient
+        zeroed = allresults[numpy.invert(useful)]  # zero coefficient
+
+        # extract data for useful channels
+        nonzerodata = {name: auxdata[name] for name in results['Channel']}
+        nonzerocoef = {name: coeff for name, coeff in results.as_array()}
+
+        # print results
+        LOGGER.info(f'Found {len(results)} channels with |Lasso coefficient| '
+                    f'>= {threshold}:\n\n')
+        print(results)
+        print('\n\n')
+
+        # convert to pandas
+        set_option('max_colwidth', None)
+        df = results.to_pandas()
+        df.index += 1
+
+        # write results to files
+        resultsfile = f'{args.ifo}-LASSO_RESULTS-{gpsstub}.csv'
+        results.write(resultsfile, format='csv', overwrite=True)
+        zerofile = f'{args.ifo}-ZERO_COEFFICIENT_CHANNELS-{gpsstub}.csv'
+        zeroed.write(zerofile, format='csv', overwrite=True)
+        flatfile = f'{args.ifo}-FLAT_CHANNELS-{gpsstub}.csv'
+        flatable.write(flatfile, format='csv', overwrite=True)
+
+        # -- generate lasso plots
+
+        modelFit = model.predict(data)
+
+        re_delim = re.compile(r'[:_-]')
+        p1 = (.1, .15, .9, .9)  # global plot defaults for plot1, lasso model
+
+        times = primaryts.times.value
+        xlim = primaryts.span
+        cmap = get_cmap('tab20')
+        colors = [cmap(i) for i in numpy.linspace(0, 1, len(nonzerodata)+1)]
+
+        plot = Plot(figsize=(12, 4))
+        plot.subplots_adjust(*p1)
+        ax = plot.gca()
+        ax.set_xscale('auto-gps')
+        ax.set_epoch(seg[0])
+        ax.set_xlim(xlim)
+        ax.plot(times, _descaler(target), label=texify(primary),
+                color='black', linewidth=line_size_primary)
+        ax.plot(times, _descaler(modelFit), label='Lasso model',
                 linewidth=line_size_aux)
-    if range_is_primary:
-        ax.set_ylabel('Sensitive range [Mpc]')
-    else:
-        ax.set_ylabel('Primary Channel Units')
-    ax.set_title('Summations of Channel Contributions to Model')
-    ax.legend(loc='center left', bbox_to_anchor=(1.05, 0.5))
-    plot2 = gwplot.save_figure(
-        plot, '%s-LASSO_CHANNEL_SUMMATION-%s.png' % (args.ifo, gpsstub),
-        bbox_inches='tight')
-
-    # individual contributions
-    plot = Plot(figsize=(12, 4))
-    plot.subplots_adjust(*p1)
-    ax = plot.gca()
-    ax.set_xscale('auto-gps')
-    ax.set_epoch(start)
-    ax.set_xlim(xlim)
-    ax.plot(times, _descaler(target), label=texify(primary),
-            color='black', linewidth=line_size_primary)
-    for i, name in enumerate(results['Channel']):
-        this = _descaler(scale(nonzerodata[name].value) * nonzerocoef[name])
-        if i:
-            label = 'Channels 1-{0}'.format(i+1)
+        if range_is_primary:
+            ax.set_ylabel('Sensitive range [Mpc]')
+            ax.set_title('Lasso Model of Range')
         else:
-            label = 'Channel 1'
-        ax.plot(times, this, label=texify(name), color=colors[i],
-                linewidth=line_size_aux)
-    if range_is_primary:
-        ax.set_ylabel('Sensitive range [Mpc]')
-    else:
-        ax.set_ylabel('Primary Channel Units')
-    ax.set_title('Individual Channel Contributions to Model')
-    ax.legend(loc='center left', bbox_to_anchor=(1.05, 0.5))
-    plot3 = gwplot.save_figure(
-        plot, '%s-LASSO_CHANNEL_CONTRIBUTIONS-%s.png' % (args.ifo, gpsstub),
-        bbox_inches='tight')
-
-    # -- process aux channels, making plots
-
-    LOGGER.info("-- Processing channels")
-    counter = multiprocessing.Value('i', 0)
-
-    # process channels
-    pool = multiprocessing.Pool(nprocplot)
-    results = pool.map(_process_channel, enumerate(list(nonzerodata.items())))
-    results = sorted(results, key=lambda x: abs(x[1]), reverse=True)
-    pool.close()
-
-    #  generate clustered time series plots
-    counter = multiprocessing.Value('i', 0)
-    max_correlated_channels = 20
+            ax.set_ylabel('Primary Channel Units')
+            ax.set_title('Lasso Model of Primary Channel')
+        ax.legend(loc='best')
+        plot1 = gwplot.save_figure(
+            plot,
+            f'{args.ifo}-LASSO_MODEL-{gpsstub}.png',
+            bbox_inches='tight')
+
+        # summed contributions
+        plot = Plot(figsize=(12, 4))
+        plot.subplots_adjust(*p1)
+        ax = plot.gca()
+        ax.set_xscale('auto-gps')
+        ax.set_epoch(seg[0])
+        ax.set_xlim(xlim)
+        ax.plot(times, _descaler(target), label=texify(primary),
+                color='black', linewidth=line_size_primary)
+        summed = 0
+        for i, name in enumerate(results['Channel']):
+            summed += scale(nonzerodata[name].value) * nonzerocoef[name]
+            if i:
+                label = f'Channels 1-{i+1}'
+            else:
+                label = 'Channel 1'
+            ax.plot(times, _descaler(summed), label=label, color=colors[i],
+                    linewidth=line_size_aux)
+        if range_is_primary:
+            ax.set_ylabel('Sensitive range [Mpc]')
+        else:
+            ax.set_ylabel('Primary Channel Units')
+        ax.set_title('Summations of Channel Contributions to Model')
+        ax.legend(loc='center left', bbox_to_anchor=(1.05, 0.5))
+        plot2 = gwplot.save_figure(
+            plot,
+            f'{args.ifo}-LASSO_CHANNEL_SUMMATION-{gpsstub}.png',
+            bbox_inches='tight')
+
+        # individual contributions
+        plot = Plot(figsize=(12, 4))
+        plot.subplots_adjust(*p1)
+        ax = plot.gca()
+        ax.set_xscale('auto-gps')
+        ax.set_epoch(seg[0])
+        ax.set_xlim(xlim)
+        ax.plot(times, _descaler(target), label=texify(primary),
+                color='black', linewidth=line_size_primary)
+        for i, name in enumerate(results['Channel']):
+            this = _descaler(
+                scale(nonzerodata[name].value) * nonzerocoef[name])
+            if i:
+                label = 'Channels 1-{0}'.format(i+1)
+            else:
+                label = 'Channel 1'
+            ax.plot(times, this, label=texify(name), color=colors[i],
+                    linewidth=line_size_aux)
+        if range_is_primary:
+            ax.set_ylabel('Sensitive range [Mpc]')
+        else:
+            ax.set_ylabel('Primary Channel Units')
+        ax.set_title('Individual Channel Contributions to Model')
+        ax.legend(loc='center left', bbox_to_anchor=(1.05, 0.5))
+        plot3 = gwplot.save_figure(
+            plot,
+            f'{args.ifo}-LASSO_CHANNEL_CONTRIBUTIONS-{gpsstub}.png',
+            bbox_inches='tight')
+
+        # -- process aux channels, making plots
+
+        LOGGER.info("-- Processing channels")
+        counter = multiprocessing.Value('i', 0)
 
-    if args.no_cluster is False:
-        LOGGER.info("-- Generating clusters")
+        # process channels
         pool = multiprocessing.Pool(nprocplot)
-        clusters = pool.map(_generate_cluster, enumerate(results))
+        results = pool.map(_process_channel,
+                           enumerate(list(nonzerodata.items())))
+        results = sorted(results, key=lambda x: abs(x[1]), reverse=True)
         pool.close()
 
-    channelsfile = '%s-CHANNELS-%s.csv' % (args.ifo, gpsstub)
-    numpy.savetxt(channelsfile, channels, delimiter=',', fmt='%s')
+        #  generate clustered time series plots
+        counter = multiprocessing.Value('i', 0)
+        max_correlated_channels = 20
+
+        if args.no_cluster is False:
+            LOGGER.info("-- Generating clusters")
+            pool = multiprocessing.Pool(nprocplot)
+            clusters = pool.map(_generate_cluster, enumerate(results))
+            pool.close()
+
+        channelsfile = f'{args.ifo}-CHANNELS-{gpsstub}.csv'
+        numpy.savetxt(channelsfile, aux_channels, delimiter=',', fmt='%s')
+
+        # -- Generate a segment summary page
+
+        # write html
+        trange = f'{seg[0]}-{seg[1]}'
+        title = f'{args.ifo} Lasso Correlation: {trange}'
+        if args.band_pass:
+            links = [trange] + [(s, '#%s' % s.lower()) for s in
+                                ['Parameters', 'Spectra', 'Model', 'Results']]
+        else:
+            links = [trange] + [(s, '#%s' % s.lower()) for s in
+                                ['Parameters', 'Model', 'Results']]
+        (brand, class_) = htmlio.get_brand(args.ifo, 'Lasso', seg[0])
+        navbar = htmlio.navbar(links, class_=class_, brand=brand)
+        page = htmlio.new_bootstrap_page(
+            title=f'{args.ifo} Lasso | {trange}',
+            navbar=navbar)
+        page.h1(title, class_='pb-2 mt-3 mb-2 border-bottom')
+
+        # -- summary table
+        content = [
+            ('Primary channel', markup.oneliner.code(primary)),
+            ('Primary frametype', markup.oneliner.code(
+                args.primary_frametype) or '-'),
+            ('Primary cache file', markup.oneliner.code(
+                args.primary_cache) or '-'),
+            ('Outlier threshold', f'{args.remove_outliers} sigma'),
+            ('Lasso coefficient threshold', str(threshold)),
+            ('Cluster coefficient threshold', str(args.cluster_coefficient)),
+            ('Non-zero coefficients', str(numpy.count_nonzero(model.coef_))),
+            ('&alpha; (model)', '%.4f' % model.alpha)]
+        if args.band_pass:
+            content.insert(2, ('Primary bandpass',
+                               f'{flower}-{fupper} Hz'))
+        page.h2('Parameters', class_='mt-4 mb-4', id_='parameters')
+        page.div(class_='row')
+        page.div(class_='col-md-9 col-sm-12')
+        page.add(htmlio.parameter_table(
+            content, start=int(seg[0]), end=int(seg[1])))
+        page.div.close()  # col-md-9 col-sm-12
+
+        # -- download button
+        files = [
+            (f'{nchan} analyzed channels (CSV)', channelsfile),
+            (f'{len(flatable)} flat channels (CSV)', flatfile),
+            (f'{len(zeroed)} zeroed channels (CSV)', zerofile)]
+        page.div(class_='col-md-3 col-sm-12')
+        page.add(htmlio.download_btn(
+            files, label='Channel information',
+            btnclass=f'btn btn-{args.ifo.lower()} dropdown-toggle'))
+        page.div.close()  # col-md-3 col-sm-12
+        page.div.close()  # rowa
+
+        # -- command-line
+        page.h5('Command-line:')
+        page.add(htmlio.get_command_line(about=False, prog=PROG))
+
+        if args.band_pass:
+            page.h2('Primary channel spectra', class_='mt-4', id_='spectra')
+            page.div(class_='card border-light card-body shadow-sm')
+            page.div(class_='row')
+            page.div(class_='col-md-6')
+            spectra_img1 = htmlio.FancyPlot(spectrum_plot_zoomed_out)
+            page.add(htmlio.fancybox_img(spectra_img1))
+            page.div.close()  # col-md-6
+            page.div(class_='col-md-6')
+            spectra_img2 = htmlio.FancyPlot(spectrum_plot_zoomed_in)
+            page.add(htmlio.fancybox_img(spectra_img2))
+            page.div.close()  # col-md-6
+            page.div.close()  # row
+            page.div.close()  # card border-light card-body shadow-sm
 
-    # write html
-    trange = '%d-%d' % (start, end)
-    title = '%s Lasso Correlation: %s' % (args.ifo, trange)
-    if args.band_pass:
-        links = [trange] + [(s, '#%s' % s.lower()) for s in
-                            ['Parameters', 'Spectra', 'Model', 'Results']]
-    else:
-        links = [trange] + [(s, '#%s' % s.lower()) for s in
-                            ['Parameters', 'Model', 'Results']]
-    (brand, class_) = htmlio.get_brand(args.ifo, 'Lasso', start)
-    navbar = htmlio.navbar(links, class_=class_, brand=brand)
-    page = htmlio.new_bootstrap_page(
-        title='%s Lasso | %s' % (args.ifo, trange),
-        navbar=navbar)
-    page.h1(title, class_='pb-2 mt-3 mb-2 border-bottom')
-
-    # -- summary table
-    content = [
-        ('Primary channel', markup.oneliner.code(primary)),
-        ('Primary frametype', markup.oneliner.code(
-            args.primary_frametype) or '-'),
-        ('Primary cache file', markup.oneliner.code(
-            args.primary_cache) or '-'),
-        ('Outlier threshold', '%s sigma' % args.remove_outliers),
-        ('Lasso coefficient threshold', str(threshold)),
-        ('Cluster coefficient threshold', str(args.cluster_coefficient)),
-        ('Non-zero coefficients', str(numpy.count_nonzero(model.coef_))),
-        ('&alpha; (model)', '%.4f' % model.alpha)]
-    if args.band_pass:
-        content.insert(2, ('Primary bandpass',
-                           '{0}-{1} Hz'.format(flower, fupper)))
-    page.h2('Parameters', class_='mt-4 mb-4', id_='parameters')
-    page.div(class_='row')
-    page.div(class_='col-md-9 col-sm-12')
-    page.add(htmlio.parameter_table(content, start=start, end=end))
-    page.div.close()  # col-md-9 col-sm-12
-
-    # -- download button
-    files = [
-        ('%s analyzed channels (CSV)' % nchan, channelsfile),
-        ('%s flat channels (CSV)' % len(flatable), flatfile),
-        ('%s zeroed channels (CSV)' % len(zeroed), zerofile)]
-    page.div(class_='col-md-3 col-sm-12')
-    page.add(htmlio.download_btn(
-        files, label='Channel information',
-        btnclass='btn btn-%s dropdown-toggle' % args.ifo.lower()))
-    page.div.close()  # col-md-3 col-sm-12
-    page.div.close()  # rowa
-
-    # -- command-line
-    page.h5('Command-line:')
-    page.add(htmlio.get_command_line(about=False, prog=PROG))
-
-    if args.band_pass:
-        page.h2('Primary channel spectra', class_='mt-4', id_='spectra')
-        page.div(class_='card border-light card-body shadow-sm')
+        # -- model information
+        page.h2('Model information', class_='mt-4', id_='model')
+
+        page.div(class_='card card-%s card-body shadow-sm' % args.ifo.lower())
         page.div(class_='row')
-        page.div(class_='col-md-6')
-        spectra_img1 = htmlio.FancyPlot(spectrum_plot_zoomed_out)
-        page.add(htmlio.fancybox_img(spectra_img1))
-        page.div.close()  # col-md-6
-        page.div(class_='col-md-6')
-        spectra_img2 = htmlio.FancyPlot(spectrum_plot_zoomed_in)
-        page.add(htmlio.fancybox_img(spectra_img2))
-        page.div.close()  # col-md-6
+        page.div(class_='col-md-8 offset-md-2', id_='results-table')
+        page.p('Below are the top {} mean minute-trend channels, ranked by '
+               'Lasso correlation with the primary.'.format(df.shape[0]))
+        page.add(df.to_html(
+            classes=('table', 'table-sm', 'table-hover'),
+            formatters={
+                'Lasso coefficient': lambda x: "%.4f" % x,
+                'Channel': lambda x: str(htmlio.cis_link(x.split('.')[0])),
+                '__index__': lambda x: str(x)
+            },
+            escape=False,
+            border=0).replace(' style="text-align: right;"', ''))
+        page.div.close()  # col-md-10 offset-md-1
         page.div.close()  # row
-        page.div.close()  # card border-light card-body shadow-sm
-
-    # -- model information
-    page.h2('Model information', class_='mt-4', id_='model')
 
-    page.div(class_='card card-%s card-body shadow-sm' % args.ifo.lower())
-    page.div(class_='row')
-    page.div(class_='col-md-8 offset-md-2', id_='results-table')
-    page.p('Below are the top {} mean minute-trend channels, ranked by '
-           'Lasso correlation with the primary.'.format(df.shape[0]))
-    page.add(df.to_html(
-        classes=('table', 'table-sm', 'table-hover'),
-        formatters={
-            'Lasso coefficient': lambda x: "%.4f" % x,
-            'Channel': lambda x: str(htmlio.cis_link(x.split('.')[0])),
-            '__index__': lambda x: str(x)
-        },
-        escape=False,
-        border=0).replace(' style="text-align: right;"', ''))
-    page.div.close()  # col-md-10 offset-md-1
-    page.div.close()  # row
+        page.div(class_='row', id_='primary-lasso')
+        page.div(class_='col-md-8 offset-md-2')
+        img1 = htmlio.FancyPlot(plot1)
+        page.add(htmlio.fancybox_img(img1))  # primary lasso plot
+        page.div.close()  # col-md-8 offset-md-2
+        page.div.close()  # primary-lasso
+
+        page.div(class_='row', id_='channel-summation')
+        img2 = htmlio.FancyPlot(plot2)
+        page.div(class_='col-md-8 offset-md-2')
+        page.add(htmlio.fancybox_img(img2))
+        page.div.close()  # col-md-8 offset-md-2
+        page.div.close()  # channel-summation
+
+        page.div(class_='row', id_='channels-and-primary')
+        img3 = htmlio.FancyPlot(plot3)
+        page.div(class_='col-md-8 offset-md-2')
+        page.add(htmlio.fancybox_img(img3))
+        page.div.close()  # col-md-8 offset-md-2
+        page.div.close()  # channels-and-primary
+
+        page.div.close()  # card card-<ifo> card-body shadow-sm
+
+        # -- results
+        page.h2('Top channels', class_='mt-4', id_='results')
+        page.div(id_='results')
+        # for each aux channel, create information container and put
+        # plots in it
+        for i, (ch, lassocoef, plot4, plot5, plot6, ts) in enumerate(results):
+            # set container color/context based on lasso coefficient
+            if lassocoef == 0:
+                break
+            elif abs(lassocoef) < threshold:
+                h = '%s [lasso coefficient = %.4f] (Below threshold)' % (
+                    ch, lassocoef)
+            else:
+                h = '%s [lasso coefficient = %.4f]' % (ch, lassocoef)
+            if ((lassocoef is None) or (lassocoef == 0)
+                    or (abs(lassocoef) < threshold)):
+                card = 'card border-light mb-1 shadow-sm'
+                card_header = 'card-header bg-light'
+            elif abs(lassocoef) >= .5:
+                card = 'card border-danger mb-1 shadow-sm'
+                card_header = 'card-header text-white bg-danger'
+            elif abs(lassocoef) >= .2:
+                card = 'card border-warning mb-1 shadow-sm'
+                card_header = 'card-header text-white bg-warning'
+            else:
+                card = 'card border-info mb-1 shadow-sm'
+                card_header = 'card-header text-white bg-info'
+            page.div(class_=card)
+
+            # heading
+            page.div(class_=card_header)
+            page.a(h, class_='collapsed card-link cis-link',
+                   href='#channel{i}', **{'data-toggle': 'collapse'})
+            page.div.close()  # card-header
+            # body
+            page.div(id_='channel%d' % i, class_='collapse',
+                     **{'data-parent': '#results'})
+            page.div(class_='card-body')
+            if lassocoef is None:
+                page.p('The amplitude data for this channel is flat (does not '
+                       'change) within the chosen time period.')
+            elif abs(lassocoef) < threshold:
+                page.p('Lasso coefficient below the threshold of %g.'
+                       % (threshold))
+            else:
+                for image in [plot4, plot5, plot6]:
+                    img = htmlio.FancyPlot(image)
+                    page.div(class_='row')
+                    page.div(class_='col-md-8 offset-md-2')
+                    page.add(htmlio.fancybox_img(img))
+                    page.div.close()  # col-md-8 offset-md-2
+                    page.div.close()  # row
+                    page.add('<hr class="row-divider">')
+                if args.no_cluster is False:
+                    if clusters[i][0] is None:
+                        page.p("<font size='3'><br />No channels were highly "
+                               "correlated with this channel.</font>")
+                    else:
+                        page.div(class_='row', id_='clusters')
+                        page.div(class_='col-md-12')
+                        cimg = htmlio.FancyPlot(clusters[i][0])
+                        page.add(htmlio.fancybox_img(cimg))
+                        page.div.close()  # col-md-12
+                        page.div.close()  # clusters
+                        if clusters[i][1] is not None:
+                            corr_link = markup.oneliner.a(
+                                'Export {} channels (CSV)'.format(
+                                    max_correlated_channels),
+                                href=clusters[i][1], download=clusters[i][1],
+                            )
+                            page.button(
+                                corr_link,
+                                class_='btn btn-%s' % args.ifo.lower(),
+                            )
+            page.div.close()  # card-body
+            page.div.close()  # collapse
+            page.div.close()  # card
+        page.div.close()  # results
+        htmlio.close_page(page, 'index.html')  # save and close
+
+    # -- Generate an overview summary page
+
+    LOGGER.info("Generating summary page")
+
+    os.makedirs(args.summary_dir, exist_ok=True)
+    os.chdir(args.summary_dir)
+
+    external_link = args.output_dir.replace(
+        os.path.join(os.environ.get('HOME'), 'public_html'),
+        f'/~{getuser()}'
+    )
 
-    page.div(class_='row', id_='primary-lasso')
-    page.div(class_='col-md-8 offset-md-2')
-    img1 = htmlio.FancyPlot(plot1)
-    page.add(htmlio.fancybox_img(img1))  # primary lasso plot
-    page.div.close()  # col-md-8 offset-md-2
-    page.div.close()  # primary-lasso
+    # get primary channel data
+    # gds_channel = '%s:DMT-SNSH_EFFECTIVE_RANGE_MPC.mean' % ifo
+    # frontend_channel = '%s:DMT-SNSW_EFFECTIVE_RANGE_MPC.mean' % ifo
+
+    primary_ts = get_data(primary, start, end, pad=numpy.nan,
+                          frametype=args.primary_frametype)
+
+    """gds_timeseries = get_data(
+        gds_channel, gpsstart, gpsend, pad=numpy.nan,
+        frametype='SenseMonitor_hoft_%s' % frametype)
+    frontend_timeseries = get_data(
+        frontend_channel, gpsstart, gpsend, pad=numpy.nan,
+        frametype='SenseMonitor_CAL_%s' % frametype)"""
+
+    # construct primary channel timseries plot
+    range_plot = Plot(figsize=(12, 6))
+    ax = range_plot.gca()
+    if args.ifo == 'H1':
+        ax.plot(primary_ts, color='gwpy:ligo-hanford', label='Primary',
+                linewidth=1)
+    else:
+        ax.plot(primary_ts, color='gwpy:ligo-livingston', label='Primary',
+                linewidth=1)
+    ax.set_xscale('hours')
+    ax.set_epoch(start)
+    ax.set_xlim(start, end)
+    if range_is_primary:
+        ax.set_ylim(-5, 180)
+        ax.set_ylabel('Angle-averaged range [Mpc]')
+        ax.set_title(f'{args.ifo} binary neutron star inspiral range '
+                     '(DMT SenseMon)')
+    else:
+        ax.set_label('Primary channel units')
+    ax.legend(loc='upper left', bbox_to_anchor=(1, 1))
+    range_plot.add_segments_bar(state, ax=ax, pad=.1, height=.14)
+    gpsstub_day = f'{start}-86400'
+    if state_is_observing:
+        range_filename = (f'{args.ifo}-OBSERVING_TIMESERIES-{gpsstub_day}.png')
+    else:
+        range_filename = (f'{args.ifo}-LOCKED-TIMESERIES-{gpsstub_day}.png')
+    range_plot.savefig(range_filename, bbox_inches='tight')
 
-    page.div(class_='row', id_='channel-summation')
-    img2 = htmlio.FancyPlot(plot2)
-    page.div(class_='col-md-8 offset-md-2')
-    page.add(htmlio.fancybox_img(img2))
-    page.div.close()  # col-md-8 offset-md-2
-    page.div.close()  # channel-summation
+    # generate summaries of lasso models for each data-quality segment
+    set_option('max_colwidth', None)
+    seg_page_links = []
+    dataframes = []
+    seg_plot_links = []
+    for i, subdir in enumerate(subdirs):
+        seg_page_links.append(os.path.join(external_link, gpsblocks[i]))
+        dataframes.append(None)
+        seg_plot_links.append(None)
+        for file_ in os.listdir(subdir):
+            if fnmatch.fnmatch(file_, f'{args.ifo}-LASSO_RESULTS-*'):
+                file_ = '/'.join([subdir, file_])
+                usefultab = Table.read(file_, format='csv')
+                df = usefultab.to_pandas()
+                df.index += 1
+                if len(df) == 0:
+                    df = None
+                dataframes[i] = df
+
+            elif fnmatch.fnmatch(file_,
+                                 f'{args.ifo}-LASSO_CHANNEL_SUMMATION-*'):
+                summations_plot_link = (os.path.join(
+                    external_link,
+                    gpsblocks[i],
+                    f'{args.ifo}-LASSO_CHANNEL_SUMMATION-{gpsstubs[i]}.png'))
+                seg_plot_links[i] = summations_plot_link
+
+    # generate HTML page
+    title = f'Lasso Slow Correlations: {start}-{end}'
+    sections = [[f'{i+1}: {gpsblocks[i]}', f'#{gpsblocks[i]}']
+                for i, seg in enumerate(gpsblocks)]
+    date = tconvert(start)
+    links = ['-'.join([date.year, date.month, date.day]),
+             ['Summary', '#'],
+             ['Segments', [['Analyses', sections]]]]
+    (brand, class_) = htmlio.get_brand(args.ifo, 'Daily Lasso', start)
+    navbar = htmlio.navbar(links, class_=class_, brand=brand)
+    page = htmlio.new_bootstrap_page(title=title, navbar=navbar)
 
-    page.div(class_='row', id_='channels-and-primary')
-    img3 = htmlio.FancyPlot(plot3)
+    # page header
+    page.div(class_='page-header')
+    page.h1(title)
+    lasso_link = 'https://www.jstor.org/stable/2346178'
+    paper_link = 'http://dx.doi.org/10.1088/1361-6382/aae593'
+    if range_is_primary:
+        primary_nickname = f'BNS range (<code>{args.primary_channel}</code>)'
+    else:
+        primary_nickname = f'<code>{args.primary_channel}</code> channel'
+    page.add(htmlio.alert(
+        'This algorithm uses <a href="{0}" class="alert-link" target="_blank">'
+        'lasso regression</a> to create a model for fluctuations in the {1} '
+        'based on information in auxiliary channels. Using minute trend data, '
+        'a minimal set of channels is selected and then clustering is '
+        'performed to find closely-related channels. For more information, '
+        'see <a href="{2}" class="alert-link" target="_blank">Walker et al. '
+        '(2018)</a>.'.format(
+            lasso_link, primary_nickname, paper_link),
+        ))
+    page.add(htmlio.get_command_line())
+    page.div.close()  # page-header
+
+    img = htmlio.FancyPlot(
+        '/'.join(
+            [external_link.replace('full-results', 'summary'),
+             range_filename]),
+        caption='{ifo} binary neutron star inspiral range on {date}. The '
+                'colorful trace represents the range based on <code>'
+                '{ifo}:GDS-CALIB_STRAIN</code>, while the gray trace is based '
+                'on <code>{ifo}:CAL-DELTAL_EXTERNAL_DQ</code>.'.format(
+                    ifo=args.ifo, date=date.strftime('%Y%m%d')))
+    page.div(class_='row')
     page.div(class_='col-md-8 offset-md-2')
-    page.add(htmlio.fancybox_img(img3))
+    page.add(htmlio.fancybox_img(img))  # primary lasso plot
     page.div.close()  # col-md-8 offset-md-2
-    page.div.close()  # channels-and-primary
-
-    page.div.close()  # card card-<ifo> card-body shadow-sm
+    page.div.close()  # row
 
-    # -- results
-    page.h2('Top channels', class_='mt-4', id_='results')
-    page.div(id_='results')
-    # for each aux channel, create information container and put plots in it
-    for i, (ch, lassocoef, plot4, plot5, plot6, ts) in enumerate(results):
-        # set container color/context based on lasso coefficient
-        if lassocoef == 0:
-            break
-        elif abs(lassocoef) < threshold:
-            h = '%s [lasso coefficient = %.4f] (Below threshold)' % (
-                ch, lassocoef)
-        else:
-            h = '%s [lasso coefficient = %.4f]' % (ch, lassocoef)
-        if ((lassocoef is None) or (lassocoef == 0)
-                or (abs(lassocoef) < threshold)):
-            card = 'card border-light mb-1 shadow-sm'
-            card_header = 'card-header bg-light'
-        elif abs(lassocoef) >= .5:
-            card = 'card border-danger mb-1 shadow-sm'
-            card_header = 'card-header text-white bg-danger'
-        elif abs(lassocoef) >= .2:
-            card = 'card border-warning mb-1 shadow-sm'
-            card_header = 'card-header text-white bg-warning'
-        else:
-            card = 'card border-info mb-1 shadow-sm'
-            card_header = 'card-header text-white bg-info'
-        page.div(class_=card)
-
-        # heading
-        page.div(class_=card_header)
-        page.a(h, class_='collapsed card-link cis-link', href='#channel%d' % i,
-               **{'data-toggle': 'collapse'})
-        page.div.close()  # card-header
-        # body
-        page.div(id_='channel%d' % i, class_='collapse',
-                 **{'data-parent': '#results'})
+    page.div(id_='main')
+    page.div(class_='banner')
+    page.h2('Results Summary', id_='summary')
+    page.div.close()  # banner
+
+    if len(lasso_segs) == 0:
+        page.add(htmlio.alert(
+            f'No segments of length {args.segment_min_length/3600} hours or '
+            f'longer were found in state <code>{state_flag}</code> on '
+            f'{date.year}-{date.month}-{date.day}',
+            dismiss=False,
+        ))
+    else:
+        page.add(htmlio.alert(
+            f'A total of {len(segs)} segments were found in state '
+            f'<code>{state_flag}</code> on {date.year}-{date.month}-'
+            f'{date.day}, of which {len(lasso_segs)} are at least '
+            f'{args.segment_min_length/3600} hours long. These are '
+            'summarized and linked below. The list of channels for each '
+            'segment represents the largest contributors in modeling '
+            f'{primary_nickname}.',
+        ))
+
+    for i, link in enumerate(seg_page_links):
+        page.div(class_=f'card card-{args.ifo.lower()} mb-4 shadow-sm')
+        page.div(class_='card-header pb-0')
+        page.h5(gpsblocks[i], class_='card-title', id_=gpsblocks[i])
+        page.div.close()  # card-header pb-0
         page.div(class_='card-body')
-        if lassocoef is None:
-            page.p('The amplitude data for this channel is flat (does not '
-                   'change) within the chosen time period.')
-        elif abs(lassocoef) < threshold:
-            page.p('Lasso coefficient below the threshold of %g.'
-                   % (threshold))
+        tableid = f'{args.ifo.lower()}_lasso_{gpsblocks[i]}'
+        page.div(class_='container')
+        if dataframes[i] is None:
+            page.div('No page was generated for this segment',
+                     class_='alert alert-danger')
         else:
-            for image in [plot4, plot5, plot6]:
-                img = htmlio.FancyPlot(image)
+            page.div(class_='row', id_='results-table')
+            page.div(class_='col-md-9 col-sm-12')
+            page.p(f'Below are the top {dataframes[i].shape[0]} mean minute-'
+                   'trend channels, ranked by Lasso correlation with the '
+                   'primary.')
+            page.add(dataframes[i].to_html(
+                classes=('table', 'table-sm', 'table-hover'),
+                formatters={
+                    'Lasso coefficient': lambda x: "%.4f" % x,
+                    'Channel': lambda x: str(htmlio.cis_link(x.split('.')[0])),
+                    '__index__': lambda x: "%d" % x
+                },
+                escape=False,
+                border=0,
+                table_id=tableid).replace(' style="text-align: right;"', ''))
+            page.div.close()  # col-md-9 col-sm-12
+            page.div(class_='col-md-3 col-sm-12')
+            page.div(class_='float-right d-none d-md-block')
+            page.a('Full results', class_=f'btn btn-{args.ifo.lower()}',
+                   href=link, role='button')
+            page.div.close()  # float-right d-none d-md-block
+            page.div.close()  # col-md-3 col-sm-12
+            page.div.close()  # results-table
+            page.hr(class_='row-divider')
+            # no summary plot available
+            if seg_plot_links[i] is None:
+                page.div('This segment failed to generate a summary plot',
+                         class_='alert alert-warning')
+            else:
+                page.div(class_='container', id_='channel-summation')
+                img2 = htmlio.FancyPlot(seg_plot_links[i])
                 page.div(class_='row')
-                page.div(class_='col-md-8 offset-md-2')
-                page.add(htmlio.fancybox_img(img))
-                page.div.close()  # col-md-8 offset-md-2
+                page.div(class_='col-md-12')
+                page.add(htmlio.fancybox_img(img2))
+                page.div.close()  # col-md-12
                 page.div.close()  # row
-                page.add('<hr class="row-divider">')
-            if args.no_cluster is False:
-                if clusters[i][0] is None:
-                    page.p("<font size='3'><br />No channels were highly "
-                           "correlated with this channel.</font>")
-                else:
-                    page.div(class_='row', id_='clusters')
-                    page.div(class_='col-md-12')
-                    cimg = htmlio.FancyPlot(clusters[i][0])
-                    page.add(htmlio.fancybox_img(cimg))
-                    page.div.close()  # col-md-12
-                    page.div.close()  # clusters
-                    if clusters[i][1] is not None:
-                        corr_link = markup.oneliner.a(
-                            'Export {} channels (CSV)'.format(
-                                max_correlated_channels),
-                            href=clusters[i][1], download=clusters[i][1],
-                        )
-                        page.button(
-                            corr_link,
-                            class_='btn btn-%s' % args.ifo.lower(),
-                        )
+                page.div.close()  # channel-summation
+        page.div.close()  # container
         page.div.close()  # card-body
-        page.div.close()  # collapse
-        page.div.close()  # card
-    page.div.close()  # results
-    htmlio.close_page(page, 'index.html')  # save and close
+        page.div.close()  # card well
+
+    # close page
+    page.div.close()  # main
+    htmlio.close_page(page, 'index.html')
+
     LOGGER.info("-- Process Completed")
 
 
 # -- run from command-line ----------------------------------------------------
 
 if __name__ == "__main__":
     main()
```

### Comparing `gwdetchar-2.1.1/gwdetchar/lasso/core.py` & `gwdetchar-2.1.2/gwdetchar/lasso/core.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.1/gwdetchar/lasso/old.py` & `gwdetchar-2.1.2/gwdetchar/lasso/old.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.1/gwdetchar/lasso/plot.py` & `gwdetchar-2.1.2/gwdetchar/lasso/plot.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.1/gwdetchar/lasso/tests/__init__.py` & `gwdetchar-2.1.2/gwdetchar/lasso/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.1/gwdetchar/lasso/tests/test_core.py` & `gwdetchar-2.1.2/gwdetchar/lasso/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.1/gwdetchar/lasso/tests/test_main.py` & `gwdetchar-2.1.2/gwdetchar/lasso/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.1/gwdetchar/lasso/tests/test_plot.py` & `gwdetchar-2.1.2/gwdetchar/lasso/tests/test_plot.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.1/gwdetchar/mct.py` & `gwdetchar-2.1.2/gwdetchar/mct.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.1/gwdetchar/nagios/__init__.py` & `gwdetchar-2.1.2/gwdetchar/nagios/__init__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.1/gwdetchar/nagios/__main__.py` & `gwdetchar-2.1.2/gwdetchar/nagios/__main__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.1/gwdetchar/nagios/core.py` & `gwdetchar-2.1.2/gwdetchar/nagios/core.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.1/gwdetchar/nagios/tests/__init__.py` & `gwdetchar-2.1.2/gwdetchar/nagios/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.1/gwdetchar/nagios/tests/test_main.py` & `gwdetchar-2.1.2/gwdetchar/nagios/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.1/gwdetchar/omega/__init__.py` & `gwdetchar-2.1.2/gwdetchar/omega/__init__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.1/gwdetchar/omega/__main__.py` & `gwdetchar-2.1.2/gwdetchar/omega/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -381,14 +381,18 @@
                 analyzed = _load_channel_from_checkpoint(
                     blocks[channel.section].name, channel, analyzed,
                     completed, record, (correlate is not None))
                 htmlv['toc'] = analyzed
                 html.write_qscan_page(ifo, gps, analyzed, **htmlv)
                 continue
 
+            if channel.name not in data:
+                # Channel must not have been found by get_data()
+                continue
+
             analyzed = _scan_channel(
                 channel, data[channel.name], analyzed, gps, block,
                 args.far_threshold, (args.frequency_scaling == 'log'),
                 args.frequency_scaling, args.colormap,
                 blocks[channel.section].name, correlate)
             htmlv['toc'] = analyzed
             html.write_qscan_page(ifo, gps, analyzed, **htmlv)
```

### Comparing `gwdetchar-2.1.1/gwdetchar/omega/batch.py` & `gwdetchar-2.1.2/gwdetchar/omega/batch.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.1/gwdetchar/omega/config.py` & `gwdetchar-2.1.2/gwdetchar/omega/config.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.1/gwdetchar/omega/core.py` & `gwdetchar-2.1.2/gwdetchar/omega/core.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.1/gwdetchar/omega/html.py` & `gwdetchar-2.1.2/gwdetchar/omega/html.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.1/gwdetchar/omega/plot.py` & `gwdetchar-2.1.2/gwdetchar/omega/plot.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.1/gwdetchar/omega/tests/__init__.py` & `gwdetchar-2.1.2/gwdetchar/omega/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.1/gwdetchar/omega/tests/test_batch.py` & `gwdetchar-2.1.2/gwdetchar/omega/tests/test_batch.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.1/gwdetchar/omega/tests/test_config.py` & `gwdetchar-2.1.2/gwdetchar/omega/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.1/gwdetchar/omega/tests/test_core.py` & `gwdetchar-2.1.2/gwdetchar/omega/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.1/gwdetchar/omega/tests/test_html.py` & `gwdetchar-2.1.2/gwdetchar/omega/tests/test_html.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.1/gwdetchar/omega/tests/test_main.py` & `gwdetchar-2.1.2/gwdetchar/omega/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.1/gwdetchar/omega/tests/test_plot.py` & `gwdetchar-2.1.2/gwdetchar/omega/tests/test_plot.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.1/gwdetchar/overflow.py` & `gwdetchar-2.1.2/gwdetchar/overflow.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.1/gwdetchar/plot.py` & `gwdetchar-2.1.2/gwdetchar/plot.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.1/gwdetchar/saturation/__init__.py` & `gwdetchar-2.1.2/gwdetchar/saturation/__init__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.1/gwdetchar/saturation/__main__.py` & `gwdetchar-2.1.2/gwdetchar/saturation/__main__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.1/gwdetchar/saturation/core.py` & `gwdetchar-2.1.2/gwdetchar/saturation/core.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.1/gwdetchar/saturation/tests/__init__.py` & `gwdetchar-2.1.2/gwdetchar/saturation/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.1/gwdetchar/saturation/tests/test_saturation.py` & `gwdetchar-2.1.2/gwdetchar/saturation/tests/test_saturation.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.1/gwdetchar/scattering/__init__.py` & `gwdetchar-2.1.2/gwdetchar/scattering/__init__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.1/gwdetchar/scattering/__main__.py` & `gwdetchar-2.1.2/gwdetchar/scattering/__main__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.1/gwdetchar/scattering/core.py` & `gwdetchar-2.1.2/gwdetchar/scattering/core.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.1/gwdetchar/scattering/plot.py` & `gwdetchar-2.1.2/gwdetchar/scattering/plot.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.1/gwdetchar/scattering/simple.py` & `gwdetchar-2.1.2/gwdetchar/scattering/simple.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.1/gwdetchar/scattering/tests/__init__.py` & `gwdetchar-2.1.2/gwdetchar/scattering/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.1/gwdetchar/scattering/tests/test_core.py` & `gwdetchar-2.1.2/gwdetchar/scattering/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.1/gwdetchar/scattering/tests/test_main.py` & `gwdetchar-2.1.2/gwdetchar/scattering/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.1/gwdetchar/scattering/tests/test_plot.py` & `gwdetchar-2.1.2/gwdetchar/scattering/tests/test_plot.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.1/gwdetchar/scattering/tests/test_simple.py` & `gwdetchar-2.1.2/gwdetchar/scattering/tests/test_simple.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.1/gwdetchar/tests/__init__.py` & `gwdetchar-2.1.2/gwdetchar/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.1/gwdetchar/tests/test_cds.py` & `gwdetchar-2.1.2/gwdetchar/tests/test_cds.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.1/gwdetchar/tests/test_cli.py` & `gwdetchar-2.1.2/gwdetchar/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.1/gwdetchar/tests/test_condor.py` & `gwdetchar-2.1.2/gwdetchar/tests/test_condor.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.1/gwdetchar/tests/test_conlog.py` & `gwdetchar-2.1.2/gwdetchar/tests/test_conlog.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.1/gwdetchar/tests/test_const.py` & `gwdetchar-2.1.2/gwdetchar/tests/test_const.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.1/gwdetchar/tests/test_daq.py` & `gwdetchar-2.1.2/gwdetchar/tests/test_daq.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.1/gwdetchar/tests/test_plot.py` & `gwdetchar-2.1.2/gwdetchar/tests/test_plot.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.1/gwdetchar/tests/test_utils.py` & `gwdetchar-2.1.2/gwdetchar/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.1/gwdetchar/utils.py` & `gwdetchar-2.1.2/gwdetchar/utils.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.1/gwdetchar.egg-info/PKG-INFO` & `gwdetchar-2.1.2/gwdetchar.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gwdetchar
-Version: 2.1.1
+Version: 2.1.2
 Summary: A python package for gravitational-wave detector characterisation
 Author-email: Alex Urban <alex.urban@ligo.org>, Duncan Macleod <duncan.macleod@ligo.org>
 Maintainer-email: Evan Goetz <evan.goetz@ligo.org>
 License: GPL-3.0-or-later
 Project-URL: Documentation, https://gwdetchar.readthedocs.io
 Project-URL: Source Code, https://github.com/gwdetchar/gwdetchar
 Project-URL: Bug Tracker, https://github.com/gwdetchar/gwdetchar/issues
```

### Comparing `gwdetchar-2.1.1/gwdetchar.egg-info/SOURCES.txt` & `gwdetchar-2.1.2/gwdetchar.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.1/gwdetchar.egg-info/entry_points.txt` & `gwdetchar-2.1.2/gwdetchar.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.1/pyproject.toml` & `gwdetchar-2.1.2/pyproject.toml`

 * *Files identical despite different names*

