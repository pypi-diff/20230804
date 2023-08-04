# Comparing `tmp/edu_rdm_integration-0.1.4.tar.gz` & `tmp/edu-rdm-integration-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edu_rdm_integration-0.1.4.tar", max compression
+gzip compressed data, was "edu-rdm-integration-0.2.0.tar", last modified: Fri Aug  4 15:43:37 2023, max compression
```

## Comparing `edu_rdm_integration-0.1.4.tar` & `edu-rdm-integration-0.2.0.tar`

### file list

```diff
@@ -1,93 +1,124 @@
--rw-r--r--   0        0        0     3458 2023-07-18 06:39:46.917456 edu_rdm_integration-0.1.4/LICENSE
--rw-r--r--   0        0        0    11460 2023-07-18 06:39:46.917456 edu_rdm_integration-0.1.4/README.md
--rw-r--r--   0        0        0      692 2023-08-03 12:28:22.249817 edu_rdm_integration-0.1.4/pyproject.toml
--rw-r--r--   0        0        0       72 2023-07-18 06:39:46.919456 edu_rdm_integration-0.1.4/src/edu_rdm_integration/__init__.py
--rw-r--r--   0        0        0       83 2023-07-18 06:39:46.920456 edu_rdm_integration-0.1.4/src/edu_rdm_integration/adapters/__init__.py
--rw-r--r--   0        0        0      363 2023-07-18 06:39:46.920456 edu_rdm_integration-0.1.4/src/edu_rdm_integration/adapters/apps.py
--rw-r--r--   0        0        0     1505 2023-07-18 06:39:46.920456 edu_rdm_integration-0.1.4/src/edu_rdm_integration/adapters/caches.py
--rw-r--r--   0        0        0       66 2023-07-18 06:39:46.920456 edu_rdm_integration-0.1.4/src/edu_rdm_integration/adapters/consts.py
--rw-r--r--   0        0        0       93 2023-07-18 06:39:46.920456 edu_rdm_integration-0.1.4/src/edu_rdm_integration/adapters/enums.py
--rw-r--r--   0        0        0      255 2023-07-18 06:39:46.920456 edu_rdm_integration-0.1.4/src/edu_rdm_integration/adapters/errors.py
--rw-r--r--   0        0        0     2075 2023-07-18 06:39:46.920456 edu_rdm_integration-0.1.4/src/edu_rdm_integration/adapters/functions.py
--rw-r--r--   0        0        0     1105 2023-07-18 06:39:46.920456 edu_rdm_integration-0.1.4/src/edu_rdm_integration/adapters/helpers.py
--rw-r--r--   0        0        0      589 2023-07-18 06:39:46.920456 edu_rdm_integration-0.1.4/src/edu_rdm_integration/adapters/managers.py
--rw-r--r--   0        0        0      327 2023-07-18 06:39:46.920456 edu_rdm_integration-0.1.4/src/edu_rdm_integration/adapters/presenters.py
--rw-r--r--   0        0        0      598 2023-07-18 06:39:46.920456 edu_rdm_integration-0.1.4/src/edu_rdm_integration/adapters/receivers.py
--rw-r--r--   0        0        0      515 2023-07-18 06:39:46.920456 edu_rdm_integration-0.1.4/src/edu_rdm_integration/adapters/results.py
--rw-r--r--   0        0        0     2164 2023-07-18 06:39:46.920456 edu_rdm_integration-0.1.4/src/edu_rdm_integration/adapters/runners.py
--rw-r--r--   0        0        0     5504 2023-07-18 06:39:46.921456 edu_rdm_integration-0.1.4/src/edu_rdm_integration/adapters/strategies.py
--rw-r--r--   0        0        0      181 2023-07-18 06:39:46.921456 edu_rdm_integration-0.1.4/src/edu_rdm_integration/adapters/strings.py
--rw-r--r--   0        0        0       59 2023-07-18 06:39:46.921456 edu_rdm_integration-0.1.4/src/edu_rdm_integration/adapters/tests.py
--rw-r--r--   0        0        0      496 2023-07-18 06:39:46.921456 edu_rdm_integration-0.1.4/src/edu_rdm_integration/adapters/validators.py
--rw-r--r--   0        0        0     1822 2023-07-18 06:39:46.921456 edu_rdm_integration-0.1.4/src/edu_rdm_integration/app_settings.py
--rw-r--r--   0        0        0     2458 2023-07-24 05:38:47.497143 edu_rdm_integration-0.1.4/src/edu_rdm_integration/apps.py
--rw-r--r--   0        0        0        0 2023-07-18 06:39:46.921456 edu_rdm_integration-0.1.4/src/edu_rdm_integration/collect_data/__init__.py
--rw-r--r--   0        0        0        0 2023-07-18 06:39:46.921456 edu_rdm_integration-0.1.4/src/edu_rdm_integration/collect_data/base/__init__.py
--rw-r--r--   0        0        0     1310 2023-07-18 06:39:46.921456 edu_rdm_integration-0.1.4/src/edu_rdm_integration/collect_data/base/caches.py
--rw-r--r--   0        0        0     2353 2023-07-24 05:38:47.497143 edu_rdm_integration-0.1.4/src/edu_rdm_integration/collect_data/base/functions.py
--rw-r--r--   0        0        0     5219 2023-07-24 05:38:47.497143 edu_rdm_integration-0.1.4/src/edu_rdm_integration/collect_data/base/managers.py
--rw-r--r--   0        0        0     1422 2023-07-24 05:38:47.497143 edu_rdm_integration-0.1.4/src/edu_rdm_integration/collect_data/base/runners.py
--rw-r--r--   0        0        0        0 2023-07-18 06:39:46.922456 edu_rdm_integration-0.1.4/src/edu_rdm_integration/collect_data/calculated/__init__.py
--rw-r--r--   0        0        0        0 2023-07-18 06:39:46.923456 edu_rdm_integration-0.1.4/src/edu_rdm_integration/collect_data/calculated/base/__init__.py
--rw-r--r--   0        0        0     7212 2023-07-18 06:39:46.923456 edu_rdm_integration-0.1.4/src/edu_rdm_integration/collect_data/calculated/base/caches.py
--rw-r--r--   0        0        0       84 2023-07-18 06:39:46.923456 edu_rdm_integration-0.1.4/src/edu_rdm_integration/collect_data/calculated/base/consts.py
--rw-r--r--   0        0        0       93 2023-07-18 06:39:46.923456 edu_rdm_integration-0.1.4/src/edu_rdm_integration/collect_data/calculated/base/enums.py
--rw-r--r--   0        0        0      326 2023-07-18 06:39:46.923456 edu_rdm_integration-0.1.4/src/edu_rdm_integration/collect_data/calculated/base/errors.py
--rw-r--r--   0        0        0     1670 2023-07-18 06:39:46.923456 edu_rdm_integration-0.1.4/src/edu_rdm_integration/collect_data/calculated/base/functions.py
--rw-r--r--   0        0        0     1490 2023-07-18 06:39:46.923456 edu_rdm_integration-0.1.4/src/edu_rdm_integration/collect_data/calculated/base/helpers.py
--rw-r--r--   0        0        0      838 2023-07-18 06:39:46.923456 edu_rdm_integration-0.1.4/src/edu_rdm_integration/collect_data/calculated/base/managers.py
--rw-r--r--   0        0        0      438 2023-07-18 06:39:46.923456 edu_rdm_integration-0.1.4/src/edu_rdm_integration/collect_data/calculated/base/presenters.py
--rw-r--r--   0        0        0      708 2023-07-18 06:39:46.923456 edu_rdm_integration-0.1.4/src/edu_rdm_integration/collect_data/calculated/base/results.py
--rw-r--r--   0        0        0     1648 2023-07-18 06:39:46.924456 edu_rdm_integration-0.1.4/src/edu_rdm_integration/collect_data/calculated/base/runners.py
--rw-r--r--   0        0        0      181 2023-07-18 06:39:46.924456 edu_rdm_integration-0.1.4/src/edu_rdm_integration/collect_data/calculated/base/strings.py
--rw-r--r--   0        0        0       59 2023-07-18 06:39:46.924456 edu_rdm_integration-0.1.4/src/edu_rdm_integration/collect_data/calculated/base/tests.py
--rw-r--r--   0        0        0     1057 2023-07-18 06:39:46.924456 edu_rdm_integration-0.1.4/src/edu_rdm_integration/collect_data/calculated/base/validators.py
--rw-r--r--   0        0        0        0 2023-07-18 06:39:46.924456 edu_rdm_integration-0.1.4/src/edu_rdm_integration/collect_data/non_calculated/__init__.py
--rw-r--r--   0        0        0        0 2023-07-18 06:39:46.924456 edu_rdm_integration-0.1.4/src/edu_rdm_integration/collect_data/non_calculated/base/__init__.py
--rw-r--r--   0        0        0     5674 2023-07-18 06:39:46.924456 edu_rdm_integration-0.1.4/src/edu_rdm_integration/collect_data/non_calculated/base/caches.py
--rw-r--r--   0        0        0       66 2023-07-18 06:39:46.924456 edu_rdm_integration-0.1.4/src/edu_rdm_integration/collect_data/non_calculated/base/consts.py
--rw-r--r--   0        0        0       93 2023-07-18 06:39:46.924456 edu_rdm_integration-0.1.4/src/edu_rdm_integration/collect_data/non_calculated/base/enums.py
--rw-r--r--   0        0        0      297 2023-07-18 06:39:46.924456 edu_rdm_integration-0.1.4/src/edu_rdm_integration/collect_data/non_calculated/base/errors.py
--rw-r--r--   0        0        0     1563 2023-07-18 06:39:46.924456 edu_rdm_integration-0.1.4/src/edu_rdm_integration/collect_data/non_calculated/base/functions.py
--rw-r--r--   0        0        0     1376 2023-07-18 06:39:46.924456 edu_rdm_integration-0.1.4/src/edu_rdm_integration/collect_data/non_calculated/base/helpers.py
--rw-r--r--   0        0        0      783 2023-07-18 06:39:46.925456 edu_rdm_integration-0.1.4/src/edu_rdm_integration/collect_data/non_calculated/base/managers.py
--rw-r--r--   0        0        0      409 2023-07-18 06:39:46.925456 edu_rdm_integration-0.1.4/src/edu_rdm_integration/collect_data/non_calculated/base/presenters.py
--rw-r--r--   0        0        0      674 2023-07-18 06:39:46.925456 edu_rdm_integration-0.1.4/src/edu_rdm_integration/collect_data/non_calculated/base/results.py
--rw-r--r--   0        0        0     1541 2023-07-18 06:39:46.925456 edu_rdm_integration-0.1.4/src/edu_rdm_integration/collect_data/non_calculated/base/runners.py
--rw-r--r--   0        0        0      181 2023-07-18 06:39:46.925456 edu_rdm_integration-0.1.4/src/edu_rdm_integration/collect_data/non_calculated/base/strings.py
--rw-r--r--   0        0        0       59 2023-07-18 06:39:46.925456 edu_rdm_integration-0.1.4/src/edu_rdm_integration/collect_data/non_calculated/base/tests.py
--rw-r--r--   0        0        0      973 2023-07-18 06:39:46.925456 edu_rdm_integration-0.1.4/src/edu_rdm_integration/collect_data/non_calculated/base/validators.py
--rw-r--r--   0        0        0      635 2023-07-18 06:39:46.925456 edu_rdm_integration-0.1.4/src/edu_rdm_integration/consts.py
--rw-r--r--   0        0        0     9117 2023-07-18 06:39:46.925456 edu_rdm_integration-0.1.4/src/edu_rdm_integration/entities.py
--rw-r--r--   0        0        0     4876 2023-07-18 06:39:46.925456 edu_rdm_integration-0.1.4/src/edu_rdm_integration/enums.py
--rw-r--r--   0        0        0        0 2023-07-18 06:39:46.925456 edu_rdm_integration-0.1.4/src/edu_rdm_integration/export_data/__init__.py
--rw-r--r--   0        0        0        0 2023-07-18 06:39:46.926456 edu_rdm_integration-0.1.4/src/edu_rdm_integration/export_data/base/__init__.py
--rw-r--r--   0        0        0     1380 2023-07-18 06:39:46.926456 edu_rdm_integration-0.1.4/src/edu_rdm_integration/export_data/base/caches.py
--rw-r--r--   0        0        0      369 2023-07-18 06:39:46.926456 edu_rdm_integration-0.1.4/src/edu_rdm_integration/export_data/base/consts.py
--rw-r--r--   0        0        0       93 2023-07-18 06:39:46.926456 edu_rdm_integration-0.1.4/src/edu_rdm_integration/export_data/base/enums.py
--rw-r--r--   0        0        0      291 2023-07-18 06:39:46.926456 edu_rdm_integration-0.1.4/src/edu_rdm_integration/export_data/base/errors.py
--rw-r--r--   0        0        0    11664 2023-07-24 05:38:47.498144 edu_rdm_integration-0.1.4/src/edu_rdm_integration/export_data/base/functions.py
--rw-r--r--   0        0        0     3076 2023-07-18 06:39:46.926456 edu_rdm_integration-0.1.4/src/edu_rdm_integration/export_data/base/helpers.py
--rw-r--r--   0        0        0     5665 2023-07-24 05:38:47.498144 edu_rdm_integration-0.1.4/src/edu_rdm_integration/export_data/base/managers.py
--rw-r--r--   0        0        0      403 2023-07-18 06:39:46.926456 edu_rdm_integration-0.1.4/src/edu_rdm_integration/export_data/base/presenters.py
--rw-r--r--   0        0        0     2548 2023-07-18 06:39:46.926456 edu_rdm_integration-0.1.4/src/edu_rdm_integration/export_data/base/requests.py
--rw-r--r--   0        0        0      662 2023-07-18 06:39:46.926456 edu_rdm_integration-0.1.4/src/edu_rdm_integration/export_data/base/results.py
--rw-r--r--   0        0        0     2716 2023-07-24 05:38:47.498144 edu_rdm_integration-0.1.4/src/edu_rdm_integration/export_data/base/runners.py
--rw-r--r--   0        0        0      181 2023-07-18 06:39:46.926456 edu_rdm_integration-0.1.4/src/edu_rdm_integration/export_data/base/strings.py
--rw-r--r--   0        0        0       59 2023-07-18 06:39:46.927456 edu_rdm_integration-0.1.4/src/edu_rdm_integration/export_data/base/tests.py
--rw-r--r--   0        0        0      961 2023-07-18 06:39:46.927456 edu_rdm_integration-0.1.4/src/edu_rdm_integration/export_data/base/validators.py
--rw-r--r--   0        0        0       16 2023-07-18 06:39:46.927456 edu_rdm_integration-0.1.4/src/edu_rdm_integration/export_data/consts.py
--rw-r--r--   0        0        0        0 2023-07-18 06:39:46.927456 edu_rdm_integration-0.1.4/src/edu_rdm_integration/management/__init__.py
--rw-r--r--   0        0        0        0 2023-07-18 06:39:46.927456 edu_rdm_integration-0.1.4/src/edu_rdm_integration/management/commands/__init__.py
--rw-r--r--   0        0        0      487 2023-07-18 06:39:46.927456 edu_rdm_integration-0.1.4/src/edu_rdm_integration/management/commands/collect_models_data.py
--rw-r--r--   0        0        0      388 2023-07-18 06:39:46.927456 edu_rdm_integration-0.1.4/src/edu_rdm_integration/management/commands/export_entities_data.py
--rw-r--r--   0        0        0    19777 2023-07-24 05:38:47.498144 edu_rdm_integration-0.1.4/src/edu_rdm_integration/management/general.py
--rw-r--r--   0        0        0     2302 2023-07-18 06:39:46.927456 edu_rdm_integration-0.1.4/src/edu_rdm_integration/management/generators.py
--rw-r--r--   0        0        0      473 2023-07-18 06:39:46.927456 edu_rdm_integration-0.1.4/src/edu_rdm_integration/mapping.py
--rw-r--r--   0        0        0    18718 2023-08-03 12:28:22.250817 edu_rdm_integration-0.1.4/src/edu_rdm_integration/migrations/0001_initial.py
--rw-r--r--   0        0        0      944 2023-07-18 06:39:46.928456 edu_rdm_integration-0.1.4/src/edu_rdm_integration/migrations/0002_init_data_uploadstatus.py
--rw-r--r--   0        0        0        0 2023-07-18 06:39:46.928456 edu_rdm_integration-0.1.4/src/edu_rdm_integration/migrations/__init__.py
--rw-r--r--   0        0        0    19850 2023-07-18 06:39:46.928456 edu_rdm_integration-0.1.4/src/edu_rdm_integration/models.py
--rw-r--r--   0        0        0     6806 2023-07-18 06:39:46.928456 edu_rdm_integration-0.1.4/src/edu_rdm_integration/storages.py
--rw-r--r--   0        0        0     1936 2023-07-18 06:39:46.928456 edu_rdm_integration-0.1.4/src/edu_rdm_integration/utils.py
--rw-r--r--   0        0        0    12064 1970-01-01 00:00:00.000000 edu_rdm_integration-0.1.4/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 15:43:37.008634 edu-rdm-integration-0.2.0/
+-rw-r--r--   0 root         (0) root         (0)     3709 2023-08-04 12:28:07.000000 edu-rdm-integration-0.2.0/CHANGELOG.md
+-rwxr-xr-x   0 root         (0) root         (0)     5358 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.0/CONDUCT.md
+-rw-r--r--   0 root         (0) root         (0)     3458 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      210 2023-08-03 12:28:22.000000 edu-rdm-integration-0.2.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    15900 2023-08-04 15:43:37.008634 edu-rdm-integration-0.2.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    11460 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 15:43:36.978634 edu-rdm-integration-0.2.0/edu_rdm_integration.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    15900 2023-08-04 15:43:36.000000 edu-rdm-integration-0.2.0/edu_rdm_integration.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5345 2023-08-04 15:43:36.000000 edu-rdm-integration-0.2.0/edu_rdm_integration.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 15:43:36.000000 edu-rdm-integration-0.2.0/edu_rdm_integration.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 15:43:36.000000 edu-rdm-integration-0.2.0/edu_rdm_integration.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 15:38:21.000000 edu-rdm-integration-0.2.0/edu_rdm_integration.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      172 2023-08-04 15:43:36.000000 edu-rdm-integration-0.2.0/edu_rdm_integration.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 15:43:36.000000 edu-rdm-integration-0.2.0/edu_rdm_integration.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      112 2023-08-04 15:38:14.000000 edu-rdm-integration-0.2.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      471 2023-08-04 15:43:37.009634 edu-rdm-integration-0.2.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2778 2023-08-04 15:43:28.000000 edu-rdm-integration-0.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 15:43:36.970634 edu-rdm-integration-0.2.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 15:43:36.982634 edu-rdm-integration-0.2.0/src/edu_rdm_integration/
+-rw-r--r--   0 root         (0) root         (0)       72 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.0/src/edu_rdm_integration/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 15:43:36.987634 edu-rdm-integration-0.2.0/src/edu_rdm_integration/adapters/
+-rw-r--r--   0 root         (0) root         (0)       83 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.0/src/edu_rdm_integration/adapters/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      363 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.0/src/edu_rdm_integration/adapters/apps.py
+-rw-r--r--   0 root         (0) root         (0)     1505 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.0/src/edu_rdm_integration/adapters/caches.py
+-rw-r--r--   0 root         (0) root         (0)       66 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.0/src/edu_rdm_integration/adapters/consts.py
+-rw-r--r--   0 root         (0) root         (0)       93 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.0/src/edu_rdm_integration/adapters/enums.py
+-rw-r--r--   0 root         (0) root         (0)      255 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.0/src/edu_rdm_integration/adapters/errors.py
+-rw-r--r--   0 root         (0) root         (0)     2075 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.0/src/edu_rdm_integration/adapters/functions.py
+-rw-r--r--   0 root         (0) root         (0)     1105 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.0/src/edu_rdm_integration/adapters/helpers.py
+-rw-r--r--   0 root         (0) root         (0)      589 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.0/src/edu_rdm_integration/adapters/managers.py
+-rw-r--r--   0 root         (0) root         (0)      327 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.0/src/edu_rdm_integration/adapters/presenters.py
+-rw-r--r--   0 root         (0) root         (0)      598 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.0/src/edu_rdm_integration/adapters/receivers.py
+-rw-r--r--   0 root         (0) root         (0)      515 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.0/src/edu_rdm_integration/adapters/results.py
+-rw-r--r--   0 root         (0) root         (0)     2164 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.0/src/edu_rdm_integration/adapters/runners.py
+-rw-r--r--   0 root         (0) root         (0)     5504 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.0/src/edu_rdm_integration/adapters/strategies.py
+-rw-r--r--   0 root         (0) root         (0)      181 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.0/src/edu_rdm_integration/adapters/strings.py
+-rw-r--r--   0 root         (0) root         (0)       59 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.0/src/edu_rdm_integration/adapters/tests.py
+-rw-r--r--   0 root         (0) root         (0)      496 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.0/src/edu_rdm_integration/adapters/validators.py
+-rw-r--r--   0 root         (0) root         (0)     1822 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.0/src/edu_rdm_integration/app_settings.py
+-rw-r--r--   0 root         (0) root         (0)     2458 2023-07-24 05:38:47.000000 edu-rdm-integration-0.2.0/src/edu_rdm_integration/apps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 15:43:36.988634 edu-rdm-integration-0.2.0/src/edu_rdm_integration/collect_data/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.0/src/edu_rdm_integration/collect_data/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 15:43:36.989634 edu-rdm-integration-0.2.0/src/edu_rdm_integration/collect_data/base/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.0/src/edu_rdm_integration/collect_data/base/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1310 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.0/src/edu_rdm_integration/collect_data/base/caches.py
+-rw-r--r--   0 root         (0) root         (0)     2353 2023-07-24 05:38:47.000000 edu-rdm-integration-0.2.0/src/edu_rdm_integration/collect_data/base/functions.py
+-rw-r--r--   0 root         (0) root         (0)     5219 2023-07-24 05:38:47.000000 edu-rdm-integration-0.2.0/src/edu_rdm_integration/collect_data/base/managers.py
+-rw-r--r--   0 root         (0) root         (0)     1422 2023-07-24 05:38:47.000000 edu-rdm-integration-0.2.0/src/edu_rdm_integration/collect_data/base/runners.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 15:43:36.989634 edu-rdm-integration-0.2.0/src/edu_rdm_integration/collect_data/calculated/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.0/src/edu_rdm_integration/collect_data/calculated/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 15:43:36.995634 edu-rdm-integration-0.2.0/src/edu_rdm_integration/collect_data/calculated/base/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.0/src/edu_rdm_integration/collect_data/calculated/base/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7212 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.0/src/edu_rdm_integration/collect_data/calculated/base/caches.py
+-rw-r--r--   0 root         (0) root         (0)       84 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.0/src/edu_rdm_integration/collect_data/calculated/base/consts.py
+-rw-r--r--   0 root         (0) root         (0)       93 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.0/src/edu_rdm_integration/collect_data/calculated/base/enums.py
+-rw-r--r--   0 root         (0) root         (0)      326 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.0/src/edu_rdm_integration/collect_data/calculated/base/errors.py
+-rw-r--r--   0 root         (0) root         (0)     1670 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.0/src/edu_rdm_integration/collect_data/calculated/base/functions.py
+-rw-r--r--   0 root         (0) root         (0)     1490 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.0/src/edu_rdm_integration/collect_data/calculated/base/helpers.py
+-rw-r--r--   0 root         (0) root         (0)      838 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.0/src/edu_rdm_integration/collect_data/calculated/base/managers.py
+-rw-r--r--   0 root         (0) root         (0)      438 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.0/src/edu_rdm_integration/collect_data/calculated/base/presenters.py
+-rw-r--r--   0 root         (0) root         (0)      708 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.0/src/edu_rdm_integration/collect_data/calculated/base/results.py
+-rw-r--r--   0 root         (0) root         (0)     1648 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.0/src/edu_rdm_integration/collect_data/calculated/base/runners.py
+-rw-r--r--   0 root         (0) root         (0)      181 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.0/src/edu_rdm_integration/collect_data/calculated/base/strings.py
+-rw-r--r--   0 root         (0) root         (0)       59 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.0/src/edu_rdm_integration/collect_data/calculated/base/tests.py
+-rw-r--r--   0 root         (0) root         (0)     1057 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.0/src/edu_rdm_integration/collect_data/calculated/base/validators.py
+-rw-r--r--   0 root         (0) root         (0)     7621 2023-08-04 12:28:07.000000 edu-rdm-integration-0.2.0/src/edu_rdm_integration/collect_data/calculated/strategies.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 15:43:36.995634 edu-rdm-integration-0.2.0/src/edu_rdm_integration/collect_data/non_calculated/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.0/src/edu_rdm_integration/collect_data/non_calculated/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 15:43:37.000634 edu-rdm-integration-0.2.0/src/edu_rdm_integration/collect_data/non_calculated/base/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.0/src/edu_rdm_integration/collect_data/non_calculated/base/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5674 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.0/src/edu_rdm_integration/collect_data/non_calculated/base/caches.py
+-rw-r--r--   0 root         (0) root         (0)       66 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.0/src/edu_rdm_integration/collect_data/non_calculated/base/consts.py
+-rw-r--r--   0 root         (0) root         (0)       93 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.0/src/edu_rdm_integration/collect_data/non_calculated/base/enums.py
+-rw-r--r--   0 root         (0) root         (0)      297 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.0/src/edu_rdm_integration/collect_data/non_calculated/base/errors.py
+-rw-r--r--   0 root         (0) root         (0)     1563 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.0/src/edu_rdm_integration/collect_data/non_calculated/base/functions.py
+-rw-r--r--   0 root         (0) root         (0)     1376 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.0/src/edu_rdm_integration/collect_data/non_calculated/base/helpers.py
+-rw-r--r--   0 root         (0) root         (0)      783 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.0/src/edu_rdm_integration/collect_data/non_calculated/base/managers.py
+-rw-r--r--   0 root         (0) root         (0)      409 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.0/src/edu_rdm_integration/collect_data/non_calculated/base/presenters.py
+-rw-r--r--   0 root         (0) root         (0)      674 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.0/src/edu_rdm_integration/collect_data/non_calculated/base/results.py
+-rw-r--r--   0 root         (0) root         (0)     1541 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.0/src/edu_rdm_integration/collect_data/non_calculated/base/runners.py
+-rw-r--r--   0 root         (0) root         (0)      181 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.0/src/edu_rdm_integration/collect_data/non_calculated/base/strings.py
+-rw-r--r--   0 root         (0) root         (0)       59 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.0/src/edu_rdm_integration/collect_data/non_calculated/base/tests.py
+-rw-r--r--   0 root         (0) root         (0)      973 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.0/src/edu_rdm_integration/collect_data/non_calculated/base/validators.py
+-rw-r--r--   0 root         (0) root         (0)     7423 2023-08-04 12:28:07.000000 edu-rdm-integration-0.2.0/src/edu_rdm_integration/collect_data/non_calculated/strategies.py
+-rw-r--r--   0 root         (0) root         (0)      635 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.0/src/edu_rdm_integration/consts.py
+-rw-r--r--   0 root         (0) root         (0)     9117 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.0/src/edu_rdm_integration/entities.py
+-rw-r--r--   0 root         (0) root         (0)     4876 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.0/src/edu_rdm_integration/enums.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 15:43:37.001634 edu-rdm-integration-0.2.0/src/edu_rdm_integration/export_data/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.0/src/edu_rdm_integration/export_data/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 15:43:37.005634 edu-rdm-integration-0.2.0/src/edu_rdm_integration/export_data/base/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.0/src/edu_rdm_integration/export_data/base/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1380 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.0/src/edu_rdm_integration/export_data/base/caches.py
+-rw-r--r--   0 root         (0) root         (0)      369 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.0/src/edu_rdm_integration/export_data/base/consts.py
+-rw-r--r--   0 root         (0) root         (0)       93 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.0/src/edu_rdm_integration/export_data/base/enums.py
+-rw-r--r--   0 root         (0) root         (0)      291 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.0/src/edu_rdm_integration/export_data/base/errors.py
+-rw-r--r--   0 root         (0) root         (0)    11664 2023-07-24 05:38:47.000000 edu-rdm-integration-0.2.0/src/edu_rdm_integration/export_data/base/functions.py
+-rw-r--r--   0 root         (0) root         (0)     3076 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.0/src/edu_rdm_integration/export_data/base/helpers.py
+-rw-r--r--   0 root         (0) root         (0)     5665 2023-07-24 05:38:47.000000 edu-rdm-integration-0.2.0/src/edu_rdm_integration/export_data/base/managers.py
+-rw-r--r--   0 root         (0) root         (0)      403 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.0/src/edu_rdm_integration/export_data/base/presenters.py
+-rw-r--r--   0 root         (0) root         (0)     2548 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.0/src/edu_rdm_integration/export_data/base/requests.py
+-rw-r--r--   0 root         (0) root         (0)      662 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.0/src/edu_rdm_integration/export_data/base/results.py
+-rw-r--r--   0 root         (0) root         (0)     2716 2023-07-24 05:38:47.000000 edu-rdm-integration-0.2.0/src/edu_rdm_integration/export_data/base/runners.py
+-rw-r--r--   0 root         (0) root         (0)      181 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.0/src/edu_rdm_integration/export_data/base/strings.py
+-rw-r--r--   0 root         (0) root         (0)       59 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.0/src/edu_rdm_integration/export_data/base/tests.py
+-rw-r--r--   0 root         (0) root         (0)      961 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.0/src/edu_rdm_integration/export_data/base/validators.py
+-rw-r--r--   0 root         (0) root         (0)       16 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.0/src/edu_rdm_integration/export_data/consts.py
+-rw-r--r--   0 root         (0) root         (0)     6718 2023-08-04 12:28:07.000000 edu-rdm-integration-0.2.0/src/edu_rdm_integration/export_data/strategies.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 15:43:37.006634 edu-rdm-integration-0.2.0/src/edu_rdm_integration/management/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.0/src/edu_rdm_integration/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 15:43:37.007634 edu-rdm-integration-0.2.0/src/edu_rdm_integration/management/commands/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.0/src/edu_rdm_integration/management/commands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      487 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.0/src/edu_rdm_integration/management/commands/collect_models_data.py
+-rw-r--r--   0 root         (0) root         (0)      388 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.0/src/edu_rdm_integration/management/commands/export_entities_data.py
+-rw-r--r--   0 root         (0) root         (0)    19777 2023-07-24 05:38:47.000000 edu-rdm-integration-0.2.0/src/edu_rdm_integration/management/general.py
+-rw-r--r--   0 root         (0) root         (0)     2302 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.0/src/edu_rdm_integration/management/generators.py
+-rw-r--r--   0 root         (0) root         (0)      473 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.0/src/edu_rdm_integration/mapping.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 15:43:37.008634 edu-rdm-integration-0.2.0/src/edu_rdm_integration/migrations/
+-rw-r--r--   0 root         (0) root         (0)    18718 2023-08-03 12:28:22.000000 edu-rdm-integration-0.2.0/src/edu_rdm_integration/migrations/0001_initial.py
+-rw-r--r--   0 root         (0) root         (0)      944 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.0/src/edu_rdm_integration/migrations/0002_init_data_uploadstatus.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.0/src/edu_rdm_integration/migrations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19850 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.0/src/edu_rdm_integration/models.py
+-rw-r--r--   0 root         (0) root         (0)     6806 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.0/src/edu_rdm_integration/storages.py
+-rw-r--r--   0 root         (0) root         (0)     1936 2023-07-18 06:39:46.000000 edu-rdm-integration-0.2.0/src/edu_rdm_integration/utils.py
```

### Comparing `edu_rdm_integration-0.1.4/LICENSE` & `edu-rdm-integration-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `edu_rdm_integration-0.1.4/README.md` & `edu-rdm-integration-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `edu_rdm_integration-0.1.4/src/edu_rdm_integration/adapters/caches.py` & `edu-rdm-integration-0.2.0/src/edu_rdm_integration/adapters/caches.py`

 * *Files identical despite different names*

### Comparing `edu_rdm_integration-0.1.4/src/edu_rdm_integration/adapters/functions.py` & `edu-rdm-integration-0.2.0/src/edu_rdm_integration/adapters/functions.py`

 * *Files identical despite different names*

### Comparing `edu_rdm_integration-0.1.4/src/edu_rdm_integration/adapters/helpers.py` & `edu-rdm-integration-0.2.0/src/edu_rdm_integration/adapters/helpers.py`

 * *Files identical despite different names*

### Comparing `edu_rdm_integration-0.1.4/src/edu_rdm_integration/adapters/managers.py` & `edu-rdm-integration-0.2.0/src/edu_rdm_integration/adapters/managers.py`

 * *Files identical despite different names*

### Comparing `edu_rdm_integration-0.1.4/src/edu_rdm_integration/adapters/receivers.py` & `edu-rdm-integration-0.2.0/src/edu_rdm_integration/adapters/receivers.py`

 * *Files identical despite different names*

### Comparing `edu_rdm_integration-0.1.4/src/edu_rdm_integration/adapters/results.py` & `edu-rdm-integration-0.2.0/src/edu_rdm_integration/adapters/results.py`

 * *Files identical despite different names*

### Comparing `edu_rdm_integration-0.1.4/src/edu_rdm_integration/adapters/runners.py` & `edu-rdm-integration-0.2.0/src/edu_rdm_integration/adapters/runners.py`

 * *Files identical despite different names*

### Comparing `edu_rdm_integration-0.1.4/src/edu_rdm_integration/adapters/strategies.py` & `edu-rdm-integration-0.2.0/src/edu_rdm_integration/adapters/strategies.py`

 * *Files identical despite different names*

### Comparing `edu_rdm_integration-0.1.4/src/edu_rdm_integration/app_settings.py` & `edu-rdm-integration-0.2.0/src/edu_rdm_integration/app_settings.py`

 * *Files identical despite different names*

### Comparing `edu_rdm_integration-0.1.4/src/edu_rdm_integration/apps.py` & `edu-rdm-integration-0.2.0/src/edu_rdm_integration/apps.py`

 * *Files identical despite different names*

### Comparing `edu_rdm_integration-0.1.4/src/edu_rdm_integration/collect_data/base/caches.py` & `edu-rdm-integration-0.2.0/src/edu_rdm_integration/collect_data/base/caches.py`

 * *Files identical despite different names*

### Comparing `edu_rdm_integration-0.1.4/src/edu_rdm_integration/collect_data/base/functions.py` & `edu-rdm-integration-0.2.0/src/edu_rdm_integration/collect_data/base/functions.py`

 * *Files identical despite different names*

### Comparing `edu_rdm_integration-0.1.4/src/edu_rdm_integration/collect_data/base/managers.py` & `edu-rdm-integration-0.2.0/src/edu_rdm_integration/collect_data/base/managers.py`

 * *Files identical despite different names*

### Comparing `edu_rdm_integration-0.1.4/src/edu_rdm_integration/collect_data/base/runners.py` & `edu-rdm-integration-0.2.0/src/edu_rdm_integration/collect_data/base/runners.py`

 * *Files identical despite different names*

### Comparing `edu_rdm_integration-0.1.4/src/edu_rdm_integration/collect_data/calculated/base/caches.py` & `edu-rdm-integration-0.2.0/src/edu_rdm_integration/collect_data/calculated/base/caches.py`

 * *Files identical despite different names*

### Comparing `edu_rdm_integration-0.1.4/src/edu_rdm_integration/collect_data/calculated/base/functions.py` & `edu-rdm-integration-0.2.0/src/edu_rdm_integration/collect_data/calculated/base/functions.py`

 * *Files identical despite different names*

### Comparing `edu_rdm_integration-0.1.4/src/edu_rdm_integration/collect_data/calculated/base/helpers.py` & `edu-rdm-integration-0.2.0/src/edu_rdm_integration/collect_data/calculated/base/helpers.py`

 * *Files identical despite different names*

### Comparing `edu_rdm_integration-0.1.4/src/edu_rdm_integration/collect_data/calculated/base/managers.py` & `edu-rdm-integration-0.2.0/src/edu_rdm_integration/collect_data/calculated/base/managers.py`

 * *Files identical despite different names*

### Comparing `edu_rdm_integration-0.1.4/src/edu_rdm_integration/collect_data/calculated/base/results.py` & `edu-rdm-integration-0.2.0/src/edu_rdm_integration/collect_data/calculated/base/results.py`

 * *Files identical despite different names*

### Comparing `edu_rdm_integration-0.1.4/src/edu_rdm_integration/collect_data/calculated/base/runners.py` & `edu-rdm-integration-0.2.0/src/edu_rdm_integration/collect_data/calculated/base/runners.py`

 * *Files identical despite different names*

### Comparing `edu_rdm_integration-0.1.4/src/edu_rdm_integration/collect_data/calculated/base/validators.py` & `edu-rdm-integration-0.2.0/src/edu_rdm_integration/collect_data/calculated/base/validators.py`

 * *Files identical despite different names*

### Comparing `edu_rdm_integration-0.1.4/src/edu_rdm_integration/collect_data/non_calculated/base/caches.py` & `edu-rdm-integration-0.2.0/src/edu_rdm_integration/collect_data/non_calculated/base/caches.py`

 * *Files identical despite different names*

### Comparing `edu_rdm_integration-0.1.4/src/edu_rdm_integration/collect_data/non_calculated/base/functions.py` & `edu-rdm-integration-0.2.0/src/edu_rdm_integration/collect_data/non_calculated/base/functions.py`

 * *Files identical despite different names*

### Comparing `edu_rdm_integration-0.1.4/src/edu_rdm_integration/collect_data/non_calculated/base/helpers.py` & `edu-rdm-integration-0.2.0/src/edu_rdm_integration/collect_data/non_calculated/base/helpers.py`

 * *Files identical despite different names*

### Comparing `edu_rdm_integration-0.1.4/src/edu_rdm_integration/collect_data/non_calculated/base/managers.py` & `edu-rdm-integration-0.2.0/src/edu_rdm_integration/collect_data/non_calculated/base/managers.py`

 * *Files identical despite different names*

### Comparing `edu_rdm_integration-0.1.4/src/edu_rdm_integration/collect_data/non_calculated/base/results.py` & `edu-rdm-integration-0.2.0/src/edu_rdm_integration/collect_data/non_calculated/base/results.py`

 * *Files identical despite different names*

### Comparing `edu_rdm_integration-0.1.4/src/edu_rdm_integration/collect_data/non_calculated/base/runners.py` & `edu-rdm-integration-0.2.0/src/edu_rdm_integration/collect_data/non_calculated/base/runners.py`

 * *Files identical despite different names*

### Comparing `edu_rdm_integration-0.1.4/src/edu_rdm_integration/collect_data/non_calculated/base/validators.py` & `edu-rdm-integration-0.2.0/src/edu_rdm_integration/collect_data/non_calculated/base/validators.py`

 * *Files identical despite different names*

### Comparing `edu_rdm_integration-0.1.4/src/edu_rdm_integration/consts.py` & `edu-rdm-integration-0.2.0/src/edu_rdm_integration/consts.py`

 * *Files identical despite different names*

### Comparing `edu_rdm_integration-0.1.4/src/edu_rdm_integration/entities.py` & `edu-rdm-integration-0.2.0/src/edu_rdm_integration/entities.py`

 * *Files identical despite different names*

### Comparing `edu_rdm_integration-0.1.4/src/edu_rdm_integration/enums.py` & `edu-rdm-integration-0.2.0/src/edu_rdm_integration/enums.py`

 * *Files identical despite different names*

### Comparing `edu_rdm_integration-0.1.4/src/edu_rdm_integration/export_data/base/caches.py` & `edu-rdm-integration-0.2.0/src/edu_rdm_integration/export_data/base/caches.py`

 * *Files identical despite different names*

### Comparing `edu_rdm_integration-0.1.4/src/edu_rdm_integration/export_data/base/functions.py` & `edu-rdm-integration-0.2.0/src/edu_rdm_integration/export_data/base/functions.py`

 * *Files identical despite different names*

### Comparing `edu_rdm_integration-0.1.4/src/edu_rdm_integration/export_data/base/helpers.py` & `edu-rdm-integration-0.2.0/src/edu_rdm_integration/export_data/base/helpers.py`

 * *Files identical despite different names*

### Comparing `edu_rdm_integration-0.1.4/src/edu_rdm_integration/export_data/base/managers.py` & `edu-rdm-integration-0.2.0/src/edu_rdm_integration/export_data/base/managers.py`

 * *Files identical despite different names*

### Comparing `edu_rdm_integration-0.1.4/src/edu_rdm_integration/export_data/base/requests.py` & `edu-rdm-integration-0.2.0/src/edu_rdm_integration/export_data/base/requests.py`

 * *Files identical despite different names*

### Comparing `edu_rdm_integration-0.1.4/src/edu_rdm_integration/export_data/base/results.py` & `edu-rdm-integration-0.2.0/src/edu_rdm_integration/export_data/base/results.py`

 * *Files identical despite different names*

### Comparing `edu_rdm_integration-0.1.4/src/edu_rdm_integration/export_data/base/runners.py` & `edu-rdm-integration-0.2.0/src/edu_rdm_integration/export_data/base/runners.py`

 * *Files identical despite different names*

### Comparing `edu_rdm_integration-0.1.4/src/edu_rdm_integration/export_data/base/validators.py` & `edu-rdm-integration-0.2.0/src/edu_rdm_integration/export_data/base/validators.py`

 * *Files identical despite different names*

### Comparing `edu_rdm_integration-0.1.4/src/edu_rdm_integration/management/general.py` & `edu-rdm-integration-0.2.0/src/edu_rdm_integration/management/general.py`

 * *Files identical despite different names*

### Comparing `edu_rdm_integration-0.1.4/src/edu_rdm_integration/management/generators.py` & `edu-rdm-integration-0.2.0/src/edu_rdm_integration/management/generators.py`

 * *Files identical despite different names*

### Comparing `edu_rdm_integration-0.1.4/src/edu_rdm_integration/migrations/0001_initial.py` & `edu-rdm-integration-0.2.0/src/edu_rdm_integration/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `edu_rdm_integration-0.1.4/src/edu_rdm_integration/migrations/0002_init_data_uploadstatus.py` & `edu-rdm-integration-0.2.0/src/edu_rdm_integration/migrations/0002_init_data_uploadstatus.py`

 * *Files identical despite different names*

### Comparing `edu_rdm_integration-0.1.4/src/edu_rdm_integration/models.py` & `edu-rdm-integration-0.2.0/src/edu_rdm_integration/models.py`

 * *Files identical despite different names*

### Comparing `edu_rdm_integration-0.1.4/src/edu_rdm_integration/storages.py` & `edu-rdm-integration-0.2.0/src/edu_rdm_integration/storages.py`

 * *Files identical despite different names*

### Comparing `edu_rdm_integration-0.1.4/src/edu_rdm_integration/utils.py` & `edu-rdm-integration-0.2.0/src/edu_rdm_integration/utils.py`

 * *Files identical despite different names*

### Comparing `edu_rdm_integration-0.1.4/PKG-INFO` & `edu-rdm-integration-0.2.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 Metadata-Version: 2.1
 Name: edu-rdm-integration
-Version: 0.1.4
+Version: 0.2.0
 Summary: Интеграция с Региональной витриной данных
-License: MIT
+Home-page: 
+Download-URL: 
 Author: BARS Group
-Requires-Python: >=3.7,<4.0
-Classifier: License :: OSI Approved :: MIT License
+Author-email: bars@bars.group
+Platform: Any
+Classifier: Development Status :: 3 - Alpha
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
+Classifier: Intended Audience :: Developers
+Classifier: Environment :: Console
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # Проект "Интеграция с Региональной витриной данных"
 
 ## Описание концепции
 
 ## Принцип работы
 
@@ -171,8 +176,110 @@
 ## Настройка PyCharm для работы
 
 ## Запуск в системе
 
 ## Запуск в контейнере
 
 ## Правила внесения изменений
+# История изменений
+Все изменения проекта должны быть отражены в этом файле.
 
+Формат основан на [Keep a Changelog](http://keepachangelog.com/)
+и проект следует [Семантическому версионированию](http://semver.org/).
+
+## [x.y.z] - гггг-мм-дд
+ 
+Здесь должно быть расширенное описание того, что было сделано, какие есть планы у команды по дальнейшему развитию. 
+Желательно будущие цели привязывать к конкретным задачам. Т.е. на каждую цель нужно поставить отдельную задачу и 
+отразить ее номер здесь.
+ 
+### Добавлено
+- [ПРОЕКТ-ZZZZ](https://jira.bars.group/browse/ПРОЕКТ-ZZZZ)
+  PATCH Название задачи или изменения.
+
+- [ПРОЕКТ-YYYY](https://jira.bars.group/browse/ПРОЕКТ-YYYY)
+  MINOR Название задачи или изменения.
+
+- [ПРОЕКТ-XXXX](https://jira.bars.group/browse/ПРОЕКТ-XXXX)
+  MAJOR Название задачи или изменения.
+ 
+### Изменено
+ 
+### Исправлено
+
+
+
+## [0.2.0] - 2023-08-04
+
+Перенос стратегий формирования Функций используемых в генерации исходников.
+ 
+### Добавлено
+
+- [EDUSCHL-19919](https://jira.bars.group/browse/EDUSCHL-19919)
+  MINOR Перенесены стратегии создания Функций из ЭШ.
+
+ 
+### Изменено
+ 
+### Исправлено
+
+
+## [0.1.4] - 2023-08-03
+ 
+Возвращение ранее удаленных зависимостей миграции
+ 
+### Добавлено
+
+### Изменено
+
+- [EDUSCHL-20209](https://jira.bars.group/browse/EDUSCHL-20209)
+  PATCH Возвращение зависимостей миграции.
+
+- [EDUSCHL-20209](https://jira.bars.group/browse/EDUSCHL-20209)
+  PATCH Доработки по формированию документации.
+
+- [EDUSCHL-20200](https://jira.bars.group/browse/EDUSCHL-20200)
+  Закреплены версии зависимостей, добавлена ссылка на uploader-client
+ 
+### Исправлено
+
+
+
+## [0.1.3] - 2023-07-24
+ 
+Для раскатки миграций на ЭШ, пришлось закомментировать зависимости в initial-миграции. 
+ 
+### Добавлено
+ 
+### Изменено
+
+- [EDUSCHL-19919](https://jira.bars.group/browse/EDUSCHL-19919)
+  PATCH Вынести общую часть для работы с РВД из ЭШ для использования в ЭК.
+ 
+### Исправлено
+
+## [0.1.2] - 2023-07-23
+
+Внесены изменения в кодовую базу после переноса механизма логирования из ЭШ в educommon.
+
+### Добавлено
+
+### Изменено
+
+- [EDUSCHL-19919](https://jira.bars.group/browse/EDUSCHL-19919)
+  PATCH Вынести общую часть для работы с РВД из ЭШ для использования в ЭК.
+
+### Исправлено
+
+
+## [0.1.0] - 2023-07-18
+
+Внесены изменения в кодовую базу после переноса механизма логирования из ЭШ в educommon.
+
+### Добавлено
+
+- [EDUSCHL-19919](https://jira.bars.group/browse/EDUSCHL-19919)
+  MINOR Перенос базовых компонентов интеграции с РВД из ЭШ.
+
+### Изменено
+
+### Исправлено
```

