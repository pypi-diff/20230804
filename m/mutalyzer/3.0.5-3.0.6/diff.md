# Comparing `tmp/mutalyzer-3.0.5.tar.gz` & `tmp/mutalyzer-3.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mutalyzer-3.0.5.tar", last modified: Tue Jan 31 18:27:47 2023, max compression
+gzip compressed data, was "/home/mihai/projects/mutalyzer/mutalyzer/dist/.tmp-uaaso1ks/mutalyzer-3.0.6.tar", last modified: Fri Aug  4 08:14:51 2023, max compression
```

## Comparing `mutalyzer-3.0.5.tar` & `mutalyzer-3.0.6.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2023-01-31 18:27:47.719730 mutalyzer-3.0.5/
--rw-r--r--   0 mihai     (1000) mihai     (1000)     1089 2019-05-28 09:25:15.000000 mutalyzer-3.0.5/LICENSE
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     1836 2023-01-31 18:27:47.719730 mutalyzer-3.0.5/PKG-INFO
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     1280 2023-01-31 14:43:31.000000 mutalyzer-3.0.5/README.rst
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2023-01-31 18:27:47.707730 mutalyzer-3.0.5/mutalyzer/
--rw-r--r--   0 mihai     (1000) mihai     (1000)      712 2021-11-15 13:20:06.000000 mutalyzer-3.0.5/mutalyzer/__init__.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)    10792 2023-01-31 14:43:31.000000 mutalyzer-3.0.5/mutalyzer/algebra.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      866 2023-01-31 14:43:31.000000 mutalyzer-3.0.5/mutalyzer/back_translator.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     5230 2023-01-31 14:43:31.000000 mutalyzer-3.0.5/mutalyzer/checker.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      764 2023-01-31 14:43:31.000000 mutalyzer-3.0.5/mutalyzer/cli.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2023-01-31 18:27:47.711730 mutalyzer-3.0.5/mutalyzer/converter/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      124 2021-09-01 09:19:06.000000 mutalyzer-3.0.5/mutalyzer/converter/__init__.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     5413 2023-01-31 14:43:31.000000 mutalyzer-3.0.5/mutalyzer/converter/extras.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     3597 2022-11-18 18:19:33.000000 mutalyzer-3.0.5/mutalyzer/converter/to_delins.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     7368 2023-01-31 14:43:31.000000 mutalyzer-3.0.5/mutalyzer/converter/to_hgvs_coordinates.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     2473 2021-02-19 19:28:53.000000 mutalyzer-3.0.5/mutalyzer/converter/to_hgvs_indexing.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     6349 2023-01-26 14:33:09.000000 mutalyzer-3.0.5/mutalyzer/converter/to_internal_coordinates.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     3332 2021-02-05 09:58:08.000000 mutalyzer-3.0.5/mutalyzer/converter/to_internal_indexing.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)    15522 2023-01-31 14:43:31.000000 mutalyzer-3.0.5/mutalyzer/converter/to_rna.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     9654 2023-01-31 14:43:31.000000 mutalyzer-3.0.5/mutalyzer/converter/variants_de_to_hgvs.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)    68838 2023-01-31 14:43:31.000000 mutalyzer-3.0.5/mutalyzer/description.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      836 2021-02-05 09:58:08.000000 mutalyzer-3.0.5/mutalyzer/description_extractor.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)    15475 2022-05-03 13:04:25.000000 mutalyzer-3.0.5/mutalyzer/description_model.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     9207 2023-01-31 14:43:31.000000 mutalyzer-3.0.5/mutalyzer/errors.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     4802 2023-01-31 14:43:31.000000 mutalyzer-3.0.5/mutalyzer/infos.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     7706 2023-01-31 14:43:31.000000 mutalyzer-3.0.5/mutalyzer/mapper.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     1100 2021-11-02 14:43:09.000000 mutalyzer-3.0.5/mutalyzer/mutator.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      820 2023-01-31 17:55:37.000000 mutalyzer-3.0.5/mutalyzer/normalizer.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     7553 2022-09-06 09:52:56.000000 mutalyzer-3.0.5/mutalyzer/position_converter.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)    12797 2022-12-15 14:41:24.000000 mutalyzer-3.0.5/mutalyzer/protein.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)    16919 2023-01-31 14:43:31.000000 mutalyzer-3.0.5/mutalyzer/reference.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     1537 2022-05-10 13:52:20.000000 mutalyzer-3.0.5/mutalyzer/spdi_converter.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     8704 2023-01-31 14:43:31.000000 mutalyzer-3.0.5/mutalyzer/util.py
--rw-r--r--   0 mihai     (1000) mihai     (1000)     2913 2021-02-02 21:13:48.000000 mutalyzer-3.0.5/mutalyzer/validation.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     3731 2022-11-21 09:50:19.000000 mutalyzer-3.0.5/mutalyzer/viewer.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2023-01-31 18:27:47.711730 mutalyzer-3.0.5/mutalyzer.egg-info/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     1836 2023-01-31 18:27:47.000000 mutalyzer-3.0.5/mutalyzer.egg-info/PKG-INFO
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     1481 2023-01-31 18:27:47.000000 mutalyzer-3.0.5/mutalyzer.egg-info/SOURCES.txt
--rw-rw-r--   0 mihai     (1000) mihai     (1000)        1 2023-01-31 18:27:47.000000 mutalyzer-3.0.5/mutalyzer.egg-info/dependency_links.txt
--rw-rw-r--   0 mihai     (1000) mihai     (1000)       60 2023-01-31 18:27:47.000000 mutalyzer-3.0.5/mutalyzer.egg-info/entry_points.txt
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      224 2023-01-31 18:27:47.000000 mutalyzer-3.0.5/mutalyzer.egg-info/requires.txt
--rw-rw-r--   0 mihai     (1000) mihai     (1000)       16 2023-01-31 18:27:47.000000 mutalyzer-3.0.5/mutalyzer.egg-info/top_level.txt
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     1277 2023-01-31 18:27:47.719730 mutalyzer-3.0.5/setup.cfg
--rw-r--r--   0 mihai     (1000) mihai     (1000)       38 2020-08-10 08:33:28.000000 mutalyzer-3.0.5/setup.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2023-01-31 18:27:47.719730 mutalyzer-3.0.5/tests/
--rw-r--r--   0 mihai     (1000) mihai     (1000)        0 2019-05-28 09:25:15.000000 mutalyzer-3.0.5/tests/__init__.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     1293 2022-05-10 13:33:48.000000 mutalyzer-3.0.5/tests/commons.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      164 2021-04-23 07:40:34.000000 mutalyzer-3.0.5/tests/conftest.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     1735 2023-01-31 14:43:31.000000 mutalyzer-3.0.5/tests/generator.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)    29065 2023-01-31 14:43:21.000000 mutalyzer-3.0.5/tests/test_algebra.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     1424 2023-01-31 14:43:31.000000 mutalyzer-3.0.5/tests/test_back_translator.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     4948 2022-10-11 07:28:20.000000 mutalyzer-3.0.5/tests/test_checker.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)    18582 2021-11-12 09:37:02.000000 mutalyzer-3.0.5/tests/test_converter.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     1638 2023-01-31 14:43:31.000000 mutalyzer-3.0.5/tests/test_description.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     1681 2022-10-11 07:28:20.000000 mutalyzer-3.0.5/tests/test_ensembl.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     7851 2023-01-31 14:43:31.000000 mutalyzer-3.0.5/tests/test_mapper.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     4081 2023-01-31 14:43:31.000000 mutalyzer-3.0.5/tests/test_normalizer.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     5545 2021-11-12 09:37:24.000000 mutalyzer-3.0.5/tests/test_position_convert.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     4149 2023-01-31 14:43:31.000000 mutalyzer-3.0.5/tests/test_protein.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)    25073 2023-01-31 14:43:31.000000 mutalyzer-3.0.5/tests/test_reference.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)    56805 2022-10-11 07:28:20.000000 mutalyzer-3.0.5/tests/test_rna.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     5142 2021-11-12 09:37:39.000000 mutalyzer-3.0.5/tests/test_to_description.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     1288 2022-05-05 15:44:03.000000 mutalyzer-3.0.5/tests/test_viewer.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)   113916 2023-01-31 14:43:31.000000 mutalyzer-3.0.5/tests/variants_set.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2023-08-04 08:14:51.706863 mutalyzer-3.0.6/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     1089 2021-12-22 14:45:14.000000 mutalyzer-3.0.6/LICENSE
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     1836 2023-08-04 08:14:51.706863 mutalyzer-3.0.6/PKG-INFO
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     1280 2023-01-10 12:35:42.000000 mutalyzer-3.0.6/README.rst
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2023-08-04 08:14:51.702863 mutalyzer-3.0.6/mutalyzer/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      712 2021-12-22 14:45:14.000000 mutalyzer-3.0.6/mutalyzer/__init__.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)    11709 2023-08-04 07:55:37.000000 mutalyzer-3.0.6/mutalyzer/algebra.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      866 2023-07-31 11:44:51.000000 mutalyzer-3.0.6/mutalyzer/back_translator.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     5230 2023-01-10 12:35:42.000000 mutalyzer-3.0.6/mutalyzer/checker.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      764 2023-01-10 12:35:42.000000 mutalyzer-3.0.6/mutalyzer/cli.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2023-08-04 08:14:51.702863 mutalyzer-3.0.6/mutalyzer/converter/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      124 2021-12-22 14:45:14.000000 mutalyzer-3.0.6/mutalyzer/converter/__init__.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     5170 2023-08-04 07:55:37.000000 mutalyzer-3.0.6/mutalyzer/converter/extras.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     3597 2022-06-04 07:38:47.000000 mutalyzer-3.0.6/mutalyzer/converter/to_delins.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     7130 2023-08-04 07:55:37.000000 mutalyzer-3.0.6/mutalyzer/converter/to_hgvs_coordinates.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     2473 2021-12-22 14:45:14.000000 mutalyzer-3.0.6/mutalyzer/converter/to_hgvs_indexing.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     6660 2023-08-04 07:55:37.000000 mutalyzer-3.0.6/mutalyzer/converter/to_internal_coordinates.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     3332 2021-12-22 14:45:14.000000 mutalyzer-3.0.6/mutalyzer/converter/to_internal_indexing.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)    15678 2023-08-04 07:55:37.000000 mutalyzer-3.0.6/mutalyzer/converter/to_rna.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     9826 2023-08-04 07:55:37.000000 mutalyzer-3.0.6/mutalyzer/converter/variants_de_to_hgvs.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)    68444 2023-08-04 07:55:37.000000 mutalyzer-3.0.6/mutalyzer/description.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      836 2021-12-22 14:45:14.000000 mutalyzer-3.0.6/mutalyzer/description_extractor.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)    15475 2022-06-04 07:38:47.000000 mutalyzer-3.0.6/mutalyzer/description_model.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     9534 2023-08-04 07:55:37.000000 mutalyzer-3.0.6/mutalyzer/errors.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     5051 2023-08-04 07:55:37.000000 mutalyzer-3.0.6/mutalyzer/infos.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     7706 2023-07-31 11:44:51.000000 mutalyzer-3.0.6/mutalyzer/mapper.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     1100 2021-12-22 14:45:14.000000 mutalyzer-3.0.6/mutalyzer/mutator.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     1209 2023-08-04 07:55:37.000000 mutalyzer-3.0.6/mutalyzer/normalizer.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     7553 2022-09-14 09:23:45.000000 mutalyzer-3.0.6/mutalyzer/position_converter.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)    12797 2023-01-10 12:35:42.000000 mutalyzer-3.0.6/mutalyzer/protein.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)    16919 2023-07-31 11:44:51.000000 mutalyzer-3.0.6/mutalyzer/reference.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     1537 2022-06-04 07:38:47.000000 mutalyzer-3.0.6/mutalyzer/spdi_converter.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     8704 2023-07-31 11:44:51.000000 mutalyzer-3.0.6/mutalyzer/util.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     2913 2021-12-22 14:45:14.000000 mutalyzer-3.0.6/mutalyzer/validation.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     3791 2023-08-04 07:55:37.000000 mutalyzer-3.0.6/mutalyzer/viewer.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2023-08-04 08:14:51.702863 mutalyzer-3.0.6/mutalyzer.egg-info/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     1836 2023-08-04 08:14:51.000000 mutalyzer-3.0.6/mutalyzer.egg-info/PKG-INFO
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     1481 2023-08-04 08:14:51.000000 mutalyzer-3.0.6/mutalyzer.egg-info/SOURCES.txt
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)        1 2023-08-04 08:14:51.000000 mutalyzer-3.0.6/mutalyzer.egg-info/dependency_links.txt
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)       60 2023-08-04 08:14:51.000000 mutalyzer-3.0.6/mutalyzer.egg-info/entry_points.txt
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      224 2023-08-04 08:14:51.000000 mutalyzer-3.0.6/mutalyzer.egg-info/requires.txt
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)       16 2023-08-04 08:14:51.000000 mutalyzer-3.0.6/mutalyzer.egg-info/top_level.txt
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     1277 2023-08-04 08:14:51.706863 mutalyzer-3.0.6/setup.cfg
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)       38 2021-12-22 14:45:14.000000 mutalyzer-3.0.6/setup.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2023-08-04 08:14:51.706863 mutalyzer-3.0.6/tests/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)        0 2021-12-22 14:45:14.000000 mutalyzer-3.0.6/tests/__init__.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     1462 2023-08-04 07:55:37.000000 mutalyzer-3.0.6/tests/commons.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      164 2021-12-22 14:45:14.000000 mutalyzer-3.0.6/tests/conftest.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     1735 2023-07-31 11:44:51.000000 mutalyzer-3.0.6/tests/generator.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)    31762 2023-08-04 07:55:37.000000 mutalyzer-3.0.6/tests/test_algebra.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     1423 2023-08-04 07:55:37.000000 mutalyzer-3.0.6/tests/test_back_translator.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     4947 2023-08-04 07:55:37.000000 mutalyzer-3.0.6/tests/test_checker.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)    18582 2021-12-22 14:45:14.000000 mutalyzer-3.0.6/tests/test_converter.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     1638 2023-01-10 12:35:42.000000 mutalyzer-3.0.6/tests/test_description.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     1680 2023-08-04 07:55:37.000000 mutalyzer-3.0.6/tests/test_ensembl.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     8119 2023-08-04 07:55:37.000000 mutalyzer-3.0.6/tests/test_mapper.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     4670 2023-08-04 07:55:37.000000 mutalyzer-3.0.6/tests/test_normalizer.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     5544 2023-08-04 07:55:37.000000 mutalyzer-3.0.6/tests/test_position_convert.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     4378 2023-08-04 07:55:37.000000 mutalyzer-3.0.6/tests/test_protein.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)    25072 2023-08-04 07:55:37.000000 mutalyzer-3.0.6/tests/test_reference.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)    45771 2023-08-04 07:55:37.000000 mutalyzer-3.0.6/tests/test_rna.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     5142 2021-12-22 14:45:14.000000 mutalyzer-3.0.6/tests/test_to_description.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     1287 2023-08-04 07:55:37.000000 mutalyzer-3.0.6/tests/test_viewer.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)   118571 2023-08-04 07:55:37.000000 mutalyzer-3.0.6/tests/variants_set.py
```

### Comparing `mutalyzer-3.0.5/LICENSE` & `mutalyzer-3.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mutalyzer-3.0.5/PKG-INFO` & `mutalyzer-3.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mutalyzer
-Version: 3.0.5
+Version: 3.0.6
 Summary: Mutalyzer HGVS variant description tools.
 Home-page: https://github.com/mutalyzer/mutalyzer
 Author: Mihai Lefter
 Author-email: M.Lefter@lumc.nl
 License: MIT
 Keywords: Mutalyzer,HGVS
 Classifier: Intended Audience :: Science/Research
```

### Comparing `mutalyzer-3.0.5/README.rst` & `mutalyzer-3.0.6/README.rst`

 * *Files identical despite different names*

### Comparing `mutalyzer-3.0.5/mutalyzer/__init__.py` & `mutalyzer-3.0.6/mutalyzer/__init__.py`

 * *Files identical despite different names*

### Comparing `mutalyzer-3.0.5/mutalyzer/algebra.py` & `mutalyzer-3.0.6/mutalyzer/algebra.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,14 +41,15 @@
     output = {"input": reference_id, "type": "id", "reference": {"id": reference_id}}
     reference_model = retrieve_reference(reference_id)[0]
     # TODO: update the reference id if different in the model?
     if reference_model is None:
         output["errors"] = [errors.reference_not_retrieved(reference_id, [])]
     else:
         output["sequence"] = reference_model["sequence"]["seq"]
+        output["annotations"] = {"id": reference_model["annotations"]["id"]}
     return output
 
 
 def _get_sequence(seq):
     return {
         "input": seq,
         "type": "sequence",
@@ -230,28 +231,45 @@
 
     if output:
         return output
 
     lhs_observed = lhs_d.get_sequences()["observed"]
     lhs_algebra_variants = _get_algebra_variants(lhs_d)
     lhs_spanning = spanning_variant(lhs_reference, lhs_observed, lhs_algebra_variants)
-    lhs_supremal = find_supremal(lhs_reference, lhs_spanning)
+    lhs_supremal, *_ = find_supremal(lhs_reference, lhs_spanning)
 
     rhs_observed = rhs_d.get_sequences()["observed"]
     rhs_algebra_variants = _get_algebra_variants(rhs_d)
     rhs_spanning = spanning_variant(rhs_reference, rhs_observed, rhs_algebra_variants)
-    rhs_supremal = find_supremal(rhs_reference, rhs_spanning)
+    rhs_supremal, *_ = find_supremal(rhs_reference, rhs_spanning)
 
     output["relation"] = compare_supremal(
         lhs_reference, lhs_supremal, rhs_supremal
     ).value
 
     output["influence_lhs"] = _influence_interval_supremal(lhs_supremal)
     output["influence_rhs"] = _influence_interval_supremal(rhs_supremal)
 
+    if lhs_d.corrected_model.get("reference"):
+        ref_id = lhs_d.corrected_model['reference']['id']
+    elif lhs_d.references["reference"].get("annotations") and lhs_d.references["reference"]["annotations"].get("id"):
+        ref_id = lhs_d.references["reference"]["annotations"]["id"]
+    else:
+        ref_id = rhs_reference
+
+    output["supremal_lhs"] = {
+        "hgvs": f"{ref_id}:g.{lhs_supremal.to_hgvs()}",
+        "spdi": lhs_supremal.to_spdi(ref_id)
+    }
+
+    output["supremal_rhs"] = {
+        "hgvs": f"{ref_id}:g.{rhs_supremal.to_hgvs()}",
+        "spdi": rhs_supremal.to_spdi(ref_id)
+    }
+
     output["view_lhs"] = view_variants_normalized(lhs_d)
     output["view_rhs"] = view_variants_normalized(rhs_d)
 
     return output
 
 
 def compare_sequences_based(reference, reference_type, lhs, lhs_type, rhs, rhs_type):
@@ -313,29 +331,33 @@
                 sequence=lhs_d.get_sequences()["reference"],
             )
             rhs_d.normalize()
         else:
             return
     elif lhs_type == "variant" and rhs_type == "variant":
         if reference_type == "sequence":
-            reference_sequence = "reference"
+            reference_sequence = reference
+            ref_id = reference
         elif reference_type == "id":
             check = _get_id(reference)
             if check.get("errors"):
                 return check
             else:
                 reference_sequence = check["sequence"]
+                ref_id = check["annotations"]["id"]
         lhs_d = Description(
             description=lhs, only_variants=True, sequence=reference_sequence
         )
         lhs_d.normalize()
+        lhs_d.references["reference"]["annotations"] = {"id": ref_id}
         rhs_d = Description(
             description=rhs, only_variants=True, sequence=reference_sequence
         )
         rhs_d.normalize()
+        rhs_d.references["reference"]["annotations"] = {"id": ref_id}
     return compare_hgvs(lhs_d, rhs_d)
 
 
 def compare(reference, reference_type, lhs, lhs_type, rhs, rhs_type):
     checks = _input_types_check(reference_type, lhs_type, rhs_type)
 
     if checks:
```

### Comparing `mutalyzer-3.0.5/mutalyzer/back_translator.py` & `mutalyzer-3.0.6/mutalyzer/back_translator.py`

 * *Files identical despite different names*

### Comparing `mutalyzer-3.0.5/mutalyzer/checker.py` & `mutalyzer-3.0.6/mutalyzer/checker.py`

 * *Files identical despite different names*

### Comparing `mutalyzer-3.0.5/mutalyzer/cli.py` & `mutalyzer-3.0.6/mutalyzer/cli.py`

 * *Files identical despite different names*

### Comparing `mutalyzer-3.0.5/mutalyzer/converter/extras.py` & `mutalyzer-3.0.6/mutalyzer/converter/extras.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,22 +140,17 @@
     ref_seq = reference_model["sequence"]["seq"]
     s_model = get_internal_selector_model(new_r_model["annotations"], selector_id, True)
 
     if slice_to == "transcript":
         ref_seq = slice_seq(ref_seq, s_model["exon"])
         new_r_model["sequence"] = {"seq": ref_seq}
         x = NonCoding(s_model["exon"]).coordinate_to_noncoding
-        exon_end = [exon[1] for exon in s_model["exon"]]
     if slice_to == "gene":
         g_l = get_gene_locations(new_r_model)
         ref_seq = slice_seq(ref_seq, [g_l])
         new_r_model["sequence"] = {"seq": ref_seq}
         x = NonCoding([g_l]).coordinate_to_noncoding
-        exon_end = [g_l[1]]
 
     for loc, feature_type in yield_locations_selector_id(new_r_model, selector_id):
         loc["start"]["position"] = x(loc["start"]["position"])[0] - 1
-        if feature_type == "exon" and loc["end"]["position"] in exon_end:
-            loc["end"]["position"] = x(loc["end"]["position"])[0]
-        else:
-            loc["end"]["position"] = x(loc["end"]["position"])[0] - 1
+        loc["end"]["position"] = x(loc["end"]["position"] - 1)[0]
     return new_r_model
```

### Comparing `mutalyzer-3.0.5/mutalyzer/converter/to_delins.py` & `mutalyzer-3.0.6/mutalyzer/converter/to_delins.py`

 * *Files identical despite different names*

### Comparing `mutalyzer-3.0.5/mutalyzer/converter/to_hgvs_coordinates.py` & `mutalyzer-3.0.6/mutalyzer/converter/to_hgvs_coordinates.py`

 * *Files 2% similar despite different names*

```diff
@@ -125,36 +125,26 @@
             variant["inserted"].reverse()
             shift = variant["location"]["start"].get("shift", 0)
             if shift and len(variant["inserted"]) > 1:
                 variant["inserted"].reverse()
                 ins_seq = construct_sequence(variant["inserted"], sequences)
                 seq = sequences["reference"]
                 start = get_start(variant)
-                new_ins_seq = reverse_complement(
-                    (seq[start - shift : start] + ins_seq)[: len(ins_seq)]
-                )
-                variant["inserted"] = [
-                    {"sequence": new_ins_seq, "source": "description"}
-                ]
+                new_ins_seq = reverse_complement((seq[start - shift : start] + ins_seq)[: len(ins_seq)])
+                variant["inserted"] = [{"sequence": new_ins_seq, "source": "description"}]
             else:
                 seq = sequences["reference"]
                 for inserted in variant["inserted"]:
                     if inserted.get("sequence"):
                         start = get_start(variant)
                         ins_seq = inserted["sequence"]
-                        inserted["sequence"] = reverse_complement(
-                            (seq[start - shift : start] + ins_seq)[: len(ins_seq)]
-                        )
+                        inserted["sequence"] = reverse_complement((seq[start - shift : start] + ins_seq)[: len(ins_seq)])
                     else:
-                        inserted["location"]["start"]["position"] -= inserted[
-                            "location"
-                        ]["start"].get("shift", 0)
-                        inserted["location"]["end"]["position"] -= inserted["location"][
-                            "start"
-                        ].get("shift", 0)
+                        inserted["location"]["start"]["position"] -= inserted["location"]["start"].get("shift", 0)
+                        inserted["location"]["end"]["position"] -= inserted["location"]["start"].get("shift", 0)
         if variant.get("deleted"):
             variant["deleted"].reverse()
             for deleted in variant["deleted"]:
                 if deleted.get("sequence"):
                     deleted["sequence"] = reverse_complement(deleted["sequence"])
```

### Comparing `mutalyzer-3.0.5/mutalyzer/converter/to_hgvs_indexing.py` & `mutalyzer-3.0.6/mutalyzer/converter/to_hgvs_indexing.py`

 * *Files identical despite different names*

### Comparing `mutalyzer-3.0.5/mutalyzer/converter/to_internal_coordinates.py` & `mutalyzer-3.0.6/mutalyzer/converter/to_internal_coordinates.py`

 * *Files 6% similar despite different names*

```diff
@@ -156,14 +156,20 @@
 
     internal_model = initialize_internal_model(model)
     crossmap = crossmap_to_internal_setup(coordinate_system, selector_model)
 
     for point, path in yield_point_locations_for_main_reference(model):
         set_by_path(internal_model, path, point_to_internal(point, crossmap))
 
+    if selector_model and selector_model.get("inverted"):
+        if internal_model.get("location") and internal_model.get("location").get("type") == "range":
+            loc = internal_model["location"]
+            loc["start"], loc["end"] = loc["end"], loc["start"]
+        internal_model["inverted"] = True
+
     return internal_model
 
 
 def to_internal_coordinates(model, references):
     """
 
     :param model: Description model.
```

### Comparing `mutalyzer-3.0.5/mutalyzer/converter/to_internal_indexing.py` & `mutalyzer-3.0.6/mutalyzer/converter/to_internal_indexing.py`

 * *Files identical despite different names*

### Comparing `mutalyzer-3.0.5/mutalyzer/converter/to_rna.py` & `mutalyzer-3.0.6/mutalyzer/converter/to_rna.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,24 +51,29 @@
             ).lower()
             if transcribe
             else slice_to_selector(reference_model, selector_id)
         },
     }
     s_m = get_internal_selector_model(rna_model["annotations"], selector_id, True)
     x = NonCoding(s_m["exon"]).coordinate_to_noncoding
+    g = Genomic().genomic_to_coordinate
 
     new_start = x(s_m["exon"][0][0])[0] - 1
     new_end = x(s_m["exon"][-1][-1])[0]
+
     for location, f_type in yield_locations(rna_model["annotations"]):
-        if f_type == "CDS":
-            set_start(location, x(get_start(location))[0] - 1)
-            set_end(location, x(get_end(location))[0] - 1)
-        elif f_type == "exon":
-            set_start(location, x(get_start(location))[0] - 1)
-            set_end(location, x(get_end(location))[0] + x(get_end(location))[1] - 1)
+        if f_type in ["CDS", "exon"]:
+            new_start_x = x(get_start(location))
+            new_start_g = g(new_start_x[0])
+
+            new_end_x = x(get_end(location))
+            new_end_g = g(new_end_x[0] + new_end_x[1])
+
+            set_start(location, new_start_g)
+            set_end(location, new_end_g)
         else:
             set_start(location, new_start)
             set_end(location, new_end)
     return rna_model
 
 
 def get_position_type(position, exons, len_ss=2, len_as=5):
@@ -233,21 +238,18 @@
     :arg dict selector_model: Selector model.
     :returns: Converted RNA variants.
     :rtype: dict
     """
     trimmed_variants = _trim_to_exons(variants, selector_model["exon"], sequences)
 
     x = NonCoding(selector_model["exon"]).coordinate_to_noncoding
-
     for variant in trimmed_variants:
         if variant.get("location"):
             set_start(variant["location"], x(get_start(variant))[0] - 1)
-            set_end(
-                variant["location"], x(get_end(variant))[0] + x(get_end(variant))[1] - 1
-            )
+            set_end(variant["location"], x(get_end(variant))[0] + x(get_end(variant))[1] - 1)
             if variant.get("inserted"):
                 variant["inserted"] = [
                     {
                         "source": "description",
                         "sequence": get_inserted_sequence(variant, sequences),
                     }
                 ]
@@ -330,16 +332,18 @@
 
 
 def reverse_start_end(variants):
     for variant in variants:
         if variant.get("location") and variant["location"]["type"] == "range":
             location = variant["location"]
             location["start"], location["end"] = location["end"], location["start"]
-            location["start"]["position"] -= 1
-            location["end"]["position"] -= 1
+            location["start"]["position"] -= 1 + location["start"].get("shift", 0)
+            location["end"]["position"] -= 1 + location["start"].get("shift", 0)
+            location["start"]["shift"] = 0
+            location["end"]["shift"] = 0
 
 
 def _get_cds_into_exons(exons, cds):
     l_index = bisect.bisect_right(exons, cds[0])
     r_index = bisect.bisect_left(exons, cds[1])
     return [cds[0]] + exons[l_index:r_index] + [cds[1]]
```

### Comparing `mutalyzer-3.0.5/mutalyzer/converter/variants_de_to_hgvs.py` & `mutalyzer-3.0.6/mutalyzer/converter/variants_de_to_hgvs.py`

 * *Files 2% similar despite different names*

```diff
@@ -142,15 +142,18 @@
     return False
 
 
 def inserted_to_hgvs(inserted):
     new_inserted = []
     for insert in inserted:
         if insert["source"] in ["reference"]:
-            new_inserted.append({"source": "reference", "location": insert["location"]})
+            if insert.get("inverted"):
+                new_inserted.append({"source": "reference", "location": insert["location"], "inverted": True})
+            else:
+                new_inserted.append({"source": "reference", "location": insert["location"]})
         else:
             new_inserted.append(
                 {"source": "description", "sequence": insert["sequence"]}
             )
     return new_inserted
```

### Comparing `mutalyzer-3.0.5/mutalyzer/description.py` & `mutalyzer-3.0.6/mutalyzer/description.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import itertools
 
 from Bio.Seq import Seq
 from Bio.SeqUtils import seq1, seq3
 from extractor import describe_dna
 from mutalyzer_backtranslate import BackTranslate
 from mutalyzer_hgvs_parser import to_model
-from mutalyzer_hgvs_parser.exceptions import UnexpectedCharacter, UnexpectedEnd
+from mutalyzer_hgvs_parser.exceptions import UnexpectedCharacter, UnexpectedEnd, NestedDescriptions
 from mutalyzer_mutator import mutate
 from mutalyzer_mutator.util import reverse_complement
 from mutalyzer_retriever.reference import (
     get_assembly_chromosome_accession,
     get_assembly_id,
     get_chromosome_accession_from_mrna_model,
     get_reference_mol_type,
@@ -191,14 +191,16 @@
         start_rule = "variants" if self.only_variants else "description"
         try:
             model = to_model(self.input_description, start_rule)
         except UnexpectedCharacter as e:
             self._add_error(errors.syntax_uc(e))
         except UnexpectedEnd as e:
             self._add_error(errors.syntax_ueof(e))
+        except NestedDescriptions as e:
+            self._add_error(errors.syntax_nested(e))
         else:
             if start_rule == "variants":
                 self.input_model = {"variants": model}
             else:
                 self.input_model = model
 
     def _set_main_reference(self):
@@ -266,16 +268,20 @@
             else:
                 reference_id_in_model = get_reference_id_from_model(reference_model)
                 if reference_id_in_model != reference_id:
                     self._correct_reference_id(
                         path, reference_id, reference_id_in_model
                     )
                     _update_references(reference_id_in_model, reference_model)
+                    ref_id = reference_id_in_model
                 else:
                     _update_references(reference_id, reference_model)
+                    ref_id = reference_id
+                if ref_id.startswith("LRG_"):
+                    self.add_info(infos.lrg_warning(ref_id, path))
                 self._set_main_reference()
 
     @check_errors
     def _check_selectors_in_references(self):
         for reference_id, selector_id, path in yield_reference_selector_ids(
             self.corrected_model
         ):
@@ -399,14 +405,15 @@
                 if c_s_s != c_s and not (
                     (c_s_s == "c" and c_s in ["r", "p"])
                     or (c_s_s == "n" and c_s == "r")
                 ):
                     self._add_error(
                         errors.coordinate_system_mismatch(c_s, s_id, c_s_s, c_s_path)
                     )
+
             else:
                 r_c_s = get_coordinate_system_from_reference(self.references[r_id])
                 if not ((r_c_s == c_s) and (c_s in ["g", "m", "p"])):
                     if is_only_one_selector(self.references[r_id]):
                         self._correct_selector_id_from_coordinate_system(
                             r_id,
                             r_path,
@@ -696,18 +703,19 @@
                         e_d = {
                             "description": model_to_string(converted_model),
                             "protein_prediction": get_protein_description(
                                 variants_to_delins(from_model["variants"]),
                                 self.references,
                                 protein_selector_model,
                             )[0],
-                        }
+                        "selector": {"id": selector["id"]}}
                     else:
                         if as_description:
-                            e_d = {"description": model_to_string(converted_model)}
+                            e_d = {"description": model_to_string(converted_model),
+                                   "reference": { "selector": {"id": selector["id"]}}}
                         else:
                             e_d = {"description": converted_model}
                     if (
                         selector.get("qualifiers")
                         and selector["qualifiers"].get("tag")
                         and "MANE" in selector["qualifiers"]["tag"]
                     ):
@@ -897,32 +905,29 @@
                     self._add_error(errors.offset(point, path))
                 if point.get("outside_cds"):
                     self._add_error(errors.outside_cds(point, path))
 
     def _check_intronic_point(self, point, path):
         if point.get("offset"):
             ref_id = self.corrected_model["reference"]["id"]
+            c_s = self.corrected_model["coordinate_system"]
             for ins_or_del in ["inserted", "deleted"]:
                 if ins_or_del in path:
-                    ins_or_del_ref_id = get_reference_id(
-                        get_submodel_by_path(
-                            self.corrected_model,
-                            path[: path.index(ins_or_del) + 2],
-                        )
-                    )
+                    submodel = get_submodel_by_path(self.corrected_model, path[: path.index(ins_or_del) + 2])
+                    ins_or_del_ref_id = get_reference_id(submodel)
                     if ins_or_del_ref_id:
                         ref_id = ins_or_del_ref_id
-            if get_reference_mol_type(self.references[ref_id]) in [
-                "mRNA",
-                "ncRNA",
-                "transcribed RNA",
-            ]:
-                if point.get("offset"):
-                    # TODO: find the actual NM(NC) description
-                    self._add_error(errors.intronic(point, path))
+                    if submodel.get("coordinate_system"):
+                        c_s = submodel["coordinate_system"]
+            ref_mol_type = get_reference_mol_type(self.references[ref_id])
+            if ref_mol_type in ["mRNA", "ncRNA", "transcribed RNA"]:
+                # TODO: find the actual NM(NC) description
+                self._add_error(errors.intronic(point, path))
+            elif ref_mol_type == "genomic DNA" and c_s == "r":
+                self._add_error(errors.intronic_rna(point, path))
 
     def _check_location_extras(self):
         for point, path in yield_sub_model(
             self.corrected_model, ["location", "start", "end"], ["point"]
         ):
             self._check_genomic_point(point, path)
             self._check_intronic_point(point, path)
@@ -1070,20 +1075,14 @@
                     set_by_path(self.internal_indexing_model, path, seq_dna)
                 else:
                     seq_lower = seq.lower()
                     if seq_lower != seq:
                         self.add_info(infos.corrected_sequence(seq, seq_lower))
                     if not is_rna(seq_lower):
                         self._add_error(errors.no_rna(seq_lower, path))
-                    seq_lower = str(Seq(seq).back_transcribe()).upper()
-                    # set_by_path(self.corrected_model, path, seq_lower)
-                    if self.is_inverted():
-                        path = reverse_path(self.corrected_model, path)
-                    set_by_path(self.internal_coordinates_model, path, seq_lower)
-                    set_by_path(self.internal_indexing_model, path, seq_lower)
 
     @check_errors
     def _check_location_amino_acids(self):
         sequences = self.get_sequences()
         for point, path in yield_sub_model(
             self.internal_coordinates_model, ["location", "start", "end"], ["point"]
         ):
@@ -1154,14 +1153,15 @@
 
     @check_errors
     def pre_conversion_checks(self):
         self._check_selectors_in_references()
         self._check_coordinate_systems()
         self._check_coordinate_system_consistency()
         self._check_selector_models()
+        self._rna()
         self._check_location_extras()
         if contains_uncertain_locations(self.corrected_model):
             self._add_error(errors.uncertain())
         if contains_insert_length(self.corrected_model):
             self._add_error(errors.inserted_length())
         self._check_cds()
 
@@ -1225,37 +1225,19 @@
             if variant.get("type") is not None:
                 return False
         return True
 
     @check_errors
     def _rna(self):
         if self.corrected_model.get("coordinate_system") == "r":
-            errors_splice, infos_splice = splice_sites(
-                self.internal_indexing_model["variants"],
-                self.get_sequences(),
-                self.get_selector_model(),
-            )
-            self.infos += infos_splice
-            self.errors += errors_splice
-            if errors_splice:
-                return
-
-            self.internal_indexing_model["variants"] = to_rna_variants(
-                self.internal_indexing_model["variants"],
-                self.get_sequences(),
-                self.get_selector_model(),
-            )
             rna_reference_model = to_rna_reference_model(
                 self.references["reference"], self.get_selector_id()
             )
-            # self.delins_model["variants"] = variants
-            self.references = {
-                get_reference_id(self.corrected_model): rna_reference_model,
-                "reference": rna_reference_model,
-            }
+            self.references["reference"] = rna_reference_model
+            self.references[get_reference_id(self.corrected_model)] = rna_reference_model
 
     def _check_amino_acids(self):
         for sequence, path in yield_values(
             self.corrected_model, ["sequence", "amino_acid"]
         ):
             seq_1a = str(seq1(sequence))
             seq_3a = str(seq3(sequence))
@@ -1283,20 +1265,22 @@
 
     def _back_translate(self):
         reference_id = get_reference_id(self.corrected_model)
         selector_id = self.get_selector_id()
         if not selector_id:
             cds_id = reference_id
             mrna_id = get_cds_to_mrna(cds_id)
-            if len(mrna_id) >= 1:
+            if mrna_id and len(mrna_id) >= 1:
                 mrna_id = mrna_id[-1]
         else:
             mrna_id = get_reference_id(self.corrected_model)
             cds_id = self.get_selector_id()
 
+        if not mrna_id:
+            return []
         cds_seq = slice_to_selector(
             retrieve_reference(mrna_id, cds_id)[0],
             cds_id,
             True,
             True,
         )
         bt = BackTranslate()
@@ -1387,15 +1371,15 @@
                     self.references["reference"]["sequence"]["seq"], observed_sequence
                 )[0],
             )
             self.de_hgvs_model = to_model(p_description)
         self.normalized_description = model_to_string(self.de_hgvs_model)
         equivalent_1a_model = copy.deepcopy(self.de_hgvs_model)
         convert_amino_acids(equivalent_1a_model, "1a")
-        self.equivalent = {"p": [model_to_string(equivalent_1a_model)]}
+        self.equivalent = {"p": [{"description": model_to_string(equivalent_1a_model)}]}
         self._back_translate()
 
     @check_errors
     def get_chromosomal_descriptions(self):
         # TODO: Add tests.
         if (
             not self.references
@@ -1532,25 +1516,25 @@
                         chromosomal_description["tag"] = tag
                     chromosomal_descriptions.append(chromosomal_description)
 
         if chromosomal_descriptions:
             self.chromosomal_descriptions = chromosomal_descriptions
 
     def to_delins(self):
+        self.assembly_checks()
         self.retrieve_references()
         self.pre_conversion_checks()
 
         self._correct_chromosome_points()
         self.to_internal_indexing_model()
         self._correct_variants_type()
         self._correct_points()
         self._check_and_correct_sequences()
 
         self.check()
-        self._rna()
         self._construct_delins_model()
 
     def normalize_only_equals_or_no_operation(self):
         self.de_hgvs_internal_indexing_model = self.internal_indexing_model
         self.references["observed"] = {
             "sequence": {"seq": self.references["reference"]["sequence"]["seq"]}
         }
@@ -1569,15 +1553,14 @@
             self._correct_chromosome_points()
             self.to_internal_indexing_model()
             self._correct_variants_type()
             self._correct_points()
             self._check_and_correct_sequences()
 
             self.check()
-            self._rna()
             self._construct_delins_model()
             if self.only_equals() or self.no_operation():
                 self.normalize_only_equals_or_no_operation()
             else:
                 self.mutate()
                 self.extract()
                 self.construct_de_hgvs_internal_indexing_model()
```

### Comparing `mutalyzer-3.0.5/mutalyzer/description_extractor.py` & `mutalyzer-3.0.6/mutalyzer/description_extractor.py`

 * *Files identical despite different names*

### Comparing `mutalyzer-3.0.5/mutalyzer/description_model.py` & `mutalyzer-3.0.6/mutalyzer/description_model.py`

 * *Files identical despite different names*

### Comparing `mutalyzer-3.0.5/mutalyzer/errors.py` & `mutalyzer-3.0.6/mutalyzer/errors.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,14 +94,22 @@
         "details": "Intronic position {} given for a non-genomic "
         "reference sequence. Tip: make use of a genomic reference "
         "sequence like NC_*(NM_*).".format(location_to_description(location)),
         "paths": [path],
     }
 
 
+def intronic_rna(location, path):
+    return {
+        "code": "EINTRONICRNA",
+        "details": f"Intronic position {location_to_description(location)} given for an RNA description.",
+        "paths": [path],
+    }
+
+
 def out_of_boundary_lesser(position, shift, path):
     plural = "s" if shift > 1 else ""
     return {
         "code": "EOUTOFBOUNDARY",
         "details": "Position {} is {} nucleotide{} before the sequence start.".format(
             point_to_description(position), shift, plural
         ),
@@ -258,14 +266,18 @@
 
 def syntax_ueof(e):
     return dict(
         {"code": "ESYNTAXUEOF", "details": "Unexpected end of input."}, **e.serialize()
     )
 
 
+def syntax_nested(e):
+    return {"code": "ESYNTAXNESTED", "details": "Nested descriptions encountered."}
+
+
 def position_syntax(details, e):
     return dict({"code": "EPOSITIONSYNTAX", "details": details}, **e.serialize())
 
 
 def position_invalid():
     return {"code": "EPOSITIONINVALID", "details": "Position must be string"}
```

### Comparing `mutalyzer-3.0.5/mutalyzer/infos.py` & `mutalyzer-3.0.6/mutalyzer/infos.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,14 +17,24 @@
         "details": "Reference {} was identified as LRG with ID {} and selector {}.".format(
             original_id, lrg_model["id"], lrg_model["selector"]["id"]
         ),
         "paths": [path],
     }
 
 
+def lrg_warning(ref_id, path):
+    return {
+        "code": "ILRGWARNING",
+        "details": "Reference {} was identified as LRG. Please note that LRGs are no longer updated.".format(
+            ref_id,
+        ),
+        "paths": [path],
+    }
+
+
 def corrected_selector_id(original_id, corrected_id, correction_source, path):
     return {
         "code": "ICORRECTEDSELECTORID",
         "details": "Selector {} was corrected to {} from {}.".format(
             original_id, corrected_id, correction_source
         ),
         "paths": [path],
```

### Comparing `mutalyzer-3.0.5/mutalyzer/mapper.py` & `mutalyzer-3.0.6/mutalyzer/mapper.py`

 * *Files identical despite different names*

### Comparing `mutalyzer-3.0.5/mutalyzer/mutator.py` & `mutalyzer-3.0.6/mutalyzer/mutator.py`

 * *Files identical despite different names*

### Comparing `mutalyzer-3.0.5/mutalyzer/position_converter.py` & `mutalyzer-3.0.6/mutalyzer/position_converter.py`

 * *Files identical despite different names*

### Comparing `mutalyzer-3.0.5/mutalyzer/protein.py` & `mutalyzer-3.0.6/mutalyzer/protein.py`

 * *Files identical despite different names*

### Comparing `mutalyzer-3.0.5/mutalyzer/reference.py` & `mutalyzer-3.0.6/mutalyzer/reference.py`

 * *Files identical despite different names*

### Comparing `mutalyzer-3.0.5/mutalyzer/spdi_converter.py` & `mutalyzer-3.0.6/mutalyzer/spdi_converter.py`

 * *Files identical despite different names*

### Comparing `mutalyzer-3.0.5/mutalyzer/util.py` & `mutalyzer-3.0.6/mutalyzer/util.py`

 * *Files identical despite different names*

### Comparing `mutalyzer-3.0.5/mutalyzer/validation.py` & `mutalyzer-3.0.6/mutalyzer/validation.py`

 * *Files identical despite different names*

### Comparing `mutalyzer-3.0.5/mutalyzer/viewer.py` & `mutalyzer-3.0.6/mutalyzer/viewer.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,15 +101,15 @@
 
     return output
 
 
 def view_variants_normalized(d, left=15, right=15, invert=True):
     return view_delins(
         d.delins_model["variants"],
-        d.corrected_model["variants"],
+        d.corrected_model["variants"][::-1] if d.is_inverted() else d.corrected_model["variants"],
         d.get_sequences(),
         left,
         right,
         invert and d.is_inverted(),
     )
```

### Comparing `mutalyzer-3.0.5/mutalyzer.egg-info/PKG-INFO` & `mutalyzer-3.0.6/mutalyzer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mutalyzer
-Version: 3.0.5
+Version: 3.0.6
 Summary: Mutalyzer HGVS variant description tools.
 Home-page: https://github.com/mutalyzer/mutalyzer
 Author: Mihai Lefter
 Author-email: M.Lefter@lumc.nl
 License: MIT
 Keywords: Mutalyzer,HGVS
 Classifier: Intended Audience :: Science/Research
```

### Comparing `mutalyzer-3.0.5/mutalyzer.egg-info/SOURCES.txt` & `mutalyzer-3.0.6/mutalyzer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mutalyzer-3.0.5/setup.cfg` & `mutalyzer-3.0.6/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = mutalyzer
-version = 3.0.5
+version = 3.0.6
 description = Mutalyzer HGVS variant description tools.
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 author = Mihai Lefter
 author_email = M.Lefter@lumc.nl
 url = https://github.com/mutalyzer/mutalyzer
 keywords = Mutalyzer, HGVS
@@ -15,22 +15,22 @@
 	Operating System :: OS Independent
 	Programming Language :: Python :: 3
 	Topic :: Scientific/Engineering :: Bio-Informatics
 
 [options]
 packages = find:
 install_requires = 
-	mutalyzer-hgvs-parser==0.3.3
-	mutalyzer-spdi-parser==0.3.0
-	mutalyzer-retriever==0.3.0
-	mutalyzer-mutator==0.2.0
-	mutalyzer_crossmapper==2.0.1
-	mutalyzer-backtranslate==1.0.0
-	description-extractor==3.0.0
-	mutalyzer-algebra==1.1.1
+	mutalyzer-hgvs-parser>=0.3.4
+	mutalyzer-spdi-parser>=0.3.0
+	mutalyzer-retriever>=0.3.2
+	mutalyzer-mutator>=0.2.0
+	mutalyzer_crossmapper>=2.0.1
+	mutalyzer-backtranslate>=1.0.0
+	description-extractor>=3.0.0
+	mutalyzer-algebra>=1.1.1
 tests_require = 
 	pytest
 
 [options.entry_points]
 console_scripts = 
 	mutalyzer_normalizer = mutalyzer.cli:main
```

### Comparing `mutalyzer-3.0.5/tests/commons.py` & `mutalyzer-3.0.6/tests/commons.py`

 * *Files 19% similar despite different names*

```diff
@@ -18,25 +18,31 @@
     reference_id,
     reference_source=None,
     reference_type=None,
     size_off=True,
     configuration_path=None,
     timeout=1,
 ):
+    print("\nretrive raw\n")
     if reference_type == "fasta":
         return _get_content("data/" + reference_id + ".fasta"), "fasta", "ncbi"
     elif reference_id.startswith("LRG_"):
         return _get_content("data/" + reference_id), "lrg", "lrg"
     else:
         return _get_content("data/" + reference_id + ".gff3"), "gff3", "ncbi"
 
 
+def get_cds_to_mrna(cds_id, timeout=10):
+    return None
+
+
 @pytest.fixture(autouse=True)
-def patch_retriever(monkeypatch):
+def monkey_patches(monkeypatch):
     monkeypatch.setattr("mutalyzer_retriever.retriever.retrieve_raw", retrieve_raw)
+    monkeypatch.setattr("mutalyzer.description.get_cds_to_mrna", get_cds_to_mrna)
     monkeypatch.setattr("mutalyzer.util.configuration", lambda: None)
 
 
 def code_in(code, messages):
     for meessage in messages:
         if meessage["code"] == code:
             return True
```

### Comparing `mutalyzer-3.0.5/tests/generator.py` & `mutalyzer-3.0.6/tests/generator.py`

 * *Files identical despite different names*

### Comparing `mutalyzer-3.0.5/tests/test_algebra.py` & `mutalyzer-3.0.6/tests/test_algebra.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 import pytest
 
 from mutalyzer.algebra import _get_hgvs_and_variant, _get_id, compare
 from mutalyzer.reference import retrieve_reference
 
-from .commons import code_in, patch_retriever
+from .commons import code_in, monkey_patches
 
 
 @pytest.mark.parametrize(
     "reference_id",
     ["NM_012459.2", "LRG_24"],
 )
 def test_get_id(reference_id):
     assert _get_id(reference_id) == {
         "input": reference_id,
         "type": "id",
         "reference": {"id": reference_id},
+        "annotations": {"id": reference_id},
         "sequence": retrieve_reference(reference_id)[0]["sequence"]["seq"],
     }
 
 
 @pytest.mark.parametrize(
     "reference_id",
     ["NO_REF"],
@@ -150,14 +151,22 @@
                 "LRG_24:g.5525_5533del",
                 "hgvs",
             ),
             {
                 "relation": "is_contained",
                 "influence_lhs": {"min_pos": 5521, "max_pos": 5534},
                 "influence_rhs": {"min_pos": 5521, "max_pos": 5534},
+                "supremal_lhs": {
+                    "hgvs": "LRG_24:g.5522_5534delinsGCCCA",
+                    "spdi": "LRG_24:5521:13:GCCCA",
+                },
+                "supremal_rhs": {
+                    "hgvs": "LRG_24:g.5522_5534delinsGCCA",
+                    "spdi": "LRG_24:5521:13:GCCA",
+                },
                 "view_lhs": {
                     "views": [
                         {
                             "start": 0,
                             "end": 5524,
                             "type": "outside",
                             "left": "GTTCACACTTCTCTC",
@@ -217,14 +226,22 @@
                 "LRG_24:g.5525_5533del",
                 "hgvs",
             ),
             {
                 "relation": "is_contained",
                 "influence_lhs": {"min_pos": 5521, "max_pos": 5534},
                 "influence_rhs": {"min_pos": 5521, "max_pos": 5534},
+                "supremal_lhs": {
+                    "hgvs": "LRG_24:g.5522_5534delinsGCCCA",
+                    "spdi": "LRG_24:5521:13:GCCCA",
+                },
+                "supremal_rhs": {
+                    "hgvs": "LRG_24:g.5522_5534delinsGCCA",
+                    "spdi": "LRG_24:5521:13:GCCA",
+                },
                 "view_lhs": {
                     "views": [
                         {
                             "start": 0,
                             "end": 5524,
                             "type": "outside",
                             "left": "GTTCACACTTCTCTC",
@@ -284,14 +301,22 @@
                 "LRG_24:g.5525_5533del",
                 "hgvs",
             ),
             {
                 "relation": "is_contained",
                 "influence_lhs": {"min_pos": 5521, "max_pos": 5534},
                 "influence_rhs": {"min_pos": 5521, "max_pos": 5534},
+                "supremal_lhs": {
+                    "hgvs": "LRG_24:g.5522_5534delinsGCCCA",
+                    "spdi": "LRG_24:5521:13:GCCCA",
+                },
+                "supremal_rhs": {
+                    "hgvs": "LRG_24:g.5522_5534delinsGCCA",
+                    "spdi": "LRG_24:5521:13:GCCA",
+                },
                 "view_lhs": {
                     "views": [
                         {
                             "start": 0,
                             "end": 5524,
                             "type": "outside",
                             "left": "GTTCACACTTCTCTC",
@@ -351,14 +376,22 @@
                 "LRG_24:g.5525_5533del",
                 "hgvs",
             ),
             {
                 "relation": "is_contained",
                 "influence_lhs": {"min_pos": 5521, "max_pos": 5534},
                 "influence_rhs": {"min_pos": 5521, "max_pos": 5534},
+                "supremal_lhs": {
+                    "hgvs": "LRG_24:g.5522_5534delinsGCCCA",
+                    "spdi": "LRG_24:5521:13:GCCCA",
+                },
+                "supremal_rhs": {
+                    "hgvs": "LRG_24:g.5522_5534delinsGCCA",
+                    "spdi": "LRG_24:5521:13:GCCA",
+                },
                 "view_lhs": {
                     "views": [
                         {
                             "start": 0,
                             "end": 5524,
                             "type": "outside",
                             "left": "GTTCACACTTCTCTC",
@@ -418,14 +451,22 @@
                 "LRG_303:g.5525_5532del",
                 "hgvs",
             ),
             {
                 "relation": "equivalent",
                 "influence_lhs": {"min_pos": 5518, "max_pos": 5534},
                 "influence_rhs": {"min_pos": 5518, "max_pos": 5534},
+                "supremal_lhs": {
+                    "hgvs": "NG_008376.4:g.5519_5534delinsGAGTTATG",
+                    "spdi": "NG_008376.4:5518:16:GAGTTATG",
+                },
+                "supremal_rhs": {
+                    "hgvs": "NG_008376.4:g.5519_5534delinsGAGTTATG",
+                    "spdi": "NG_008376.4:5518:16:GAGTTATG",
+                },
                 "view_lhs": {
                     "views": [
                         {
                             "start": 0,
                             "end": 5524,
                             "type": "outside",
                             "left": "GTGTCTGCCAAGGGT",
@@ -485,14 +526,22 @@
                 "274del",
                 "variant",
             ),
             {
                 "relation": "contains",
                 "influence_lhs": {"min_pos": 272, "max_pos": 275},
                 "influence_rhs": {"min_pos": 273, "max_pos": 274},
+                "supremal_lhs": {
+                    "hgvs": "NG_012337.3:g.273_275delinsAAA",
+                    "spdi": "NG_012337.3:272:3:AAA",
+                },
+                "supremal_rhs": {
+                    "hgvs": "NG_012337.3:g.274del",
+                    "spdi": "NG_012337.3:273:1:",
+                },
                 "view_lhs": {
                     "views": [
                         {
                             "start": 0,
                             "end": 273,
                             "type": "outside",
                             "left": "GGGCTTGGTTCTACC",
@@ -553,14 +602,22 @@
                 "274del",
                 "variant",
             ),
             {
                 "relation": "contains",
                 "influence_lhs": {"min_pos": 272, "max_pos": 275},
                 "influence_rhs": {"min_pos": 273, "max_pos": 274},
+                "supremal_lhs": {
+                    "hgvs": "NG_012337.3:g.273_275delinsAAA",
+                    "spdi": "NG_012337.3:272:3:AAA",
+                },
+                "supremal_rhs": {
+                    "hgvs": "NG_012337.3:g.274del",
+                    "spdi": "NG_012337.3:273:1:",
+                },
                 "view_lhs": {
                     "views": [
                         {
                             "start": 0,
                             "end": 273,
                             "type": "outside",
                             "left": "GGGCTTGGTTCTACC",
@@ -621,14 +678,22 @@
                 "274del",
                 "variant",
             ),
             {
                 "relation": "contains",
                 "influence_lhs": {"min_pos": 272, "max_pos": 275},
                 "influence_rhs": {"min_pos": 273, "max_pos": 274},
+                "supremal_lhs": {
+                    "hgvs": "NG_012337.3:g.273_275delinsAAA",
+                    "spdi": "NG_012337.3:272:3:AAA",
+                },
+                "supremal_rhs": {
+                    "hgvs": "NG_012337.3:g.274del",
+                    "spdi": "NG_012337.3:273:1:",
+                },
                 "view_lhs": {
                     "views": [
                         {
                             "start": 0,
                             "end": 273,
                             "type": "outside",
                             "left": "GGGCTTGGTTCTACC",
```

### Comparing `mutalyzer-3.0.5/tests/test_back_translator.py` & `mutalyzer-3.0.6/tests/test_back_translator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import pytest
 
 from mutalyzer.back_translator import back_translate
 
-from .commons import code_in, patch_retriever
+from .commons import code_in, monkey_patches
 
 
 @pytest.mark.parametrize(
     "protein_description, back_translated_descriptions",
     [
         (
             "NM_003002.2:p.Asp92Tyr",
```

### Comparing `mutalyzer-3.0.5/tests/test_checker.py` & `mutalyzer-3.0.6/tests/test_checker.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import pytest
 
 from mutalyzer.normalizer import normalize
 
-from .commons import code_in, patch_retriever
+from .commons import code_in, monkey_patches
 from .variants_set import TESTS_ALL
 
 TESTS_ERROR = [
     ("NG_007485.1:g.0del", "EOUTOFBOUNDARY"),
     ("NG_007485.1:g.-1del", "EOUTSIDECDS"),
     ("NG_007485.1:g.1000000del", "EOUTOFBOUNDARY"),
     ("NG_007485.1(NM_000077.4):c.40000del", "EOUTOFBOUNDARY"),
```

### Comparing `mutalyzer-3.0.5/tests/test_converter.py` & `mutalyzer-3.0.6/tests/test_converter.py`

 * *Files identical despite different names*

### Comparing `mutalyzer-3.0.5/tests/test_description.py` & `mutalyzer-3.0.6/tests/test_description.py`

 * *Files identical despite different names*

### Comparing `mutalyzer-3.0.5/tests/test_ensembl.py` & `mutalyzer-3.0.6/tests/test_ensembl.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pytest
 
 from mutalyzer.normalizer import normalize
 from mutalyzer.reference import retrieve_reference, slice_to_selector
 
-from .commons import code_in, patch_retriever
+from .commons import code_in, monkey_patches
 from .variants_set import TESTS_ALL
 
 
 def get_tests(tests, t_type):
     output = []
     for test in tests:
         if test.get("to_test") and test.get(t_type):
```

### Comparing `mutalyzer-3.0.5/tests/test_mapper.py` & `mutalyzer-3.0.6/tests/test_mapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 import pytest
 
 from mutalyzer.mapper import map_description
 
-from .commons import code_in, patch_retriever
+from .commons import code_in, monkey_patches
 
 TEST_SET = [
     (
         # Transcript to same transcript.
         ("NM_003002.2:c.274G>T", "NM_003002.2"),
         "NM_003002.2:c.274G>T",
     ),
     (
+        # Transcript to same transcript.
+        ("NM_003002.4:c.274G>T", "NM_003002.4"),
+        "NM_003002.4:c.274G>T",
+    ),
+    (
         # Transcript to NG with transcript slice.
         ("NM_003002.2:c.274G>T", "NG_012337.1", "NM_003002.2", "transcript", False),
         "NG_012337.1(NM_003002.2):c.[274G>T;*824A[18]]",
     ),
     (
         # Transcript to NG with transcript slice with filtering.
         ("NM_003002.2:c.274G>T", "NG_012337.1", "NM_003002.2", "transcript", True),
@@ -151,14 +156,18 @@
         ),
         "NM_012459.2:c.130G>A",
     ),
     (
         ("NM_012459.2:c.130G>A", "NG_012337.1", "NM_012459.2", "transcript", False),
         "NG_012337.1(NM_012459.2):c.130G>A",
     ),
+    (
+        ("NG_012337.3(NM_003002.4):c.274G>T", "NM_003002.4", None, "transcript", False),
+        "NM_003002.4:c.274G>T",
+    ),
 ]
 
 
 @pytest.mark.parametrize("input_params, correct_output", TEST_SET)
 def test_mapper(input_params, correct_output):
     assert map_description(*input_params)["mapped_description"] == correct_output
```

### Comparing `mutalyzer-3.0.5/tests/test_normalizer.py` & `mutalyzer-3.0.6/tests/test_normalizer.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,31 @@
 import pytest
 
 from mutalyzer.normalizer import normalize
 
-from .commons import code_in, patch_retriever
+from .commons import code_in, monkey_patches
 from .variants_set import TESTS_ALL
 
 
 def get_tests(tests, t_type):
     output = []
     for test in tests:
         if test.get("to_test") and test.get(t_type):
             output.append((test["input"], test[t_type]))
     return output
 
 
+def get_tests_rna_protein(tests):
+    output = []
+    for test in tests:
+        if test.get("rna_description") and test.get("protein_description"):
+            output.append((test["rna_description"], test["protein_description"]))
+    return output
+
+
 @pytest.mark.parametrize(
     "input_description, normalized", get_tests(TESTS_ALL, "normalized")
 )
 def test_normalize(input_description, normalized):
     d = normalize(input_description)
     assert d["normalized_description"] == normalized
 
@@ -67,23 +75,35 @@
         ]
     )
 
     assert coding_protein_descriptions.issubset(normalizer_descriptions)
 
 
 @pytest.mark.parametrize(
+    "rna_description, protein_description",
+    get_tests_rna_protein(TESTS_ALL),
+)
+def test_rna_protein(rna_description, protein_description):
+
+    normalized_output = normalize(rna_description)
+    normalizer_protein = normalized_output["protein"]["description"]
+
+    assert normalizer_protein == protein_description
+
+
+@pytest.mark.parametrize(
     "input_description, rna_description",
     get_tests(TESTS_ALL, "rna_description"),
 )
 def test_rna(input_description, rna_description):
 
     normalized_output = normalize(input_description)
-    normalizer_protein = normalized_output["rna"]["description"]
+    normalized_rna = normalized_output["rna"]["description"]
 
-    assert normalizer_protein == rna_description
+    assert normalized_rna == rna_description
 
 
 @pytest.mark.parametrize("input_description, codes", get_tests(TESTS_ALL, "errors"))
 def test_errors(input_description, codes):
     assert codes == [error["code"] for error in normalize(input_description)["errors"]]
```

### Comparing `mutalyzer-3.0.5/tests/test_position_convert.py` & `mutalyzer-3.0.6/tests/test_position_convert.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from mutalyzer_hgvs_parser import to_model
 
 from mutalyzer.description_model import model_to_string
 from mutalyzer.position_converter import position_convert
 
-from .commons import code_in, get_codes, patch_retriever
+from .commons import code_in, get_codes, monkey_patches
 
 
 def test_error_no_required_inputs_reference_id():
     p_c = position_convert(
         reference_id=None,
         position="100",
         from_selector_id=None,
```

### Comparing `mutalyzer-3.0.5/tests/test_protein.py` & `mutalyzer-3.0.6/tests/test_protein.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import pytest
 
 from mutalyzer.normalizer import normalize
 
-from .commons import code_in, patch_retriever
+from .commons import code_in, monkey_patches
 
 TESTS = [
     {
         "keywords": ["protein", "equal", "genomic"],
         "input": "NG_012337.1(NP_002993.1):p.(=)",
         "normalized": "NG_012337.1(NP_002993.1):p.(=)",
         "to_test": True,
@@ -103,14 +103,22 @@
                 "code": "EAMINOACIDMISMATCH",
                 "details": "D not found in the reference sequence, found H instead.",
                 "paths": [["variants", 0, "inserted", 0, "location", "start"]],
             },
         ],
         "to_test": True,
     },
+    {
+        "keywords": [
+            "protein missing mrna for backtranslation",
+        ],
+        "input": "YP_009725300.1:p.(Leu360Ter)",
+        "normalized": "YP_009725300.1:p.(Leu360Ter)",
+        "to_test": True,
+    },
 ]
 
 
 def get_tests(tests, t_type):
     output = []
     for test in tests:
         if test.get("to_test"):
```

### Comparing `mutalyzer-3.0.5/tests/test_reference.py` & `mutalyzer-3.0.6/tests/test_reference.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pytest
 from mutalyzer_retriever.retriever import get_reference_model_segmented
 
 from mutalyzer.reference import get_internal_selector_model, get_selector_feature
 
-from .commons import patch_retriever
+from .commons import monkey_patches
 
 
 def test_get_reference_model_segmented_record_no_siblings_ancestors_no_descendants():
     feature_model = {
         "id": "NG_012337.1",
         "type": "record",
         "location": {
```

### Comparing `mutalyzer-3.0.5/tests/test_to_description.py` & `mutalyzer-3.0.6/tests/test_to_description.py`

 * *Files identical despite different names*

### Comparing `mutalyzer-3.0.5/tests/test_viewer.py` & `mutalyzer-3.0.6/tests/test_viewer.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import pytest
 
 from mutalyzer.viewer import view_variants
 
-from .commons import patch_retriever
+from .commons import monkey_patches
 
 
 @pytest.mark.parametrize(
     "description, output",
     [
         (
             "NM_003002.2:r.274g>u",
```

### Comparing `mutalyzer-3.0.5/tests/variants_set.py` & `mutalyzer-3.0.6/tests/variants_set.py`

 * *Files 1% similar despite different names*

```diff
@@ -1137,15 +1137,15 @@
             "M2: test_lrg_reference",
             "M2: We should be able to use LRG reference sequence without error.",
         ],
         "input": "LRG_1t1:c.266G>T",
         "normalized": "LRG_1(t1):c.266G>T",  # TODO: check if OK.
         "genomic": "LRG_1:g.6855G>T",
         "protein_description": "LRG_1(p1):p.(Gly89Val)",
-        "infos": ["ICORRECTEDLRGREFERENCE"],
+        "infos": ["ICORRECTEDLRGREFERENCE", "ILRGWARNING"],
         "to_test": True,
     },
     # test_gi_reference_plain: gi numbers not supported in M3.
     # test_gi_reference_prefix:
     # test_gi_reference_prefix_colon:
     {
         "keywords": [
@@ -2448,15 +2448,15 @@
             ),
             (
                 "NG_009299.1(NM_001143979.2):c.41A>C",
                 "NG_009299.1(NP_001137451.1):p.(Gln14Profs*68)",
             ),
         },
         "protein_description": "NG_009299.1(NP_060138.1):p.(Gln14Profs*68)",
-        "rna_description": "NG_009299.1(NM_017668.3):r.(40a>c)",
+        "rna_description": "NG_009299.1(NM_017668.3):r.(41a>c)",
         "to_test": True,
     },
     {
         "keywords": [],
         "input": "NG_012337.1:g.7125G>T",
         "coding_protein_descriptions": {
             (
@@ -2495,15 +2495,15 @@
         "rna_description": "NG_012337.1(NM_012459.2):r.(4_6delinsgua)",
         "to_test": True,
     },
     {
         "keywords": ["reference", "LRG", "replace"],
         "input": "LRG_303(t1):c.10_11insLRG_1t1:c.100_101",
         "normalized": "LRG_303(t1):c.10_11insGA",
-        "infos": ["ICORRECTEDLRGREFERENCE"],
+        "infos": ["ILRGWARNING", "ICORRECTEDLRGREFERENCE", "ILRGWARNING"],
         "to_test": True,
     },
     {
         "keywords": [],
         "input": "LRG_303:g.[105_106del;6681G>C;6883_6884insTTTCGCCCCTTTCGCCCC]",
         "normalized": "LRG_303:g.[108_109del;6681G>C;6875_6883TTTCGCCCC[3]]",
         "to_test": True,
@@ -3113,14 +3113,138 @@
         "keywords": ["no cds for coding transcripts #73"],
         "input": "NG_012337.3(NM_003002.4):c.274delinsNG_009930.1(NM_001099625.2):c.1010",
         "errors": [
             "ENOCDS",
         ],
         "to_test": True,
     },
+    {
+        "keywords": [
+            "protein reverse strand whole exon deletion with shift"
+        ],
+        "input": "NG_008835.1(NM_022153.2):c.677-21_704+62del",
+        "normalized": "NG_008835.1(NM_022153.2):c.677-18_704+65del",
+        "rna_description": "NG_008835.1(NM_022153.2):r.(677_704del)",
+        "protein_description": "NG_008835.1(NP_071436.1):p.(Arg226Profs*102)",
+        "to_test": True,
+    },
+    {
+        "keywords": [
+            "protein reverse whole exon deletion no shift"
+        ],
+        "input": "NG_008835.1(NM_022153.2):c.677-20_704+62del",
+        "normalized": "NG_008835.1(NM_022153.2):c.677-20_704+62del",
+        "rna_description": "NG_008835.1(NM_022153.2):r.(677_704del)",
+        "protein_description": "NG_008835.1(NP_071436.1):p.(Arg226Profs*102)",
+        "to_test": True,
+    },
+    {
+        "keywords": [
+            "delins inversion"
+        ],
+        "input": "NM_003002.4:c.206_210delins190_220inv",
+        "normalized": "NM_003002.4:c.206_209delins191_220inv",
+        "rna_description": "NM_003002.4:r.(206_209delinscacugacaacccucucgcuaguccagugga)",
+        "protein_description": "NM_003002.4(NP_002993.1):p.(Glu69Alafs*26)",
+        "to_test": True,
+    },
+    {
+        "keywords": [
+            "insertion with positions other reference reverse strand"
+        ],
+        "input": "NG_012337.3:g.136delinsNG_012337.1(NM_012459.2):c.200",
+        "normalized": "NG_012337.3:g.136A>C",
+        "to_test": True,
+    },
+    {
+        "keywords": [
+            "insertion with positions other reference reverse strand"
+        ],
+        "input": "NG_012337.3(NM_003002.4):c.274delinsNG_012337.1(NM_012459.2):c.200_203",
+        "normalized": "NG_012337.3(NM_003002.4):c.274delinsCTGA",
+        "rna_description": "NG_012337.3(NM_003002.4):r.(274delinscuga)",
+        "protein_description": "NG_012337.3(NP_002993.1):p.(Asp92delinsLeuAsn)",
+        "to_test": True,
+    },
+    {
+        "keywords": [
+            "insertion with positions other reference reverse strand"
+        ],
+        "input": "NG_012337.1(NM_012459.2):c.274delinsNG_012337.3(NM_003002.4):c.200_203",
+        "normalized": "NG_012337.1(NM_012459.2):c.274delinsCTAG",
+        "rna_description": "NG_012337.1(NM_012459.2):r.(274delinscuag)",
+        "protein_description": "NG_012337.1(NP_036591.2):p.(Ile92delinsLeuVal)",
+        "to_test": True,
+    },
+
+    # {
+    #     "keywords": [
+    #         "rna",
+    #         "deletion",
+    #         "genomic",
+    #         "mRNA",
+    #         "same intron",
+    #         "plus strand",
+    #     ],
+    #     "input": "NG_012337.3(NM_003002.4):c.52+8_53-8del",
+    #     "normalized": "NG_012337.3(NM_003002.4):c.52+8_53-8del",
+    #     "rna_description": "NG_012337.3(NM_003002.4):r.=",
+    #     "protein_description": "NG_012337.3(NP_002993.1):p.(=)",
+    #     "infos": ["IVARIANTDISCARDED"],
+    #     "to_test": True,
+    # },
+    # {
+    #     "keywords": [
+    #         "rna",
+    #         "deletion",
+    #         "genomic",
+    #         "mRNA",
+    #         "intron - intron",
+    #         "same intron",
+    #         "minus strand",
+    #     ],
+    #     "input": "NG_012337.3(NM_012459.4):c.84+8_85-8del",
+    #     "normalized": "NG_012337.3(NM_012459.4):c.84+8_85-8del",
+    #     "rna_description": "NG_012337.3(NM_012459.4):r.(=)",
+    #     "protein_description": "NG_012337.3(NP_036591.3):p.(=)",
+    #     "infos": ["IVARIANTDISCARDED"],
+    #     "to_test": True,
+    # },
+    # {
+    #     "keywords": [
+    #         "rna",
+    #         "deletion",
+    #         "genomic",
+    #         "mRNA",
+    #         "intron - intron",
+    #         "plus strand",
+    #     ],
+    #     "input": "NG_012337.3(NM_003002.4):c.52+8_169+8del",
+    #     "normalized": "NG_012337.3(NM_003002.4):c.52+8_169+8del",
+    #     "rna_description": "NG_012337.3(NM_003002.4):r.(55_171del)",
+    #     "protein_description": "NG_012337.3(NP_002993.1):p.(Leu19_Ser57del)",
+    #     "infos": ["ISPLICESITEREMOVED"],
+    #     "to_test": True,
+    # },
+    # {
+    #     "keywords": [
+    #         "rna",
+    #         "deletion",
+    #         "genomic",
+    #         "mRNA",
+    #         "intron - intron",
+    #         "minus strand",
+    #     ],
+    #     "input": "NG_012337.3(NM_012459.4):c.84+8_*503del",
+    #     "normalized": "NG_012337.3(NM_012459.4):c.84+9_*504del",
+    #     "rna_description": "NG_012337.3(NM_012459.4):r.85_*495del",
+    #     "protein_description": "NG_012337.3(NP_036591.3):p.(Met1_Gln28dup)",
+    #     "infos": ["ISPLICESITEREMOVED"],
+    #     "to_test": True,
+    # },
     # {
     #     "keywords": [
     #
     #     ],
     #     "input": "",
     #     "normalized": "",
     #     "genomic": "",
```

