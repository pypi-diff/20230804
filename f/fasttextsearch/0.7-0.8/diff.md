# Comparing `tmp/fasttextsearch-0.7.tar.gz` & `tmp/fasttextsearch-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fasttextsearch-0.7.tar", last modified: Tue Jul 25 03:33:14 2023, max compression
+gzip compressed data, was "fasttextsearch-0.8.tar", last modified: Fri Aug  4 14:25:14 2023, max compression
```

## Comparing `fasttextsearch-0.7.tar` & `fasttextsearch-0.8.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 03:33:14.384418 fasttextsearch-0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-07-25 03:29:42.000000 fasttextsearch-0.7/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-25 03:29:42.000000 fasttextsearch-0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-07-25 03:33:14.384418 fasttextsearch-0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-25 03:29:42.000000 fasttextsearch-0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 03:33:14.368418 fasttextsearch-0.7/cmake/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 03:33:14.368418 fasttextsearch-0.7/cmake/Modules/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 03:33:14.368418 fasttextsearch-0.7/cmake/Modules/FetchContent/
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-07-25 03:29:42.000000 fasttextsearch-0.7/cmake/Modules/FetchContent/CMakeLists.cmake.in
--rw-r--r--   0 runner    (1001) docker     (123)    38023 2023-07-25 03:29:42.000000 fasttextsearch-0.7/cmake/Modules/FetchContent.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-25 03:29:42.000000 fasttextsearch-0.7/cmake/Modules/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 03:29:42.000000 fasttextsearch-0.7/cmake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-07-25 03:29:42.000000 fasttextsearch-0.7/cmake/googletest.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-07-25 03:29:42.000000 fasttextsearch-0.7/cmake/pybind11.cmake
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 03:33:14.368418 fasttextsearch-0.7/fasttextsearch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-07-25 03:33:14.000000 fasttextsearch-0.7/fasttextsearch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-07-25 03:33:14.000000 fasttextsearch-0.7/fasttextsearch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 03:33:14.000000 fasttextsearch-0.7/fasttextsearch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-25 03:33:14.000000 fasttextsearch-0.7/fasttextsearch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-25 03:33:14.000000 fasttextsearch-0.7/fasttextsearch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-07-25 03:29:42.000000 fasttextsearch-0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-25 03:29:42.000000 fasttextsearch-0.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 03:33:14.384418 fasttextsearch-0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4215 2023-07-25 03:29:42.000000 fasttextsearch-0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 03:33:14.372418 fasttextsearch-0.7/textsearch/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-25 03:29:42.000000 fasttextsearch-0.7/textsearch/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 03:33:14.372418 fasttextsearch-0.7/textsearch/csrc/
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-25 03:29:42.000000 fasttextsearch-0.7/textsearch/csrc/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)    13272 2023-07-25 03:29:42.000000 fasttextsearch-0.7/textsearch/csrc/levenshtein.h
--rw-r--r--   0 runner    (1001) docker     (123)     4137 2023-07-25 03:29:42.000000 fasttextsearch-0.7/textsearch/csrc/levenshtein_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)     4694 2023-07-25 03:29:42.000000 fasttextsearch-0.7/textsearch/csrc/match.cc
--rw-r--r--   0 runner    (1001) docker     (123)     4611 2023-07-25 03:29:42.000000 fasttextsearch-0.7/textsearch/csrc/match.h
--rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-07-25 03:29:42.000000 fasttextsearch-0.7/textsearch/csrc/match_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)     5273 2023-07-25 03:29:42.000000 fasttextsearch-0.7/textsearch/csrc/suffix_array.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3207 2023-07-25 03:29:42.000000 fasttextsearch-0.7/textsearch/csrc/suffix_array.h
--rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-07-25 03:29:42.000000 fasttextsearch-0.7/textsearch/csrc/suffix_array_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-07-25 03:29:42.000000 fasttextsearch-0.7/textsearch/csrc/utils.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-07-25 03:29:42.000000 fasttextsearch-0.7/textsearch/csrc/utils.h
--rw-r--r--   0 runner    (1001) docker     (123)     4862 2023-07-25 03:29:42.000000 fasttextsearch-0.7/textsearch/csrc/utils_test.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 03:33:14.376418 fasttextsearch-0.7/textsearch/python/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-25 03:29:42.000000 fasttextsearch-0.7/textsearch/python/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 03:33:14.376418 fasttextsearch-0.7/textsearch/python/csrc/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-25 03:29:42.000000 fasttextsearch-0.7/textsearch/python/csrc/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5003 2023-07-25 03:29:42.000000 fasttextsearch-0.7/textsearch/python/csrc/levenshtein.cc
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-07-25 03:29:42.000000 fasttextsearch-0.7/textsearch/python/csrc/levenshtein.h
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-07-25 03:29:42.000000 fasttextsearch-0.7/textsearch/python/csrc/match.cc
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-07-25 03:29:42.000000 fasttextsearch-0.7/textsearch/python/csrc/match.h
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-07-25 03:29:42.000000 fasttextsearch-0.7/textsearch/python/csrc/suffix_array.cc
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-07-25 03:29:42.000000 fasttextsearch-0.7/textsearch/python/csrc/suffix_array.h
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-07-25 03:29:42.000000 fasttextsearch-0.7/textsearch/python/csrc/text_search.cc
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-25 03:29:42.000000 fasttextsearch-0.7/textsearch/python/csrc/text_search.h
--rw-r--r--   0 runner    (1001) docker     (123)     4599 2023-07-25 03:29:42.000000 fasttextsearch-0.7/textsearch/python/csrc/utils.cc
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-25 03:29:42.000000 fasttextsearch-0.7/textsearch/python/csrc/utils.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 03:33:14.380418 fasttextsearch-0.7/textsearch/python/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-07-25 03:29:42.000000 fasttextsearch-0.7/textsearch/python/tests/CMakeLists.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     4748 2023-07-25 03:29:42.000000 fasttextsearch-0.7/textsearch/python/tests/test_find_close_matches.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1943 2023-07-25 03:29:42.000000 fasttextsearch-0.7/textsearch/python/tests/test_levenshtein_distance.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1414 2023-07-25 03:29:42.000000 fasttextsearch-0.7/textsearch/python/tests/test_match.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      950 2023-07-25 03:29:42.000000 fasttextsearch-0.7/textsearch/python/tests/test_row_ids_to_row_splits.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10687 2023-07-25 03:29:42.000000 fasttextsearch-0.7/textsearch/python/tests/test_sourced_text.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1359 2023-07-25 03:29:42.000000 fasttextsearch-0.7/textsearch/python/tests/test_suffix_array.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2007 2023-07-25 03:29:42.000000 fasttextsearch-0.7/textsearch/python/tests/test_text_source.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2314 2023-07-25 03:29:42.000000 fasttextsearch-0.7/textsearch/python/tests/test_transcript.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 03:33:14.384418 fasttextsearch-0.7/textsearch/python/textsearch/
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-25 03:33:14.000000 fasttextsearch-0.7/textsearch/python/textsearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13469 2023-07-25 03:29:42.000000 fasttextsearch-0.7/textsearch/python/textsearch/datatypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-07-25 03:29:42.000000 fasttextsearch-0.7/textsearch/python/textsearch/levenshtein.py
--rw-r--r--   0 runner    (1001) docker     (123)    52271 2023-07-25 03:29:42.000000 fasttextsearch-0.7/textsearch/python/textsearch/match.py
--rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-07-25 03:29:42.000000 fasttextsearch-0.7/textsearch/python/textsearch/suffix_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-07-25 03:29:42.000000 fasttextsearch-0.7/textsearch/python/textsearch/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 14:25:14.846183 fasttextsearch-0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-08-04 14:21:28.000000 fasttextsearch-0.8/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-08-04 14:21:28.000000 fasttextsearch-0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-08-04 14:25:14.846183 fasttextsearch-0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-08-04 14:21:28.000000 fasttextsearch-0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 14:25:14.838183 fasttextsearch-0.8/cmake/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 14:25:14.838183 fasttextsearch-0.8/cmake/Modules/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 14:25:14.838183 fasttextsearch-0.8/cmake/Modules/FetchContent/
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-08-04 14:21:28.000000 fasttextsearch-0.8/cmake/Modules/FetchContent/CMakeLists.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (123)    38023 2023-08-04 14:21:28.000000 fasttextsearch-0.8/cmake/Modules/FetchContent.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-08-04 14:21:28.000000 fasttextsearch-0.8/cmake/Modules/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 14:21:28.000000 fasttextsearch-0.8/cmake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-08-04 14:21:28.000000 fasttextsearch-0.8/cmake/googletest.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-08-04 14:21:28.000000 fasttextsearch-0.8/cmake/pybind11.cmake
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 14:25:14.838183 fasttextsearch-0.8/fasttextsearch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-08-04 14:25:14.000000 fasttextsearch-0.8/fasttextsearch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-08-04 14:25:14.000000 fasttextsearch-0.8/fasttextsearch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 14:25:14.000000 fasttextsearch-0.8/fasttextsearch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-04 14:25:14.000000 fasttextsearch-0.8/fasttextsearch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-04 14:25:14.000000 fasttextsearch-0.8/fasttextsearch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-08-04 14:21:28.000000 fasttextsearch-0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-04 14:21:28.000000 fasttextsearch-0.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 14:25:14.846183 fasttextsearch-0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4215 2023-08-04 14:21:28.000000 fasttextsearch-0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 14:25:14.838183 fasttextsearch-0.8/textsearch/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-08-04 14:21:28.000000 fasttextsearch-0.8/textsearch/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 14:25:14.842183 fasttextsearch-0.8/textsearch/csrc/
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-08-04 14:21:28.000000 fasttextsearch-0.8/textsearch/csrc/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    13272 2023-08-04 14:21:28.000000 fasttextsearch-0.8/textsearch/csrc/levenshtein.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4137 2023-08-04 14:21:28.000000 fasttextsearch-0.8/textsearch/csrc/levenshtein_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     4694 2023-08-04 14:21:28.000000 fasttextsearch-0.8/textsearch/csrc/match.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     4611 2023-08-04 14:21:28.000000 fasttextsearch-0.8/textsearch/csrc/match.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-08-04 14:21:28.000000 fasttextsearch-0.8/textsearch/csrc/match_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     5273 2023-08-04 14:21:28.000000 fasttextsearch-0.8/textsearch/csrc/suffix_array.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3207 2023-08-04 14:21:28.000000 fasttextsearch-0.8/textsearch/csrc/suffix_array.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-08-04 14:21:28.000000 fasttextsearch-0.8/textsearch/csrc/suffix_array_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-08-04 14:21:28.000000 fasttextsearch-0.8/textsearch/csrc/utils.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-08-04 14:21:28.000000 fasttextsearch-0.8/textsearch/csrc/utils.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4862 2023-08-04 14:21:28.000000 fasttextsearch-0.8/textsearch/csrc/utils_test.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 14:25:14.842183 fasttextsearch-0.8/textsearch/python/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-04 14:21:28.000000 fasttextsearch-0.8/textsearch/python/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 14:25:14.842183 fasttextsearch-0.8/textsearch/python/csrc/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-08-04 14:21:28.000000 fasttextsearch-0.8/textsearch/python/csrc/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5003 2023-08-04 14:21:28.000000 fasttextsearch-0.8/textsearch/python/csrc/levenshtein.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-08-04 14:21:28.000000 fasttextsearch-0.8/textsearch/python/csrc/levenshtein.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-08-04 14:21:28.000000 fasttextsearch-0.8/textsearch/python/csrc/match.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-08-04 14:21:28.000000 fasttextsearch-0.8/textsearch/python/csrc/match.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-08-04 14:21:28.000000 fasttextsearch-0.8/textsearch/python/csrc/suffix_array.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-08-04 14:21:28.000000 fasttextsearch-0.8/textsearch/python/csrc/suffix_array.h
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-08-04 14:21:28.000000 fasttextsearch-0.8/textsearch/python/csrc/text_search.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-08-04 14:21:28.000000 fasttextsearch-0.8/textsearch/python/csrc/text_search.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4599 2023-08-04 14:21:28.000000 fasttextsearch-0.8/textsearch/python/csrc/utils.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-08-04 14:21:28.000000 fasttextsearch-0.8/textsearch/python/csrc/utils.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 14:25:14.842183 fasttextsearch-0.8/textsearch/python/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-08-04 14:21:28.000000 fasttextsearch-0.8/textsearch/python/tests/CMakeLists.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4748 2023-08-04 14:21:28.000000 fasttextsearch-0.8/textsearch/python/tests/test_find_close_matches.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1943 2023-08-04 14:21:28.000000 fasttextsearch-0.8/textsearch/python/tests/test_levenshtein_distance.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1414 2023-08-04 14:21:28.000000 fasttextsearch-0.8/textsearch/python/tests/test_match.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      950 2023-08-04 14:21:28.000000 fasttextsearch-0.8/textsearch/python/tests/test_row_ids_to_row_splits.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10687 2023-08-04 14:21:28.000000 fasttextsearch-0.8/textsearch/python/tests/test_sourced_text.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1359 2023-08-04 14:21:28.000000 fasttextsearch-0.8/textsearch/python/tests/test_suffix_array.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2007 2023-08-04 14:21:28.000000 fasttextsearch-0.8/textsearch/python/tests/test_text_source.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2314 2023-08-04 14:21:28.000000 fasttextsearch-0.8/textsearch/python/tests/test_transcript.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 14:25:14.846183 fasttextsearch-0.8/textsearch/python/textsearch/
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-08-04 14:25:14.000000 fasttextsearch-0.8/textsearch/python/textsearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13469 2023-08-04 14:21:28.000000 fasttextsearch-0.8/textsearch/python/textsearch/datatypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-08-04 14:21:28.000000 fasttextsearch-0.8/textsearch/python/textsearch/levenshtein.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53131 2023-08-04 14:21:28.000000 fasttextsearch-0.8/textsearch/python/textsearch/match.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-08-04 14:21:28.000000 fasttextsearch-0.8/textsearch/python/textsearch/suffix_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-08-04 14:21:28.000000 fasttextsearch-0.8/textsearch/python/textsearch/utils.py
```

### Comparing `fasttextsearch-0.7/CMakeLists.txt` & `fasttextsearch-0.8/CMakeLists.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 cmake_minimum_required(VERSION 3.12 FATAL_ERROR)
 project(textsearch)
 
-set(TS_VERSION "0.7")
+set(TS_VERSION "0.8")
 
 set(CMAKE_ARCHIVE_OUTPUT_DIRECTORY "${CMAKE_BINARY_DIR}/lib")
 set(CMAKE_LIBRARY_OUTPUT_DIRECTORY "${CMAKE_BINARY_DIR}/lib")
 set(CMAKE_RUNTIME_OUTPUT_DIRECTORY "${CMAKE_BINARY_DIR}/bin")
 
 set(CMAKE_SKIP_BUILD_RPATH FALSE)
 set(BUILD_RPATH_USE_ORIGIN TRUE)
```

### Comparing `fasttextsearch-0.7/PKG-INFO` & `fasttextsearch-0.8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fasttextsearch
-Version: 0.7
+Version: 0.8
 Summary: Some fast-ish algorithms for batch text search in moderate-sized collections, intended for data cleanup.
 Author-email: Next-gen Kaldi development team <wkang.pku@gmail.com>
 Project-URL: Homepage, https://github.com/k2-fsa/text_search
 Project-URL: Bug Tracker, https://github.com/k2-fsa/text_search/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `fasttextsearch-0.7/README.md` & `fasttextsearch-0.8/README.md`

 * *Files identical despite different names*

### Comparing `fasttextsearch-0.7/cmake/Modules/FetchContent/CMakeLists.cmake.in` & `fasttextsearch-0.8/cmake/Modules/FetchContent/CMakeLists.cmake.in`

 * *Files identical despite different names*

### Comparing `fasttextsearch-0.7/cmake/Modules/FetchContent.cmake` & `fasttextsearch-0.8/cmake/Modules/FetchContent.cmake`

 * *Files identical despite different names*

### Comparing `fasttextsearch-0.7/cmake/googletest.cmake` & `fasttextsearch-0.8/cmake/googletest.cmake`

 * *Files identical despite different names*

### Comparing `fasttextsearch-0.7/cmake/pybind11.cmake` & `fasttextsearch-0.8/cmake/pybind11.cmake`

 * *Files identical despite different names*

### Comparing `fasttextsearch-0.7/fasttextsearch.egg-info/PKG-INFO` & `fasttextsearch-0.8/fasttextsearch.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fasttextsearch
-Version: 0.7
+Version: 0.8
 Summary: Some fast-ish algorithms for batch text search in moderate-sized collections, intended for data cleanup.
 Author-email: Next-gen Kaldi development team <wkang.pku@gmail.com>
 Project-URL: Homepage, https://github.com/k2-fsa/text_search
 Project-URL: Bug Tracker, https://github.com/k2-fsa/text_search/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `fasttextsearch-0.7/fasttextsearch.egg-info/SOURCES.txt` & `fasttextsearch-0.8/fasttextsearch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fasttextsearch-0.7/pyproject.toml` & `fasttextsearch-0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     "cmake>=3.12",
 ]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "fasttextsearch"
-version = "0.7"
+version = "0.8"
 authors = [
   { name="Next-gen Kaldi development team", email="wkang.pku@gmail.com" },
 ]
 description="Some fast-ish algorithms for batch text search in moderate-sized collections, intended for data cleanup."
 dependencies = [
   "numpy",
   "regex",
@@ -29,10 +29,7 @@
 
 [project.urls]
 "Homepage" = "https://github.com/k2-fsa/text_search"
 "Bug Tracker" = "https://github.com/k2-fsa/text_search/issues"
 
 [tool.black]
 line-length = 80
-
-
-
```

### Comparing `fasttextsearch-0.7/setup.py` & `fasttextsearch-0.8/setup.py`

 * *Files identical despite different names*

### Comparing `fasttextsearch-0.7/textsearch/csrc/CMakeLists.txt` & `fasttextsearch-0.8/textsearch/csrc/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `fasttextsearch-0.7/textsearch/csrc/levenshtein.h` & `fasttextsearch-0.8/textsearch/csrc/levenshtein.h`

 * *Files identical despite different names*

### Comparing `fasttextsearch-0.7/textsearch/csrc/levenshtein_test.cc` & `fasttextsearch-0.8/textsearch/csrc/levenshtein_test.cc`

 * *Files identical despite different names*

### Comparing `fasttextsearch-0.7/textsearch/csrc/match.cc` & `fasttextsearch-0.8/textsearch/csrc/match.cc`

 * *Files identical despite different names*

### Comparing `fasttextsearch-0.7/textsearch/csrc/match.h` & `fasttextsearch-0.8/textsearch/csrc/match.h`

 * *Files identical despite different names*

### Comparing `fasttextsearch-0.7/textsearch/csrc/match_test.cc` & `fasttextsearch-0.8/textsearch/csrc/match_test.cc`

 * *Files identical despite different names*

### Comparing `fasttextsearch-0.7/textsearch/csrc/suffix_array.cc` & `fasttextsearch-0.8/textsearch/csrc/suffix_array.cc`

 * *Files identical despite different names*

### Comparing `fasttextsearch-0.7/textsearch/csrc/suffix_array.h` & `fasttextsearch-0.8/textsearch/csrc/suffix_array.h`

 * *Files identical despite different names*

### Comparing `fasttextsearch-0.7/textsearch/csrc/suffix_array_test.cc` & `fasttextsearch-0.8/textsearch/csrc/suffix_array_test.cc`

 * *Files identical despite different names*

### Comparing `fasttextsearch-0.7/textsearch/csrc/utils.cc` & `fasttextsearch-0.8/textsearch/csrc/utils.cc`

 * *Files identical despite different names*

### Comparing `fasttextsearch-0.7/textsearch/csrc/utils.h` & `fasttextsearch-0.8/textsearch/csrc/utils.h`

 * *Files identical despite different names*

### Comparing `fasttextsearch-0.7/textsearch/csrc/utils_test.cc` & `fasttextsearch-0.8/textsearch/csrc/utils_test.cc`

 * *Files identical despite different names*

### Comparing `fasttextsearch-0.7/textsearch/python/csrc/levenshtein.cc` & `fasttextsearch-0.8/textsearch/python/csrc/levenshtein.cc`

 * *Files identical despite different names*

### Comparing `fasttextsearch-0.7/textsearch/python/csrc/levenshtein.h` & `fasttextsearch-0.8/textsearch/python/csrc/levenshtein.h`

 * *Files identical despite different names*

### Comparing `fasttextsearch-0.7/textsearch/python/csrc/match.cc` & `fasttextsearch-0.8/textsearch/python/csrc/match.cc`

 * *Files identical despite different names*

### Comparing `fasttextsearch-0.7/textsearch/python/csrc/match.h` & `fasttextsearch-0.8/textsearch/python/csrc/match.h`

 * *Files identical despite different names*

### Comparing `fasttextsearch-0.7/textsearch/python/csrc/suffix_array.cc` & `fasttextsearch-0.8/textsearch/python/csrc/suffix_array.cc`

 * *Files identical despite different names*

### Comparing `fasttextsearch-0.7/textsearch/python/csrc/suffix_array.h` & `fasttextsearch-0.8/textsearch/python/csrc/suffix_array.h`

 * *Files identical despite different names*

### Comparing `fasttextsearch-0.7/textsearch/python/csrc/text_search.cc` & `fasttextsearch-0.8/textsearch/python/csrc/text_search.cc`

 * *Files identical despite different names*

### Comparing `fasttextsearch-0.7/textsearch/python/csrc/utils.cc` & `fasttextsearch-0.8/textsearch/python/csrc/utils.cc`

 * *Files identical despite different names*

### Comparing `fasttextsearch-0.7/textsearch/python/tests/CMakeLists.txt` & `fasttextsearch-0.8/textsearch/python/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `fasttextsearch-0.7/textsearch/python/tests/test_find_close_matches.py` & `fasttextsearch-0.8/textsearch/python/tests/test_find_close_matches.py`

 * *Files identical despite different names*

### Comparing `fasttextsearch-0.7/textsearch/python/tests/test_levenshtein_distance.py` & `fasttextsearch-0.8/textsearch/python/tests/test_levenshtein_distance.py`

 * *Files identical despite different names*

### Comparing `fasttextsearch-0.7/textsearch/python/tests/test_match.py` & `fasttextsearch-0.8/textsearch/python/tests/test_match.py`

 * *Files identical despite different names*

### Comparing `fasttextsearch-0.7/textsearch/python/tests/test_row_ids_to_row_splits.py` & `fasttextsearch-0.8/textsearch/python/tests/test_row_ids_to_row_splits.py`

 * *Files identical despite different names*

### Comparing `fasttextsearch-0.7/textsearch/python/tests/test_sourced_text.py` & `fasttextsearch-0.8/textsearch/python/tests/test_sourced_text.py`

 * *Files identical despite different names*

### Comparing `fasttextsearch-0.7/textsearch/python/tests/test_suffix_array.py` & `fasttextsearch-0.8/textsearch/python/tests/test_suffix_array.py`

 * *Files identical despite different names*

### Comparing `fasttextsearch-0.7/textsearch/python/tests/test_text_source.py` & `fasttextsearch-0.8/textsearch/python/tests/test_text_source.py`

 * *Files identical despite different names*

### Comparing `fasttextsearch-0.7/textsearch/python/tests/test_transcript.py` & `fasttextsearch-0.8/textsearch/python/tests/test_transcript.py`

 * *Files identical despite different names*

### Comparing `fasttextsearch-0.7/textsearch/python/textsearch/__init__.py` & `fasttextsearch-0.8/textsearch/python/textsearch/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,8 +17,8 @@
 
 from .suffix_array import create_suffix_array
 
 from .utils import AttributeDict
 from .utils import is_punctuation
 from .utils import row_ids_to_row_splits
 from .utils import str2bool
-__version__ = '0.7'
+__version__ = '0.8'
```

### Comparing `fasttextsearch-0.7/textsearch/python/textsearch/datatypes.py` & `fasttextsearch-0.8/textsearch/python/textsearch/datatypes.py`

 * *Files identical despite different names*

### Comparing `fasttextsearch-0.7/textsearch/python/textsearch/levenshtein.py` & `fasttextsearch-0.8/textsearch/python/textsearch/levenshtein.py`

 * *Files identical despite different names*

### Comparing `fasttextsearch-0.7/textsearch/python/textsearch/match.py` & `fasttextsearch-0.8/textsearch/python/textsearch/match.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,20 @@
 from _textsearch import (
     find_close_matches,
     get_longest_increasing_pairs as _get_longest_increasing_pairs,
     levenshtein_distance,
 )
 from .suffix_array import create_suffix_array
 from .datatypes import SourcedText, TextSource, Transcript
-from .utils import is_overlap, is_punctuation, row_ids_to_row_splits
+from .utils import (
+    PUCTUATIONS,
+    is_overlap,
+    is_punctuation,
+    row_ids_to_row_splits,
+)
 
 
 def get_longest_increasing_pairs(
     seq1: np.ndarray, seq2: np.ndarray
 ) -> List[Tuple[int, int]]:
     """
     Get the longest increasing pairs for given sequences.
@@ -237,15 +242,15 @@
             segments[-1] = (
                 segments[-1][0],
                 query_end,
                 segments[-1][2],
                 target_end,
             )
         else:
-            segments.append((query_start, query_end, target_start, target_end,))
+            segments.append((query_start, query_end, target_start, target_end))
     else:
         add_segments(
             query_start,
             query_end,
             target_start,
             target_end,
             segment_length,
@@ -678,15 +683,15 @@
     cumsum_error = [0] * len(aligns)
 
     # to avoid breaking at somethings like Mr. Mrs. etc.
     period_patterns = regex.compile(
         "(?<!Mr|Mrs|Dr|Ms|Prof|Pro|Capt|Gen|Sen|Rev|Hon|St)\."
     )
     # the largest length of the patterns.
-    period_pattern_length = 4
+    period_pattern_length = 5
 
     for i, align in enumerate(aligns):
         matched = align["ref"] == align["hyp"]
         cumsum_match[i] = (
             int(matched) if i == 0 else (cumsum_match[i - 1] + int(matched))
         )
         cumsum_error[i] = (
@@ -737,15 +742,18 @@
                     [
                         chr(x)
                         for x in target_source.binary_text[
                             j - period_pattern_length : j + 1
                         ]
                     ]
                 )
-                if period_patterns.search(tmp) is not None:
+                if current_token != "." or (
+                    current_token == "."
+                    and period_patterns.search(tmp) is not None
+                ):
                     prev_punctuation = punctuation_score
                     break
                 else:
                     j -= 1
             elif current_token == " " or is_punctuation(current_token):
                 j -= 1
             else:
@@ -760,15 +768,18 @@
                     [
                         chr(x)
                         for x in target_source.binary_text[
                             j - period_pattern_length : j + 1
                         ]
                     ]
                 )
-                if period_patterns.search(tmp) is not None:
+                if current_token != "." or (
+                    current_token == "."
+                    and period_patterns.search(tmp) is not None
+                ):
                     succ_punctuation = punctuation_score
                     break
                 else:
                     j += 1
             elif current_token == " " or is_punctuation(current_token):
                 j += 1
             else:
@@ -784,24 +795,24 @@
             succ_silence
             + succ_punctuation
             - errors_in_region / half_region_size
         )
 
         if target_source.has_punctuation:
             if prev_punctuation > 0 or i == 0:
-                begin_scores.append((i, begin_score,))
+                begin_scores.append((i, begin_score))
             if succ_punctuation > 0 or i == len(aligns) - 1:
-                end_scores.append((i, end_score,))
+                end_scores.append((i, end_score))
         else:
             if matched and (prev_silence >= silence_length_to_break or i == 0):
-                begin_scores.append((i, begin_score,))
+                begin_scores.append((i, begin_score))
             if matched and (
                 succ_silence >= silence_length_to_break or i == len(aligns) - 1
             ):
-                end_scores.append((i, end_score,))
+                end_scores.append((i, end_score))
 
     # (start, end, score)
     begin_list: List[Tuple[int, int, float]] = []
     end_list: List[Tuple[int, int, float]] = []
 
     init_duration_score = (
         base_score  # duration_score for segment between 5 ~ 20 seconds
@@ -871,15 +882,15 @@
                 else duration_score
             )
 
             heappush(
                 item_q,
                 (
                     point_score + matched_score - error_score + duration_score,
-                    (item[0], end_scores[ind][0],),
+                    (item[0], end_scores[ind][0]),
                 ),
             )
             if len(item_q) > num_of_best_position:
                 heappop(item_q)
             ind += 1
         while item_q:
             x = heappop(item_q)
@@ -952,15 +963,15 @@
                 else duration_score
             )
 
             heappush(
                 item_q,
                 (
                     point_score + matched_score - error_score + duration_score,
-                    (begin_scores[ind][0], item[0],),
+                    (begin_scores[ind][0], item[0]),
                 ),
             )
             if len(item_q) > num_of_best_position:
                 heappop(item_q)
             ind -= 1
         while item_q:
             x = heappop(item_q)
@@ -1076,15 +1087,31 @@
         ):
             segments.append(r)
 
     results = []
 
     for seg in segments:
         begin_pos = aligns[seg[0]]["ref_pos"]
-        end_pos = aligns[seg[1]]["ref_pos"] + 1
+        while begin_pos >= 1:
+            current_token = chr(target_source.binary_text[begin_pos - 1])
+            if current_token in PUCTUATIONS["left"]:
+                begin_pos -= 1
+            else:
+                break
+
+        end_pos = aligns[seg[1]]["ref_pos"]
+        while end_pos + 1 < target_source.binary_text.size:
+            current_token = chr(target_source.binary_text[end_pos + 1])
+            if (
+                current_token in PUCTUATIONS["right"]
+                or current_token in PUCTUATIONS["eos"]
+            ):
+                end_pos += 1
+            else:
+                break
 
         preceding_index = seg[0] if seg[0] == 0 else seg[0] - 1
         succeeding_index = seg[1] if seg[1] == len(aligns) - 1 else seg[1] + 1
 
         if timestamp_position == "middle":
             start_time = (
                 aligns[preceding_index]["hyp_time"] + aligns[seg[0]]["hyp_time"]
@@ -1101,19 +1128,21 @@
                 timestamp_position,
                 "current",
             )
             start_time = aligns[seg[0]]["hyp_time"]
             end_time = aligns[succeeding_index]["hyp_time"]
 
         hyp_begin_pos = aligns[seg[0]]["hyp_pos"]
-        hyp_end_pos = aligns[seg[1]]["hyp_pos"] + 1
+        hyp_end_pos = aligns[seg[1]]["hyp_pos"]
         hyp = "".join(
             [
                 chr(i)
-                for i in query_source.binary_text[hyp_begin_pos:hyp_end_pos]
+                for i in query_source.binary_text[
+                    hyp_begin_pos : hyp_end_pos + 1
+                ]
             ]
         )
 
         # output one more token for reference to include the possible punctuation.
         # end_pos plus 1 here is safe, it is probably a space or punctuation.
         ref = "".join(
             [chr(i) for i in target_source.binary_text[begin_pos : end_pos + 1]]
@@ -1127,15 +1156,15 @@
         preceding_ref = "".join(
             [chr(i) for i in target_source.binary_text[preceding_pos:begin_pos]]
         )
         succeeding_ref = "".join(
             [
                 chr(i)
                 for i in target_source.binary_text[
-                    end_pos : end_pos + preceding_context_length
+                    end_pos + 1 : end_pos + preceding_context_length
                 ]
             ]
         )
 
         preceding_pos = (
             hyp_begin_pos - preceding_context_length
             if hyp_begin_pos - preceding_context_length > 0
@@ -1147,15 +1176,15 @@
                 for i in query_source.binary_text[preceding_pos:hyp_begin_pos]
             ]
         )
         succeeding_hyp = "".join(
             [
                 chr(i)
                 for i in query_source.binary_text[
-                    hyp_end_pos : hyp_begin_pos + preceding_context_length
+                    hyp_end_pos + 1 : hyp_begin_pos + preceding_context_length
                 ]
             ]
         )
 
         results.append(
             {
                 "begin_byte": begin_pos,
```

### Comparing `fasttextsearch-0.7/textsearch/python/textsearch/suffix_array.py` & `fasttextsearch-0.8/textsearch/python/textsearch/suffix_array.py`

 * *Files identical despite different names*

### Comparing `fasttextsearch-0.7/textsearch/python/textsearch/utils.py` & `fasttextsearch-0.8/textsearch/python/textsearch/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,14 +5,21 @@
 from datetime import datetime
 from pathlib import Path
 import numpy as np
 from _textsearch import row_ids_to_row_splits as _row_ids_to_row_splits
 
 Pathlike = Union[str, Path]
 
+PUCTUATIONS = {
+    "all": set("',.;?!():-<>/\"，。；？！（）：-《》【】”“"),
+    "eos": set(".?!。？！"),
+    "left": set("\"'(<《【“"),
+    "right": set("\"')>》】”"),
+}
+
 
 class AttributeDict(dict):
     def __getattr__(self, key):
         if key in self:
             return self[key]
         raise AttributeError(f"No such attribute '{key}'")
 
@@ -157,16 +164,16 @@
     Args:
       c:
         The given character.
       eos_only:
         If True the punctuations are only those indicating end of a sentence (.?! for now).
     """
     if eos_only:
-        return c in ".?!"
-    return c in ',.;?!():-<>-/"'
+        return c in PUCTUATIONS["eos"]
+    return c in PUCTUATIONS["all"]
 
 
 def str2bool(v):
     """Used in argparse.ArgumentParser.add_argument to indicate
     that a type is a bool type and user can enter
 
         - yes, true, t, y, 1, to represent True
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

