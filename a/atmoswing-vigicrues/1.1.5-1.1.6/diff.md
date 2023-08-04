# Comparing `tmp/atmoswing-vigicrues-1.1.5.tar.gz` & `tmp/atmoswing-vigicrues-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atmoswing-vigicrues-1.1.5.tar", last modified: Sun Jul  2 21:21:55 2023, max compression
+gzip compressed data, was "atmoswing-vigicrues-1.1.6.tar", last modified: Fri Aug  4 11:09:52 2023, max compression
```

## Comparing `atmoswing-vigicrues-1.1.5.tar` & `atmoswing-vigicrues-1.1.6.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 21:21:55.451140 atmoswing-vigicrues-1.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-02 21:21:34.000000 atmoswing-vigicrues-1.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-07-02 21:21:55.451140 atmoswing-vigicrues-1.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-07-02 21:21:34.000000 atmoswing-vigicrues-1.1.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-02 21:21:34.000000 atmoswing-vigicrues-1.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-02 21:21:55.451140 atmoswing-vigicrues-1.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-02 21:21:34.000000 atmoswing-vigicrues-1.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 21:21:55.447140 atmoswing-vigicrues-1.1.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 21:21:55.447140 atmoswing-vigicrues-1.1.5/src/atmoswing_vigicrues/
--rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-07-02 21:21:34.000000 atmoswing-vigicrues-1.1.5/src/atmoswing_vigicrues/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-07-02 21:21:34.000000 atmoswing-vigicrues-1.1.5/src/atmoswing_vigicrues/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11916 2023-07-02 21:21:34.000000 atmoswing-vigicrues-1.1.5/src/atmoswing_vigicrues/controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 21:21:55.447140 atmoswing-vigicrues-1.1.5/src/atmoswing_vigicrues/disseminations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 21:21:34.000000 atmoswing-vigicrues-1.1.5/src/atmoswing_vigicrues/disseminations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-02 21:21:34.000000 atmoswing-vigicrues-1.1.5/src/atmoswing_vigicrues/disseminations/dissemination.py
--rw-r--r--   0 runner    (1001) docker     (123)     5662 2023-07-02 21:21:34.000000 atmoswing-vigicrues-1.1.5/src/atmoswing_vigicrues/disseminations/transfer_sftp_out.py
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-07-02 21:21:34.000000 atmoswing-vigicrues-1.1.5/src/atmoswing_vigicrues/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-07-02 21:21:34.000000 atmoswing-vigicrues-1.1.5/src/atmoswing_vigicrues/options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 21:21:55.451140 atmoswing-vigicrues-1.1.5/src/atmoswing_vigicrues/postactions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 21:21:34.000000 atmoswing-vigicrues-1.1.5/src/atmoswing_vigicrues/postactions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13301 2023-07-02 21:21:34.000000 atmoswing-vigicrues-1.1.5/src/atmoswing_vigicrues/postactions/export_bdapbp.py
--rw-r--r--   0 runner    (1001) docker     (123)     9190 2023-07-02 21:21:34.000000 atmoswing-vigicrues-1.1.5/src/atmoswing_vigicrues/postactions/export_prv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-07-02 21:21:34.000000 atmoswing-vigicrues-1.1.5/src/atmoswing_vigicrues/postactions/postaction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 21:21:55.451140 atmoswing-vigicrues-1.1.5/src/atmoswing_vigicrues/preactions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 21:21:34.000000 atmoswing-vigicrues-1.1.5/src/atmoswing_vigicrues/preactions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9156 2023-07-02 21:21:34.000000 atmoswing-vigicrues-1.1.5/src/atmoswing_vigicrues/preactions/download_gfs.py
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-07-02 21:21:34.000000 atmoswing-vigicrues-1.1.5/src/atmoswing_vigicrues/preactions/preaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     9208 2023-07-02 21:21:34.000000 atmoswing-vigicrues-1.1.5/src/atmoswing_vigicrues/preactions/transfer_sftp_in.py
--rw-r--r--   0 runner    (1001) docker     (123)     3994 2023-07-02 21:21:34.000000 atmoswing-vigicrues-1.1.5/src/atmoswing_vigicrues/preactions/transform_ecmwf.py
--rw-r--r--   0 runner    (1001) docker     (123)     4035 2023-07-02 21:21:34.000000 atmoswing-vigicrues-1.1.5/src/atmoswing_vigicrues/preactions/transform_gfs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6156 2023-07-02 21:21:34.000000 atmoswing-vigicrues-1.1.5/src/atmoswing_vigicrues/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 21:21:55.447140 atmoswing-vigicrues-1.1.5/src/atmoswing_vigicrues.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-07-02 21:21:55.000000 atmoswing-vigicrues-1.1.5/src/atmoswing_vigicrues.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-07-02 21:21:55.000000 atmoswing-vigicrues-1.1.5/src/atmoswing_vigicrues.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 21:21:55.000000 atmoswing-vigicrues-1.1.5/src/atmoswing_vigicrues.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-02 21:21:55.000000 atmoswing-vigicrues-1.1.5/src/atmoswing_vigicrues.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-02 21:21:55.000000 atmoswing-vigicrues-1.1.5/src/atmoswing_vigicrues.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 21:21:55.451140 atmoswing-vigicrues-1.1.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6878 2023-07-02 21:21:34.000000 atmoswing-vigicrues-1.1.5/tests/test_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-07-02 21:21:34.000000 atmoswing-vigicrues-1.1.5/tests/test_download_gfs.py
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-07-02 21:21:34.000000 atmoswing-vigicrues-1.1.5/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-07-02 21:21:34.000000 atmoswing-vigicrues-1.1.5/tests/test_export_bdapbp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-07-02 21:21:34.000000 atmoswing-vigicrues-1.1.5/tests/test_export_prv.py
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-02 21:21:34.000000 atmoswing-vigicrues-1.1.5/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-07-02 21:21:34.000000 atmoswing-vigicrues-1.1.5/tests/test_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-07-02 21:21:34.000000 atmoswing-vigicrues-1.1.5/tests/test_transfer_sftp_in.py
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-07-02 21:21:34.000000 atmoswing-vigicrues-1.1.5/tests/test_transfer_sftp_out.py
--rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-07-02 21:21:34.000000 atmoswing-vigicrues-1.1.5/tests/test_transform_ecmwf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-07-02 21:21:34.000000 atmoswing-vigicrues-1.1.5/tests/test_transform_gfs.py
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-02 21:21:34.000000 atmoswing-vigicrues-1.1.5/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 11:09:52.346074 atmoswing-vigicrues-1.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-08-04 11:09:28.000000 atmoswing-vigicrues-1.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-08-04 11:09:52.346074 atmoswing-vigicrues-1.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-08-04 11:09:28.000000 atmoswing-vigicrues-1.1.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-08-04 11:09:28.000000 atmoswing-vigicrues-1.1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-08-04 11:09:52.346074 atmoswing-vigicrues-1.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-08-04 11:09:28.000000 atmoswing-vigicrues-1.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 11:09:52.338074 atmoswing-vigicrues-1.1.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 11:09:52.342074 atmoswing-vigicrues-1.1.6/src/atmoswing_vigicrues/
+-rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-08-04 11:09:28.000000 atmoswing-vigicrues-1.1.6/src/atmoswing_vigicrues/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-08-04 11:09:28.000000 atmoswing-vigicrues-1.1.6/src/atmoswing_vigicrues/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12089 2023-08-04 11:09:28.000000 atmoswing-vigicrues-1.1.6/src/atmoswing_vigicrues/controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 11:09:52.342074 atmoswing-vigicrues-1.1.6/src/atmoswing_vigicrues/disseminations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:09:28.000000 atmoswing-vigicrues-1.1.6/src/atmoswing_vigicrues/disseminations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-08-04 11:09:28.000000 atmoswing-vigicrues-1.1.6/src/atmoswing_vigicrues/disseminations/dissemination.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5662 2023-08-04 11:09:28.000000 atmoswing-vigicrues-1.1.6/src/atmoswing_vigicrues/disseminations/transfer_sftp_out.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-08-04 11:09:28.000000 atmoswing-vigicrues-1.1.6/src/atmoswing_vigicrues/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-08-04 11:09:28.000000 atmoswing-vigicrues-1.1.6/src/atmoswing_vigicrues/options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 11:09:52.342074 atmoswing-vigicrues-1.1.6/src/atmoswing_vigicrues/postactions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:09:28.000000 atmoswing-vigicrues-1.1.6/src/atmoswing_vigicrues/postactions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13301 2023-08-04 11:09:28.000000 atmoswing-vigicrues-1.1.6/src/atmoswing_vigicrues/postactions/export_bdapbp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9190 2023-08-04 11:09:28.000000 atmoswing-vigicrues-1.1.6/src/atmoswing_vigicrues/postactions/export_prv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-08-04 11:09:28.000000 atmoswing-vigicrues-1.1.6/src/atmoswing_vigicrues/postactions/postaction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 11:09:52.342074 atmoswing-vigicrues-1.1.6/src/atmoswing_vigicrues/preactions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:09:28.000000 atmoswing-vigicrues-1.1.6/src/atmoswing_vigicrues/preactions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9815 2023-08-04 11:09:28.000000 atmoswing-vigicrues-1.1.6/src/atmoswing_vigicrues/preactions/download_gfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-08-04 11:09:28.000000 atmoswing-vigicrues-1.1.6/src/atmoswing_vigicrues/preactions/preaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9208 2023-08-04 11:09:28.000000 atmoswing-vigicrues-1.1.6/src/atmoswing_vigicrues/preactions/transfer_sftp_in.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3994 2023-08-04 11:09:28.000000 atmoswing-vigicrues-1.1.6/src/atmoswing_vigicrues/preactions/transform_ecmwf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4035 2023-08-04 11:09:28.000000 atmoswing-vigicrues-1.1.6/src/atmoswing_vigicrues/preactions/transform_gfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6156 2023-08-04 11:09:28.000000 atmoswing-vigicrues-1.1.6/src/atmoswing_vigicrues/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 11:09:52.342074 atmoswing-vigicrues-1.1.6/src/atmoswing_vigicrues.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-08-04 11:09:52.000000 atmoswing-vigicrues-1.1.6/src/atmoswing_vigicrues.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-08-04 11:09:52.000000 atmoswing-vigicrues-1.1.6/src/atmoswing_vigicrues.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 11:09:52.000000 atmoswing-vigicrues-1.1.6/src/atmoswing_vigicrues.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-08-04 11:09:52.000000 atmoswing-vigicrues-1.1.6/src/atmoswing_vigicrues.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-04 11:09:52.000000 atmoswing-vigicrues-1.1.6/src/atmoswing_vigicrues.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 11:09:52.346074 atmoswing-vigicrues-1.1.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6878 2023-08-04 11:09:28.000000 atmoswing-vigicrues-1.1.6/tests/test_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-08-04 11:09:28.000000 atmoswing-vigicrues-1.1.6/tests/test_download_gfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-08-04 11:09:28.000000 atmoswing-vigicrues-1.1.6/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-08-04 11:09:28.000000 atmoswing-vigicrues-1.1.6/tests/test_export_bdapbp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-08-04 11:09:28.000000 atmoswing-vigicrues-1.1.6/tests/test_export_prv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-08-04 11:09:28.000000 atmoswing-vigicrues-1.1.6/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-08-04 11:09:28.000000 atmoswing-vigicrues-1.1.6/tests/test_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-08-04 11:09:28.000000 atmoswing-vigicrues-1.1.6/tests/test_transfer_sftp_in.py
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-08-04 11:09:28.000000 atmoswing-vigicrues-1.1.6/tests/test_transfer_sftp_out.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-08-04 11:09:28.000000 atmoswing-vigicrues-1.1.6/tests/test_transform_ecmwf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-08-04 11:09:28.000000 atmoswing-vigicrues-1.1.6/tests/test_transform_gfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-08-04 11:09:28.000000 atmoswing-vigicrues-1.1.6/tests/test_utils.py
```

### Comparing `atmoswing-vigicrues-1.1.5/LICENSE` & `atmoswing-vigicrues-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.1.5/PKG-INFO` & `atmoswing-vigicrues-1.1.6/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 Metadata-Version: 2.1
 Name: atmoswing-vigicrues
-Version: 1.1.5
+Version: 1.1.6
 Summary: Package to integrate AtmoSwing in the Vigicrues network.
 Author: Pascal Horton
 Author-email: Pascal Horton <pascal.horton@terranum.ch>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: tests
 License-File: LICENSE
 
 # atmoswing-vigicrues
 
+[![GitHub release](https://img.shields.io/github/v/release/atmoswing/atmoswing-vigicrues)](https://github.com/atmoswing/atmoswing-vigicrues)
+[![PyPI](https://img.shields.io/pypi/v/atmoswing-vigicrues)](https://pypi.org/project/atmoswing-vigicrues/)
+[![Docker Image Version](https://img.shields.io/docker/v/atmoswing/atmoswing-vigicrues)](https://hub.docker.com/r/atmoswing/atmoswing-vigicrues)
+![Static Badge](https://img.shields.io/badge/python-%3E%3D3.7-blue)
+   
 Module Python pour l'intégration d'AtmoSwing dans le réseau Vigicrues.
 
 Documentation API: http://atmoswing.org/atmoswing-vigicrues
 
 
 Objectif
 --------
@@ -41,15 +46,19 @@
 * AtmoSwing Forecaster (de préférence la version serveur)
 * Le module atmoswing-vigicrues (``pip install atmoswing-vigicrues`` ou l'image docker ``docker pull atmoswing/atmoswing-vigicrues``)
 
 Utilisation
 -----------
 
 Le paquet est constitué de plusieurs modules qui peuvent être activés et configurés dans un fichier de configuration. Plusieurs flux de prévision peuvent être configurés sur un serveur / PC par la création de différents fichiers de configuration. Il n’y a pas de paramètres codés en dur dans le code. L’exécution d’un flux de prévision est effectuée par la commande :
-``python -m atmoswing_vigicrues --config-file="chemin/vers/fichier/config.yaml``
+
+```
+python -m atmoswing_vigicrues --config-file="chemin/vers/fichier/config.yaml
+```
+
 Le fichier de configuration définit :
 
 * Les propriétés de la prévision par AtmoSwing
 * Les pré-actions : les actions à effectuer préalablement à la prévision par AtmoSwing
 * Les post-actions : les actions à effectuer après la prévision par AtmoSwing
 * Les disséminations : les actions de transfert des résultats
```

### Comparing `atmoswing-vigicrues-1.1.5/README.md` & `atmoswing-vigicrues-1.1.6/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 # atmoswing-vigicrues
 
+[![GitHub release](https://img.shields.io/github/v/release/atmoswing/atmoswing-vigicrues)](https://github.com/atmoswing/atmoswing-vigicrues)
+[![PyPI](https://img.shields.io/pypi/v/atmoswing-vigicrues)](https://pypi.org/project/atmoswing-vigicrues/)
+[![Docker Image Version](https://img.shields.io/docker/v/atmoswing/atmoswing-vigicrues)](https://hub.docker.com/r/atmoswing/atmoswing-vigicrues)
+![Static Badge](https://img.shields.io/badge/python-%3E%3D3.7-blue)
+   
 Module Python pour l'intégration d'AtmoSwing dans le réseau Vigicrues.
 
 Documentation API: http://atmoswing.org/atmoswing-vigicrues
 
 
 Objectif
 --------
@@ -26,15 +31,19 @@
 * AtmoSwing Forecaster (de préférence la version serveur)
 * Le module atmoswing-vigicrues (``pip install atmoswing-vigicrues`` ou l'image docker ``docker pull atmoswing/atmoswing-vigicrues``)
 
 Utilisation
 -----------
 
 Le paquet est constitué de plusieurs modules qui peuvent être activés et configurés dans un fichier de configuration. Plusieurs flux de prévision peuvent être configurés sur un serveur / PC par la création de différents fichiers de configuration. Il n’y a pas de paramètres codés en dur dans le code. L’exécution d’un flux de prévision est effectuée par la commande :
-``python -m atmoswing_vigicrues --config-file="chemin/vers/fichier/config.yaml``
+
+```
+python -m atmoswing_vigicrues --config-file="chemin/vers/fichier/config.yaml
+```
+
 Le fichier de configuration définit :
 
 * Les propriétés de la prévision par AtmoSwing
 * Les pré-actions : les actions à effectuer préalablement à la prévision par AtmoSwing
 * Les post-actions : les actions à effectuer après la prévision par AtmoSwing
 * Les disséminations : les actions de transfert des résultats
```

### Comparing `atmoswing-vigicrues-1.1.5/pyproject.toml` & `atmoswing-vigicrues-1.1.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "atmoswing-vigicrues"
-version = "1.1.5"
+version = "1.1.6"
 authors = [
   { name="Pascal Horton", email="pascal.horton@terranum.ch" },
 ]
 description = "Package to integrate AtmoSwing in the Vigicrues network."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `atmoswing-vigicrues-1.1.5/src/atmoswing_vigicrues/__init__.py` & `atmoswing-vigicrues-1.1.6/src/atmoswing_vigicrues/__init__.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.1.5/src/atmoswing_vigicrues/__main__.py` & `atmoswing-vigicrues-1.1.6/src/atmoswing_vigicrues/__main__.py`

 * *Files 21% similar despite different names*

```diff
@@ -10,14 +10,17 @@
                     "le réseau Vigicrues.")
     parser.add_argument(
         '-c', '--config-file', type=str, required=False,
         help="Fichier de configuration du présent module.")
     parser.add_argument(
         '-d', '--date', type=str, required=False,
         help="Date pour laquelle émettre une prévision (YYYYMMDDHH).")
+    parser.add_argument(
+        '-i', '--time-increment', type=int, required=False,
+        help="Incrément en heures pour l'émission de la prévision (par défaut 6h).")
 
     args = parser.parse_args(args)
 
     controller = Controller(args)
 
     if args.date:
         date = datetime.strptime(args.date, '%Y%m%d%H')
```

### Comparing `atmoswing-vigicrues-1.1.5/src/atmoswing_vigicrues/controller.py` & `atmoswing-vigicrues-1.1.6/src/atmoswing_vigicrues/controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,14 +41,17 @@
 
     def __init__(self, cli_options):
         """
         Initialisation de l'instance Controller
         """
         self.options = asv.Options(cli_options)
         self.time_increment = 6
+        if hasattr(cli_options, 'time_increment') and \
+                cli_options.time_increment is not None:
+            self.time_increment = cli_options.time_increment
         self.date = datetime.datetime.utcnow()
         self.existing_files = []
         self.pre_actions = []
         self.post_actions = []
         self.disseminations = []
         self._register_pre_actions()
         self._register_post_actions()
```

### Comparing `atmoswing-vigicrues-1.1.5/src/atmoswing_vigicrues/disseminations/dissemination.py` & `atmoswing-vigicrues-1.1.6/src/atmoswing_vigicrues/disseminations/dissemination.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.1.5/src/atmoswing_vigicrues/disseminations/transfer_sftp_out.py` & `atmoswing-vigicrues-1.1.6/src/atmoswing_vigicrues/disseminations/transfer_sftp_out.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.1.5/src/atmoswing_vigicrues/exceptions.py` & `atmoswing-vigicrues-1.1.6/src/atmoswing_vigicrues/exceptions.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.1.5/src/atmoswing_vigicrues/options.py` & `atmoswing-vigicrues-1.1.6/src/atmoswing_vigicrues/options.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.1.5/src/atmoswing_vigicrues/postactions/export_bdapbp.py` & `atmoswing-vigicrues-1.1.6/src/atmoswing_vigicrues/postactions/export_bdapbp.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.1.5/src/atmoswing_vigicrues/postactions/export_prv.py` & `atmoswing-vigicrues-1.1.6/src/atmoswing_vigicrues/postactions/export_prv.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.1.5/src/atmoswing_vigicrues/postactions/postaction.py` & `atmoswing-vigicrues-1.1.6/src/atmoswing_vigicrues/postactions/postaction.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.1.5/src/atmoswing_vigicrues/preactions/download_gfs.py` & `atmoswing-vigicrues-1.1.6/src/atmoswing_vigicrues/preactions/download_gfs.py`

 * *Files 7% similar despite different names*

```diff
@@ -43,14 +43,22 @@
             L'adresse du proxy (si nécessaire). Format : proxy_ip:proxy_port
         * proxy_user : str
             L'utilisateur et le mot de passe pour le proxy. Format : username:password
         * attempts_max_hours : int
             Décalage temporel autorisé pour rechercher d'anciens fichiers
         * attempts_step_hours : int
             Pas de temps auquel décrémenter la date pour rechercher d'anciens fichiers
+            lorsque le fichier n'est pas trouvé
+        * time_increment : int
+            Pas de temps auquel décrémenter la date pour rechercher d'anciens fichiers
+            afin de compléter les fichiers précédents de la journée
+            Valeur par défaut : 6
+        * time_step_back : int
+            Nombre de pas de temps autorisé pour rechercher d'anciens fichiers
+            Valeur par défaut : 4
 
     Attributes
     ----------
     type_name : str
         Le nom du type de l'action
     name : str
         Le nom de l'action
@@ -124,16 +132,23 @@
             proxies = options['proxies']
             for key in proxies:
                 if proxies[key]:
                     self.proxies = proxies
                     continue
 
         # Télécharge également les 4 pas de temps précédents (pas de temps de 6 h)
-        self.time_increment = 6
-        self.time_step_back = 4
+        if 'time_increment' in options:
+            self.time_increment = options['time_increment']
+        else:
+            self.time_increment = 6
+
+        if 'time_step_back' in options:
+            self.time_step_back = options['time_step_back']
+        else:
+            self.time_step_back = 4
 
         super().__init__()
 
     def run(self, date) -> bool:
         """
         Exécute l'action.
```

### Comparing `atmoswing-vigicrues-1.1.5/src/atmoswing_vigicrues/preactions/preaction.py` & `atmoswing-vigicrues-1.1.6/src/atmoswing_vigicrues/preactions/preaction.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.1.5/src/atmoswing_vigicrues/preactions/transfer_sftp_in.py` & `atmoswing-vigicrues-1.1.6/src/atmoswing_vigicrues/preactions/transfer_sftp_in.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.1.5/src/atmoswing_vigicrues/preactions/transform_ecmwf.py` & `atmoswing-vigicrues-1.1.6/src/atmoswing_vigicrues/preactions/transform_ecmwf.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.1.5/src/atmoswing_vigicrues/preactions/transform_gfs.py` & `atmoswing-vigicrues-1.1.6/src/atmoswing_vigicrues/preactions/transform_gfs.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.1.5/src/atmoswing_vigicrues/utils.py` & `atmoswing-vigicrues-1.1.6/src/atmoswing_vigicrues/utils.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.1.5/src/atmoswing_vigicrues.egg-info/PKG-INFO` & `atmoswing-vigicrues-1.1.6/src/atmoswing_vigicrues.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 Metadata-Version: 2.1
 Name: atmoswing-vigicrues
-Version: 1.1.5
+Version: 1.1.6
 Summary: Package to integrate AtmoSwing in the Vigicrues network.
 Author: Pascal Horton
 Author-email: Pascal Horton <pascal.horton@terranum.ch>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: tests
 License-File: LICENSE
 
 # atmoswing-vigicrues
 
+[![GitHub release](https://img.shields.io/github/v/release/atmoswing/atmoswing-vigicrues)](https://github.com/atmoswing/atmoswing-vigicrues)
+[![PyPI](https://img.shields.io/pypi/v/atmoswing-vigicrues)](https://pypi.org/project/atmoswing-vigicrues/)
+[![Docker Image Version](https://img.shields.io/docker/v/atmoswing/atmoswing-vigicrues)](https://hub.docker.com/r/atmoswing/atmoswing-vigicrues)
+![Static Badge](https://img.shields.io/badge/python-%3E%3D3.7-blue)
+   
 Module Python pour l'intégration d'AtmoSwing dans le réseau Vigicrues.
 
 Documentation API: http://atmoswing.org/atmoswing-vigicrues
 
 
 Objectif
 --------
@@ -41,15 +46,19 @@
 * AtmoSwing Forecaster (de préférence la version serveur)
 * Le module atmoswing-vigicrues (``pip install atmoswing-vigicrues`` ou l'image docker ``docker pull atmoswing/atmoswing-vigicrues``)
 
 Utilisation
 -----------
 
 Le paquet est constitué de plusieurs modules qui peuvent être activés et configurés dans un fichier de configuration. Plusieurs flux de prévision peuvent être configurés sur un serveur / PC par la création de différents fichiers de configuration. Il n’y a pas de paramètres codés en dur dans le code. L’exécution d’un flux de prévision est effectuée par la commande :
-``python -m atmoswing_vigicrues --config-file="chemin/vers/fichier/config.yaml``
+
+```
+python -m atmoswing_vigicrues --config-file="chemin/vers/fichier/config.yaml
+```
+
 Le fichier de configuration définit :
 
 * Les propriétés de la prévision par AtmoSwing
 * Les pré-actions : les actions à effectuer préalablement à la prévision par AtmoSwing
 * Les post-actions : les actions à effectuer après la prévision par AtmoSwing
 * Les disséminations : les actions de transfert des résultats
```

### Comparing `atmoswing-vigicrues-1.1.5/src/atmoswing_vigicrues.egg-info/SOURCES.txt` & `atmoswing-vigicrues-1.1.6/src/atmoswing_vigicrues.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.1.5/tests/test_controller.py` & `atmoswing-vigicrues-1.1.6/tests/test_controller.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.1.5/tests/test_download_gfs.py` & `atmoswing-vigicrues-1.1.6/tests/test_download_gfs.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.1.5/tests/test_exceptions.py` & `atmoswing-vigicrues-1.1.6/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.1.5/tests/test_export_bdapbp.py` & `atmoswing-vigicrues-1.1.6/tests/test_export_bdapbp.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.1.5/tests/test_export_prv.py` & `atmoswing-vigicrues-1.1.6/tests/test_export_prv.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.1.5/tests/test_options.py` & `atmoswing-vigicrues-1.1.6/tests/test_options.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.1.5/tests/test_transfer_sftp_in.py` & `atmoswing-vigicrues-1.1.6/tests/test_transfer_sftp_in.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.1.5/tests/test_transfer_sftp_out.py` & `atmoswing-vigicrues-1.1.6/tests/test_transfer_sftp_out.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.1.5/tests/test_transform_ecmwf.py` & `atmoswing-vigicrues-1.1.6/tests/test_transform_ecmwf.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.1.5/tests/test_transform_gfs.py` & `atmoswing-vigicrues-1.1.6/tests/test_transform_gfs.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.1.5/tests/test_utils.py` & `atmoswing-vigicrues-1.1.6/tests/test_utils.py`

 * *Files identical despite different names*

