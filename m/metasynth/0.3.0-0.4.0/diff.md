# Comparing `tmp/metasynth-0.3.0.tar.gz` & `tmp/metasynth-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metasynth-0.3.0.tar", last modified: Tue May 30 10:06:34 2023, max compression
+gzip compressed data, was "metasynth-0.4.0.tar", last modified: Fri Aug  4 17:09:59 2023, max compression
```

## Comparing `metasynth-0.3.0.tar` & `metasynth-0.4.0.tar`

### file list

```diff
@@ -1,84 +1,119 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:06:34.425552 metasynth-0.3.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:06:34.413552 metasynth-0.3.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:06:34.417552 metasynth-0.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-05-30 10:06:22.000000 metasynth-0.3.0/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-05-30 10:06:22.000000 metasynth-0.3.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-30 10:06:22.000000 metasynth-0.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-05-30 10:06:22.000000 metasynth-0.3.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-05-30 10:06:22.000000 metasynth-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6154 2023-05-30 10:06:34.425552 metasynth-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4030 2023-05-30 10:06:22.000000 metasynth-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:06:34.417552 metasynth-0.3.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-30 10:06:22.000000 metasynth-0.3.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-30 10:06:22.000000 metasynth-0.3.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-30 10:06:22.000000 metasynth-0.3.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)    85618 2023-05-30 10:06:22.000000 metasynth-0.3.0/docs/soda.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:06:34.417552 metasynth-0.3.0/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:06:34.417552 metasynth-0.3.0/docs/source/api/
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-30 10:06:22.000000 metasynth-0.3.0/docs/source/api/metasynth.distribution.regex.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-05-30 10:06:22.000000 metasynth-0.3.0/docs/source/api/metasynth.distribution.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-30 10:06:22.000000 metasynth-0.3.0/docs/source/api/metasynth.rst
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-30 10:06:22.000000 metasynth-0.3.0/docs/source/api/metasynth.schema.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-05-30 10:06:22.000000 metasynth-0.3.0/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     7074 2023-05-30 10:06:22.000000 metasynth-0.3.0/docs/source/developer.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-05-30 10:06:22.000000 metasynth-0.3.0/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-05-30 10:06:22.000000 metasynth-0.3.0/docs/source/quick_start.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:06:34.417552 metasynth-0.3.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)    59754 2023-05-30 10:06:22.000000 metasynth-0.3.0/examples/advanced_tutorial.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-05-30 10:06:22.000000 metasynth-0.3.0/examples/basic_example.json
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-05-30 10:06:22.000000 metasynth-0.3.0/examples/basic_example.py
--rw-r--r--   0 runner    (1001) docker     (123)    81698 2023-05-30 10:06:22.000000 metasynth-0.3.0/examples/demonstration.csv
--rw-r--r--   0 runner    (1001) docker     (123)    12709 2023-05-30 10:06:22.000000 metasynth-0.3.0/examples/descriptions.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    37464 2023-05-30 10:06:22.000000 metasynth-0.3.0/examples/titanic.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-05-30 10:06:22.000000 metasynth-0.3.0/examples/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:06:34.421552 metasynth-0.3.0/metasynth/
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-05-30 10:06:22.000000 metasynth-0.3.0/metasynth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-30 10:06:34.000000 metasynth-0.3.0/metasynth/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     9861 2023-05-30 10:06:22.000000 metasynth-0.3.0/metasynth/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:06:34.421552 metasynth-0.3.0/metasynth/demo/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-30 10:06:22.000000 metasynth-0.3.0/metasynth/demo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-05-30 10:06:22.000000 metasynth-0.3.0/metasynth/demo/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    81698 2023-05-30 10:06:22.000000 metasynth-0.3.0/metasynth/demo/demo_titanic.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:06:34.421552 metasynth-0.3.0/metasynth/distribution/
--rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-05-30 10:06:22.000000 metasynth-0.3.0/metasynth/distribution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7326 2023-05-30 10:06:22.000000 metasynth-0.3.0/metasynth/distribution/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-05-30 10:06:22.000000 metasynth-0.3.0/metasynth/distribution/categorical.py
--rw-r--r--   0 runner    (1001) docker     (123)     6846 2023-05-30 10:06:22.000000 metasynth-0.3.0/metasynth/distribution/continuous.py
--rw-r--r--   0 runner    (1001) docker     (123)     5938 2023-05-30 10:06:22.000000 metasynth-0.3.0/metasynth/distribution/datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)     4411 2023-05-30 10:06:22.000000 metasynth-0.3.0/metasynth/distribution/discrete.py
--rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-05-30 10:06:22.000000 metasynth-0.3.0/metasynth/distribution/faker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:06:34.421552 metasynth-0.3.0/metasynth/distribution/regex/
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-30 10:06:22.000000 metasynth-0.3.0/metasynth/distribution/regex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7768 2023-05-30 10:06:22.000000 metasynth-0.3.0/metasynth/distribution/regex/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    17577 2023-05-30 10:06:22.000000 metasynth-0.3.0/metasynth/distribution/regex/element.py
--rw-r--r--   0 runner    (1001) docker     (123)    11484 2023-05-30 10:06:22.000000 metasynth-0.3.0/metasynth/distribution/regex/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-05-30 10:06:22.000000 metasynth-0.3.0/metasynth/privacy.py
--rw-r--r--   0 runner    (1001) docker     (123)    13495 2023-05-30 10:06:22.000000 metasynth-0.3.0/metasynth/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 10:06:22.000000 metasynth-0.3.0/metasynth/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:06:34.421552 metasynth-0.3.0/metasynth/schema/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-30 10:06:22.000000 metasynth-0.3.0/metasynth/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10418 2023-05-30 10:06:22.000000 metasynth-0.3.0/metasynth/schema/generative_metadata_format.json
--rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-05-30 10:06:22.000000 metasynth-0.3.0/metasynth/testutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-05-30 10:06:22.000000 metasynth-0.3.0/metasynth/validation.py
--rw-r--r--   0 runner    (1001) docker     (123)    10119 2023-05-30 10:06:22.000000 metasynth-0.3.0/metasynth/var.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:06:34.421552 metasynth-0.3.0/metasynth.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6154 2023-05-30 10:06:34.000000 metasynth-0.3.0/metasynth.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-05-30 10:06:34.000000 metasynth-0.3.0/metasynth.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 10:06:34.000000 metasynth-0.3.0/metasynth.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-30 10:06:34.000000 metasynth-0.3.0/metasynth.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-30 10:06:34.000000 metasynth-0.3.0/metasynth.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-30 10:06:34.000000 metasynth-0.3.0/metasynth.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-05-30 10:06:22.000000 metasynth-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 10:06:34.425552 metasynth-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:06:34.421552 metasynth-0.3.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:06:34.421552 metasynth-0.3.0/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)    60302 2023-05-30 10:06:22.000000 metasynth-0.3.0/tests/data/titanic.csv
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-05-30 10:06:22.000000 metasynth-0.3.0/tests/test_builtin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-05-30 10:06:22.000000 metasynth-0.3.0/tests/test_continuous.py
--rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-05-30 10:06:22.000000 metasynth-0.3.0/tests/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3361 2023-05-30 10:06:22.000000 metasynth-0.3.0/tests/test_datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-05-30 10:06:22.000000 metasynth-0.3.0/tests/test_discrete.py
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-05-30 10:06:22.000000 metasynth-0.3.0/tests/test_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-30 10:06:22.000000 metasynth-0.3.0/tests/test_faker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-05-30 10:06:22.000000 metasynth-0.3.0/tests/test_regex.py
--rw-r--r--   0 runner    (1001) docker     (123)     8300 2023-05-30 10:06:22.000000 metasynth-0.3.0/tests/test_var.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 17:09:59.663968 metasynth-0.4.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 17:09:59.651968 metasynth-0.4.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 17:09:59.651968 metasynth-0.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-08-04 17:09:46.000000 metasynth-0.4.0/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-08-04 17:09:46.000000 metasynth-0.4.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-08-04 17:09:46.000000 metasynth-0.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-08-04 17:09:46.000000 metasynth-0.4.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-08-04 17:09:46.000000 metasynth-0.4.0/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-08-04 17:09:46.000000 metasynth-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13844 2023-08-04 17:09:59.663968 metasynth-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11720 2023-08-04 17:09:46.000000 metasynth-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 17:09:59.651968 metasynth-0.4.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-08-04 17:09:46.000000 metasynth-0.4.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-08-04 17:09:46.000000 metasynth-0.4.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-08-04 17:09:46.000000 metasynth-0.4.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 17:09:59.651968 metasynth-0.4.0/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 17:09:59.651968 metasynth-0.4.0/docs/source/about/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-08-04 17:09:46.000000 metasynth-0.4.0/docs/source/about/about.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-08-04 17:09:46.000000 metasynth-0.4.0/docs/source/about/contact.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-08-04 17:09:46.000000 metasynth-0.4.0/docs/source/about/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-08-04 17:09:46.000000 metasynth-0.4.0/docs/source/about/what_is.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 17:09:59.655968 metasynth-0.4.0/docs/source/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-08-04 17:09:46.000000 metasynth-0.4.0/docs/source/api/metasynth.distribution.regex.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-08-04 17:09:46.000000 metasynth-0.4.0/docs/source/api/metasynth.distribution.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-08-04 17:09:46.000000 metasynth-0.4.0/docs/source/api/metasynth.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-08-04 17:09:46.000000 metasynth-0.4.0/docs/source/api/metasynth.schema.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-08-04 17:09:46.000000 metasynth-0.4.0/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 17:09:59.655968 metasynth-0.4.0/docs/source/developer/
+-rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-08-04 17:09:46.000000 metasynth-0.4.0/docs/source/developer/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7020 2023-08-04 17:09:46.000000 metasynth-0.4.0/docs/source/developer/detailed_overview.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-08-04 17:09:46.000000 metasynth-0.4.0/docs/source/developer/developer.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-08-04 17:09:46.000000 metasynth-0.4.0/docs/source/faq.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 17:09:59.655968 metasynth-0.4.0/docs/source/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    53165 2023-08-04 17:09:46.000000 metasynth-0.4.0/docs/source/images/flow_metadata_generation.png
+-rw-r--r--   0 runner    (1001) docker     (123)    59443 2023-08-04 17:09:46.000000 metasynth-0.4.0/docs/source/images/flow_metadata_generation_code.png
+-rw-r--r--   0 runner    (1001) docker     (123)    56147 2023-08-04 17:09:46.000000 metasynth-0.4.0/docs/source/images/flow_synthetic_data_generation.png
+-rw-r--r--   0 runner    (1001) docker     (123)    60571 2023-08-04 17:09:46.000000 metasynth-0.4.0/docs/source/images/flow_synthetic_data_generation_code.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 17:09:59.655968 metasynth-0.4.0/docs/source/images/logos/
+-rw-r--r--   0 runner    (1001) docker     (123)    88176 2023-08-04 17:09:46.000000 metasynth-0.4.0/docs/source/images/logos/blue.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   113476 2023-08-04 17:09:46.000000 metasynth-0.4.0/docs/source/images/logos/blue_large.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    51542 2023-08-04 17:09:46.000000 metasynth-0.4.0/docs/source/images/logos/blue_med.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    75402 2023-08-04 17:09:46.000000 metasynth-0.4.0/docs/source/images/logos/grey.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     7898 2023-08-04 17:09:46.000000 metasynth-0.4.0/docs/source/images/logos/grey.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    29156 2023-08-04 17:09:46.000000 metasynth-0.4.0/docs/source/images/logos/grey_med.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    85618 2023-08-04 17:09:46.000000 metasynth-0.4.0/docs/source/images/logos/soda.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7893 2023-08-04 17:09:46.000000 metasynth-0.4.0/docs/source/images/logos/white.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    21471 2023-08-04 17:09:46.000000 metasynth-0.4.0/docs/source/images/logos/white_med.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-08-04 17:09:46.000000 metasynth-0.4.0/docs/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 17:09:59.655968 metasynth-0.4.0/docs/source/usage/
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-08-04 17:09:46.000000 metasynth-0.4.0/docs/source/usage/extensions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6136 2023-08-04 17:09:46.000000 metasynth-0.4.0/docs/source/usage/generating_metadata.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-08-04 17:09:46.000000 metasynth-0.4.0/docs/source/usage/generating_synthetic_data.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-08-04 17:09:46.000000 metasynth-0.4.0/docs/source/usage/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-08-04 17:09:46.000000 metasynth-0.4.0/docs/source/usage/interactive_tutorials.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-08-04 17:09:46.000000 metasynth-0.4.0/docs/source/usage/quick_start.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-08-04 17:09:46.000000 metasynth-0.4.0/docs/source/usage/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 17:09:59.659968 metasynth-0.4.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)    60353 2023-08-04 17:09:46.000000 metasynth-0.4.0/examples/advanced_tutorial.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-08-04 17:09:46.000000 metasynth-0.4.0/examples/basic_example.json
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-08-04 17:09:46.000000 metasynth-0.4.0/examples/basic_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81698 2023-08-04 17:09:46.000000 metasynth-0.4.0/examples/demonstration.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    12704 2023-08-04 17:09:46.000000 metasynth-0.4.0/examples/descriptions.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     7713 2023-08-04 17:09:46.000000 metasynth-0.4.0/examples/getting_started.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    37457 2023-08-04 17:09:46.000000 metasynth-0.4.0/examples/titanic.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     6863 2023-08-04 17:09:46.000000 metasynth-0.4.0/examples/titanic_example.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-08-04 17:09:46.000000 metasynth-0.4.0/examples/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 17:09:59.659968 metasynth-0.4.0/metasynth/
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-08-04 17:09:46.000000 metasynth-0.4.0/metasynth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-08-04 17:09:59.000000 metasynth-0.4.0/metasynth/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10457 2023-08-04 17:09:46.000000 metasynth-0.4.0/metasynth/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 17:09:59.659968 metasynth-0.4.0/metasynth/demo/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-04 17:09:46.000000 metasynth-0.4.0/metasynth/demo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-08-04 17:09:46.000000 metasynth-0.4.0/metasynth/demo/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81698 2023-08-04 17:09:46.000000 metasynth-0.4.0/metasynth/demo/demo_titanic.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 17:09:59.659968 metasynth-0.4.0/metasynth/distribution/
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-08-04 17:09:46.000000 metasynth-0.4.0/metasynth/distribution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7878 2023-08-04 17:09:46.000000 metasynth-0.4.0/metasynth/distribution/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-08-04 17:09:46.000000 metasynth-0.4.0/metasynth/distribution/categorical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6732 2023-08-04 17:09:46.000000 metasynth-0.4.0/metasynth/distribution/continuous.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-08-04 17:09:46.000000 metasynth-0.4.0/metasynth/distribution/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-08-04 17:09:46.000000 metasynth-0.4.0/metasynth/distribution/discrete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-08-04 17:09:46.000000 metasynth-0.4.0/metasynth/distribution/faker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-08-04 17:09:46.000000 metasynth-0.4.0/metasynth/distribution/na.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 17:09:59.663968 metasynth-0.4.0/metasynth/distribution/regex/
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-08-04 17:09:46.000000 metasynth-0.4.0/metasynth/distribution/regex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7869 2023-08-04 17:09:46.000000 metasynth-0.4.0/metasynth/distribution/regex/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17577 2023-08-04 17:09:46.000000 metasynth-0.4.0/metasynth/distribution/regex/element.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11484 2023-08-04 17:09:46.000000 metasynth-0.4.0/metasynth/distribution/regex/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-08-04 17:09:46.000000 metasynth-0.4.0/metasynth/privacy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13802 2023-08-04 17:09:46.000000 metasynth-0.4.0/metasynth/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 17:09:46.000000 metasynth-0.4.0/metasynth/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 17:09:59.663968 metasynth-0.4.0/metasynth/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-08-04 17:09:46.000000 metasynth-0.4.0/metasynth/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10418 2023-08-04 17:09:46.000000 metasynth-0.4.0/metasynth/schema/generative_metadata_format.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-08-04 17:09:46.000000 metasynth-0.4.0/metasynth/testutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-08-04 17:09:46.000000 metasynth-0.4.0/metasynth/validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10899 2023-08-04 17:09:46.000000 metasynth-0.4.0/metasynth/var.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 17:09:59.659968 metasynth-0.4.0/metasynth.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13844 2023-08-04 17:09:59.000000 metasynth-0.4.0/metasynth.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-08-04 17:09:59.000000 metasynth-0.4.0/metasynth.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 17:09:59.000000 metasynth-0.4.0/metasynth.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-08-04 17:09:59.000000 metasynth-0.4.0/metasynth.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-08-04 17:09:59.000000 metasynth-0.4.0/metasynth.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-04 17:09:59.000000 metasynth-0.4.0/metasynth.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-08-04 17:09:46.000000 metasynth-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 17:09:59.663968 metasynth-0.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 17:09:59.663968 metasynth-0.4.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 17:09:59.663968 metasynth-0.4.0/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    60302 2023-08-04 17:09:46.000000 metasynth-0.4.0/tests/data/titanic.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-08-04 17:09:46.000000 metasynth-0.4.0/tests/test_builtin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-08-04 17:09:46.000000 metasynth-0.4.0/tests/test_continuous.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-08-04 17:09:46.000000 metasynth-0.4.0/tests/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3361 2023-08-04 17:09:46.000000 metasynth-0.4.0/tests/test_datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-08-04 17:09:46.000000 metasynth-0.4.0/tests/test_discrete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-08-04 17:09:46.000000 metasynth-0.4.0/tests/test_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-08-04 17:09:46.000000 metasynth-0.4.0/tests/test_faker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-08-04 17:09:46.000000 metasynth-0.4.0/tests/test_na.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-08-04 17:09:46.000000 metasynth-0.4.0/tests/test_regex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8562 2023-08-04 17:09:46.000000 metasynth-0.4.0/tests/test_var.py
```

### Comparing `metasynth-0.3.0/.github/workflows/python-package.yml` & `metasynth-0.4.0/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `metasynth-0.3.0/.github/workflows/python-publish.yml` & `metasynth-0.4.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `metasynth-0.3.0/.gitignore` & `metasynth-0.4.0/.gitignore`

 * *Files 4% similar despite different names*

```diff
@@ -133,7 +133,12 @@
 dmypy.json
 
 # Pyre type checker
 .pyre/
 
 # pycharm
 .idea/
+.vscode/
+
+#DS_Store
+.DS_Store
+.DS_Store
```

### Comparing `metasynth-0.3.0/.readthedocs.yaml` & `metasynth-0.4.0/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `metasynth-0.3.0/LICENSE` & `metasynth-0.4.0/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 SoDa
+Copyright (c) 2023 SoDa
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `metasynth-0.3.0/docs/Makefile` & `metasynth-0.4.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `metasynth-0.3.0/docs/make.bat` & `metasynth-0.4.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `metasynth-0.3.0/docs/soda.png` & `metasynth-0.4.0/docs/source/images/logos/soda.png`

 * *Files identical despite different names*

### Comparing `metasynth-0.3.0/docs/source/api/metasynth.distribution.regex.rst` & `metasynth-0.4.0/docs/source/api/metasynth.distribution.regex.rst`

 * *Files identical despite different names*

### Comparing `metasynth-0.3.0/docs/source/api/metasynth.distribution.rst` & `metasynth-0.4.0/docs/source/api/metasynth.distribution.rst`

 * *Files identical despite different names*

### Comparing `metasynth-0.3.0/docs/source/api/metasynth.rst` & `metasynth-0.4.0/docs/source/api/metasynth.rst`

 * *Files identical despite different names*

### Comparing `metasynth-0.3.0/docs/source/conf.py` & `metasynth-0.4.0/docs/source/conf.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,28 +15,29 @@
 import sphinx_rtd_theme
 sys.path.insert(0, os.path.abspath('..'))
 
 
 # -- Project information -----------------------------------------------------
 
 project = 'MetaSynth'
-copyright = '2022, SODA Team'
+copyright = '2023, SODA Team'
 author = 'SODA Team'
 
+
 # The full version, including alpha/beta/rc tags
-release = '0.1'
+release = '0.3'
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = ['sphinx.ext.napoleon', "sphinx.ext.autodoc", "sphinx_autodoc_typehints",
-              'sphinx_rtd_theme']
+              'sphinx_rtd_theme', "sphinx_inline_tabs", "sphinx_copybutton"]
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ['_templates']
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This pattern also affects html_static_path and html_extra_path.
@@ -45,13 +46,17 @@
 
 # -- Options for HTML output -------------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 #
 html_theme = 'sphinx_rtd_theme'
+html_logo = 'images/logos/white_med.png'
+html_theme_options = {
+    'logo_only': True, 
+}
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
 # html_static_path = ['_static']
 napoleon_use_param = True
```

### Comparing `metasynth-0.3.0/docs/source/developer.rst` & `metasynth-0.4.0/docs/source/developer/detailed_overview.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-Developer's Guide
+Detailed Overview
 =================
 
-This guide is mainly directed at developers working on the MetaSynth package, but it may be useful for users that want
-more control over the workings of the MetaSynth package.
+This page features a detailed overview of MetaSynth's modules, with the goal of helping developers get started developing for MetaSynth.
 
 MetaSynth File
 --------------
 
 The core of the MetaSynth is the MetaSynth Dataset Format. This is a file in with the JSON format, that describes a *dataset*.
 It includes on the base level:
 
@@ -27,50 +26,49 @@
 
 * ``name``: Name of the distribution.
 * ``parameters``: Dictionary containing the parameters of the distribution.
 
 The full schema that describes the structure of this file is included in the
 `GitHub repository <https://github.com/sodascience/meta-synth/blob/main/metasynth/schema/metasynth-1_0.json>`_.
 
-MetaDataSet
------------
+MetaFrame
+---------
 
 The main datastructure that the user will interface with. It contains exactly the information of the MetaSynth File. The main
-initialization methods are the classmethods :meth:`metasynth.dataset.MetaDataset.from_json` (to load from a file) and 
-:meth:`metasynth.dataset.MetaDataset.from_dataframe` to fit variables from a
+initialization methods are the classmethods :meth:`metasynth.dataset.MetaFrame.from_json` (to load from a file) and 
+:meth:`metasynth.dataset.MetaFrame.from_dataframe` to fit variables from a
 polars DataFrame. It implements ``__getitem__`` so that access to variables is easier, either by variable name or index.
 
-The last important method is :meth:`metasynth.dataset.MetaDataset.synthesize`, which creates a synthesized dataset.
+The last important method is :meth:`metasynth.dataset.MetaFrame.synthesize`, which creates a synthesized dataset.
 
 MetaVar
 -------
 
-This is the variable level building block for the MetaDataset. It contains the methods to convert a polars `Series` into a 
+This is the variable level building block for the MetaFrame. It contains the methods to convert a polars `Series` into a 
 variable with an appropriate distribution.
 
 The variable can be manually created with direct initialization, but usually it is easier to use the
 :meth:`metasynth.var.MetaVar.detect` method. This method does not fit any distribution, but it does infer the correct types for
 the MetaVar and saves the `Series` for later fitting.
 
 Next is the :meth:`metasynth.var.MetaVar.fit` method that actually fits a distribution to the data. Here you can again set the
 distribution, privacy package and uniqueness for the variable.
 
 Lastly, there is the :meth:`metasynth.var.MetaVar.draw_series` method that synthesizes a new series. For this to work,
 the variable has to be fitted of course.
 
-As can be inferred from the previous methods, the `MetaVar` class is to the `MetaDataset` what a polars `Series` is to a
+As can be inferred from the previous methods, the `MetaVar` class is to the `MetaFrame` what a polars `Series` is to a
 `DataFrame`.
 
 MetaDistribution
 ----------------
 
 This class will likely be removed at some point due to a lack of functionality. Only the fit function is currently used by
 `MetaVar`. It should be either be removed or added to a new `DistributionTree` class.
 
-
 Distributions
 -------------
 
 All distribution code can be found in `metasynth.distribution`. The distributions are somewhat ordered by variable type.
 
 BaseDistribution
 ~~~~~~~~~~~~~~~~
```

### Comparing `metasynth-0.3.0/docs/source/quick_start.rst` & `metasynth-0.4.0/docs/source/usage/quick_start.rst`

 * *Files 25% similar despite different names*

```diff
@@ -1,110 +1,103 @@
 Quick start guide
 =================
 
-The MetaSynth package contains two discrete functionalities: creating a statistical metadata file (smf) from tabular data,
-and a synthetic data generator. On this page you should be able to:
+Get started quickly with MetaSynth using the following example. In this concise demonstration, you'll learn the basic functionality of MetaSynth by generating synthetic data from `titanic <https://raw.githubusercontent.com/pandas-dev/pandas/main/doc/data/titanic.csv>`_ dataset.
 
-- Install the package
-- Prepare your data
-- Create an smf file
-- Read the smf file and create a synthetic dataset.
+.. note:: 
+   The steps on this page correspond to the basic tutorial available on the :doc:`/usage/interactive_tutorials` page. As such, if you prefer an interactive experience, check out the basic tutorial for a guided walkthrough!
 
-Installing MetaSynth
---------------------
+Importing Libraries
+-------------------
 
-First you need to create a working Python installation, with a version above or equal to Python 3.7.
-If you're not familiar with Python and have never installed it you can use the following
-`guide <https://docs.python-guide.org/starting/installation/>`_.
+The first step in any Python project is to import the necessary libraries. For this example, we will need Polars and MetaSynth.
 
-For the first official release of MetaSynth, it will be installable directly from `PyPi <https://pypi.org/>`_.
-For now, the MetaSynth package can be installed using the following command in the console:
 
+.. code:: python
 
-.. code-block:: console
+   import polars as pl
+   from metasynth import MetaFrame, demo_file
 
-	pip install git+https://github.com/sodascience/meta-synth.git
 
-To test the successful installation of MetaSynth, type the following in a python console and it should not give
-any errors:
+Loading the Dataset
+-------------------
+
+Next, load the Titanic CSV file, for this we can use the built-in :meth:`metasynth.demo_file` function.
 
 .. code-block:: python
 
-	import metasynth
+   dataset_csv = demo_file() 
 
+Then, we create a dictionary with information on the data types of the various columns/variables. This will be used in the next step, when we convert the CSV file to a DataFrame.
 
-Preparing the data
-------------------
+.. code-block:: python
 
-To prepare the data for usage with MetaSynth, it is useful to have some basic knowledge about 
-`polars <https://pola-rs.github.io/polars-book/user-guide/>`_. We use the
-`titanic <https://raw.githubusercontent.com/pandas-dev/pandas/main/doc/data/titanic.csv>`_ dataset
-to show the basic concepts here. To follow along, download the dataset to a folder and start Python
-in the same folder.
+   data_types = { 
+       "Sex": pl.Categorical,
+       "Embarked": pl.Categorical,
+       "Survived": pl.Categorical,
+       "Pclass": pl.Categorical,
+       "SibSp": pl.Categorical,
+       "Parch": pl.Categorical
+   }
 
-First read the csv file with polars:
+To finish loading the dataset, we simply use the :meth:`polars.read_csv` function, passing in our CSV file and dictionary as parameters. 
 
 .. code-block:: python
 
-	import polars as pl
-	
-	dtypes = {
-	    "Sex": pl.Categorical,
-	    "Embarked": pl.Categorical,
-	    "Survived": pl.Categorical,
-	    "Pclass": pl.Categorical,
-	    "SibSp": pl.Categorical,
-	    "Parch": pl.Categorical
-	}
-	df = pl.read_csv("titanic.csv", dtype=dtypes)
+   df = pl.read_csv(dataset_csv, dtypes=data_types)
 
-The dtypes argument is used to set the columns to their correct type. Only categorical variables
-need to be manually set. Dates, times and datetimes can be parsed by polars with the `parse_dates=True` keyword argument.
-There are seven differnt data types supported by MetaSynth: string, category, integer, float, date, time and datetime.
 
+This converts the CSV file into a DataFrame named ``df``.
 
-Create a statistical metadata file
-----------------------------------
+.. note:: 
+	In this example, we used a Polars DataFrame, but Pandas DataFrames are also supported by MetaSynth. 
 
-Currently, only the JSON file format is supported. First we need to create a MetaSynth dataset, which infers the
-distributions of the polars DataFrame:
 
-.. code-block:: python
+Generating the MetaFrame
+------------------------
+With the DataFrame loaded, you can now generate a :obj:`MetaFrame <metasynth.dataset.MetaFrame>`.
 
-	from metasynth import MetaDataset
 
-	dataset = MetaDataset.from_dataframe(df)
+.. code-block:: python
 
+   mf = MetaFrame.fit_dataframe(df)
 
-Internally, the dataset is simply a list of all the column variables, with their statistical properties. Next, write it
-to a JSON file:
+This creates a MetaFrame named ``mf``.
+
+.. Note:: 
+	At this point, you might get a warning about a potential unique variable, but we can ignore that for now as it's safe to continue.
+	
+	``Variable PassengerId seems unique, but not set to be unique. Set the variable to be either unique or not unique to remove this warning. warnings.warn(f"\nVariable {series.name} seems unique, but not set to be unique.\n"``
 
-.. code-block:: python
 
-	dataset.to_json("titanic.json")
+Saving and Loading the MetaFrame
+--------------------------------
 
-The file titanic.json should have a statistical metadata summary that can be used to generate synthetic data.
+The MetaFrame can be saved to a .JSON file for future use.
 
+.. code-block:: python
 
-Create a synthetic dataset
---------------------------
+   mf.to_json("exported_metaframe.json")
 
-To create the synthetic dataset we will first read the file (this is technically not necessary in this case):
+To load a saved MetaDataset, use the following code:
 
 .. code-block:: python
 
-	dataset = MetaDataset.from_json("titanic.json")
+   mf = MetaFrame.from_json("exported_metaframe.json")
 
+Synthesizing the Data
+---------------------
+
+With the :obj:`MetaFrame <metasynth.dataset.MetaFrame>` loaded, you can synthesize new data. To do so, we simply call the :meth:`metasynth.dataset.MetaFrame.synthesize` function on the :obj:`MetaFrame<metasynth.dataset.MetaFrame>`, and pass in the number of rows we'd like to generate as a parameter. Let's generate five rows of synthetic data.
 
-From the dataset it is easy to create a synthetic dataset with e.g. 100 rows:
 
 .. code-block:: python
 
-	synthetic_df = dataset.synthesize(100)
+   synthetic_data = mf.synthesize(5) 
+
 
+Conclusion
+----------
 
-More advanced uses of MetaSynth
--------------------------------
+Congratulations! You've successfully generated synthetic data using MetaSynth. The synthesized data is returned as a DataFrame, so you can inspect and manipulate it as you would with any DataFrame.
 
-A more advanced tutorial is available on our 
-`GitHub <https://github.com/sodascience/meta-synth/blob/main/examples/advanced tutorial.ipynb`>_
-page.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `metasynth-0.3.0/examples/advanced_tutorial.ipynb` & `metasynth-0.4.0/examples/advanced_tutorial.ipynb`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9989719575079665%*

 * *Differences: {"'cells'": "{2: {'source': {insert: [(3, 'from metasynth import MetaFrame, demo_file')], delete: "*

 * *            "[3]}}, 8: {'source': {insert: [(0, '## Step 2: Creating a MetaFrame object from a "*

 * *            "DataFrame\\n')], delete: [0]}}, 9: {'outputs': {0: {'text': {insert: [(0, "*

 * *            "'/Users/qubix/Documents/work/metasynth/metasynth/metasynth/provider.py:202: "*

 * *            "UserWarning: \\n')], delete: [0]}}}, 'source': ['meta_dataset = "*

 * *            "MetaFrame.fit_dataframe(df)']}, 11: {'outpu […]*

```diff
@@ -28,15 +28,15 @@
             "id": "2442cb34",
             "metadata": {},
             "outputs": [],
             "source": [
                 "# import required packages\n",
                 "import datetime as dt\n",
                 "import polars as pl\n",
-                "from metasynth import MetaDataset, demo_file"
+                "from metasynth import MetaFrame, demo_file"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "04466c26",
             "metadata": {},
             "source": [
@@ -147,39 +147,39 @@
             ]
         },
         {
             "cell_type": "markdown",
             "id": "13f849ed",
             "metadata": {},
             "source": [
-                "## Step 2: Creating a MetaDataset object from a DataFrame\n",
+                "## Step 2: Creating a MetaFrame object from a DataFrame\n",
                 "\n",
                 "Now a lot of work has already gone into creating a properly formatted dataframe. This work pays off at this stage: let's convert the DataFrame to a meta_dataset structure with the default options. Note: this takes a little bit of time!"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 5,
             "id": "e0c58473",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
-                        "/Users/qubix/Documents/work/metasynth/metasynth/metasynth/provider.py:199: UserWarning: \n",
+                        "/Users/qubix/Documents/work/metasynth/metasynth/metasynth/provider.py:202: UserWarning: \n",
                         "Variable PassengerId seems unique, but not set to be unique.\n",
                         "Set the variable to be either unique or not unique to remove this warning.\n",
                         "\n",
                         "  warnings.warn(f\"\\nVariable {series.name} seems unique, but not set to be unique.\\n\"\n"
                     ]
                 }
             ],
             "source": [
-                "meta_dataset = MetaDataset.from_dataframe(df)"
+                "meta_dataset = MetaFrame.fit_dataframe(df)"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "1e8a772d",
             "metadata": {},
             "source": [
@@ -217,15 +217,15 @@
                         "\n",
                         "{'name': 'Birthday', 'description': None, 'type': 'date', 'dtype': 'Date', 'prop_missing': 0.08754208754208755, 'distribution': \"{'implements': 'core.uniform_date', 'provenance': 'builtin', 'class_name': 'UniformDateDistribution', 'parameters': {'start': '1903-07-28', 'end': '1940-05-27'}}\"}\n",
                         "\n",
                         "{'name': 'Board time', 'description': None, 'type': 'time', 'dtype': 'Time', 'prop_missing': 0.08866442199775533, 'distribution': \"{'implements': 'core.uniform_time', 'provenance': 'builtin', 'class_name': 'UniformTimeDistribution', 'parameters': {'start': '10:39:40', 'end': '18:39:28', 'precision': 'seconds'}}\"}\n",
                         "\n",
                         "{'name': 'Married since', 'description': None, 'type': 'datetime', 'dtype': \"Datetime(time_unit='us', time_zone=None)\", 'prop_missing': 0.10325476992143659, 'distribution': \"{'implements': 'core.uniform_datetime', 'provenance': 'builtin', 'class_name': 'UniformDateTimeDistribution', 'parameters': {'start': '2022-07-15T12:21:15', 'end': '2022-08-15T10:32:05', 'precision': 'seconds'}}\"}\n",
                         "\n",
-                        "{'name': 'all_NA', 'description': None, 'type': 'string', 'dtype': 'Utf8', 'prop_missing': 1.0, 'distribution': '\\\\d{3,4}'}\n",
+                        "{'name': 'all_NA', 'description': None, 'type': 'string', 'dtype': 'Utf8', 'prop_missing': 1.0, 'distribution': \"{'implements': 'core.na', 'provenance': 'builtin', 'class_name': 'NADistribution', 'parameters': {}}\"}\n",
                         "\n"
                     ]
                 }
             ],
             "source": [
                 "print(meta_dataset)"
             ]
@@ -278,55 +278,60 @@
                         "text/html": [
                             "<div><style>\n",
                             ".dataframe > thead > tr > th,\n",
                             ".dataframe > tbody > tr > td {\n",
                             "  text-align: right;\n",
                             "}\n",
                             "</style>\n",
-                            "<small>shape: (5, 12)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>PassengerId</th><th>Name</th><th>Sex</th><th>Age</th><th>Parch</th><th>Fare</th><th>Cabin</th><th>Embarked</th><th>Birthday</th><th>Board time</th><th>Married since</th><th>all_NA</th></tr><tr><td>i64</td><td>str</td><td>cat</td><td>i64</td><td>i64</td><td>f64</td><td>f32</td><td>cat</td><td>date</td><td>time</td><td>datetime[\u03bcs]</td><td>f32</td></tr></thead><tbody><tr><td>238</td><td>&quot;$1H3mrvWcFvW&gt;4\u2026</td><td>&quot;female&quot;</td><td>67</td><td>1</td><td>30.093937</td><td>null</td><td>&quot;Q&quot;</td><td>1930-01-05</td><td>12:31:25</td><td>2022-08-15 01:35:55</td><td>null</td></tr><tr><td>808</td><td>&quot;puoj\u000b",
-                            "^?}u_);SQ\u2026</td><td>&quot;female&quot;</td><td>null</td><td>0</td><td>1.572982</td><td>null</td><td>&quot;S&quot;</td><td>1911-09-25</td><td>12:05:16</td><td>2022-07-24 14:20:05</td><td>null</td></tr><tr><td>571</td><td>&quot;eI+&gt;k\tI&#x27;S&lt;gs\r",
-                            "P\u2026</td><td>&quot;female&quot;</td><td>61</td><td>0</td><td>66.063047</td><td>null</td><td>&quot;S&quot;</td><td>1940-03-12</td><td>null</td><td>2022-08-10 02:14:20</td><td>null</td></tr><tr><td>53</td><td>&quot;\tk62+Ij*4hks%p\u2026</td><td>&quot;male&quot;</td><td>null</td><td>0</td><td>0.302661</td><td>null</td><td>&quot;C&quot;</td><td>1920-06-17</td><td>null</td><td>2022-07-17 16:29:17</td><td>null</td></tr><tr><td>833</td><td>&quot;hYcHE|hm,mQ.0S\u2026</td><td>&quot;female&quot;</td><td>35</td><td>1</td><td>20.32786</td><td>null</td><td>&quot;C&quot;</td><td>1933-02-26</td><td>11:54:27</td><td>2022-07-25 10:34:40</td><td>null</td></tr></tbody></table></div>"
+                            "<small>shape: (5, 12)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>PassengerId</th><th>Name</th><th>Sex</th><th>Age</th><th>Parch</th><th>Fare</th><th>Cabin</th><th>Embarked</th><th>Birthday</th><th>Board time</th><th>Married since</th><th>all_NA</th></tr><tr><td>i64</td><td>str</td><td>cat</td><td>i64</td><td>i64</td><td>f64</td><td>str</td><td>cat</td><td>date</td><td>time</td><td>datetime[\u03bcs]</td><td>f32</td></tr></thead><tbody><tr><td>214</td><td>&quot;9&quot;\n",
+                            "w])z0#XuNK8\u2026</td><td>&quot;male&quot;</td><td>19</td><td>0</td><td>19.020167</td><td>&quot;TLz~/=[4!Y/&quot;</td><td>&quot;S&quot;</td><td>1932-11-07</td><td>15:06:07</td><td>2022-07-27 11:20:49</td><td>null</td></tr><tr><td>679</td><td>&quot;-A@C&amp;s3kGrFlI&quot;</td><td>&quot;female&quot;</td><td>null</td><td>2</td><td>22.278076</td><td>null</td><td>&quot;S&quot;</td><td>1919-05-15</td><td>16:58:22</td><td>2022-07-25 23:06:38</td><td>null</td></tr><tr><td>21</td><td>&quot;\\OqxLpRUb`pb&amp;$\u2026</td><td>&quot;male&quot;</td><td>50</td><td>2</td><td>1.349379</td><td>&quot;D27W&quot;</td><td>&quot;S&quot;</td><td>1921-10-27</td><td>null</td><td>2022-08-09 01:03:33</td><td>null</td></tr><tr><td>107</td><td>&quot;tr:#\r",
+                            "NgUA,T\u000b",
+                            "xR\u2026</td><td>&quot;female&quot;</td><td>69</td><td>0</td><td>77.426879</td><td>&quot;G=Bs[\tV24]tqe#\u2026</td><td>&quot;S&quot;</td><td>1905-02-18</td><td>11:17:27</td><td>2022-07-16 01:45:17</td><td>null</td></tr><tr><td>515</td><td>&quot;q}L+3\r",
+                            "Q)1:C5D?\u2026</td><td>&quot;male&quot;</td><td>13</td><td>0</td><td>67.02794</td><td>null</td><td>&quot;S&quot;</td><td>1906-11-08</td><td>17:45:01</td><td>null</td><td>null</td></tr></tbody></table></div>"
                         ],
                         "text/plain": [
                             "shape: (5, 12)\n",
                             "\u250c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2510\n",
                             "\u2502 PassengerId \u2506 Name         \u2506 Sex    \u2506 Age  \u2506 \u2026 \u2506 Birthday   \u2506 Board time \u2506 Married      \u2506 all_NA \u2502\n",
                             "\u2502 ---         \u2506 ---          \u2506 ---    \u2506 ---  \u2506   \u2506 ---        \u2506 ---        \u2506 since        \u2506 ---    \u2502\n",
                             "\u2502 i64         \u2506 str          \u2506 cat    \u2506 i64  \u2506   \u2506 date       \u2506 time       \u2506 ---          \u2506 f32    \u2502\n",
                             "\u2502             \u2506              \u2506        \u2506      \u2506   \u2506            \u2506            \u2506 datetime[\u03bcs] \u2506        \u2502\n",
                             "\u255e\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2561\n",
-                            "\u2502 238         \u2506 $1H3mrvWcFvW \u2506 female \u2506 67   \u2506 \u2026 \u2506 1930-01-05 \u2506 12:31:25   \u2506 2022-08-15   \u2506 null   \u2502\n",
-                            "\u2502             \u2506 >4EW\\%b9[[#6 \u2506        \u2506      \u2506   \u2506            \u2506            \u2506 01:35:55     \u2506        \u2502\n",
-                            "\u2502             \u2506 Ix\n",
-                            "D:mmN\u2026     \u2506        \u2506      \u2506   \u2506            \u2506            \u2506              \u2506        \u2502\n",
-                            "\u2502 808         \u2506 puoj\n",
-                            "^?}u_);  \u2506 female \u2506 null \u2506 \u2026 \u2506 1911-09-25 \u2506 12:05:16   \u2506 2022-07-24   \u2506 null   \u2502\n",
-                            "\u2502             \u2506 SQ)DCN@)~cZ' \u2506        \u2506      \u2506   \u2506            \u2506            \u2506 14:20:05     \u2506        \u2502\n",
-                            "\u2502             \u2506 </^l\t=)'\u2026     \u2506        \u2506      \u2506   \u2506            \u2506            \u2506              \u2506        \u2502\n",
-                            "\u2502 571         \u2506 eI+>k\tI'S<gs  \u2506 female \u2506 61   \u2506 \u2026 \u2506 1940-03-12 \u2506 null       \u2506 2022-08-10   \u2506 null   \u2502\n",
+                            "\u2502 214         \u2506 9\"           \u2506 male   \u2506 19   \u2506 \u2026 \u2506 1932-11-07 \u2506 15:06:07   \u2506 2022-07-27   \u2506 null   \u2502\n",
+                            "\u2502             \u2506 w])z0#XuNK8\n",
+                            "  \u2506        \u2506      \u2506   \u2506            \u2506            \u2506 11:20:49     \u2506        \u2502\n",
+                            "\u2502             \u2506 r[fj\t>.Pc|    \u2506        \u2506      \u2506   \u2506            \u2506            \u2506              \u2506        \u2502\n",
                             "\u2502             \u2506 \n",
-                            "PjT          \u2506        \u2506      \u2506   \u2506            \u2506            \u2506 02:14:20     \u2506        \u2502\n",
-                            "\u2502             \u2506 z|pj         \u2506        \u2506      \u2506   \u2506            \u2506            \u2506              \u2506        \u2502\n",
-                            "\u2502 53          \u2506 \tk62+Ij*4hks  \u2506 male   \u2506 null \u2506 \u2026 \u2506 1920-06-17 \u2506 null       \u2506 2022-07-17   \u2506 null   \u2502\n",
-                            "\u2502             \u2506 %pB\n",
-                            "$J-,7gl`  \u2506        \u2506      \u2506   \u2506            \u2506            \u2506 16:29:17     \u2506        \u2502\n",
-                            "\u2502             \u2506 SW\n",
-                            "qEW~N\u2026     \u2506        \u2506      \u2506   \u2506            \u2506            \u2506              \u2506        \u2502\n",
-                            "\u2502 833         \u2506 hYcHE|hm,mQ. \u2506 female \u2506 35   \u2506 \u2026 \u2506 1933-02-26 \u2506 11:54:27   \u2506 2022-07-25   \u2506 null   \u2502\n",
-                            "\u2502             \u2506 0SCD\ta~t\tZIg%  \u2506        \u2506      \u2506   \u2506            \u2506            \u2506 10:34:40     \u2506        \u2502\n",
+                            "OL,^4\u2026       \u2506        \u2506      \u2506   \u2506            \u2506            \u2506              \u2506        \u2502\n",
+                            "\u2502 679         \u2506 -A@C&s3kGrFl \u2506 female \u2506 null \u2506 \u2026 \u2506 1919-05-15 \u2506 16:58:22   \u2506 2022-07-25   \u2506 null   \u2502\n",
+                            "\u2502             \u2506 I            \u2506        \u2506      \u2506   \u2506            \u2506            \u2506 23:06:38     \u2506        \u2502\n",
+                            "\u2502 21          \u2506 \\OqxLpRUb`pb \u2506 male   \u2506 50   \u2506 \u2026 \u2506 1921-10-27 \u2506 null       \u2506 2022-08-09   \u2506 null   \u2502\n",
+                            "\u2502             \u2506 &$&          \u2506        \u2506      \u2506   \u2506            \u2506            \u2506 01:03:33     \u2506        \u2502\n",
+                            "\u2502             \u2506 \n",
+                            "V=\"_BCP<hBq  \u2506        \u2506      \u2506   \u2506            \u2506            \u2506              \u2506        \u2502\n",
+                            "\u2502             \u2506 c8ry\u2026        \u2506        \u2506      \u2506   \u2506            \u2506            \u2506              \u2506        \u2502\n",
+                            "\u2502 107         \u2506 tr:#\n",
+                            "NgUA,T\n",
+                            "   \u2506 female \u2506 69   \u2506 \u2026 \u2506 1905-02-18 \u2506 11:17:27   \u2506 2022-07-16   \u2506 null   \u2502\n",
+                            "\u2502             \u2506 xR&)F4mi#al. \u2506        \u2506      \u2506   \u2506            \u2506            \u2506 01:45:17     \u2506        \u2502\n",
+                            "\u2502             \u2506 @U&5F]de\u2026    \u2506        \u2506      \u2506   \u2506            \u2506            \u2506              \u2506        \u2502\n",
+                            "\u2502 515         \u2506 q}L+3\n",
+                            "Q)1:C5  \u2506 male   \u2506 13   \u2506 \u2026 \u2506 1906-11-08 \u2506 17:45:01   \u2506 null         \u2506 null   \u2502\n",
+                            "\u2502             \u2506 D?&\"ecS.n`KD \u2506        \u2506      \u2506   \u2506            \u2506            \u2506              \u2506        \u2502\n",
+                            "\u2502             \u2506 twbrz\"%O\u2026    \u2506        \u2506      \u2506   \u2506            \u2506            \u2506              \u2506        \u2502\n",
                             "\u2514\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518"
                         ]
                     },
                     "execution_count": 8,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "new_meta_dataset = MetaDataset.from_json(file_path)\n",
+                "new_meta_dataset = MetaFrame.from_json(file_path)\n",
                 "new_meta_dataset.synthesize(5)"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "669b1e95",
             "metadata": {},
@@ -383,15 +388,15 @@
             "source": [
                 "# First, we create a specification dictionary for the variables\n",
                 "var_spec = {\n",
                 "    \"PassengerId\": {\"unique\": True}\n",
                 "}\n",
                 "\n",
                 "# then, we add that dictionary as the `spec` argument\n",
-                "meta_dataset = MetaDataset.from_dataframe(df, spec=var_spec)\n",
+                "meta_dataset = MetaFrame.fit_dataframe(df, spec=var_spec)\n",
                 "\n",
                 "# then, let's check what the metadata about PassengerId contains!\n",
                 "meta_dataset[\"PassengerId\"].to_dict()"
             ]
         },
         {
             "cell_type": "markdown",
@@ -412,45 +417,50 @@
                         "text/html": [
                             "<div><style>\n",
                             ".dataframe > thead > tr > th,\n",
                             ".dataframe > tbody > tr > td {\n",
                             "  text-align: right;\n",
                             "}\n",
                             "</style>\n",
-                            "<small>shape: (5, 12)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>PassengerId</th><th>Name</th><th>Sex</th><th>Age</th><th>Parch</th><th>Fare</th><th>Cabin</th><th>Embarked</th><th>Birthday</th><th>Board time</th><th>Married since</th><th>all_NA</th></tr><tr><td>i64</td><td>str</td><td>cat</td><td>i64</td><td>i64</td><td>f64</td><td>str</td><td>cat</td><td>date</td><td>time</td><td>datetime[\u03bcs]</td><td>f32</td></tr></thead><tbody><tr><td>1</td><td>&quot;y^dpnvg8&quot;XE(FP\u2026</td><td>&quot;male&quot;</td><td>24</td><td>0</td><td>16.383339</td><td>null</td><td>&quot;S&quot;</td><td>1914-11-20</td><td>15:48:40</td><td>2022-07-31 03:53:33</td><td>null</td></tr><tr><td>2</td><td>&quot;$L?0zKsN+C=&#x27;O4\u2026</td><td>&quot;male&quot;</td><td>36</td><td>1</td><td>28.624349</td><td>null</td><td>&quot;S&quot;</td><td>1924-12-02</td><td>12:36:07</td><td>2022-07-18 13:18:52</td><td>null</td></tr><tr><td>3</td><td>&quot;Odi0i*}C0m9)&lt;W\u2026</td><td>&quot;male&quot;</td><td>null</td><td>0</td><td>6.618381</td><td>null</td><td>&quot;C&quot;</td><td>null</td><td>null</td><td>2022-08-07 20:27:11</td><td>null</td></tr><tr><td>4</td><td>&quot;lX\t&lt;:voFlq]h@=\u2026</td><td>&quot;male&quot;</td><td>72</td><td>2</td><td>11.135868</td><td>null</td><td>&quot;S&quot;</td><td>1918-04-27</td><td>14:12:48</td><td>2022-08-02 16:28:51</td><td>null</td></tr><tr><td>5</td><td>&quot;uD\\,Cy#2pi\u000b",
-                            "rH3\u2026</td><td>&quot;male&quot;</td><td>62</td><td>1</td><td>141.462069</td><td>&quot;AeFX&quot;</td><td>&quot;S&quot;</td><td>1910-03-20</td><td>null</td><td>2022-08-10 18:31:35</td><td>null</td></tr></tbody></table></div>"
+                            "<small>shape: (5, 12)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>PassengerId</th><th>Name</th><th>Sex</th><th>Age</th><th>Parch</th><th>Fare</th><th>Cabin</th><th>Embarked</th><th>Birthday</th><th>Board time</th><th>Married since</th><th>all_NA</th></tr><tr><td>i64</td><td>str</td><td>cat</td><td>i64</td><td>i64</td><td>f64</td><td>str</td><td>cat</td><td>date</td><td>time</td><td>datetime[\u03bcs]</td><td>f32</td></tr></thead><tbody><tr><td>1</td><td>&quot;&amp;c{&amp;oVHiru-x_H\u2026</td><td>&quot;female&quot;</td><td>12</td><td>1</td><td>64.685147</td><td>&quot;AV0Hb,\f",
+                            "wo\u000b",
+                            "&quot;</td><td>&quot;C&quot;</td><td>1911-07-07</td><td>11:27:14</td><td>2022-07-29 07:59:06</td><td>null</td></tr><tr><td>2</td><td>&quot;,=x/6ly}&gt;d[ceK\u2026</td><td>&quot;female&quot;</td><td>22</td><td>0</td><td>11.644796</td><td>null</td><td>&quot;S&quot;</td><td>1928-09-20</td><td>17:17:14</td><td>2022-08-12 07:07:39</td><td>null</td></tr><tr><td>3</td><td>&quot;hfbf&#x27;Zc\tC$=:S[\u2026</td><td>&quot;male&quot;</td><td>30</td><td>0</td><td>1.893007</td><td>null</td><td>&quot;S&quot;</td><td>null</td><td>17:08:55</td><td>2022-08-03 22:43:55</td><td>null</td></tr><tr><td>4</td><td>&quot;qDjS6Y&gt;}kl6Z&#x27;\n",
+                            "\u2026</td><td>&quot;male&quot;</td><td>67</td><td>0</td><td>70.434857</td><td>null</td><td>&quot;S&quot;</td><td>1940-05-22</td><td>13:13:42</td><td>2022-08-05 10:39:48</td><td>null</td></tr><tr><td>5</td><td>&quot;/@@tvl#\u000b",
+                            "\u000b",
+                            "Wi\r",
+                            "q~\u2026</td><td>&quot;male&quot;</td><td>null</td><td>0</td><td>2.197158</td><td>null</td><td>&quot;C&quot;</td><td>null</td><td>17:33:28</td><td>2022-08-01 01:17:44</td><td>null</td></tr></tbody></table></div>"
                         ],
                         "text/plain": [
                             "shape: (5, 12)\n",
-                            "\u250c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2510\n",
-                            "\u2502 PassengerId \u2506 Name          \u2506 Sex  \u2506 Age  \u2506 \u2026 \u2506 Birthday   \u2506 Board time \u2506 Married since \u2506 all_NA \u2502\n",
-                            "\u2502 ---         \u2506 ---           \u2506 ---  \u2506 ---  \u2506   \u2506 ---        \u2506 ---        \u2506 ---           \u2506 ---    \u2502\n",
-                            "\u2502 i64         \u2506 str           \u2506 cat  \u2506 i64  \u2506   \u2506 date       \u2506 time       \u2506 datetime[\u03bcs]  \u2506 f32    \u2502\n",
-                            "\u255e\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2561\n",
-                            "\u2502 1           \u2506 y^dpnvg8\"XE(F \u2506 male \u2506 24   \u2506 \u2026 \u2506 1914-11-20 \u2506 15:48:40   \u2506 2022-07-31    \u2506 null   \u2502\n",
-                            "\u2502             \u2506 P]vd?0vl8IW5< \u2506      \u2506      \u2506   \u2506            \u2506            \u2506 03:53:33      \u2506        \u2502\n",
-                            "\u2502             \u2506 E^62|^\u2026       \u2506      \u2506      \u2506   \u2506            \u2506            \u2506               \u2506        \u2502\n",
-                            "\u2502 2           \u2506 $L?0zKsN+C='O \u2506 male \u2506 36   \u2506 \u2026 \u2506 1924-12-02 \u2506 12:36:07   \u2506 2022-07-18    \u2506 null   \u2502\n",
-                            "\u2502             \u2506 4\n",
-                            "Yv{c1FZL-Sg  \u2506      \u2506      \u2506   \u2506            \u2506            \u2506 13:18:52      \u2506        \u2502\n",
-                            "\u2502             \u2506 2R_d0d\u2026       \u2506      \u2506      \u2506   \u2506            \u2506            \u2506               \u2506        \u2502\n",
-                            "\u2502 3           \u2506 Odi0i*}C0m9)< \u2506 male \u2506 null \u2506 \u2026 \u2506 null       \u2506 null       \u2506 2022-08-07    \u2506 null   \u2502\n",
-                            "\u2502             \u2506 WBb>M+U9,1[I\n",
-                            "  \u2506      \u2506      \u2506   \u2506            \u2506            \u2506 20:27:11      \u2506        \u2502\n",
-                            "\u2502             \u2506 /&+           \u2506      \u2506      \u2506   \u2506            \u2506            \u2506               \u2506        \u2502\n",
-                            "\u2502 4           \u2506 lX\t<:voFlq]h@  \u2506 male \u2506 72   \u2506 \u2026 \u2506 1918-04-27 \u2506 14:12:48   \u2506 2022-08-02    \u2506 null   \u2502\n",
-                            "\u2502             \u2506 =(Zh\n",
-                            "U         \u2506      \u2506      \u2506   \u2506            \u2506            \u2506 16:28:51      \u2506        \u2502\n",
-                            "\u2502 5           \u2506 uD\\,Cy#2pi\n",
-                            "rH  \u2506 male \u2506 62   \u2506 \u2026 \u2506 1910-03-20 \u2506 null       \u2506 2022-08-10    \u2506 null   \u2502\n",
-                            "\u2502             \u2506 3wi=9}&G<nj<\n",
-                            "  \u2506      \u2506      \u2506   \u2506            \u2506            \u2506 18:31:35      \u2506        \u2502\n",
-                            "\u2502             \u2506 A.O\n",
-                            "4`\u2026        \u2506      \u2506      \u2506   \u2506            \u2506            \u2506               \u2506        \u2502\n",
-                            "\u2514\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518"
+                            "\u250c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2510\n",
+                            "\u2502 PassengerId \u2506 Name         \u2506 Sex    \u2506 Age  \u2506 \u2026 \u2506 Birthday   \u2506 Board time \u2506 Married      \u2506 all_NA \u2502\n",
+                            "\u2502 ---         \u2506 ---          \u2506 ---    \u2506 ---  \u2506   \u2506 ---        \u2506 ---        \u2506 since        \u2506 ---    \u2502\n",
+                            "\u2502 i64         \u2506 str          \u2506 cat    \u2506 i64  \u2506   \u2506 date       \u2506 time       \u2506 ---          \u2506 f32    \u2502\n",
+                            "\u2502             \u2506              \u2506        \u2506      \u2506   \u2506            \u2506            \u2506 datetime[\u03bcs] \u2506        \u2502\n",
+                            "\u255e\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2561\n",
+                            "\u2502 1           \u2506 &c{&oVHiru-x \u2506 female \u2506 12   \u2506 \u2026 \u2506 1911-07-07 \u2506 11:27:14   \u2506 2022-07-29   \u2506 null   \u2502\n",
+                            "\u2502             \u2506 _Hi8RwvD     \u2506        \u2506      \u2506   \u2506            \u2506            \u2506 07:59:06     \u2506        \u2502\n",
+                            "\u2502             \u2506 cu:fw2j9=X_\u2026 \u2506        \u2506      \u2506   \u2506            \u2506            \u2506              \u2506        \u2502\n",
+                            "\u2502 2           \u2506 ,=x/6ly}>d[c \u2506 female \u2506 22   \u2506 \u2026 \u2506 1928-09-20 \u2506 17:17:14   \u2506 2022-08-12   \u2506 null   \u2502\n",
+                            "\u2502             \u2506 eK^+U        \u2506        \u2506      \u2506   \u2506            \u2506            \u2506 07:07:39     \u2506        \u2502\n",
+                            "\u2502 3           \u2506 hfbf'Zc\tC$=:  \u2506 male   \u2506 30   \u2506 \u2026 \u2506 null       \u2506 17:08:55   \u2506 2022-08-03   \u2506 null   \u2502\n",
+                            "\u2502             \u2506 S[v          \u2506        \u2506      \u2506   \u2506            \u2506            \u2506 22:43:55     \u2506        \u2502\n",
+                            "\u2502 4           \u2506 qDjS6Y>}kl6Z \u2506 male   \u2506 67   \u2506 \u2026 \u2506 1940-05-22 \u2506 13:13:42   \u2506 2022-08-05   \u2506 null   \u2502\n",
+                            "\u2502             \u2506 '            \u2506        \u2506      \u2506   \u2506            \u2506            \u2506 10:39:48     \u2506        \u2502\n",
+                            "\u2502             \u2506 g@:p/y       \u2506        \u2506      \u2506   \u2506            \u2506            \u2506              \u2506        \u2502\n",
+                            "\u2502             \u2506 )#fz\n",
+                            ")wL7F+\u2026  \u2506        \u2506      \u2506   \u2506            \u2506            \u2506              \u2506        \u2502\n",
+                            "\u2502 5           \u2506 /@@tvl#\n",
+                            "\n",
+                            "Wi\n",
+                            "    \u2506 male   \u2506 null \u2506 \u2026 \u2506 null       \u2506 17:33:28   \u2506 2022-08-01   \u2506 null   \u2502\n",
+                            "\u2502             \u2506 q~m,E0e\n",
+                            "v8cl  \u2506        \u2506      \u2506   \u2506            \u2506            \u2506 01:17:44     \u2506        \u2502\n",
+                            "\u2502             \u2506 p@           \u2506        \u2506      \u2506   \u2506            \u2506            \u2506              \u2506        \u2502\n",
+                            "\u2514\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518"
                         ]
                     },
                     "execution_count": 10,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -489,34 +499,34 @@
                         "text/html": [
                             "<div><style>\n",
                             ".dataframe > thead > tr > th,\n",
                             ".dataframe > tbody > tr > td {\n",
                             "  text-align: right;\n",
                             "}\n",
                             "</style>\n",
-                            "<small>shape: (5, 12)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>PassengerId</th><th>Name</th><th>Sex</th><th>Age</th><th>Parch</th><th>Fare</th><th>Cabin</th><th>Embarked</th><th>Birthday</th><th>Board time</th><th>Married since</th><th>all_NA</th></tr><tr><td>i64</td><td>str</td><td>cat</td><td>i64</td><td>i64</td><td>f64</td><td>str</td><td>cat</td><td>date</td><td>time</td><td>datetime[\u03bcs]</td><td>f32</td></tr></thead><tbody><tr><td>1</td><td>&quot;Denise Smith&quot;</td><td>&quot;male&quot;</td><td>80</td><td>1</td><td>19.745816</td><td>null</td><td>&quot;C&quot;</td><td>1912-03-27</td><td>18:03:23</td><td>2022-07-29 03:11:55</td><td>null</td></tr><tr><td>2</td><td>&quot;Sarah James&quot;</td><td>&quot;female&quot;</td><td>57</td><td>0</td><td>14.240361</td><td>&quot;T|K&amp;k :QX&quot;</td><td>&quot;S&quot;</td><td>1918-02-22</td><td>13:18:24</td><td>2022-07-17 06:15:29</td><td>null</td></tr><tr><td>3</td><td>&quot;Thomas Oliver&quot;</td><td>&quot;male&quot;</td><td>70</td><td>0</td><td>23.827499</td><td>null</td><td>&quot;S&quot;</td><td>1904-05-07</td><td>13:24:53</td><td>null</td><td>null</td></tr><tr><td>4</td><td>&quot;Kimberly Randa\u2026</td><td>&quot;female&quot;</td><td>12</td><td>0</td><td>7.388182</td><td>null</td><td>&quot;C&quot;</td><td>1905-06-14</td><td>13:40:48</td><td>2022-07-19 18:44:26</td><td>null</td></tr><tr><td>5</td><td>&quot;Kathleen Reill\u2026</td><td>&quot;female&quot;</td><td>42</td><td>0</td><td>1.015004</td><td>null</td><td>&quot;C&quot;</td><td>1935-08-26</td><td>13:44:49</td><td>2022-08-13 14:59:58</td><td>null</td></tr></tbody></table></div>"
+                            "<small>shape: (5, 12)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>PassengerId</th><th>Name</th><th>Sex</th><th>Age</th><th>Parch</th><th>Fare</th><th>Cabin</th><th>Embarked</th><th>Birthday</th><th>Board time</th><th>Married since</th><th>all_NA</th></tr><tr><td>i64</td><td>str</td><td>cat</td><td>i64</td><td>i64</td><td>f64</td><td>str</td><td>cat</td><td>date</td><td>time</td><td>datetime[\u03bcs]</td><td>f32</td></tr></thead><tbody><tr><td>1</td><td>&quot;Carlos Kelly&quot;</td><td>&quot;male&quot;</td><td>null</td><td>0</td><td>36.098234</td><td>null</td><td>&quot;S&quot;</td><td>1920-01-16</td><td>15:11:33</td><td>2022-08-10 19:37:08</td><td>null</td></tr><tr><td>2</td><td>&quot;Tara Jackson&quot;</td><td>&quot;male&quot;</td><td>50</td><td>0</td><td>51.496397</td><td>null</td><td>&quot;S&quot;</td><td>1908-08-28</td><td>13:24:30</td><td>2022-08-11 21:29:41</td><td>null</td></tr><tr><td>3</td><td>&quot;John Hall&quot;</td><td>&quot;male&quot;</td><td>51</td><td>0</td><td>59.436604</td><td>null</td><td>&quot;S&quot;</td><td>1920-11-11</td><td>13:33:26</td><td>2022-08-05 11:51:47</td><td>null</td></tr><tr><td>4</td><td>&quot;Tina Coleman&quot;</td><td>&quot;male&quot;</td><td>42</td><td>0</td><td>35.83177</td><td>null</td><td>&quot;C&quot;</td><td>1940-02-22</td><td>12:11:58</td><td>2022-07-24 06:04:20</td><td>null</td></tr><tr><td>5</td><td>&quot;Erik Gentry&quot;</td><td>&quot;male&quot;</td><td>31</td><td>0</td><td>5.418221</td><td>&quot;T~[&lt;;&quot;</td><td>&quot;Q&quot;</td><td>1930-12-15</td><td>16:40:35</td><td>2022-08-01 23:17:03</td><td>null</td></tr></tbody></table></div>"
                         ],
                         "text/plain": [
                             "shape: (5, 12)\n",
-                            "\u250c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2510\n",
-                            "\u2502 PassengerId \u2506 Name          \u2506 Sex    \u2506 Age \u2506 \u2026 \u2506 Birthday   \u2506 Board time \u2506 Married      \u2506 all_NA \u2502\n",
-                            "\u2502 ---         \u2506 ---           \u2506 ---    \u2506 --- \u2506   \u2506 ---        \u2506 ---        \u2506 since        \u2506 ---    \u2502\n",
-                            "\u2502 i64         \u2506 str           \u2506 cat    \u2506 i64 \u2506   \u2506 date       \u2506 time       \u2506 ---          \u2506 f32    \u2502\n",
-                            "\u2502             \u2506               \u2506        \u2506     \u2506   \u2506            \u2506            \u2506 datetime[\u03bcs] \u2506        \u2502\n",
-                            "\u255e\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2561\n",
-                            "\u2502 1           \u2506 Denise Smith  \u2506 male   \u2506 80  \u2506 \u2026 \u2506 1912-03-27 \u2506 18:03:23   \u2506 2022-07-29   \u2506 null   \u2502\n",
-                            "\u2502             \u2506               \u2506        \u2506     \u2506   \u2506            \u2506            \u2506 03:11:55     \u2506        \u2502\n",
-                            "\u2502 2           \u2506 Sarah James   \u2506 female \u2506 57  \u2506 \u2026 \u2506 1918-02-22 \u2506 13:18:24   \u2506 2022-07-17   \u2506 null   \u2502\n",
-                            "\u2502             \u2506               \u2506        \u2506     \u2506   \u2506            \u2506            \u2506 06:15:29     \u2506        \u2502\n",
-                            "\u2502 3           \u2506 Thomas Oliver \u2506 male   \u2506 70  \u2506 \u2026 \u2506 1904-05-07 \u2506 13:24:53   \u2506 null         \u2506 null   \u2502\n",
-                            "\u2502 4           \u2506 Kimberly      \u2506 female \u2506 12  \u2506 \u2026 \u2506 1905-06-14 \u2506 13:40:48   \u2506 2022-07-19   \u2506 null   \u2502\n",
-                            "\u2502             \u2506 Randall       \u2506        \u2506     \u2506   \u2506            \u2506            \u2506 18:44:26     \u2506        \u2502\n",
-                            "\u2502 5           \u2506 Kathleen      \u2506 female \u2506 42  \u2506 \u2026 \u2506 1935-08-26 \u2506 13:44:49   \u2506 2022-08-13   \u2506 null   \u2502\n",
-                            "\u2502             \u2506 Reilly        \u2506        \u2506     \u2506   \u2506            \u2506            \u2506 14:59:58     \u2506        \u2502\n",
-                            "\u2514\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518"
+                            "\u250c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2510\n",
+                            "\u2502 PassengerId \u2506 Name         \u2506 Sex  \u2506 Age  \u2506 \u2026 \u2506 Birthday   \u2506 Board time \u2506 Married since  \u2506 all_NA \u2502\n",
+                            "\u2502 ---         \u2506 ---          \u2506 ---  \u2506 ---  \u2506   \u2506 ---        \u2506 ---        \u2506 ---            \u2506 ---    \u2502\n",
+                            "\u2502 i64         \u2506 str          \u2506 cat  \u2506 i64  \u2506   \u2506 date       \u2506 time       \u2506 datetime[\u03bcs]   \u2506 f32    \u2502\n",
+                            "\u255e\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2561\n",
+                            "\u2502 1           \u2506 Carlos Kelly \u2506 male \u2506 null \u2506 \u2026 \u2506 1920-01-16 \u2506 15:11:33   \u2506 2022-08-10     \u2506 null   \u2502\n",
+                            "\u2502             \u2506              \u2506      \u2506      \u2506   \u2506            \u2506            \u2506 19:37:08       \u2506        \u2502\n",
+                            "\u2502 2           \u2506 Tara Jackson \u2506 male \u2506 50   \u2506 \u2026 \u2506 1908-08-28 \u2506 13:24:30   \u2506 2022-08-11     \u2506 null   \u2502\n",
+                            "\u2502             \u2506              \u2506      \u2506      \u2506   \u2506            \u2506            \u2506 21:29:41       \u2506        \u2502\n",
+                            "\u2502 3           \u2506 John Hall    \u2506 male \u2506 51   \u2506 \u2026 \u2506 1920-11-11 \u2506 13:33:26   \u2506 2022-08-05     \u2506 null   \u2502\n",
+                            "\u2502             \u2506              \u2506      \u2506      \u2506   \u2506            \u2506            \u2506 11:51:47       \u2506        \u2502\n",
+                            "\u2502 4           \u2506 Tina Coleman \u2506 male \u2506 42   \u2506 \u2026 \u2506 1940-02-22 \u2506 12:11:58   \u2506 2022-07-24     \u2506 null   \u2502\n",
+                            "\u2502             \u2506              \u2506      \u2506      \u2506   \u2506            \u2506            \u2506 06:04:20       \u2506        \u2502\n",
+                            "\u2502 5           \u2506 Erik Gentry  \u2506 male \u2506 31   \u2506 \u2026 \u2506 1930-12-15 \u2506 16:40:35   \u2506 2022-08-01     \u2506 null   \u2502\n",
+                            "\u2502             \u2506              \u2506      \u2506      \u2506   \u2506            \u2506            \u2506 23:17:03       \u2506        \u2502\n",
+                            "\u2514\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518"
                         ]
                     },
                     "execution_count": 11,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -525,15 +535,15 @@
                 "from metasynth.distribution import FakerDistribution\n",
                 "\n",
                 "var_spec = {\n",
                 "    \"PassengerId\": {\"unique\": True}, \n",
                 "    \"Name\": {\"distribution\": FakerDistribution(\"name\")}\n",
                 "}\n",
                 "\n",
-                "meta_dataset = MetaDataset.from_dataframe(df, spec=var_spec)\n",
+                "meta_dataset = MetaFrame.fit_dataframe(df, spec=var_spec)\n",
                 "meta_dataset.synthesize(5)"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "de1fa66b",
             "metadata": {},
@@ -562,34 +572,34 @@
                         "text/html": [
                             "<div><style>\n",
                             ".dataframe > thead > tr > th,\n",
                             ".dataframe > tbody > tr > td {\n",
                             "  text-align: right;\n",
                             "}\n",
                             "</style>\n",
-                            "<small>shape: (5, 12)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>PassengerId</th><th>Name</th><th>Sex</th><th>Age</th><th>Parch</th><th>Fare</th><th>Cabin</th><th>Embarked</th><th>Birthday</th><th>Board time</th><th>Married since</th><th>all_NA</th></tr><tr><td>i64</td><td>str</td><td>cat</td><td>i64</td><td>i64</td><td>f64</td><td>str</td><td>cat</td><td>date</td><td>time</td><td>datetime[\u03bcs]</td><td>f32</td></tr></thead><tbody><tr><td>1</td><td>&quot;Denise Smith&quot;</td><td>&quot;male&quot;</td><td>33</td><td>0</td><td>0.188708</td><td>&quot;FS{P&quot;</td><td>&quot;S&quot;</td><td>1921-12-01</td><td>12:41:34</td><td>2022-07-16 12:17:32</td><td>null</td></tr><tr><td>2</td><td>&quot;Sarah James&quot;</td><td>&quot;male&quot;</td><td>25</td><td>0</td><td>0.459442</td><td>null</td><td>&quot;S&quot;</td><td>1929-08-06</td><td>15:34:47</td><td>2022-08-06 04:17:38</td><td>null</td></tr><tr><td>3</td><td>&quot;Thomas Oliver&quot;</td><td>&quot;male&quot;</td><td>34</td><td>0</td><td>7.043431</td><td>&quot;FA@e9]4F2J&#x27;&quot;</td><td>&quot;S&quot;</td><td>1929-07-26</td><td>13:24:31</td><td>2022-07-24 15:10:43</td><td>null</td></tr><tr><td>4</td><td>&quot;Kimberly Randa\u2026</td><td>&quot;male&quot;</td><td>27</td><td>0</td><td>0.682256</td><td>null</td><td>&quot;C&quot;</td><td>1912-10-05</td><td>15:12:25</td><td>2022-07-15 13:27:17</td><td>null</td></tr><tr><td>5</td><td>&quot;Kathleen Reill\u2026</td><td>&quot;male&quot;</td><td>28</td><td>0</td><td>0.256727</td><td>null</td><td>&quot;C&quot;</td><td>1930-08-14</td><td>12:38:52</td><td>2022-08-05 07:29:42</td><td>null</td></tr></tbody></table></div>"
+                            "<small>shape: (5, 12)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>PassengerId</th><th>Name</th><th>Sex</th><th>Age</th><th>Parch</th><th>Fare</th><th>Cabin</th><th>Embarked</th><th>Birthday</th><th>Board time</th><th>Married since</th><th>all_NA</th></tr><tr><td>i64</td><td>str</td><td>cat</td><td>i64</td><td>i64</td><td>f64</td><td>str</td><td>cat</td><td>date</td><td>time</td><td>datetime[\u03bcs]</td><td>f32</td></tr></thead><tbody><tr><td>1</td><td>&quot;Carlos Kelly&quot;</td><td>&quot;male&quot;</td><td>38</td><td>0</td><td>0.877191</td><td>null</td><td>&quot;S&quot;</td><td>1912-11-12</td><td>17:20:09</td><td>2022-08-12 22:25:55</td><td>null</td></tr><tr><td>2</td><td>&quot;Tara Jackson&quot;</td><td>&quot;male&quot;</td><td>31</td><td>0</td><td>4.810884</td><td>null</td><td>&quot;S&quot;</td><td>1912-08-27</td><td>17:55:01</td><td>2022-08-11 15:14:53</td><td>null</td></tr><tr><td>3</td><td>&quot;John Hall&quot;</td><td>&quot;male&quot;</td><td>null</td><td>0</td><td>4.352428</td><td>null</td><td>&quot;C&quot;</td><td>1932-07-13</td><td>11:00:45</td><td>2022-07-22 14:01:09</td><td>null</td></tr><tr><td>4</td><td>&quot;Tina Coleman&quot;</td><td>&quot;male&quot;</td><td>25</td><td>0</td><td>0.198071</td><td>&quot;T..}X7&quot;</td><td>&quot;S&quot;</td><td>1911-07-18</td><td>11:10:25</td><td>2022-07-27 17:43:37</td><td>null</td></tr><tr><td>5</td><td>&quot;Erik Gentry&quot;</td><td>&quot;male&quot;</td><td>21</td><td>1</td><td>0.560526</td><td>&quot;A1\\khuU5\\FDj&quot;</td><td>&quot;S&quot;</td><td>1934-04-16</td><td>10:51:19</td><td>2022-07-23 10:42:34</td><td>null</td></tr></tbody></table></div>"
                         ],
                         "text/plain": [
                             "shape: (5, 12)\n",
-                            "\u250c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2510\n",
-                            "\u2502 PassengerId \u2506 Name           \u2506 Sex  \u2506 Age \u2506 \u2026 \u2506 Birthday   \u2506 Board time \u2506 Married since \u2506 all_NA \u2502\n",
-                            "\u2502 ---         \u2506 ---            \u2506 ---  \u2506 --- \u2506   \u2506 ---        \u2506 ---        \u2506 ---           \u2506 ---    \u2502\n",
-                            "\u2502 i64         \u2506 str            \u2506 cat  \u2506 i64 \u2506   \u2506 date       \u2506 time       \u2506 datetime[\u03bcs]  \u2506 f32    \u2502\n",
-                            "\u255e\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2561\n",
-                            "\u2502 1           \u2506 Denise Smith   \u2506 male \u2506 33  \u2506 \u2026 \u2506 1921-12-01 \u2506 12:41:34   \u2506 2022-07-16    \u2506 null   \u2502\n",
-                            "\u2502             \u2506                \u2506      \u2506     \u2506   \u2506            \u2506            \u2506 12:17:32      \u2506        \u2502\n",
-                            "\u2502 2           \u2506 Sarah James    \u2506 male \u2506 25  \u2506 \u2026 \u2506 1929-08-06 \u2506 15:34:47   \u2506 2022-08-06    \u2506 null   \u2502\n",
-                            "\u2502             \u2506                \u2506      \u2506     \u2506   \u2506            \u2506            \u2506 04:17:38      \u2506        \u2502\n",
-                            "\u2502 3           \u2506 Thomas Oliver  \u2506 male \u2506 34  \u2506 \u2026 \u2506 1929-07-26 \u2506 13:24:31   \u2506 2022-07-24    \u2506 null   \u2502\n",
-                            "\u2502             \u2506                \u2506      \u2506     \u2506   \u2506            \u2506            \u2506 15:10:43      \u2506        \u2502\n",
-                            "\u2502 4           \u2506 Kimberly       \u2506 male \u2506 27  \u2506 \u2026 \u2506 1912-10-05 \u2506 15:12:25   \u2506 2022-07-15    \u2506 null   \u2502\n",
-                            "\u2502             \u2506 Randall        \u2506      \u2506     \u2506   \u2506            \u2506            \u2506 13:27:17      \u2506        \u2502\n",
-                            "\u2502 5           \u2506 Kathleen       \u2506 male \u2506 28  \u2506 \u2026 \u2506 1930-08-14 \u2506 12:38:52   \u2506 2022-08-05    \u2506 null   \u2502\n",
-                            "\u2502             \u2506 Reilly         \u2506      \u2506     \u2506   \u2506            \u2506            \u2506 07:29:42      \u2506        \u2502\n",
-                            "\u2514\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518"
+                            "\u250c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2510\n",
+                            "\u2502 PassengerId \u2506 Name         \u2506 Sex  \u2506 Age  \u2506 \u2026 \u2506 Birthday   \u2506 Board time \u2506 Married since  \u2506 all_NA \u2502\n",
+                            "\u2502 ---         \u2506 ---          \u2506 ---  \u2506 ---  \u2506   \u2506 ---        \u2506 ---        \u2506 ---            \u2506 ---    \u2502\n",
+                            "\u2502 i64         \u2506 str          \u2506 cat  \u2506 i64  \u2506   \u2506 date       \u2506 time       \u2506 datetime[\u03bcs]   \u2506 f32    \u2502\n",
+                            "\u255e\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2561\n",
+                            "\u2502 1           \u2506 Carlos Kelly \u2506 male \u2506 38   \u2506 \u2026 \u2506 1912-11-12 \u2506 17:20:09   \u2506 2022-08-12     \u2506 null   \u2502\n",
+                            "\u2502             \u2506              \u2506      \u2506      \u2506   \u2506            \u2506            \u2506 22:25:55       \u2506        \u2502\n",
+                            "\u2502 2           \u2506 Tara Jackson \u2506 male \u2506 31   \u2506 \u2026 \u2506 1912-08-27 \u2506 17:55:01   \u2506 2022-08-11     \u2506 null   \u2502\n",
+                            "\u2502             \u2506              \u2506      \u2506      \u2506   \u2506            \u2506            \u2506 15:14:53       \u2506        \u2502\n",
+                            "\u2502 3           \u2506 John Hall    \u2506 male \u2506 null \u2506 \u2026 \u2506 1932-07-13 \u2506 11:00:45   \u2506 2022-07-22     \u2506 null   \u2502\n",
+                            "\u2502             \u2506              \u2506      \u2506      \u2506   \u2506            \u2506            \u2506 14:01:09       \u2506        \u2502\n",
+                            "\u2502 4           \u2506 Tina Coleman \u2506 male \u2506 25   \u2506 \u2026 \u2506 1911-07-18 \u2506 11:10:25   \u2506 2022-07-27     \u2506 null   \u2502\n",
+                            "\u2502             \u2506              \u2506      \u2506      \u2506   \u2506            \u2506            \u2506 17:43:37       \u2506        \u2502\n",
+                            "\u2502 5           \u2506 Erik Gentry  \u2506 male \u2506 21   \u2506 \u2026 \u2506 1934-04-16 \u2506 10:51:19   \u2506 2022-07-23     \u2506 null   \u2502\n",
+                            "\u2502             \u2506              \u2506      \u2506      \u2506   \u2506            \u2506            \u2506 10:42:34       \u2506        \u2502\n",
+                            "\u2514\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518"
                         ]
                     },
                     "execution_count": 12,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -599,15 +609,15 @@
                 "var_spec = {\n",
                 "    \"PassengerId\": {\"unique\": True}, \n",
                 "    \"Name\": {\"distribution\": FakerDistribution(\"name\")},\n",
                 "    \"Fare\": {\"distribution\": \"LogNormalDistribution\"}, # estimate / fit an exponential distribution based on the data\n",
                 "    \"Age\": {\"distribution\": DiscreteUniformDistribution(20, 40)} # fully specify a distribution for age (uniform between 20 and 40)\n",
                 "}\n",
                 "\n",
-                "meta_dataset = MetaDataset.from_dataframe(df, spec=var_spec)\n",
+                "meta_dataset = MetaFrame.fit_dataframe(df, spec=var_spec)\n",
                 "meta_dataset.synthesize(5)"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "2897133c",
             "metadata": {},
@@ -628,41 +638,41 @@
                         "text/html": [
                             "<div><style>\n",
                             ".dataframe > thead > tr > th,\n",
                             ".dataframe > tbody > tr > td {\n",
                             "  text-align: right;\n",
                             "}\n",
                             "</style>\n",
-                            "<small>shape: (10, 12)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>PassengerId</th><th>Name</th><th>Sex</th><th>Age</th><th>Parch</th><th>Fare</th><th>Cabin</th><th>Embarked</th><th>Birthday</th><th>Board time</th><th>Married since</th><th>all_NA</th></tr><tr><td>i64</td><td>str</td><td>cat</td><td>i64</td><td>i64</td><td>f64</td><td>str</td><td>cat</td><td>date</td><td>time</td><td>datetime[\u03bcs]</td><td>f32</td></tr></thead><tbody><tr><td>1</td><td>&quot;Denise Smith&quot;</td><td>&quot;female&quot;</td><td>29</td><td>0</td><td>44.372505</td><td>null</td><td>&quot;S&quot;</td><td>1907-06-11</td><td>10:50:55</td><td>2022-07-22 19:35:36</td><td>null</td></tr><tr><td>2</td><td>&quot;Sarah James&quot;</td><td>&quot;male&quot;</td><td>24</td><td>0</td><td>35.821083</td><td>null</td><td>&quot;S&quot;</td><td>1918-01-28</td><td>13:07:14</td><td>2022-07-18 00:44:24</td><td>null</td></tr><tr><td>3</td><td>&quot;Thomas Oliver&quot;</td><td>&quot;female&quot;</td><td>21</td><td>0</td><td>60.5651</td><td>null</td><td>&quot;Q&quot;</td><td>1937-07-31</td><td>18:16:35</td><td>2022-07-21 15:15:27</td><td>null</td></tr><tr><td>4</td><td>&quot;Kimberly Randa\u2026</td><td>&quot;male&quot;</td><td>29</td><td>0</td><td>9.463605</td><td>null</td><td>&quot;S&quot;</td><td>1929-07-13</td><td>12:03:07</td><td>2022-07-26 16:50:49</td><td>null</td></tr><tr><td>5</td><td>&quot;Kathleen Reill\u2026</td><td>&quot;female&quot;</td><td>33</td><td>0</td><td>11.661819</td><td>null</td><td>&quot;C&quot;</td><td>1932-11-27</td><td>18:36:59</td><td>2022-08-01 02:39:56</td><td>null</td></tr><tr><td>6</td><td>&quot;James Sexton&quot;</td><td>&quot;male&quot;</td><td>23</td><td>1</td><td>5.705814</td><td>&quot;E108&quot;</td><td>&quot;C&quot;</td><td>1905-12-15</td><td>14:10:42</td><td>2022-07-19 16:26:28</td><td>null</td></tr><tr><td>7</td><td>&quot;Richard Smith&quot;</td><td>&quot;female&quot;</td><td>32</td><td>0</td><td>40.989583</td><td>null</td><td>&quot;S&quot;</td><td>1903-12-07</td><td>17:06:55</td><td>2022-07-19 14:33:52</td><td>null</td></tr><tr><td>8</td><td>&quot;Rachel Brooks&quot;</td><td>&quot;male&quot;</td><td>29</td><td>0</td><td>32.674552</td><td>&quot;D175&quot;</td><td>&quot;S&quot;</td><td>1903-08-05</td><td>12:39:56</td><td>2022-07-16 11:48:45</td><td>null</td></tr><tr><td>9</td><td>&quot;Diane Perry&quot;</td><td>&quot;male&quot;</td><td>34</td><td>1</td><td>55.406916</td><td>null</td><td>&quot;C&quot;</td><td>null</td><td>15:40:15</td><td>2022-07-26 18:17:59</td><td>null</td></tr><tr><td>10</td><td>&quot;Nicholas Conne\u2026</td><td>&quot;male&quot;</td><td>38</td><td>1</td><td>6.052691</td><td>null</td><td>&quot;S&quot;</td><td>1911-04-08</td><td>17:57:16</td><td>2022-07-28 22:00:21</td><td>null</td></tr></tbody></table></div>"
+                            "<small>shape: (10, 12)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>PassengerId</th><th>Name</th><th>Sex</th><th>Age</th><th>Parch</th><th>Fare</th><th>Cabin</th><th>Embarked</th><th>Birthday</th><th>Board time</th><th>Married since</th><th>all_NA</th></tr><tr><td>i64</td><td>str</td><td>cat</td><td>i64</td><td>i64</td><td>f64</td><td>str</td><td>cat</td><td>date</td><td>time</td><td>datetime[\u03bcs]</td><td>f32</td></tr></thead><tbody><tr><td>1</td><td>&quot;Carlos Kelly&quot;</td><td>&quot;female&quot;</td><td>29</td><td>0</td><td>11.779226</td><td>null</td><td>&quot;S&quot;</td><td>1905-06-15</td><td>15:52:19</td><td>2022-07-24 21:13:12</td><td>null</td></tr><tr><td>2</td><td>&quot;Tara Jackson&quot;</td><td>&quot;male&quot;</td><td>38</td><td>0</td><td>16.717372</td><td>&quot;F932&quot;</td><td>&quot;S&quot;</td><td>null</td><td>13:23:20</td><td>2022-08-12 03:33:40</td><td>null</td></tr><tr><td>3</td><td>&quot;John Hall&quot;</td><td>&quot;male&quot;</td><td>34</td><td>0</td><td>21.10042</td><td>null</td><td>&quot;S&quot;</td><td>1919-11-24</td><td>17:38:41</td><td>2022-08-07 15:14:21</td><td>null</td></tr><tr><td>4</td><td>&quot;Tina Coleman&quot;</td><td>&quot;male&quot;</td><td>33</td><td>0</td><td>38.372983</td><td>null</td><td>&quot;S&quot;</td><td>1938-09-24</td><td>12:35:36</td><td>2022-07-18 07:01:43</td><td>null</td></tr><tr><td>5</td><td>&quot;Erik Gentry&quot;</td><td>&quot;female&quot;</td><td>30</td><td>1</td><td>30.103301</td><td>null</td><td>&quot;S&quot;</td><td>1935-10-12</td><td>16:28:10</td><td>2022-08-09 14:26:30</td><td>null</td></tr><tr><td>6</td><td>&quot;William Davis&quot;</td><td>&quot;male&quot;</td><td>21</td><td>0</td><td>37.616158</td><td>null</td><td>&quot;S&quot;</td><td>1930-08-13</td><td>16:38:30</td><td>2022-08-12 12:41:44</td><td>null</td></tr><tr><td>7</td><td>&quot;Andrew Moreno&quot;</td><td>&quot;male&quot;</td><td>37</td><td>0</td><td>24.799106</td><td>null</td><td>&quot;S&quot;</td><td>1919-11-26</td><td>17:57:46</td><td>2022-07-17 23:24:14</td><td>null</td></tr><tr><td>8</td><td>&quot;Whitney Brown&quot;</td><td>&quot;male&quot;</td><td>34</td><td>0</td><td>22.466841</td><td>null</td><td>&quot;S&quot;</td><td>1919-07-10</td><td>11:40:18</td><td>2022-08-05 04:17:00</td><td>null</td></tr><tr><td>9</td><td>&quot;Jose Smith&quot;</td><td>&quot;male&quot;</td><td>38</td><td>0</td><td>5.049875</td><td>null</td><td>&quot;S&quot;</td><td>1933-03-06</td><td>16:53:17</td><td>2022-08-10 04:20:27</td><td>null</td></tr><tr><td>10</td><td>&quot;Yolanda Dunn&quot;</td><td>&quot;female&quot;</td><td>27</td><td>1</td><td>1.96723</td><td>null</td><td>&quot;S&quot;</td><td>1927-09-04</td><td>15:17:45</td><td>2022-08-13 23:51:02</td><td>null</td></tr></tbody></table></div>"
                         ],
                         "text/plain": [
                             "shape: (10, 12)\n",
                             "\u250c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2510\n",
                             "\u2502 PassengerId \u2506 Name          \u2506 Sex    \u2506 Age \u2506 \u2026 \u2506 Birthday   \u2506 Board time \u2506 Married      \u2506 all_NA \u2502\n",
                             "\u2502 ---         \u2506 ---           \u2506 ---    \u2506 --- \u2506   \u2506 ---        \u2506 ---        \u2506 since        \u2506 ---    \u2502\n",
                             "\u2502 i64         \u2506 str           \u2506 cat    \u2506 i64 \u2506   \u2506 date       \u2506 time       \u2506 ---          \u2506 f32    \u2502\n",
                             "\u2502             \u2506               \u2506        \u2506     \u2506   \u2506            \u2506            \u2506 datetime[\u03bcs] \u2506        \u2502\n",
                             "\u255e\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2561\n",
-                            "\u2502 1           \u2506 Denise Smith  \u2506 female \u2506 29  \u2506 \u2026 \u2506 1907-06-11 \u2506 10:50:55   \u2506 2022-07-22   \u2506 null   \u2502\n",
-                            "\u2502             \u2506               \u2506        \u2506     \u2506   \u2506            \u2506            \u2506 19:35:36     \u2506        \u2502\n",
-                            "\u2502 2           \u2506 Sarah James   \u2506 male   \u2506 24  \u2506 \u2026 \u2506 1918-01-28 \u2506 13:07:14   \u2506 2022-07-18   \u2506 null   \u2502\n",
-                            "\u2502             \u2506               \u2506        \u2506     \u2506   \u2506            \u2506            \u2506 00:44:24     \u2506        \u2502\n",
-                            "\u2502 3           \u2506 Thomas Oliver \u2506 female \u2506 21  \u2506 \u2026 \u2506 1937-07-31 \u2506 18:16:35   \u2506 2022-07-21   \u2506 null   \u2502\n",
-                            "\u2502             \u2506               \u2506        \u2506     \u2506   \u2506            \u2506            \u2506 15:15:27     \u2506        \u2502\n",
-                            "\u2502 4           \u2506 Kimberly      \u2506 male   \u2506 29  \u2506 \u2026 \u2506 1929-07-13 \u2506 12:03:07   \u2506 2022-07-26   \u2506 null   \u2502\n",
-                            "\u2502             \u2506 Randall       \u2506        \u2506     \u2506   \u2506            \u2506            \u2506 16:50:49     \u2506        \u2502\n",
+                            "\u2502 1           \u2506 Carlos Kelly  \u2506 female \u2506 29  \u2506 \u2026 \u2506 1905-06-15 \u2506 15:52:19   \u2506 2022-07-24   \u2506 null   \u2502\n",
+                            "\u2502             \u2506               \u2506        \u2506     \u2506   \u2506            \u2506            \u2506 21:13:12     \u2506        \u2502\n",
+                            "\u2502 2           \u2506 Tara Jackson  \u2506 male   \u2506 38  \u2506 \u2026 \u2506 null       \u2506 13:23:20   \u2506 2022-08-12   \u2506 null   \u2502\n",
+                            "\u2502             \u2506               \u2506        \u2506     \u2506   \u2506            \u2506            \u2506 03:33:40     \u2506        \u2502\n",
+                            "\u2502 3           \u2506 John Hall     \u2506 male   \u2506 34  \u2506 \u2026 \u2506 1919-11-24 \u2506 17:38:41   \u2506 2022-08-07   \u2506 null   \u2502\n",
+                            "\u2502             \u2506               \u2506        \u2506     \u2506   \u2506            \u2506            \u2506 15:14:21     \u2506        \u2502\n",
+                            "\u2502 4           \u2506 Tina Coleman  \u2506 male   \u2506 33  \u2506 \u2026 \u2506 1938-09-24 \u2506 12:35:36   \u2506 2022-07-18   \u2506 null   \u2502\n",
+                            "\u2502             \u2506               \u2506        \u2506     \u2506   \u2506            \u2506            \u2506 07:01:43     \u2506        \u2502\n",
                             "\u2502 \u2026           \u2506 \u2026             \u2506 \u2026      \u2506 \u2026   \u2506 \u2026 \u2506 \u2026          \u2506 \u2026          \u2506 \u2026            \u2506 \u2026      \u2502\n",
-                            "\u2502 7           \u2506 Richard Smith \u2506 female \u2506 32  \u2506 \u2026 \u2506 1903-12-07 \u2506 17:06:55   \u2506 2022-07-19   \u2506 null   \u2502\n",
-                            "\u2502             \u2506               \u2506        \u2506     \u2506   \u2506            \u2506            \u2506 14:33:52     \u2506        \u2502\n",
-                            "\u2502 8           \u2506 Rachel Brooks \u2506 male   \u2506 29  \u2506 \u2026 \u2506 1903-08-05 \u2506 12:39:56   \u2506 2022-07-16   \u2506 null   \u2502\n",
-                            "\u2502             \u2506               \u2506        \u2506     \u2506   \u2506            \u2506            \u2506 11:48:45     \u2506        \u2502\n",
-                            "\u2502 9           \u2506 Diane Perry   \u2506 male   \u2506 34  \u2506 \u2026 \u2506 null       \u2506 15:40:15   \u2506 2022-07-26   \u2506 null   \u2502\n",
-                            "\u2502             \u2506               \u2506        \u2506     \u2506   \u2506            \u2506            \u2506 18:17:59     \u2506        \u2502\n",
-                            "\u2502 10          \u2506 Nicholas      \u2506 male   \u2506 38  \u2506 \u2026 \u2506 1911-04-08 \u2506 17:57:16   \u2506 2022-07-28   \u2506 null   \u2502\n",
-                            "\u2502             \u2506 Conner        \u2506        \u2506     \u2506   \u2506            \u2506            \u2506 22:00:21     \u2506        \u2502\n",
+                            "\u2502 7           \u2506 Andrew Moreno \u2506 male   \u2506 37  \u2506 \u2026 \u2506 1919-11-26 \u2506 17:57:46   \u2506 2022-07-17   \u2506 null   \u2502\n",
+                            "\u2502             \u2506               \u2506        \u2506     \u2506   \u2506            \u2506            \u2506 23:24:14     \u2506        \u2502\n",
+                            "\u2502 8           \u2506 Whitney Brown \u2506 male   \u2506 34  \u2506 \u2026 \u2506 1919-07-10 \u2506 11:40:18   \u2506 2022-08-05   \u2506 null   \u2502\n",
+                            "\u2502             \u2506               \u2506        \u2506     \u2506   \u2506            \u2506            \u2506 04:17:00     \u2506        \u2502\n",
+                            "\u2502 9           \u2506 Jose Smith    \u2506 male   \u2506 38  \u2506 \u2026 \u2506 1933-03-06 \u2506 16:53:17   \u2506 2022-08-10   \u2506 null   \u2502\n",
+                            "\u2502             \u2506               \u2506        \u2506     \u2506   \u2506            \u2506            \u2506 04:20:27     \u2506        \u2502\n",
+                            "\u2502 10          \u2506 Yolanda Dunn  \u2506 female \u2506 27  \u2506 \u2026 \u2506 1927-09-04 \u2506 15:17:45   \u2506 2022-08-13   \u2506 null   \u2502\n",
+                            "\u2502             \u2506               \u2506        \u2506     \u2506   \u2506            \u2506            \u2506 23:51:02     \u2506        \u2502\n",
                             "\u2514\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518"
                         ]
                     },
                     "execution_count": 13,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
@@ -680,15 +690,15 @@
                 "    \"PassengerId\": {\"unique\": True}, \n",
                 "    \"Name\": {\"distribution\": FakerDistribution(\"name\")},\n",
                 "    \"Fare\": {\"distribution\": \"ExponentialDistribution\"}, # estimate / fit an exponential distribution based on the data\n",
                 "    \"Age\": {\"distribution\": DiscreteUniformDistribution(20, 40)}, # fully specify a distribution for age (uniform between 20 and 40)\n",
                 "    \"Cabin\": {\"distribution\": cabin_distribution}\n",
                 "}\n",
                 "\n",
-                "meta_dataset = MetaDataset.from_dataframe(df, spec=var_spec)\n",
+                "meta_dataset = MetaFrame.fit_dataframe(df, spec=var_spec)\n",
                 "meta_dataset.synthesize(10)"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "93499251",
             "metadata": {},
@@ -752,24 +762,24 @@
                         "text/html": [
                             "<div><style>\n",
                             ".dataframe > thead > tr > th,\n",
                             ".dataframe > tbody > tr > td {\n",
                             "  text-align: right;\n",
                             "}\n",
                             "</style>\n",
-                            "<small>shape: (1, 12)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>PassengerId</th><th>Name</th><th>Sex</th><th>Age</th><th>Parch</th><th>Fare</th><th>Cabin</th><th>Embarked</th><th>Birthday</th><th>Board time</th><th>Married since</th><th>all_NA</th></tr><tr><td>f64</td><td>str</td><td>cat</td><td>f64</td><td>f64</td><td>f64</td><td>str</td><td>cat</td><td>date</td><td>time</td><td>datetime[\u03bcs]</td><td>f32</td></tr></thead><tbody><tr><td>446.0</td><td>null</td><td>null</td><td>29.493075</td><td>0.42312</td><td>32.710142</td><td>null</td><td>null</td><td>null</td><td>null</td><td>null</td><td>null</td></tr></tbody></table></div>"
+                            "<small>shape: (1, 12)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>PassengerId</th><th>Name</th><th>Sex</th><th>Age</th><th>Parch</th><th>Fare</th><th>Cabin</th><th>Embarked</th><th>Birthday</th><th>Board time</th><th>Married since</th><th>all_NA</th></tr><tr><td>f64</td><td>str</td><td>cat</td><td>f64</td><td>f64</td><td>f64</td><td>str</td><td>cat</td><td>date</td><td>time</td><td>datetime[\u03bcs]</td><td>f32</td></tr></thead><tbody><tr><td>446.0</td><td>null</td><td>null</td><td>29.707042</td><td>0.379349</td><td>29.770945</td><td>null</td><td>null</td><td>null</td><td>null</td><td>null</td><td>null</td></tr></tbody></table></div>"
                         ],
                         "text/plain": [
                             "shape: (1, 12)\n",
                             "\u250c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2510\n",
                             "\u2502 PassengerId \u2506 Name \u2506 Sex  \u2506 Age       \u2506 \u2026 \u2506 Birthday \u2506 Board time \u2506 Married since \u2506 all_NA \u2502\n",
                             "\u2502 ---         \u2506 ---  \u2506 ---  \u2506 ---       \u2506   \u2506 ---      \u2506 ---        \u2506 ---           \u2506 ---    \u2502\n",
                             "\u2502 f64         \u2506 str  \u2506 cat  \u2506 f64       \u2506   \u2506 date     \u2506 time       \u2506 datetime[\u03bcs]  \u2506 f32    \u2502\n",
                             "\u255e\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2561\n",
-                            "\u2502 446.0       \u2506 null \u2506 null \u2506 29.493075 \u2506 \u2026 \u2506 null     \u2506 null       \u2506 null          \u2506 null   \u2502\n",
+                            "\u2502 446.0       \u2506 null \u2506 null \u2506 29.707042 \u2506 \u2026 \u2506 null     \u2506 null       \u2506 null          \u2506 null   \u2502\n",
                             "\u2514\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518"
                         ]
                     },
                     "execution_count": 15,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
@@ -834,24 +844,24 @@
                         "text/html": [
                             "<div><style>\n",
                             ".dataframe > thead > tr > th,\n",
                             ".dataframe > tbody > tr > td {\n",
                             "  text-align: right;\n",
                             "}\n",
                             "</style>\n",
-                            "<small>shape: (1, 12)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>PassengerId</th><th>Name</th><th>Sex</th><th>Age</th><th>Parch</th><th>Fare</th><th>Cabin</th><th>Embarked</th><th>Birthday</th><th>Board time</th><th>Married since</th><th>all_NA</th></tr><tr><td>u32</td><td>u32</td><td>u32</td><td>u32</td><td>u32</td><td>u32</td><td>u32</td><td>u32</td><td>u32</td><td>u32</td><td>u32</td><td>u32</td></tr></thead><tbody><tr><td>0</td><td>0</td><td>0</td><td>185</td><td>0</td><td>0</td><td>700</td><td>1</td><td>96</td><td>76</td><td>95</td><td>891</td></tr></tbody></table></div>"
+                            "<small>shape: (1, 12)</small><table border=\"1\" class=\"dataframe\"><thead><tr><th>PassengerId</th><th>Name</th><th>Sex</th><th>Age</th><th>Parch</th><th>Fare</th><th>Cabin</th><th>Embarked</th><th>Birthday</th><th>Board time</th><th>Married since</th><th>all_NA</th></tr><tr><td>u32</td><td>u32</td><td>u32</td><td>u32</td><td>u32</td><td>u32</td><td>u32</td><td>u32</td><td>u32</td><td>u32</td><td>u32</td><td>u32</td></tr></thead><tbody><tr><td>0</td><td>0</td><td>0</td><td>175</td><td>0</td><td>0</td><td>694</td><td>2</td><td>73</td><td>81</td><td>98</td><td>891</td></tr></tbody></table></div>"
                         ],
                         "text/plain": [
                             "shape: (1, 12)\n",
                             "\u250c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u252c\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2510\n",
                             "\u2502 PassengerId \u2506 Name \u2506 Sex \u2506 Age \u2506 \u2026 \u2506 Birthday \u2506 Board time \u2506 Married since \u2506 all_NA \u2502\n",
                             "\u2502 ---         \u2506 ---  \u2506 --- \u2506 --- \u2506   \u2506 ---      \u2506 ---        \u2506 ---           \u2506 ---    \u2502\n",
                             "\u2502 u32         \u2506 u32  \u2506 u32 \u2506 u32 \u2506   \u2506 u32      \u2506 u32        \u2506 u32           \u2506 u32    \u2502\n",
                             "\u255e\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u256a\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2550\u2561\n",
-                            "\u2502 0           \u2506 0    \u2506 0   \u2506 185 \u2506 \u2026 \u2506 96       \u2506 76         \u2506 95            \u2506 891    \u2502\n",
+                            "\u2502 0           \u2506 0    \u2506 0   \u2506 175 \u2506 \u2026 \u2506 73       \u2506 81         \u2506 98            \u2506 891    \u2502\n",
                             "\u2514\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518"
                         ]
                     },
                     "execution_count": 17,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
```

### Comparing `metasynth-0.3.0/examples/basic_example.json` & `metasynth-0.4.0/examples/basic_example.json`

 * *Files identical despite different names*

### Comparing `metasynth-0.3.0/examples/basic_example.py` & `metasynth-0.4.0/examples/basic_example.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import polars as pl
-from metasynth import MetaDataset
+from metasynth import MetaFrame
 
 # example dataframe from polars website
 df = pl.DataFrame(
     {
         "ID": [1, 2, 3, 4, 5],
         "fruits": ["banana", "banana", "apple", "apple", "banana"],
         "B": [5, 4, 3, 2, 1],
@@ -20,20 +20,20 @@
 
 # set A to unique and B to not unique
 spec_dict = {
     "ID": {"unique": True},
     "B": {"unique": False}
 }
 
-# create metadataset
-mds = MetaDataset.from_dataframe(df, spec=spec_dict)
+# create MetaFrame
+mf = MetaFrame.fit_dataframe(df, spec=spec_dict)
 
 # write to json
-mds.to_json("examples/basic_example.json")
+mf.to_json("examples/basic_example.json")
 
 # then, export json from secure environment
 
 # outside secure environment, load json
-mds_out = MetaDataset.from_json("examples/basic_example.json")
+mf_out = MetaFrame.from_json("examples/basic_example.json")
 
 # create a fake dataset
-mds_out.synthesize(10)
+mf_out.synthesize(10)
```

### Comparing `metasynth-0.3.0/examples/demonstration.csv` & `metasynth-0.4.0/examples/demonstration.csv`

 * *Files identical despite different names*

### Comparing `metasynth-0.3.0/examples/descriptions.ipynb` & `metasynth-0.4.0/examples/descriptions.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999732905982906%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(2, 'from metasynth import MetaFrame, MetaVar\\n')], delete: "*

 * *            "[2]}}, 11: {'source': {insert: [(1, 'meta_dataset = MetaFrame.fit_dataframe(\\n')], "*

 * *            'delete: [1]}}}'}*

```diff
@@ -19,15 +19,15 @@
             "execution_count": 1,
             "id": "2442cb34",
             "metadata": {},
             "outputs": [],
             "source": [
                 "import datetime as dt\n",
                 "import pandas as pd\n",
-                "from metasynth import MetaDataset, MetaVar\n",
+                "from metasynth import MetaFrame, MetaVar\n",
                 "from metasynth.distribution import DiscreteUniformDistribution\n",
                 "from pprint import pprint"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "04466c26",
@@ -285,15 +285,15 @@
                     "text": [
                         "{'Cabin': 'The cabin number of the passenger.'}\n"
                     ]
                 }
             ],
             "source": [
                 "from metasynth.distribution import FakerDistribution\n",
-                "meta_dataset = MetaDataset.from_dataframe(\n",
+                "meta_dataset = MetaFrame.fit_dataframe(\n",
                 "    df,\n",
                 "    spec={\n",
                 "        \"Name\": {\"distribution\": FakerDistribution(\"name\")},\n",
                 "        \"Fare\": {\"distribution\": \"LogNormalDistribution\"},\n",
                 "        \"Age\": {\"distribution\": DiscreteUniformDistribution(20, 40)},\n",
                 "        \"PassengerId\": {\"unique\": True},\n",
                 "        \"Cabin\": {\"distribution\": FakerDistribution(\"city\"), \"description\": \"The cabin number of the passenger.\"},\n",
```

### Comparing `metasynth-0.3.0/examples/titanic.ipynb` & `metasynth-0.4.0/examples/titanic.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9990924873737373%*

 * *Differences: {"'cells'": "{3: {'source': {insert: [(6, 'from metasynth import MetaFrame')], delete: [6]}}, 11: "*

 * *            '{\'source\': {insert: [(0, \'dataset = MetaFrame.fit_dataframe(df, spec={"Cabin": '*

 * *            '{"distribution": "regex", "fit_kwargs": {"mode": "fast"}}\\n\')], delete: [0]}}, 19: '*

 * *            '{\'source\': [\'print(MetaFrame.from_json("test.json"))\']}}'}*

```diff
@@ -33,15 +33,15 @@
             "source": [
                 "import json\n",
                 "from pathlib import Path\n",
                 "\n",
                 "import pandas as pd\n",
                 "import wget\n",
                 "\n",
-                "from metasynth import MetaDataset"
+                "from metasynth import MetaFrame"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "872c6e15",
             "metadata": {},
             "source": [
@@ -133,15 +133,15 @@
                         "Set the variable to be either unique or not unique to remove this warning.\n",
                         "\n",
                         "  warnings.warn(f\"\\nVariable {series.name} seems unique, but not set to be unique.\\n\"\n"
                     ]
                 }
             ],
             "source": [
-                "dataset = MetaDataset.from_dataframe(df, spec={\"Cabin\": {\"distribution\": \"regex\", \"fit_kwargs\": {\"mode\": \"fast\"}}\n",
+                "dataset = MetaFrame.fit_dataframe(df, spec={\"Cabin\": {\"distribution\": \"regex\", \"fit_kwargs\": {\"mode\": \"fast\"}}\n",
                 "                                              })"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "a30a428e",
             "metadata": {},
@@ -569,15 +569,15 @@
                         "\n",
                         "{'name': 'Embarked', 'description': None, 'type': 'categorical', 'dtype': 'Categorical', 'prop_missing': 0.002244668911335578, 'distribution': \"{'implements': 'core.multinoulli', 'provenance': 'builtin', 'class_name': 'MultinoulliDistribution', 'parameters': {'labels': ['C', 'Q', 'S'], 'probs': [0.1889763779527559, 0.08661417322834646, 0.7244094488188977]}}\"}\n",
                         "\n"
                     ]
                 }
             ],
             "source": [
-                "print(MetaDataset.from_json(\"test.json\"))"
+                "print(MetaFrame.from_json(\"test.json\"))"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "26e6ac69",
             "metadata": {},
             "source": [
```

### Comparing `metasynth-0.3.0/examples/utils.py` & `metasynth-0.4.0/examples/utils.py`

 * *Files identical despite different names*

### Comparing `metasynth-0.3.0/metasynth/dataset.py` & `metasynth-0.4.0/metasynth/dataset.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,32 @@
-"""Conversion of pandas dataframes to MetaSynth datasets."""   # pylint: disable=invalid-name
+"""Conversion of dataframes to MetaSynth datasets."""   # pylint: disable=invalid-name
 
 from __future__ import annotations
 
 import json
 import pathlib
 from copy import deepcopy
 from datetime import datetime
 from importlib.metadata import version
-from importlib.resources import read_text
 from typing import Any, Dict, List, Optional, Sequence, Union
 
-import jsonschema
 import numpy as np
 import polars as pl
 
 from metasynth.privacy import BasePrivacy, BasicPrivacy
 from metasynth.provider import BaseDistributionProvider
 from metasynth.validation import validate_gmf_dict
 from metasynth.var import MetaVar
 
 
-class MetaDataset():
+class MetaFrame():
     """MetaSynth dataset consisting of variables.
 
     The MetaSynth dataset structure that is most easily created from
-    a pandas dataset with the from_dataframe class method.
+    a polars dataset with the from_dataframe class method.
 
     Parameters
     ----------
     meta_vars:
         List of variables representing columns in a dataframe.
     n_rows:
         Number of rows in the original dataframe.
@@ -43,29 +41,30 @@
 
     @property
     def n_columns(self) -> int:
         """int: Number of columns of the original dataframe."""
         return len(self.meta_vars)
 
     @classmethod
-    def from_dataframe(cls,
-                       df: pl.DataFrame,
-                       spec: Optional[dict[str, dict]] = None,
-                       dist_providers: Union[str, list[str], BaseDistributionProvider,
-                                             list[BaseDistributionProvider]] = "builtin",
-                       privacy: Optional[BasePrivacy] = None):
-        """Create dataset from a Pandas dataframe.
+    def fit_dataframe(
+            cls,
+            df: pl.DataFrame,
+            spec: Optional[dict[str, dict]] = None,
+            dist_providers: Union[str, list[str], BaseDistributionProvider,
+                                  list[BaseDistributionProvider]] = "builtin",
+            privacy: Optional[BasePrivacy] = None):
+        """Create a MetaSynth object from a polars (or pandas) dataframe.
 
-        The pandas dataframe should be formatted already with the correct
-        datatypes.
+        The Polars dataframe should be formatted already with the correct
+        datatypes, such as pl.Categorical (or the pandas equivalent).
 
         Parameters
         ----------
         df:
-            Pandas dataframe with the correct column dtypes.
+            Polars dataframe with the correct column dtypes.
         spec:
             Column specifications to modify the defaults. For each of the columns additional
             directives can be supplied here. There are 3 different directives currently supported:
 
             distribution
 
             Set the distribution, either with a string that gives one of their
@@ -105,39 +104,52 @@
             Distribution providers to use when fitting distributions to variables.
             Can be a string, provider, or provider type.
         privacy:
             Privacy level to use by default.
 
         Returns
         -------
-        MetaDataset:
+        MetaFrame:
             Initialized MetaSynth dataset.
         """
         if privacy is None:
             privacy = BasicPrivacy()
         if spec is None:
             spec = {}
         else:
             spec = deepcopy(spec)
 
+        if set(list(spec)) - set(df.columns):
+            raise ValueError(
+                "Argument 'spec' includes the specifications for column names that do "
+                "not exist in the supplied dataframe:"
+                f" '{set(list(spec)) - set(df.columns)}'")
         all_vars = []
         for col_name in df.columns:
             series = df[col_name]
             col_spec = spec.get(col_name, {})
             dist = col_spec.pop("distribution", None)
             unq = col_spec.pop("unique", None)
             description = col_spec.pop("description", None)
             prop_missing = col_spec.pop("prop_missing", None)
             cur_privacy = col_spec.pop("privacy", privacy)
             fit_kwargs = col_spec.pop("fit_kwargs", {})
             if len(col_spec) != 0:
-                raise ValueError(f"Unknown spec items '{col_spec}' for variable '{col_name}'.")
-            var = MetaVar.detect(series, description=description, prop_missing=prop_missing)
-            var.fit(dist=dist, dist_providers=dist_providers, unique=unq, privacy=cur_privacy,
-                    fit_kwargs=fit_kwargs)
+                raise ValueError(
+                    f"Unknown spec items '{col_spec}' for variable '{col_name}'.")
+            var = MetaVar.detect(
+                series,
+                description=description,
+                prop_missing=prop_missing)
+            var.fit(
+                dist=dist,
+                dist_providers=dist_providers,
+                unique=unq,
+                privacy=cur_privacy,
+                fit_kwargs=fit_kwargs)
 
             all_vars.append(var)
 
         return cls(all_vars, len(df))
 
     def to_dict(self) -> Dict[str, Any]:
         """Create dictionary with the properties for recreation."""
@@ -164,40 +176,46 @@
             for var in self.meta_vars:
                 if var.name == key:
                     return var
             raise KeyError(f"Cannot find variable '{key}'")
         raise TypeError(f"Cannot get item for key '{key}'")
 
     def __str__(self) -> str:
-        """Create a readable string that shows the variables."""
-        cur_str = "# Rows: "+str(self.n_rows)+"\n"
-        cur_str += "# Columns: "+str(self.n_columns)+"\n"
-        for var in self.meta_vars:
-            cur_str += "\n"+str(var)+"\n"
-        return cur_str
+        """Return an easy to read formatted string for the dataset."""
+        vars_formatted = "\n".join(
+            f"Column {i + 1}: {str(var)}" for i,
+            var in enumerate(
+                self.meta_vars))
+        return (
+            f"# Rows: {self.n_rows}\n"
+            f"# Columns: {self.n_columns}\n\n"
+            f"{vars_formatted}\n"
+        )
 
     @property
     def descriptions(self) -> dict[str, str]:
         """Return the descriptions of the columns."""
         return {var.name: var.description for var in self.meta_vars
                 if var.name is not None and var.description is not None}
 
     @descriptions.setter
-    def descriptions(self, new_descriptions: Union[dict[str, str], Sequence[str]]):
+    def descriptions(
+            self, new_descriptions: Union[dict[str, str], Sequence[str]]):
         if isinstance(new_descriptions, dict):
             for var_name, new_desc in new_descriptions.items():
                 self[var_name].description = new_desc
         else:
             assert len(new_descriptions) == self.n_columns, (
                 "Descriptions need to be either a dict or a "
                 "sequence with the length of the number of variables.")
             for i_desc, new_desc in enumerate(new_descriptions):
                 self[i_desc].description = new_desc
 
-    def to_json(self, fp: Union[pathlib.Path, str], validate: bool = True) -> None:
+    def to_json(self, fp: Union[pathlib.Path, str],
+                validate: bool = True) -> None:
         """Write the MetaSynth dataset to a JSON file.
 
         Optional validation against a JSON schema included in the package.
 
         Parameters
         ----------
         fp:
@@ -208,56 +226,62 @@
         self_dict = _jsonify(self.to_dict())
         if validate:
             validate_gmf_dict(self_dict)
         with open(fp, "w", encoding="utf-8") as f:
             json.dump(self_dict, f, indent=4)
 
     @classmethod
-    def from_json(cls, fp: Union[pathlib.Path, str], validate: bool = True) -> MetaDataset:
+    def from_json(cls, fp: Union[pathlib.Path, str],
+                  validate: bool = True) -> MetaFrame:
         """Read a MetaSynth dataset from a JSON file.
 
         Parameters
         ----------
         fp:
             Path to read the data from.
         validate:
             Validate the JSON file with a schema.
 
         Returns
         -------
-        MetaDataset:
-            A restored metadataset from the file.
+        MetaFrame:
+            A restored MetaFrame from the file.
         """
         with open(fp, "r", encoding="utf-8") as f:
             self_dict = json.load(f)
 
         if validate:
-            schema = json.loads(read_text("metasynth.schema", "generative_metadata_format.json"))
-            jsonschema.validate(instance=self_dict, schema=schema)
+            validate_gmf_dict(self_dict)
 
         n_rows = self_dict["n_rows"]
         meta_vars = [MetaVar.from_dict(d) for d in self_dict["vars"]]
         return cls(meta_vars, n_rows)
 
     def synthesize(self, n: int) -> pl.DataFrame:
-        """Create a synthetic pandas dataframe.
+        """Create a synthetic Polars dataframe.
 
         Parameters
         ----------
         n:
             Number of rows to generate.
 
         Returns
         -------
-        pandas.DataFrame:
+        polars.DataFrame:
             Dataframe with the synthetic data.
         """
         synth_dict = {var.name: var.draw_series(n) for var in self.meta_vars}
         return pl.DataFrame(synth_dict)
 
+    def __repr__(self) -> str:
+        """Return the MetaFrame as it would be output to JSON."""
+        pretty_data = _jsonify(self.to_dict())
+        output = json.dumps(pretty_data, indent=4)
+        return output
+
 
 def _jsonify(data):
     if isinstance(data, (list, tuple)):
         return [_jsonify(d) for d in data]
     if isinstance(data, dict):
         return {key: _jsonify(value) for key, value in data.items()}
```

### Comparing `metasynth-0.3.0/metasynth/demo/dataset.py` & `metasynth-0.4.0/metasynth/demo/dataset.py`

 * *Files identical despite different names*

### Comparing `metasynth-0.3.0/metasynth/demo/demo_titanic.csv` & `metasynth-0.4.0/metasynth/demo/demo_titanic.csv`

 * *Files identical despite different names*

### Comparing `metasynth-0.3.0/metasynth/distribution/__init__.py` & `metasynth-0.4.0/metasynth/distribution/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,14 @@
 """Distributions for variables.
 
 These distributions can be fit to datasets/series so that the synthesis is
 somewhat realistic. The concept of distributions here is not only for
 numerical data, but also for generating strings for example.
 """  # pylint: disable=invalid-name
 
-from metasynth.distribution.base import (CategoricalDistribution,
-                                         ContinuousDistribution,
-                                         DateDistribution,
-                                         DateTimeDistribution,
-                                         DiscreteDistribution,
-                                         StringDistribution, TimeDistribution)
 from metasynth.distribution.categorical import MultinoulliDistribution
 from metasynth.distribution.continuous import (ExponentialDistribution,
                                                LogNormalDistribution,
                                                NormalDistribution,
                                                TruncatedNormalDistribution,
                                                UniformDistribution)
 from metasynth.distribution.datetime import (UniformDateDistribution,
@@ -22,17 +16,16 @@
                                              UniformTimeDistribution)
 from metasynth.distribution.discrete import (DiscreteUniformDistribution,
                                              PoissonDistribution,
                                              UniqueKeyDistribution)
 from metasynth.distribution.faker import FakerDistribution
 from metasynth.distribution.regex import (RegexDistribution,
                                           UniqueRegexDistribution)
-
+from metasynth.distribution.na import NADistribution
 __all__ = [
-    "DiscreteDistribution", "ContinuousDistribution", "CategoricalDistribution",
-    "DateDistribution", "DateTimeDistribution", "StringDistribution", "TimeDistribution",
     "MultinoulliDistribution", "UniformDistribution", "NormalDistribution",
     "LogNormalDistribution", "TruncatedNormalDistribution", "ExponentialDistribution",
     "DiscreteUniformDistribution", "PoissonDistribution", "UniqueKeyDistribution",
     "UniformDateDistribution", "UniformDateTimeDistribution", "UniformTimeDistribution",
     "FakerDistribution", "RegexDistribution", "UniqueRegexDistribution",
+    "NADistribution",
 ]
```

### Comparing `metasynth-0.3.0/metasynth/distribution/base.py` & `metasynth-0.4.0/metasynth/distribution/continuous.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,255 +1,223 @@
-"""Module for the base distribution and the scipy distribution."""
-
-from __future__ import annotations
-
-from abc import ABC, abstractmethod
-from copy import deepcopy
-from typing import Iterable, Sequence, Union
+"""Implemented floating point distributions."""
 
 import numpy as np
-import pandas as pd
-import polars as pl
-
-
-class BaseDistribution(ABC):
-    """Abstract base class to define a distribution.
-
-    All distributions should be derived from this class, and the following
-    methods need to be implemented: _fit, draw, to_dict.
+from scipy.optimize import minimize
+from scipy.stats import expon, lognorm, norm, truncnorm, uniform
+from scipy.stats._continuous_distns import FitDataError
+
+from metasynth.distribution.base import metadist, ScipyDistribution
+
+
+@metadist(implements="core.uniform", var_type="continuous")
+class UniformDistribution(ScipyDistribution):
+    """Uniform distribution for floating point type.
+
+    This class implements the uniform distribution between a minimum
+    and maximum.
+
+    Parameters
+    ----------
+    min_val: float
+        Lower bound for uniform distribution.
+    max_val: float
+        Upper bound for uniform distribution.
     """
 
-    implements = "unknown"
-    provenance = "unknown"
-    privacy = "unknown"
-    is_unique = False
-    var_type: str = "unknown"
-
-    @classmethod
-    def fit(cls, series: Union[Sequence, pl.Series], *args, **kwargs) -> BaseDistribution:
-        """Fit the distribution to the series.
-
-        Parameters
-        ----------
-        series: pandas.Series
-            Data to fit the distribution to.
-
-        Returns
-        -------
-        BaseDistribution:
-            Fitted distribution.
-        """
-        pd_series = cls._to_series(series)
-        if len(pd_series) == 0:
-            return cls.default_distribution()
-        distribution = cls._fit(pd_series, *args, **kwargs)
-        return distribution
+    dist_class = uniform
 
-    @staticmethod
-    def _to_series(values: Union[Sequence, pl.Series]):
-        if isinstance(values, pl.Series):
-            series = values.drop_nulls()
-        elif isinstance(values, pd.Series):
-            series = pl.Series(values).drop_nulls()  # pylint: disable=assignment-from-no-return
-        else:
-            series_array = np.array(values)
-            series_array = series_array[~np.isnan(series_array)]
-            series = pl.Series(series_array)
-        return series
-
-    @classmethod
-    @abstractmethod
-    def _fit(cls, values: pl.Series) -> BaseDistribution:
-        """See fit method, but does not need to deal with NA's."""
-
-    @abstractmethod
-    def draw(self) -> object:
-        """Draw a random element from the fitted distribution."""
-
-    def draw_reset(self) -> None:
-        """Reset the drawing of elements to start again."""
-
-    def __str__(self) -> str:
-        """Create a human readable string of the object."""
-        return str(self.to_dict())
-
-    @abstractmethod
-    def _param_dict(self):
-        """Get dictionary with the parameters of the distribution."""
+    def __init__(self, min_val: float, max_val: float):
+        self.par = {"min_val": min_val, "max_val": max_val}
+        self.dist = uniform(loc=self.min_val, scale=max(self.max_val-self.min_val, 1e-8))
 
-    def to_dict(self) -> dict:
-        """Convert the distribution to a dictionary."""
-        return {
-            "implements": self.implements,
-            "provenance": self.provenance,
-            "class_name": self.__class__.__name__,
-            "parameters": deepcopy(self._param_dict()),
-        }
+    @classmethod
+    def _fit(cls, values):
+        return cls(values.min(), values.max())
+
+    def _information_criterion(self, values):
+        if np.any(np.array(values) < self.min_val) or np.any(np.array(values) > self.max_val):
+            return 2*self.n_par + 100*len(values)
+        if np.fabs(self.max_val-self.min_val) < 1e-8:
+            return 2*self.n_par - 100*len(values)
+        return 2*self.n_par - 2*len(values)*np.log((self.max_val-self.min_val)**-1)
 
     @classmethod
-    @abstractmethod
-    def _param_schema(cls):
-        """Get schema for the parameters of the distribution."""
+    def default_distribution(cls):
+        return cls(0, 1)
 
     @classmethod
-    def schema(cls) -> dict:
-        """Create sub-schema to validate GMF file."""
+    def _param_schema(cls):
         return {
-            "type": "object",
-            "properties": {
-                "implements": {"const": cls.implements},
-                "provenance": {"const": cls.provenance},
-                "class_name": {"const": cls.__name__},
-                "parameters": {
-                    "type": "object",
-                    "properties": cls._param_schema(),
-                    "required": list(cls.default_distribution()._param_dict())
-                }
-            },
-            "required": ["implements", "provenance", "class_name", "parameters"]
+            "min_val": {"type": "number"},
+            "max_val": {"type": "number"},
         }
 
-    @classmethod
-    def from_dict(cls, dist_dict: dict) -> BaseDistribution:
-        """Create a distribution from a dictionary."""
-        return cls(**dist_dict["parameters"])
 
-    def information_criterion(self, values: Iterable) -> float:  # pylint: disable=unused-argument
-        """Get the AIC value for a particular set of values.
+@metadist(implements="core.normal", var_type="continuous")
+class NormalDistribution(ScipyDistribution):
+    """Normal distribution for floating point type.
+
+    This class implements the normal/gaussian distribution and takes
+    the average and standard deviation as initialization input.
+
+    Parameters
+    ----------
+    mean: float
+        Mean of the normal distribution.
 
-        Parameters
-        ----------
-        values: array_like
-            Values to determine the AIC value of.
-        """
-        return 0.0
-
-    @classmethod
-    def matches_name(cls, name: str) -> bool:
-        """Check whether the name matches the distribution.
+    std_dev: float
+        Standard deviation of the normal distribution.
+    """
 
-        Parameters
-        ----------
-        name: str
-            Name to match to the distribution.
+    implements = "core.normal"
+    dist_class = norm
 
-        Returns
-        -------
-        bool:
-            Whether the name matches.
-        """
-        assert cls.implements != "unknown", f"Internal error in class {cls.__name__}"
-        return name in (cls.implements.split(".")[1],
-                        cls.implements,
-                        cls.__name__,
-                        )
+    def __init__(self, mean: float, std_dev: float):
+        self.par = {"mean": mean, "std_dev": std_dev}
+        self.dist = norm(loc=mean, scale=max(std_dev, 1e-8))
 
     @classmethod
-    @abstractmethod
-    def default_distribution(cls) -> BaseDistribution:
-        """Get a distribution with default parameters."""
-        return cls()
-
-
-class CoreDistribution():  # pylint: disable=too-few-public-methods
-    """Distributions belonging to the core set."""
-
-    privacy = "none"
-    provenance = "builtin"
-
+    def default_distribution(cls):
+        return cls(0, 1)
 
-class CategoricalDistribution(BaseDistribution):
-    """Base Class for categorical distributions."""
-
-    var_type = "categorical"
-
-
-class DiscreteDistribution(BaseDistribution):
-    """Base Class for discrete distributions."""
-
-    var_type = "discrete"
-
-
-class ContinuousDistribution(BaseDistribution):
-    """Base Class for continuous distributions."""
+    @classmethod
+    def _param_schema(cls):
+        return {
+            "mean": {"type": "number"},
+            "std_dev": {"type": "number"},
+        }
 
-    var_type = "continuous"
 
+@metadist(implements="core.lognormal", var_type="continuous")
+class LogNormalDistribution(ScipyDistribution):
+    """Log-normal distribution for floating point type.
+
+    This class implements the log-normal mu and sigma as initialization input.
+
+    Parameters
+    ----------
+    sigma: float
+        Controls the width of the distribution.
+    mu: float
+        Controls the mean of the distribution.
+    """
 
-class StringDistribution(BaseDistribution):
-    """Base Class for string distributions."""
+    dist_class = lognorm
 
-    var_type = "string"
+    def __init__(self, mu: float, sigma: float):  # pylint: disable=invalid-name
+        self.par = {"mu": mu, "sigma": sigma}
+        self.dist = lognorm(s=max(sigma, 1e-8), scale=np.exp(mu))
 
+    @classmethod
+    def _fit(cls, values):
+        try:
+            sigma, _, scale = cls.dist_class.fit(values, floc=0)
+        except FitDataError:
+            return cls(0, 1)
+        return cls(np.log(scale), sigma)
 
-class DateTimeDistribution(BaseDistribution):
-    """Base Class for date-time distributions."""
+    @classmethod
+    def default_distribution(cls):
+        return cls(0, 1)
 
-    var_type = "datetime"
+    @classmethod
+    def _param_schema(cls):
+        return {
+            "mu": {"type": "number"},
+            "sigma": {"type": "number"},
+        }
 
 
-class DateDistribution(BaseDistribution):
-    """Base Class for date distributions."""
+@metadist(implements="core.truncated_normal", var_type="continuous")
+class TruncatedNormalDistribution(ScipyDistribution):
+    """Truncated normal distribution for floating point type.
+
+    Parameters
+    ----------
+    lower_bound: float
+        Lower bound of the truncated normal distribution.
+    upper_bound: float
+        Upper bound of the truncated normal distribution.
+    mu: float
+        Mean of the non-truncated normal distribution.
+    sigma: float
+        Standard deviation of the non-truncated normal distribution.
+    """
 
-    var_type = "date"
+    dist_class = truncnorm
 
+    def __init__(self, lower_bound: float, upper_bound: float,
+                 mu: float, sigma: float):
+        self.par = {"lower_bound": lower_bound, "upper_bound": upper_bound,
+                    "mu": mu, "sigma": sigma}
+        a, b = (lower_bound-mu)/sigma, (upper_bound-mu)/sigma
+        self.dist = truncnorm(a=a, b=b, loc=mu, scale=max(sigma, 1e-8))
 
-class TimeDistribution(BaseDistribution):
-    """Base Class for time distributions."""
+    @classmethod
+    def _fit(cls, values):
+        lower_bound = values.min() - 1e-8
+        upper_bound = values.max() + 1e-8
+        return cls._fit_with_bounds(values, lower_bound, upper_bound)
+
+    @classmethod
+    def _fit_with_bounds(cls, values, lower_bound, upper_bound):
+        def minimizer(param):
+            mu, sigma = param
+            a, b = (lower_bound-mu)/sigma, (upper_bound-mu)/sigma
+            dist = truncnorm(a=a, b=b, loc=mu, scale=sigma)
+            return -np.sum(dist.logpdf(values))
+
+        x_start = [(lower_bound+upper_bound)/2, (upper_bound-lower_bound)/4]
+        mu, sigma = minimize(minimizer, x_start,
+                             bounds=[(None, None),
+                                     ((upper_bound-lower_bound)/100, None)]).x
+        return cls(lower_bound, upper_bound, mu, sigma)
 
-    var_type = "time"
+    @classmethod
+    def default_distribution(cls):
+        return cls(-1, 2, 0, 1)
 
+    @classmethod
+    def _param_schema(cls):
+        return {
+            "lower_bound": {"type": "number"},
+            "upper_bound": {"type": "number"},
+            "mu": {"type": "number"},
+            "sigma": {"type": "number"},
+        }
 
-class ScipyDistribution(BaseDistribution):
-    """Base class for numerical Scipy distributions.
 
-    This base class makes it easy to implement new numerical
-    distributions. One could also use this base class for non-scipy
-    distributions, in which case the distribution class should implement
-    logpdf, rvs and fit methods.
+@metadist(implements="core.exponential", var_type="continuous")
+class ExponentialDistribution(ScipyDistribution):
+    """Exponential distribution for floating point type.
+
+    This class implements the exponential distribution with the rate as its
+    single parameter.
+
+    Parameters
+    ----------
+    rate: float
+        Rate of the exponential distribution. This is equal to 1/mean of the distribution.
     """
 
-    @property
-    def n_par(self) -> int:
-        """int: Number of parameters for distribution."""
-        return len(self.par)
-
-    def __getattr__(self, attr: str):
-        """Get attribute for easy access to parameters.
-
-        Parameters
-        ----------
-        attr:
-            Attribute to retrieve. If the attribute is a parameter
-            name, then retrieve that parameter, otherwise use the default
-            implementation for getting the attribute.
-
-        Returns
-        -------
-        object:
-            Parameter or attribute.
-        """
-        if attr != "par" and attr in self.par:
-            return self.par[attr]
-        return object.__getattribute__(self, attr)
+    dist_class = expon
+
+    def __init__(self, rate: float):
+        self.par = {"rate": rate}
+        self.dist = expon(loc=0, scale=1/max(rate, 1e-8))
 
     @classmethod
     def _fit(cls, values):
+        values = values.filter(values > 0)
         if len(values) == 0:
             return cls.default_distribution()
-        param = cls.dist_class.fit(values)
-        return cls(*param)
-
-    def _param_dict(self):
-        return self.par
+        return cls(rate=1/expon.fit(values, floc=0)[1])
 
-    def draw(self):
-        return self.dist.rvs()
-
-    def information_criterion(self, values):
-        vals = self._to_series(values)
-        if len(vals) == 0:
-            return 2*self.n_par
-        return self._information_criterion(vals)
+    @classmethod
+    def default_distribution(cls):
+        return cls(1.0)
 
-    def _information_criterion(self, values):
-        return 2*self.n_par - 2*np.sum(self.dist.logpdf(values))
+    @classmethod
+    def _param_schema(cls):
+        return {
+            "rate": {"type": "number"}
+        }
```

### Comparing `metasynth-0.3.0/metasynth/distribution/categorical.py` & `metasynth-0.4.0/metasynth/distribution/categorical.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,46 @@
 """Module containing categorical distributions."""
 
+from __future__ import annotations
+
 from typing import Union
+import warnings
 
 import numpy as np
 import numpy.typing as npt
 import pandas as pd
 import polars as pl
 
-from metasynth.distribution.base import (CategoricalDistribution,
-                                         CoreDistribution)
+from metasynth.distribution.base import metadist, BaseDistribution
 
 
-class MultinoulliDistribution(CoreDistribution, CategoricalDistribution):
+@metadist(implements="core.multinoulli", var_type="categorical")
+class MultinoulliDistribution(BaseDistribution):
     """Categorical distribution that stores category labels and probabilities.
 
     Parameters
     ----------
     labels: list of str
         List containing the label belonging to each category.
     probs: list of int
         List containing the probability of each category.
         Probabilities will be normalized, so frequencies are valid too.
     """
 
-    implements = "core.multinoulli"
-
-    def __init__(self, labels: npt.NDArray[np.str_],
-                 probs: npt.NDArray[np.float_]):
-        self.labels = labels
-        self.probs = probs
-        if np.sum(self.probs) != 1:
-            self.probs = self.probs/np.sum(self.probs)
+    def __init__(self, labels: Union[npt.NDArray[np.str_], list[str]],
+                 probs: Union[npt.NDArray[np.float_], list[float]]):
+        self.labels = np.array(labels)
+        self.probs = np.array(probs)
+        if not np.isclose(np.sum(self.probs), 1):
+            if np.any(self.probs < 0):
+                raise ValueError("Cannot create multinoulli distribution with probabilities < 0.")
+            warnings.simplefilter("always")
+            warnings.warn("Multinoulli probabilities do not add up to 1 "
+                          f" ({np.sum(self.probs)}); they will be rescaled.")
+        self.probs = self.probs/np.sum(self.probs)
 
     @classmethod
     def _fit(cls, values: pl.Series):
         labels, counts = np.unique(values, return_counts=True)
         probs = counts/np.sum(counts)
         return cls(labels.astype(str), probs)
 
@@ -65,8 +71,8 @@
             # account for missing values / missing categories
             # by setting default of .get to 1 (add log(1)=0 to log_lik)
             log_lik += count * np.log(pdict.get(lab, 1))
         return 2*(len(self.probs) - 1) - 2 * log_lik
 
     @classmethod
     def default_distribution(cls):
-        return cls(["a", "b", "c"], [10, 4, 20])
+        return cls(["a", "b", "c"], [0.1, 0.3, 0.6])
```

### Comparing `metasynth-0.3.0/metasynth/distribution/continuous.py` & `metasynth-0.4.0/metasynth/distribution/regex/base.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,223 +1,220 @@
-"""Implemented floating point distributions."""
+"""Module containing string distributions."""
 
-import numpy as np
-from scipy.optimize import minimize
-from scipy.stats import expon, lognorm, norm, truncnorm, uniform
-from scipy.stats._continuous_distns import FitDataError
-
-from metasynth.distribution.base import (ContinuousDistribution,
-                                         CoreDistribution, ScipyDistribution)
+from __future__ import annotations
 
+from typing import List, Sequence, Set, Tuple, Type, Union
 
-class UniformDistribution(CoreDistribution, ScipyDistribution, ContinuousDistribution):
-    """Uniform distribution for floating point type.
+import numpy as np
 
-    This class implements the uniform distribution between a minimum
-    and maximum.
+from metasynth.distribution.base import metadist, BaseDistribution
+from metasynth.distribution.regex.element import (AlphaNumericRegex, AnyRegex,
+                                                  BaseRegexElement, DigitRegex,
+                                                  LettersRegex, LowercaseRegex,
+                                                  SingleRegex, UppercaseRegex)
+from metasynth.distribution.regex.optimizer import RegexOptimizer
+
+
+def _get_gradient_start(values: Sequence[str], new_values: Sequence[str],
+                        regex_elem: BaseRegexElement) -> float:
+    """Get the proportion of the characters that were resolved with the regex."""
+    digits_used: List[int] = []
+    for i_val, old_val in enumerate(values):
+        new_val = new_values[i_val]
+        d_len = len(old_val) - len(new_val)
+        if len(digits_used) <= d_len:
+            digits_used += (d_len - len(digits_used) + 1)*[0]
+        digits_used[d_len] += 1
+    regex_stat = {
+        "n_values": len(values),
+        "frac_used": regex_elem.frac_used,
+        "digits_used": digits_used,
+    }
+    old_energy = RegexOptimizer.energy_from_values(values)
+    new_energy = RegexOptimizer.energy_from_values(new_values)
+    energy_budget = regex_elem.information_budget(regex_stat)
+
+    delta_energy = old_energy - new_energy
+    return delta_energy/energy_budget
+
+
+@metadist(implements="core.regex", var_type="string")
+class RegexDistribution(BaseDistribution):
+    """Distribution that uses a strategy similar to regex.
+
+    The idea behind this method is that for structured strings
+    regexes works very well. It uses a greedy algorithm to build the
+    regex. It does not implement all regexes, nor does it claim to be
+    compliant with standard ones.
 
     Parameters
     ----------
-    min_val: float
-        Lower bound for uniform distribution.
-    max_val: float
-        Upper bound for uniform distribution.
+    re_list: list of BaseRegexElement
+        List of basic regex elements in the order that they occur.
     """
 
-    implements = "core.uniform"
-    dist_class = uniform
-
-    def __init__(self, min_val: float, max_val: float):
-        self.par = {"min_val": min_val, "max_val": max_val}
-        self.dist = uniform(loc=self.min_val, scale=max(self.max_val-self.min_val, 1e-8))
-
-    @classmethod
-    def _fit(cls, values):
-        return cls(values.min(), values.max())
-
-    def _information_criterion(self, values):
-        if np.any(np.array(values) < self.min_val) or np.any(np.array(values) > self.max_val):
-            return 2*self.n_par + 100*len(values)
-        if np.fabs(self.max_val-self.min_val) < 1e-8:
-            return 2*self.n_par - 100*len(values)
-        return 2*self.n_par - 2*len(values)*np.log((self.max_val-self.min_val)**-1)
+    implements = "core.regex"
 
-    @classmethod
-    def default_distribution(cls):
-        return cls(0, 1)
+    def __init__(self, re_list: Union[Sequence[Union[BaseRegexElement, Tuple[str, float]]], str]):
+        self.re_list = []
+        if isinstance(re_list, str):
+            self.re_list = self._unpack_regex(re_list)
+            return
+
+        for re_elem in re_list:
+            if isinstance(re_elem, BaseRegexElement):
+                self.re_list.append(re_elem)
+                continue
+            regex_str, frac_used = re_elem
+            regex_return = None
+            for regex_class in self.all_regex_classes():
+                regex_return = regex_class.from_string(regex_str, frac_used)
+                if regex_return is not None and regex_return[1] == "":
+                    break
+            if regex_return is None:
+                raise ValueError(f"Unrecognized regex element '{regex_str}'")
+            regex_dist_elem = regex_return[0]
+            self.re_list.append(regex_dist_elem)
+
+    @classmethod
+    def all_regex_classes(cls) -> List[Type[BaseRegexElement]]:
+        """Return all regex element classes."""
+        return [
+            DigitRegex, AlphaNumericRegex, LowercaseRegex, UppercaseRegex,
+            LettersRegex, SingleRegex, AnyRegex,
+        ]
+
+    def _unpack_regex(self, regex_str: str):
+        if len(regex_str) == 0:
+            return []
+        for re_elem_class in self.all_regex_classes():
+            ret = re_elem_class.from_string(regex_str)
+            if ret is not None:
+                return [ret[0]] + self._unpack_regex(ret[1])
+        raise ValueError("Failed to determine regex from '" + regex_str + "'")
+
+    @classmethod
+    def _fit(cls, values, mode: str = "fast"):
+        if mode == "fast":
+            return cls._fit_fast(values)
+        return cls._fit_slow(values)
+
+    @classmethod
+    def _fit_slow(cls, values):
+        if np.sum([len(val) for val in values]) == 0:
+            return cls([])
+
+        best_solution = None
+        regex_classes = cls.all_regex_classes()
+
+        # Iterate over all RegexElements and find the best one.
+        for re_class in regex_classes:
+            new_values, gradient, regexer = re_class.fit(list(values))
+            if best_solution is None or gradient > best_solution["gradient"]:
+                best_solution = {
+                    "re": regexer,
+                    "gradient": gradient,
+                    "values": new_values,
+                }
+        if best_solution is None:
+            return cls([])
+        left_fit = cls._fit_slow(best_solution["values"][0])
+        middle_fit = cls([best_solution["re"]])
+        right_fit = cls._fit_slow(best_solution["values"][1])
+        return left_fit + middle_fit + right_fit
+
+    @classmethod
+    def _fit_fast(cls, values):
+        n_char = np.sum([len(val) for val in values])
+        if n_char == 0:
+            return cls([])
+        best_solution = None
+        regex_classes = cls.all_regex_classes()
+
+        # Iterate over all RegexElements and find the best one.
+        for re_class in regex_classes:
+            new_values, regexer = re_class.fit_start(list(values))
+            # n_char_removed = _get_n_char_removed(values, new_values)
+            # cur_ic = regexer.information_criterion(n_char_removed)
+            # if cur_ic > 1.5:
+            # continue
+            gradient = _get_gradient_start(values, new_values, regexer)
+            if best_solution is None or gradient > best_solution["gradient"]:
+                best_solution = {
+                    "gradient": gradient,
+                    "re": regexer,
+                    "values": new_values,
+                }
+        if best_solution is None:
+            return cls([])
+        return cls([best_solution["re"]]) + cls._fit_fast(best_solution["values"])
+
+    def __add__(self, other: RegexDistribution) -> RegexDistribution:
+        return self.__class__(self.re_list + other.re_list)
+
+    def draw(self):
+        cur_str = ""
+        for rex in self.re_list:
+            cur_str += rex.draw()
+        return cur_str
+
+    @property
+    def regex_string(self) -> str:
+        """String representation of the string."""
+        return "".join([str(x) for x in self.re_list])
 
-    @classmethod
-    def _param_schema(cls):
+    def _param_dict(self):
         return {
-            "min_val": {"type": "number"},
-            "max_val": {"type": "number"},
+            "re_list": [(str(x), x.frac_used) for x in self.re_list],
         }
 
-
-class NormalDistribution(CoreDistribution, ScipyDistribution, ContinuousDistribution):
-    """Normal distribution for floating point type.
-
-    This class implements the normal/gaussian distribution and takes
-    the average and standard deviation as initialization input.
-
-    Parameters
-    ----------
-    mean: float
-        Mean of the normal distribution.
-
-    std_dev: float
-        Standard deviation of the normal distribution.
-    """
-
-    implements = "core.normal"
-    dist_class = norm
-
-    def __init__(self, mean: float, std_dev: float):
-        self.par = {"mean": mean, "std_dev": std_dev}
-        self.dist = norm(loc=mean, scale=max(std_dev, 1e-8))
-
-    @classmethod
-    def default_distribution(cls):
-        return cls(0, 1)
-
     @classmethod
     def _param_schema(cls):
         return {
-            "mean": {"type": "number"},
-            "std_dev": {"type": "number"},
+            "re_list": {
+                "type": "array",
+                "items": {
+                    "type": "array",
+                    "prefixItems": [{"type": "string"}, {"type": "number"}],
+                    "minItems": 2,
+                    "additionalItems": False
+                }
+            }
         }
 
-
-class LogNormalDistribution(CoreDistribution, ScipyDistribution, ContinuousDistribution):
-    """Log-normal distribution for floating point type.
-
-    This class implements the log-normal mu and sigma as initialization input.
-
-    Parameters
-    ----------
-    sigma: float
-        Controls the width of the distribution.
-    mu: float
-        Controls the mean of the distribution.
-    """
-
-    implements = "core.lognormal"
-    dist_class = lognorm
-
-    def __init__(self, mu: float, sigma: float):  # pylint: disable=invalid-name
-        self.par = {"mu": mu, "sigma": sigma}
-        self.dist = lognorm(s=max(sigma, 1e-8), scale=np.exp(mu))
-
-    @classmethod
-    def _fit(cls, values):
-        try:
-            sigma, _, scale = cls.dist_class.fit(values, floc=0)
-        except FitDataError:
-            return cls(0, 1)
-        return cls(np.log(scale), sigma)
-
     @classmethod
     def default_distribution(cls):
-        return cls(0, 1)
+        return cls([(r"\d{3,4}", 0.67)])
 
-    @classmethod
-    def _param_schema(cls):
-        return {
-            "mu": {"type": "number"},
-            "sigma": {"type": "number"},
-        }
 
+@metadist(implements="core.unique_regex", var_type="string", is_unique=True)
+class UniqueRegexDistribution(RegexDistribution):
+    """Unique variant of the regex distribution.
 
-class TruncatedNormalDistribution(CoreDistribution, ScipyDistribution, ContinuousDistribution):
-    """Truncated normal distribution for floating point type.
+    Same as the normal regex distribution, but checks whether a key
+    has already been used.
 
     Parameters
     ----------
-    lower_bound: float
-        Lower bound of the truncated normal distribution.
-    upper_bound: float
-        Upper bound of the truncated normal distribution.
-    mu: float
-        Mean of the non-truncated normal distribution.
-    sigma: float
-        Standard deviation of the non-truncated normal distribution.
+    re_list: list of BaseRegexElement
+        List of basic regex elements in the order that they occur.
     """
 
-    implements = "core.truncated_normal"
-    dist_class = truncnorm
-
-    def __init__(self, lower_bound: float, upper_bound: float,
-                 mu: float, sigma: float):
-        self.par = {"lower_bound": lower_bound, "upper_bound": upper_bound,
-                    "mu": mu, "sigma": sigma}
-        a, b = (lower_bound-mu)/sigma, (upper_bound-mu)/sigma
-        self.dist = truncnorm(a=a, b=b, loc=mu, scale=max(sigma, 1e-8))
-
-    @classmethod
-    def _fit(cls, values):
-        lower_bound = values.min() - 1e-8
-        upper_bound = values.max() + 1e-8
-        return cls._fit_with_bounds(values, lower_bound, upper_bound)
-
-    @classmethod
-    def _fit_with_bounds(cls, values, lower_bound, upper_bound):
-        def minimizer(param):
-            mu, sigma = param
-            a, b = (lower_bound-mu)/sigma, (upper_bound-mu)/sigma
-            dist = truncnorm(a=a, b=b, loc=mu, scale=sigma)
-            return -np.sum(dist.logpdf(values))
-
-        x_start = [(lower_bound+upper_bound)/2, (upper_bound-lower_bound)/4]
-        mu, sigma = minimize(minimizer, x_start,
-                             bounds=[(None, None),
-                                     ((upper_bound-lower_bound)/100, None)]).x
-        return cls(lower_bound, upper_bound, mu, sigma)
-
-    @classmethod
-    def default_distribution(cls):
-        return cls(-1, 2, 0, 1)
-
-    @classmethod
-    def _param_schema(cls):
-        return {
-            "lower_bound": {"type": "number"},
-            "upper_bound": {"type": "number"},
-            "mu": {"type": "number"},
-            "sigma": {"type": "number"},
-        }
-
-
-class ExponentialDistribution(CoreDistribution, ScipyDistribution, ContinuousDistribution):
-    """Exponential distribution for floating point type.
-
-    This class implements the exponential distribution with the rate as its
-    single parameter.
+    def __init__(self, re_list: Sequence[Union[BaseRegexElement, Tuple[str, float]]]):
+        super().__init__(re_list)
+        self.key_set: Set[str] = set()
+
+    def draw_reset(self):
+        self.key_set = set()
+
+    def draw(self) -> str:
+        n_try = 0
+        while n_try < 1e5:
+            new_val = super().draw()
+            if new_val not in self.key_set:
+                self.key_set.add(new_val)
+                return new_val
+            n_try += 1
+        raise ValueError("Failed to draw unique string after 100.000 tries.")
 
-    Parameters
-    ----------
-    rate: float
-        Rate of the exponential distribution. This is equal to 1/mean of the distribution.
-    """
-
-    implements = "core.exponential"
-    dist_class = expon
-
-    def __init__(self, rate: float):
-        self.par = {"rate": rate}
-        self.dist = expon(loc=0, scale=1/max(rate, 1e-8))
-
-    @classmethod
-    def _fit(cls, values):
-        values = values.filter(values > 0)
-        if len(values) == 0:
-            return cls.default_distribution()
-        return cls(rate=1/expon.fit(values, floc=0)[1])
-
-    @classmethod
-    def default_distribution(cls):
-        return cls(1.0)
-
-    @classmethod
-    def _param_schema(cls):
-        return {
-            "rate": {"type": "number"}
-        }
+    def information_criterion(self, values):
+        return 99999
```

### Comparing `metasynth-0.3.0/metasynth/distribution/datetime.py` & `metasynth-0.4.0/metasynth/distribution/datetime.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,17 +3,15 @@
 import datetime as dt
 from abc import abstractmethod
 from random import random
 from typing import Any, Dict
 
 import numpy as np
 
-from metasynth.distribution.base import (CoreDistribution, DateDistribution,
-                                         DateTimeDistribution,
-                                         ScipyDistribution, TimeDistribution)
+from metasynth.distribution.base import metadist, ScipyDistribution
 
 
 def convert_numpy_datetime(time_obj: np.datetime64) -> dt.datetime:
     """Convert numpy datetime to python stdlib datetime.
 
     Parameters
     ----------
@@ -110,19 +108,18 @@
         return {
             "start": self.start.isoformat(),
             "end": self.end.isoformat(),
             "precision": self.precision,
         }
 
 
-class UniformDateTimeDistribution(CoreDistribution, DateTimeDistribution, BaseUniformDistribution):
+@metadist(implements="core.uniform_datetime", var_type="datetime")
+class UniformDateTimeDistribution(BaseUniformDistribution):
     """Uniform DateTime distribution."""
 
-    implements = "core.uniform_datetime"
-
     def fromisoformat(self, dt_obj: str) -> dt.datetime:
         return dt.datetime.fromisoformat(dt_obj)
 
     @classmethod
     def default_distribution(cls):
         return cls("2022-07-15T10:39:36", "2022-08-15T10:39:36", precision="seconds")
 
@@ -131,19 +128,18 @@
         return {
             "start": {"type": "string"},
             "end": {"type": "string"},
             "precision": {"type": "string"},
         }
 
 
-class UniformTimeDistribution(CoreDistribution, TimeDistribution, BaseUniformDistribution):
+@metadist(implements="core.uniform_time", var_type="time")
+class UniformTimeDistribution(BaseUniformDistribution):
     """Uniform time distribution."""
 
-    implements = "core.uniform_time"
-
     def fromisoformat(self, dt_obj: str) -> dt.time:
         return dt.time.fromisoformat(dt_obj)
 
     @classmethod
     def default_distribution(cls):
         return cls("10:39:36", "18:39:36", precision="seconds")
 
@@ -158,18 +154,18 @@
         return {
             "start": {"type": "string"},
             "end": {"type": "string"},
             "precision": {"type": "string"},
         }
 
 
-class UniformDateDistribution(CoreDistribution, DateDistribution, BaseUniformDistribution):
+@metadist(implements="core.uniform_date", var_type="date")
+class UniformDateDistribution(BaseUniformDistribution):
     """Uniform date distribution."""
 
-    implements = "core.uniform_date"
     precision_possibilities = ["days"]
 
     def __init__(self, start: Any, end: Any):
         super().__init__(start, end, precision="days")
 
     def fromisoformat(self, dt_obj: str) -> dt.date:
         return dt.date.fromisoformat(dt_obj)
```

### Comparing `metasynth-0.3.0/metasynth/distribution/discrete.py` & `metasynth-0.4.0/metasynth/distribution/discrete.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 """Module with discrete distributions."""
 
 from typing import Set
 
 import numpy as np
 from scipy.stats import poisson, randint
 
-from metasynth.distribution.base import (CoreDistribution,
-                                         DiscreteDistribution,
+from metasynth.distribution.base import (metadist,
                                          ScipyDistribution)
 
 
-class DiscreteUniformDistribution(CoreDistribution, ScipyDistribution, DiscreteDistribution):
+@metadist(implements="core.discrete_uniform", var_type="discrete")
+class DiscreteUniformDistribution(ScipyDistribution):
     """Integer uniform distribution.
 
     It differs from the floating point uniform distribution by
     being a discrete distribution instead.
 
     Parameters
     ----------
     low: int
         Lower bound (inclusive) of the uniform distribution.
     high: int
         Upper bound (exclusive) of the uniform distribution.
     """
 
-    implements = "core.discrete_uniform"
     dist_class = randint
 
     def __init__(self, low: int, high: int):
         self.par = {"low": low, "high": high}
         self.dist = self.dist_class(low=low, high=high)
 
     def _information_criterion(self, values):
@@ -47,18 +46,18 @@
     def _param_schema(cls):
         return {
             "low": {"type": "integer"},
             "high": {"type": "integer"},
         }
 
 
-class PoissonDistribution(CoreDistribution, ScipyDistribution, DiscreteDistribution):
+@metadist(implements="core.poisson", var_type="discrete")
+class PoissonDistribution(ScipyDistribution):
     """Poisson distribution."""
 
-    implements = "core.poisson"
     dist_class = poisson
 
     def __init__(self, mu: float):
         self.par = {"mu": mu}
         self.dist = self.dist_class(mu=mu)
 
     def _information_criterion(self, values):
@@ -75,30 +74,28 @@
     @classmethod
     def _param_schema(cls):
         return {
             "mu": {"type": "number"},
         }
 
 
-class UniqueKeyDistribution(CoreDistribution, ScipyDistribution, DiscreteDistribution):
+@metadist(implements="core.unique_key", var_type="discrete", is_unique=True)
+class UniqueKeyDistribution(ScipyDistribution):
     """Integer distribution with unique keys.
 
     Discrete distribution that ensures the uniqueness of the drawn values.
 
     Parameters
     ----------
     low: int
         Minimum value for the keys.
     consecutive: int
         1 if keys are consecutive and increasing, 0 otherwise.
     """
 
-    implements = "core.unique_key"
-    is_unique = True
-
     def __init__(self, low: int, consecutive: int):
         self.par = {"low": low, "consecutive": consecutive}
         self.last_key = low - 1
         self.key_set: Set[int] = set()
 
     @classmethod
     def _fit(cls, values):
```

### Comparing `metasynth-0.3.0/metasynth/distribution/faker.py` & `metasynth-0.4.0/metasynth/distribution/faker.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """Module containing an interface to the faker package."""
 from typing import Iterable
 
 from faker import Faker
 
-from metasynth.distribution.base import CoreDistribution, StringDistribution
+from metasynth.distribution.base import metadist, BaseDistribution
 
 
-class FakerDistribution(CoreDistribution, StringDistribution):
+@metadist(implements="core.faker", var_type="string")
+class FakerDistribution(BaseDistribution):
     """Distribution for the faker package.
 
     This is mainly an interface for the faker package, so that it
     can be used within the MetaSynth package. It doesn't have any
     true fitting/statistical inference method, so it has to be manually
     selected.
 
@@ -18,16 +19,14 @@
     ----------
     faker_type: str
         The provider function in the faker package, e.g. 'city' or 'ipv4', etc.
     locale: str
         Locale used for the faker package.
     """
 
-    implements = "core.faker"
-
     def __init__(self, faker_type: str, locale: str = "en_US"):
         self.faker_type: str = faker_type
         self.locale: str = locale
         self.fake: Faker = Faker(locale=locale)
 
     @classmethod
     def _fit(cls, values, faker_type: str = "city", locale: str = "en_US"):  \
```

### Comparing `metasynth-0.3.0/metasynth/distribution/regex/element.py` & `metasynth-0.4.0/metasynth/distribution/regex/element.py`

 * *Files identical despite different names*

### Comparing `metasynth-0.3.0/metasynth/distribution/regex/optimizer.py` & `metasynth-0.4.0/metasynth/distribution/regex/optimizer.py`

 * *Files identical despite different names*

### Comparing `metasynth-0.3.0/metasynth/privacy.py` & `metasynth-0.4.0/metasynth/privacy.py`

 * *Files identical despite different names*

### Comparing `metasynth-0.3.0/metasynth/provider.py` & `metasynth-0.4.0/metasynth/provider.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     from importlib_metadata import entry_points, EntryPoint
 except ImportError:
     from importlib.metadata import entry_points, EntryPoint  # type: ignore
 
 import numpy as np
 import polars as pl
 
+from metasynth.distribution.na import NADistribution
 from metasynth.distribution.base import BaseDistribution
 from metasynth.distribution.categorical import MultinoulliDistribution
 from metasynth.distribution.continuous import (ExponentialDistribution,
                                                LogNormalDistribution,
                                                NormalDistribution,
                                                TruncatedNormalDistribution,
                                                UniformDistribution)
@@ -184,14 +185,16 @@
             Privacy level to find the best fit with.
 
         Returns
         -------
         BaseDistribution:
             Distribution fitted to the series.
         """
+        if len(series.drop_nulls()) == 0:
+            return NADistribution()
         dist_list = self._get_dist_list(privacy, var_type)
         if len(dist_list) == 0:
             raise ValueError(f"No available distributions with variable type: '{var_type}'")
         dist_instances = [d.fit(series, **privacy.fit_kwargs) for d in dist_list]
         dist_aic = [d.information_criterion(series) for d in dist_instances]
         i_best_dist = np.argmin(dist_aic)
         warnings.simplefilter("always")
@@ -224,15 +227,18 @@
             Type of privacy to be applied.
 
         Returns
         -------
         tuple[Type[BaseDistribution], dict[str, Any]]:
             A distribution and the arguments to create an instance.
         """
-        for dist_class in self._get_dist_list(privacy):
+        if NADistribution.matches_name(dist_name):
+            return NADistribution
+
+        for dist_class in self._get_dist_list(privacy) + [NADistribution]:
             if dist_class.matches_name(dist_name) and dist_class.privacy == privacy.name:
                 return dist_class
         raise ValueError(f"Cannot find distribution with name '{dist_name}'.")
 
     def _fit_distribution(self, series: pl.Series,
                           dist: Union[str, Type[BaseDistribution], BaseDistribution],
                           privacy: BasePrivacy,
@@ -254,27 +260,28 @@
 
         Returns
         -------
         BaseDistribution:
             Fitted distribution.
         """
         dist_instance = None
+        if isinstance(dist, BaseDistribution):
+            return dist
 
         if isinstance(dist, str):
             dist_class = self.find_distribution(dist, privacy=privacy)
-            dist_instance = dist_class.fit(series, **privacy.fit_kwargs, **fit_kwargs)
         elif inspect.isclass(dist) and issubclass(dist, BaseDistribution):
-            dist_instance = dist.fit(series, **privacy.fit_kwargs, **fit_kwargs)
-        if isinstance(dist, BaseDistribution):
-            dist_instance = dist
-
-        if dist_instance is None:
+            dist_class = dist
+        else:
             raise TypeError(
-                f"Distribution with type {type(dist)} is not a BaseDistribution")
-
+                f"Distribution {dist} with type {type(dist)} is not a BaseDistribution")
+        if issubclass(dist_class, NADistribution):
+            dist_instance = dist_class.default_distribution()
+        else:
+            dist_instance = dist_class.fit(series, **privacy.fit_kwargs, **fit_kwargs)
         return dist_instance
 
     def _get_dist_list(self, privacy: Optional[BasePrivacy] = None,
                        var_type: Optional[str] = None) -> list[type[BaseDistribution]]:
         dist_list = []
         for dist_provider in self.dist_packages:
             if var_type is None:
@@ -296,15 +303,15 @@
             Variable dictionary that includes the distribution properties.
 
         Returns
         -------
         BaseDistribution:
             Distribution representing the dictionary.
         """
-        for dist_class in self._get_dist_list(var_type=var_dict["type"]):
+        for dist_class in self._get_dist_list(var_type=var_dict["type"]) + [NADistribution]:
             if dist_class.implements == var_dict["distribution"]["implements"]:
                 return dist_class.from_dict(var_dict["distribution"])
         raise ValueError(f"Cannot find distribution with name "
                          f"'{var_dict['distribution']['implements']}'"
                          f"and type '{var_dict['type']}'.")
```

### Comparing `metasynth-0.3.0/metasynth/schema/generative_metadata_format.json` & `metasynth-0.4.0/metasynth/schema/generative_metadata_format.json`

 * *Files identical despite different names*

### Comparing `metasynth-0.3.0/metasynth/testutils.py` & `metasynth-0.4.0/metasynth/testutils.py`

 * *Files identical despite different names*

### Comparing `metasynth-0.3.0/metasynth/validation.py` & `metasynth-0.4.0/metasynth/validation.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,14 +8,16 @@
     from importlib_metadata import entry_points
 except ImportError:
     from importlib.metadata import entry_points  # type: ignore
 
 import jsonschema
 
 from metasynth.provider import get_distribution_provider
+from metasynth.distribution.na import NADistribution
+
 
 SCHEMA_BASE = {
     "$schema": "https://json-schema.org/draft/2020-12/schema",
     "$id": "http://sodascience.github.io/generative_metadata_format/core/1.0.0/generative_metadata_format",  # noqa # pylint: disable=line-too-long
     "type": "object",
     "properties": {
         "n_rows": {"type": "number"},
@@ -81,11 +83,12 @@
         Schema containing all the distributions in the distribution packages.
     """
     defs: list[dict] = []
     for package_name in packages:
         pkg = get_distribution_provider(package_name)
         for dist in pkg.distributions:
             defs.append(dist.schema())
+    defs.append(NADistribution.schema())
 
     schema = deepcopy(SCHEMA_BASE)
     schema.update({"$defs": {"all_dist_def": {"anyOf": defs}}})
     return schema
```

### Comparing `metasynth-0.3.0/metasynth/var.py` & `metasynth-0.4.0/metasynth/var.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,28 +58,36 @@
             self.name = name
             if dtype is not None:
                 self.dtype = dtype
         else:
             series = _to_polars(series)
             self.name = series.name
             if prop_missing is None:
-                self.prop_missing = (len(series) - len(series.drop_nulls()))/len(series)
+                self.prop_missing = (
+                    len(series) - len(series.drop_nulls())) / len(series)
             self.dtype = str(series.dtype)
 
         self.series = series
         self.distribution = distribution
         self.description = description
 
         if self.prop_missing is None:
             raise ValueError(f"Error while initializing variable {self.name}."
                              " prop_missing is None.")
+        if self.prop_missing < -1e-8 or self.prop_missing > 1+1e-8:
+            raise ValueError(f"Cannot create variable '{self.name}' with proportion missing "
+                             "outside range [0, 1]")
 
     @classmethod
-    def detect(cls, series_or_dataframe: Union[pd.Series, pl.Series, pl.DataFrame],
-               description: Optional[str] = None, prop_missing: Optional[float] = None):
+    def detect(cls,
+               series_or_dataframe: Union[pd.Series,
+                                          pl.Series,
+                                          pl.DataFrame],
+               description: Optional[str] = None,
+               prop_missing: Optional[float] = None):
         """Detect variable class(es) of series or dataframe.
 
         Parameters
         ----------
         series_or_dataframe: pd.Series or pd.Dataframe
             If the variable is a pandas Series, then find the correct
             variable type and create an instance of that variable.
@@ -122,15 +130,16 @@
             "time": "time",
             "str": "string",
             "categorical": "categorical"
         }
         try:
             return convert_dict[polars_dtype]
         except KeyError as exc:
-            raise ValueError(f"Unsupported polars type '{polars_dtype}") from exc
+            raise ValueError(
+                f"Unsupported polars type '{polars_dtype}") from exc
 
     def to_dict(self) -> Dict[str, Any]:
         """Create a dictionary from the variable."""
         if self.distribution is None:
             dist_dict = {}
         else:
             dist_dict = self.distribution.to_dict()
@@ -142,27 +151,37 @@
             "distribution": dist_dict,
         }
         if self.description is not None:
             var_dict["description"] = self.description
         return var_dict
 
     def __str__(self) -> str:
-        """Create a readable string from a variable."""
-        return str({
-            "name": self.name,
-            "description": self.description,
-            "type": self.var_type,
-            "dtype": self.dtype,
-            "prop_missing": self.prop_missing,
-            "distribution": str(self.distribution),
-        })
+        """Return an easy to read formatted string for the variable."""
+        description = f'Description: "{self.description}"\n' if self.description else ""
+
+        if self.distribution is None:
+            distribution_formatted = "No distribution information available"
+        else:
+            distribution_formatted = "\n".join(
+                "\t" + line for line in str(self.distribution).split("\n")
+            )
+
+        return (
+            f'"{self.name}"\n'
+            f'{description}'
+            f'- Variable Type: {self.var_type}\n'
+            f'- Data Type: {self.dtype}\n'
+            f'- Proportion of Missing Values: {self.prop_missing:.4f}\n'
+            f'- Distribution:\n{distribution_formatted}\n'
+        )
 
     def fit(self,  # pylint: disable=too-many-arguments
             dist: Optional[Union[str, BaseDistribution, type]] = None,
-            dist_providers: Union[str, type, BaseDistributionProvider] = "builtin",
+            dist_providers: Union[str, type,
+                                  BaseDistributionProvider] = "builtin",
             privacy: BasePrivacy = BasicPrivacy(),
             unique: Optional[bool] = None,
             fit_kwargs: Optional[dict] = None):
         """Fit distributions to the data.
 
         If multiple distributions are available for the current data type,
         use the one that fits the data the best.
@@ -189,16 +208,16 @@
             Extra options for distributions during the fitting stage.
         """
         if self.series is None:
             raise ValueError("Cannot fit distribution if we don't have the"
                              "original data.")
 
         provider_list = DistributionProviderList(dist_providers)
-        self.distribution = provider_list.fit(self.series, self.var_type, dist, privacy, unique,
-                                              fit_kwargs)
+        self.distribution = provider_list.fit(
+            self.series, self.var_type, dist, privacy, unique, fit_kwargs)
 
     def draw(self) -> Any:
         """Draw a random item for the variable in whatever type is required."""
         if self.distribution is None:
             raise ValueError("Cannot draw without distribution")
 
         # Return NA's -> None
```

### Comparing `metasynth-0.3.0/pyproject.toml` & `metasynth-0.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 [project.urls]
 GitHub = "https://github.com/sodascience/metasynth"
 documentation = "https://metasynth.readthedocs.io/en/latest/index.html"
 
 [project.optional-dependencies]
 test = [
 	"pytest", "pylint", "pydocstyle", "mypy", "flake8", "nbval",
-	"sphinx", "sphinx-rtd-theme", "sphinxcontrib-napoleon", "sphinx-autodoc-typehints"
+	"sphinx<7.0.0", "sphinx-rtd-theme", "sphinxcontrib-napoleon", "sphinx-autodoc-typehints", "sphinx_inline_tabs", "sphinx_copybutton"
 ]
 
 [project.entry-points."metasynth.distribution_provider"]
 builtin = "metasynth.provider:BuiltinDistributionProvider"
 
 [tool.setuptools]
 packages = ["metasynth"]
```

### Comparing `metasynth-0.3.0/tests/data/titanic.csv` & `metasynth-0.4.0/tests/data/titanic.csv`

 * *Files identical despite different names*

### Comparing `metasynth-0.3.0/tests/test_builtin.py` & `metasynth-0.4.0/tests/test_builtin.py`

 * *Files identical despite different names*

### Comparing `metasynth-0.3.0/tests/test_continuous.py` & `metasynth-0.4.0/tests/test_continuous.py`

 * *Files identical despite different names*

### Comparing `metasynth-0.3.0/tests/test_dataset.py` & `metasynth-0.4.0/tests/test_dataset.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 import pytest
 import pandas as pd
 import polars as pl
 from pytest import mark
 
-from metasynth.dataset import MetaDataset
+from metasynth.dataset import MetaFrame
 from metasynth.var import MetaVar
 from metasynth.provider import get_distribution_provider
 
 
 dtypes = {
     "PassengerId": "int",
     "Survived": "category",
@@ -37,15 +37,15 @@
 
 
 @mark.parametrize("dataframe_lib", ["polars", "pandas"])
 def test_dataset(tmp_path, dataframe_lib):
     titanic_fp = Path("tests", "data", "titanic.csv")
     tmp_fp = tmp_path / "tmp.json"
     df = _read_csv(titanic_fp, dataframe_lib)
-    dataset = MetaDataset.from_dataframe(
+    dataset = MetaFrame.fit_dataframe(
         df,
         spec={
                 "Name": {"prop_missing": 0.5},
                 "Ticket": {"description": "test_description"},
                 "Fare": {"distribution": "normal"},
                 "PassengerId": {"unique": True},
              })
@@ -69,15 +69,15 @@
         with pytest.raises(TypeError):
             dataset[MetaVar]
 
         assert "Rows" in str(dataset)
 
     check_dataset(dataset)
     dataset.to_json(tmp_fp)
-    dataset = MetaDataset.from_json(tmp_fp)
+    dataset = MetaFrame.from_json(tmp_fp)
     check_dataset(dataset)
 
     dataset.descriptions = {"Embarked": "Some description", "Sex": "Other description"}
     assert dataset.descriptions["Embarked"] == "Some description"
     with pytest.raises(AssertionError):
         dataset.descriptions = "12345"
     dataset.descriptions = {"Embarked": "New description"}
@@ -88,18 +88,22 @@
     else:
         col_names = list(df)
     dataset.descriptions = col_names
     for name in col_names:
         print(name, dataset.descriptions[name])
         assert dataset.descriptions[name] == name
 
+    # Check whether non-columns raise an error
+    with pytest.raises(ValueError):
+        dataset = MetaFrame.fit_dataframe(df, spec={"unicorn": {"prop_missing": 0.5}})
+
 
 def test_distributions(tmp_path):
     tmp_fp = tmp_path / "tmp.json"
 
     provider = get_distribution_provider()
     for var_type in provider.all_var_types:
         for dist in provider.get_dist_list(var_type):
             var = MetaVar(var_type, name="None", distribution=dist.default_distribution(),
                           prop_missing=random())
-            dataset = MetaDataset([var], n_rows=10)
+            dataset = MetaFrame([var], n_rows=10)
             dataset.to_json(tmp_fp)
```

### Comparing `metasynth-0.3.0/tests/test_datetime.py` & `metasynth-0.4.0/tests/test_datetime.py`

 * *Files identical despite different names*

### Comparing `metasynth-0.3.0/tests/test_discrete.py` & `metasynth-0.4.0/tests/test_discrete.py`

 * *Files identical despite different names*

### Comparing `metasynth-0.3.0/tests/test_distribution.py` & `metasynth-0.4.0/tests/test_distribution.py`

 * *Files identical despite different names*

### Comparing `metasynth-0.3.0/tests/test_regex.py` & `metasynth-0.4.0/tests/test_regex.py`

 * *Files 11% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     def check_regex_dist(dist):
         assert len(dist.re_list) == 2
         assert isinstance(dist.re_list[0], SingleRegex)
         assert isinstance(dist.re_list[1], DigitRegex)
         assert dist.re_list[0].character_selection == ["R"]
         assert dist.re_list[1].min_digit == 3
         assert dist.re_list[1].max_digit == 3
-        assert str(dist) == r"[R]\d{3,3}"
+        assert dist.regex_string == r"[R]\d{3,3}"
 
         for draw_str in [dist.draw() for _ in range(10)]:
             assert len(draw_str) == 4
             assert draw_str[0] == "R"
 
     check_regex_dist(dist)
 
@@ -92,15 +92,15 @@
     assert len(dist.re_list) == 1
     assert isinstance(dist.re_list[0], dist_class)
     assert dist.re_list[0].min_digit == n_digits
     assert dist.re_list[0].max_digit == n_digits
     assert dist.to_dict()["parameters"]["re_list"][0][0] == regex_str
     assert np.all([len(dist.draw()) == n_digits for _ in range(100)])
     assert np.all([c in digit_set for c in dist.draw()])
-    new_dist = dist_class.from_string(str(dist), 1.0)[0]
+    new_dist = dist_class.from_string(dist.regex_string, 1.0)[0]
     with raises(ValueError):
-        dist_class.from_string(str(dist), 3)[0]
+        dist_class.from_string(dist.regex_string, 3)[0]
     assert isinstance(new_dist, dist_class)
     assert new_dist.min_digit == dist.re_list[0].min_digit
     assert new_dist.max_digit == dist.re_list[0].max_digit
```

### Comparing `metasynth-0.3.0/tests/test_var.py` & `metasynth-0.4.0/tests/test_var.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         if type(series_a) == type(series_b):
             assert base_type_a == base_type_b
         assert (len(series_a)-len(_series_drop_nans(series_a)) > 0) == (len(series_b) - len(_series_drop_nans(series_b)) > 0)
 
     assert isinstance(series, (pd.Series, pl.Series))
     var = MetaVar.detect(series)
     assert isinstance(str(var), str)
-    assert "prop_missing" in str(var)
+    assert "Proportion of Missing Values" in str(var)
 
     with raises(ValueError):
         var.draw_series(100)
     var.fit()
     new_series = var.draw_series(len(series))
     check_similar(series, new_series)
     assert var.var_type == var_type
@@ -149,14 +149,25 @@
 def test_bool(tmp_path, series_type):
     series = series_type(np.random.choice([True, False], size=100))
     with raises(ValueError):
         check_var(series, "categorical", tmp_path)
 
 
 @mark.parametrize(
+    "prop_missing",
+    [-1, -0.1, 1.2],
+)
+def test_invalid_prop(prop_missing):
+    with raises(ValueError):
+        MetaVar("continuous")
+    with raises(ValueError):
+        MetaVar("continuous", prop_missing=prop_missing)
+
+
+@mark.parametrize(
     "dataframe",
     [
         pd.DataFrame({
             "int": pd.Series([np.random.randint(0, 10) for _ in range(100)]),
             "float": pd.Series([np.random.rand() for _ in range(100)])
         }),
         pl.DataFrame({
```

