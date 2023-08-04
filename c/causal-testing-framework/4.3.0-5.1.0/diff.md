# Comparing `tmp/causal_testing_framework-4.3.0.tar.gz` & `tmp/causal_testing_framework-5.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "causal_testing_framework-4.3.0.tar", last modified: Tue Jul 11 10:18:34 2023, max compression
+gzip compressed data, was "causal_testing_framework-5.1.0.tar", last modified: Fri Aug  4 13:19:01 2023, max compression
```

## Comparing `causal_testing_framework-4.3.0.tar` & `causal_testing_framework-5.1.0.tar`

### file list

```diff
@@ -1,163 +1,164 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:18:34.880614 causal_testing_framework-4.3.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:18:34.864614 causal_testing_framework-4.3.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/.github/CONTRIBUTING.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:18:34.864614 causal_testing_framework-4.3.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:18:34.864614 causal_testing_framework-4.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/.github/workflows/ci-tests.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/.github/workflows/lint-format.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/.github/workflows/publish-to-pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/.mega-linter.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    20375 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-07-11 10:18:34.880614 causal_testing_framework-4.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:18:34.864614 causal_testing_framework-4.3.0/causal_testing/
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/causal_testing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:18:34.864614 causal_testing_framework-4.3.0/causal_testing/data_collection/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/causal_testing/data_collection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6772 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/causal_testing/data_collection/data_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:18:34.864614 causal_testing_framework-4.3.0/causal_testing/generation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/causal_testing/generation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12764 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/causal_testing/generation/abstract_causal_test_case.py
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/causal_testing/generation/enum_gen.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:18:34.864614 causal_testing_framework-4.3.0/causal_testing/json_front/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/causal_testing/json_front/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20247 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/causal_testing/json_front/json_class.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:18:34.864614 causal_testing_framework-4.3.0/causal_testing/specification/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/causal_testing/specification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26885 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/causal_testing/specification/causal_dag.py
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/causal_testing/specification/causal_specification.py
--rw-r--r--   0 runner    (1001) docker     (123)    11932 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/causal_testing/specification/metamorphic_relation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5752 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/causal_testing/specification/scenario.py
--rw-r--r--   0 runner    (1001) docker     (123)     9665 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/causal_testing/specification/variable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:18:34.868614 causal_testing_framework-4.3.0/causal_testing/testing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/causal_testing/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/causal_testing/testing/base_test_case.py
--rw-r--r--   0 runner    (1001) docker     (123)     3894 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/causal_testing/testing/causal_test_case.py
--rw-r--r--   0 runner    (1001) docker     (123)    13499 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/causal_testing/testing/causal_test_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     4792 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/causal_testing/testing/causal_test_outcome.py
--rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/causal_testing/testing/causal_test_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/causal_testing/testing/causal_test_suite.py
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/causal_testing/testing/effect.py
--rw-r--r--   0 runner    (1001) docker     (123)    29865 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/causal_testing/testing/estimators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/causal_testing/testing/intervention.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:18:34.868614 causal_testing_framework-4.3.0/causal_testing/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/causal_testing/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/causal_testing/utils/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:18:34.868614 causal_testing_framework-4.3.0/causal_testing_framework.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-07-11 10:18:34.000000 causal_testing_framework-4.3.0/causal_testing_framework.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4685 2023-07-11 10:18:34.000000 causal_testing_framework-4.3.0/causal_testing_framework.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 10:18:34.000000 causal_testing_framework-4.3.0/causal_testing_framework.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-11 10:18:34.000000 causal_testing_framework-4.3.0/causal_testing_framework.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-11 10:18:34.000000 causal_testing_framework-4.3.0/causal_testing_framework.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:18:34.868614 causal_testing_framework-4.3.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/docs/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:18:34.868614 causal_testing_framework-4.3.0/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5424 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/docs/source/description.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:18:34.868614 causal_testing_framework-4.3.0/docs/source/dev/
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/docs/source/dev/actions_and_webhooks.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/docs/source/dev/documentation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/docs/source/dev/version_release.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:18:34.868614 causal_testing_framework-4.3.0/docs/source/frontends/
--rw-r--r--   0 runner    (1001) docker     (123)     4247 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/docs/source/frontends/json_front_end.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/docs/source/frontends/test_suite.rst
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/docs/source/glossary.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:18:34.868614 causal_testing_framework-4.3.0/docs/source/images/
--rw-r--r--   0 runner    (1001) docker     (123)   184134 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/docs/source/images/workflow.png
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/docs/source/installation.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:18:34.872614 causal_testing_framework-4.3.0/docs/source/modules/
--rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/docs/source/modules/causal_specification.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5629 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/docs/source/modules/causal_tests.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/docs/source/modules/data_collector.rst
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/docs/source/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6429 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/docs/source/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:18:34.872614 causal_testing_framework-4.3.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/examples/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:18:34.860614 causal_testing_framework-4.3.0/examples/covasim_/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:18:34.872614 causal_testing_framework-4.3.0/examples/covasim_/doubling_beta/
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/examples/covasim_/doubling_beta/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/examples/covasim_/doubling_beta/dag.dot
--rw-r--r--   0 runner    (1001) docker     (123)    24596 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/examples/covasim_/doubling_beta/dag.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:18:34.872614 causal_testing_framework-4.3.0/examples/covasim_/doubling_beta/data/
--rw-r--r--   0 runner    (1001) docker     (123)  1355776 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/examples/covasim_/doubling_beta/data/10k_observational_data.csv
--rw-r--r--   0 runner    (1001) docker     (123)    15697 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/examples/covasim_/doubling_beta/example_beta.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:18:34.872614 causal_testing_framework-4.3.0/examples/covasim_/vaccinating_elderly/
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/examples/covasim_/vaccinating_elderly/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/examples/covasim_/vaccinating_elderly/dag.dot
--rw-r--r--   0 runner    (1001) docker     (123)    23290 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/examples/covasim_/vaccinating_elderly/dag.png
--rw-r--r--   0 runner    (1001) docker     (123)    11838 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/examples/covasim_/vaccinating_elderly/example_vaccine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:18:34.872614 causal_testing_framework-4.3.0/examples/lr91/
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/examples/lr91/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/examples/lr91/dag.dot
--rw-r--r--   0 runner    (1001) docker     (123)    73886 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/examples/lr91/dag.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:18:34.872614 causal_testing_framework-4.3.0/examples/lr91/data/
--rw-r--r--   0 runner    (1001) docker     (123)    40715 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/examples/lr91/data/normalised_results.csv
--rw-r--r--   0 runner    (1001) docker     (123)    40686 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/examples/lr91/data/results.csv
--rw-r--r--   0 runner    (1001) docker     (123)     8820 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/examples/lr91/example_max_conductances.py
--rw-r--r--   0 runner    (1001) docker     (123)     8582 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/examples/lr91/example_max_conductances_test_suite.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:18:34.876613 causal_testing_framework-4.3.0/examples/poisson/
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/examples/poisson/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     7603 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/examples/poisson/causal_tests.json
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/examples/poisson/dag.dot
--rw-r--r--   0 runner    (1001) docker     (123)    61017 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/examples/poisson/data.csv
--rw-r--r--   0 runner    (1001) docker     (123)     7307 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/examples/poisson/example_run_causal_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:18:34.876613 causal_testing_framework-4.3.0/examples/poisson-line-process/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/examples/poisson-line-process/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/examples/poisson-line-process/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/examples/poisson-line-process/dag.dot
--rw-r--r--   0 runner    (1001) docker     (123)    53765 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/examples/poisson-line-process/dag.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:18:34.860614 causal_testing_framework-4.3.0/examples/poisson-line-process/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:18:34.876613 causal_testing_framework-4.3.0/examples/poisson-line-process/data/random/
--rw-r--r--   0 runner    (1001) docker     (123)   102007 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/examples/poisson-line-process/data/random/data_random_1000.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:18:34.876613 causal_testing_framework-4.3.0/examples/poisson-line-process/data/smt_100/
--rw-r--r--   0 runner    (1001) docker     (123)    15080 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/examples/poisson-line-process/data/smt_100/data_smt_wh10_100.csv
--rw-r--r--   0 runner    (1001) docker     (123)    12100 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/examples/poisson-line-process/data/smt_100/data_smt_wh1_100.csv
--rw-r--r--   0 runner    (1001) docker     (123)    12945 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/examples/poisson-line-process/data/smt_100/data_smt_wh2_100.csv
--rw-r--r--   0 runner    (1001) docker     (123)    24851 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/examples/poisson-line-process/data/smt_100/data_smt_wh3_100.csv
--rw-r--r--   0 runner    (1001) docker     (123)    14925 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/examples/poisson-line-process/data/smt_100/data_smt_wh4_100.csv
--rw-r--r--   0 runner    (1001) docker     (123)    13682 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/examples/poisson-line-process/data/smt_100/data_smt_wh5_100.csv
--rw-r--r--   0 runner    (1001) docker     (123)    25451 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/examples/poisson-line-process/data/smt_100/data_smt_wh6_100.csv
--rw-r--r--   0 runner    (1001) docker     (123)    26544 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/examples/poisson-line-process/data/smt_100/data_smt_wh7_100.csv
--rw-r--r--   0 runner    (1001) docker     (123)    17103 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/examples/poisson-line-process/data/smt_100/data_smt_wh8_100.csv
--rw-r--r--   0 runner    (1001) docker     (123)    26889 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/examples/poisson-line-process/data/smt_100/data_smt_wh9_100.csv
--rw-r--r--   0 runner    (1001) docker     (123)     9067 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/examples/poisson-line-process/example_poisson_process.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:18:34.876613 causal_testing_framework-4.3.0/images/
--rw-r--r--   0 runner    (1001) docker     (123)   184134 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/images/workflow.png
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 10:18:34.880614 causal_testing_framework-4.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:18:34.876613 causal_testing_framework-4.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:18:34.876613 causal_testing_framework-4.3.0/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)   374288 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/tests/data/nhefs.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:18:34.876613 causal_testing_framework-4.3.0/tests/data_collection_tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3322 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/tests/data_collection_tests/test_observational_data_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:18:34.876613 causal_testing_framework-4.3.0/tests/generation_tests/
--rw-r--r--   0 runner    (1001) docker     (123)     8842 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/tests/generation_tests/test_abstract_test_case.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:18:34.876613 causal_testing_framework-4.3.0/tests/json_front_tests/
--rw-r--r--   0 runner    (1001) docker     (123)    13172 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/tests/json_front_tests/test_json_class.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:18:34.864614 causal_testing_framework-4.3.0/tests/resources/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:18:34.880614 causal_testing_framework-4.3.0/tests/resources/data/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/tests/resources/data/dag.dot
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/tests/resources/data/data.csv
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/tests/resources/data/data_with_meta.csv
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/tests/resources/data/tests.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:18:34.880614 causal_testing_framework-4.3.0/tests/specification_tests/
--rw-r--r--   0 runner    (1001) docker     (123)    18020 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/tests/specification_tests/test_causal_dag.py
--rw-r--r--   0 runner    (1001) docker     (123)    13830 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/tests/specification_tests/test_metamorphic_relations.py
--rw-r--r--   0 runner    (1001) docker     (123)     5819 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/tests/specification_tests/test_variable.py
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/tests/test_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:18:34.880614 causal_testing_framework-4.3.0/tests/testing_tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/tests/testing_tests/test_causal_test_case.py
--rw-r--r--   0 runner    (1001) docker     (123)    13931 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/tests/testing_tests/test_causal_test_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)    10472 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/tests/testing_tests/test_causal_test_outcome.py
--rw-r--r--   0 runner    (1001) docker     (123)     6275 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/tests/testing_tests/test_causal_test_suite.py
--rw-r--r--   0 runner    (1001) docker     (123)    19261 2023-07-11 10:17:42.000000 causal_testing_framework-4.3.0/tests/testing_tests/test_estimators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:19:01.874665 causal_testing_framework-5.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:19:01.846664 causal_testing_framework-5.1.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/.github/CONTRIBUTING.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:19:01.846664 causal_testing_framework-5.1.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:19:01.846664 causal_testing_framework-5.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/.github/workflows/ci-tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/.github/workflows/lint-format.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/.github/workflows/publish-to-pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/.mega-linter.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    20375 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-08-04 13:19:01.874665 causal_testing_framework-5.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:19:01.850664 causal_testing_framework-5.1.0/causal_testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/causal_testing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:19:01.850664 causal_testing_framework-5.1.0/causal_testing/data_collection/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/causal_testing/data_collection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7047 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/causal_testing/data_collection/data_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:19:01.850664 causal_testing_framework-5.1.0/causal_testing/generation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/causal_testing/generation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12764 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/causal_testing/generation/abstract_causal_test_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/causal_testing/generation/enum_gen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:19:01.850664 causal_testing_framework-5.1.0/causal_testing/json_front/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/causal_testing/json_front/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20352 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/causal_testing/json_front/json_class.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:19:01.850664 causal_testing_framework-5.1.0/causal_testing/specification/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/causal_testing/specification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26885 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/causal_testing/specification/causal_dag.py
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/causal_testing/specification/causal_specification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11959 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/causal_testing/specification/metamorphic_relation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5752 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/causal_testing/specification/scenario.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9665 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/causal_testing/specification/variable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:19:01.854664 causal_testing_framework-5.1.0/causal_testing/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/causal_testing/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/causal_testing/testing/base_test_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4189 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/causal_testing/testing/causal_test_adequacy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5460 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/causal_testing/testing/causal_test_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5224 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/causal_testing/testing/causal_test_outcome.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4671 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/causal_testing/testing/causal_test_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/causal_testing/testing/causal_test_suite.py
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/causal_testing/testing/effect.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28237 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/causal_testing/testing/estimators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/causal_testing/testing/intervention.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:19:01.854664 causal_testing_framework-5.1.0/causal_testing/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/causal_testing/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/causal_testing/utils/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:19:01.854664 causal_testing_framework-5.1.0/causal_testing_framework.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-08-04 13:19:01.000000 causal_testing_framework-5.1.0/causal_testing_framework.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4736 2023-08-04 13:19:01.000000 causal_testing_framework-5.1.0/causal_testing_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 13:19:01.000000 causal_testing_framework-5.1.0/causal_testing_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-08-04 13:19:01.000000 causal_testing_framework-5.1.0/causal_testing_framework.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-04 13:19:01.000000 causal_testing_framework-5.1.0/causal_testing_framework.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:19:01.854664 causal_testing_framework-5.1.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:19:01.854664 causal_testing_framework-5.1.0/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5424 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/docs/source/description.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:19:01.858664 causal_testing_framework-5.1.0/docs/source/dev/
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/docs/source/dev/actions_and_webhooks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/docs/source/dev/documentation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/docs/source/dev/version_release.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:19:01.858664 causal_testing_framework-5.1.0/docs/source/frontends/
+-rw-r--r--   0 runner    (1001) docker     (123)     4247 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/docs/source/frontends/json_front_end.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/docs/source/frontends/test_suite.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/docs/source/glossary.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:19:01.858664 causal_testing_framework-5.1.0/docs/source/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   184134 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/docs/source/images/workflow.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/docs/source/installation.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:19:01.858664 causal_testing_framework-5.1.0/docs/source/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/docs/source/modules/causal_specification.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5629 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/docs/source/modules/causal_tests.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/docs/source/modules/data_collector.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/docs/source/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6429 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/docs/source/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:19:01.858664 causal_testing_framework-5.1.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/examples/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:19:01.842663 causal_testing_framework-5.1.0/examples/covasim_/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:19:01.858664 causal_testing_framework-5.1.0/examples/covasim_/doubling_beta/
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/examples/covasim_/doubling_beta/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/examples/covasim_/doubling_beta/dag.dot
+-rw-r--r--   0 runner    (1001) docker     (123)    24596 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/examples/covasim_/doubling_beta/dag.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:19:01.858664 causal_testing_framework-5.1.0/examples/covasim_/doubling_beta/data/
+-rw-r--r--   0 runner    (1001) docker     (123)  1355776 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/examples/covasim_/doubling_beta/data/10k_observational_data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    15562 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/examples/covasim_/doubling_beta/example_beta.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:19:01.862664 causal_testing_framework-5.1.0/examples/covasim_/vaccinating_elderly/
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/examples/covasim_/vaccinating_elderly/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/examples/covasim_/vaccinating_elderly/dag.dot
+-rw-r--r--   0 runner    (1001) docker     (123)    23290 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/examples/covasim_/vaccinating_elderly/dag.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11636 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/examples/covasim_/vaccinating_elderly/example_vaccine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:19:01.862664 causal_testing_framework-5.1.0/examples/lr91/
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/examples/lr91/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/examples/lr91/dag.dot
+-rw-r--r--   0 runner    (1001) docker     (123)    73886 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/examples/lr91/dag.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:19:01.862664 causal_testing_framework-5.1.0/examples/lr91/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    40715 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/examples/lr91/data/normalised_results.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    40686 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/examples/lr91/data/results.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     8600 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/examples/lr91/example_max_conductances.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8374 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/examples/lr91/example_max_conductances_test_suite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:19:01.866665 causal_testing_framework-5.1.0/examples/poisson/
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/examples/poisson/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7603 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/examples/poisson/causal_tests.json
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/examples/poisson/dag.dot
+-rw-r--r--   0 runner    (1001) docker     (123)    61017 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/examples/poisson/data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     7330 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/examples/poisson/example_run_causal_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:19:01.866665 causal_testing_framework-5.1.0/examples/poisson-line-process/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/examples/poisson-line-process/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/examples/poisson-line-process/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/examples/poisson-line-process/dag.dot
+-rw-r--r--   0 runner    (1001) docker     (123)    53765 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/examples/poisson-line-process/dag.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:19:01.842663 causal_testing_framework-5.1.0/examples/poisson-line-process/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:19:01.866665 causal_testing_framework-5.1.0/examples/poisson-line-process/data/random/
+-rw-r--r--   0 runner    (1001) docker     (123)   102007 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/examples/poisson-line-process/data/random/data_random_1000.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:19:01.870665 causal_testing_framework-5.1.0/examples/poisson-line-process/data/smt_100/
+-rw-r--r--   0 runner    (1001) docker     (123)    15080 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/examples/poisson-line-process/data/smt_100/data_smt_wh10_100.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    12100 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/examples/poisson-line-process/data/smt_100/data_smt_wh1_100.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    12945 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/examples/poisson-line-process/data/smt_100/data_smt_wh2_100.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    24851 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/examples/poisson-line-process/data/smt_100/data_smt_wh3_100.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    14925 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/examples/poisson-line-process/data/smt_100/data_smt_wh4_100.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    13682 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/examples/poisson-line-process/data/smt_100/data_smt_wh5_100.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    25451 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/examples/poisson-line-process/data/smt_100/data_smt_wh6_100.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    26544 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/examples/poisson-line-process/data/smt_100/data_smt_wh7_100.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    17103 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/examples/poisson-line-process/data/smt_100/data_smt_wh8_100.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    26889 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/examples/poisson-line-process/data/smt_100/data_smt_wh9_100.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     8856 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/examples/poisson-line-process/example_poisson_process.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:19:01.870665 causal_testing_framework-5.1.0/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   184134 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/images/workflow.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 13:19:01.874665 causal_testing_framework-5.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:19:01.870665 causal_testing_framework-5.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:19:01.870665 causal_testing_framework-5.1.0/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   374288 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/tests/data/nhefs.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:19:01.870665 causal_testing_framework-5.1.0/tests/data_collection_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/tests/data_collection_tests/test_observational_data_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:19:01.870665 causal_testing_framework-5.1.0/tests/generation_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     8842 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/tests/generation_tests/test_abstract_test_case.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:19:01.870665 causal_testing_framework-5.1.0/tests/json_front_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    13013 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/tests/json_front_tests/test_json_class.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:19:01.846664 causal_testing_framework-5.1.0/tests/resources/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:19:01.870665 causal_testing_framework-5.1.0/tests/resources/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/tests/resources/data/dag.dot
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/tests/resources/data/data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/tests/resources/data/data_with_categorical.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/tests/resources/data/data_with_meta.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/tests/resources/data/tests.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:19:01.870665 causal_testing_framework-5.1.0/tests/specification_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    17985 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/tests/specification_tests/test_causal_dag.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13861 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/tests/specification_tests/test_metamorphic_relations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5819 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/tests/specification_tests/test_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/tests/test_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:19:01.874665 causal_testing_framework-5.1.0/tests/testing_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6840 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/tests/testing_tests/test_causal_test_adequacy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12320 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/tests/testing_tests/test_causal_test_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10683 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/tests/testing_tests/test_causal_test_outcome.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5782 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/tests/testing_tests/test_causal_test_suite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19315 2023-08-04 13:17:52.000000 causal_testing_framework-5.1.0/tests/testing_tests/test_estimators.py
```

### Comparing `causal_testing_framework-4.3.0/.github/CONTRIBUTING.md` & `causal_testing_framework-5.1.0/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.3.0/.github/ISSUE_TEMPLATE/bug_report.md` & `causal_testing_framework-5.1.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.3.0/.github/ISSUE_TEMPLATE/feature_request.md` & `causal_testing_framework-5.1.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.3.0/.github/workflows/ci-tests.yaml` & `causal_testing_framework-5.1.0/.github/workflows/ci-tests.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -18,17 +18,16 @@
       - name: Set up Python using Miniconda
         uses: conda-incubator/setup-miniconda@v2
         with:
           auto-update-conda: true
           python-version: ${{ matrix.python-version }}
       - name: Install package and dependencies
         run: |
-          conda install -c conda-forge pygraphviz
           python --version
-          pip install -e . --no-cache-dir
+          pip install -e .
           pip install -e .[test]
           pip install pytest pytest-cov
         shell: bash -l {0}
       - name: Test with pytest
         run: |
           pytest --cov=causal_testing --cov-report=xml
         shell: bash -l {0}
```

### Comparing `causal_testing_framework-4.3.0/.github/workflows/lint-format.yaml` & `causal_testing_framework-5.1.0/.github/workflows/lint-format.yaml`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.3.0/.github/workflows/publish-to-pypi.yaml` & `causal_testing_framework-5.1.0/.github/workflows/publish-to-pypi.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         uses: actions/setup-python@v3
         with:
           python-version: 3.9
       - name: Installing package
         run: |
           pip3 install .
           pip3 install .[pypi]
-          pip3 install build
+          pip3 install build wheel
           pip3 install setuptools --upgrade
           pip3 install setuptools_scm
       - name: Build Package
         run: |
           python -m build --no-isolation
       - name: Publish package to PyPI
         uses: pypa/gh-action-pypi-publish@release/v1
```

### Comparing `causal_testing_framework-4.3.0/.gitignore` & `causal_testing_framework-5.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.3.0/.pylintrc` & `causal_testing_framework-5.1.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.3.0/.readthedocs.yaml` & `causal_testing_framework-5.1.0/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.3.0/LICENSE` & `causal_testing_framework-5.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.3.0/PKG-INFO` & `causal_testing_framework-5.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: causal_testing_framework
-Version: 4.3.0
+Version: 5.1.0
 Summary: A framework for causal testing using causal directed acyclic graphs.
 Author: The CITCOM team
 License: MIT
 Project-URL: Bug_Tracker, https://github.com/CITCOM-project/CausalTestingFramework/issues
 Project-URL: Documentation, https://causal-testing-framework.readthedocs.io/
 Project-URL: Source, https://github.com/CITCOM-project/CausalTestingFramework
 Keywords: causal inference,verification
```

### Comparing `causal_testing_framework-4.3.0/README.md` & `causal_testing_framework-5.1.0/README.md`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.3.0/causal_testing/data_collection/data_collector.py` & `causal_testing_framework-5.1.0/causal_testing/data_collection/data_collector.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,23 +44,29 @@
             set(data.columns)
         ):
             missing_variables = scenario_variables - set(data.columns)
             raise IndexError(
                 f"Missing columns: missing data for variables {missing_variables}. Should they be marked as hidden?"
             )
 
+        # Quick out if we don't have any constraints
+        if len(self.scenario.constraints) == 0:
+            return data
+
         # For each row, does it satisfy the constraints?
         solver = z3.Solver()
         for c in self.scenario.constraints:
             solver.assert_and_track(c, f"background: {c}")
         sat = []
         unsat_core = None
         for _, row in data.iterrows():
             solver.push()
+            # Check that the row does not violate any scenario constraints
             # Need to explicitly cast variables to their specified type. Z3 will not take e.g. np.int64 to be an int.
+            # Check that the row does not violate any scenario constraints
             model = [
                 self.scenario.variables[var].z3
                 == self.scenario.variables[var].z3_val(self.scenario.variables[var].z3, row[var])
                 for var in self.scenario.variables
                 if var in row and not pd.isnull(row[var])
             ]
             for c in model:
@@ -140,15 +146,14 @@
         """Read a pandas dataframe and filter to remove
         any data which is invalid for the scenario-under-test.
 
         Data is invalid if it does not meet the constraints outlined in the scenario-under-test (Scenario).
 
         :return: A pandas dataframe containing execution data that is valid for the scenario-under-test.
         """
-
         execution_data_df = self.data
         for meta in self.scenario.metas():
             if meta.name not in self.data:
                 meta.populate(execution_data_df)
         scenario_execution_data_df = self.filter_valid_data(execution_data_df)
         for var_name, var in self.scenario.variables.items():
             if issubclass(var.datatype, Enum):
```

### Comparing `causal_testing_framework-4.3.0/causal_testing/generation/abstract_causal_test_case.py` & `causal_testing_framework-5.1.0/causal_testing/generation/abstract_causal_test_case.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.3.0/causal_testing/generation/enum_gen.py` & `causal_testing_framework-5.1.0/causal_testing/generation/enum_gen.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.3.0/causal_testing/json_front/json_class.py` & `causal_testing_framework-5.1.0/causal_testing/json_front/json_class.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """This module contains the JsonUtility class, details of using this class can be found here:
 https://causal-testing-framework.readthedocs.io/en/latest/json_front_end.html"""
 
 import argparse
 import json
 import logging
 
-from collections.abc import Iterable, Mapping
+from collections.abc import Mapping
 from dataclasses import dataclass
 from pathlib import Path
 from statistics import StatisticsError
 
 import pandas as pd
 import scipy
 from fitter import Fitter, get_common_distributions
@@ -18,17 +18,17 @@
 from causal_testing.generation.abstract_causal_test_case import AbstractCausalTestCase
 from causal_testing.specification.causal_dag import CausalDAG
 from causal_testing.specification.causal_specification import CausalSpecification
 from causal_testing.specification.scenario import Scenario
 from causal_testing.specification.variable import Input, Meta, Output
 from causal_testing.testing.causal_test_case import CausalTestCase
 from causal_testing.testing.causal_test_result import CausalTestResult
-from causal_testing.testing.causal_test_engine import CausalTestEngine
 from causal_testing.testing.estimators import Estimator
 from causal_testing.testing.base_test_case import BaseTestCase
+from causal_testing.testing.causal_test_adequacy import DataAdequacy
 
 logger = logging.getLogger(__name__)
 
 
 class JsonUtility:
     """
     The JsonUtility Class provides the functionality to use structured JSON to setup and run causal tests on the
@@ -45,59 +45,60 @@
     :attr {Scenario} scenario:
     :attr {CausalSpecification} causal_specification:
     """
 
     def __init__(self, output_path: str, output_overwrite: bool = False):
         self.input_paths = None
         self.variables = {"inputs": {}, "outputs": {}, "metas": {}}
-        self.data = []
         self.test_plan = None
         self.scenario = None
         self.causal_specification = None
         self.output_path = Path(output_path)
         self.check_file_exists(self.output_path, output_overwrite)
+        self.data_collector = None
 
     def set_paths(self, json_path: str, dag_path: str, data_paths: list[str] = None):
         """
         Takes a path of the directory containing all scenario specific files and creates individual paths for each file
         :param json_path: string path representation to .json file containing test specifications
         :param dag_path: string path representation to the .dot file containing the Causal DAG
         :param data_paths: string path representation to the data files
         """
         if data_paths is None:
             data_paths = []
         self.input_paths = JsonClassPaths(json_path=json_path, dag_path=dag_path, data_paths=data_paths)
 
-    def setup(self, scenario: Scenario):
+    def setup(self, scenario: Scenario, data=None):
         """Function to populate all the necessary parts of the json_class needed to execute tests"""
         self.scenario = scenario
         self._get_scenario_variables()
         self.scenario.setup_treatment_variables()
         self.causal_specification = CausalSpecification(
             scenario=self.scenario, causal_dag=CausalDAG(self.input_paths.dag_path)
         )
         # Parse the JSON test plan
         with open(self.input_paths.json_path, encoding="utf-8") as f:
             self.test_plan = json.load(f)
         # Populate the data
         if self.input_paths.data_paths:
-            self.data = pd.concat([pd.read_csv(data_file, header=0) for data_file in self.input_paths.data_paths])
-        if len(self.data) == 0:
+            data = pd.concat([pd.read_csv(data_file, header=0) for data_file in self.input_paths.data_paths])
+        if data is None or len(data) == 0:
             raise ValueError(
-                "No data found, either provide a path to a file containing data or manually populate the .data "
+                "No data found. Please either provide a path to a file containing data or manually populate the .data "
                 "attribute with a dataframe before calling .setup()"
             )
+        self.data_collector = ObservationalDataCollector(self.scenario, data)
         self._populate_metas()
 
     def _create_abstract_test_case(self, test, mutates, effects):
         assert len(test["mutations"]) == 1
         treatment_var = next(self.scenario.variables[v] for v in test["mutations"])
 
         if not treatment_var.distribution:
-            fitter = Fitter(self.data[treatment_var.name], distributions=get_common_distributions())
+            fitter = Fitter(self.data_collector.data[treatment_var.name], distributions=get_common_distributions())
             fitter.fit()
             (dist, params) = list(fitter.get_best(method="sumsquare_error").items())[0]
             treatment_var.distribution = getattr(scipy.stats, dist)(**params)
             self._append_to_file(treatment_var.name + f" {dist}({params})", logging.INFO)
 
         abstract_test = AbstractCausalTestCase(
             scenario=self.scenario,
@@ -123,47 +124,28 @@
         :param estimators: Dictionary mapping estimator classes to string representations.
         :param f_flag: Failure flag that if True the script will stop executing when a test fails.
         """
         for test in self.test_plan["tests"]:
             if "skip" in test and test["skip"]:
                 continue
             test["estimator"] = estimators[test["estimator"]]
-            if "mutations" in test:
+            # If we have specified concrete control and treatment value
+            if "mutations" not in test:
+                failed, msg = self._run_concrete_metamorphic_test(test, f_flag, effects)
+            # If we have a variable to mutate
+            else:
                 if test["estimate_type"] == "coefficient":
-                    msg = self._run_coefficient_test(test=test, f_flag=f_flag, effects=effects)
+                    failed, msg = self._run_coefficient_test(test=test, f_flag=f_flag, effects=effects)
                 else:
-                    msg = self._run_ate_test(test=test, f_flag=f_flag, effects=effects, mutates=mutates)
-                self._append_to_file(msg, logging.INFO)
-            else:
-                outcome_variable = next(
-                    iter(test["expected_effect"])
-                )  # Take first key from dictionary of expected effect
-                base_test_case = BaseTestCase(
-                    treatment_variable=self.variables["inputs"][test["treatment_variable"]],
-                    outcome_variable=self.variables["outputs"][outcome_variable],
-                )
-
-                causal_test_case = CausalTestCase(
-                    base_test_case=base_test_case,
-                    expected_causal_effect=effects[test["expected_effect"][outcome_variable]],
-                    control_value=test["control_value"],
-                    treatment_value=test["treatment_value"],
-                    estimate_type=test["estimate_type"],
-                )
-                failed, _ = self._execute_test_case(causal_test_case=causal_test_case, test=test, f_flag=f_flag)
-
-                msg = (
-                    f"Executing concrete test: {test['name']} \n"
-                    + f"treatment variable: {test['treatment_variable']} \n"
-                    + f"outcome_variable = {outcome_variable} \n"
-                    + f"control value = {test['control_value']}, treatment value = {test['treatment_value']} \n"
-                    + f"Result: {'FAILED' if failed else 'Passed'}"
-                )
-                print(msg)
-                self._append_to_file(msg, logging.INFO)
+                    failed, msg = self._run_metamorphic_tests(
+                        test=test, f_flag=f_flag, effects=effects, mutates=mutates
+                    )
+            test["failed"] = failed
+            test["result"] = msg
+        return self.test_plan["tests"]
 
     def _run_coefficient_test(self, test: dict, f_flag: bool, effects: dict):
         """Builds structures and runs test case for tests with an estimate_type of 'coefficient'.
 
         :param test: Single JSON test definition stored in a mapping (dict)
         :param f_flag: Failure flag that if True the script will stop executing when a test fails.
         :param effects: Dictionary mapping effect class instances to string representations.
@@ -177,26 +159,53 @@
         assert len(test["expected_effect"]) == 1, "Can only have one expected effect."
         causal_test_case = CausalTestCase(
             base_test_case=base_test_case,
             expected_causal_effect=next(effects[effect] for variable, effect in test["expected_effect"].items()),
             estimate_type="coefficient",
             effect_modifier_configuration={self.scenario.variables[v] for v in test.get("effect_modifiers", [])},
         )
-        result = self._execute_test_case(causal_test_case=causal_test_case, test=test, f_flag=f_flag)
+        failed, result = self._execute_test_case(causal_test_case=causal_test_case, test=test, f_flag=f_flag)
         msg = (
             f"Executing test: {test['name']} \n"
             + f"  {causal_test_case} \n"
             + "  "
-            + ("\n  ").join(str(result[1]).split("\n"))
+            + ("\n  ").join(str(result).split("\n"))
             + "==============\n"
-            + f"  Result: {'FAILED' if result[0] else 'Passed'}"
+            + f"  Result: {'FAILED' if failed else 'Passed'}"
+        )
+        self._append_to_file(msg, logging.INFO)
+        return failed, result
+
+    def _run_concrete_metamorphic_test(self, test: dict, f_flag: bool, effects: dict):
+        outcome_variable = next(iter(test["expected_effect"]))  # Take first key from dictionary of expected effect
+        base_test_case = BaseTestCase(
+            treatment_variable=self.variables["inputs"][test["treatment_variable"]],
+            outcome_variable=self.variables["outputs"][outcome_variable],
+        )
+
+        causal_test_case = CausalTestCase(
+            base_test_case=base_test_case,
+            expected_causal_effect=effects[test["expected_effect"][outcome_variable]],
+            control_value=test["control_value"],
+            treatment_value=test["treatment_value"],
+            estimate_type=test["estimate_type"],
+        )
+        failed, msg = self._execute_test_case(causal_test_case=causal_test_case, test=test, f_flag=f_flag)
+
+        msg = (
+            f"Executing concrete test: {test['name']} \n"
+            + f"treatment variable: {test['treatment_variable']} \n"
+            + f"outcome_variable = {outcome_variable} \n"
+            + f"control value = {test['control_value']}, treatment value = {test['treatment_value']} \n"
+            + f"Result: {'FAILED' if failed else 'Passed'}"
         )
-        return msg
+        self._append_to_file(msg, logging.INFO)
+        return failed, msg
 
-    def _run_ate_test(self, test: dict, f_flag: bool, effects: dict, mutates: dict):
+    def _run_metamorphic_tests(self, test: dict, f_flag: bool, effects: dict, mutates: dict):
         """Builds structures and runs test case for tests with an estimate_type of 'ate'.
 
         :param test: Single JSON test definition stored in a mapping (dict)
         :param f_flag: Failure flag that if True the script will stop executing when a test fails.
         :param effects: Dictionary mapping effect class instances to string representations.
         :param mutates: Dictionary mapping mutation functions to string representations.
         :return: String containing the message to be outputted
@@ -220,55 +229,61 @@
             + "  abstract_test \n"
             + f"  {abstract_test} \n"
             + f"  {abstract_test.treatment_variable.name},"
             + f"  {abstract_test.treatment_variable.distribution} \n"
             + f"  Number of concrete tests for test case: {str(len(concrete_tests))} \n"
             + f"  {failures}/{len(concrete_tests)} failed for {test['name']}"
         )
-        return msg
+        self._append_to_file(msg, logging.INFO)
+        return failures, msg
 
     def _execute_tests(self, concrete_tests, test, f_flag):
         failures = 0
         details = []
         if "formula" in test:
             self._append_to_file(f"Estimator formula used for test: {test['formula']}")
+
         for concrete_test in concrete_tests:
             failed, result = self._execute_test_case(concrete_test, test, f_flag)
             details.append(result)
             if failed:
                 failures += 1
         return failures, details
 
     def _populate_metas(self):
         """
         Populate data with meta-variable values and add distributions to Causal Testing Framework Variables
         """
         for meta in self.scenario.variables_of_type(Meta):
-            meta.populate(self.data)
+            meta.populate(self.data_collector.data)
 
     def _execute_test_case(
-        self, causal_test_case: CausalTestCase, test: Iterable[Mapping], f_flag: bool
+        self, causal_test_case: CausalTestCase, test: Mapping, f_flag: bool
     ) -> (bool, CausalTestResult):
         """Executes a singular test case, prints the results and returns the test case result
         :param causal_test_case: The concrete test case to be executed
         :param test: Single JSON test definition stored in a mapping (dict)
         :param f_flag: Failure flag that if True the script will stop executing when a test fails.
         :return: A boolean that if True indicates the causal test case passed and if false indicates the test case
          failed.
         :rtype: bool
         """
         failed = False
 
-        causal_test_engine, estimation_model = self._setup_test(
-            causal_test_case, test, test["conditions"] if "conditions" in test else None
+        estimation_model = self._setup_test(causal_test_case=causal_test_case, test=test)
+        causal_test_result = causal_test_case.execute_test(
+            estimator=estimation_model, data_collector=self.data_collector
         )
-        causal_test_result = causal_test_engine.execute_test(estimation_model, causal_test_case)
-
         test_passes = causal_test_case.expected_causal_effect.apply(causal_test_result)
 
+        if "coverage" in test and test["coverage"]:
+            adequacy_metric = DataAdequacy(causal_test_case, estimation_model, self.data_collector)
+            adequacy_metric.measure_adequacy()
+            causal_test_result.adequacy = adequacy_metric
+
         if causal_test_result.ci_low() is not None and causal_test_result.ci_high() is not None:
             result_string = (
                 f"{causal_test_result.ci_low()} < {causal_test_result.test_value.value} <  "
                 f"{causal_test_result.ci_high()}"
             )
         else:
             result_string = f"{causal_test_result.test_value.value} no confidence intervals"
@@ -276,52 +291,42 @@
         if not test_passes:
             if f_flag:
                 raise StatisticsError(
                     f"{causal_test_case}\n    FAILED - expected {causal_test_case.expected_causal_effect}, "
                     f"got {result_string}"
                 )
             failed = True
-            logger.warning("   FAILED- expected %s, got %s", causal_test_case.expected_causal_effect, result_string)
         return failed, causal_test_result
 
-    def _setup_test(
-        self, causal_test_case: CausalTestCase, test: Mapping, conditions: list[str] = None
-    ) -> tuple[CausalTestEngine, Estimator]:
+    def _setup_test(self, causal_test_case: CausalTestCase, test: Mapping) -> Estimator:
         """Create the necessary inputs for a single test case
         :param causal_test_case: The concrete test case to be executed
         :param test: Single JSON test definition stored in a mapping (dict)
         :param conditions: A list of conditions which should be applied to the
         data. Conditions should be in the query format detailed at
         https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.query.html
         :returns:
-                - causal_test_engine - Test Engine instance for the test being run
                 - estimation_model - Estimator instance for the test being run
         """
-
-        data_collector = ObservationalDataCollector(
-            self.scenario, self.data.query(" & ".join(conditions)) if conditions else self.data
-        )
-        causal_test_engine = CausalTestEngine(self.causal_specification, data_collector, index_col=0)
-
         minimal_adjustment_set = self.causal_specification.causal_dag.identification(causal_test_case.base_test_case)
         treatment_var = causal_test_case.treatment_variable
         minimal_adjustment_set = minimal_adjustment_set - {treatment_var}
         estimator_kwargs = {
             "treatment": treatment_var.name,
             "treatment_value": causal_test_case.treatment_value,
             "control_value": causal_test_case.control_value,
             "adjustment_set": minimal_adjustment_set,
             "outcome": causal_test_case.outcome_variable.name,
-            "df": causal_test_engine.scenario_execution_data_df,
             "effect_modifiers": causal_test_case.effect_modifier_configuration,
+            "alpha": test["alpha"] if "alpha" in test else 0.05,
         }
         if "formula" in test:
             estimator_kwargs["formula"] = test["formula"]
         estimation_model = test["estimator"](**estimator_kwargs)
-        return causal_test_engine, estimation_model
+        return estimation_model
 
     def _append_to_file(self, line: str, log_level: int = None):
         """Appends given line(s) to the current output file. If log_level is specified it also logs that message to the
         logging level.
         :param line: The line or lines of text to be appended to the file
         :param log_level: An integer representing the logging level as specified by pythons inbuilt logging module. It
         is possible to use the inbuilt logging level variables such as logging.INFO and logging.WARNING
@@ -371,15 +376,14 @@
             help="Specify to overwrite any existing output files. This can lead to the loss of existing outputs if not "
             "careful",
             action="store_true",
         )
         parser.add_argument(
             "--log_path",
             help="Specify a directory to change the location of the log file",
-            default="./json_frontend.log",
         )
         parser.add_argument(
             "--data_path",
             help="Specify path to file containing runtime data",
             nargs="+",
         )
         parser.add_argument(
```

### Comparing `causal_testing_framework-4.3.0/causal_testing/specification/causal_dag.py` & `causal_testing_framework-5.1.0/causal_testing/specification/causal_dag.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.3.0/causal_testing/specification/metamorphic_relation.py` & `causal_testing_framework-5.1.0/causal_testing/specification/metamorphic_relation.py`

 * *Files 1% similar despite different names*

```diff
@@ -177,14 +177,15 @@
             "name": str(self),
             "estimator": "LinearRegressionEstimator",
             "estimate_type": "coefficient",
             "effect": "direct",
             "mutations": [self.treatment_var],
             "expected_effect": {self.output_var: "NoEffect"},
             "formula": f"{self.output_var} ~ {' + '.join([self.treatment_var] + self.adjustment_vars)}",
+            "alpha": 0.05,
             "skip": skip,
         }
 
     def __str__(self):
         formatted_str = f"{self.treatment_var} _||_ {self.output_var}"
         if self.adjustment_vars:
             formatted_str += f" | {self.adjustment_vars}"
```

### Comparing `causal_testing_framework-4.3.0/causal_testing/specification/scenario.py` & `causal_testing_framework-5.1.0/causal_testing/specification/scenario.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.3.0/causal_testing/specification/variable.py` & `causal_testing_framework-5.1.0/causal_testing/specification/variable.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.3.0/causal_testing/testing/base_test_case.py` & `causal_testing_framework-5.1.0/causal_testing/testing/base_test_case.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.3.0/causal_testing/testing/causal_test_outcome.py` & `causal_testing_framework-5.1.0/causal_testing/testing/causal_test_outcome.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,26 +37,38 @@
             return (1 < res.ci_low() < res.ci_high()) or (res.ci_low() < res.ci_high() < 1)
         raise ValueError(f"Test Value type {res.test_value.type} is not valid for this TestOutcome")
 
 
 class NoEffect(CausalTestOutcome):
     """An extension of TestOutcome representing that the expected causal effect should be zero."""
 
-    def __init__(self, atol: float = 1e-10):
+    def __init__(self, atol: float = 1e-10, ctol: float = 0.05):
+        """
+        :param atol: Arithmetic tolerance. The test will pass if the absolute value of the causal effect is less than
+                     atol.
+        :param ctol: Categorical tolerance. The test will pass if this proportion of categories pass.
+        """
         self.atol = atol
+        self.ctol = ctol
 
     def apply(self, res: CausalTestResult) -> bool:
         if res.test_value.type == "ate":
             return (res.ci_low() < 0 < res.ci_high()) or (abs(res.test_value.value) < self.atol)
         if res.test_value.type == "coefficient":
             ci_low = res.ci_low() if isinstance(res.ci_low(), Iterable) else [res.ci_low()]
             ci_high = res.ci_high() if isinstance(res.ci_high(), Iterable) else [res.ci_high()]
             value = res.test_value.value if isinstance(res.ci_high(), Iterable) else [res.test_value.value]
-            return all(ci_low < 0 < ci_high for ci_low, ci_high in zip(ci_low, ci_high)) or all(
-                abs(v) < self.atol for v in value
+
+            return (
+                sum(
+                    not ((ci_low < 0 < ci_high) or abs(v) < self.atol)
+                    for ci_low, ci_high, v in zip(ci_low, ci_high, value)
+                )
+                / len(value)
+                < self.ctol
             )
         if res.test_value.type == "risk_ratio":
             return (res.ci_low() < 1 < res.ci_high()) or np.isclose(res.test_value.value, 1.0, atol=self.atol)
         raise ValueError(f"Test Value type {res.test_value.type} is not valid for this TestOutcome")
 
 
 class ExactValue(SomeEffect):
```

### Comparing `causal_testing_framework-4.3.0/causal_testing/testing/causal_test_result.py` & `causal_testing_framework-5.1.0/causal_testing/testing/causal_test_result.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,21 +19,24 @@
 
 class CausalTestResult:
     """A container to hold the results of a causal test case. Every causal test case provides a point estimate of
     the ATE, given a particular treatment, outcome, and adjustment set. Some but not all estimators can provide
     confidence intervals."""
 
     def __init__(
+        # pylint: disable=too-many-arguments
         self,
         estimator: Estimator,
         test_value: TestValue,
         confidence_intervals: [float, float] = None,
         effect_modifier_configuration: {Variable: Any} = None,
+        adequacy=None,
     ):
         self.estimator = estimator
+        self.adequacy = adequacy
         if estimator.adjustment_set:
             self.adjustment_set = estimator.adjustment_set
         else:
             self.adjustment_set = set()
         self.test_value = test_value
         self.confidence_intervals = confidence_intervals
 
@@ -52,39 +55,46 @@
         base_str = (
             f"Causal Test Result\n==============\n"
             f"Treatment: {self.estimator.treatment}\n"
             f"Control value: {self.estimator.control_value}\n"
             f"Treatment value: {self.estimator.treatment_value}\n"
             f"Outcome: {self.estimator.outcome}\n"
             f"Adjustment set: {self.adjustment_set}\n"
+            f"Formula: {self.estimator.formula}\n"
             f"{self.test_value.type}: {result_str}\n"
         )
         confidence_str = ""
         if self.confidence_intervals:
             ci_str = " " + str(self.confidence_intervals)
             if "\n" in ci_str:
                 ci_str = " " + push(pd.DataFrame(self.confidence_intervals).transpose().to_string(header=False))
             confidence_str += f"Confidence intervals:{ci_str}\n"
-        return base_str + confidence_str
+            confidence_str += f"Alpha:{self.estimator.alpha}\n"
+        adequacy_str = ""
+        if self.adequacy:
+            adequacy_str = str(self.adequacy)
+        return base_str + confidence_str + adequacy_str
 
-    def to_dict(self):
+    def to_dict(self, json=False):
         """Return result contents as a dictionary
         :return: Dictionary containing contents of causal_test_result
         """
         base_dict = {
-            "treatment": self.estimator.treatment[0],
+            "treatment": self.estimator.treatment,
             "control_value": self.estimator.control_value,
             "treatment_value": self.estimator.treatment_value,
-            "outcome": self.estimator.outcome[0],
-            "adjustment_set": self.adjustment_set,
-            "test_value": self.test_value,
+            "outcome": self.estimator.outcome,
+            "adjustment_set": list(self.adjustment_set) if json else self.adjustment_set,
+            "effect_measure": self.test_value.type,
+            "effect_estimate": self.test_value.value,
+            "ci_low": self.ci_low(),
+            "ci_high": self.ci_high(),
         }
-        if self.confidence_intervals and all(self.confidence_intervals):
-            base_dict["ci_low"] = min(self.confidence_intervals)
-            base_dict["ci_high"] = max(self.confidence_intervals)
+        if self.adequacy:
+            base_dict["adequacy"] = self.adequacy.to_dict()
         return base_dict
 
     def ci_low(self):
         """Return the lower bracket of the confidence intervals."""
         if self.confidence_intervals:
             return self.confidence_intervals[0]
         return None
```

### Comparing `causal_testing_framework-4.3.0/causal_testing/testing/estimators.py` & `causal_testing_framework-5.1.0/causal_testing/testing/estimators.py`

 * *Files 7% similar despite different names*

```diff
@@ -45,21 +45,23 @@
         treatment: str,
         treatment_value: float,
         control_value: float,
         adjustment_set: set,
         outcome: str,
         df: pd.DataFrame = None,
         effect_modifiers: dict[str:Any] = None,
+        alpha: float = 0.05,
     ):
         self.treatment = treatment
         self.treatment_value = treatment_value
         self.control_value = control_value
         self.adjustment_set = adjustment_set
         self.outcome = outcome
         self.df = df
+        self.alpha = alpha
         if effect_modifiers is None:
             self.effect_modifiers = {}
         elif isinstance(effect_modifiers, dict):
             self.effect_modifiers = effect_modifiers
         else:
             raise ValueError(f"Unsupported type for effect_modifiers {effect_modifiers}. Expected iterable")
         self.modelling_assumptions = []
@@ -123,35 +125,16 @@
         self.modelling_assumptions += "Independently and identically distributed errors."
 
     def _run_logistic_regression(self, data) -> RegressionResultsWrapper:
         """Run logistic regression of the treatment and adjustment set against the outcome and return the model.
 
         :return: The model after fitting to data.
         """
-        # 1. Reduce dataframe to contain only the necessary columns
-        reduced_df = data.copy()
-        necessary_cols = [self.treatment] + list(self.adjustment_set) + [self.outcome]
-        missing_rows = reduced_df[necessary_cols].isnull().any(axis=1)
-        reduced_df = reduced_df[~missing_rows]
-        reduced_df = reduced_df.sort_values([self.treatment])
-        logger.debug(reduced_df[necessary_cols])
-
-        # 2. Add intercept
-        reduced_df["Intercept"] = 1  # self.intercept
-
-        # 3. Estimate the unit difference in outcome caused by unit difference in treatment
-        cols = [self.treatment]
-        cols += [x for x in self.adjustment_set if x not in cols]
-        treatment_and_adjustments_cols = reduced_df[cols + ["Intercept"]]
-        for col in treatment_and_adjustments_cols:
-            if str(treatment_and_adjustments_cols.dtypes[col]) == "object":
-                treatment_and_adjustments_cols = pd.get_dummies(
-                    treatment_and_adjustments_cols, columns=[col], drop_first=True
-                )
         model = smf.logit(formula=self.formula, data=data).fit(disp=0)
+        self.model = model
         return model
 
     def estimate(self, data: pd.DataFrame, adjustment_config: dict = None) -> RegressionResultsWrapper:
         """add terms to the dataframe and estimate the outcome from the data
         :param data: A pandas dataframe containing execution data from the system-under-test.
         :param adjustment_config: Dictionary containing the adjustment configuration of the adjustment set
         """
@@ -159,15 +142,14 @@
             adjustment_config = {}
         if set(self.adjustment_set) != set(adjustment_config):
             raise ValueError(
                 f"Invalid adjustment configuration {adjustment_config}. Must specify values for {self.adjustment_set}"
             )
 
         model = self._run_logistic_regression(data)
-        self.model = model
 
         x = pd.DataFrame(columns=self.df.columns)
         x["Intercept"] = 1  # self.intercept
         x[self.treatment] = [self.treatment_value, self.control_value]
         for k, v in adjustment_config.items():
             x[k] = v
         for k, v in self.effect_modifiers.items():
@@ -233,15 +215,15 @@
         ) = self.estimate_control_treatment(bootstrap_size=bootstrap_size, adjustment_config=adjustment_config)
         estimate = treatment_outcome - control_outcome
 
         if control_bootstraps is None or treatment_bootstraps is None:
             return estimate, (None, None)
 
         bootstraps = sorted(list(treatment_bootstraps - control_bootstraps))
-        bound = int((bootstrap_size * 0.05) / 2)
+        bound = int((bootstrap_size * self.alpha) / 2)
         ci_low = bootstraps[bound]
         ci_high = bootstraps[bootstrap_size - bound]
 
         logger.info(
             f"Changing {self.treatment} from {self.control_value} to {self.treatment_value} gives an estimated "
             f"ATE of {ci_low} < {estimate} < {ci_high}"
         )
@@ -267,15 +249,15 @@
         ) = self.estimate_control_treatment(bootstrap_size=bootstrap_size, adjustment_config=adjustment_config)
         estimate = treatment_outcome / control_outcome
 
         if control_bootstraps is None or treatment_bootstraps is None:
             return estimate, (None, None)
 
         bootstraps = sorted(list(treatment_bootstraps / control_bootstraps))
-        bound = ceil((bootstrap_size * 0.05) / 2)
+        bound = ceil((bootstrap_size * self.alpha) / 2)
         ci_low = bootstraps[bound]
         ci_high = bootstraps[bootstrap_size - bound]
 
         logger.info(
             f"Changing {self.treatment} from {self.control_value} to {self.treatment_value} gives an estimated "
             f"risk ratio of {ci_low} < {estimate} < {ci_high}"
         )
@@ -305,16 +287,19 @@
         treatment_value: float,
         control_value: float,
         adjustment_set: set,
         outcome: str,
         df: pd.DataFrame = None,
         effect_modifiers: dict[Variable:Any] = None,
         formula: str = None,
+        alpha: float = 0.05,
     ):
-        super().__init__(treatment, treatment_value, control_value, adjustment_set, outcome, df, effect_modifiers)
+        super().__init__(
+            treatment, treatment_value, control_value, adjustment_set, outcome, df, effect_modifiers, alpha=alpha
+        )
 
         self.model = None
         if effect_modifiers is None:
             effect_modifiers = []
 
         if formula is not None:
             self.formula = formula
@@ -332,23 +317,22 @@
         """
         self.modelling_assumptions += (
             "The variables in the data must fit a shape which can be expressed as a linear"
             "combination of parameters and functions of variables. Note that these functions"
             "do not need to be linear."
         )
 
-    def estimate_unit_ate(self) -> float:
+    def estimate_coefficient(self) -> float:
         """Estimate the unit average treatment effect of the treatment on the outcome. That is, the change in outcome
         caused by a unit change in treatment.
 
         :return: The unit average treatment effect and the 95% Wald confidence intervals.
         """
         model = self._run_linear_regression()
         newline = "\n"
-        print(model.conf_int())
         treatment = [self.treatment]
         if str(self.df.dtypes[self.treatment]) == "object":
             design_info = dmatrix(self.formula.split("~")[1], self.df).design_info
             treatment = design_info.column_names[design_info.term_name_slices[self.treatment]]
         assert set(treatment).issubset(
             model.params.index.tolist()
         ), f"{treatment} not in\n{'  '+str(model.params.index).replace(newline, newline+'  ')}"
@@ -363,41 +347,39 @@
     def estimate_ate(self) -> tuple[float, list[float, float], float]:
         """Estimate the average treatment effect of the treatment on the outcome. That is, the change in outcome caused
         by changing the treatment variable from the control value to the treatment value.
 
         :return: The average treatment effect and the 95% Wald confidence intervals.
         """
         model = self._run_linear_regression()
-        self.model = model
 
         # Create an empty individual for the control and treated
         individuals = pd.DataFrame(1, index=["control", "treated"], columns=model.params.index)
 
         # It is ABSOLUTELY CRITICAL that these go last, otherwise we can't index
         # the effect with "ate = t_test_results.effect[0]"
         individuals.loc["control", [self.treatment]] = self.control_value
         individuals.loc["treated", [self.treatment]] = self.treatment_value
 
         # Perform a t-test to compare the predicted outcome of the control and treated individual (ATE)
         t_test_results = model.t_test(individuals.loc["treated"] - individuals.loc["control"])
         ate = t_test_results.effect[0]
-        confidence_intervals = list(t_test_results.conf_int().flatten())
+        confidence_intervals = list(t_test_results.conf_int(alpha=self.alpha).flatten())
         return ate, confidence_intervals
 
     def estimate_control_treatment(self, adjustment_config: dict = None) -> tuple[pd.Series, pd.Series]:
         """Estimate the outcomes under control and treatment.
 
         :return: The estimated outcome under control and treatment in the form
         (control_outcome, treatment_outcome).
         """
         if adjustment_config is None:
             adjustment_config = {}
 
         model = self._run_linear_regression()
-        self.model = model
 
         x = pd.DataFrame(columns=self.df.columns)
         x[self.treatment] = [self.treatment_value, self.control_value]
         x["Intercept"] = 1  # self.intercept
         for k, v in adjustment_config.items():
             x[k] = v
         for k, v in self.effect_modifiers.items():
@@ -438,33 +420,20 @@
         return (treatment_outcome["mean"] - control_outcome["mean"]), [ci_low, ci_high]
 
     def _run_linear_regression(self) -> RegressionResultsWrapper:
         """Run linear regression of the treatment and adjustment set against the outcome and return the model.
 
         :return: The model after fitting to data.
         """
-        # 1. Reduce dataframe to contain only the necessary columns
-        reduced_df = self.df.copy()
-        necessary_cols = [self.treatment] + list(self.adjustment_set) + [self.outcome]
-        missing_rows = reduced_df[necessary_cols].isnull().any(axis=1)
-        reduced_df = reduced_df[~missing_rows]
-        reduced_df = reduced_df.sort_values([self.treatment])
-        logger.debug(reduced_df[necessary_cols])
-
-        # 2. Add intercept
-        reduced_df["Intercept"] = 1  # self.intercept
-
-        # 3. Estimate the unit difference in outcome caused by unit difference in treatment
-        cols = [self.treatment]
-        cols += [x for x in self.adjustment_set if x not in cols]
         model = smf.ols(formula=self.formula, data=self.df).fit()
+        self.model = model
         return model
 
     def _get_confidence_intervals(self, model, treatment):
-        confidence_intervals = model.conf_int(alpha=0.05, cols=None)
+        confidence_intervals = model.conf_int(alpha=self.alpha, cols=None)
         ci_low, ci_high = (
             confidence_intervals[0].loc[treatment],
             confidence_intervals[1].loc[treatment],
         )
         return [ci_low, ci_high]
 
 
@@ -501,41 +470,41 @@
         related linearly in the form Y = aX + b."""
         self.modelling_assumptions += """The three IV conditions must hold
             (i) Instrument is associated with treatment
             (ii) Instrument does not affect outcome except through its potential effect on treatment
             (iii) Instrument and outcome do not share causes
         """
 
-    def estimate_coefficient(self, df):
+    def estimate_iv_coefficient(self, df):
         """
         Estimate the linear regression coefficient of the treatment on the
         outcome.
         """
         # Estimate the total effect of instrument I on outcome Y = abI + c1
         ab = sm.OLS(df[self.outcome], df[[self.instrument]]).fit().params[self.instrument]
 
         # Estimate the direct effect of instrument I on treatment X = aI + c1
         a = sm.OLS(df[self.treatment], df[[self.instrument]]).fit().params[self.instrument]
 
         # Estimate the coefficient of I on X by cancelling
         return ab / a
 
-    def estimate_unit_ate(self, bootstrap_size=100):
+    def estimate_coefficient(self, bootstrap_size=100):
         """
         Estimate the unit ate (i.e. coefficient) of the treatment on the
         outcome.
         """
         bootstraps = sorted(
-            [self.estimate_coefficient(self.df.sample(len(self.df), replace=True)) for _ in range(bootstrap_size)]
+            [self.estimate_iv_coefficient(self.df.sample(len(self.df), replace=True)) for _ in range(bootstrap_size)]
         )
-        bound = ceil((bootstrap_size * 0.05) / 2)
+        bound = ceil((bootstrap_size * self.alpha) / 2)
         ci_low = bootstraps[bound]
         ci_high = bootstraps[bootstrap_size - bound]
 
-        return self.estimate_coefficient(self.df), (ci_low, ci_high)
+        return self.estimate_iv_coefficient(self.df), (ci_low, ci_high)
 
 
 class CausalForestEstimator(Estimator):
     """A causal random forest estimator is a non-parametric estimator which recursively partitions the covariate space
     to learn a low-dimensional representation of treatment effect heterogeneity. This form of estimator is best suited
     to the estimation of heterogeneous treatment effects i.e. the estimated effect for every sample rather than the
     population average.
@@ -614,15 +583,15 @@
         # Fit a model to the data
         model = CausalForestDML(model_y=GradientBoostingRegressor(), model_t=GradientBoostingRegressor())
         model.fit(outcome_df, treatment_df, X=effect_modifier_df, W=confounders_df)
 
         # Obtain CATES and confidence intervals
         conditional_ates = model.effect(effect_modifier_df, T0=self.control_value, T1=self.treatment_value).flatten()
         [ci_low, ci_high] = model.effect_interval(
-            effect_modifier_df, T0=self.control_value, T1=self.treatment_value, alpha=0.05
+            effect_modifier_df, T0=self.control_value, T1=self.treatment_value, alpha=self.alpha
         )
 
         # Merge results into a dataframe (CATE, confidence intervals, and effect modifier values)
         results_df = pd.DataFrame(columns=["cate", "ci_low", "ci_high"])
         results_df["cate"] = list(conditional_ates)
         results_df["ci_low"] = list(ci_low.flatten())
         results_df["ci_high"] = list(ci_high.flatten())
```

### Comparing `causal_testing_framework-4.3.0/causal_testing/testing/intervention.py` & `causal_testing_framework-5.1.0/causal_testing/testing/intervention.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.3.0/causal_testing/utils/validation.py` & `causal_testing_framework-5.1.0/causal_testing/utils/validation.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.3.0/causal_testing_framework.egg-info/PKG-INFO` & `causal_testing_framework-5.1.0/causal_testing_framework.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: causal-testing-framework
-Version: 4.3.0
+Version: 5.1.0
 Summary: A framework for causal testing using causal directed acyclic graphs.
 Author: The CITCOM team
 License: MIT
 Project-URL: Bug_Tracker, https://github.com/CITCOM-project/CausalTestingFramework/issues
 Project-URL: Documentation, https://causal-testing-framework.readthedocs.io/
 Project-URL: Source, https://github.com/CITCOM-project/CausalTestingFramework
 Keywords: causal inference,verification
```

### Comparing `causal_testing_framework-4.3.0/causal_testing_framework.egg-info/SOURCES.txt` & `causal_testing_framework-5.1.0/causal_testing_framework.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -24,16 +24,16 @@
 causal_testing/specification/causal_dag.py
 causal_testing/specification/causal_specification.py
 causal_testing/specification/metamorphic_relation.py
 causal_testing/specification/scenario.py
 causal_testing/specification/variable.py
 causal_testing/testing/__init__.py
 causal_testing/testing/base_test_case.py
+causal_testing/testing/causal_test_adequacy.py
 causal_testing/testing/causal_test_case.py
-causal_testing/testing/causal_test_engine.py
 causal_testing/testing/causal_test_outcome.py
 causal_testing/testing/causal_test_result.py
 causal_testing/testing/causal_test_suite.py
 causal_testing/testing/effect.py
 causal_testing/testing/estimators.py
 causal_testing/testing/intervention.py
 causal_testing/utils/__init__.py
@@ -105,17 +105,18 @@
 tests/test_helpers.py
 tests/data/nhefs.csv
 tests/data_collection_tests/test_observational_data_collector.py
 tests/generation_tests/test_abstract_test_case.py
 tests/json_front_tests/test_json_class.py
 tests/resources/data/dag.dot
 tests/resources/data/data.csv
+tests/resources/data/data_with_categorical.csv
 tests/resources/data/data_with_meta.csv
 tests/resources/data/tests.json
 tests/specification_tests/test_causal_dag.py
 tests/specification_tests/test_metamorphic_relations.py
 tests/specification_tests/test_variable.py
+tests/testing_tests/test_causal_test_adequacy.py
 tests/testing_tests/test_causal_test_case.py
-tests/testing_tests/test_causal_test_engine.py
 tests/testing_tests/test_causal_test_outcome.py
 tests/testing_tests/test_causal_test_suite.py
 tests/testing_tests/test_estimators.py
```

### Comparing `causal_testing_framework-4.3.0/docs/Makefile` & `causal_testing_framework-5.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.3.0/docs/README.md` & `causal_testing_framework-5.1.0/docs/README.md`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.3.0/docs/make.bat` & `causal_testing_framework-5.1.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.3.0/docs/source/conf.py` & `causal_testing_framework-5.1.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.3.0/docs/source/description.rst` & `causal_testing_framework-5.1.0/docs/source/description.rst`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.3.0/docs/source/dev/actions_and_webhooks.rst` & `causal_testing_framework-5.1.0/docs/source/dev/actions_and_webhooks.rst`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.3.0/docs/source/dev/documentation.rst` & `causal_testing_framework-5.1.0/docs/source/dev/documentation.rst`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.3.0/docs/source/dev/version_release.rst` & `causal_testing_framework-5.1.0/docs/source/dev/version_release.rst`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.3.0/docs/source/frontends/json_front_end.rst` & `causal_testing_framework-5.1.0/docs/source/frontends/json_front_end.rst`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.3.0/docs/source/frontends/test_suite.rst` & `causal_testing_framework-5.1.0/docs/source/frontends/test_suite.rst`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.3.0/docs/source/images/workflow.png` & `causal_testing_framework-5.1.0/docs/source/images/workflow.png`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.3.0/docs/source/index.rst` & `causal_testing_framework-5.1.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.3.0/docs/source/installation.rst` & `causal_testing_framework-5.1.0/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.3.0/docs/source/modules/causal_specification.rst` & `causal_testing_framework-5.1.0/docs/source/modules/causal_specification.rst`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.3.0/docs/source/modules/causal_tests.rst` & `causal_testing_framework-5.1.0/docs/source/modules/causal_tests.rst`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.3.0/docs/source/modules/data_collector.rst` & `causal_testing_framework-5.1.0/docs/source/modules/data_collector.rst`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.3.0/docs/source/usage.rst` & `causal_testing_framework-5.1.0/docs/source/usage.rst`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.3.0/examples/covasim_/doubling_beta/README.md` & `causal_testing_framework-5.1.0/examples/covasim_/doubling_beta/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -10,11 +10,11 @@
 (Doubling Beta) of the paper.
 
 ## How to run
 To run this case study:
 1. Ensure all project dependencies are installed by running `pip install .` from the top
 level of this directory (instructions are provided in the project README).
 2. Change directory to `causal_testing/examples/covasim_/doubling_beta`.
-3. Run the command `python test_beta.py`.
+3. Run the command `python example_beta.py`.
 
 This will print out a series of test results covering a range of different causal questions that correspond to those
 in Table 3 of the paper.
```

### Comparing `causal_testing_framework-4.3.0/examples/covasim_/doubling_beta/dag.png` & `causal_testing_framework-5.1.0/examples/covasim_/doubling_beta/dag.png`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.3.0/examples/covasim_/doubling_beta/data/10k_observational_data.csv` & `causal_testing_framework-5.1.0/examples/covasim_/doubling_beta/data/10k_observational_data.csv`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.3.0/examples/covasim_/doubling_beta/example_beta.py` & `causal_testing_framework-5.1.0/examples/covasim_/doubling_beta/example_beta.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
+from pathlib import Path
 import matplotlib.pyplot as plt
 import pandas as pd
 import numpy as np
 from causal_testing.specification.causal_dag import CausalDAG
 from causal_testing.specification.scenario import Scenario
 from causal_testing.specification.variable import Input, Output
 from causal_testing.specification.causal_specification import CausalSpecification
 from causal_testing.data_collection.data_collector import ObservationalDataCollector
 from causal_testing.testing.causal_test_case import CausalTestCase
 from causal_testing.testing.causal_test_outcome import Positive
-from causal_testing.testing.causal_test_engine import CausalTestEngine
 from causal_testing.testing.estimators import LinearRegressionEstimator
 from causal_testing.testing.base_test_case import BaseTestCase
 from matplotlib.pyplot import rcParams
 
 import os
 import logging
 
@@ -27,16 +27,16 @@
 #     "figure.figsize": (10, 6),
 #     "text.usetex": True,
 #     "font.family": "serif",
 #     "text.latex.preamble": r"\usepackage{libertine}",
 # }
 # rcParams.update(rc_fonts)
 
-ROOT = os.path.realpath(os.path.dirname(__file__))
-OBSERVATIONAL_DATA_PATH = f"{ROOT}/data/10k_observational_data.csv"
+ROOT = Path(os.path.realpath(os.path.dirname(__file__)))
+OBSERVATIONAL_DATA_PATH = ROOT / "data" / "10k_observational_data.csv"
 
 
 def doubling_beta_CATE_on_csv(
     observational_data_path: str, simulate_counterfactuals: bool = False, verbose: bool = False
 ):
     """Compute the CATE of increasing beta from 0.016 to 0.032 on cum_infections using the dataframe
     loaded from the specified path. Additionally simulate the counterfactuals by repeating the analysis
@@ -46,43 +46,45 @@
     :param simulate_counterfactuals: Whether to repeat analysis with counterfactuals.
     :param verbose: Whether to print verbose details (causal test results).
     :return results_dict: A nested dictionary containing results (ate and confidence intervals)
                           for association, causation, and counterfactual (if completed).
     """
     results_dict = {"association": {}, "causation": {}}
 
-    # Read in the observational data, perform identification, and setup the causal_test_engine
+    # Read in the observational data, perform identification
     past_execution_df = pd.read_csv(observational_data_path)
-    _, causal_test_engine, causal_test_case = engine_setup(observational_data_path)
+    data_collector, _, causal_test_case, causal_specification = setup(past_execution_df)
 
     linear_regression_estimator = LinearRegressionEstimator(
         "beta",
         0.032,
         0.016,
         {"avg_age", "contacts"},  # We use custom adjustment set
         "cum_infections",
         df=past_execution_df,
         formula="cum_infections ~ beta + np.power(beta, 2) + avg_age + contacts",
     )
 
     # Add squared terms for beta, since it has a quadratic relationship with cumulative infections
-    causal_test_result = causal_test_engine.execute_test(linear_regression_estimator, causal_test_case)
+    causal_test_result = causal_test_case.execute_test(
+        estimator=linear_regression_estimator, data_collector=data_collector
+    )
 
     # Repeat for association estimate (no adjustment)
     no_adjustment_linear_regression_estimator = LinearRegressionEstimator(
         "beta",
         0.032,
         0.016,
         set(),
         "cum_infections",
         df=past_execution_df,
         formula="cum_infections ~ beta + np.power(beta, 2)",
     )
-    association_test_result = causal_test_engine.execute_test(
-        no_adjustment_linear_regression_estimator, causal_test_case
+    association_test_result = causal_test_case.execute_test(
+        estimator=no_adjustment_linear_regression_estimator, data_collector=data_collector
     )
 
     # Store results for plotting
     results_dict["association"] = {
         "ate": association_test_result.test_value.value,
         "cis": association_test_result.confidence_intervals,
         "df": past_execution_df,
@@ -105,17 +107,18 @@
             0.032,
             0.016,
             {"avg_age", "contacts"},
             "cum_infections",
             df=counterfactual_past_execution_df,
             formula="cum_infections ~ beta + np.power(beta, 2) + avg_age + contacts",
         )
-        counterfactual_causal_test_result = causal_test_engine.execute_test(
-            linear_regression_estimator, causal_test_case
+        counterfactual_causal_test_result = causal_test_case.execute_test(
+            estimator=linear_regression_estimator, data_collector=data_collector
         )
+
         results_dict["counterfactual"] = {
             "ate": counterfactual_causal_test_result.test_value.value,
             "cis": counterfactual_causal_test_result.confidence_intervals,
             "df": counterfactual_past_execution_df,
         }
         if verbose:
             print(f"Counterfactual:\n{counterfactual_causal_test_result}")
@@ -214,15 +217,15 @@
     else:
         outpath_base_str = f"{ROOT}/"
     all_fig.savefig(outpath_base_str + "all_executions.pdf", format="pdf")
     age_fig.savefig(outpath_base_str + "age_executions.pdf", format="pdf")
     age_contact_fig.savefig(outpath_base_str + "age_contact_executions.pdf", format="pdf")
 
 
-def engine_setup(observational_data_path):
+def setup(observational_data):
     # 1. Read in the Causal DAG
     causal_dag = CausalDAG(f"{ROOT}/dag.dot")
 
     # 2. Create variables
     pop_size = Input("pop_size", int)
     pop_infected = Input("pop_infected", int)
     n_days = Input("n_days", int)
@@ -259,23 +262,20 @@
 
     # 6. Create a causal test case
     causal_test_case = CausalTestCase(
         base_test_case=base_test_case, expected_causal_effect=Positive, control_value=0.016, treatment_value=0.032
     )
 
     # 7. Create a data collector
-    data_collector = ObservationalDataCollector(scenario, pd.read_csv(observational_data_path))
-
-    # 8. Create an instance of the causal test engine
-    causal_test_engine = CausalTestEngine(causal_specification, data_collector)
+    data_collector = ObservationalDataCollector(scenario, observational_data)
 
-    # 9. Obtain the minimal adjustment set for the base test case from the causal DAG
+    # 8. Obtain the minimal adjustment set for the base test case from the causal DAG
     minimal_adjustment_set = causal_dag.identification(base_test_case)
 
-    return minimal_adjustment_set, causal_test_engine, causal_test_case
+    return data_collector, minimal_adjustment_set, causal_test_case, causal_specification
 
 
 def plot_doubling_beta_CATEs(results_dict, title, figure=None, axes=None, row=None, col=None):
     # Get the CATE as a percentage for association and causation
     ate = results_dict["causation"]["ate"]
     association_ate = results_dict["association"]["ate"]
```

### Comparing `causal_testing_framework-4.3.0/examples/covasim_/vaccinating_elderly/README.md` & `causal_testing_framework-5.1.0/examples/covasim_/vaccinating_elderly/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -15,11 +15,11 @@
 
 ## How to run
 To run this case study:
 1. Ensure all project dependencies are installed by running `pip install .` from the top
 level of this directory (instructions are provided in the project README).
 2. Additionally, in order to run Covasim, install version 3.0.7 by running `pip install covasim==3.0.7`.
 3. Change directory to `causal_testing/examples/covasim_/vaccinating_elderly`.
-4. Run the command `python test_vaccine.py`.
+4. Run the command `python example_vaccine.py`.
 
 This will run Covasim as described above and print out the causal test results for the effect of each input on each
 output.
```

### Comparing `causal_testing_framework-4.3.0/examples/covasim_/vaccinating_elderly/dag.png` & `causal_testing_framework-5.1.0/examples/covasim_/vaccinating_elderly/dag.png`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.3.0/examples/covasim_/vaccinating_elderly/example_vaccine.py` & `causal_testing_framework-5.1.0/examples/covasim_/vaccinating_elderly/example_vaccine.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 from causal_testing.specification.causal_dag import CausalDAG
 from causal_testing.specification.scenario import Scenario
 from causal_testing.specification.variable import Input, Output
 from causal_testing.specification.causal_specification import CausalSpecification
 from causal_testing.data_collection.data_collector import ExperimentalDataCollector
 from causal_testing.testing.causal_test_case import CausalTestCase
 from causal_testing.testing.causal_test_outcome import Positive, Negative, NoEffect
-from causal_testing.testing.causal_test_engine import CausalTestEngine
 from causal_testing.testing.estimators import LinearRegressionEstimator
 from causal_testing.testing.base_test_case import BaseTestCase
 
 import os
 import logging
 
 logger = logging.getLogger(__name__)
@@ -77,33 +76,30 @@
         cum_infections: Positive(),
         cum_vaccinations: Negative(),
         cum_vaccinated: Negative(),
         max_doses: NoEffect(),
     }
     results_dict = {"cum_infections": {}, "cum_vaccinations": {}, "cum_vaccinated": {}, "max_doses": {}}
 
-    # 7. Create an instance of the causal test engine
-    causal_test_engine = CausalTestEngine(causal_specification, data_collector, index_col=0)
-
     for outcome_variable, expected_effect in expected_outcome_effects.items():
         base_test_case = BaseTestCase(treatment_variable=vaccine, outcome_variable=outcome_variable)
         causal_test_case = CausalTestCase(
             base_test_case=base_test_case, expected_causal_effect=expected_effect, control_value=0, treatment_value=1
         )
 
-        # 8. Obtain the minimal adjustment set for the causal test case from the causal DAG
+        # 7. Obtain the minimal adjustment set for the causal test case from the causal DAG
         minimal_adjustment_set = causal_dag.identification(base_test_case)
 
-        # 9. Build statistical model
+        # 8. Build statistical model
         linear_regression_estimator = LinearRegressionEstimator(
             vaccine.name, 1, 0, minimal_adjustment_set, outcome_variable.name
         )
 
-        # 10. Execute test and save results in dict
-        causal_test_result = causal_test_engine.execute_test(linear_regression_estimator, causal_test_case)
+        # 9. Execute test and save results in dict
+        causal_test_result = causal_test_case.execute_test(linear_regression_estimator, data_collector)
         if verbose:
             logging.info("Causation:\n%s", causal_test_result)
         results_dict[outcome_variable.name]["ate"] = causal_test_result.test_value.value
         results_dict[outcome_variable.name]["cis"] = causal_test_result.confidence_intervals
         results_dict[outcome_variable.name]["test_passes"] = causal_test_case.expected_causal_effect.apply(
             causal_test_result
         )
@@ -208,15 +204,15 @@
                 # Append inputs to results
                 for param in pars_dict.keys():
                     results_dict[param].append(run.pars[param])
 
                 # Append outputs to results
                 for output in desired_outputs:
                     if output not in results:
-                        raise IndexError(f"{output} is not in the Covasim outputs.")
+                        raise IndexError(f"{output} is not in the Covasim outputs. Are you using v3.0.7?")
                     results_dict[output].append(
                         results[output][-1]
                     )  # Append the final recorded value for each variable
 
         # Any parameters without results are assigned np.nan for each execution
         for param, results in results_dict.items():
             if not results:
```

### Comparing `causal_testing_framework-4.3.0/examples/lr91/README.md` & `causal_testing_framework-5.1.0/examples/lr91/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -14,11 +14,11 @@
 1. `causal_test_max_conductances.py` which has a for loop to iteratively call the `causal_test_engine`
 2. `causal_test_max_conductances_test_suite.py`, which uses the `causal_test_suite` object to interact with the `causal_test_engine`
 
 To run this case study:
 1. Ensure all project dependencies are installed by running `pip install .` in the top level directory
    (instructions are provided in the project README).
 2. Change directory to `causal_testing/examples/lr91`.
-3. Run the command `python test_max_conductances.py` or `python test_max_conductances_test_suite.py`
+3. Run the command `python example_max_conductances.py` or `python example_max_conductances_test_suite.py`
 
 This should print a series of causal test results covering the effects of a range of different sized interventions made
 to the inputs on APD90, and should also plot Figure 2 from the paper.
```

### Comparing `causal_testing_framework-4.3.0/examples/lr91/dag.dot` & `causal_testing_framework-5.1.0/examples/lr91/dag.dot`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.3.0/examples/lr91/dag.png` & `causal_testing_framework-5.1.0/examples/lr91/dag.png`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.3.0/examples/lr91/data/normalised_results.csv` & `causal_testing_framework-5.1.0/examples/lr91/data/normalised_results.csv`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.3.0/examples/lr91/data/results.csv` & `causal_testing_framework-5.1.0/examples/lr91/data/results.csv`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.3.0/examples/lr91/example_max_conductances.py` & `causal_testing_framework-5.1.0/examples/lr91/example_max_conductances.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from causal_testing.specification.causal_dag import CausalDAG
 from causal_testing.specification.scenario import Scenario
 from causal_testing.specification.variable import Input, Output
 from causal_testing.specification.causal_specification import CausalSpecification
 from causal_testing.data_collection.data_collector import ObservationalDataCollector
 from causal_testing.testing.causal_test_case import CausalTestCase
 from causal_testing.testing.causal_test_outcome import Positive, Negative, NoEffect
-from causal_testing.testing.causal_test_engine import CausalTestEngine
 from causal_testing.testing.estimators import LinearRegressionEstimator
 from causal_testing.testing.base_test_case import BaseTestCase
 from matplotlib.pyplot import rcParams
 
 import os
 import logging
 
@@ -134,25 +133,22 @@
         control_value=control_val,
         treatment_value=treatment_val,
     )
 
     # 7. Create a data collector
     data_collector = ObservationalDataCollector(scenario, pd.read_csv(observational_data_path))
 
-    # 8. Create an instance of the causal test engine
-    causal_test_engine = CausalTestEngine(causal_specification, data_collector)
-
-    # 9. Obtain the minimal adjustment set from the causal DAG
+    # 8. Obtain the minimal adjustment set from the causal DAG
     minimal_adjustment_set = causal_dag.identification(base_test_case)
     linear_regression_estimator = LinearRegressionEstimator(
         treatment_var.name, treatment_val, control_val, minimal_adjustment_set, "APD90"
     )
 
-    # 10. Run the causal test and print results
-    causal_test_result = causal_test_engine.execute_test(linear_regression_estimator, causal_test_case)
+    # 9. Run the causal test and print results
+    causal_test_result = causal_test_case.execute_test(linear_regression_estimator, data_collector)
     logger.info("%s", causal_test_result)
     return causal_test_result.test_value.value, causal_test_result.confidence_intervals
 
 
 def plot_ates_with_cis(results_dict: dict, xs: list, save: bool = False, show: bool = False):
     """Plot the average treatment effects for a given treatment against a list of x-values with confidence intervals.
 
@@ -194,8 +190,8 @@
         df[columns] = (df[columns] - df[columns].min()) / (df[columns].max() - df[columns].min())
         return df
     else:
         return (df - df.min()) / (df.max() - df.min())
 
 
 if __name__ == "__main__":
-    test_sensitivity_analysis(show=True)
+    test_sensitivity_analysis()
```

### Comparing `causal_testing_framework-4.3.0/examples/lr91/example_max_conductances_test_suite.py` & `causal_testing_framework-5.1.0/examples/lr91/example_max_conductances_test_suite.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from causal_testing.specification.causal_dag import CausalDAG
 from causal_testing.specification.scenario import Scenario
 from causal_testing.specification.variable import Input, Output
 from causal_testing.specification.causal_specification import CausalSpecification
 from causal_testing.data_collection.data_collector import ObservationalDataCollector
 from causal_testing.testing.causal_test_case import CausalTestCase
 from causal_testing.testing.causal_test_outcome import Positive, Negative, NoEffect
-from causal_testing.testing.causal_test_engine import CausalTestEngine
 from causal_testing.testing.estimators import LinearRegressionEstimator
 from causal_testing.testing.base_test_case import BaseTestCase
 from causal_testing.testing.causal_test_suite import CausalTestSuite
 from matplotlib.pyplot import rcParams
 
 import os
 
@@ -143,19 +142,16 @@
 
     # 5. Create a causal specification from the scenario and causal DAG
     causal_specification = CausalSpecification(scenario, causal_dag)
 
     # 7. Create a data collector
     data_collector = ObservationalDataCollector(scenario, pd.read_csv(observational_data_path))
 
-    # 8. Create an instance of the causal test engine
-    causal_test_engine = CausalTestEngine(causal_specification, data_collector)
-
-    # 9. Run the causal test suite
-    causal_test_results = causal_test_engine.execute_test_suite(test_suite)
+    # 8. Run the causal test suite
+    causal_test_results = test_suite.execute_test_suite(data_collector, causal_specification)
     return causal_test_results
 
 
 def plot_ates_with_cis(results_dict: dict, xs: list, save: bool = False, show=False):
     """Plot the average treatment effects for a given treatment against a list of x-values with confidence intervals.
 
     :param results_dict: A dictionary containing results for sensitivity analysis of each input parameter.
@@ -196,8 +192,8 @@
         df[columns] = (df[columns] - df[columns].min()) / (df[columns].max() - df[columns].min())
         return df
     else:
         return (df - df.min()) / (df.max() - df.min())
 
 
 if __name__ == "__main__":
-    test_sensitivity_analysis(show=True, save=True)
+    test_sensitivity_analysis()
```

### Comparing `causal_testing_framework-4.3.0/examples/poisson/README.md` & `causal_testing_framework-5.1.0/examples/poisson/README.md`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.3.0/examples/poisson/causal_tests.json` & `causal_testing_framework-5.1.0/examples/poisson/causal_tests.json`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.3.0/examples/poisson/dag.dot` & `causal_testing_framework-5.1.0/examples/poisson/dag.dot`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.3.0/examples/poisson/data.csv` & `causal_testing_framework-5.1.0/examples/poisson/data.csv`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.3.0/examples/poisson/example_run_causal_tests.py` & `causal_testing_framework-5.1.0/examples/poisson/example_run_causal_tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -153,15 +153,15 @@
     ROOT = os.path.realpath(os.path.dirname(__file__))
 
     log_path = f"{ROOT}/json_frontend.log"
     json_path = f"{ROOT}/causal_tests.json"
     dag_path = f"{ROOT}/dag.dot"
     data_path = f"{ROOT}/data.csv"
 
-    json_utility = JsonUtility(log_path)  # Create an instance of the extended JsonUtility class
+    json_utility = JsonUtility(log_path, output_overwrite=True)  # Create an instance of the extended JsonUtility class
     json_utility.set_paths(
         json_path, dag_path, [data_path]
     )  # Set the path to the data.csv, dag.dot and causal_tests.json file
 
     # Load the Causal Variables into the JsonUtility class ready to be used in the tests
     json_utility.setup(
         scenario=modelling_scenario
```

### Comparing `causal_testing_framework-4.3.0/examples/poisson-line-process/README.md` & `causal_testing_framework-5.1.0/examples/poisson-line-process/README.md`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.3.0/examples/poisson-line-process/dag.png` & `causal_testing_framework-5.1.0/examples/poisson-line-process/dag.png`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.3.0/examples/poisson-line-process/data/random/data_random_1000.csv` & `causal_testing_framework-5.1.0/examples/poisson-line-process/data/random/data_random_1000.csv`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.3.0/examples/poisson-line-process/data/smt_100/data_smt_wh10_100.csv` & `causal_testing_framework-5.1.0/examples/poisson-line-process/data/smt_100/data_smt_wh10_100.csv`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.3.0/examples/poisson-line-process/data/smt_100/data_smt_wh1_100.csv` & `causal_testing_framework-5.1.0/examples/poisson-line-process/data/smt_100/data_smt_wh1_100.csv`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.3.0/examples/poisson-line-process/data/smt_100/data_smt_wh2_100.csv` & `causal_testing_framework-5.1.0/examples/poisson-line-process/data/smt_100/data_smt_wh2_100.csv`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.3.0/examples/poisson-line-process/data/smt_100/data_smt_wh3_100.csv` & `causal_testing_framework-5.1.0/examples/poisson-line-process/data/smt_100/data_smt_wh3_100.csv`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.3.0/examples/poisson-line-process/data/smt_100/data_smt_wh4_100.csv` & `causal_testing_framework-5.1.0/examples/poisson-line-process/data/smt_100/data_smt_wh4_100.csv`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.3.0/examples/poisson-line-process/data/smt_100/data_smt_wh5_100.csv` & `causal_testing_framework-5.1.0/examples/poisson-line-process/data/smt_100/data_smt_wh5_100.csv`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.3.0/examples/poisson-line-process/data/smt_100/data_smt_wh6_100.csv` & `causal_testing_framework-5.1.0/examples/poisson-line-process/data/smt_100/data_smt_wh6_100.csv`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.3.0/examples/poisson-line-process/data/smt_100/data_smt_wh7_100.csv` & `causal_testing_framework-5.1.0/examples/poisson-line-process/data/smt_100/data_smt_wh7_100.csv`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.3.0/examples/poisson-line-process/data/smt_100/data_smt_wh8_100.csv` & `causal_testing_framework-5.1.0/examples/poisson-line-process/data/smt_100/data_smt_wh8_100.csv`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.3.0/examples/poisson-line-process/data/smt_100/data_smt_wh9_100.csv` & `causal_testing_framework-5.1.0/examples/poisson-line-process/data/smt_100/data_smt_wh9_100.csv`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.3.0/examples/poisson-line-process/example_poisson_process.py` & `causal_testing_framework-5.1.0/examples/poisson-line-process/example_poisson_process.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from causal_testing.specification.causal_dag import CausalDAG
 from causal_testing.specification.scenario import Scenario
 from causal_testing.specification.variable import Input, Output
 from causal_testing.specification.causal_specification import CausalSpecification
 from causal_testing.data_collection.data_collector import ObservationalDataCollector
 from causal_testing.testing.causal_test_case import CausalTestCase
 from causal_testing.testing.causal_test_outcome import ExactValue, Positive
-from causal_testing.testing.causal_test_engine import CausalTestEngine
 from causal_testing.testing.estimators import LinearRegressionEstimator, Estimator
 from causal_testing.testing.base_test_case import BaseTestCase
 
 import pandas as pd
 import os
 import logging
 
@@ -81,21 +80,18 @@
     square_terms=[],
     inverse_terms=[],
     empirical=False,
 ):
     # 6. Create a data collector
     data_collector = ObservationalDataCollector(scenario, pd.read_csv(observational_data_path))
 
-    # 7. Create an instance of the causal test engine
-    causal_test_engine = CausalTestEngine(causal_specification, data_collector)
-
-    # 8. Obtain the minimal adjustment set for the causal test case from the causal DAG
+    # 7. Obtain the minimal adjustment set for the causal test case from the causal DAG
     minimal_adjustment_set = causal_dag.identification(causal_test_case.base_test_case)
 
-    # 9. Set up an estimator
+    # 8. Set up an estimator
     data = pd.read_csv(observational_data_path)
 
     treatment = causal_test_case.get_treatment_variable()
     outcome = causal_test_case.get_outcome_variable()
 
     estimator = None
     if empirical:
@@ -118,16 +114,16 @@
             adjustment_set=set(),
             outcome=outcome,
             df=data,
             effect_modifiers=causal_test_case.effect_modifier_configuration,
             formula=f"{outcome} ~ {treatment} + {'+'.join(square_terms + inverse_terms + list([e for e in causal_test_case.effect_modifier_configuration]))} -1",
         )
 
-    # 10. Execute the test
-    causal_test_result = causal_test_engine.execute_test(estimator, causal_test_case)
+    # 9. Execute the test
+    causal_test_result = causal_test_case.execute_test(estimator, data_collector)
 
     return causal_test_result
 
 
 def test_poisson_intensity_num_shapes(save=False):
     intensity_num_shapes_results = []
     for wh in range(1, 11):
```

### Comparing `causal_testing_framework-4.3.0/images/workflow.png` & `causal_testing_framework-5.1.0/images/workflow.png`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.3.0/pyproject.toml` & `causal_testing_framework-5.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.3.0/tests/data/nhefs.csv` & `causal_testing_framework-5.1.0/tests/data/nhefs.csv`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.3.0/tests/data_collection_tests/test_observational_data_collector.py` & `causal_testing_framework-5.1.0/tests/data_collection_tests/test_observational_data_collector.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,14 +57,15 @@
     def test_meta_population(self):
         def populate_m(data):
             data["M"] = data["X1"] * 2
 
         meta = Meta("M", int, populate_m)
         scenario = Scenario({self.X1, meta})
         observational_data_collector = ObservationalDataCollector(scenario, self.observational_df)
+        observational_data_collector.collect_data()
         data = observational_data_collector.collect_data()
         assert all((m == 2 * x1 for x1, m in zip(data["X1"], data["M"])))
 
     def tearDown(self) -> None:
         remove_temp_dir_if_existent()
```

### Comparing `causal_testing_framework-4.3.0/tests/generation_tests/test_abstract_test_case.py` & `causal_testing_framework-5.1.0/tests/generation_tests/test_abstract_test_case.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.3.0/tests/json_front_tests/test_json_class.py` & `causal_testing_framework-5.1.0/tests/json_front_tests/test_json_class.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import unittest
 from pathlib import Path
 from statistics import StatisticsError
 import scipy
+import os
 
 from causal_testing.testing.estimators import LinearRegressionEstimator
 from causal_testing.testing.causal_test_outcome import NoEffect, Positive
 from tests.test_helpers import remove_temp_dir_if_existent
 from causal_testing.json_front.json_class import JsonUtility, CausalVariables
 from causal_testing.specification.variable import Input, Output, Meta
 from causal_testing.specification.scenario import Scenario
@@ -94,15 +95,15 @@
                 }
             ]
         }
         self.json_class.test_plan = example_test
         effects = {"NoEffect": NoEffect()}
         mutates = {
             "Increase": lambda x: self.json_class.scenario.treatment_variables[x].z3
-                                  > self.json_class.scenario.variables[x].z3
+            > self.json_class.scenario.variables[x].z3
         }
         estimators = {"LinearRegressionEstimator": LinearRegressionEstimator}
         with self.assertRaises(StatisticsError):
             self.json_class.run_json_tests(effects, estimators, True, mutates)
 
     def test_generate_coefficient_tests_from_json(self):
         example_test = {
@@ -132,36 +133,34 @@
     def test_run_json_tests_from_json(self):
         example_test = {
             "tests": [
                 {
                     "name": "test1",
                     "mutations": {"test_input": "Increase"},
                     "estimator": "LinearRegressionEstimator",
-                    "estimate_type": "ate",
+                    "estimate_type": "coefficient",
                     "effect_modifiers": [],
                     "expected_effect": {"test_output": "NoEffect"},
+                    "coverage": True,
                     "skip": False,
                 }
             ]
         }
         self.json_class.test_plan = example_test
         effects = {"NoEffect": NoEffect()}
         mutates = {
             "Increase": lambda x: self.json_class.scenario.treatment_variables[x].z3
-                                  > self.json_class.scenario.variables[x].z3
+            > self.json_class.scenario.variables[x].z3
         }
         estimators = {"LinearRegressionEstimator": LinearRegressionEstimator}
 
-        self.json_class.run_json_tests(effects=effects, estimators=estimators, f_flag=False, mutates=mutates)
-
-        # Test that the final log message prints that failed tests are printed, which is expected behaviour for this
-        # scenario
-        with open("temp_out.txt", "r") as reader:
-            temp_out = reader.readlines()
-        self.assertIn("failed", temp_out[-1])
+        test_results = self.json_class.run_json_tests(
+            effects=effects, estimators=estimators, f_flag=False, mutates=mutates
+        )
+        self.assertTrue(test_results[0]["failed"])
 
     def test_generate_tests_from_json_no_dist(self):
         example_test = {
             "tests": [
                 {
                     "name": "test1",
                     "mutations": {"test_input_no_dist": "Increase"},
@@ -173,15 +172,15 @@
                 }
             ]
         }
         self.json_class.test_plan = example_test
         effects = {"NoEffect": NoEffect()}
         mutates = {
             "Increase": lambda x: self.json_class.scenario.treatment_variables[x].z3
-                                  > self.json_class.scenario.variables[x].z3
+            > self.json_class.scenario.variables[x].z3
         }
         estimators = {"LinearRegressionEstimator": LinearRegressionEstimator}
 
         self.json_class.run_json_tests(effects=effects, mutates=mutates, estimators=estimators, f_flag=False)
 
         # Test that the final log message prints that failed tests are printed, which is expected behaviour for this scenario
         with open("temp_out.txt", "r") as reader:
@@ -203,15 +202,15 @@
                 }
             ]
         }
         self.json_class.test_plan = example_test
         effects = {"Positive": Positive()}
         mutates = {
             "Increase": lambda x: self.json_class.scenario.treatment_variables[x].z3
-                                  > self.json_class.scenario.variables[x].z3
+            > self.json_class.scenario.variables[x].z3
         }
         estimators = {"LinearRegressionEstimator": LinearRegressionEstimator}
 
         self.json_class.run_json_tests(effects=effects, mutates=mutates, estimators=estimators, f_flag=False)
         with open("temp_out.txt", "r") as reader:
             temp_out = reader.readlines()
         self.assertIn("test_output ~ test_input", "".join(temp_out))
@@ -235,14 +234,15 @@
         effects = {"NoEffect": NoEffect()}
         estimators = {"LinearRegressionEstimator": LinearRegressionEstimator}
 
         self.json_class.run_json_tests(effects=effects, estimators=estimators, f_flag=False)
         with open("temp_out.txt", "r") as reader:
             temp_out = reader.readlines()
         self.assertIn("FAILED", temp_out[-1])
+
     def test_concrete_generate_params(self):
         example_test = {
             "tests": [
                 {
                     "name": "test1",
                     "mutations": {"test_input": "Increase"},
                     "estimator": "LinearRegressionEstimator",
@@ -255,15 +255,15 @@
                 }
             ]
         }
         self.json_class.test_plan = example_test
         effects = {"NoEffect": NoEffect()}
         mutates = {
             "Increase": lambda x: self.json_class.scenario.treatment_variables[x].z3
-                                  > self.json_class.scenario.variables[x].z3
+            > self.json_class.scenario.variables[x].z3
         }
         estimators = {"LinearRegressionEstimator": LinearRegressionEstimator}
 
         self.json_class.run_json_tests(effects=effects, estimators=estimators, f_flag=False, mutates=mutates)
 
         # Test that the final log message prints that failed tests are printed, which is expected behaviour for this
         # scenario
@@ -289,11 +289,13 @@
         json_class.set_paths(self.json_path, self.dag_path)
 
         with self.assertRaises(ValueError):
             json_class.setup(self.scenario)
 
     def tearDown(self) -> None:
         remove_temp_dir_if_existent()
+        if os.path.exists("temp_out.txt"):
+            os.remove("temp_out.txt")
 
 
 def populate_example(*args, **kwargs):
     pass
```

### Comparing `causal_testing_framework-4.3.0/tests/specification_tests/test_causal_dag.py` & `causal_testing_framework-5.1.0/tests/specification_tests/test_causal_dag.py`

 * *Files 0% similar despite different names*

```diff
@@ -170,45 +170,46 @@
         self.assertEqual(list(indirect_graph.graph.edges), original_edges)
         self.assertEqual(indirect_graph.graph.nodes, causal_dag.graph.nodes)
 
     def test_proper_backdoor_graph(self):
         """Test whether converting a Causal DAG to a proper back-door graph works correctly."""
         causal_dag = CausalDAG(self.dag_dot_path)
         proper_backdoor_graph = causal_dag.get_proper_backdoor_graph(["X1", "X2"], ["Y"])
-        edges = set([
-                    ("X1", "X2"),
-                    ("X2", "V"),
-                    ("X2", "D2"),
-                    ("D1", "D2"),
-                    ("D1", "Y"),
-                    ("Y", "D3"),
-                    ("Z", "X2"),
-                    ("Z", "Y"),
-                ])
-        self.assertTrue(
-            set(proper_backdoor_graph.graph.edges).issubset(edges))
+        edges = set(
+            [
+                ("X1", "X2"),
+                ("X2", "V"),
+                ("X2", "D2"),
+                ("D1", "D2"),
+                ("D1", "Y"),
+                ("Y", "D3"),
+                ("Z", "X2"),
+                ("Z", "Y"),
+            ]
+        )
+        self.assertTrue(set(proper_backdoor_graph.graph.edges).issubset(edges))
 
     def test_constructive_backdoor_criterion_should_hold(self):
         """Test whether the constructive criterion holds when it should."""
         causal_dag = CausalDAG(self.dag_dot_path)
         xs, ys, zs = ["X1", "X2"], ["Y"], ["Z"]
         proper_backdoor_graph = causal_dag.get_proper_backdoor_graph(xs, ys)
         self.assertTrue(causal_dag.constructive_backdoor_criterion(proper_backdoor_graph, xs, ys, zs))
 
     def test_constructive_backdoor_criterion_should_not_hold_not_d_separator_in_proper_backdoor_graph(
-            self,
+        self,
     ):
         """Test whether the constructive criterion fails when the adjustment set is not a d-separator."""
         causal_dag = CausalDAG(self.dag_dot_path)
         xs, ys, zs = ["X1", "X2"], ["Y"], ["V"]
         proper_backdoor_graph = causal_dag.get_proper_backdoor_graph(xs, ys)
         self.assertFalse(causal_dag.constructive_backdoor_criterion(proper_backdoor_graph, xs, ys, zs))
 
     def test_constructive_backdoor_criterion_should_not_hold_descendent_of_proper_causal_path(
-            self,
+        self,
     ):
         """Test whether the constructive criterion holds when the adjustment set Z contains a descendent of a variable
         on a proper causal path between X and Y."""
         causal_dag = CausalDAG(self.dag_dot_path)
         xs, ys, zs = ["X1", "X2"], ["Y"], ["D1"]
         proper_backdoor_graph = causal_dag.get_proper_backdoor_graph(xs, ys)
         self.assertFalse(causal_dag.constructive_backdoor_criterion(proper_backdoor_graph, xs, ys, zs))
```

### Comparing `causal_testing_framework-4.3.0/tests/specification_tests/test_metamorphic_relations.py` & `causal_testing_framework-5.1.0/tests/specification_tests/test_metamorphic_relations.py`

 * *Files 0% similar despite different names*

```diff
@@ -116,14 +116,15 @@
                 "estimate_type": "coefficient",
                 "estimator": "LinearRegressionEstimator",
                 "expected_effect": {"Z": "NoEffect"},
                 "formula": "Z ~ X1",
                 "mutations": ["X1"],
                 "name": "X1 _||_ Z",
                 "formula": "Z ~ X1",
+                "alpha": 0.05,
                 "skip": True,
             },
         )
 
     def test_should_cause_json_stub(self):
         """Test if the ShouldCause MR passes all metamorphic tests where the DAG perfectly represents the program
         and there is only a single input."""
```

### Comparing `causal_testing_framework-4.3.0/tests/specification_tests/test_variable.py` & `causal_testing_framework-5.1.0/tests/specification_tests/test_variable.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.3.0/tests/test_helpers.py` & `causal_testing_framework-5.1.0/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-4.3.0/tests/testing_tests/test_causal_test_engine.py` & `causal_testing_framework-5.1.0/tests/testing_tests/test_causal_test_case.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,71 @@
 import unittest
 import os
 import pandas as pd
 import numpy as np
+
 from tests.test_helpers import create_temp_dir_if_non_existent, remove_temp_dir_if_existent
 from causal_testing.specification.causal_specification import CausalSpecification, Scenario
 from causal_testing.specification.variable import Input, Output
 from causal_testing.specification.causal_dag import CausalDAG
 from causal_testing.data_collection.data_collector import ObservationalDataCollector
 from causal_testing.testing.causal_test_case import CausalTestCase
-from causal_testing.testing.causal_test_engine import CausalTestEngine
 from causal_testing.testing.causal_test_outcome import ExactValue
 from causal_testing.testing.estimators import CausalForestEstimator, LinearRegressionEstimator
 from causal_testing.testing.base_test_case import BaseTestCase
 
 
-class TestCausalTestEngineObservational(unittest.TestCase):
-    """Test the CausalTestEngine workflow using observational data.
+class TestCausalTestCase(unittest.TestCase):
+    """Test the CausalTestCase class.
+
+    The base test case is a data class which contains the minimum information
+    necessary to perform identification. The CausalTestCase class represents
+    a causal test case. We here test the basic getter methods.
+    """
+
+    def setUp(self) -> None:
+        # 2. Create Scenario and Causal Specification
+        A = Input("A", float)
+        C = Output("C", float)
+
+        # 3. Create an intervention and causal test case
+        self.expected_causal_effect = ExactValue(4)
+        self.base_test_case = BaseTestCase(A, C)
+        self.causal_test_case = CausalTestCase(
+            base_test_case=self.base_test_case,
+            expected_causal_effect=self.expected_causal_effect,
+            control_value=0,
+            treatment_value=1,
+        )
+
+    def test_get_treatment_variable(self):
+        self.assertEqual(self.causal_test_case.get_treatment_variable(), "A")
+
+    def test_get_outcome_variable(self):
+        self.assertEqual(self.causal_test_case.get_outcome_variable(), "C")
+
+    def test_get_treatment_value(self):
+        self.assertEqual(self.causal_test_case.get_treatment_value(), 1)
+
+    def test_get_control_value(self):
+        self.assertEqual(self.causal_test_case.get_control_value(), 0)
+
+    def test_str(self):
+        self.assertEqual(
+            str(self.causal_test_case),
+            "Running {'A': 1} instead of {'A': 0} should cause the following changes to"
+            " {Output: C::float}: ExactValue: 4±0.2.",
+        )
+
+    def tearDown(self) -> None:
+        remove_temp_dir_if_existent()
+
+
+class TestCausalTestExecution(unittest.TestCase):
+    """Test the causal test execution workflow using observational data.
 
     The causal test engine (CTE) is the main workflow for the causal testing framework. The CTE takes a causal test case
     and a causal specification and computes the causal effect of the intervention on the outcome of interest.
     """
 
     def setUp(self) -> None:
         # 1. Create Causal DAG
@@ -56,79 +102,38 @@
         df["C"] = df["D"] + (4 * (df["A"] + 2))  # C = (4*(A+2)) + D
         self.observational_data_csv_path = os.path.join(temp_dir_path, "observational_data.csv")
         df.to_csv(self.observational_data_csv_path, index=False)
 
         # 5. Create observational data collector
         # Obsolete?
         self.data_collector = ObservationalDataCollector(self.scenario, df)
-
-        # 5. Create causal test engine
-        self.causal_test_engine = CausalTestEngine(self.causal_specification, self.data_collector)
+        self.data_collector.collect_data()
+        self.df = self.data_collector.collect_data()
         self.minimal_adjustment_set = self.causal_dag.identification(self.base_test_case)
         # 6. Easier to access treatment and outcome values
         self.treatment_value = 1
         self.control_value = 0
 
-    def test_positivity_violation_throws_exception(self):
-        causal_test_engine = CausalTestEngine(self.causal_specification, self.data_collector)
-        causal_test_engine.scenario_execution_data_df.drop("A", axis=1, inplace=True)
-        estimation_model = LinearRegressionEstimator(
-            "A",
-            self.treatment_value,
-            self.control_value,
-            self.minimal_adjustment_set,
-            "C",
-            self.causal_test_engine.scenario_execution_data_df,
-        )
-        with self.assertRaises(Exception):
-            causal_test_engine.execute_test(estimation_model)
-
-    def test_check_no_positivity_violation(self):
-        """Check that no positivity violation is identified when there is no positivity violation."""
-        variables_to_check = list(self.minimal_adjustment_set) + ["A"] + ["C"]
-        self.assertFalse(self.causal_test_engine._check_positivity_violation(variables_to_check))
-
-    def test_check_positivity_violation_missing_confounder(self):
-        """Check that a positivity violation is identified when there is a positivity violation due to a missing
-        confounder."""
-        self.causal_test_engine.scenario_execution_data_df.drop(columns=["D"], inplace=True)  # Remove confounder
-        variables_to_check = list(self.minimal_adjustment_set) + ["A"] + ["C"]
-        self.assertTrue(self.causal_test_engine._check_positivity_violation(variables_to_check))
-
-    def test_check_positivity_violation_missing_treatment(self):
-        """Check that a positivity violation is identified when there is a positivity violation due to a missing
-        treatment."""
-        self.causal_test_engine.scenario_execution_data_df.drop(columns=["A"], inplace=True)  # Remove treatment
-        variables_to_check = list(self.minimal_adjustment_set) + ["A"] + ["C"]
-        self.assertTrue(self.causal_test_engine._check_positivity_violation(variables_to_check))
-
-    def test_check_positivity_violation_missing_outcome(self):
-        """Check that a positivity violation is identified when there is a positivity violation due to a missing
-        outcome."""
-        self.causal_test_engine.scenario_execution_data_df.drop(columns=["C"], inplace=True)  # Remove outcome
-        variables_to_check = list(self.minimal_adjustment_set) + ["A"] + ["C"]
-        self.assertTrue(self.causal_test_engine._check_positivity_violation(variables_to_check))
-
     def test_check_minimum_adjustment_set(self):
         """Check that the minimum adjustment set is correctly made"""
         minimal_adjustment_set = self.causal_dag.identification(self.base_test_case)
         self.assertEqual(minimal_adjustment_set, {"D"})
 
     def test_execute_test_observational_causal_forest_estimator(self):
         """Check that executing the causal test case returns the correct results for the dummy data using a causal
         forest estimator."""
         estimation_model = CausalForestEstimator(
             "A",
             self.treatment_value,
             self.control_value,
             self.minimal_adjustment_set,
             "C",
-            self.causal_test_engine.scenario_execution_data_df,
+            self.df,
         )
-        causal_test_result = self.causal_test_engine.execute_test(estimation_model, self.causal_test_case)
+        causal_test_result = self.causal_test_case.execute_test(estimation_model, self.data_collector)
         self.assertAlmostEqual(causal_test_result.test_value.value, 4, delta=1)
 
     def test_invalid_causal_effect(self):
         """Check that executing the causal test case returns the correct results for dummy data using a linear
         regression estimator."""
         base_test_case = BaseTestCase(treatment_variable=self.A, outcome_variable=self.C, effect="error")
 
@@ -140,129 +145,123 @@
         regression estimator."""
         estimation_model = LinearRegressionEstimator(
             "A",
             self.treatment_value,
             self.control_value,
             self.minimal_adjustment_set,
             "C",
-            self.causal_test_engine.scenario_execution_data_df,
+            self.df,
         )
-        causal_test_result = self.causal_test_engine.execute_test(estimation_model, self.causal_test_case)
+        causal_test_result = self.causal_test_case.execute_test(estimation_model, self.data_collector)
         self.assertAlmostEqual(causal_test_result.test_value.value, 4, delta=1e-10)
 
     def test_execute_test_observational_linear_regression_estimator_direct_effect(self):
         """Check that executing the causal test case returns the correct results for dummy data using a linear
         regression estimator."""
         base_test_case = BaseTestCase(treatment_variable=self.A, outcome_variable=self.C, effect="direct")
 
         causal_test_case = CausalTestCase(
             base_test_case=base_test_case,
             expected_causal_effect=self.expected_causal_effect,
             control_value=0,
             treatment_value=1,
         )
 
-        # 5. Create causal test engine
-        causal_test_engine = CausalTestEngine(self.causal_specification, self.data_collector)
         minimal_adjustment_set = self.causal_dag.identification(base_test_case)
         # 6. Easier to access treatment and outcome values
         self.treatment_value = 1
         self.control_value = 0
         estimation_model = LinearRegressionEstimator(
             "A",
             self.treatment_value,
             self.control_value,
             minimal_adjustment_set,
             "C",
-            causal_test_engine.scenario_execution_data_df,
+            self.df,
         )
-        causal_test_result = causal_test_engine.execute_test(estimation_model, causal_test_case)
+        causal_test_result = causal_test_case.execute_test(estimation_model, self.data_collector)
         self.assertAlmostEqual(causal_test_result.test_value.value, 4, delta=1e-10)
 
     def test_execute_test_observational_linear_regression_estimator_coefficient(self):
         """Check that executing the causal test case returns the correct results for dummy data using a linear
         regression estimator."""
         estimation_model = LinearRegressionEstimator(
             "D",
             self.treatment_value,
             self.control_value,
             self.minimal_adjustment_set,
             "A",
-            self.causal_test_engine.scenario_execution_data_df,
+            self.df,
         )
         self.causal_test_case.estimate_type = "coefficient"
-        causal_test_result = self.causal_test_engine.execute_test(estimation_model, self.causal_test_case)
+        causal_test_result = self.causal_test_case.execute_test(estimation_model, self.data_collector)
         self.assertEqual(int(causal_test_result.test_value.value), 0)
 
     def test_execute_test_observational_linear_regression_estimator_risk_ratio(self):
         """Check that executing the causal test case returns the correct results for dummy data using a linear
         regression estimator."""
         estimation_model = LinearRegressionEstimator(
             "D",
             self.treatment_value,
             self.control_value,
             self.minimal_adjustment_set,
             "A",
-            self.causal_test_engine.scenario_execution_data_df,
+            self.df,
         )
         self.causal_test_case.estimate_type = "risk_ratio"
-        causal_test_result = self.causal_test_engine.execute_test(estimation_model, self.causal_test_case)
+        causal_test_result = self.causal_test_case.execute_test(estimation_model, self.data_collector)
         self.assertEqual(int(causal_test_result.test_value.value), 0)
 
     def test_invalid_estimate_type(self):
         """Check that executing the causal test case returns the correct results for dummy data using a linear
         regression estimator."""
         estimation_model = LinearRegressionEstimator(
             "D",
             self.treatment_value,
             self.control_value,
             self.minimal_adjustment_set,
             "A",
-            self.causal_test_engine.scenario_execution_data_df,
+            self.df,
         )
         self.causal_test_case.estimate_type = "invalid"
-        with self.assertRaises(ValueError):
-            self.causal_test_engine.execute_test(estimation_model, self.causal_test_case)
+        with self.assertRaises(AttributeError):
+            self.causal_test_case.execute_test(estimation_model, self.data_collector)
 
     def test_execute_test_observational_linear_regression_estimator_squared_term(self):
         """Check that executing the causal test case returns the correct results for dummy data with a squared term
         using a linear regression estimator. C ~ 4*(A+2) + D + D^2"""
         estimation_model = LinearRegressionEstimator(
             "A",
             self.treatment_value,
             self.control_value,
             self.minimal_adjustment_set,
             "C",
-            self.causal_test_engine.scenario_execution_data_df,
+            self.df,
             formula=f"C ~ A + {'+'.join(self.minimal_adjustment_set)} + (D ** 2)",
         )
-        causal_test_result = self.causal_test_engine.execute_test(estimation_model, self.causal_test_case)
+        causal_test_result = self.causal_test_case.execute_test(estimation_model, self.data_collector)
         self.assertAlmostEqual(round(causal_test_result.test_value.value, 1), 4, delta=1)
 
     def test_execute_observational_causal_forest_estimator_cates(self):
         """Check that executing the causal test case returns the correct conditional average treatment effects for
         dummy data with effect multiplicative effect modification. C ~ (4*(A+2) + D)*M"""
         # Add some effect modifier M that has a multiplicative effect on C
-        self.causal_test_engine.scenario_execution_data_df["M"] = np.random.randint(
-            1, 5, len(self.causal_test_engine.scenario_execution_data_df)
-        )
-        self.causal_test_engine.scenario_execution_data_df["C"] *= self.causal_test_engine.scenario_execution_data_df[
-            "M"
-        ]
+        self.df["M"] = np.random.randint(1, 5, len(self.df))
+        self.df["C"] *= self.df["M"]
         estimation_model = CausalForestEstimator(
             "A",
             self.treatment_value,
             self.control_value,
             self.minimal_adjustment_set,
             "C",
-            self.causal_test_engine.scenario_execution_data_df,
+            self.df,
             effect_modifiers={"M": None},
         )
-        self.causal_test_case.estimate_type = "cate"
-        causal_test_result = self.causal_test_engine.execute_test(estimation_model, self.causal_test_case)
+        self.causal_test_case.estimate_type = "cates"
+        causal_test_result = self.causal_test_case.execute_test(estimation_model, self.data_collector)
         causal_test_result = causal_test_result.test_value.value
         # Check that each effect modifier's strata has a greater ATE than the last (ascending order)
         causal_test_result_m1 = causal_test_result.loc[causal_test_result["M"] == 1]
         causal_test_result_m2 = causal_test_result.loc[causal_test_result["M"] == 2]
         causal_test_result_m3 = causal_test_result.loc[causal_test_result["M"] == 3]
         causal_test_result_m4 = causal_test_result.loc[causal_test_result["M"] == 4]
         self.assertLess(causal_test_result_m1["cate"].mean(), causal_test_result_m2["cate"].mean())
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `causal_testing_framework-4.3.0/tests/testing_tests/test_causal_test_outcome.py` & `causal_testing_framework-5.1.0/tests/testing_tests/test_causal_test_outcome.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,15 +32,18 @@
             ctr.to_dict(),
             {
                 "treatment": "A",
                 "control_value": 0,
                 "treatment_value": 1,
                 "outcome": "A",
                 "adjustment_set": set(),
-                "test_value": test_value,
+                "effect_estimate": 0,
+                "effect_measure": "ate",
+                "ci_high": None,
+                "ci_low": None,
             },
         )
 
     def test_empty_adjustment_set(self):
         test_value = TestValue(type="ate", value=0)
         ctr = CausalTestResult(
             estimator=self.estimator,
@@ -56,14 +59,15 @@
             (
                 "Causal Test Result\n==============\n"
                 "Treatment: A\n"
                 "Control value: 0\n"
                 "Treatment value: 1\n"
                 "Outcome: A\n"
                 "Adjustment set: set()\n"
+                "Formula: A ~ A\n"
                 "ate: 0\n"
             ),
         )
 
     def test_Positive_ate_pass(self):
         test_value = TestValue(type="ate", value=5.05)
         ctr = CausalTestResult(
@@ -259,15 +263,16 @@
             ctr.to_dict(),
             {
                 "treatment": "A",
                 "control_value": 0,
                 "treatment_value": 1,
                 "outcome": "A",
                 "adjustment_set": set(),
-                "test_value": test_value,
+                "effect_estimate": 0,
+                "effect_measure": "ate",
                 "ci_low": -0.1,
                 "ci_high": 0.2,
             },
         )
 
     def test_someEffect_dict(self):
         test_value = TestValue(type="ate", value=0)
@@ -282,15 +287,16 @@
             ctr.to_dict(),
             {
                 "treatment": "A",
                 "control_value": 0,
                 "treatment_value": 1,
                 "outcome": "A",
                 "adjustment_set": set(),
-                "test_value": test_value,
+                "effect_estimate": 0,
+                "effect_measure": "ate",
                 "ci_low": -0.1,
                 "ci_high": 0.2,
             },
         )
 
     def test_positive_risk_ratio_e_value(self):
         cv = CausalValidator()
```

### Comparing `causal_testing_framework-4.3.0/tests/testing_tests/test_causal_test_suite.py` & `causal_testing_framework-5.1.0/tests/testing_tests/test_causal_test_suite.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import unittest
 import os
 import numpy as np
 import pandas as pd
-from causal_testing.testing.causal_test_engine import CausalTestEngine
-from causal_testing.testing.causal_test_engine import CausalTestSuite
+from causal_testing.testing.causal_test_suite import CausalTestSuite
 from causal_testing.testing.causal_test_case import CausalTestCase
 from causal_testing.testing.base_test_case import BaseTestCase
 from causal_testing.specification.variable import Input, Output
 from causal_testing.testing.causal_test_outcome import ExactValue
 from causal_testing.testing.estimators import CausalForestEstimator, LinearRegressionEstimator
 from causal_testing.specification.causal_specification import CausalSpecification, Scenario
 from causal_testing.data_collection.data_collector import ObservationalDataCollector
@@ -57,14 +56,17 @@
         self.estimators = [LinearRegressionEstimator]
 
         # 3. Create test_suite and add a test
         self.test_suite = CausalTestSuite()
         self.test_suite.add_test_object(
             base_test_case=self.base_test_case, causal_test_case_list=test_list, estimators_classes=self.estimators
         )
+        self.causal_specification = CausalSpecification(self.scenario, self.causal_dag)
+
+        self.data_collector = ObservationalDataCollector(self.scenario, self.df)
 
     def test_adding_test_object(self):
         "test an object can be added to the test_suite using the add_test_object function"
         test_suite = CausalTestSuite()
         test_list = [CausalTestCase(self.base_test_case, self.expected_causal_effect, 0, 1)]
         estimators = [LinearRegressionEstimator]
         test_suite.add_test_object(
@@ -89,41 +91,28 @@
 
         test_case = self.test_suite[base_test_case]
 
         self.assertEqual(test_case, manual_test_case)
 
     def test_execute_test_suite_single_base_test_case(self):
         """Check that the test suite can return the correct results from dummy data for a single base_test-case"""
-        causal_test_engine = self.create_causal_test_engine()
 
-        causal_test_results = causal_test_engine.execute_test_suite(test_suite=self.test_suite)
+        causal_test_results = self.test_suite.execute_test_suite(self.data_collector, self.causal_specification)
         causal_test_case_result = causal_test_results[self.base_test_case]
         self.assertAlmostEqual(causal_test_case_result["LinearRegressionEstimator"][0].test_value.value, 4, delta=1e-10)
 
     def test_execute_test_suite_multiple_estimators(self):
         """Check that executing a test suite with multiple estimators returns correct results for the dummy data
         for each estimator
         """
         estimators = [LinearRegressionEstimator, CausalForestEstimator]
         test_suite_2_estimators = CausalTestSuite()
         test_list = [CausalTestCase(self.base_test_case, self.expected_causal_effect, 0, 1)]
         test_suite_2_estimators.add_test_object(
             base_test_case=self.base_test_case, causal_test_case_list=test_list, estimators_classes=estimators
         )
-        causal_test_engine = self.create_causal_test_engine()
-        causal_test_results = causal_test_engine.execute_test_suite(test_suite=test_suite_2_estimators)
+        causal_test_results = test_suite_2_estimators.execute_test_suite(self.data_collector, self.causal_specification)
         causal_test_case_result = causal_test_results[self.base_test_case]
         linear_regression_result = causal_test_case_result["LinearRegressionEstimator"][0]
         causal_forrest_result = causal_test_case_result["CausalForestEstimator"][0]
         self.assertAlmostEqual(linear_regression_result.test_value.value, 4, delta=1e-1)
         self.assertAlmostEqual(causal_forrest_result.test_value.value, 4, delta=1e-1)
-
-    def create_causal_test_engine(self):
-        """
-        Creating test engine is relatively computationally complex, this function allows for it to
-        easily be made in only the tests that require it.
-        """
-        causal_specification = CausalSpecification(self.scenario, self.causal_dag)
-
-        data_collector = ObservationalDataCollector(self.scenario, self.df)
-        causal_test_engine = CausalTestEngine(causal_specification, data_collector)
-        return causal_test_engine
```

### Comparing `causal_testing_framework-4.3.0/tests/testing_tests/test_estimators.py` & `causal_testing_framework-5.1.0/tests/testing_tests/test_estimators.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,15 +94,15 @@
         )
 
     # Yes, this probably shouldn't be in here, but it uses the scarf data so it makes more sense to put it
     # here than duplicating the scarf data for a single test
     def test_linear_regression_categorical_ate(self):
         df = self.scarf_df.copy()
         logistic_regression_estimator = LinearRegressionEstimator("color", None, None, set(), "completed", df)
-        ate, confidence = logistic_regression_estimator.estimate_unit_ate()
+        ate, confidence = logistic_regression_estimator.estimate_coefficient()
         self.assertTrue(all([ci_low < 0 < ci_high for ci_low, ci_high in zip(confidence[0], confidence[1])]))
 
     def test_ate(self):
         df = self.scarf_df.copy()
         logistic_regression_estimator = LogisticRegressionEstimator("length_in", 65, 55, set(), "completed", df)
         ate, _ = logistic_regression_estimator.estimate_ate()
         self.assertEqual(round(ate, 4), -0.1987)
@@ -127,15 +127,17 @@
         ate, _ = logistic_regression_estimator.estimate_ate(estimator_params={"adjustment_config": {"large_gauge": 0}})
         self.assertEqual(round(ate, 4), -0.3388)
 
     def test_ate_invalid_adjustment(self):
         df = self.scarf_df.copy()
         logistic_regression_estimator = LogisticRegressionEstimator("length_in", 65, 55, {}, "completed", df)
         with self.assertRaises(ValueError):
-            ate, _ = logistic_regression_estimator.estimate_ate(estimator_params={"adjustment_config": {"large_gauge": 0}})
+            ate, _ = logistic_regression_estimator.estimate_ate(
+                estimator_params={"adjustment_config": {"large_gauge": 0}}
+            )
 
     def test_ate_effect_modifiers(self):
         df = self.scarf_df.copy()
         logistic_regression_estimator = LogisticRegressionEstimator(
             "length_in", 65, 55, set(), "completed", df, effect_modifiers={"large_gauge": 0}
         )
         ate, _ = logistic_regression_estimator.estimate_ate()
@@ -180,29 +182,29 @@
             control_value=None,
             adjustment_set=set(),
             outcome="Y",
             instrument="Z",
         )
         self.assertEqual(iv_estimator.estimate_coefficient(self.df), 2)
 
-    def test_estimate_unit_ate(self):
+    def test_estimate_coefficient(self):
         """
         Test we get the correct coefficient.
         """
         iv_estimator = InstrumentalVariableEstimator(
             df=self.df,
             treatment="X",
             treatment_value=None,
             control_value=None,
             adjustment_set=set(),
             outcome="Y",
             instrument="Z",
         )
-        unit_ate, [low, high] = iv_estimator.estimate_unit_ate()
-        self.assertEqual(unit_ate, 2)
+        coefficient, [low, high] = iv_estimator.estimate_coefficient()
+        self.assertEqual(coefficient, 2)
 
 
 class TestLinearRegressionEstimator(unittest.TestCase):
     """Test the linear regression estimator against the programming exercises in Section 2 of Hernán and Robins [1].
 
     Reference: Hernán MA, Robins JM (2020). Causal Inference: What If. Boca Raton: Chapman & Hall/CRC.
     Link: https://www.hsph.harvard.edu/miguel-hernan/causal-inference-book/
@@ -214,29 +216,29 @@
         cls.chapter_11_df = load_chapter_11_df()
 
     def test_program_11_2(self):
         """Test whether our linear regression implementation produces the same results as program 11.2 (p. 141)."""
         df = self.chapter_11_df
         linear_regression_estimator = LinearRegressionEstimator("treatments", None, None, set(), "outcomes", df)
         model = linear_regression_estimator._run_linear_regression()
-        ate, _ = linear_regression_estimator.estimate_unit_ate()
+        ate, _ = linear_regression_estimator.estimate_coefficient()
 
         self.assertEqual(round(model.params["Intercept"] + 90 * model.params["treatments"], 1), 216.9)
 
         # Increasing treatments from 90 to 100 should be the same as 10 times the unit ATE
         self.assertEqual(round(model.params["treatments"], 1), round(ate, 1))
 
     def test_program_11_3(self):
         """Test whether our linear regression implementation produces the same results as program 11.3 (p. 144)."""
         df = self.chapter_11_df.copy()
         linear_regression_estimator = LinearRegressionEstimator(
             "treatments", None, None, set(), "outcomes", df, formula="outcomes ~ treatments + np.power(treatments, 2)"
         )
         model = linear_regression_estimator._run_linear_regression()
-        ate, _ = linear_regression_estimator.estimate_unit_ate()
+        ate, _ = linear_regression_estimator.estimate_coefficient()
         self.assertEqual(
             round(
                 model.params["Intercept"]
                 + 90 * model.params["treatments"]
                 + 90 * 90 * model.params["np.power(treatments, 2)"],
                 1,
             ),
@@ -316,15 +318,15 @@
             covariates,
             "wt82_71",
             df,
             formula="wt82_71 ~ qsmk + age + np.power(age, 2) + wt71 + np.power(wt71, 2) + smokeintensity + np.power(smokeintensity, 2) + smokeyrs + np.power(smokeyrs, 2)",
         )
         # terms_to_square = ["age", "wt71", "smokeintensity", "smokeyrs"]
         # for term_to_square in terms_to_square:
-        ate, [ci_low, ci_high] = linear_regression_estimator.estimate_unit_ate()
+        ate, [ci_low, ci_high] = linear_regression_estimator.estimate_coefficient()
         self.assertEqual(round(ate, 1), 3.5)
         self.assertEqual([round(ci_low, 1), round(ci_high, 1)], [2.6, 4.3])
 
     def test_program_15_no_interaction_ate(self):
         """Test whether our linear regression implementation produces the same results as program 15.1 (p. 163, 184)
         without product parameter."""
         df = self.nhefs_df
```

