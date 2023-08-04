# Comparing `tmp/bw_matchbox-0.4.0.tar.gz` & `tmp/bw_matchbox-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bw_matchbox-0.4.0.tar", last modified: Thu Aug  3 20:46:27 2023, max compression
+gzip compressed data, was "bw_matchbox-0.5.0.tar", last modified: Fri Aug  4 13:03:39 2023, max compression
```

## Comparing `bw_matchbox-0.4.0.tar` & `bw_matchbox-0.5.0.tar`

### file list

```diff
@@ -1,79 +1,82 @@
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-03 20:46:27.899150 bw_matchbox-0.4.0/
--rw-r--r--   0 chrismutel   (501) staff       (20)     1067 2023-06-20 12:26:53.000000 bw_matchbox-0.4.0/LICENSE
--rw-r--r--   0 chrismutel   (501) staff       (20)      226 2023-08-02 21:05:25.000000 bw_matchbox-0.4.0/MANIFEST.in
--rw-r--r--   0 chrismutel   (501) staff       (20)     6349 2023-08-03 20:46:27.899222 bw_matchbox-0.4.0/PKG-INFO
--rw-r--r--   0 chrismutel   (501) staff       (20)     5325 2023-08-01 07:10:26.000000 bw_matchbox-0.4.0/README.md
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-03 20:46:27.887092 bw_matchbox-0.4.0/bw_matchbox/
--rw-r--r--   0 chrismutel   (501) staff       (20)        6 2023-08-03 20:45:33.000000 bw_matchbox-0.4.0/bw_matchbox/VERSION
--rw-r--r--   0 chrismutel   (501) staff       (20)      215 2023-08-01 17:17:21.000000 bw_matchbox-0.4.0/bw_matchbox/__init__.py
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-03 20:46:27.885300 bw_matchbox-0.4.0/bw_matchbox/assets/
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-03 20:46:27.889036 bw_matchbox-0.4.0/bw_matchbox/assets/css/
--rw-r--r--   0 chrismutel   (501) staff       (20)     1891 2023-08-03 20:45:26.000000 bw_matchbox-0.4.0/bw_matchbox/assets/css/common.css
--rw-r--r--   0 chrismutel   (501) staff       (20)     6452 2023-08-03 20:45:26.000000 bw_matchbox-0.4.0/bw_matchbox/assets/css/compare.css
--rw-r--r--   0 chrismutel   (501) staff       (20)      640 2023-08-03 20:45:26.000000 bw_matchbox-0.4.0/bw_matchbox/assets/css/customizations.css
--rw-r--r--   0 chrismutel   (501) staff       (20)     2251 2023-08-03 20:45:26.000000 bw_matchbox-0.4.0/bw_matchbox/assets/css/modal.css
--rw-r--r--   0 chrismutel   (501) staff       (20)     7618 2023-08-01 07:10:26.000000 bw_matchbox-0.4.0/bw_matchbox/assets/css/normalize.css
--rw-r--r--   0 chrismutel   (501) staff       (20)     3243 2023-08-03 20:45:26.000000 bw_matchbox-0.4.0/bw_matchbox/assets/css/processes-list.css
--rw-r--r--   0 chrismutel   (501) staff       (20)    11556 2023-08-01 07:10:26.000000 bw_matchbox-0.4.0/bw_matchbox/assets/css/skeleton.css
--rw-r--r--   0 chrismutel   (501) staff       (20)      916 2023-08-01 07:10:26.000000 bw_matchbox-0.4.0/bw_matchbox/assets/css/tooltip.css
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-03 20:46:27.889316 bw_matchbox-0.4.0/bw_matchbox/assets/images/
--rw-r--r--   0 chrismutel   (501) staff       (20)    32038 2023-06-20 12:27:44.000000 bw_matchbox-0.4.0/bw_matchbox/assets/images/favicon.ico
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-03 20:46:27.885139 bw_matchbox-0.4.0/bw_matchbox/assets/js/
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-03 20:46:27.890162 bw_matchbox-0.4.0/bw_matchbox/assets/js/Compare/
--rw-r--r--   0 chrismutel   (501) staff       (20)    22750 2023-08-03 20:45:26.000000 bw_matchbox-0.4.0/bw_matchbox/assets/js/Compare/CompareCore.js
--rw-r--r--   0 chrismutel   (501) staff       (20)     1251 2023-08-03 20:45:26.000000 bw_matchbox-0.4.0/bw_matchbox/assets/js/Compare/CompareRowClick.js
--rw-r--r--   0 chrismutel   (501) staff       (20)    11340 2023-08-03 20:45:26.000000 bw_matchbox-0.4.0/bw_matchbox/assets/js/Compare/CompareRowsHelpers.js
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-03 20:46:27.891438 bw_matchbox-0.4.0/bw_matchbox/assets/js/ProcessesList/
--rw-r--r--   0 chrismutel   (501) staff       (20)     3578 2023-08-03 20:45:26.000000 bw_matchbox-0.4.0/bw_matchbox/assets/js/ProcessesList/ProcessesList.js
--rw-r--r--   0 chrismutel   (501) staff       (20)      497 2023-08-03 20:45:26.000000 bw_matchbox-0.4.0/bw_matchbox/assets/js/ProcessesList/ProcessesListConstants.js
--rw-r--r--   0 chrismutel   (501) staff       (20)      993 2023-08-03 20:45:26.000000 bw_matchbox-0.4.0/bw_matchbox/assets/js/ProcessesList/ProcessesListData.js
--rw-r--r--   0 chrismutel   (501) staff       (20)     4710 2023-08-03 20:45:26.000000 bw_matchbox-0.4.0/bw_matchbox/assets/js/ProcessesList/ProcessesListDataLoad.js
--rw-r--r--   0 chrismutel   (501) staff       (20)     4675 2023-08-03 20:45:26.000000 bw_matchbox-0.4.0/bw_matchbox/assets/js/ProcessesList/ProcessesListDataRender.js
--rw-r--r--   0 chrismutel   (501) staff       (20)     1128 2023-08-03 20:45:26.000000 bw_matchbox-0.4.0/bw_matchbox/assets/js/ProcessesList/ProcessesListNodes.js
--rw-r--r--   0 chrismutel   (501) staff       (20)     4909 2023-08-03 20:45:26.000000 bw_matchbox-0.4.0/bw_matchbox/assets/js/ProcessesList/ProcessesListPagination.UNUSED.js
--rw-r--r--   0 chrismutel   (501) staff       (20)     2523 2023-08-03 20:45:26.000000 bw_matchbox-0.4.0/bw_matchbox/assets/js/ProcessesList/ProcessesListSearch.js
--rw-r--r--   0 chrismutel   (501) staff       (20)     3775 2023-08-03 20:45:26.000000 bw_matchbox-0.4.0/bw_matchbox/assets/js/ProcessesList/ProcessesListStates.js
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-03 20:46:27.891584 bw_matchbox-0.4.0/bw_matchbox/assets/js/common/
--rw-r--r--   0 chrismutel   (501) staff       (20)     4947 2023-08-03 20:45:26.000000 bw_matchbox-0.4.0/bw_matchbox/assets/js/common/CommonHelpers.js
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-03 20:46:27.885185 bw_matchbox-0.4.0/bw_matchbox/assets/js/libs/
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-03 20:46:27.891870 bw_matchbox-0.4.0/bw_matchbox/assets/js/libs/ym/
--rw-r--r--   0 chrismutel   (501) staff       (20)    13286 2023-08-03 20:45:26.000000 bw_matchbox-0.4.0/bw_matchbox/assets/js/libs/ym/ym-modules-0.1.2.js
--rw-r--r--   0 chrismutel   (501) staff       (20)     6018 2023-08-03 20:45:26.000000 bw_matchbox-0.4.0/bw_matchbox/assets/js/libs/ym/ym-modules-0.1.2.min.js
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-03 20:46:27.894594 bw_matchbox-0.4.0/bw_matchbox/assets/templates/
--rw-r--r--   0 chrismutel   (501) staff       (20)     3901 2023-08-03 20:45:26.000000 bw_matchbox-0.4.0/bw_matchbox/assets/templates/compare.html
--rw-r--r--   0 chrismutel   (501) staff       (20)     2566 2023-07-23 12:42:57.000000 bw_matchbox-0.4.0/bw_matchbox/assets/templates/databases.html
--rw-r--r--   0 chrismutel   (501) staff       (20)      461 2023-07-23 15:09:13.000000 bw_matchbox-0.4.0/bw_matchbox/assets/templates/expand.html
--rw-r--r--   0 chrismutel   (501) staff       (20)       16 2023-06-20 12:27:44.000000 bw_matchbox-0.4.0/bw_matchbox/assets/templates/footer.html
--rw-r--r--   0 chrismutel   (501) staff       (20)     2660 2023-08-03 20:45:26.000000 bw_matchbox-0.4.0/bw_matchbox/assets/templates/header.html
--rw-r--r--   0 chrismutel   (501) staff       (20)     4347 2023-08-03 20:45:26.000000 bw_matchbox-0.4.0/bw_matchbox/assets/templates/index.html
--rw-r--r--   0 chrismutel   (501) staff       (20)      733 2023-06-21 04:56:26.000000 bw_matchbox-0.4.0/bw_matchbox/assets/templates/match-status.html
--rw-r--r--   0 chrismutel   (501) staff       (20)     1721 2023-08-03 20:45:26.000000 bw_matchbox-0.4.0/bw_matchbox/assets/templates/match.html
--rw-r--r--   0 chrismutel   (501) staff       (20)      798 2023-07-23 12:44:06.000000 bw_matchbox-0.4.0/bw_matchbox/assets/templates/navigation.html
--rw-r--r--   0 chrismutel   (501) staff       (20)     3536 2023-08-01 11:49:18.000000 bw_matchbox-0.4.0/bw_matchbox/assets/templates/process_detail.html
--rw-r--r--   0 chrismutel   (501) staff       (20)      599 2023-07-22 21:06:00.000000 bw_matchbox-0.4.0/bw_matchbox/assets/templates/project.html
--rw-r--r--   0 chrismutel   (501) staff       (20)      412 2023-08-01 07:10:26.000000 bw_matchbox-0.4.0/bw_matchbox/assets/templates/search-embedded.html
--rw-r--r--   0 chrismutel   (501) staff       (20)      850 2023-06-20 12:27:44.000000 bw_matchbox-0.4.0/bw_matchbox/assets/templates/search.html
--rw-r--r--   0 chrismutel   (501) staff       (20)      947 2023-06-20 12:27:44.000000 bw_matchbox-0.4.0/bw_matchbox/assets/templates/search_result.html
--rw-r--r--   0 chrismutel   (501) staff       (20)     1243 2023-07-23 08:33:52.000000 bw_matchbox-0.4.0/bw_matchbox/assets/templates/select_files.html
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-03 20:46:27.894886 bw_matchbox-0.4.0/bw_matchbox/bin/
--rw-r--r--   0 chrismutel   (501) staff       (20)        0 2023-06-20 12:27:44.000000 bw_matchbox-0.4.0/bw_matchbox/bin/__init__.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     2931 2023-08-01 17:17:21.000000 bw_matchbox-0.4.0/bw_matchbox/bin/matchbox.py
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-03 20:46:27.896879 bw_matchbox-0.4.0/bw_matchbox/data/
--rw-r--r--   0 chrismutel   (501) staff       (20)   123246 2023-08-01 17:17:21.000000 bw_matchbox-0.4.0/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-mining.json
--rw-r--r--   0 chrismutel   (501) staff       (20)    93862 2023-07-23 09:30:53.000000 bw_matchbox-0.4.0/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-string-matching.json
--rw-r--r--   0 chrismutel   (501) staff       (20)   116072 2023-08-01 17:17:21.000000 bw_matchbox-0.4.0/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-transport.json
--rw-r--r--   0 chrismutel   (501) staff       (20)      603 2023-07-23 09:34:59.000000 bw_matchbox-0.4.0/bw_matchbox/data/dare.json
--rw-r--r--   0 chrismutel   (501) staff       (20)     1388 2023-08-01 17:17:21.000000 bw_matchbox-0.4.0/bw_matchbox/utils.py
--rw-r--r--   0 chrismutel   (501) staff       (20)    20517 2023-08-01 17:17:21.000000 bw_matchbox-0.4.0/bw_matchbox/webapp.py
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-03 20:46:27.898041 bw_matchbox-0.4.0/bw_matchbox.egg-info/
--rw-r--r--   0 chrismutel   (501) staff       (20)     6349 2023-08-03 20:46:27.000000 bw_matchbox-0.4.0/bw_matchbox.egg-info/PKG-INFO
--rw-r--r--   0 chrismutel   (501) staff       (20)     4694 2023-08-03 20:46:27.000000 bw_matchbox-0.4.0/bw_matchbox.egg-info/SOURCES.txt
--rw-r--r--   0 chrismutel   (501) staff       (20)        1 2023-08-03 20:46:27.000000 bw_matchbox-0.4.0/bw_matchbox.egg-info/dependency_links.txt
--rw-r--r--   0 chrismutel   (501) staff       (20)       59 2023-08-03 20:46:27.000000 bw_matchbox-0.4.0/bw_matchbox.egg-info/entry_points.txt
--rw-r--r--   0 chrismutel   (501) staff       (20)        1 2023-07-23 07:30:31.000000 bw_matchbox-0.4.0/bw_matchbox.egg-info/not-zip-safe
--rw-r--r--   0 chrismutel   (501) staff       (20)      167 2023-08-03 20:46:27.000000 bw_matchbox-0.4.0/bw_matchbox.egg-info/requires.txt
--rw-r--r--   0 chrismutel   (501) staff       (20)       12 2023-08-03 20:46:27.000000 bw_matchbox-0.4.0/bw_matchbox.egg-info/top_level.txt
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-03 20:46:27.897109 bw_matchbox-0.4.0/docs/
--rw-r--r--   0 chrismutel   (501) staff       (20)     1145 2023-07-23 07:23:19.000000 bw_matchbox-0.4.0/docs/conf.py
--rw-r--r--   0 chrismutel   (501) staff       (20)       87 2023-06-20 12:26:53.000000 bw_matchbox-0.4.0/pyproject.toml
--rw-r--r--   0 chrismutel   (501) staff       (20)     1900 2023-08-03 20:46:27.899662 bw_matchbox-0.4.0/setup.cfg
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-04 13:03:39.597715 bw_matchbox-0.5.0/
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1067 2023-06-20 12:26:53.000000 bw_matchbox-0.5.0/LICENSE
+-rw-r--r--   0 chrismutel   (501) staff       (20)      226 2023-08-02 21:05:25.000000 bw_matchbox-0.5.0/MANIFEST.in
+-rw-r--r--   0 chrismutel   (501) staff       (20)     6349 2023-08-04 13:03:39.597768 bw_matchbox-0.5.0/PKG-INFO
+-rw-r--r--   0 chrismutel   (501) staff       (20)     5325 2023-08-01 07:10:26.000000 bw_matchbox-0.5.0/README.md
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-04 13:03:39.581874 bw_matchbox-0.5.0/bw_matchbox/
+-rw-r--r--   0 chrismutel   (501) staff       (20)        6 2023-08-04 13:03:17.000000 bw_matchbox-0.5.0/bw_matchbox/VERSION
+-rw-r--r--   0 chrismutel   (501) staff       (20)      215 2023-08-01 17:17:21.000000 bw_matchbox-0.5.0/bw_matchbox/__init__.py
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-04 13:03:39.579888 bw_matchbox-0.5.0/bw_matchbox/assets/
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-04 13:03:39.585126 bw_matchbox-0.5.0/bw_matchbox/assets/css/
+-rw-r--r--   0 chrismutel   (501) staff       (20)     3291 2023-08-04 13:00:53.000000 bw_matchbox-0.5.0/bw_matchbox/assets/css/common-modal.css
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1891 2023-08-03 20:45:26.000000 bw_matchbox-0.5.0/bw_matchbox/assets/css/common.css
+-rw-r--r--   0 chrismutel   (501) staff       (20)     3834 2023-08-04 13:00:53.000000 bw_matchbox-0.5.0/bw_matchbox/assets/css/compare.css
+-rw-r--r--   0 chrismutel   (501) staff       (20)      640 2023-08-03 20:45:26.000000 bw_matchbox-0.5.0/bw_matchbox/assets/css/customizations.css
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1392 2023-08-04 13:00:53.000000 bw_matchbox-0.5.0/bw_matchbox/assets/css/fixed-table.css
+-rw-r--r--   0 chrismutel   (501) staff       (20)     7618 2023-08-01 07:10:26.000000 bw_matchbox-0.5.0/bw_matchbox/assets/css/normalize.css
+-rw-r--r--   0 chrismutel   (501) staff       (20)     3353 2023-08-04 13:00:53.000000 bw_matchbox-0.5.0/bw_matchbox/assets/css/processes-list.css
+-rw-r--r--   0 chrismutel   (501) staff       (20)    11556 2023-08-01 07:10:26.000000 bw_matchbox-0.5.0/bw_matchbox/assets/css/skeleton.css
+-rw-r--r--   0 chrismutel   (501) staff       (20)      916 2023-08-01 07:10:26.000000 bw_matchbox-0.5.0/bw_matchbox/assets/css/tooltip.css
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-04 13:03:39.585317 bw_matchbox-0.5.0/bw_matchbox/assets/images/
+-rw-r--r--   0 chrismutel   (501) staff       (20)    32038 2023-06-20 12:27:44.000000 bw_matchbox-0.5.0/bw_matchbox/assets/images/favicon.ico
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-04 13:03:39.579781 bw_matchbox-0.5.0/bw_matchbox/assets/js/
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-04 13:03:39.586325 bw_matchbox-0.5.0/bw_matchbox/assets/js/Compare/
+-rw-r--r--   0 chrismutel   (501) staff       (20)    23101 2023-08-04 13:00:53.000000 bw_matchbox-0.5.0/bw_matchbox/assets/js/Compare/CompareCore.js
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1251 2023-08-03 20:45:26.000000 bw_matchbox-0.5.0/bw_matchbox/assets/js/Compare/CompareRowClick.js
+-rw-r--r--   0 chrismutel   (501) staff       (20)    11340 2023-08-03 20:45:26.000000 bw_matchbox-0.5.0/bw_matchbox/assets/js/Compare/CompareRowsHelpers.js
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-04 13:03:39.588646 bw_matchbox-0.5.0/bw_matchbox/assets/js/ProcessesList/
+-rw-r--r--   0 chrismutel   (501) staff       (20)     3578 2023-08-03 20:45:26.000000 bw_matchbox-0.5.0/bw_matchbox/assets/js/ProcessesList/ProcessesList.js
+-rw-r--r--   0 chrismutel   (501) staff       (20)      497 2023-08-04 13:00:53.000000 bw_matchbox-0.5.0/bw_matchbox/assets/js/ProcessesList/ProcessesListConstants.js
+-rw-r--r--   0 chrismutel   (501) staff       (20)      993 2023-08-03 20:45:26.000000 bw_matchbox-0.5.0/bw_matchbox/assets/js/ProcessesList/ProcessesListData.js
+-rw-r--r--   0 chrismutel   (501) staff       (20)     4710 2023-08-03 20:45:26.000000 bw_matchbox-0.5.0/bw_matchbox/assets/js/ProcessesList/ProcessesListDataLoad.js
+-rw-r--r--   0 chrismutel   (501) staff       (20)     3494 2023-08-04 13:00:53.000000 bw_matchbox-0.5.0/bw_matchbox/assets/js/ProcessesList/ProcessesListDataRender.js
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1128 2023-08-03 20:45:26.000000 bw_matchbox-0.5.0/bw_matchbox/assets/js/ProcessesList/ProcessesListNodes.js
+-rw-r--r--   0 chrismutel   (501) staff       (20)     4909 2023-08-03 20:45:26.000000 bw_matchbox-0.5.0/bw_matchbox/assets/js/ProcessesList/ProcessesListPagination.UNUSED.js
+-rw-r--r--   0 chrismutel   (501) staff       (20)     2523 2023-08-03 20:45:26.000000 bw_matchbox-0.5.0/bw_matchbox/assets/js/ProcessesList/ProcessesListSearch.js
+-rw-r--r--   0 chrismutel   (501) staff       (20)     3775 2023-08-03 20:45:26.000000 bw_matchbox-0.5.0/bw_matchbox/assets/js/ProcessesList/ProcessesListStates.js
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-04 13:03:39.588980 bw_matchbox-0.5.0/bw_matchbox/assets/js/common/
+-rw-r--r--   0 chrismutel   (501) staff       (20)     5634 2023-08-04 13:00:53.000000 bw_matchbox-0.5.0/bw_matchbox/assets/js/common/CommonHelpers.js
+-rw-r--r--   0 chrismutel   (501) staff       (20)     5782 2023-08-04 13:00:53.000000 bw_matchbox-0.5.0/bw_matchbox/assets/js/common/CommonModal.js
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-04 13:03:39.579824 bw_matchbox-0.5.0/bw_matchbox/assets/js/libs/
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-04 13:03:39.589299 bw_matchbox-0.5.0/bw_matchbox/assets/js/libs/ym/
+-rw-r--r--   0 chrismutel   (501) staff       (20)    13286 2023-08-03 20:45:26.000000 bw_matchbox-0.5.0/bw_matchbox/assets/js/libs/ym/ym-modules-0.1.2.js
+-rw-r--r--   0 chrismutel   (501) staff       (20)     6018 2023-08-03 20:45:26.000000 bw_matchbox-0.5.0/bw_matchbox/assets/js/libs/ym/ym-modules-0.1.2.min.js
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-04 13:03:39.593005 bw_matchbox-0.5.0/bw_matchbox/assets/templates/
+-rw-r--r--   0 chrismutel   (501) staff       (20)      756 2023-08-04 13:00:53.000000 bw_matchbox-0.5.0/bw_matchbox/assets/templates/common-modal.html
+-rw-r--r--   0 chrismutel   (501) staff       (20)     3760 2023-08-04 13:00:53.000000 bw_matchbox-0.5.0/bw_matchbox/assets/templates/compare.html
+-rw-r--r--   0 chrismutel   (501) staff       (20)     2566 2023-07-23 12:42:57.000000 bw_matchbox-0.5.0/bw_matchbox/assets/templates/databases.html
+-rw-r--r--   0 chrismutel   (501) staff       (20)      461 2023-07-23 15:09:13.000000 bw_matchbox-0.5.0/bw_matchbox/assets/templates/expand.html
+-rw-r--r--   0 chrismutel   (501) staff       (20)       16 2023-06-20 12:27:44.000000 bw_matchbox-0.5.0/bw_matchbox/assets/templates/footer.html
+-rw-r--r--   0 chrismutel   (501) staff       (20)     2666 2023-08-04 13:00:53.000000 bw_matchbox-0.5.0/bw_matchbox/assets/templates/header.html
+-rw-r--r--   0 chrismutel   (501) staff       (20)     4442 2023-08-04 13:00:53.000000 bw_matchbox-0.5.0/bw_matchbox/assets/templates/index.html
+-rw-r--r--   0 chrismutel   (501) staff       (20)      733 2023-06-21 04:56:26.000000 bw_matchbox-0.5.0/bw_matchbox/assets/templates/match-status.html
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1721 2023-08-03 20:45:26.000000 bw_matchbox-0.5.0/bw_matchbox/assets/templates/match.html
+-rw-r--r--   0 chrismutel   (501) staff       (20)      798 2023-07-23 12:44:06.000000 bw_matchbox-0.5.0/bw_matchbox/assets/templates/navigation.html
+-rw-r--r--   0 chrismutel   (501) staff       (20)     3583 2023-08-04 09:48:51.000000 bw_matchbox-0.5.0/bw_matchbox/assets/templates/process_detail.html
+-rw-r--r--   0 chrismutel   (501) staff       (20)      599 2023-07-22 21:06:00.000000 bw_matchbox-0.5.0/bw_matchbox/assets/templates/project.html
+-rw-r--r--   0 chrismutel   (501) staff       (20)      412 2023-08-01 07:10:26.000000 bw_matchbox-0.5.0/bw_matchbox/assets/templates/search-embedded.html
+-rw-r--r--   0 chrismutel   (501) staff       (20)      850 2023-06-20 12:27:44.000000 bw_matchbox-0.5.0/bw_matchbox/assets/templates/search.html
+-rw-r--r--   0 chrismutel   (501) staff       (20)      947 2023-06-20 12:27:44.000000 bw_matchbox-0.5.0/bw_matchbox/assets/templates/search_result.html
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1243 2023-07-23 08:33:52.000000 bw_matchbox-0.5.0/bw_matchbox/assets/templates/select_files.html
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-04 13:03:39.593523 bw_matchbox-0.5.0/bw_matchbox/bin/
+-rw-r--r--   0 chrismutel   (501) staff       (20)        0 2023-06-20 12:27:44.000000 bw_matchbox-0.5.0/bw_matchbox/bin/__init__.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     2931 2023-08-01 17:17:21.000000 bw_matchbox-0.5.0/bw_matchbox/bin/matchbox.py
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-04 13:03:39.595358 bw_matchbox-0.5.0/bw_matchbox/data/
+-rw-r--r--   0 chrismutel   (501) staff       (20)   123246 2023-08-01 17:17:21.000000 bw_matchbox-0.5.0/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-mining.json
+-rw-r--r--   0 chrismutel   (501) staff       (20)    93862 2023-07-23 09:30:53.000000 bw_matchbox-0.5.0/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-string-matching.json
+-rw-r--r--   0 chrismutel   (501) staff       (20)   116072 2023-08-01 17:17:21.000000 bw_matchbox-0.5.0/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-transport.json
+-rw-r--r--   0 chrismutel   (501) staff       (20)      603 2023-07-23 09:34:59.000000 bw_matchbox-0.5.0/bw_matchbox/data/dare.json
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1388 2023-08-01 17:17:21.000000 bw_matchbox-0.5.0/bw_matchbox/utils.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)    20822 2023-08-04 13:01:12.000000 bw_matchbox-0.5.0/bw_matchbox/webapp.py
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-04 13:03:39.596636 bw_matchbox-0.5.0/bw_matchbox.egg-info/
+-rw-r--r--   0 chrismutel   (501) staff       (20)     6349 2023-08-04 13:03:39.000000 bw_matchbox-0.5.0/bw_matchbox.egg-info/PKG-INFO
+-rw-r--r--   0 chrismutel   (501) staff       (20)     4974 2023-08-04 13:03:39.000000 bw_matchbox-0.5.0/bw_matchbox.egg-info/SOURCES.txt
+-rw-r--r--   0 chrismutel   (501) staff       (20)        1 2023-08-04 13:03:39.000000 bw_matchbox-0.5.0/bw_matchbox.egg-info/dependency_links.txt
+-rw-r--r--   0 chrismutel   (501) staff       (20)       59 2023-08-04 13:03:39.000000 bw_matchbox-0.5.0/bw_matchbox.egg-info/entry_points.txt
+-rw-r--r--   0 chrismutel   (501) staff       (20)        1 2023-07-23 07:30:31.000000 bw_matchbox-0.5.0/bw_matchbox.egg-info/not-zip-safe
+-rw-r--r--   0 chrismutel   (501) staff       (20)      167 2023-08-04 13:03:39.000000 bw_matchbox-0.5.0/bw_matchbox.egg-info/requires.txt
+-rw-r--r--   0 chrismutel   (501) staff       (20)       12 2023-08-04 13:03:39.000000 bw_matchbox-0.5.0/bw_matchbox.egg-info/top_level.txt
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-04 13:03:39.595605 bw_matchbox-0.5.0/docs/
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1145 2023-07-23 07:23:19.000000 bw_matchbox-0.5.0/docs/conf.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)       87 2023-06-20 12:26:53.000000 bw_matchbox-0.5.0/pyproject.toml
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1900 2023-08-04 13:03:39.598136 bw_matchbox-0.5.0/setup.cfg
```

### Comparing `bw_matchbox-0.4.0/LICENSE` & `bw_matchbox-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.4.0/PKG-INFO` & `bw_matchbox-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bw_matchbox
-Version: 0.4.0
+Version: 0.5.0
 Summary: Browser to match Brightway databases
 Home-page: https://github.com/cauldron/bw_matchbox
 Author: Chris Mutel
 Author-email: <cmutel@gmail.com>
 Maintainer: Chris Mutel
 Maintainer-email: <cmutel@gmail.com>
 License: MIT
```

### Comparing `bw_matchbox-0.4.0/README.md` & `bw_matchbox-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.4.0/bw_matchbox/assets/css/common.css` & `bw_matchbox-0.5.0/bw_matchbox/assets/css/common.css`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.4.0/bw_matchbox/assets/css/customizations.css` & `bw_matchbox-0.5.0/bw_matchbox/assets/css/customizations.css`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.4.0/bw_matchbox/assets/css/normalize.css` & `bw_matchbox-0.5.0/bw_matchbox/assets/css/normalize.css`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.4.0/bw_matchbox/assets/css/processes-list.css` & `bw_matchbox-0.5.0/bw_matchbox/assets/css/processes-list.css`

 * *Files 3% similar despite different names*

```diff
@@ -35,14 +35,19 @@
   opacity: 0;
 }
 
 /* Table */
 .processes-list-table {
   margin-bottom: 0;
 }
+.processes-list-table tr td:last-child div > .button {
+  display: block;
+  width: 100%;
+  margin-bottom: 0;
+}
 
 /* Filter controls section */
 .processes-list .page-filters label {
   display: inline-block;
   margin-left: 4px;
   margin-right: 8px;
 }
```

### Comparing `bw_matchbox-0.4.0/bw_matchbox/assets/css/skeleton.css` & `bw_matchbox-0.5.0/bw_matchbox/assets/css/skeleton.css`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.4.0/bw_matchbox/assets/css/tooltip.css` & `bw_matchbox-0.5.0/bw_matchbox/assets/css/tooltip.css`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.4.0/bw_matchbox/assets/images/favicon.ico` & `bw_matchbox-0.5.0/bw_matchbox/assets/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.4.0/bw_matchbox/assets/js/Compare/CompareCore.js` & `bw_matchbox-0.5.0/bw_matchbox/assets/js/Compare/CompareCore.js`

 * *Files 9% similar despite different names*

#### js-beautify {}

```diff
@@ -1,21 +1,23 @@
 modules.define(
     'CompareCore',
     [
         // Required modules...
         'CommonHelpers',
-        'CompareRowsHelpers',
+        'CommonModal',
         'CompareRowClick',
+        'CompareRowsHelpers',
     ],
     function provide_CompareCore(
         provide,
         // Resolved modules...
         CommonHelpers,
-        CompareRowsHelpers,
+        CommonModal,
         CompareRowClick,
+        CompareRowsHelpers,
     ) {
         /* Compare tables feature code (via global variable `CompareCore`).
          *
          * Mouse handler methods are used:
          * - CompareRowsHelpers.clickRow -- Click on regular row to select or collapse selected rows.
          * - CompareRowsHelpers.clickUncollapseRow -- Click on collapsed row handler to uncollapse.
          * - CompareRowClick.disableRowClick -- To disable row click effect (if we have some nested interactive elements).
@@ -51,15 +53,14 @@
             sharedData: undefined, // Initializing in `CompareCore.start` from `bw_matchbox/assets/templates/compare.html`
 
             // Counter for making unique records (see `replaceWithTarget`)
             targetNodesCounter: 0,
 
             // Local data...
             comment: '',
-            modal: undefined, // HTMLDivElement -- modal window node
 
             // Methods...
 
             shiftRow(event, row, row_id) {
                 CompareRowClick.disableRowClick();
                 // Add row from source to target array
                 event.preventDefault();
@@ -99,18 +100,35 @@
                 const rowKind = is_target ? 'target' : 'source';
                 const collapsedId = CompareRowsHelpers.getCollapsedId(rowKind, rowId);
                 if (collapsed && !collapsedRows[collapsedId] && collapsedRows[collapsedId] !== false) {
                     const otherRowKind = !is_target ? 'target' : 'source';
                     const otherTableDataKey = otherRowKind + '_data';
                     const otherTableData = this.sharedData[otherTableDataKey];
                     const collapsedGroupId = data['collapsed-group'];
-                    const otherRowId = otherTableData.findIndex(
+                    /* // ORIGONAL BUG: Don't use indices as row_id's!
+                     * const otherRowId = otherTableData.findIndex(
+                     *   (other) => other['collapsed-group'] === collapsedGroupId,
+                     * );
+                     */
+                    const otherRowData = otherTableData.find(
                         (other) => other['collapsed-group'] === collapsedGroupId,
                     );
-                    // const otherRowData = otherRowId !== -1 && otherTableData[otherRowId]; // UNUSED
+                    if (!otherRowData) {
+                        throw new Error('Cannot find other collapsed record');
+                    }
+                    const otherRowId = otherRowData.row_id;
+                    /* console.log('[CompareCore:buildRow] check', {
+                     *   otherRowId,
+                     *   otherRowKind,
+                     *   otherTableDataKey,
+                     *   otherTableData,
+                     *   collapsedGroupId,
+                     *   otherRowData,
+                     * });
+                     */
                     const otherCollapsedId = CompareRowsHelpers.getCollapsedId(otherRowKind, otherRowId);
                     collapsedRows[collapsedId] = {
                         rowKind,
                         rowId,
                         pairId: otherRowId,
                         // rowEl, // OBSOLETE: Avoid of use it.
                     };
@@ -268,68 +286,78 @@
                 });
             },
 
             createProxyFunc(event) {
                 event.preventDefault();
                 const {
                     target_name,
-                    comment,
+                    // comment,
                     source_node_unit,
                     source_node_location,
                     target_data,
                     source_id,
                 } = this.sharedData;
-                const span = document.getElementById('modal-content-wrapper');
-                const title = 'Proxy name';
+                const {
+                    comment
+                } = this;
                 const name =
                     'Proxy for ' +
                     target_name
                     .replace('Market group for ', '')
                     .replace('market group for ', '')
                     .replace('Market for ', '')
                     .replace('market for ', '')
                     .trim();
-                let text = `
+
+                const begin = `
           <form>
-            <!--
-            <label for="proxy-name">${title}</label>
-            -->
             <input class="u-full-width" type="text" id="proxy-name" name="proxy-name" value="${name}">
             <label for="proxy-comment">Comment</label>
             <textarea class="u-full-width" id="proxy-comment" name="proxy-comment">${comment}</textarea>
             <p><button class="button-primary" id="create-proxy-submit-button">Create Proxy Process</button>
             | Unit: ${source_node_unit}
             | Location: ${source_node_location}</p>
-            <table width="100%">
-              <tr>
-                <th>Name</th>
-                <th>Amount</th>
-                <th>Comment</th>
-              </tr>
+            <table id="proxy-table" class="fixed-table" width="100%">
+              <thead>
+                <tr>
+                  <th>Name</th>
+                  <th>Amount</th>
+                  <th>Comment</th>
+                </tr>
+              </thead>
+              <tbody>
         `;
 
-                target_data.forEach(function(item, _index) {
-                    text += `
+                const rows = target_data.map(function(item, _index) {
+                    return `
               <tr input_id=${item.input_id}>
                 <td><div>${item.name}</div></td>
                 <td><div>${item.amount_display}</div></td>
                 <td><div><textarea type="text" id="proxy-name-${item.input_id}" name="proxy-name-${item.input_id}"></textarea></div></td>
               </tr>
           `;
                 });
 
-                text += `
+                const end = `
+              </tbody>
             </table>
           </form>
         `;
-                span.innerHTML = text;
 
-                this.showModal({
-                    title
-                });
+                const title = 'Proxy name';
+                const content = begin + rows.join('') + end;
+
+                CommonModal.setModalContentId('proxy-dialog-modal')
+                    .setTitle(title)
+                    .setModalContentOptions({
+                        scrollable: true,
+                        padded: true,
+                    })
+                    .setContent(content)
+                    .showModal();
 
                 const submit = document.getElementById('create-proxy-submit-button');
                 submit.addEventListener('click', async (e) => {
                     e.preventDefault();
                     const submission_data = {
                         exchanges: target_data,
                         source: source_id,
@@ -452,52 +480,48 @@
                 } = this.sharedData;
                 CompareRowClick.disableRowClick();
                 const rowId = elem.getAttribute('row_id');
                 const current = Number(document.getElementById('number-current-amount').innerText);
                 const item = target_data.find(({
                     row_id
                 }) => row_id === rowId);
-                const itemOrig = {
-                    ...item
-                };
                 if (item) {
                     item.amount = current;
                     item.amount_display = current.toExponential();
                 }
-                console.log('[CompareCore:setNumber]', {
-                    itemOrig,
-                    item,
-                    rowId,
-                    current,
-                });
+                // TODO: Number formatting is weird here. It would be nice to fix it.
+                /* console.log('[CompareCore:setNumber]', {
+                 *   // itemOrig,
+                 *   item,
+                 *   rowId,
+                 *   current,
+                 * });
+                 */
                 // this.modal.style.display = 'none';
-                this.hideModal();
+                CommonModal.hideModal();
                 this.sortTable(target_data);
                 this.buildTable('target-table', target_data, true);
             },
 
             editNumber(link) {
+                CompareRowClick.disableRowClick();
                 const {
                     source_data,
                     target_data
                 } = this.sharedData;
                 const td = link.closest('td');
-                CompareRowClick.disableRowClick();
                 const rowId = td.getAttribute('row_id');
                 const row = target_data.find(({
                     row_id
                 }) => row_id == rowId);
-                const span = document.getElementById('modal-content-wrapper');
-
-                const title = [row.name, row.location, row.unit].filter(Boolean).join(' | ');
 
                 let start = `
           <div>
             <p>Click on a row to take that value</p>
-            <table class="modal-table" width="100%">
+            <table id="edit-number-table" class="fixed-table modal-table" width="100%">
               <thead>
                 <tr>
                   <th>Amount</th>
                   <th>Name</th>
                   <th>Unit</th>
                 </tr>
               </thead>
@@ -535,55 +559,42 @@
                 <input type="number" id="rescale_number" value="1.0">
                 <button onClick="CompareCore.rescaleAmount(${row.row_id})" id="rescale-button">Rescale</button>
               </div>
             </form>
           </div>
         `;
 
-                span.innerHTML = start + end;
+                const title = [row.name, row.location, row.unit].filter(Boolean).join(' | ');
+                const content = start + end;
+
+                CommonModal.setModalContentId('set-number-modal')
+                    .setTitle(title)
+                    .setModalContentOptions({
+                        // Scrollings and paddings will be set for inner components particaluary.
+                        scrollable: false,
+                        padded: false,
+                    })
+                    .setContent(content)
+                    .showModal();
 
+                // Set modal handlers...
                 const boundStop = this.stop.bind(this);
                 document.getElementById('rescale-button').addEventListener('click', boundStop, false);
                 document.getElementById('new-number-button').addEventListener('click', boundStop, false);
                 document.getElementById('close-number-editor').addEventListener('click', boundStop, false);
-
-                this.showModal({
-                    title
-                });
+                // TODO: To integrate this code (`event.preventDefault()`) into the
+                // handlers (`rescaleAmount`, `setNewNumber`, `setNumber`), by refactor
+                // handlers to get stored `row_id`, and get event object from arguments
+                // instead.
             },
 
             stop(event) {
                 event.preventDefault();
             },
 
-            /** showModal -- Show modal window
-             * @param {object} [params] - Modal parameters
-             * @param {string} [params.title] - Modal title
-             */
-            showModal(params = {}) {
-                const {
-                    title
-                } = params;
-                // this.modal.style.display = 'block';
-                this.modal.classList.toggle('show', true);
-                document.body.classList.toggle('has-modal', true);
-                // Update title (if passed)...
-                if (title) {
-                    const titleEl = this.modal.getElementsByClassName('modal-title')[0];
-                    if (titleEl) {
-                        titleEl.innerHTML = title;
-                    }
-                }
-            },
-
-            hideModal() {
-                this.modal.classList.toggle('show', false);
-                document.body.classList.toggle('has-modal', false);
-            },
-
             // Start...
 
             /** start -- Initialize compare feature (entry point)
              * @param {object} sharedData -- See initialization in `bw_matchbox/assets/templates/compare.html`
              */
             start(sharedData) {
                 // Save public data...
@@ -606,27 +617,18 @@
                 // Create tables...
                 this.buildTable('source-table', source_data, false);
                 this.buildTable('target-table', target_data, true);
 
                 // Button handlers...
                 document
                     .getElementById('save-mapping-button')
-                    .addEventListener('click', this.createProxyFunc, false);
+                    .addEventListener('click', this.createProxyFunc.bind(this), false);
                 document
                     .getElementById('one-to-one')
-                    .addEventListener('click', this.createOneToOneProxyFunc, false);
-
-                // Get modal node...
-                this.modal = document.getElementById('modal-number-editor');
-
-                // Link close modal button handler (TODO: To use more specific class name?)...
-                const closer = this.modal.getElementsByClassName('close')[0];
-                if (closer) {
-                    closer.onclick = this.hideModal.bind(this);
-                }
+                    .addEventListener('click', this.createOneToOneProxyFunc.bind(this), false);
             },
 
             // Re-exported handlers for access from the html code (only core module is exposed as global)...
 
             /** clickRow
              * @param {<TRowEl>} rowEl
              */
```

### Comparing `bw_matchbox-0.4.0/bw_matchbox/assets/js/Compare/CompareRowClick.js` & `bw_matchbox-0.5.0/bw_matchbox/assets/js/Compare/CompareRowClick.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.4.0/bw_matchbox/assets/js/Compare/CompareRowsHelpers.js` & `bw_matchbox-0.5.0/bw_matchbox/assets/js/Compare/CompareRowsHelpers.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.4.0/bw_matchbox/assets/js/ProcessesList/ProcessesList.js` & `bw_matchbox-0.5.0/bw_matchbox/assets/js/ProcessesList/ProcessesList.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.4.0/bw_matchbox/assets/js/ProcessesList/ProcessesListData.js` & `bw_matchbox-0.5.0/bw_matchbox/assets/js/ProcessesList/ProcessesListData.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.4.0/bw_matchbox/assets/js/ProcessesList/ProcessesListDataLoad.js` & `bw_matchbox-0.5.0/bw_matchbox/assets/js/ProcessesList/ProcessesListDataLoad.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.4.0/bw_matchbox/assets/js/ProcessesList/ProcessesListNodes.js` & `bw_matchbox-0.5.0/bw_matchbox/assets/js/ProcessesList/ProcessesListNodes.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.4.0/bw_matchbox/assets/js/ProcessesList/ProcessesListPagination.UNUSED.js` & `bw_matchbox-0.5.0/bw_matchbox/assets/js/ProcessesList/ProcessesListPagination.UNUSED.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.4.0/bw_matchbox/assets/js/ProcessesList/ProcessesListSearch.js` & `bw_matchbox-0.5.0/bw_matchbox/assets/js/ProcessesList/ProcessesListSearch.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.4.0/bw_matchbox/assets/js/ProcessesList/ProcessesListStates.js` & `bw_matchbox-0.5.0/bw_matchbox/assets/js/ProcessesList/ProcessesListStates.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.4.0/bw_matchbox/assets/js/common/CommonHelpers.js` & `bw_matchbox-0.5.0/bw_matchbox/assets/js/common/CommonHelpers.js`

 * *Files 11% similar despite different names*

#### js-beautify {}

```diff
@@ -63,14 +63,35 @@
                     html = html.join('');
                 }
                 html = html.trim(); // Never return a text node of whitespace as the result
                 template.innerHTML = html;
                 const content = template.content;
                 return content.children;
             },
+
+            /** updateNodeContent -- Replace all inner dom node content.
+             * @param {HTMLElement} node
+             * @param {string|HTMLElement|HTMLElement[]} content
+             */
+            updateNodeContent(node, content) {
+                if (!node) {
+                    throw new Error('Undefined node to update content');
+                }
+                if (typeof content === 'string') {
+                    // Replace with string content...
+                    node.innerHTML = content;
+                } else if (Array.isArray(content)) {
+                    // Replace multiple elements...
+                    node.replaceChildren.apply(node, content);
+                } else {
+                    // Replace single element...
+                    node.replaceChildren(content);
+                }
+            },
+
             /** decodeQuery
              * @param {string | string[]} qs
              * @param {string} sep
              * @param {string} eq
              * @param {any} options
              * @returns {{}}
              */
```

### Comparing `bw_matchbox-0.4.0/bw_matchbox/assets/js/libs/ym/ym-modules-0.1.2.js` & `bw_matchbox-0.5.0/bw_matchbox/assets/js/libs/ym/ym-modules-0.1.2.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.4.0/bw_matchbox/assets/js/libs/ym/ym-modules-0.1.2.min.js` & `bw_matchbox-0.5.0/bw_matchbox/assets/js/libs/ym/ym-modules-0.1.2.min.js`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.4.0/bw_matchbox/assets/templates/compare.html` & `bw_matchbox-0.5.0/bw_matchbox/assets/templates/compare.html`

 * *Files 18% similar despite different names*

```diff
@@ -1,58 +1,51 @@
 {% include 'header.html' %}
 
+{# Common dependencies... #}
+
+{% include 'common-modal.html' %}
+
+{# Module-specific dependencies... #}
+
 <link rel="stylesheet" href="{{ url_for('static', filename='css/compare.css') }}">
 
 <script src="{{ url_for('static', filename='js/Compare/CompareRowsHelpers.js') }}"></script>
 <script src="{{ url_for('static', filename='js/Compare/CompareRowClick.js') }}"></script>
 <script src="{{ url_for('static', filename='js/Compare/CompareCore.js') }}"></script>
 
 {# Core js module:
   - `CompareCore` (from `bw_matchbox/assets/js/compare-core.js`)
 #}
 
-<div class="modal-wrapper">
-  <div class="modal" id="modal-number-editor">
-    <div class="modal-splash"></div>
-    <div class="modal-window">
-      <div class="modal-header">
-        <h3 class="modal-title">Modal title</h3>
-        <div class="close">&times;</div>
-      </div>
-      <div class="modal-content non-padded non-scrollable">
-        <div id="modal-content-wrapper">
-          Sample content
-        </div>
-      </div>
-    </div>
-  </div>
-</div>
-
 <div class="container compare">
   {% include 'navigation.html' %}
   <div class="row">
     <div class="four columns">
-      <h4>Location: {% if source_node.location == target_node.location %}Same{% else %}{{ source_node.location }} | {{ target_node.location }}{% endif %}</h4>
+      <h4>Location: {% if source_node.location == target_node.location %}Same{% else %}{{ source_node.location }}
+        | {{ target_node.location }}{% endif %}</h4>
     </div>
     <div class="three columns">
-      <h4>Unit: {% if source_node.unit == target_node.unit %}Same{% else %}{{ source_node.unit }} | {{ target_node.unit }}{% endif %}</h4>
+      <h4>Unit: {% if source_node.unit == target_node.unit %}Same{% else %}{{ source_node.unit }}
+        | {{ target_node.unit }}{% endif %}</h4>
     </div>
     <div class="five columns">
-      <button class="button-primary" id="save-mapping-button">{% if proxy and proxy != "None" %}Create Proxy</button> <button class="button-primary" id="one-to-one">1-to-1 Proxy</button>{% else %}Save{% endif %}</button>
+    <button class="button-primary" id="save-mapping-button">{% if proxy and proxy != "None" %}Create Proxy</button>
+    <button class="button-primary" id="one-to-one">1-to-1 Proxy</button>{% else %}Save{% endif %}</button>
     </div>
   </div>
   <div class="row compare-tables">
     <div class="column one-half">
-      <h3>{{ source_node.name }}</h3>
-      <table class="compare-table" id="source-table" width="100%">
+      <h3><a href="{{ url_for('process_detail', id=source_node.id) }}">{{ source_node.name }}</a></h3>
+      <table class="fixed-table fixed-table-active compare-table" id="source-table" width="100%">
       </table>
     </div>
     <div class="column one-half">
-      <h3>{{ target_node.name }} <span onclick="CompareCore.replaceWithTarget(this)"><a><i class="fa-solid fa-arrow-up"></i></a></span></h3>
-      <table class="compare-table" id="target-table" width="100%">
+      <h3><a href="{{ url_for('process_detail', id=target_node.id) }}">{{ target_node.name }}</a>
+      <span onclick="CompareCore.replaceWithTarget(this)"><a><i class="fa-solid fa-arrow-up"></i></a></span></h3>
+      <table class="fixed-table fixed-table-active compare-table" id="target-table" width="100%">
       </table>
     </div>
   </div>
 </div>
 
 <script>
   modules.require('CompareCore', (CompareCore) => {
```

#### html2text {}

```diff
@@ -1,16 +1,14 @@
-{% include 'header.html' %}
+{% include 'header.html' %} {# Common dependencies... #} {% include 'common-
+modal.html' %} {# Module-specific dependencies... #}
  {# Core js module: - `CompareCore` (from `bw_matchbox/assets/js/compare-
 core.js`) #}
-**** Modal title ****
-×
-Sample content
 {% include 'navigation.html' %}
 *** Location: {% if source_node.location == target_node.location %}Same{% else
 %}{{ source_node.location }} | {{ target_node.location }}{% endif %} ***
 *** Unit: {% if source_node.unit == target_node.unit %}Same{% else %}{
 { source_node.unit }} | {{ target_node.unit }}{% endif %} ***
 {% if proxy and proxy != "None" %}Create Proxy 1-to-1 Proxy{% else %}Save{%
 endif %}
-**** {{ source_node.name }} ****
-{{ target_node.name }}
+**** {{_source_node.name_}} ****
+{{_target_node.name_}}
  {% include 'footer.html' %}
```

### Comparing `bw_matchbox-0.4.0/bw_matchbox/assets/templates/databases.html` & `bw_matchbox-0.5.0/bw_matchbox/assets/templates/databases.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.4.0/bw_matchbox/assets/templates/header.html` & `bw_matchbox-0.5.0/bw_matchbox/assets/templates/header.html`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
   <!-- CSS
   –––––––––––––––––––––––––––––––––––––––––––––––––– -->
   <link rel="stylesheet" href="{{ url_for('static', filename='css/normalize.css') }}">
   <link rel="stylesheet" href="{{ url_for('static', filename='css/tooltip.css') }}">
   <link rel="stylesheet" href="{{ url_for('static', filename='css/skeleton.css') }}">
   <link rel="stylesheet" href="{{ url_for('static', filename='css/customizations.css') }}">
   <link rel="stylesheet" href="{{ url_for('static', filename='css/common.css') }}">
-  <link rel="stylesheet" href="{{ url_for('static', filename='css/modal.css') }}">
+  <link rel="stylesheet" href="{{ url_for('static', filename='css/fixed-table.css') }}">
 
   <!-- Scripts
   –––––––––––––––––––––––––––––––––––––––––––––––––– -->
   <script src="{{ url_for('static', filename='js/libs/ym/ym-modules-0.1.2.min.js') }}"></script>
   <script src="{{ url_for('static', filename='js/common/CommonHelpers.js') }}"></script>
   {# TODO: to move to the body end? #}
```

### Comparing `bw_matchbox-0.4.0/bw_matchbox/assets/templates/index.html` & `bw_matchbox-0.5.0/bw_matchbox/assets/templates/index.html`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 {% include 'header.html' %}
 
+{# Module-specific dependencies... #}
+
 <link rel="stylesheet" href="{{ url_for('static', filename='css/processes-list.css') }}">
 
 <script src="{{ url_for('static', filename='js/ProcessesList/ProcessesListConstants.js') }}"></script>
 <script src="{{ url_for('static', filename='js/ProcessesList/ProcessesListData.js') }}"></script>
 <script src="{{ url_for('static', filename='js/ProcessesList/ProcessesListDataLoad.js') }}"></script>
 <script src="{{ url_for('static', filename='js/ProcessesList/ProcessesListDataRender.js') }}"></script>
 <script src="{{ url_for('static', filename='js/ProcessesList/ProcessesListNodes.js') }}"></script>
@@ -45,21 +47,21 @@
         <label for="order_by_location">Location</label>
         <input type="radio" name="order_by" id="order_by_product" value="product" onChange="ProcessesList.onOrderByChange(this)">
         <label for="order_by_product">Product</label>
       </div>
       <div id="processes-list-error" class="error">
         <!-- Error text comes here -->
       </div>
-      <table id="processes-list-table" class="processes-list-table" width="100%">
+      <table id="processes-list-table" class="fixed-table processes-list-table" width="100%">
         <thead>
           <tr>
-            <th>Name</th>
-            <th>Location</th>
-            <th>Unit</th>
-            <th>Matched</th>
+            <th><div>Name</div></th>
+            <th><div>Location</div></th>
+            <th><div>Unit</div></th>
+            <th><div>Matched</div></th>
           </tr>
         </thead>
         <tbody id="processes-list-table-body">
           {# NOTE: Content is dynamically populated in client's js code, see `ProcessesListDataRender` #}
         </tbody>
       </table>
       <div class="bottom-actions">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-{% include 'header.html' %}
+{% include 'header.html' %} {# Module-specific dependencies... #}
  {# UNUSED ProcessesListPagination -- Using incremental data loading
  #} {# Core module: - `ProcessesList` (from `bw_matchbox/assets/js/
 ProcessesList.js`) #}
 {% include 'navigation.html' %}
 ****** {% if unmatched_link %}Source Database (Only_unmatched) {% else
 %}Unmatched in Source Database {% endif %} ******
 [{{ query_string }}  ]
```

### Comparing `bw_matchbox-0.4.0/bw_matchbox/assets/templates/match-status.html` & `bw_matchbox-0.5.0/bw_matchbox/assets/templates/match-status.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.4.0/bw_matchbox/assets/templates/match.html` & `bw_matchbox-0.5.0/bw_matchbox/assets/templates/match.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.4.0/bw_matchbox/assets/templates/navigation.html` & `bw_matchbox-0.5.0/bw_matchbox/assets/templates/navigation.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.4.0/bw_matchbox/assets/templates/process_detail.html` & `bw_matchbox-0.5.0/bw_matchbox/assets/templates/process_detail.html`

 * *Files 9% similar despite different names*

```diff
@@ -79,15 +79,15 @@
       </table>
     </div>
   </div>
 </div>
 
 <script type="text/javascript">
 function markMatched (button) {
-  var url = "/mark-matched/{{ ds.id }}";
+  var url = "{{ url_for('add_attribute', id=ds.id, attr='matched', value='1')|safe }}";
   fetch(url).then((response) => {
     if (!response.ok) {
         throw new Error(`HTTP error ${response.status}`);
     };
     button.innerText = "Matched";
     button.classList.remove("button-primary");
   });
```

### Comparing `bw_matchbox-0.4.0/bw_matchbox/assets/templates/project.html` & `bw_matchbox-0.5.0/bw_matchbox/assets/templates/project.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.4.0/bw_matchbox/assets/templates/search.html` & `bw_matchbox-0.5.0/bw_matchbox/assets/templates/search.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.4.0/bw_matchbox/assets/templates/search_result.html` & `bw_matchbox-0.5.0/bw_matchbox/assets/templates/search_result.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.4.0/bw_matchbox/assets/templates/select_files.html` & `bw_matchbox-0.5.0/bw_matchbox/assets/templates/select_files.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.4.0/bw_matchbox/bin/matchbox.py` & `bw_matchbox-0.5.0/bw_matchbox/bin/matchbox.py`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.4.0/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-mining.json` & `bw_matchbox-0.5.0/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-mining.json`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.4.0/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-string-matching.json` & `bw_matchbox-0.5.0/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-string-matching.json`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.4.0/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-transport.json` & `bw_matchbox-0.5.0/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-transport.json`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.4.0/bw_matchbox/data/dare.json` & `bw_matchbox-0.5.0/bw_matchbox/data/dare.json`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.4.0/bw_matchbox/utils.py` & `bw_matchbox-0.5.0/bw_matchbox/utils.py`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.4.0/bw_matchbox/webapp.py` & `bw_matchbox-0.5.0/bw_matchbox/webapp.py`

 * *Files 2% similar despite different names*

```diff
@@ -416,22 +416,33 @@
             title="bw_matchbox Search Result",
             table_data=bd.Database(search_db).search(q, limit=100),
             query_string=q,
             database=s,
         )
 
 
-@matchbox_app.route("/mark-matched/<id>", methods=["GET"])
+@matchbox_app.route("/add-attribute/<id>", methods=["GET"])
 @auth.login_required
-def mark_matched(id):
+def add_attribute(id):
     context = get_context()
     proj, s, t, proxy = context
     bd.projects.set_current(proj)
     node = bd.get_node(id=id)
-    node["matched"] = True
+
+    attr = flask.request.args.get("attr")
+    value = flask.request.args.get("value")
+
+    if attr is None or value is None:
+        flask.abort(400)
+    if attr in ("highlighted", "matched"):
+        if value not in ("0", "1"):
+            flask.abort(400)
+        value = {"0": False, "1": True}[value]
+
+    node[attr] = value
     node.save()
     return ""
 
 
 @matchbox_app.route("/process/<id>", methods=["GET"])
 @auth.login_required
 def process_detail(id):
```

### Comparing `bw_matchbox-0.4.0/bw_matchbox.egg-info/PKG-INFO` & `bw_matchbox-0.5.0/bw_matchbox.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bw-matchbox
-Version: 0.4.0
+Version: 0.5.0
 Summary: Browser to match Brightway databases
 Home-page: https://github.com/cauldron/bw_matchbox
 Author: Chris Mutel
 Author-email: <cmutel@gmail.com>
 Maintainer: Chris Mutel
 Maintainer-email: <cmutel@gmail.com>
 License: MIT
```

### Comparing `bw_matchbox-0.4.0/bw_matchbox.egg-info/SOURCES.txt` & `bw_matchbox-0.5.0/bw_matchbox.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -3,18 +3,19 @@
 README.md
 pyproject.toml
 setup.cfg
 ./bw_matchbox/VERSION
 ./bw_matchbox/__init__.py
 ./bw_matchbox/utils.py
 ./bw_matchbox/webapp.py
+./bw_matchbox/assets/css/common-modal.css
 ./bw_matchbox/assets/css/common.css
 ./bw_matchbox/assets/css/compare.css
 ./bw_matchbox/assets/css/customizations.css
-./bw_matchbox/assets/css/modal.css
+./bw_matchbox/assets/css/fixed-table.css
 ./bw_matchbox/assets/css/normalize.css
 ./bw_matchbox/assets/css/processes-list.css
 ./bw_matchbox/assets/css/skeleton.css
 ./bw_matchbox/assets/css/tooltip.css
 ./bw_matchbox/assets/images/favicon.ico
 ./bw_matchbox/assets/js/Compare/CompareCore.js
 ./bw_matchbox/assets/js/Compare/CompareRowClick.js
@@ -25,16 +26,18 @@
 ./bw_matchbox/assets/js/ProcessesList/ProcessesListDataLoad.js
 ./bw_matchbox/assets/js/ProcessesList/ProcessesListDataRender.js
 ./bw_matchbox/assets/js/ProcessesList/ProcessesListNodes.js
 ./bw_matchbox/assets/js/ProcessesList/ProcessesListPagination.UNUSED.js
 ./bw_matchbox/assets/js/ProcessesList/ProcessesListSearch.js
 ./bw_matchbox/assets/js/ProcessesList/ProcessesListStates.js
 ./bw_matchbox/assets/js/common/CommonHelpers.js
+./bw_matchbox/assets/js/common/CommonModal.js
 ./bw_matchbox/assets/js/libs/ym/ym-modules-0.1.2.js
 ./bw_matchbox/assets/js/libs/ym/ym-modules-0.1.2.min.js
+./bw_matchbox/assets/templates/common-modal.html
 ./bw_matchbox/assets/templates/compare.html
 ./bw_matchbox/assets/templates/databases.html
 ./bw_matchbox/assets/templates/expand.html
 ./bw_matchbox/assets/templates/footer.html
 ./bw_matchbox/assets/templates/header.html
 ./bw_matchbox/assets/templates/index.html
 ./bw_matchbox/assets/templates/match-status.html
@@ -57,18 +60,19 @@
 bw_matchbox.egg-info/PKG-INFO
 bw_matchbox.egg-info/SOURCES.txt
 bw_matchbox.egg-info/dependency_links.txt
 bw_matchbox.egg-info/entry_points.txt
 bw_matchbox.egg-info/not-zip-safe
 bw_matchbox.egg-info/requires.txt
 bw_matchbox.egg-info/top_level.txt
+bw_matchbox/assets/css/common-modal.css
 bw_matchbox/assets/css/common.css
 bw_matchbox/assets/css/compare.css
 bw_matchbox/assets/css/customizations.css
-bw_matchbox/assets/css/modal.css
+bw_matchbox/assets/css/fixed-table.css
 bw_matchbox/assets/css/normalize.css
 bw_matchbox/assets/css/processes-list.css
 bw_matchbox/assets/css/skeleton.css
 bw_matchbox/assets/css/tooltip.css
 bw_matchbox/assets/images/favicon.ico
 bw_matchbox/assets/js/Compare/CompareCore.js
 bw_matchbox/assets/js/Compare/CompareRowClick.js
@@ -79,16 +83,18 @@
 bw_matchbox/assets/js/ProcessesList/ProcessesListDataLoad.js
 bw_matchbox/assets/js/ProcessesList/ProcessesListDataRender.js
 bw_matchbox/assets/js/ProcessesList/ProcessesListNodes.js
 bw_matchbox/assets/js/ProcessesList/ProcessesListPagination.UNUSED.js
 bw_matchbox/assets/js/ProcessesList/ProcessesListSearch.js
 bw_matchbox/assets/js/ProcessesList/ProcessesListStates.js
 bw_matchbox/assets/js/common/CommonHelpers.js
+bw_matchbox/assets/js/common/CommonModal.js
 bw_matchbox/assets/js/libs/ym/ym-modules-0.1.2.js
 bw_matchbox/assets/js/libs/ym/ym-modules-0.1.2.min.js
+bw_matchbox/assets/templates/common-modal.html
 bw_matchbox/assets/templates/compare.html
 bw_matchbox/assets/templates/databases.html
 bw_matchbox/assets/templates/expand.html
 bw_matchbox/assets/templates/footer.html
 bw_matchbox/assets/templates/header.html
 bw_matchbox/assets/templates/index.html
 bw_matchbox/assets/templates/match-status.html
```

### Comparing `bw_matchbox-0.4.0/docs/conf.py` & `bw_matchbox-0.5.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.4.0/setup.cfg` & `bw_matchbox-0.5.0/setup.cfg`

 * *Files identical despite different names*

