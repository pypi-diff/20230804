# Comparing `tmp/bw_matchbox-0.3.0.tar.gz` & `tmp/bw_matchbox-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bw_matchbox-0.3.0.tar", last modified: Wed Aug  2 21:10:16 2023, max compression
+gzip compressed data, was "bw_matchbox-0.4.0.tar", last modified: Thu Aug  3 20:46:27 2023, max compression
```

## Comparing `bw_matchbox-0.3.0.tar` & `bw_matchbox-0.4.0.tar`

### file list

```diff
@@ -1,74 +1,79 @@
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-02 21:10:16.457498 bw_matchbox-0.3.0/
--rw-r--r--   0 chrismutel   (501) staff       (20)     1067 2023-06-20 12:26:53.000000 bw_matchbox-0.3.0/LICENSE
--rw-r--r--   0 chrismutel   (501) staff       (20)      226 2023-08-02 21:05:25.000000 bw_matchbox-0.3.0/MANIFEST.in
--rw-r--r--   0 chrismutel   (501) staff       (20)     6349 2023-08-02 21:10:16.457621 bw_matchbox-0.3.0/PKG-INFO
--rw-r--r--   0 chrismutel   (501) staff       (20)     5325 2023-08-01 07:10:26.000000 bw_matchbox-0.3.0/README.md
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-02 21:10:16.438184 bw_matchbox-0.3.0/bw_matchbox/
--rw-r--r--   0 chrismutel   (501) staff       (20)        6 2023-08-02 21:10:10.000000 bw_matchbox-0.3.0/bw_matchbox/VERSION
--rw-r--r--   0 chrismutel   (501) staff       (20)      215 2023-08-01 17:17:21.000000 bw_matchbox-0.3.0/bw_matchbox/__init__.py
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-02 21:10:16.435615 bw_matchbox-0.3.0/bw_matchbox/assets/
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-02 21:10:16.440408 bw_matchbox-0.3.0/bw_matchbox/assets/css/
--rw-r--r--   0 chrismutel   (501) staff       (20)     2144 2023-08-02 20:57:45.000000 bw_matchbox-0.3.0/bw_matchbox/assets/css/common.css
--rw-r--r--   0 chrismutel   (501) staff       (20)     5022 2023-08-02 20:57:45.000000 bw_matchbox-0.3.0/bw_matchbox/assets/css/compare.css
--rw-r--r--   0 chrismutel   (501) staff       (20)     1501 2023-08-01 07:10:26.000000 bw_matchbox-0.3.0/bw_matchbox/assets/css/customizations.css
--rw-r--r--   0 chrismutel   (501) staff       (20)     7618 2023-08-01 07:10:26.000000 bw_matchbox-0.3.0/bw_matchbox/assets/css/normalize.css
--rw-r--r--   0 chrismutel   (501) staff       (20)     3320 2023-08-02 20:57:45.000000 bw_matchbox-0.3.0/bw_matchbox/assets/css/processes-list.css
--rw-r--r--   0 chrismutel   (501) staff       (20)    11556 2023-08-01 07:10:26.000000 bw_matchbox-0.3.0/bw_matchbox/assets/css/skeleton.css
--rw-r--r--   0 chrismutel   (501) staff       (20)      916 2023-08-01 07:10:26.000000 bw_matchbox-0.3.0/bw_matchbox/assets/css/tooltip.css
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-02 21:10:16.440580 bw_matchbox-0.3.0/bw_matchbox/assets/images/
--rw-r--r--   0 chrismutel   (501) staff       (20)    32038 2023-06-20 12:27:44.000000 bw_matchbox-0.3.0/bw_matchbox/assets/images/favicon.ico
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-02 21:10:16.441127 bw_matchbox-0.3.0/bw_matchbox/assets/js/
--rw-r--r--   0 chrismutel   (501) staff       (20)     4283 2023-08-02 20:57:45.000000 bw_matchbox-0.3.0/bw_matchbox/assets/js/CommonHelpers.js
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-02 21:10:16.443479 bw_matchbox-0.3.0/bw_matchbox/assets/js/Compare/
--rw-r--r--   0 chrismutel   (501) staff       (20)    18042 2023-08-02 20:57:45.000000 bw_matchbox-0.3.0/bw_matchbox/assets/js/Compare/CompareCore.js
--rw-r--r--   0 chrismutel   (501) staff       (20)      946 2023-08-02 20:57:45.000000 bw_matchbox-0.3.0/bw_matchbox/assets/js/Compare/CompareRowClick.js
--rw-r--r--   0 chrismutel   (501) staff       (20)    10108 2023-08-02 20:57:45.000000 bw_matchbox-0.3.0/bw_matchbox/assets/js/Compare/CompareRowsHelpers.js
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-02 21:10:16.444803 bw_matchbox-0.3.0/bw_matchbox/assets/js/ProcessesList/
--rw-r--r--   0 chrismutel   (501) staff       (20)     2764 2023-08-02 20:57:45.000000 bw_matchbox-0.3.0/bw_matchbox/assets/js/ProcessesList/ProcessesList.js
--rw-r--r--   0 chrismutel   (501) staff       (20)      269 2023-08-02 20:57:45.000000 bw_matchbox-0.3.0/bw_matchbox/assets/js/ProcessesList/ProcessesListConstants.js
--rw-r--r--   0 chrismutel   (501) staff       (20)      651 2023-08-02 20:57:45.000000 bw_matchbox-0.3.0/bw_matchbox/assets/js/ProcessesList/ProcessesListData.js
--rw-r--r--   0 chrismutel   (501) staff       (20)     3867 2023-08-02 20:57:45.000000 bw_matchbox-0.3.0/bw_matchbox/assets/js/ProcessesList/ProcessesListDataLoad.js
--rw-r--r--   0 chrismutel   (501) staff       (20)     3968 2023-08-02 20:57:45.000000 bw_matchbox-0.3.0/bw_matchbox/assets/js/ProcessesList/ProcessesListDataRender.js
--rw-r--r--   0 chrismutel   (501) staff       (20)      755 2023-08-02 20:57:45.000000 bw_matchbox-0.3.0/bw_matchbox/assets/js/ProcessesList/ProcessesListNodes.js
--rw-r--r--   0 chrismutel   (501) staff       (20)     3918 2023-08-02 20:57:45.000000 bw_matchbox-0.3.0/bw_matchbox/assets/js/ProcessesList/ProcessesListPagination.UNUSED.js
--rw-r--r--   0 chrismutel   (501) staff       (20)     1982 2023-08-02 20:57:45.000000 bw_matchbox-0.3.0/bw_matchbox/assets/js/ProcessesList/ProcessesListSearch.js
--rw-r--r--   0 chrismutel   (501) staff       (20)     3143 2023-08-02 20:57:45.000000 bw_matchbox-0.3.0/bw_matchbox/assets/js/ProcessesList/ProcessesListStates.js
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-02 21:10:16.448195 bw_matchbox-0.3.0/bw_matchbox/assets/templates/
--rw-r--r--   0 chrismutel   (501) staff       (20)     4144 2023-08-02 20:57:45.000000 bw_matchbox-0.3.0/bw_matchbox/assets/templates/compare.html
--rw-r--r--   0 chrismutel   (501) staff       (20)     2566 2023-07-23 12:42:57.000000 bw_matchbox-0.3.0/bw_matchbox/assets/templates/databases.html
--rw-r--r--   0 chrismutel   (501) staff       (20)      461 2023-07-23 15:09:13.000000 bw_matchbox-0.3.0/bw_matchbox/assets/templates/expand.html
--rw-r--r--   0 chrismutel   (501) staff       (20)    11784 2023-06-20 12:27:44.000000 bw_matchbox-0.3.0/bw_matchbox/assets/templates/file.html
--rw-r--r--   0 chrismutel   (501) staff       (20)       16 2023-06-20 12:27:44.000000 bw_matchbox-0.3.0/bw_matchbox/assets/templates/footer.html
--rw-r--r--   0 chrismutel   (501) staff       (20)     2341 2023-08-02 20:57:45.000000 bw_matchbox-0.3.0/bw_matchbox/assets/templates/header.html
--rw-r--r--   0 chrismutel   (501) staff       (20)     4135 2023-08-02 20:57:45.000000 bw_matchbox-0.3.0/bw_matchbox/assets/templates/index.html
--rw-r--r--   0 chrismutel   (501) staff       (20)      733 2023-06-21 04:56:26.000000 bw_matchbox-0.3.0/bw_matchbox/assets/templates/match-status.html
--rw-r--r--   0 chrismutel   (501) staff       (20)     1711 2023-06-21 09:42:53.000000 bw_matchbox-0.3.0/bw_matchbox/assets/templates/match.html
--rw-r--r--   0 chrismutel   (501) staff       (20)      798 2023-07-23 12:44:06.000000 bw_matchbox-0.3.0/bw_matchbox/assets/templates/navigation.html
--rw-r--r--   0 chrismutel   (501) staff       (20)     3536 2023-08-01 11:49:18.000000 bw_matchbox-0.3.0/bw_matchbox/assets/templates/process_detail.html
--rw-r--r--   0 chrismutel   (501) staff       (20)      599 2023-07-22 21:06:00.000000 bw_matchbox-0.3.0/bw_matchbox/assets/templates/project.html
--rw-r--r--   0 chrismutel   (501) staff       (20)      412 2023-08-01 07:10:26.000000 bw_matchbox-0.3.0/bw_matchbox/assets/templates/search-embedded.html
--rw-r--r--   0 chrismutel   (501) staff       (20)      850 2023-06-20 12:27:44.000000 bw_matchbox-0.3.0/bw_matchbox/assets/templates/search.html
--rw-r--r--   0 chrismutel   (501) staff       (20)      947 2023-06-20 12:27:44.000000 bw_matchbox-0.3.0/bw_matchbox/assets/templates/search_result.html
--rw-r--r--   0 chrismutel   (501) staff       (20)     1243 2023-07-23 08:33:52.000000 bw_matchbox-0.3.0/bw_matchbox/assets/templates/select_files.html
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-02 21:10:16.448639 bw_matchbox-0.3.0/bw_matchbox/bin/
--rw-r--r--   0 chrismutel   (501) staff       (20)        0 2023-06-20 12:27:44.000000 bw_matchbox-0.3.0/bw_matchbox/bin/__init__.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     2931 2023-08-01 17:17:21.000000 bw_matchbox-0.3.0/bw_matchbox/bin/matchbox.py
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-02 21:10:16.451048 bw_matchbox-0.3.0/bw_matchbox/data/
--rw-r--r--   0 chrismutel   (501) staff       (20)   123246 2023-08-01 17:17:21.000000 bw_matchbox-0.3.0/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-mining.json
--rw-r--r--   0 chrismutel   (501) staff       (20)    93862 2023-07-23 09:30:53.000000 bw_matchbox-0.3.0/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-string-matching.json
--rw-r--r--   0 chrismutel   (501) staff       (20)   116072 2023-08-01 17:17:21.000000 bw_matchbox-0.3.0/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-transport.json
--rw-r--r--   0 chrismutel   (501) staff       (20)      603 2023-07-23 09:34:59.000000 bw_matchbox-0.3.0/bw_matchbox/data/dare.json
--rw-r--r--   0 chrismutel   (501) staff       (20)     1388 2023-08-01 17:17:21.000000 bw_matchbox-0.3.0/bw_matchbox/utils.py
--rw-r--r--   0 chrismutel   (501) staff       (20)    20517 2023-08-01 17:17:21.000000 bw_matchbox-0.3.0/bw_matchbox/webapp.py
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-02 21:10:16.455962 bw_matchbox-0.3.0/bw_matchbox.egg-info/
--rw-r--r--   0 chrismutel   (501) staff       (20)     6349 2023-08-02 21:10:16.000000 bw_matchbox-0.3.0/bw_matchbox.egg-info/PKG-INFO
--rw-r--r--   0 chrismutel   (501) staff       (20)     4480 2023-08-02 21:10:16.000000 bw_matchbox-0.3.0/bw_matchbox.egg-info/SOURCES.txt
--rw-r--r--   0 chrismutel   (501) staff       (20)        1 2023-08-02 21:10:16.000000 bw_matchbox-0.3.0/bw_matchbox.egg-info/dependency_links.txt
--rw-r--r--   0 chrismutel   (501) staff       (20)       59 2023-08-02 21:10:16.000000 bw_matchbox-0.3.0/bw_matchbox.egg-info/entry_points.txt
--rw-r--r--   0 chrismutel   (501) staff       (20)        1 2023-07-23 07:30:31.000000 bw_matchbox-0.3.0/bw_matchbox.egg-info/not-zip-safe
--rw-r--r--   0 chrismutel   (501) staff       (20)      167 2023-08-02 21:10:16.000000 bw_matchbox-0.3.0/bw_matchbox.egg-info/requires.txt
--rw-r--r--   0 chrismutel   (501) staff       (20)       12 2023-08-02 21:10:16.000000 bw_matchbox-0.3.0/bw_matchbox.egg-info/top_level.txt
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-02 21:10:16.453494 bw_matchbox-0.3.0/docs/
--rw-r--r--   0 chrismutel   (501) staff       (20)     1145 2023-07-23 07:23:19.000000 bw_matchbox-0.3.0/docs/conf.py
--rw-r--r--   0 chrismutel   (501) staff       (20)       87 2023-06-20 12:26:53.000000 bw_matchbox-0.3.0/pyproject.toml
--rw-r--r--   0 chrismutel   (501) staff       (20)     1935 2023-08-02 21:10:16.458064 bw_matchbox-0.3.0/setup.cfg
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-03 20:46:27.899150 bw_matchbox-0.4.0/
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1067 2023-06-20 12:26:53.000000 bw_matchbox-0.4.0/LICENSE
+-rw-r--r--   0 chrismutel   (501) staff       (20)      226 2023-08-02 21:05:25.000000 bw_matchbox-0.4.0/MANIFEST.in
+-rw-r--r--   0 chrismutel   (501) staff       (20)     6349 2023-08-03 20:46:27.899222 bw_matchbox-0.4.0/PKG-INFO
+-rw-r--r--   0 chrismutel   (501) staff       (20)     5325 2023-08-01 07:10:26.000000 bw_matchbox-0.4.0/README.md
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-03 20:46:27.887092 bw_matchbox-0.4.0/bw_matchbox/
+-rw-r--r--   0 chrismutel   (501) staff       (20)        6 2023-08-03 20:45:33.000000 bw_matchbox-0.4.0/bw_matchbox/VERSION
+-rw-r--r--   0 chrismutel   (501) staff       (20)      215 2023-08-01 17:17:21.000000 bw_matchbox-0.4.0/bw_matchbox/__init__.py
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-03 20:46:27.885300 bw_matchbox-0.4.0/bw_matchbox/assets/
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-03 20:46:27.889036 bw_matchbox-0.4.0/bw_matchbox/assets/css/
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1891 2023-08-03 20:45:26.000000 bw_matchbox-0.4.0/bw_matchbox/assets/css/common.css
+-rw-r--r--   0 chrismutel   (501) staff       (20)     6452 2023-08-03 20:45:26.000000 bw_matchbox-0.4.0/bw_matchbox/assets/css/compare.css
+-rw-r--r--   0 chrismutel   (501) staff       (20)      640 2023-08-03 20:45:26.000000 bw_matchbox-0.4.0/bw_matchbox/assets/css/customizations.css
+-rw-r--r--   0 chrismutel   (501) staff       (20)     2251 2023-08-03 20:45:26.000000 bw_matchbox-0.4.0/bw_matchbox/assets/css/modal.css
+-rw-r--r--   0 chrismutel   (501) staff       (20)     7618 2023-08-01 07:10:26.000000 bw_matchbox-0.4.0/bw_matchbox/assets/css/normalize.css
+-rw-r--r--   0 chrismutel   (501) staff       (20)     3243 2023-08-03 20:45:26.000000 bw_matchbox-0.4.0/bw_matchbox/assets/css/processes-list.css
+-rw-r--r--   0 chrismutel   (501) staff       (20)    11556 2023-08-01 07:10:26.000000 bw_matchbox-0.4.0/bw_matchbox/assets/css/skeleton.css
+-rw-r--r--   0 chrismutel   (501) staff       (20)      916 2023-08-01 07:10:26.000000 bw_matchbox-0.4.0/bw_matchbox/assets/css/tooltip.css
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-03 20:46:27.889316 bw_matchbox-0.4.0/bw_matchbox/assets/images/
+-rw-r--r--   0 chrismutel   (501) staff       (20)    32038 2023-06-20 12:27:44.000000 bw_matchbox-0.4.0/bw_matchbox/assets/images/favicon.ico
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-03 20:46:27.885139 bw_matchbox-0.4.0/bw_matchbox/assets/js/
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-03 20:46:27.890162 bw_matchbox-0.4.0/bw_matchbox/assets/js/Compare/
+-rw-r--r--   0 chrismutel   (501) staff       (20)    22750 2023-08-03 20:45:26.000000 bw_matchbox-0.4.0/bw_matchbox/assets/js/Compare/CompareCore.js
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1251 2023-08-03 20:45:26.000000 bw_matchbox-0.4.0/bw_matchbox/assets/js/Compare/CompareRowClick.js
+-rw-r--r--   0 chrismutel   (501) staff       (20)    11340 2023-08-03 20:45:26.000000 bw_matchbox-0.4.0/bw_matchbox/assets/js/Compare/CompareRowsHelpers.js
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-03 20:46:27.891438 bw_matchbox-0.4.0/bw_matchbox/assets/js/ProcessesList/
+-rw-r--r--   0 chrismutel   (501) staff       (20)     3578 2023-08-03 20:45:26.000000 bw_matchbox-0.4.0/bw_matchbox/assets/js/ProcessesList/ProcessesList.js
+-rw-r--r--   0 chrismutel   (501) staff       (20)      497 2023-08-03 20:45:26.000000 bw_matchbox-0.4.0/bw_matchbox/assets/js/ProcessesList/ProcessesListConstants.js
+-rw-r--r--   0 chrismutel   (501) staff       (20)      993 2023-08-03 20:45:26.000000 bw_matchbox-0.4.0/bw_matchbox/assets/js/ProcessesList/ProcessesListData.js
+-rw-r--r--   0 chrismutel   (501) staff       (20)     4710 2023-08-03 20:45:26.000000 bw_matchbox-0.4.0/bw_matchbox/assets/js/ProcessesList/ProcessesListDataLoad.js
+-rw-r--r--   0 chrismutel   (501) staff       (20)     4675 2023-08-03 20:45:26.000000 bw_matchbox-0.4.0/bw_matchbox/assets/js/ProcessesList/ProcessesListDataRender.js
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1128 2023-08-03 20:45:26.000000 bw_matchbox-0.4.0/bw_matchbox/assets/js/ProcessesList/ProcessesListNodes.js
+-rw-r--r--   0 chrismutel   (501) staff       (20)     4909 2023-08-03 20:45:26.000000 bw_matchbox-0.4.0/bw_matchbox/assets/js/ProcessesList/ProcessesListPagination.UNUSED.js
+-rw-r--r--   0 chrismutel   (501) staff       (20)     2523 2023-08-03 20:45:26.000000 bw_matchbox-0.4.0/bw_matchbox/assets/js/ProcessesList/ProcessesListSearch.js
+-rw-r--r--   0 chrismutel   (501) staff       (20)     3775 2023-08-03 20:45:26.000000 bw_matchbox-0.4.0/bw_matchbox/assets/js/ProcessesList/ProcessesListStates.js
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-03 20:46:27.891584 bw_matchbox-0.4.0/bw_matchbox/assets/js/common/
+-rw-r--r--   0 chrismutel   (501) staff       (20)     4947 2023-08-03 20:45:26.000000 bw_matchbox-0.4.0/bw_matchbox/assets/js/common/CommonHelpers.js
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-03 20:46:27.885185 bw_matchbox-0.4.0/bw_matchbox/assets/js/libs/
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-03 20:46:27.891870 bw_matchbox-0.4.0/bw_matchbox/assets/js/libs/ym/
+-rw-r--r--   0 chrismutel   (501) staff       (20)    13286 2023-08-03 20:45:26.000000 bw_matchbox-0.4.0/bw_matchbox/assets/js/libs/ym/ym-modules-0.1.2.js
+-rw-r--r--   0 chrismutel   (501) staff       (20)     6018 2023-08-03 20:45:26.000000 bw_matchbox-0.4.0/bw_matchbox/assets/js/libs/ym/ym-modules-0.1.2.min.js
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-03 20:46:27.894594 bw_matchbox-0.4.0/bw_matchbox/assets/templates/
+-rw-r--r--   0 chrismutel   (501) staff       (20)     3901 2023-08-03 20:45:26.000000 bw_matchbox-0.4.0/bw_matchbox/assets/templates/compare.html
+-rw-r--r--   0 chrismutel   (501) staff       (20)     2566 2023-07-23 12:42:57.000000 bw_matchbox-0.4.0/bw_matchbox/assets/templates/databases.html
+-rw-r--r--   0 chrismutel   (501) staff       (20)      461 2023-07-23 15:09:13.000000 bw_matchbox-0.4.0/bw_matchbox/assets/templates/expand.html
+-rw-r--r--   0 chrismutel   (501) staff       (20)       16 2023-06-20 12:27:44.000000 bw_matchbox-0.4.0/bw_matchbox/assets/templates/footer.html
+-rw-r--r--   0 chrismutel   (501) staff       (20)     2660 2023-08-03 20:45:26.000000 bw_matchbox-0.4.0/bw_matchbox/assets/templates/header.html
+-rw-r--r--   0 chrismutel   (501) staff       (20)     4347 2023-08-03 20:45:26.000000 bw_matchbox-0.4.0/bw_matchbox/assets/templates/index.html
+-rw-r--r--   0 chrismutel   (501) staff       (20)      733 2023-06-21 04:56:26.000000 bw_matchbox-0.4.0/bw_matchbox/assets/templates/match-status.html
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1721 2023-08-03 20:45:26.000000 bw_matchbox-0.4.0/bw_matchbox/assets/templates/match.html
+-rw-r--r--   0 chrismutel   (501) staff       (20)      798 2023-07-23 12:44:06.000000 bw_matchbox-0.4.0/bw_matchbox/assets/templates/navigation.html
+-rw-r--r--   0 chrismutel   (501) staff       (20)     3536 2023-08-01 11:49:18.000000 bw_matchbox-0.4.0/bw_matchbox/assets/templates/process_detail.html
+-rw-r--r--   0 chrismutel   (501) staff       (20)      599 2023-07-22 21:06:00.000000 bw_matchbox-0.4.0/bw_matchbox/assets/templates/project.html
+-rw-r--r--   0 chrismutel   (501) staff       (20)      412 2023-08-01 07:10:26.000000 bw_matchbox-0.4.0/bw_matchbox/assets/templates/search-embedded.html
+-rw-r--r--   0 chrismutel   (501) staff       (20)      850 2023-06-20 12:27:44.000000 bw_matchbox-0.4.0/bw_matchbox/assets/templates/search.html
+-rw-r--r--   0 chrismutel   (501) staff       (20)      947 2023-06-20 12:27:44.000000 bw_matchbox-0.4.0/bw_matchbox/assets/templates/search_result.html
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1243 2023-07-23 08:33:52.000000 bw_matchbox-0.4.0/bw_matchbox/assets/templates/select_files.html
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-03 20:46:27.894886 bw_matchbox-0.4.0/bw_matchbox/bin/
+-rw-r--r--   0 chrismutel   (501) staff       (20)        0 2023-06-20 12:27:44.000000 bw_matchbox-0.4.0/bw_matchbox/bin/__init__.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     2931 2023-08-01 17:17:21.000000 bw_matchbox-0.4.0/bw_matchbox/bin/matchbox.py
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-03 20:46:27.896879 bw_matchbox-0.4.0/bw_matchbox/data/
+-rw-r--r--   0 chrismutel   (501) staff       (20)   123246 2023-08-01 17:17:21.000000 bw_matchbox-0.4.0/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-mining.json
+-rw-r--r--   0 chrismutel   (501) staff       (20)    93862 2023-07-23 09:30:53.000000 bw_matchbox-0.4.0/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-string-matching.json
+-rw-r--r--   0 chrismutel   (501) staff       (20)   116072 2023-08-01 17:17:21.000000 bw_matchbox-0.4.0/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-transport.json
+-rw-r--r--   0 chrismutel   (501) staff       (20)      603 2023-07-23 09:34:59.000000 bw_matchbox-0.4.0/bw_matchbox/data/dare.json
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1388 2023-08-01 17:17:21.000000 bw_matchbox-0.4.0/bw_matchbox/utils.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)    20517 2023-08-01 17:17:21.000000 bw_matchbox-0.4.0/bw_matchbox/webapp.py
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-03 20:46:27.898041 bw_matchbox-0.4.0/bw_matchbox.egg-info/
+-rw-r--r--   0 chrismutel   (501) staff       (20)     6349 2023-08-03 20:46:27.000000 bw_matchbox-0.4.0/bw_matchbox.egg-info/PKG-INFO
+-rw-r--r--   0 chrismutel   (501) staff       (20)     4694 2023-08-03 20:46:27.000000 bw_matchbox-0.4.0/bw_matchbox.egg-info/SOURCES.txt
+-rw-r--r--   0 chrismutel   (501) staff       (20)        1 2023-08-03 20:46:27.000000 bw_matchbox-0.4.0/bw_matchbox.egg-info/dependency_links.txt
+-rw-r--r--   0 chrismutel   (501) staff       (20)       59 2023-08-03 20:46:27.000000 bw_matchbox-0.4.0/bw_matchbox.egg-info/entry_points.txt
+-rw-r--r--   0 chrismutel   (501) staff       (20)        1 2023-07-23 07:30:31.000000 bw_matchbox-0.4.0/bw_matchbox.egg-info/not-zip-safe
+-rw-r--r--   0 chrismutel   (501) staff       (20)      167 2023-08-03 20:46:27.000000 bw_matchbox-0.4.0/bw_matchbox.egg-info/requires.txt
+-rw-r--r--   0 chrismutel   (501) staff       (20)       12 2023-08-03 20:46:27.000000 bw_matchbox-0.4.0/bw_matchbox.egg-info/top_level.txt
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-08-03 20:46:27.897109 bw_matchbox-0.4.0/docs/
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1145 2023-07-23 07:23:19.000000 bw_matchbox-0.4.0/docs/conf.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)       87 2023-06-20 12:26:53.000000 bw_matchbox-0.4.0/pyproject.toml
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1900 2023-08-03 20:46:27.899662 bw_matchbox-0.4.0/setup.cfg
```

### Comparing `bw_matchbox-0.3.0/LICENSE` & `bw_matchbox-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.3.0/PKG-INFO` & `bw_matchbox-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bw_matchbox
-Version: 0.3.0
+Version: 0.4.0
 Summary: Browser to match Brightway databases
 Home-page: https://github.com/cauldron/bw_matchbox
 Author: Chris Mutel
 Author-email: <cmutel@gmail.com>
 Maintainer: Chris Mutel
 Maintainer-email: <cmutel@gmail.com>
 License: MIT
```

### Comparing `bw_matchbox-0.3.0/README.md` & `bw_matchbox-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.3.0/bw_matchbox/assets/css/common.css` & `bw_matchbox-0.4.0/bw_matchbox/assets/css/common.css`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,7 @@
-/* stylelint-disable
-    declaration-block-single-line-max-declarations
-    declaration-colon-space-after
-    rule-empty-line-before
-    comment-empty-line-before
-    at-rule-empty-line-before
-    declaration-block-no-redundant-longhand-properties
- */
-
 :root {
   /* Primary color */
   --layout-theme-primary-color: #33c3f0; /* aka rgb(51,195,240) */
   /* Primary colors for hovered elements */
   --layout-theme-primary-color-dark1: #1eaedb; /* aks rgb(30,174,219) */
   --layout-theme-primary-color-dark2: #0fa0ce; /* aks gb(15,160,206) */
   /* Error color */
```

### Comparing `bw_matchbox-0.3.0/bw_matchbox/assets/css/compare.css` & `bw_matchbox-0.4.0/bw_matchbox/assets/css/compare.css`

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,7 @@
-/* stylelint-disable
-    declaration-block-single-line-max-declarations
-    declaration-colon-space-after
- */
-
 :root {
   /* // UNUSED: Collapsed rows are just hidden.
    * --compare-collapsed-color: #F60;
    * --compare-collapsed-bg-color: rgba(255,102,0,.1);
    */
   --compare-selected-color: var(--layout-theme-primary-color-dark1); /* #1EAEDB; */
   --compare-selected-bg-color05: rgb(30 174 219 / 5%);
@@ -55,18 +50,15 @@
 }
 
 /* Table cells basic styles... */
 .compare-table thead th,
 .compare-table tbody td {
   padding: var(--compare-td-padding-v) var(--compare-td-padding-h);
   line-height: 1.3;
-  width: 50px;
-  white-space: nowrap;
   overflow: hidden;
-  text-overflow: ellipsis;
 }
 
 .compare-table thead th > div,
 .compare-table tbody td > div {
   overflow: hidden;
   text-overflow: ellipsis;
   width: 100%;
@@ -80,29 +72,27 @@
 .compare-table tbody td a:hover {
   text-decoration: underline;
 }
 
 /* Particular columns width */
 .compare-table .cell-actions {
   width: 3.5em;
+  white-space: nowrap;
 }
-
 .compare-table .cell-amount {
-  width: 4.5em;
+  width: 5.5em;
+  white-space: nowrap;
 }
-
 .compare-table .cell-name {
   width: 50%;
   white-space: wrap;
 }
-
 .compare-table .cell-location {
   width: 30%;
 }
-
 .compare-table .cell-unit {
   width: 2em;
 }
 
 /* Name cell */
 .compare-table .cell-name {
   white-space: wrap;
@@ -203,7 +193,71 @@
   line-height: 1;
   transition: all var(--compare-animation-time) ease;
 }
 
 .compare-table tr.collapsed-handler td:hover {
   background-color: var(--compare-selected-bg-color2);
 }
+
+/* Modal customizations */
+.modal#modal-number-editor .modal-content {
+  display: flex;
+  overflow: hidden;
+  align-items: stretch;
+  align-content: stretch;
+}
+.modal#modal-number-editor #modal-content-wrapper {
+  display: flex;
+  overflow: hidden;
+  text-overflow: ellipsis;
+  height: 100%;
+  /* padding: 20px 0; */
+}
+
+.modal#modal-number-editor #modal-content-wrapper > div {
+  overflow: auto;
+  /* padding: 0 20px; */
+  padding: 20px;
+  flex: 1;
+  width: 50%;
+}
+.modal#modal-number-editor #modal-content-wrapper > div:first-child {
+}
+
+/* Modal table */
+.modal#modal-number-editor .modal-table {
+  border: 0;
+  table-layout: fixed;
+  width: 100%;
+  border-style: solid;
+}
+.modal#modal-number-editor .modal-table tbody tr {
+  transition: all var(--compare-animation-time) ease;
+}
+.modal#modal-number-editor .modal-table tbody tr:focus,
+.modal#modal-number-editor .modal-table tbody tr:hover {
+  background-color: var(--compare-selected-bg-color1);
+  cursor: pointer;
+}
+.modal#modal-number-editor .modal-table th,
+.modal#modal-number-editor .modal-table td {
+  padding: var(--compare-td-padding-v) var(--compare-td-padding-h);
+  line-height: 1.3;
+  overflow: hidden;
+}
+.modal#modal-number-editor .modal-table tbody td > div {
+  overflow: hidden;
+  text-overflow: ellipsis;
+  width: 100%;
+  position: relative;
+}
+/* Adjust widths */
+.modal#modal-number-editor .modal-table th:last-child {
+  width: 50px;
+}
+.modal#modal-number-editor .modal-table th:first-child {
+  width: 80px;
+}
+/* Adjust content styles */
+.modal#modal-number-editor .strong {
+  margin: 5px 0;
+}
```

### Comparing `bw_matchbox-0.3.0/bw_matchbox/assets/css/normalize.css` & `bw_matchbox-0.4.0/bw_matchbox/assets/css/normalize.css`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.3.0/bw_matchbox/assets/css/processes-list.css` & `bw_matchbox-0.4.0/bw_matchbox/assets/css/processes-list.css`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 /* stylelint-disable
-    declaration-block-single-line-max-declarations
-    declaration-colon-space-after
-    rule-empty-line-before
-    comment-empty-line-before
+    declaration-block-single-line-max-declarations,
+    declaration-colon-space-after,
 */
 
 /* Root node */
 .processes-list {
   margin-bottom: 20px;
 }
 
@@ -110,23 +108,21 @@
 }
 .processes-list .bottom-actions-links a {
   display: none;
   color: var(-layout-theme-primary-color-dark1);
   cursor: pointer;
   margin: 0 10px;
 }
-.processes-list .bottom-actions-links a + a:before {
-  content: ' | ',
+.processes-list .bottom-actions-links a + a::before {
   display: inline-block;
 }
 .processes-list .bottom-actions-links a:hover {
   text-decoration: underline;
 }
 /* Show 'Reload' (after error) button if error... */
 .processes-list.error .bottom-actions-links a#action-clear-and-reload,
 /* Show 'Load more' button for all 'order by' values except for 'random'... */
-.processes-list:not(.order-random):not(.error) .bottom-actions-links a#action-load-more,
+.processes-list:not(.order-random, .error) .bottom-actions-links a#action-load-more,
 /* Show 'Refresh' button for 'random' 'order by' value... */
 .processes-list.order-random:not(.error) .bottom-actions-links a#action-reload-random {
   display: inline-block;
 }
-
```

### Comparing `bw_matchbox-0.3.0/bw_matchbox/assets/css/skeleton.css` & `bw_matchbox-0.4.0/bw_matchbox/assets/css/skeleton.css`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.3.0/bw_matchbox/assets/css/tooltip.css` & `bw_matchbox-0.4.0/bw_matchbox/assets/css/tooltip.css`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.3.0/bw_matchbox/assets/images/favicon.ico` & `bw_matchbox-0.4.0/bw_matchbox/assets/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.3.0/bw_matchbox/assets/js/CommonHelpers.js` & `bw_matchbox-0.4.0/bw_matchbox/assets/js/common/CommonHelpers.js`

 * *Files 7% similar despite different names*

#### js-beautify {}

```diff
@@ -1,146 +1,159 @@
-// global module variable
-// eslint-disable-next-line no-unused-vars
-const CommonHelpers = {
-    numberSorter: function(a, b) {
-        if (a.amount < b.amount) {
-            // Reversed because want ascending order
-            return -1;
-        }
-        if (a.amount > b.amount) {
-            return 1;
-        }
-        return 0;
-    },
+modules.define(
+    'CommonHelpers',
+    [
+        // Required modules...
+    ],
+    function provide_CommonHelpers(
+        provide,
+        // Resolved modules...
+    ) {
+        // Define module...
 
-    /** quoteHtmlAttr -- quote all invalid characters for html
-     * @param {string} str
-     * @param [{boolean}] preserveCR
-     */
-    quoteHtmlAttr: function(str, preserveCR) {
-        preserveCR = preserveCR ? '&#13;' : '\n';
-        return (
-            String(str) // Forces the conversion to string
-            .replace(/&/g, '&amp;') // This MUST be the 1st replacement
-            .replace(/'/g, '&apos;') // The 4 other predefined entities, required
-            .replace(/"/g, '&quot;')
-            .replace(/</g, '&lt;')
-            .replace(/>/g, '&gt;')
-            // You may add other replacements here for HTML only (but it's not
-            // necessary). Or for XML, only if the named entities are defined in its
-            // DTD.
-            .replace(/\r\n/g, preserveCR) // Must be before the next replacement
-            .replace(/[\r\n]/g, preserveCR)
-        );
-    },
+        const CommonHelpers = {
+            sortByAmountProperty(a, b) {
+                if (a.amount < b.amount) {
+                    // Reversed because want ascending order
+                    return -1;
+                }
+                if (a.amount > b.amount) {
+                    return 1;
+                }
+                return 0;
+            },
 
-    /** htmlToElement -- Create dom node instance from html string
-     * @param {string} HTML representing a single element
-     * @return {HTMLElement}
-     */
-    htmlToElement: function(html) {
-        const template = document.createElement('template');
-        if (Array.isArray(html)) {
-            html = html.join('');
-        }
-        html = html.trim(); // Never return a text node of whitespace as the result
-        template.innerHTML = html;
-        const content = template.content;
-        return content.firstChild;
-    },
+            /** quoteHtmlAttr -- quote all invalid characters for html
+             * @param {string} str
+             * @param [{boolean}] preserveCR
+             */
+            quoteHtmlAttr(str, preserveCR) {
+                preserveCR = preserveCR ? '&#13;' : '\n';
+                return (
+                    String(str) // Forces the conversion to string
+                    .replace(/&/g, '&amp;') // This MUST be the 1st replacement
+                    .replace(/'/g, '&apos;') // The 4 other predefined entities, required
+                    .replace(/"/g, '&quot;')
+                    .replace(/</g, '&lt;')
+                    .replace(/>/g, '&gt;')
+                    // You may add other replacements here for HTML only (but it's not
+                    // necessary). Or for XML, only if the named entities are defined in its
+                    // DTD.
+                    .replace(/\r\n/g, preserveCR) // Must be before the next replacement
+                    .replace(/[\r\n]/g, preserveCR)
+                );
+            },
 
-    htmlToElements: function(html) {
-        const template = document.createElement('template');
-        if (Array.isArray(html)) {
-            html = html.join('');
-        }
-        html = html.trim(); // Never return a text node of whitespace as the result
-        template.innerHTML = html;
-        const content = template.content;
-        return content.children;
-    },
-    /** decodeQuery
-     * @param {string | string[]} qs
-     * @param {string} sep
-     * @param {string} eq
-     * @param {any} options
-     * @returns {{}}
-     */
-    decodeQuery(qs, sep, eq, options) {
-        sep = sep || '&';
-        eq = eq || '=';
-        const obj = {};
-        if (typeof qs !== 'string' || qs.length === 0) {
-            return obj;
-        }
-        const regexp = /\+/g;
-        qs = qs.split(sep);
-        let maxKeys = 1000;
-        if (options && typeof options.maxKeys === 'number') {
-            maxKeys = options.maxKeys;
-        }
-        let len = qs.length;
-        // maxKeys <= 0 means that we should not limit keys count
-        if (maxKeys > 0 && len > maxKeys) {
-            len = maxKeys;
-        }
-        for (let i = 0; i < len; ++i) {
-            const x = qs[i].replace(regexp, '%20'),
-                idx = x.indexOf(eq);
-            let kstr, vstr;
-            if (idx >= 0) {
-                kstr = x.substring(0, idx);
-                vstr = x.substring(idx + 1);
-            } else {
-                kstr = x;
-                vstr = '';
-            }
-            const k = decodeURIComponent(kstr);
-            const v = decodeURIComponent(vstr);
-            // if (!hasOwnProperty(obj, k)) {
-            if (!Object.prototype.hasOwnProperty.call(obj, k)) {
-                obj[k] = v;
-            } else if (Array.isArray(obj[k])) {
-                obj[k].push(v);
-            } else {
-                obj[k] = [obj[k], v];
-            }
-        }
-        return obj;
-    },
+            /** htmlToElement -- Create dom node instance from html string
+             * @param {string} HTML representing a single element
+             * @return {HTMLElement}
+             */
+            htmlToElement(html) {
+                const template = document.createElement('template');
+                if (Array.isArray(html)) {
+                    html = html.join('');
+                }
+                html = html.trim(); // Never return a text node of whitespace as the result
+                template.innerHTML = html;
+                const content = template.content;
+                return content.firstChild;
+            },
 
-    /** parseQuery -- Parse url query string (in form `?xx=yy&...` or `xx=yy&...`)
-     * @param {string} search  - Query string
-     * @return {Record<string, string>} query - Query object
-     */
-    parseQuery(search) {
-        if (!search) {
-            return {};
-        }
-        if (search.indexOf('?') === 0) {
-            search = search.substring(1);
-        }
-        return CommonHelpers.decodeQuery(search);
-    },
+            htmlToElements(html) {
+                const template = document.createElement('template');
+                if (Array.isArray(html)) {
+                    html = html.join('');
+                }
+                html = html.trim(); // Never return a text node of whitespace as the result
+                template.innerHTML = html;
+                const content = template.content;
+                return content.children;
+            },
+            /** decodeQuery
+             * @param {string | string[]} qs
+             * @param {string} sep
+             * @param {string} eq
+             * @param {any} options
+             * @returns {{}}
+             */
+            decodeQuery(qs, sep, eq, options) {
+                sep = sep || '&';
+                eq = eq || '=';
+                const obj = {};
+                if (typeof qs !== 'string' || qs.length === 0) {
+                    return obj;
+                }
+                const regexp = /\+/g;
+                qs = qs.split(sep);
+                let maxKeys = 1000;
+                if (options && typeof options.maxKeys === 'number') {
+                    maxKeys = options.maxKeys;
+                }
+                let len = qs.length;
+                // maxKeys <= 0 means that we should not limit keys count
+                if (maxKeys > 0 && len > maxKeys) {
+                    len = maxKeys;
+                }
+                for (let i = 0; i < len; ++i) {
+                    const x = qs[i].replace(regexp, '%20'),
+                        idx = x.indexOf(eq);
+                    let kstr, vstr;
+                    if (idx >= 0) {
+                        kstr = x.substring(0, idx);
+                        vstr = x.substring(idx + 1);
+                    } else {
+                        kstr = x;
+                        vstr = '';
+                    }
+                    const k = decodeURIComponent(kstr);
+                    const v = decodeURIComponent(vstr);
+                    // if (!hasOwnProperty(obj, k)) {
+                    if (!Object.prototype.hasOwnProperty.call(obj, k)) {
+                        obj[k] = v;
+                    } else if (Array.isArray(obj[k])) {
+                        obj[k].push(v);
+                    } else {
+                        obj[k] = [obj[k], v];
+                    }
+                }
+                return obj;
+            },
+
+            /** parseQuery -- Parse url query string (in form `?xx=yy&...` or `xx=yy&...`)
+             * @param {string} search  - Query string
+             * @return {Record<string, string>} query - Query object
+             */
+            parseQuery(search) {
+                if (!search) {
+                    return {};
+                }
+                if (search.indexOf('?') === 0) {
+                    search = search.substring(1);
+                }
+                return CommonHelpers.decodeQuery(search);
+            },
+
+            /** makeQuery
+             * @param {Record<string, string | number | boolean>} params
+             * @param {{ addQuestionSymbol?: boolean; useEmptyValues?: boolean }} opts
+             * @returns {string}
+             */
+            makeQuery(params, opts = {}) {
+                let url = Object.entries(params)
+                    .map(([id, val]) => {
+                        const valStr = String(val);
+                        if ((val == undefined || valStr === '') && !opts.useEmptyValues) {
+                            return undefined;
+                        }
+                        return encodeURI(id) + '=' + encodeURI(String(val));
+                    })
+                    .filter(Boolean)
+                    .join('&');
+                if (opts.addQuestionSymbol && url) {
+                    url = '?' + url;
+                }
+                return url;
+            },
+        };
 
-    /** makeQuery
-     * @param {Record<string, string | number | boolean>} params
-     * @param {{ addQuestionSymbol?: boolean; useEmptyValues?: boolean }} opts
-     * @returns {string}
-     */
-    makeQuery(params, opts = {}) {
-        let url = Object.entries(params)
-            .map(([id, val]) => {
-                const valStr = String(val);
-                if ((val == undefined || valStr === '') && !opts.useEmptyValues) {
-                    return undefined;
-                }
-                return encodeURI(id) + '=' + encodeURI(String(val));
-            })
-            .filter(Boolean)
-            .join('&');
-        if (opts.addQuestionSymbol && url) {
-            url = '?' + url;
-        }
-        return url;
+        provide(CommonHelpers);
     },
-};
+);
```

### Comparing `bw_matchbox-0.3.0/bw_matchbox/assets/js/Compare/CompareRowClick.js` & `bw_matchbox-0.4.0/bw_matchbox/assets/js/Compare/CompareRowClick.js`

 * *Files 10% similar despite different names*

#### js-beautify {}

```diff
@@ -1,33 +1,47 @@
-// global module variable
-const CompareRowClick = {
-    // Public data...
-    disabled: false, // public
-
-    // Private data...
-    timeout: 100,
-    releaseHandler: undefined,
-
-    /** clearRowClickHandler - Clear row click disbale timer handler.
-     */
-    clearRowClickHandler: function() {
-        if (CompareRowClick.releaseHandler) {
-            clearTimeout(CompareRowClick.releaseHandler);
-            CompareRowClick.releaseHandler = undefined;
-        }
-    },
+modules.define(
+    'CompareRowClick',
+    [
+        // Required modules...
+    ],
+    function provide_CompareRowClick(
+        provide,
+        // Resolved modules...
+    ) {
+        // Define module...
 
-    /** releaseRowClick - Enable processing of `clickRow`
-     */
-    releaseRowClick: function() {
-        CompareRowClick.disabled = false;
-        CompareRowClick.clearRowClickHandler();
-    },
+        const CompareRowClick = {
+            // Public data...
+            disabled: false, // public
+
+            // Private data...
+            timeout: 100,
+            releaseHandler: undefined,
+
+            /** clearRowClickHandler - Clear row click disbale timer handler.
+             */
+            clearRowClickHandler: function() {
+                if (CompareRowClick.releaseHandler) {
+                    clearTimeout(CompareRowClick.releaseHandler);
+                    CompareRowClick.releaseHandler = undefined;
+                }
+            },
+
+            /** releaseRowClick - Enable processing of `clickRow`
+             */
+            releaseRowClick: function() {
+                CompareRowClick.disabled = false;
+                CompareRowClick.clearRowClickHandler();
+            },
+
+            /** disableRowClick - Disable processing of `clickRow` handlers for some time (allow to process clicks on inner elements)
+             */
+            disableRowClick: function() {
+                CompareRowClick.clearRowClickHandler();
+                CompareRowClick.disabled = true;
+                setTimeout(CompareRowClick.releaseRowClick, CompareRowClick.timeout);
+            },
+        };
 
-    /** disableRowClick - Disable processing of `clickRow` handlers for some time (allow to process clicks on inner elements)
-     */
-    disableRowClick: function() {
-        CompareRowClick.clearRowClickHandler();
-        CompareRowClick.disabled = true;
-        setTimeout(CompareRowClick.releaseRowClick, CompareRowClick.timeout);
+        provide(CompareRowClick);
     },
-};
+);
```

### Comparing `bw_matchbox-0.3.0/bw_matchbox/assets/js/Compare/CompareRowsHelpers.js` & `bw_matchbox-0.4.0/bw_matchbox/assets/js/Compare/CompareRowsHelpers.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,296 +1,314 @@
-/* global CommonHelpers, CompareRowClick */
-
-/* // Compare rows-related feature types (ts-like):
- * type TRowKind = 'source' | 'target';
- * type TRowEl = HTMLTableRowElement;
- * type TRowId = string;
- * interface TSelectedRow {
- *   rowKind: TRowKind;
- *   // TODO: It will be impossible to use elements for paginated tables
- *   // (because the nodes for the same elements could be different).
- *   rowEl: TRowEl;
- *   rowId: TRowId;
- * };
- * interface TCollapsedRow extends TSelectedRow { pairId: TRowId };
- */
-
-// global module variable
-const CompareRowsHelpers = {
-    // Data...
-    sharedData: undefined, // Initializing in `CompareCore.initCompare` from `bw_matchbox/assets/templates/compare.html`
-    rowColumnsCount: 5, // Number of columns in a table row...
-    selectedFirst: undefined, // <undefined | TSelectedRow>
-    collapsedRows: {}, // Record<TRowId, TCollapsedRow> -- Hash of collapsed row
-
-    // Methods...
-
-    /** getRowData -- Get row data
-     * @param {<TRowKind>} rowKind
-     * @param {<TRowId>} rowId
-     * @return {<TDataRecord>}
-     */
-    getRowData: function(rowKind, rowId) {
-        const {
-            target_data,
-            source_data
-        } = CompareRowsHelpers.sharedData;
-        const data = rowKind === 'source' ? source_data : target_data;
-        const found = data.find((item) => item.row_id === rowId);
-        return found;
-    },
-
-    /** getRowId -- Get row id
-     * @param {<TRowEl>} rowEl
-     * @return {<TRowId>}
-     */
-    getRowId(rowEl) {
-        return rowEl.getAttribute('row_id');
-    },
-
-    /** getRowKind -- Get row kind (source or target)
-     * @param {<TRowEl>} rowEl
-     * @return {<TRowKind>} (<'source' | 'target'>)
-     */
-    getRowKind(rowEl) {
-        // Find main table (source or target one)
-        const table = rowEl.closest('table');
-        const tableId = table.getAttribute('id');
-        const isSource = tableId === 'source-table';
-        // Row kind (source or target)...
-        return isSource ? 'source' : 'target';
-    },
-
-    /** selectRow -- Make row selected
-     * @param {<TRowEl>} rowEl
-     */
-    selectRow(rowEl) {
-        const rowId = CompareRowsHelpers.getRowId(rowEl);
-        const rowKind = CompareRowsHelpers.getRowKind(rowEl);
-        // Save record...
-        CompareRowsHelpers.selectedFirst = {
-            rowKind,
-            rowEl,
-            rowId
-        };
-        // Add styles...
-        rowEl.classList.add('selected');
-    },
-
-    /** unselectRow -- Make row selected
-     * @param {<TRowEl>} rowEl
-     */
-    unselectRow(rowEl) {
-        // Clear styles...
-        rowEl.classList.remove('selected');
-        // Reset saved selected record (if it's the same)...
-        if (CompareRowsHelpers.selectedFirst && CompareRowsHelpers.selectedFirst.rowEl === rowEl) {
-            CompareRowsHelpers.selectedFirst = undefined;
-        }
-    },
-
-    /** getCollapsedHandlerTooltipText -- Get collpased node tooltip text
-     * @param {<TDataRecord>} data
-     * @return {string}
-     */
-    getCollapsedHandlerTooltipText: function(data) {
-        if (!data) {
-            return 'Data is undefined';
-        }
-        const {
-            // amount, // Eg: 7.135225509515751e-9
-            amount_display, // Eg: '7.1e-09'
-            // input_id, // Eg: 633
-            location, // Eg: 'United States'
-            name, // Eg: 'Clothing; at manufacturer'
-            // row_id, // Eg: '0'
-            unit, // Eg: ''
-            // url, // Eg: '/process/633'
-        } = data;
-        const text = [
-                ['Amount', amount_display], // Eg: '7.1e-09'
-                ['Name', name], // Eg: 'Clothing; at manufacturer'
-                ['Location', location], // Eg: 'United States'
-                ['Unit', unit], // Eg: ''
-            ]
-            .map(([text, value]) => {
-                if (value) {
-                    return text + ': ' + value;
+modules.define(
+    'CompareRowsHelpers',
+    [
+        // Required modules...
+        'CommonHelpers',
+        'CompareRowClick',
+    ],
+    function provide_CompareRowsHelpers(
+        provide,
+        // Resolved modules...
+        CommonHelpers,
+        CompareRowClick,
+    ) {
+        /* // Compare rows-related feature types (ts-like):
+         * type TRowKind = 'source' | 'target';
+         * type TRowEl = HTMLTableRowElement;
+         * type TRowId = string;
+         * interface TSelectedRow {
+         *   rowKind: TRowKind;
+         *   // TODO: It will be impossible to use elements for paginated tables
+         *   // (because the nodes for the same elements could be different).
+         *   rowEl: TRowEl;
+         *   rowId: TRowId;
+         * };
+         * interface TCollapsedRow extends TSelectedRow { pairId: TRowId };
+         */
+
+        // Define module...
+
+        const CompareRowsHelpers = {
+            // Data...
+            sharedData: undefined, // Initializing in `CompareCore.initCompare` from `bw_matchbox/assets/templates/compare.html`
+            rowColumnsCount: 5, // Number of columns in a table row...
+            selectedFirst: undefined, // <undefined | TSelectedRow>
+            collapsedRows: {}, // Record<TRowId, TCollapsedRow> -- Hash of collapsed row
+
+            // Methods...
+
+            /** getRowData -- Get row data
+             * @param {<TRowKind>} rowKind
+             * @param {<TRowId>} rowId
+             * @return {<TDataRecord>}
+             */
+            getRowData(rowKind, rowId) {
+                const {
+                    target_data,
+                    source_data
+                } = CompareRowsHelpers.sharedData;
+                const data = rowKind === 'source' ? source_data : target_data;
+                const found = data.find((item) => item.row_id === rowId);
+                return found;
+            },
+
+            /** getRowId -- Get row id
+             * @param {<TRowEl>} rowEl
+             * @return {<TRowId>}
+             */
+            getRowId(rowEl) {
+                return rowEl.getAttribute('row_id');
+            },
+
+            /** getRowKind -- Get row kind (source or target)
+             * @param {<TRowEl>} rowEl
+             * @return {<TRowKind>} (<'source' | 'target'>)
+             */
+            getRowKind(rowEl) {
+                // Find main table (source or target one)
+                const table = rowEl.closest('table');
+                const tableId = table.getAttribute('id');
+                const isSource = tableId === 'source-table';
+                // Row kind (source or target)...
+                return isSource ? 'source' : 'target';
+            },
+
+            /** selectRow -- Make row selected
+             * @param {<TRowEl>} rowEl
+             */
+            selectRow(rowEl) {
+                const rowId = CompareRowsHelpers.getRowId(rowEl);
+                const rowKind = CompareRowsHelpers.getRowKind(rowEl);
+                // Save record...
+                CompareRowsHelpers.selectedFirst = {
+                    rowKind,
+                    rowEl,
+                    rowId
+                };
+                // Add styles...
+                rowEl.classList.add('selected');
+            },
+
+            /** unselectRow -- Make row selected
+             * @param {<TRowEl>} rowEl
+             */
+            unselectRow(rowEl) {
+                // Clear styles...
+                rowEl.classList.remove('selected');
+                // Reset saved selected record (if it's the same)...
+                if (CompareRowsHelpers.selectedFirst && CompareRowsHelpers.selectedFirst.rowEl === rowEl) {
+                    CompareRowsHelpers.selectedFirst = undefined;
                 }
-            })
-            .filter(Boolean)
-            .join('\n');
-        return 'COLLAPSED ROW\n' + text;
-    },
-
-    /** getCollapsedId -- Get collapsed id (`{rowKind}-{rowId}`)
-     * @param {<TRowKind>} rowKind
-     * @param {<TRowId>} rowId
-     * @return {string}
-     */
-    getCollapsedId(rowKind, rowId) {
-        return [rowKind, rowId].join('-');
-    },
-
-    /** buildCollapsedHandlerRow -- Get html content of collapsed handler node.
-     * @param {<TRowKind>} rowKind
-     * @param {<TRowId>} rowId
-     * @param [{<TDataRecord>}] optionalData
-     * @return {string}
-     */
-    buildCollapsedHandlerRow: function(rowKind, rowId, optionalData) {
-        const collapsedId = CompareRowsHelpers.getCollapsedId(rowKind, rowId);
-        const data = optionalData || CompareRowsHelpers.getRowData(rowKind, rowId);
-        const tooltipText = CompareRowsHelpers.getCollapsedHandlerTooltipText(data);
-        const quotedTooltipText = CommonHelpers.quoteHtmlAttr(tooltipText);
-        const start = `<tr
-      class="collapsed-handler"
-      for-collapsed-id="${collapsedId}"
-      title="${quotedTooltipText}"
-      onClick="CompareRowsHelpers.clickUncollapseRow(this)"
-    >`;
-        const content = `<td colspan="${CompareRowsHelpers.rowColumnsCount}"><br/></td>`;
-        const end = `</tr>`;
-        return start + content + end;
-    },
+                // TODO: Update `collapsed` field in original data?
+            },
 
-    /** collapseRowByRecord -- Collapse particular row record
-     * @param {<TCollapsedRow>} collapsedRowRecord
-     */
-    collapseRowByRecord: function(collapsedRowRecord) {
-        // TODO: For paginated tables -- don't use saved elements (they would by dynamic)!
-        // See ` uncollapseRowByRecord` for example.
-        const {
-            rowKind,
-            rowId,
-            rowEl
-        } = collapsedRowRecord;
-        const collapsedId = CompareRowsHelpers.getCollapsedId(rowKind, rowId);
-        // Add styles...
-        rowEl.classList.add('collapsed');
-        // Save id in the dom node...
-        rowEl.setAttribute('collapsed-id', collapsedId);
-        // Save record...
-        CompareRowsHelpers.collapsedRows[collapsedId] = collapsedRowRecord;
-        // Add interactive elements and other stuff (to uncollapse it later)...
-        // Create html representation and dom node to append...
-        const handlerRowHtml = CompareRowsHelpers.buildCollapsedHandlerRow(rowKind, rowId);
-        const handlerRowEl = CommonHelpers.htmlToElement(handlerRowHtml);
-        // Find parent node...
-        const parentNode = rowEl.parentNode;
-        // Add handler before current row...
-        parentNode.insertBefore(handlerRowEl, rowEl);
-    },
+            /** getCollapsedHandlerTooltipText -- Get collpased node tooltip text
+             * @param {<TDataRecord>} data
+             * @return {string}
+             */
+            getCollapsedHandlerTooltipText(data) {
+                if (!data) {
+                    return 'Data is undefined';
+                }
+                const {
+                    // amount, // Eg: 7.135225509515751e-9
+                    amount_display, // Eg: '7.1e-09'
+                    // input_id, // Eg: 633
+                    location, // Eg: 'United States'
+                    name, // Eg: 'Clothing; at manufacturer'
+                    // row_id, // Eg: '0'
+                    unit, // Eg: ''
+                    // url, // Eg: '/process/633'
+                } = data;
+                const text = [
+                        ['Amount', amount_display], // Eg: '7.1e-09'
+                        ['Name', name], // Eg: 'Clothing; at manufacturer'
+                        ['Location', location], // Eg: 'United States'
+                        ['Unit', unit], // Eg: ''
+                    ]
+                    .map(([text, value]) => {
+                        if (value) {
+                            return text + ': ' + value;
+                        }
+                    })
+                    .filter(Boolean)
+                    .join('\n');
+                return 'COLLAPSED ROW\n' + text;
+            },
+
+            /** getCollapsedId -- Get collapsed id (`{rowKind}-{rowId}`)
+             * @param {<TRowKind>} rowKind
+             * @param {<TRowId>} rowId
+             * @return {string}
+             */
+            getCollapsedId(rowKind, rowId) {
+                return [rowKind, rowId].join('-');
+            },
+
+            /** buildCollapsedHandlerRow -- Get html content of collapsed handler node.
+             * @param {<TRowKind>} rowKind
+             * @param {<TRowId>} rowId
+             * @param [{<TDataRecord>}] optionalData
+             * @return {string}
+             */
+            buildCollapsedHandlerRow(rowKind, rowId, optionalData) {
+                const collapsedId = CompareRowsHelpers.getCollapsedId(rowKind, rowId);
+                const data = optionalData || CompareRowsHelpers.getRowData(rowKind, rowId);
+                const tooltipText = CompareRowsHelpers.getCollapsedHandlerTooltipText(data);
+                const quotedTooltipText = CommonHelpers.quoteHtmlAttr(tooltipText);
+                const start = `<tr
+          class="collapsed-handler"
+          for-collapsed-id="${collapsedId}"
+          title="${quotedTooltipText}"
+          onClick="CompareCore.clickUncollapseRow(this)"
+        >`;
+                const content = `<td colspan="${CompareRowsHelpers.rowColumnsCount}"><br/></td>`;
+                const end = `</tr>`;
+                return start + content + end;
+            },
+
+            /** collapseRowByRecord -- Collapse particular row record
+             * @param {<TCollapsedRow>} collapsedRowRecord
+             */
+            collapseRowByRecord(collapsedRowRecord) {
+                // TODO: For paginated tables -- don't use saved elements (they would by dynamic)!
+                // See ` uncollapseRowByRecord` for example.
+                const {
+                    rowKind,
+                    rowId,
+                    rowEl
+                } = collapsedRowRecord;
+                const collapsedId = CompareRowsHelpers.getCollapsedId(rowKind, rowId);
+                // Add styles...
+                rowEl.classList.add('collapsed');
+                // Save id in the dom node...
+                rowEl.setAttribute('collapsed-id', collapsedId);
+                // Save record...
+                CompareRowsHelpers.collapsedRows[collapsedId] = collapsedRowRecord;
+                // Add interactive elements and other stuff (to uncollapse it later)...
+                // Create html representation and dom node to append...
+                const handlerRowHtml = CompareRowsHelpers.buildCollapsedHandlerRow(rowKind, rowId);
+                const handlerRowEl = CommonHelpers.htmlToElement(handlerRowHtml);
+                // Find parent node...
+                const parentNode = rowEl.parentNode;
+                // Add handler before current row...
+                parentNode.insertBefore(handlerRowEl, rowEl);
+            },
+
+            /** uncollapseRowByRecord -- Collapse particular row record
+             * @param {<TCollapsedRow>} collapsedRowRecord
+             */
+            uncollapseRowByRecord(collapsedRowRecord) {
+                const {
+                    rowKind,
+                    rowId
+                } = collapsedRowRecord;
+                const collapsedId = CompareRowsHelpers.getCollapsedId(rowKind, rowId);
+                const tableId = rowKind + '-table';
+                const tableNode = document.getElementById(tableId);
+                const handlerEl = tableNode.querySelector('[for-collapsed-id="' + collapsedId + '"]');
+                const rowEl = tableNode.querySelector('[collapsed-id="' + collapsedId + '"]');
+                // Remove collapsed record data...
+                CompareRowsHelpers.collapsedRows[collapsedId] = false;
+                if (handlerEl) {
+                    // Remove collapsed handler from dom (if exist in dom)...
+                    handlerEl.remove();
+                }
+                // Restore row element state (id exist in dom)...
+                if (rowEl) {
+                    rowEl.classList.remove('collapsed');
+                    rowEl.removeAttribute('collapsed-id');
+                }
+            },
 
-    /** uncollapseRowByRecord -- Collapse particular row record
-     * @param {<TCollapsedRow>} collapsedRowRecord
-     */
-    uncollapseRowByRecord: function(collapsedRowRecord) {
-        const {
-            rowKind,
-            rowId
-        } = collapsedRowRecord;
-        const collapsedId = CompareRowsHelpers.getCollapsedId(rowKind, rowId);
-        const tableId = rowKind + '-table';
-        const tableNode = document.getElementById(tableId);
-        const handlerEl = tableNode.querySelector('[for-collapsed-id="' + collapsedId + '"]');
-        const rowEl = tableNode.querySelector('[collapsed-id="' + collapsedId + '"]');
-        // Remove collapsed record data...
-        CompareRowsHelpers.collapsedRows[collapsedId] = undefined;
-        if (handlerEl) {
-            // Remove collapsed handler from dom (if exist in dom)...
-            handlerEl.remove();
-        }
-        // Restore row element state (id exist in dom)...
-        if (rowEl) {
-            rowEl.classList.remove('collapsed');
-            rowEl.removeAttribute('collapsed-id');
-        }
-    },
+            /** makeRowsCollapsed
+             * @param {<TSelectedRow>} selectedFirst
+             * @param {<TSelectedRow>} selectedSecond
+             */
+            makeRowsCollapsed(selectedFirst, selectedSecond) {
+                // TODO: To check data validity (both records are defined and well-formed)?
+                // Remove selected status...
+                CompareRowsHelpers.unselectRow(selectedFirst.rowEl);
+                CompareRowsHelpers.unselectRow(selectedSecond.rowEl);
+                // Collapse the rows...
+                const collapsedFirst = {
+                    ...selectedFirst,
+                    pairId: selectedSecond.rowId
+                };
+                const collapsedSecond = {
+                    ...selectedSecond,
+                    pairId: selectedFirst.rowId
+                };
+                CompareRowsHelpers.collapseRowByRecord(collapsedFirst);
+                CompareRowsHelpers.collapseRowByRecord(collapsedSecond);
+            },
+
+            /** clickRow
+             * @param {<TRowEl>} rowEl
+             */
+            clickRow(rowEl) {
+                if (CompareRowClick.disabled) {
+                    // Do nothing if disabled
+                    return;
+                }
+                if (rowEl.classList.contains('collapsed')) {
+                    // Do nothing if row is already collapsed
+                    return;
+                }
+                const rowId = CompareRowsHelpers.getRowId(rowEl);
+                const rowKind = CompareRowsHelpers.getRowKind(rowEl);
+                if (!CompareRowsHelpers.selectedFirst) {
+                    // Nothing selected -- select as first element...
+                    CompareRowsHelpers.selectRow(rowEl);
+                } else if (CompareRowsHelpers.selectedFirst.rowEl === rowEl) {
+                    // Already selected and clicked again -- deselect...
+                    CompareRowsHelpers.unselectRow(rowEl);
+                } else if (CompareRowsHelpers.selectedFirst.rowKind === rowKind) {
+                    // Clicked another node in the same table -- deselect old and select new...
+                    CompareRowsHelpers.unselectRow(CompareRowsHelpers.selectedFirst.rowEl);
+                    CompareRowsHelpers.selectRow(rowEl);
+                } else {
+                    // Selected second element -- make both nodes collapsed...
+                    const selectedSecond = {
+                        rowKind,
+                        rowEl,
+                        rowId
+                    };
+                    CompareRowsHelpers.makeRowsCollapsed(CompareRowsHelpers.selectedFirst, selectedSecond);
+                }
+            },
 
-    /** makeRowsCollapsed
-     * @param {<TSelectedRow>} selectedFirst
-     * @param {<TSelectedRow>} selectedSecond
-     */
-    makeRowsCollapsed: function(selectedFirst, selectedSecond) {
-        // TODO: To check data validity (both records are defined and well-formed)?
-        // Remove selected status...
-        CompareRowsHelpers.unselectRow(selectedFirst.rowEl);
-        CompareRowsHelpers.unselectRow(selectedSecond.rowEl);
-        // Collapse the rows...
-        const collapsedFirst = {
-            ...selectedFirst,
-            pairId: selectedSecond.rowId
-        };
-        const collapsedSecond = {
-            ...selectedSecond,
-            pairId: selectedFirst.rowId
+            /** clickUncollapseRow -- Uncollapse both rows for this clicked collpase handler
+             * @param {<HTMLTableRowElement>} firstHandlerEl
+             */
+            clickUncollapseRow(firstHandlerEl) {
+                // Get first collpased record by id...
+                const firstId = firstHandlerEl.getAttribute('for-collapsed-id');
+                const collapsedFirst = CompareRowsHelpers.collapsedRows[firstId];
+                if (!collapsedFirst) {
+                    throw new Error('Cannot find first collapsed element by collapsed-id: ' + firstId);
+                }
+                // Get seconds collapsed record (compose id from first `pairId`)...
+                const {
+                    rowKind,
+                    pairId
+                } = collapsedFirst;
+                const secondRowKind = rowKind === 'source' ? 'target' : 'source';
+                const secondId = CompareRowsHelpers.getCollapsedId(secondRowKind, pairId);
+                const collapsedSecond = CompareRowsHelpers.collapsedRows[secondId];
+                if (!collapsedSecond) {
+                    throw new Error('Cannot find second collapsed element by collapsed-id: ' + secondId);
+                }
+                const rootNode = firstHandlerEl.closest('.compare-tables');
+                if (!rootNode) {
+                    throw new Error('Cannot find root dom node (`.compare-tables`)');
+                }
+                // Uncollapse found rows...
+                CompareRowsHelpers.uncollapseRowByRecord(collapsedFirst);
+                CompareRowsHelpers.uncollapseRowByRecord(collapsedSecond);
+            },
         };
-        CompareRowsHelpers.collapseRowByRecord(collapsedFirst);
-        CompareRowsHelpers.collapseRowByRecord(collapsedSecond);
-    },
-
-    /** clickRow
-     * @param {<TRowEl>} rowEl
-     */
-    clickRow: function(rowEl) {
-        if (CompareRowClick.disabled) {
-            // Do nothing if disabled
-            return;
-        }
-        if (rowEl.classList.contains('collapsed')) {
-            // Do nothing if row is already collapsed
-            return;
-        }
-        const rowId = CompareRowsHelpers.getRowId(rowEl);
-        const rowKind = CompareRowsHelpers.getRowKind(rowEl);
-        if (!CompareRowsHelpers.selectedFirst) {
-            // Nothing selected -- select as first element...
-            CompareRowsHelpers.selectRow(rowEl);
-        } else if (CompareRowsHelpers.selectedFirst.rowEl === rowEl) {
-            // Already selected and clicked again -- deselect...
-            CompareRowsHelpers.unselectRow(rowEl);
-        } else if (CompareRowsHelpers.selectedFirst.rowKind === rowKind) {
-            // Clicked another node in the same table -- deselect old and select new...
-            CompareRowsHelpers.unselectRow(CompareRowsHelpers.selectedFirst.rowEl);
-            CompareRowsHelpers.selectRow(rowEl);
-        } else {
-            // Selected second element -- make both nodes collapsed...
-            const selectedSecond = {
-                rowKind,
-                rowEl,
-                rowId
-            };
-            CompareRowsHelpers.makeRowsCollapsed(CompareRowsHelpers.selectedFirst, selectedSecond);
-        }
-    },
 
-    /** clickUncollapseRow -- Uncollapse both rows for this clicked collpase handler
-     * @param {<HTMLTableRowElement>} firstHandlerEl
-     */
-    clickUncollapseRow: function(firstHandlerEl) {
-        // Get first collpased record by id...
-        const firstId = firstHandlerEl.getAttribute('for-collapsed-id');
-        const collapsedFirst = CompareRowsHelpers.collapsedRows[firstId];
-        if (!collapsedFirst) {
-            throw new Error('Cannot find first collapsed element by collapsed-id: ' + firstId);
-        }
-        // Get seconds collapsed record (compose id from first `pairId`)...
-        const {
-            rowKind,
-            pairId
-        } = collapsedFirst;
-        const secondRowKind = rowKind === 'source' ? 'target' : 'source';
-        const secondId = CompareRowsHelpers.getCollapsedId(secondRowKind, pairId);
-        const collapsedSecond = CompareRowsHelpers.collapsedRows[secondId];
-        if (!collapsedSecond) {
-            throw new Error('Cannot find second collapsed element by collapsed-id: ' + secondId);
-        }
-        const rootNode = firstHandlerEl.closest('.compare-tables');
-        if (!rootNode) {
-            throw new Error('Cannot find root dom node (`.compare-tables`)');
-        }
-        // Uncollapse found rows...
-        CompareRowsHelpers.uncollapseRowByRecord(collapsedFirst);
-        CompareRowsHelpers.uncollapseRowByRecord(collapsedSecond);
+        //; Provide module...
+        provide(CompareRowsHelpers);
     },
-};
+);
```

### Comparing `bw_matchbox-0.3.0/bw_matchbox/assets/js/ProcessesList/ProcessesListDataRender.js` & `bw_matchbox-0.4.0/bw_matchbox/assets/js/ProcessesList/ProcessesListDataRender.js`

 * *Files 16% similar despite different names*

#### js-beautify {}

```diff
@@ -1,109 +1,124 @@
-/* global
-    CommonHelpers
-    ProcessesListNodes
-*/
+modules.define(
+    'ProcessesListDataRender',
+    [
+        // Required modules...
+        'CommonHelpers',
+        'ProcessesListNodes',
+    ],
+    function provide_ProcessesListDataRender(
+        provide,
+        // Resolved modules...
+        CommonHelpers,
+        ProcessesListNodes,
+    ) {
+        // Define module...
 
-/** @descr Render table content.
- */
+        /** @descr Render table content.
+         */
 
-// global module variable
-// eslint-disable-next-line no-unused-vars
-const ProcessesListDataRender = {
-    clearTableData() {
-        const tBodyNode = ProcessesListNodes.getTBodyNode();
-        tBodyNode.replaceChildren();
-    },
+        // global module variable
+        // eslint-disable-next-line no-unused-vars
+        const ProcessesListDataRender = {
+            clearTableData() {
+                const tBodyNode = ProcessesListNodes.getTBodyNode();
+                tBodyNode.replaceChildren();
+            },
 
-    renderDataRow(rowData) {
-        const {
-            id, // 726 (required!)
-            name, // 'Electronic capacitors, resistors, coils, transformers, connectors and other components (except  semiconductors and printed circuit assemblies); at manufacturer'
-            location, // 'United States'
-            unit, // ''
-            // details_url, // '/process/726'
-            // match_url, // '/match/726'
-            matched, // false
-        } = rowData;
-        /* console.log('[ProcessesListDataRender:renderDataRow]: start', {
-         *   details_url, // '/process/726'
-         *   id, // 726
-         *   location, // 'United States'
-         *   match_url, // '/match/726'
-         *   matched, // false
-         *   name, // 'Electronic capacitors, resistors, coils, transformers, connectors and other components (except  semiconductors and printed circuit assemblies); at manufacturer'
-         *   unit, // ''
-         *   rowData,
-         * });
-         */
-        const matchUrl = '/match/' + id;
-        const matchButton = matched ?
-            `<a class="button" href="${matchUrl || ''}"><i class="fa-solid fa-check"></i> EDIT</a>` :
-            `<a class="button button-primary" href="${
-          matchUrl || ''
-        }"><i class="fa-solid fa-circle-xmark"></i> ADD</a>`;
-        const content = `
-      <tr>
-        <td><a href="/process/${id || ''}">${name || ''}</a></td>
-        <td>${location || ''}</td>
-        <td>${unit || ''}</td>
-        <td>${matchButton || ''}</td>
-      </tr>
-    `;
-        /* // Original server-side template code:
+            renderDataRow(rowData) {
+                const {
+                    id, // 726 (required!)
+                    name, // 'Electronic capacitors, resistors, coils, transformers, connectors and other components (except  semiconductors and printed circuit assemblies); at manufacturer'
+                    location, // 'United States'
+                    unit, // ''
+                    // details_url, // '/process/726'
+                    // match_url, // '/match/726'
+                    matched, // false
+                } = rowData;
+                /* console.log('[ProcessesListDataRender:renderDataRow]: start', {
+                 *   details_url, // '/process/726'
+                 *   id, // 726
+                 *   location, // 'United States'
+                 *   match_url, // '/match/726'
+                 *   matched, // false
+                 *   name, // 'Electronic capacitors, resistors, coils, transformers, connectors and other components (except  semiconductors and printed circuit assemblies); at manufacturer'
+                 *   unit, // ''
+                 *   rowData,
+                 * });
+                 */
+                const matchUrl = '/match/' + id;
+                const matchButton = matched ?
+                    `<a class="button" href="${matchUrl || ''}"><i class="fa-solid fa-check"></i> EDIT</a>` :
+                    `<a class="button button-primary" href="${
+              matchUrl || ''
+            }"><i class="fa-solid fa-circle-xmark"></i> ADD</a>`;
+                const content = `
           <tr>
-            <td><a href="{{ url_for('process_detail', id=row.id) }}">{{row.name}}</a></td>
-            <td>{{row.location}}</td>
-            <td>{{row.unit}}</td>
-            <td>
-              {% if row.matched %}
-                <a class="button" href="{{ url_for("match", source=row.id)}}"><i class="fa-solid fa-check"></i> EDIT</a>
-              {% else %}
-                <a class="button button-primary" href="{{ url_for("match", source=row.id)}}"><i class="fa-solid fa-circle-xmark"></i> ADD</a>
-              {% endif %}
-            </td>
+            <td><a href="/process/${id || ''}">${name || ''}</a></td>
+            <td>${location || ''}</td>
+            <td>${unit || ''}</td>
+            <td>${matchButton || ''}</td>
           </tr>
-        */
-        /* console.log('[ProcessesListDataRender:renderDataRow]: result', {
-         *   content,
-         *   matchUrl,
-         *   matchButton,
-         *   details_url, // '/process/726'
-         *   id, // 726
-         *   location, // 'United States'
-         *   match_url, // '/match/726'
-         *   matched, // false
-         *   name, // 'Electronic capacitors, resistors, coils, transformers, connectors and other components (except  semiconductors and printed circuit assemblies); at manufacturer'
-         *   unit, // ''
-         *   rowData,
-         * });
-         */
-        return content;
-    },
+        `;
+                /* // Original server-side template code:
+                  <tr>
+                    <td><a href="{{ url_for('process_detail', id=row.id) }}">{{row.name}}</a></td>
+                    <td>{{row.location}}</td>
+                    <td>{{row.unit}}</td>
+                    <td>
+                      {% if row.matched %}
+                        <a class="button" href="{{ url_for("match", source=row.id)}}"><i class="fa-solid fa-check"></i> EDIT</a>
+                      {% else %}
+                        <a class="button button-primary" href="{{ url_for("match", source=row.id)}}"><i class="fa-solid fa-circle-xmark"></i> ADD</a>
+                      {% endif %}
+                    </td>
+                  </tr>
+                */
+                /* console.log('[ProcessesListDataRender:renderDataRow]: result', {
+                 *   content,
+                 *   matchUrl,
+                 *   matchButton,
+                 *   details_url, // '/process/726'
+                 *   id, // 726
+                 *   location, // 'United States'
+                 *   match_url, // '/match/726'
+                 *   matched, // false
+                 *   name, // 'Electronic capacitors, resistors, coils, transformers, connectors and other components (except  semiconductors and printed circuit assemblies); at manufacturer'
+                 *   unit, // ''
+                 *   rowData,
+                 * });
+                 */
+                return content;
+            },
 
-    /** renderTableData -- Display new data rows at the end of the table.
-     * @param {<TProcessItem[]>} rows
-     * @param {object} [opts] - Options
-     * @param {boolean} [opts.append] - Append data to the end of the table (default behavior: replace)
-     */
-    renderTableData(rows, opts = {}) {
-        const tBodyNode = ProcessesListNodes.getTBodyNode();
-        /* Data item sample:
-         * - details_url: '/process/726'
-         * - id: 726
-         * - location: 'United States'
-         * - match_url: '/match/726'
-         * - matched: false
-         * - name: 'Electronic capacitors, resistors, coils, transformers, connectors and other components (except  semiconductors and printed circuit assemblies); at manufacturer'
-         * - unit: ''
-         */
-        const rowsContent = rows.map(this.renderDataRow.bind(this));
-        const rowsNodes = CommonHelpers.htmlToElements(rowsContent);
-        if (opts.append) {
-            // Append new data (will be used for incremental update)...
-            tBodyNode.append.apply(tBodyNode, rowsNodes);
-        } else {
-            // Replace data...
-            tBodyNode.replaceChildren.apply(tBodyNode, rowsNodes);
-        }
+            /** renderTableData -- Display new data rows at the end of the table.
+             * @param {<TProcessItem[]>} rows
+             * @param {object} [opts] - Options
+             * @param {boolean} [opts.append] - Append data to the end of the table (default behavior: replace)
+             */
+            renderTableData(rows, opts = {}) {
+                const tBodyNode = ProcessesListNodes.getTBodyNode();
+                /* Data item sample:
+                 * - details_url: '/process/726'
+                 * - id: 726
+                 * - location: 'United States'
+                 * - match_url: '/match/726'
+                 * - matched: false
+                 * - name: 'Electronic capacitors, resistors, coils, transformers, connectors and other components (except  semiconductors and printed circuit assemblies); at manufacturer'
+                 * - unit: ''
+                 */
+                const rowsContent = rows.map(this.renderDataRow.bind(this));
+                const rowsNodes = CommonHelpers.htmlToElements(rowsContent);
+                if (opts.append) {
+                    // Append new data (will be used for incremental update)...
+                    tBodyNode.append.apply(tBodyNode, rowsNodes);
+                } else {
+                    // Replace data...
+                    tBodyNode.replaceChildren.apply(tBodyNode, rowsNodes);
+                }
+            },
+        };
+
+        // Provide module...
+        provide(ProcessesListDataRender);
     },
-};
+);
```

### Comparing `bw_matchbox-0.3.0/bw_matchbox/assets/js/ProcessesList/ProcessesListPagination.UNUSED.js` & `bw_matchbox-0.4.0/bw_matchbox/assets/js/ProcessesList/ProcessesListPagination.UNUSED.js`

 * *Files 21% similar despite different names*

#### js-beautify {}

```diff
@@ -1,151 +1,170 @@
-/* global
-    CommonHelpers
-    ProcessesListConstants
-    ProcessesListDataLoad
-    ProcessesListNodes
-    ProcessesListData
-*/
-
-/* @desc UNUSED: Pagination support.
- *
- * Sample of pagination node in html:
- * ```
- *   <div class="table-pagination"></div>
- * ```
- */
-
-// global module variable
-// eslint-disable-next-line no-unused-vars
-const ProcessesListPagination = {
-    renderNavigationLink(id, text) {
-        return `<a pagination-id="${id}" class="link" onClick="ProcessesListPagination.onNavigationClick(this)">${text}</a>`;
-    },
-
-    renderNavigationText(text) {
-        return `<span class="text">${text}</span>`;
-    },
-
-    renderNavigationItem(item) {
-        return `<span class="item">${item}</span>`;
-    },
-
-    createPaginationItems() {
-        const {
-            pageSize
-        } = ProcessesListConstants;
-        const {
-            currentPage,
-            totalRecords
-        } = ProcessesListData;
-        const totalPages = Math.ceil(totalRecords / pageSize);
-        const lastPageNo = totalPages - 1;
-        const isFirstPage = !currentPage;
-        const isLastPage = currentPage === lastPageNo;
-        const items = [
-            // prettier-ignore
-            // this.renderNavigationText('text'),
-            !isFirstPage && this.renderNavigationLink('prev', 'Prev'),
-            !isLastPage && this.renderNavigationLink('next', 'Next'),
-            // TODO: first, last, pages...
-        ].filter(Boolean);
-        /* console.log('[ProcessesListPagination:createPaginationItems]', {
-         *   items,
-         *   pageSize,
-         *   currentPage,
-         *   totalPages,
-         *   totalRecords,
-         *   isFirstPage,
-         *   isLastPage,
-         * });
-         */
-        return items;
-    },
-
-    renderPaginationNodes() {
-        const items = this.createPaginationItems();
-        const nodes = CommonHelpers.htmlToElements(items);
-        return nodes;
-    },
-
-    renderAllPaginations() {
-        // Create pagination contents...
-        const contentItems = this.createPaginationItems();
-        // Find all the pagination blocks...
-        const rootNode = ProcessesListNodes.getRootNode();
-        const paginationNodes = rootNode.getElementsByClassName('table-pagination');
-        /* console.log('[ProcessesListPagination:renderAllPaginations]', {
-         *   contentItems,
-         *   rootNode,
-         *   paginationNodes,
-         * });
+modules.define(
+    'ProcessesListPagination',
+    [
+        // Required modules...
+        'CommonHelpers',
+        'ProcessesListConstants',
+        'ProcessesListDataLoad',
+        'ProcessesListNodes',
+        'ProcessesListData',
+    ],
+    function provide_ProcessesListPagination(
+        provide,
+        // Resolved modules...
+        CommonHelpers,
+        ProcessesListConstants,
+        ProcessesListDataLoad,
+        ProcessesListNodes,
+        ProcessesListData,
+    ) {
+        // Define module...
+
+        /* @desc UNUSED: Pagination support.
+         *
+         * Sample of pagination node in html:
+         * ```
+         *   <div class="table-pagination"></div>
+         * ```
          */
-        // Update contents of all the pagination blocks...
-        for (const node of paginationNodes) {
-            const contentNodes = CommonHelpers.htmlToElements(contentItems);
-            node.replaceChildren.apply(node, contentNodes);
-        }
-    },
 
-    /** getNavigationPageNo -- Get page number by pagination id
-     * @param {string|number} id - 'prev', 'next', 'first', 'last' or page number (as string or number)
-     * @return {number}
-     */
-    getNavigationPageNo(id) {
-        const isNumber = !isNaN(id);
-        // Number?
-        if (isNumber) {
-            return Number(id);
-        }
-        // First?
-        if (id === 'first') {
-            return 0;
-        }
-        // Next or prev?
-        const {
-            currentPage
-        } = ProcessesListData;
-        if (id === 'prev') {
-            return currentPage - 1;
-        }
-        if (id === 'next') {
-            return currentPage + 1;
-        }
-        // Last?
-        const {
-            totalRecords
-        } = ProcessesListData;
-        const {
-            pageSize
-        } = ProcessesListConstants;
-        const totalPages = Math.ceil(totalRecords / pageSize);
-        if (id === 'last') {
-            return totalPages - 1;
-        }
-        // WTF?
-        throw new Error('Unknown navigation id: ' + id);
-    },
-
-    /** onNavigationClick -- Process navigation item click
-     * @param {HTMLElement} target
-     */
-    onNavigationClick(target) {
-        const id = target.getAttribute('pagination-id');
-        const pageNo = this.getNavigationPageNo(id);
-        /* console.log('[ProcessesListPagination:onNavigationClick]', {
-         *   pageNo,
-         *   id,
-         * });
-         */
-        // TODO: Use `setPageNo` method?
-        ProcessesListData.currentPage = pageNo;
-        // TODO: Load data...
-        ProcessesListDataLoad.loadData();
-    },
+        // global module variable
+        // eslint-disable-next-line no-unused-vars
+        const ProcessesListPagination = {
+            // TODO: `ProcessesListPagination` should be exposed to global scope or `onNavigationClick` should be proxied.
+            renderNavigationLink(id, text) {
+                return `<a pagination-id="${id}" class="link" onClick="ProcessesListPagination.onNavigationClick(this)">${text}</a>`;
+            },
+
+            renderNavigationText(text) {
+                return `<span class="text">${text}</span>`;
+            },
+
+            renderNavigationItem(item) {
+                return `<span class="item">${item}</span>`;
+            },
+
+            createPaginationItems() {
+                const {
+                    pageSize
+                } = ProcessesListConstants;
+                const {
+                    currentPage,
+                    totalRecords
+                } = ProcessesListData;
+                const totalPages = Math.ceil(totalRecords / pageSize);
+                const lastPageNo = totalPages - 1;
+                const isFirstPage = !currentPage;
+                const isLastPage = currentPage === lastPageNo;
+                const items = [
+                    // prettier-ignore
+                    // this.renderNavigationText('text'),
+                    !isFirstPage && this.renderNavigationLink('prev', 'Prev'),
+                    !isLastPage && this.renderNavigationLink('next', 'Next'),
+                    // TODO: first, last, pages...
+                ].filter(Boolean);
+                /* console.log('[ProcessesListPagination:createPaginationItems]', {
+                 *   items,
+                 *   pageSize,
+                 *   currentPage,
+                 *   totalPages,
+                 *   totalRecords,
+                 *   isFirstPage,
+                 *   isLastPage,
+                 * });
+                 */
+                return items;
+            },
+
+            renderPaginationNodes() {
+                const items = this.createPaginationItems();
+                const nodes = CommonHelpers.htmlToElements(items);
+                return nodes;
+            },
+
+            renderAllPaginations() {
+                // Create pagination contents...
+                const contentItems = this.createPaginationItems();
+                // Find all the pagination blocks...
+                const rootNode = ProcessesListNodes.getRootNode();
+                const paginationNodes = rootNode.getElementsByClassName('table-pagination');
+                /* console.log('[ProcessesListPagination:renderAllPaginations]', {
+                 *   contentItems,
+                 *   rootNode,
+                 *   paginationNodes,
+                 * });
+                 */
+                // Update contents of all the pagination blocks...
+                for (const node of paginationNodes) {
+                    const contentNodes = CommonHelpers.htmlToElements(contentItems);
+                    node.replaceChildren.apply(node, contentNodes);
+                }
+            },
+
+            /** getNavigationPageNo -- Get page number by pagination id
+             * @param {string|number} id - 'prev', 'next', 'first', 'last' or page number (as string or number)
+             * @return {number}
+             */
+            getNavigationPageNo(id) {
+                const isNumber = !isNaN(id);
+                // Number?
+                if (isNumber) {
+                    return Number(id);
+                }
+                // First?
+                if (id === 'first') {
+                    return 0;
+                }
+                // Next or prev?
+                const {
+                    currentPage
+                } = ProcessesListData;
+                if (id === 'prev') {
+                    return currentPage - 1;
+                }
+                if (id === 'next') {
+                    return currentPage + 1;
+                }
+                // Last?
+                const {
+                    totalRecords
+                } = ProcessesListData;
+                const {
+                    pageSize
+                } = ProcessesListConstants;
+                const totalPages = Math.ceil(totalRecords / pageSize);
+                if (id === 'last') {
+                    return totalPages - 1;
+                }
+                // WTF?
+                throw new Error('Unknown navigation id: ' + id);
+            },
+
+            /** onNavigationClick -- Process navigation item click
+             * @param {HTMLElement} target
+             */
+            onNavigationClick(target) {
+                const id = target.getAttribute('pagination-id');
+                const pageNo = this.getNavigationPageNo(id);
+                /* console.log('[ProcessesListPagination:onNavigationClick]', {
+                 *   pageNo,
+                 *   id,
+                 * });
+                 */
+                // TODO: Use `setPageNo` method?
+                ProcessesListData.currentPage = pageNo;
+                // TODO: Load data...
+                ProcessesListDataLoad.loadData();
+            },
+
+            start() {
+                const {
+                    updatePageHandlers
+                } = ProcessesListData;
+                updatePageHandlers.push(this.renderAllPaginations.bind(this));
+            },
+        };
 
-    start() {
-        const {
-            updatePageHandlers
-        } = ProcessesListData;
-        updatePageHandlers.push(this.renderAllPaginations.bind(this));
+        // Provide module...
+        provide(ProcessesListPagination);
     },
-};
+);
```

### Comparing `bw_matchbox-0.3.0/bw_matchbox/assets/js/ProcessesList/ProcessesListSearch.js` & `bw_matchbox-0.4.0/bw_matchbox/assets/js/ProcessesList/ProcessesListSearch.js`

 * *Files 10% similar despite different names*

#### js-beautify {}

```diff
@@ -1,71 +1,87 @@
-/* global
-    CommonHelpers
-    ProcessesListData
-    ProcessesListNodes
-*/
+modules.define(
+    'ProcessesListSearch',
+    [
+        // Required modules...
+        'CommonHelpers',
+        'ProcessesListData',
+        'ProcessesListNodes',
+    ],
+    function provide_ProcessesListSearch(
+        provide,
+        // Resolved modules...
+        CommonHelpers,
+        ProcessesListData,
+        ProcessesListNodes,
+    ) {
+        // Define module...
 
-/** @descr Search bar support
- */
+        /** @descr Search bar support
+         */
 
-// global module variable
-// eslint-disable-next-line no-unused-vars
-const ProcessesListSearch = {
-    /** Go to the search page (TODO: to refactor?) */
-    doSearch() {
-        const {
-            database
-        } = ProcessesListData;
-        const {
-            searchUrl
-        } = ProcessesListData.sharedParams;
-        const searchBar = ProcessesListNodes.getSearchBarNode();
-        const searchValue = searchBar && searchBar.value;
-        // TODO: pare search value with previous (if exists)?
-        if (searchValue !== ProcessesListData.searchValue) {
-            ProcessesListData.searchValue = searchValue; // Useless due to following redirect
-            // If searchValue is empty, then go to index (processes-list, root) page, else -- to the search page...
-            const urlParams = {
-                database,
-                q: searchValue,
-            };
-            const urlQuery = CommonHelpers.makeQuery(urlParams, {
-                addQuestionSymbol: true
-            });
-            const urlBase = searchValue ? searchUrl : '/';
-            const url = urlBase + urlQuery;
-            /* console.log('[ProcessesListSearch:doSearch]', {
-             *   url,
-             *   urlQuery,
-             *   urlParams,
-             *   urlBase,
-             *   searchValue,
-             *   searchUrl,
-             * });
-             */
-            location.assign(url);
-        }
-        return false;
-    },
+        // global module variable
+        // eslint-disable-next-line no-unused-vars
+        const ProcessesListSearch = {
+            /** Go to the search page (TODO: to refactor?) */
+            doSearch() {
+                const {
+                    database
+                } = ProcessesListData;
+                const {
+                    searchUrl
+                } = ProcessesListData.sharedParams;
+                const searchBar = ProcessesListNodes.getSearchBarNode();
+                const searchValue = searchBar && searchBar.value;
+                // TODO: pare search value with previous (if exists)?
+                if (searchValue !== ProcessesListData.searchValue) {
+                    ProcessesListData.searchValue = searchValue; // Useless due to following redirect
+                    // If searchValue is empty, then go to index (processes-list, root) page, else -- to the search page...
+                    const urlParams = {
+                        database,
+                        q: searchValue,
+                    };
+                    const urlQuery = CommonHelpers.makeQuery(urlParams, {
+                        addQuestionSymbol: true
+                    });
+                    const urlBase = searchValue ? searchUrl : '/';
+                    const url = urlBase + urlQuery;
+                    /* console.log('[ProcessesListSearch:doSearch]', {
+                     *   url,
+                     *   urlQuery,
+                     *   urlParams,
+                     *   urlBase,
+                     *   searchValue,
+                     *   searchUrl,
+                     * });
+                     */
+                    location.assign(url);
+                }
+                return false;
+            },
 
-    searchKeyHandler(event) {
-        if (event.key === 'Enter') {
-            this.doSearch();
-        }
-    },
+            searchKeyHandler(event) {
+                if (event.key === 'Enter') {
+                    this.doSearch();
+                }
+            },
 
-    /** Initialize search field */
-    start() {
-        // Find the search input...
-        const searchBar = ProcessesListNodes.getSearchBarNode();
-        if (!searchBar) {
-            throw new Error('Not found search input!');
-        }
-        /* // UNUSED: ...and activate (default focus)...
-         * searchBar.focus();
-         */
-        // ...And add search handlers...
-        // Start search on input end (on focus out), not on click!
-        searchBar.addEventListener('focusout', this.doSearch.bind(this));
-        searchBar.addEventListener('keypress', this.searchKeyHandler.bind(this));
+            /** Initialize search field */
+            start() {
+                // Find the search input...
+                const searchBar = ProcessesListNodes.getSearchBarNode();
+                if (!searchBar) {
+                    throw new Error('Not found search input!');
+                }
+                /* // UNUSED: ...and activate (default focus)...
+                 * searchBar.focus();
+                 */
+                // ...And add search handlers...
+                // Start search on input end (on focus out), not on click!
+                searchBar.addEventListener('focusout', this.doSearch.bind(this));
+                searchBar.addEventListener('keypress', this.searchKeyHandler.bind(this));
+            },
+        };
+
+        // Provide module...
+        provide(ProcessesListSearch);
     },
-};
+);
```

### Comparing `bw_matchbox-0.3.0/bw_matchbox/assets/js/ProcessesList/ProcessesListStates.js` & `bw_matchbox-0.4.0/bw_matchbox/assets/js/ProcessesList/ProcessesListStates.js`

 * *Files 20% similar despite different names*

#### js-beautify {}

```diff
@@ -1,105 +1,121 @@
-/* global
-    ProcessesListData
-    ProcessesListNodes
-    ProcessesListDataRender
-    ProcessesListDataLoad
-*/
-
-/** @descr Control component's states
- */
-
-// global module variable
-// eslint-disable-next-line no-unused-vars
-const ProcessesListStates = {
-    setLoading(isLoading) {
-        // Set css class for id="processes-list-root" --> loading, set local status
-        const rootNode = ProcessesListNodes.getRootNode();
-        rootNode.classList.toggle('loading', isLoading);
-        ProcessesListData.isLoading = isLoading;
-    },
-
-    setHasData(hasData) {
-        // Set css class for root node, update local state
-        const rootNode = ProcessesListNodes.getRootNode();
-        rootNode.classList.toggle('empty', !hasData);
-        ProcessesListData.hasData = hasData;
-    },
-
-    setHasMoreData(hasMoreData) {
-        // Set css class for root node, update local state
-        const rootNode = ProcessesListNodes.getRootNode();
-        rootNode.classList.toggle('has-more-data', hasMoreData);
-        ProcessesListData.hasMoreData = hasMoreData;
-    },
-
-    /* // UNUSED: setError -- Shorthand for `setHasData`
-     * setEmpty(isEmpty) {
-     *   this.setHasData(false);
-     * },
-     */
-
-    setError(error) {
-        // TODO: Set css class for id="processes-list-root" --> error, update local state
-        const isError = !!error;
-        const rootNode = ProcessesListNodes.getRootNode();
-        const errorNode = ProcessesListNodes.getErrorNode();
-        rootNode.classList.toggle('error', isError);
-        ProcessesListData.isError = isError;
-        ProcessesListData.error = error;
-        const errorText = error ? error.message || String(error) : '';
-        // DEBUG
-        if (errorText) {
-            // eslint-disable-next-line no-console
-            console.error('[ProcessesListStates:setError]: got the error', {
-                error,
-                errorText,
-            });
-            // eslint-disable-next-line no-debugger
-            debugger;
-        }
-        // Update error block content...
-        errorNode.innerHTML = errorText;
-    },
-
-    clearData() {
-        this.setHasData(false);
-        this.setHasMoreData(true);
-        ProcessesListDataRender.clearTableData();
-    },
-
-    setOrderBy(orderBy) {
-        const rootNode = ProcessesListNodes.getRootNode();
-        const prevClass = ['order', ProcessesListData.orderBy || 'random'].filter(Boolean).join('-');
-        const nextClass = ['order', orderBy || 'random'].filter(Boolean).join('-');
-        rootNode.classList.toggle(prevClass, false);
-        rootNode.classList.toggle(nextClass, true);
-        ProcessesListData.orderBy = orderBy;
-        // Clear current data and call load data method...
-        this.clearData();
-        ProcessesListDataLoad.loadData();
-    },
-
-    /** updatePage -- Update all the page dynamic elements
-     */
-    updatePage() {
-        const {
-            updatePageHandlers
-        } = ProcessesListData;
-        // Call all the registered update handlers...
-        updatePageHandlers.forEach((handler) => {
-            try {
-                if (handler) {
-                    handler();
+modules.define(
+    'ProcessesListStates',
+    [
+        // Required modules...
+        'ProcessesListData',
+        'ProcessesListDataRender',
+        'ProcessesListNodes',
+    ],
+    function provide_ProcessesListStates(
+        provide,
+        // Resolved modules...
+        ProcessesListData,
+        ProcessesListDataRender,
+        ProcessesListNodes,
+    ) {
+        // Define module...
+
+        /** @descr Control component's states
+         */
+
+        // global module variable
+        // eslint-disable-next-line no-unused-vars
+        const ProcessesListStates = {
+            setLoading(isLoading) {
+                // Set css class for id="processes-list-root" --> loading, set local status
+                const rootNode = ProcessesListNodes.getRootNode();
+                rootNode.classList.toggle('loading', isLoading);
+                ProcessesListData.isLoading = isLoading;
+            },
+
+            setHasData(hasData) {
+                // Set css class for root node, update local state
+                const rootNode = ProcessesListNodes.getRootNode();
+                rootNode.classList.toggle('empty', !hasData);
+                ProcessesListData.hasData = hasData;
+            },
+
+            setHasMoreData(hasMoreData) {
+                // Set css class for root node, update local state
+                const rootNode = ProcessesListNodes.getRootNode();
+                rootNode.classList.toggle('has-more-data', hasMoreData);
+                ProcessesListData.hasMoreData = hasMoreData;
+            },
+
+            /* // UNUSED: setError -- Shorthand for `setHasData`
+             * setEmpty(isEmpty) {
+             *   this.setHasData(false);
+             * },
+             */
+
+            setError(error) {
+                // TODO: Set css class for id="processes-list-root" --> error, update local state
+                const isError = !!error;
+                const rootNode = ProcessesListNodes.getRootNode();
+                const errorNode = ProcessesListNodes.getErrorNode();
+                rootNode.classList.toggle('error', isError);
+                ProcessesListData.isError = isError;
+                ProcessesListData.error = error;
+                const errorText = error ? error.message || String(error) : '';
+                // DEBUG: Show error in console
+                if (errorText) {
+                    // eslint-disable-next-line no-console
+                    console.error('[ProcessesListStates:setError]: got the error', {
+                        error,
+                        errorText,
+                    });
+                    // eslint-disable-next-line no-debugger
+                    debugger;
                 }
-            } catch (error) {
-                // eslint-disable-next-line no-console
-                console.error('[ProcessesListStates:updatePage]: error (catched)', {
-                    error,
-                    handler,
+                // Update error block content...
+                errorNode.innerHTML = errorText;
+            },
+
+            clearData() {
+                this.setHasData(false);
+                this.setHasMoreData(true);
+                ProcessesListDataRender.clearTableData();
+            },
+
+            setOrderBy(orderBy) {
+                const rootNode = ProcessesListNodes.getRootNode();
+                const prevClass = ['order', ProcessesListData.orderBy || 'random']
+                    .filter(Boolean)
+                    .join('-');
+                const nextClass = ['order', orderBy || 'random'].filter(Boolean).join('-');
+                rootNode.classList.toggle(prevClass, false);
+                rootNode.classList.toggle(nextClass, true);
+                ProcessesListData.orderBy = orderBy;
+                // Clear current dataod...
+                this.clearData();
+            },
+
+            /** updatePage -- Update all the page dynamic elements
+             */
+            updatePage() {
+                const {
+                    updatePageHandlers
+                } = ProcessesListData;
+                // Call all the registered update handlers...
+                updatePageHandlers.forEach((handler) => {
+                    try {
+                        if (handler) {
+                            handler();
+                        }
+                    } catch (error) {
+                        // eslint-disable-next-line no-console
+                        console.error('[ProcessesListStates:updatePage]: error (catched)', {
+                            error,
+                            handler,
+                        });
+                        // eslint-disable-next-line no-debugger
+                        debugger;
+                    }
                 });
-                // eslint-disable-next-line no-debugger
-                debugger;
-            }
-        });
+            },
+        };
+
+        // Provide module...
+        provide(ProcessesListStates);
     },
-};
+);
```

### Comparing `bw_matchbox-0.3.0/bw_matchbox/assets/templates/compare.html` & `bw_matchbox-0.4.0/bw_matchbox/assets/templates/compare.html`

 * *Files 14% similar despite different names*

```diff
@@ -2,29 +2,37 @@
 
 <link rel="stylesheet" href="{{ url_for('static', filename='css/compare.css') }}">
 
 <script src="{{ url_for('static', filename='js/Compare/CompareRowsHelpers.js') }}"></script>
 <script src="{{ url_for('static', filename='js/Compare/CompareRowClick.js') }}"></script>
 <script src="{{ url_for('static', filename='js/Compare/CompareCore.js') }}"></script>
 
-{# Globals:
+{# Core js module:
   - `CompareCore` (from `bw_matchbox/assets/js/compare-core.js`)
 #}
 
-<div class="container compare">
-  {% include 'navigation.html' %}
-  <span class="modal-wrapper">
-    <div class="modal" id="number-editor">
-      <div class="modal-content">
-        <span class="close">&times;</span>
-        <span id="modal-content-wrapper">Number Editor</span>
+<div class="modal-wrapper">
+  <div class="modal" id="modal-number-editor">
+    <div class="modal-splash"></div>
+    <div class="modal-window">
+      <div class="modal-header">
+        <h3 class="modal-title">Modal title</h3>
+        <div class="close">&times;</div>
+      </div>
+      <div class="modal-content non-padded non-scrollable">
+        <div id="modal-content-wrapper">
+          Sample content
+        </div>
       </div>
     </div>
-  </span>
+  </div>
+</div>
 
+<div class="container compare">
+  {% include 'navigation.html' %}
   <div class="row">
     <div class="four columns">
       <h4>Location: {% if source_node.location == target_node.location %}Same{% else %}{{ source_node.location }} | {{ target_node.location }}{% endif %}</h4>
     </div>
     <div class="three columns">
       <h4>Unit: {% if source_node.unit == target_node.unit %}Same{% else %}{{ source_node.unit }} | {{ target_node.unit }}{% endif %}</h4>
     </div>
@@ -43,70 +51,56 @@
       <table class="compare-table" id="target-table" width="100%">
       </table>
     </div>
   </div>
 </div>
 
 <script>
-
-  /* // Enable debug mode...
-   * const useDebug = true;
-   */
-
-  /* // Common types (ts-like):
-   *
-   * Data record item (for `source_data` and `target_data` tables):
-   *
-   * interface TDataRecord {
-   *   amount: number; // Eg: 7.135225509515751e-9
-   *   amount_display: string; // Eg: '7.1e-09'
-   *   input_id: number; // Eg: 633
-   *   location: string; // Eg: 'United States'
-   *   name: string; // Eg: 'Clothing; at manufacturer'
-   *   row_id: string; // "0" (auto increment primary key; initilizes dynamically on the client from the first iteration)
-   *   unit: string; // Eg: ''
-   *   url: string; // Eg: '/process/633'
-   *   collapsed: boolean; // true
-   *   collapsed-group: string; // "Collapsed-XXX-YYYYYY" -- unique key to locate corresponding pair.
-   * }
-   */
-
-  // Global variables for compare tables feature (via global variable `sharedData`)...
-  const sharedData = {
-    // TODO: Separate data by shared and local.
-    source_data: {{ source_data_json|safe }}, // TDataRecord[]
-    target_data: {{ target_data_json|safe }}, // TDataRecord[]
-    target_node: {{ target_json|safe}},
-    source_id: {{ source_node.id }},
-    target_id: {{ target_node.id }},
-    target_name: '{{ target_node.name|safe }}',
-    source_node_unit: '{{source_node.unit}}',
-    source_node_location: '{{source_node.location}}',
-  };
-
-  /* // DEBUG: Crop data table to easier debugging...
-   * if (useDebug) {
-   *   sharedData.source_data.length = 2;
-   *   sharedData.target_data.length = 2;
-   * }
-   */
-
-  /* // DEBUG: Emulate pre-collapsed elements data...
-   * if (useDebug) {
-   *   // Link first columns...
-   *   const collapsedGroupId = 'Collapsed-0-abcdef'
-   *   sharedData.source_data[0].collapsed = true
-   *   sharedData.source_data[0]['collapsed-group'] = collapsedGroupId;
-   *   sharedData.target_data[0].collapsed = true
-   *   sharedData.target_data[0]['collapsed-group'] = collapsedGroupId;
-   *   console.log('DEBUG: Emulate pre-collapsed elements data', {
-   *     source_data: sharedData.source_data,
-   *     target_data: sharedData.target_data,
-   *   });
-   *   debugger;
-   * }
-   */
-
-  CompareCore.initCompare(sharedData);
-
+  modules.require('CompareCore', (CompareCore) => {
+    /* // Enable debug mode...
+     * const useDebug = true;
+     * // TODO: Expose it to global scope?
+     */
+
+    // Global variables for compare tables feature (via global variable `sharedData`)...
+    const sharedData = {
+      source_data: {{ source_data_json|safe }}, // TDataRecord[]
+      target_data: {{ target_data_json|safe }}, // TDataRecord[]
+      target_node: {{ target_json|safe}},
+      source_id: {{ source_node.id }},
+      target_id: {{ target_node.id }},
+      target_name: '{{ target_node.name|safe }}',
+      source_node_unit: '{{source_node.unit}}',
+      source_node_location: '{{source_node.location}}',
+    };
+
+    /* // DEBUG: Crop data table to easier debugging...
+     * if (useDebug) {
+     *   sharedData.source_data.length = 2;
+     *   sharedData.target_data.length = 2;
+     * }
+     */
+
+    /* // DEBUG: Emulate pre-collapsed elements data...
+     * if (useDebug) {
+     *   // Link first columns...
+     *   const collapsedGroupId = 'Collapsed-0-abcdef'
+     *   sharedData.source_data[0].collapsed = true
+     *   sharedData.source_data[0]['collapsed-group'] = collapsedGroupId;
+     *   sharedData.target_data[0].collapsed = true
+     *   sharedData.target_data[0]['collapsed-group'] = collapsedGroupId;
+     *   console.log('DEBUG: Emulate pre-collapsed elements data', {
+     *     source_data: sharedData.source_data,
+     *     target_data: sharedData.target_data,
+     *   });
+     *   debugger;
+     * }
+     */
+
+    // Export to global scope (to access from generated html code handlers).
+    window.CompareCore = CompareCore;
+
+    // Start core module...
+    CompareCore.start(sharedData);
+  });
 </script>
 {% include 'footer.html' %}
```

#### html2text {}

```diff
@@ -1,11 +1,14 @@
 {% include 'header.html' %}
- {# Globals: - `CompareCore` (from `bw_matchbox/assets/js/compare-core.js`) #}
+ {# Core js module: - `CompareCore` (from `bw_matchbox/assets/js/compare-
+core.js`) #}
+**** Modal title ****
+×
+Sample content
 {% include 'navigation.html' %}
-× Number Editor
 *** Location: {% if source_node.location == target_node.location %}Same{% else
 %}{{ source_node.location }} | {{ target_node.location }}{% endif %} ***
 *** Unit: {% if source_node.unit == target_node.unit %}Same{% else %}{
 { source_node.unit }} | {{ target_node.unit }}{% endif %} ***
 {% if proxy and proxy != "None" %}Create Proxy 1-to-1 Proxy{% else %}Save{%
 endif %}
 **** {{ source_node.name }} ****
```

### Comparing `bw_matchbox-0.3.0/bw_matchbox/assets/templates/databases.html` & `bw_matchbox-0.4.0/bw_matchbox/assets/templates/databases.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.3.0/bw_matchbox/assets/templates/header.html` & `bw_matchbox-0.4.0/bw_matchbox/assets/templates/header.html`

 * *Files 7% similar despite different names*

```diff
@@ -9,33 +9,35 @@
   <meta name="description" content="">
   <meta name="author" content="">
 
   <!-- Mobile Specific Metas
   –––––––––––––––––––––––––––––––––––––––––––––––––– -->
   <meta name="viewport" content="width=device-width, initial-scale=1">
 
+  {# DEBUG: Reming of next two rows allows to debug current code w/o live internet (don't need to make external connections). #}
   <!-- FONT
-  –––––––––––––––––––––––––––––––––––––––––––––––––– -->
+    –––––––––––––––––––––––––––––––––––––––––––––––––– -->
   <link href="//fonts.googleapis.com/css?family=Raleway:400,300,600" rel="stylesheet" type="text/css">
-
   <!-- ICONS
-  –––––––––––––––––––––––––––––––––––––––––––––––––– -->
+    –––––––––––––––––––––––––––––––––––––––––––––––––– -->
   <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
 
   <!-- CSS
   –––––––––––––––––––––––––––––––––––––––––––––––––– -->
   <link rel="stylesheet" href="{{ url_for('static', filename='css/normalize.css') }}">
   <link rel="stylesheet" href="{{ url_for('static', filename='css/tooltip.css') }}">
   <link rel="stylesheet" href="{{ url_for('static', filename='css/skeleton.css') }}">
   <link rel="stylesheet" href="{{ url_for('static', filename='css/customizations.css') }}">
   <link rel="stylesheet" href="{{ url_for('static', filename='css/common.css') }}">
+  <link rel="stylesheet" href="{{ url_for('static', filename='css/modal.css') }}">
 
   <!-- Scripts
   –––––––––––––––––––––––––––––––––––––––––––––––––– -->
-  <script src="{{ url_for('static', filename='js/CommonHelpers.js') }}"></script>
+  <script src="{{ url_for('static', filename='js/libs/ym/ym-modules-0.1.2.min.js') }}"></script>
+  <script src="{{ url_for('static', filename='js/common/CommonHelpers.js') }}"></script>
   {# TODO: to move to the body end? #}
 
   <!-- Favicon
   –––––––––––––––––––––––––––––––––––––––––––––––––– -->
   <link rel="icon" type="image/png" href="{{ url_for('static', filename='images/favicon.ico') }}">
 
 </head>
```

#### html2text {}

```diff
@@ -1,10 +1,12 @@
 
 
 
+ {# DEBUG: Reming of next two rows allows to debug current code w/o live
+internet (don't need to make external connections). #}
```

### Comparing `bw_matchbox-0.3.0/bw_matchbox/assets/templates/index.html` & `bw_matchbox-0.4.0/bw_matchbox/assets/templates/index.html`

 * *Files 15% similar despite different names*

```diff
@@ -3,38 +3,38 @@
 <link rel="stylesheet" href="{{ url_for('static', filename='css/processes-list.css') }}">
 
 <script src="{{ url_for('static', filename='js/ProcessesList/ProcessesListConstants.js') }}"></script>
 <script src="{{ url_for('static', filename='js/ProcessesList/ProcessesListData.js') }}"></script>
 <script src="{{ url_for('static', filename='js/ProcessesList/ProcessesListDataLoad.js') }}"></script>
 <script src="{{ url_for('static', filename='js/ProcessesList/ProcessesListDataRender.js') }}"></script>
 <script src="{{ url_for('static', filename='js/ProcessesList/ProcessesListNodes.js') }}"></script>
-{# UNUSED ProcessesListPagination -- Using incremental data loading
-<script src="{{ url_for('static', filename='js/ProcessesList/ProcessesListPagination.js') }}"></script>
-#}
 <script src="{{ url_for('static', filename='js/ProcessesList/ProcessesListSearch.js') }}"></script>
 <script src="{{ url_for('static', filename='js/ProcessesList/ProcessesListStates.js') }}"></script>
 <script src="{{ url_for('static', filename='js/ProcessesList/ProcessesList.js') }}"></script>
+{# UNUSED ProcessesListPagination -- Using incremental data loading
+<script src="{{ url_for('static', filename='js/ProcessesList/ProcessesListPagination.js') }}"></script>
+#}
 
-{# Globals:
-  - `ProcessesList` (from `bw_matchbox/assets/js/processes-list.js`)
+{# Core module:
+  - `ProcessesList` (from `bw_matchbox/assets/js/ProcessesList.js`)
 #}
 
 <div id="processes-list-root" class="container processes-list empty loading order-random">
   {% include 'navigation.html' %}
   <div class="row">
     <div class="column">
       <div class="page-header">
         <h1>
           {% if unmatched_link %}Source Database <a href="{{ url_for('unmatched') }}">(Only unmatched)</a>
           {% else %}Unmatched in Source Database
           {% endif %}
         </h1>
       </div>
       <div class="page-search">
-        <p><input class="u-full-width" placeholder="Enter value to search" value="{{ query_string }}" id="query_string"></p>
+        <p><input type="text" class="u-full-width" placeholder="Enter value to search" value="{{ query_string }}" id="query_string" /></p>
       </div>
       <div class="page-filters">
         {# Controls for `order_by` parameter (name, location, product; default
         is (empty) i.e. random (see `order-random` for `.processes-list` root
         node. #}
         <label class="radio-group-title">Order by:</label>
         <input type="radio" name="order_by" id="order_by_random" value="" onChange="ProcessesList.onOrderByChange(this)" checked>
@@ -71,16 +71,22 @@
         <div id="loader-splash" class="loader-splash full-cover"><div class="loader-spinner"></div></div>
       </div>
     </div>
   </div>
 </div>
 
 <script type="text/javascript">
-  // Initialize page data...
-  const sharedParams = {
-    searchUrl: '{{ url_for("search") }}',
-    database: '{{ database }}',
-  };
-  // Start page routines...
-  ProcessesList.start(sharedParams);
+  modules.require('ProcessesList', (ProcessesList) => {
+    // Initialize page data...
+    const sharedParams = {
+      searchUrl: '{{ url_for("search") }}',
+      database: '{{ database }}',
+    };
+
+    // Export to global scope (to access from generated html code handlers).
+    window.ProcessesList = ProcessesList;
+
+    // Start core module...
+    ProcessesList.start(sharedParams);
+  });
 </script>
 {% include 'footer.html' %}
```

#### html2text {}

```diff
@@ -1,12 +1,11 @@
 {% include 'header.html' %}
  {# UNUSED ProcessesListPagination -- Using incremental data loading
- #}
- {# Globals: - `ProcessesList` (from `bw_matchbox/assets/js/processes-list.js`)
-#}
+ #} {# Core module: - `ProcessesList` (from `bw_matchbox/assets/js/
+ProcessesList.js`) #}
 {% include 'navigation.html' %}
 ****** {% if unmatched_link %}Source Database (Only_unmatched) {% else
 %}Unmatched in Source Database {% endif %} ******
 [{{ query_string }}  ]
 {# Controls for `order_by` parameter (name, location, product; default is
 (empty) i.e. random (see `order-random` for `.processes-list` root node. #}
 Order by: # Random o Name o Location o Product
```

### Comparing `bw_matchbox-0.3.0/bw_matchbox/assets/templates/match-status.html` & `bw_matchbox-0.4.0/bw_matchbox/assets/templates/match-status.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.3.0/bw_matchbox/assets/templates/match.html` & `bw_matchbox-0.4.0/bw_matchbox/assets/templates/match.html`

 * *Files 20% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     <div class="column">
       <h2>{{ ds.name }}</h2>
       <ul>
         <li>Location: {{ds.location}}</li>
         <li>Unit: {{ds.unit}}</li>
         <li>Comment: {{ds.comment}}</li>
       </ul>
-      <p><input class="u-full-width" placeholder="{{ query_string }}" id="query_string"></p>
+      <p><input type="text" class="u-full-width" placeholder="Enter value to search" value="{{ query_string }}" id="query_string" /></p>
       <table id="result-table">
         <tr>
           <th>Activity</th>
           <th>Product</th>
           <th>Location</th>
           <th>Unit</th>
         </tr>
@@ -27,33 +27,33 @@
         {% endfor %}
       </table>
     </div>
   </div>
 </div>
 
 <script type="text/javascript">
-var search_bar = document.getElementById("query_string");
-search_bar.focus();
+var searchBar = document.getElementById('query_string');
+searchBar.focus();
 
-var result_table = document.getElementById("result-table");
+var result_table = document.getElementById('result-table');
 function search_result_updater() {
   result_table.innerHTML = this.responseText;
 }
 
-var do_search = function () {
-  var qs = encodeURIComponent(document.getElementById("query_string").value);
+var doSearch = function () {
+  var qs = encodeURIComponent(searchBar.value);
   if (qs) {
     const req = new XMLHttpRequest();
-    req.addEventListener("load", search_result_updater);
-    req.open("GET", "{{ url_for('search') }}?e=1&source={{ ds.id }}&database=ecoinvent-3.9-cutoff&q=" + qs);
+    req.addEventListener('load', search_result_updater);
+    req.open('GET', '{{ url_for('search') }}?e=1&source={{ ds.id }}&database=ecoinvent-3.9-cutoff&q=' + qs);
     req.send();
   };
 };
 
-search_bar.addEventListener("click", do_search);
-search_bar.addEventListener("keypress", function(event) {
-  if (event.key === "Enter") {
-    do_search();
+searchBar.addEventListener('focusout', doSearch);
+searchBar.addEventListener('keypress', function(event) {
+  if (event.key === 'Enter') {
+    doSearch();
   }
 });
 </script>
 {% include 'footer.html' %}
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
 {% include 'header.html' %}
 {% include 'navigation.html' %}
 ***** {{ ds.name }} *****
     * Location: {{ds.location}}
     * Unit: {{ds.unit}}
     * Comment: {{ds.comment}}
-[                    ]
+[{{ query_string }}  ]
 Activity     Product                       Location           Unit
 {{obj.name}} {{ obj["reference product"]}} {{ obj.location }} {{ obj.unit }}
  {% include 'footer.html' %}
```

### Comparing `bw_matchbox-0.3.0/bw_matchbox/assets/templates/navigation.html` & `bw_matchbox-0.4.0/bw_matchbox/assets/templates/navigation.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.3.0/bw_matchbox/assets/templates/process_detail.html` & `bw_matchbox-0.4.0/bw_matchbox/assets/templates/process_detail.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.3.0/bw_matchbox/assets/templates/project.html` & `bw_matchbox-0.4.0/bw_matchbox/assets/templates/project.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.3.0/bw_matchbox/assets/templates/search.html` & `bw_matchbox-0.4.0/bw_matchbox/assets/templates/search.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.3.0/bw_matchbox/assets/templates/search_result.html` & `bw_matchbox-0.4.0/bw_matchbox/assets/templates/search_result.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.3.0/bw_matchbox/assets/templates/select_files.html` & `bw_matchbox-0.4.0/bw_matchbox/assets/templates/select_files.html`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.3.0/bw_matchbox/bin/matchbox.py` & `bw_matchbox-0.4.0/bw_matchbox/bin/matchbox.py`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.3.0/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-mining.json` & `bw_matchbox-0.4.0/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-mining.json`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.3.0/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-string-matching.json` & `bw_matchbox-0.4.0/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-string-matching.json`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.3.0/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-transport.json` & `bw_matchbox-0.4.0/bw_matchbox/data/UVEK-2022-to-ecoinvent-3.9-partial-transport.json`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.3.0/bw_matchbox/data/dare.json` & `bw_matchbox-0.4.0/bw_matchbox/data/dare.json`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.3.0/bw_matchbox/utils.py` & `bw_matchbox-0.4.0/bw_matchbox/utils.py`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.3.0/bw_matchbox/webapp.py` & `bw_matchbox-0.4.0/bw_matchbox/webapp.py`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.3.0/bw_matchbox.egg-info/PKG-INFO` & `bw_matchbox-0.4.0/bw_matchbox.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bw-matchbox
-Version: 0.3.0
+Version: 0.4.0
 Summary: Browser to match Brightway databases
 Home-page: https://github.com/cauldron/bw_matchbox
 Author: Chris Mutel
 Author-email: <cmutel@gmail.com>
 Maintainer: Chris Mutel
 Maintainer-email: <cmutel@gmail.com>
 License: MIT
```

### Comparing `bw_matchbox-0.3.0/bw_matchbox.egg-info/SOURCES.txt` & `bw_matchbox-0.4.0/bw_matchbox.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -6,36 +6,38 @@
 ./bw_matchbox/VERSION
 ./bw_matchbox/__init__.py
 ./bw_matchbox/utils.py
 ./bw_matchbox/webapp.py
 ./bw_matchbox/assets/css/common.css
 ./bw_matchbox/assets/css/compare.css
 ./bw_matchbox/assets/css/customizations.css
+./bw_matchbox/assets/css/modal.css
 ./bw_matchbox/assets/css/normalize.css
 ./bw_matchbox/assets/css/processes-list.css
 ./bw_matchbox/assets/css/skeleton.css
 ./bw_matchbox/assets/css/tooltip.css
 ./bw_matchbox/assets/images/favicon.ico
-./bw_matchbox/assets/js/CommonHelpers.js
 ./bw_matchbox/assets/js/Compare/CompareCore.js
 ./bw_matchbox/assets/js/Compare/CompareRowClick.js
 ./bw_matchbox/assets/js/Compare/CompareRowsHelpers.js
 ./bw_matchbox/assets/js/ProcessesList/ProcessesList.js
 ./bw_matchbox/assets/js/ProcessesList/ProcessesListConstants.js
 ./bw_matchbox/assets/js/ProcessesList/ProcessesListData.js
 ./bw_matchbox/assets/js/ProcessesList/ProcessesListDataLoad.js
 ./bw_matchbox/assets/js/ProcessesList/ProcessesListDataRender.js
 ./bw_matchbox/assets/js/ProcessesList/ProcessesListNodes.js
 ./bw_matchbox/assets/js/ProcessesList/ProcessesListPagination.UNUSED.js
 ./bw_matchbox/assets/js/ProcessesList/ProcessesListSearch.js
 ./bw_matchbox/assets/js/ProcessesList/ProcessesListStates.js
+./bw_matchbox/assets/js/common/CommonHelpers.js
+./bw_matchbox/assets/js/libs/ym/ym-modules-0.1.2.js
+./bw_matchbox/assets/js/libs/ym/ym-modules-0.1.2.min.js
 ./bw_matchbox/assets/templates/compare.html
 ./bw_matchbox/assets/templates/databases.html
 ./bw_matchbox/assets/templates/expand.html
-./bw_matchbox/assets/templates/file.html
 ./bw_matchbox/assets/templates/footer.html
 ./bw_matchbox/assets/templates/header.html
 ./bw_matchbox/assets/templates/index.html
 ./bw_matchbox/assets/templates/match-status.html
 ./bw_matchbox/assets/templates/match.html
 ./bw_matchbox/assets/templates/navigation.html
 ./bw_matchbox/assets/templates/process_detail.html
@@ -58,36 +60,38 @@
 bw_matchbox.egg-info/entry_points.txt
 bw_matchbox.egg-info/not-zip-safe
 bw_matchbox.egg-info/requires.txt
 bw_matchbox.egg-info/top_level.txt
 bw_matchbox/assets/css/common.css
 bw_matchbox/assets/css/compare.css
 bw_matchbox/assets/css/customizations.css
+bw_matchbox/assets/css/modal.css
 bw_matchbox/assets/css/normalize.css
 bw_matchbox/assets/css/processes-list.css
 bw_matchbox/assets/css/skeleton.css
 bw_matchbox/assets/css/tooltip.css
 bw_matchbox/assets/images/favicon.ico
-bw_matchbox/assets/js/CommonHelpers.js
 bw_matchbox/assets/js/Compare/CompareCore.js
 bw_matchbox/assets/js/Compare/CompareRowClick.js
 bw_matchbox/assets/js/Compare/CompareRowsHelpers.js
 bw_matchbox/assets/js/ProcessesList/ProcessesList.js
 bw_matchbox/assets/js/ProcessesList/ProcessesListConstants.js
 bw_matchbox/assets/js/ProcessesList/ProcessesListData.js
 bw_matchbox/assets/js/ProcessesList/ProcessesListDataLoad.js
 bw_matchbox/assets/js/ProcessesList/ProcessesListDataRender.js
 bw_matchbox/assets/js/ProcessesList/ProcessesListNodes.js
 bw_matchbox/assets/js/ProcessesList/ProcessesListPagination.UNUSED.js
 bw_matchbox/assets/js/ProcessesList/ProcessesListSearch.js
 bw_matchbox/assets/js/ProcessesList/ProcessesListStates.js
+bw_matchbox/assets/js/common/CommonHelpers.js
+bw_matchbox/assets/js/libs/ym/ym-modules-0.1.2.js
+bw_matchbox/assets/js/libs/ym/ym-modules-0.1.2.min.js
 bw_matchbox/assets/templates/compare.html
 bw_matchbox/assets/templates/databases.html
 bw_matchbox/assets/templates/expand.html
-bw_matchbox/assets/templates/file.html
 bw_matchbox/assets/templates/footer.html
 bw_matchbox/assets/templates/header.html
 bw_matchbox/assets/templates/index.html
 bw_matchbox/assets/templates/match-status.html
 bw_matchbox/assets/templates/match.html
 bw_matchbox/assets/templates/navigation.html
 bw_matchbox/assets/templates/process_detail.html
```

### Comparing `bw_matchbox-0.3.0/docs/conf.py` & `bw_matchbox-0.4.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `bw_matchbox-0.3.0/setup.cfg` & `bw_matchbox-0.4.0/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -45,20 +45,19 @@
 [options.packages.find]
 where = .
 exclude = 
 	tests
 
 [options.package_data]
 bw_matchbox = 
-	assets/js/*.js
-	assets/js/ProcessesList/*.js
-	assets/js/Compare/*.js
+	assets/css/*.css
 	assets/images/*.ico
+	assets/js/**/*.js
+	assets/js/*.js
 	assets/templates/*.html
-	assets/css/*.css
 	data/*.json
 	VERSION
 
 [options.extras_require]
 testing = 
 	setuptools
 	pytest
```

