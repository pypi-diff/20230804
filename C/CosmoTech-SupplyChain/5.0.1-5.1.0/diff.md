# Comparing `tmp/CosmoTech-SupplyChain-5.0.1.tar.gz` & `tmp/CosmoTech-SupplyChain-5.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CosmoTech-SupplyChain-5.0.1.tar", last modified: Tue Jul 11 13:07:49 2023, max compression
+gzip compressed data, was "CosmoTech-SupplyChain-5.1.0.tar", last modified: Fri Aug  4 10:32:30 2023, max compression
```

## Comparing `CosmoTech-SupplyChain-5.0.1.tar` & `CosmoTech-SupplyChain-5.1.0.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 13:07:49.041760 CosmoTech-SupplyChain-5.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 13:07:49.033760 CosmoTech-SupplyChain-5.0.1/CosmoTech_SupplyChain.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      323 2023-07-11 13:07:49.000000 CosmoTech-SupplyChain-5.0.1/CosmoTech_SupplyChain.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2332 2023-07-11 13:07:49.000000 CosmoTech-SupplyChain-5.0.1/CosmoTech_SupplyChain.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-11 13:07:49.000000 CosmoTech-SupplyChain-5.0.1/CosmoTech_SupplyChain.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      216 2023-07-11 13:07:49.000000 CosmoTech-SupplyChain-5.0.1/CosmoTech_SupplyChain.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       12 2023-07-11 13:07:49.000000 CosmoTech-SupplyChain-5.0.1/CosmoTech_SupplyChain.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1195 2023-07-11 13:07:40.000000 CosmoTech-SupplyChain-5.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      323 2023-07-11 13:07:49.041760 CosmoTech-SupplyChain-5.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3447 2023-07-11 13:07:40.000000 CosmoTech-SupplyChain-5.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 13:07:49.033760 CosmoTech-SupplyChain-5.0.1/Supplychain/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 13:07:49.037760 CosmoTech-SupplyChain-5.0.1/Supplychain/Generic/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-11 13:07:40.000000 CosmoTech-SupplyChain-5.0.1/Supplychain/Generic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3344 2023-07-11 13:07:40.000000 CosmoTech-SupplyChain-5.0.1/Supplychain/Generic/adt_writer.py
--rw-r--r--   0 runner    (1001) docker     (122)     1488 2023-07-11 13:07:40.000000 CosmoTech-SupplyChain-5.0.1/Supplychain/Generic/adx_and_file_writer.py
--rw-r--r--   0 runner    (1001) docker     (122)     6620 2023-07-11 13:07:40.000000 CosmoTech-SupplyChain-5.0.1/Supplychain/Generic/adx_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (122)     4451 2023-07-11 13:07:40.000000 CosmoTech-SupplyChain-5.0.1/Supplychain/Generic/cosmo_api_parameters.py
--rw-r--r--   0 runner    (1001) docker     (122)     3385 2023-07-11 13:07:40.000000 CosmoTech-SupplyChain-5.0.1/Supplychain/Generic/csv_folder_reader.py
--rw-r--r--   0 runner    (1001) docker     (122)     1282 2023-07-11 13:07:40.000000 CosmoTech-SupplyChain-5.0.1/Supplychain/Generic/csv_folder_writer.py
--rw-r--r--   0 runner    (1001) docker     (122)      694 2023-07-11 13:07:40.000000 CosmoTech-SupplyChain-5.0.1/Supplychain/Generic/duration.py
--rw-r--r--   0 runner    (1001) docker     (122)     1908 2023-07-11 13:07:40.000000 CosmoTech-SupplyChain-5.0.1/Supplychain/Generic/excel_folder_reader.py
--rw-r--r--   0 runner    (1001) docker     (122)     1710 2023-07-11 13:07:40.000000 CosmoTech-SupplyChain-5.0.1/Supplychain/Generic/excel_folder_writer.py
--rw-r--r--   0 runner    (1001) docker     (122)     1287 2023-07-11 13:07:40.000000 CosmoTech-SupplyChain-5.0.1/Supplychain/Generic/folder_io.py
--rw-r--r--   0 runner    (1001) docker     (122)     1460 2023-07-11 13:07:40.000000 CosmoTech-SupplyChain-5.0.1/Supplychain/Generic/json_folder_reader.py
--rw-r--r--   0 runner    (1001) docker     (122)      780 2023-07-11 13:07:40.000000 CosmoTech-SupplyChain-5.0.1/Supplychain/Generic/json_folder_writer.py
--rw-r--r--   0 runner    (1001) docker     (122)      682 2023-07-11 13:07:40.000000 CosmoTech-SupplyChain-5.0.1/Supplychain/Generic/memory_folder_io.py
--rw-r--r--   0 runner    (1001) docker     (122)      679 2023-07-11 13:07:40.000000 CosmoTech-SupplyChain-5.0.1/Supplychain/Generic/simulator_io.py
--rw-r--r--   0 runner    (1001) docker     (122)      869 2023-07-11 13:07:40.000000 CosmoTech-SupplyChain-5.0.1/Supplychain/Generic/storage_queue_writer.py
--rw-r--r--   0 runner    (1001) docker     (122)     2935 2023-07-11 13:07:40.000000 CosmoTech-SupplyChain-5.0.1/Supplychain/Generic/timer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 13:07:49.037760 CosmoTech-SupplyChain-5.0.1/Supplychain/Protocol/
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-11 13:07:40.000000 CosmoTech-SupplyChain-5.0.1/Supplychain/Protocol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1101 2023-07-11 13:07:40.000000 CosmoTech-SupplyChain-5.0.1/Supplychain/Protocol/cmaes_optimization_algorithm.py
--rw-r--r--   0 runner    (1001) docker     (122)     7621 2023-07-11 13:07:40.000000 CosmoTech-SupplyChain-5.0.1/Supplychain/Protocol/default_transformation.py
--rw-r--r--   0 runner    (1001) docker     (122)     4276 2023-07-11 13:07:40.000000 CosmoTech-SupplyChain-5.0.1/Supplychain/Protocol/multiprocessing_optimization.py
--rw-r--r--   0 runner    (1001) docker     (122)      761 2023-07-11 13:07:40.000000 CosmoTech-SupplyChain-5.0.1/Supplychain/Protocol/objective_functions.py
--rw-r--r--   0 runner    (1001) docker     (122)     2044 2023-07-11 13:07:40.000000 CosmoTech-SupplyChain-5.0.1/Supplychain/Protocol/protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 13:07:49.037760 CosmoTech-SupplyChain-5.0.1/Supplychain/Run/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-11 13:07:40.000000 CosmoTech-SupplyChain-5.0.1/Supplychain/Run/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5391 2023-07-11 13:07:40.000000 CosmoTech-SupplyChain-5.0.1/Supplychain/Run/cmaes_optimization.py
--rw-r--r--   0 runner    (1001) docker     (122)     3232 2023-07-11 13:07:40.000000 CosmoTech-SupplyChain-5.0.1/Supplychain/Run/consumers.py
--rw-r--r--   0 runner    (1001) docker     (122)    31357 2023-07-11 13:07:40.000000 CosmoTech-SupplyChain-5.0.1/Supplychain/Run/local_sensitivity_analysis_comets.py
--rw-r--r--   0 runner    (1001) docker     (122)      962 2023-07-11 13:07:40.000000 CosmoTech-SupplyChain-5.0.1/Supplychain/Run/simulation.py
--rw-r--r--   0 runner    (1001) docker     (122)     1025 2023-07-11 13:07:40.000000 CosmoTech-SupplyChain-5.0.1/Supplychain/Run/simulation_comets.py
--rw-r--r--   0 runner    (1001) docker     (122)    20691 2023-07-11 13:07:40.000000 CosmoTech-SupplyChain-5.0.1/Supplychain/Run/stochastic_optimization.py
--rw-r--r--   0 runner    (1001) docker     (122)     7760 2023-07-11 13:07:40.000000 CosmoTech-SupplyChain-5.0.1/Supplychain/Run/uncertainty_analysis.py
--rw-r--r--   0 runner    (1001) docker     (122)    23910 2023-07-11 13:07:40.000000 CosmoTech-SupplyChain-5.0.1/Supplychain/Run/uncertainty_analysis_comets.py
--rw-r--r--   0 runner    (1001) docker     (122)    22140 2023-07-11 13:07:40.000000 CosmoTech-SupplyChain-5.0.1/Supplychain/Run/uncertainty_analysis_helper_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 13:07:49.037760 CosmoTech-SupplyChain-5.0.1/Supplychain/Schema/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-11 13:07:40.000000 CosmoTech-SupplyChain-5.0.1/Supplychain/Schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6223 2023-07-11 13:07:40.000000 CosmoTech-SupplyChain-5.0.1/Supplychain/Schema/adt_column_description.py
--rw-r--r--   0 runner    (1001) docker     (122)     5318 2023-07-11 13:07:40.000000 CosmoTech-SupplyChain-5.0.1/Supplychain/Schema/default_values.py
--rw-r--r--   0 runner    (1001) docker     (122)     3149 2023-07-11 13:07:40.000000 CosmoTech-SupplyChain-5.0.1/Supplychain/Schema/simulator_files_description.py
--rw-r--r--   0 runner    (1001) docker     (122)    23192 2023-07-11 13:07:40.000000 CosmoTech-SupplyChain-5.0.1/Supplychain/Schema/validation_schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 13:07:49.037760 CosmoTech-SupplyChain-5.0.1/Supplychain/Transform/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-11 13:07:40.000000 CosmoTech-SupplyChain-5.0.1/Supplychain/Transform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6539 2023-07-11 13:07:40.000000 CosmoTech-SupplyChain-5.0.1/Supplychain/Transform/complete_dict.py
--rw-r--r--   0 runner    (1001) docker     (122)    39924 2023-07-11 13:07:40.000000 CosmoTech-SupplyChain-5.0.1/Supplychain/Transform/from_dict_to_simulator.py
--rw-r--r--   0 runner    (1001) docker     (122)    11669 2023-07-11 13:07:40.000000 CosmoTech-SupplyChain-5.0.1/Supplychain/Transform/from_dict_to_table.py
--rw-r--r--   0 runner    (1001) docker     (122)     6822 2023-07-11 13:07:40.000000 CosmoTech-SupplyChain-5.0.1/Supplychain/Transform/from_table_to_dict.py
--rw-r--r--   0 runner    (1001) docker     (122)    52415 2023-07-11 13:07:40.000000 CosmoTech-SupplyChain-5.0.1/Supplychain/Transform/from_table_to_dict_old.py
--rw-r--r--   0 runner    (1001) docker     (122)    15664 2023-07-11 13:07:40.000000 CosmoTech-SupplyChain-5.0.1/Supplychain/Transform/patch_dict_with_parameters.py
--rw-r--r--   0 runner    (1001) docker     (122)     3080 2023-07-11 13:07:40.000000 CosmoTech-SupplyChain-5.0.1/Supplychain/Transform/production_route.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 13:07:49.041760 CosmoTech-SupplyChain-5.0.1/Supplychain/Validate/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-11 13:07:40.000000 CosmoTech-SupplyChain-5.0.1/Supplychain/Validate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    21965 2023-07-11 13:07:40.000000 CosmoTech-SupplyChain-5.0.1/Supplychain/Validate/validate_dict.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 13:07:49.041760 CosmoTech-SupplyChain-5.0.1/Supplychain/Wrappers/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-11 13:07:40.000000 CosmoTech-SupplyChain-5.0.1/Supplychain/Wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1646 2023-07-11 13:07:40.000000 CosmoTech-SupplyChain-5.0.1/Supplychain/Wrappers/environment_variables.py
--rw-r--r--   0 runner    (1001) docker     (122)    18535 2023-07-11 13:07:40.000000 CosmoTech-SupplyChain-5.0.1/Supplychain/Wrappers/simulator.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-11 13:07:40.000000 CosmoTech-SupplyChain-5.0.1/Supplychain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-11 13:07:49.041760 CosmoTech-SupplyChain-5.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      851 2023-07-11 13:07:40.000000 CosmoTech-SupplyChain-5.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 10:32:30.734869 CosmoTech-SupplyChain-5.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 10:32:30.726869 CosmoTech-SupplyChain-5.1.0/CosmoTech_SupplyChain.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      323 2023-08-04 10:32:30.000000 CosmoTech-SupplyChain-5.1.0/CosmoTech_SupplyChain.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2332 2023-08-04 10:32:30.000000 CosmoTech-SupplyChain-5.1.0/CosmoTech_SupplyChain.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-04 10:32:30.000000 CosmoTech-SupplyChain-5.1.0/CosmoTech_SupplyChain.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      216 2023-08-04 10:32:30.000000 CosmoTech-SupplyChain-5.1.0/CosmoTech_SupplyChain.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2023-08-04 10:32:30.000000 CosmoTech-SupplyChain-5.1.0/CosmoTech_SupplyChain.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1195 2023-08-04 10:32:20.000000 CosmoTech-SupplyChain-5.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      323 2023-08-04 10:32:30.734869 CosmoTech-SupplyChain-5.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3447 2023-08-04 10:32:20.000000 CosmoTech-SupplyChain-5.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 10:32:30.726869 CosmoTech-SupplyChain-5.1.0/Supplychain/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 10:32:30.730869 CosmoTech-SupplyChain-5.1.0/Supplychain/Generic/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-04 10:32:20.000000 CosmoTech-SupplyChain-5.1.0/Supplychain/Generic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3344 2023-08-04 10:32:20.000000 CosmoTech-SupplyChain-5.1.0/Supplychain/Generic/adt_writer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1488 2023-08-04 10:32:20.000000 CosmoTech-SupplyChain-5.1.0/Supplychain/Generic/adx_and_file_writer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6620 2023-08-04 10:32:20.000000 CosmoTech-SupplyChain-5.1.0/Supplychain/Generic/adx_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4451 2023-08-04 10:32:20.000000 CosmoTech-SupplyChain-5.1.0/Supplychain/Generic/cosmo_api_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3385 2023-08-04 10:32:20.000000 CosmoTech-SupplyChain-5.1.0/Supplychain/Generic/csv_folder_reader.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1282 2023-08-04 10:32:20.000000 CosmoTech-SupplyChain-5.1.0/Supplychain/Generic/csv_folder_writer.py
+-rw-r--r--   0 runner    (1001) docker     (122)      694 2023-08-04 10:32:20.000000 CosmoTech-SupplyChain-5.1.0/Supplychain/Generic/duration.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1908 2023-08-04 10:32:20.000000 CosmoTech-SupplyChain-5.1.0/Supplychain/Generic/excel_folder_reader.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1710 2023-08-04 10:32:20.000000 CosmoTech-SupplyChain-5.1.0/Supplychain/Generic/excel_folder_writer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1287 2023-08-04 10:32:20.000000 CosmoTech-SupplyChain-5.1.0/Supplychain/Generic/folder_io.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1460 2023-08-04 10:32:20.000000 CosmoTech-SupplyChain-5.1.0/Supplychain/Generic/json_folder_reader.py
+-rw-r--r--   0 runner    (1001) docker     (122)      780 2023-08-04 10:32:20.000000 CosmoTech-SupplyChain-5.1.0/Supplychain/Generic/json_folder_writer.py
+-rw-r--r--   0 runner    (1001) docker     (122)      682 2023-08-04 10:32:20.000000 CosmoTech-SupplyChain-5.1.0/Supplychain/Generic/memory_folder_io.py
+-rw-r--r--   0 runner    (1001) docker     (122)      679 2023-08-04 10:32:20.000000 CosmoTech-SupplyChain-5.1.0/Supplychain/Generic/simulator_io.py
+-rw-r--r--   0 runner    (1001) docker     (122)      869 2023-08-04 10:32:20.000000 CosmoTech-SupplyChain-5.1.0/Supplychain/Generic/storage_queue_writer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2935 2023-08-04 10:32:20.000000 CosmoTech-SupplyChain-5.1.0/Supplychain/Generic/timer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 10:32:30.730869 CosmoTech-SupplyChain-5.1.0/Supplychain/Protocol/
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-04 10:32:20.000000 CosmoTech-SupplyChain-5.1.0/Supplychain/Protocol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1101 2023-08-04 10:32:20.000000 CosmoTech-SupplyChain-5.1.0/Supplychain/Protocol/cmaes_optimization_algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7621 2023-08-04 10:32:20.000000 CosmoTech-SupplyChain-5.1.0/Supplychain/Protocol/default_transformation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4276 2023-08-04 10:32:20.000000 CosmoTech-SupplyChain-5.1.0/Supplychain/Protocol/multiprocessing_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (122)      761 2023-08-04 10:32:20.000000 CosmoTech-SupplyChain-5.1.0/Supplychain/Protocol/objective_functions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2044 2023-08-04 10:32:20.000000 CosmoTech-SupplyChain-5.1.0/Supplychain/Protocol/protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 10:32:30.734869 CosmoTech-SupplyChain-5.1.0/Supplychain/Run/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-04 10:32:20.000000 CosmoTech-SupplyChain-5.1.0/Supplychain/Run/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5391 2023-08-04 10:32:20.000000 CosmoTech-SupplyChain-5.1.0/Supplychain/Run/cmaes_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3232 2023-08-04 10:32:20.000000 CosmoTech-SupplyChain-5.1.0/Supplychain/Run/consumers.py
+-rw-r--r--   0 runner    (1001) docker     (122)    31650 2023-08-04 10:32:20.000000 CosmoTech-SupplyChain-5.1.0/Supplychain/Run/local_sensitivity_analysis_comets.py
+-rw-r--r--   0 runner    (1001) docker     (122)      962 2023-08-04 10:32:20.000000 CosmoTech-SupplyChain-5.1.0/Supplychain/Run/simulation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1025 2023-08-04 10:32:20.000000 CosmoTech-SupplyChain-5.1.0/Supplychain/Run/simulation_comets.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20824 2023-08-04 10:32:20.000000 CosmoTech-SupplyChain-5.1.0/Supplychain/Run/stochastic_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7760 2023-08-04 10:32:20.000000 CosmoTech-SupplyChain-5.1.0/Supplychain/Run/uncertainty_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23910 2023-08-04 10:32:20.000000 CosmoTech-SupplyChain-5.1.0/Supplychain/Run/uncertainty_analysis_comets.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22140 2023-08-04 10:32:20.000000 CosmoTech-SupplyChain-5.1.0/Supplychain/Run/uncertainty_analysis_helper_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 10:32:30.734869 CosmoTech-SupplyChain-5.1.0/Supplychain/Schema/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-04 10:32:20.000000 CosmoTech-SupplyChain-5.1.0/Supplychain/Schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6277 2023-08-04 10:32:20.000000 CosmoTech-SupplyChain-5.1.0/Supplychain/Schema/adt_column_description.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5371 2023-08-04 10:32:20.000000 CosmoTech-SupplyChain-5.1.0/Supplychain/Schema/default_values.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3195 2023-08-04 10:32:20.000000 CosmoTech-SupplyChain-5.1.0/Supplychain/Schema/simulator_files_description.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23267 2023-08-04 10:32:20.000000 CosmoTech-SupplyChain-5.1.0/Supplychain/Schema/validation_schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 10:32:30.734869 CosmoTech-SupplyChain-5.1.0/Supplychain/Transform/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-04 10:32:20.000000 CosmoTech-SupplyChain-5.1.0/Supplychain/Transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6539 2023-08-04 10:32:20.000000 CosmoTech-SupplyChain-5.1.0/Supplychain/Transform/complete_dict.py
+-rw-r--r--   0 runner    (1001) docker     (122)    40023 2023-08-04 10:32:20.000000 CosmoTech-SupplyChain-5.1.0/Supplychain/Transform/from_dict_to_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11670 2023-08-04 10:32:20.000000 CosmoTech-SupplyChain-5.1.0/Supplychain/Transform/from_dict_to_table.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6822 2023-08-04 10:32:20.000000 CosmoTech-SupplyChain-5.1.0/Supplychain/Transform/from_table_to_dict.py
+-rw-r--r--   0 runner    (1001) docker     (122)    52415 2023-08-04 10:32:20.000000 CosmoTech-SupplyChain-5.1.0/Supplychain/Transform/from_table_to_dict_old.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15664 2023-08-04 10:32:20.000000 CosmoTech-SupplyChain-5.1.0/Supplychain/Transform/patch_dict_with_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3080 2023-08-04 10:32:20.000000 CosmoTech-SupplyChain-5.1.0/Supplychain/Transform/production_route.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 10:32:30.734869 CosmoTech-SupplyChain-5.1.0/Supplychain/Validate/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-04 10:32:20.000000 CosmoTech-SupplyChain-5.1.0/Supplychain/Validate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21965 2023-08-04 10:32:20.000000 CosmoTech-SupplyChain-5.1.0/Supplychain/Validate/validate_dict.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 10:32:30.734869 CosmoTech-SupplyChain-5.1.0/Supplychain/Wrappers/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-04 10:32:20.000000 CosmoTech-SupplyChain-5.1.0/Supplychain/Wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1646 2023-08-04 10:32:20.000000 CosmoTech-SupplyChain-5.1.0/Supplychain/Wrappers/environment_variables.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18535 2023-08-04 10:32:20.000000 CosmoTech-SupplyChain-5.1.0/Supplychain/Wrappers/simulator.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-04 10:32:20.000000 CosmoTech-SupplyChain-5.1.0/Supplychain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-08-04 10:32:30.734869 CosmoTech-SupplyChain-5.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      851 2023-08-04 10:32:21.000000 CosmoTech-SupplyChain-5.1.0/setup.py
```

### Comparing `CosmoTech-SupplyChain-5.0.1/CosmoTech_SupplyChain.egg-info/SOURCES.txt` & `CosmoTech-SupplyChain-5.1.0/CosmoTech_SupplyChain.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.0.1/LICENSE` & `CosmoTech-SupplyChain-5.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.0.1/README.md` & `CosmoTech-SupplyChain-5.1.0/README.md`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.0.1/Supplychain/Generic/adt_writer.py` & `CosmoTech-SupplyChain-5.1.0/Supplychain/Generic/adt_writer.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.0.1/Supplychain/Generic/adx_and_file_writer.py` & `CosmoTech-SupplyChain-5.1.0/Supplychain/Generic/adx_and_file_writer.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.0.1/Supplychain/Generic/adx_wrapper.py` & `CosmoTech-SupplyChain-5.1.0/Supplychain/Generic/adx_wrapper.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.0.1/Supplychain/Generic/cosmo_api_parameters.py` & `CosmoTech-SupplyChain-5.1.0/Supplychain/Generic/cosmo_api_parameters.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.0.1/Supplychain/Generic/csv_folder_reader.py` & `CosmoTech-SupplyChain-5.1.0/Supplychain/Generic/csv_folder_reader.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.0.1/Supplychain/Generic/csv_folder_writer.py` & `CosmoTech-SupplyChain-5.1.0/Supplychain/Generic/csv_folder_writer.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.0.1/Supplychain/Generic/duration.py` & `CosmoTech-SupplyChain-5.1.0/Supplychain/Generic/duration.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.0.1/Supplychain/Generic/excel_folder_reader.py` & `CosmoTech-SupplyChain-5.1.0/Supplychain/Generic/excel_folder_reader.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.0.1/Supplychain/Generic/excel_folder_writer.py` & `CosmoTech-SupplyChain-5.1.0/Supplychain/Generic/excel_folder_writer.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.0.1/Supplychain/Generic/folder_io.py` & `CosmoTech-SupplyChain-5.1.0/Supplychain/Generic/folder_io.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.0.1/Supplychain/Generic/json_folder_reader.py` & `CosmoTech-SupplyChain-5.1.0/Supplychain/Generic/json_folder_reader.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.0.1/Supplychain/Generic/json_folder_writer.py` & `CosmoTech-SupplyChain-5.1.0/Supplychain/Generic/json_folder_writer.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.0.1/Supplychain/Generic/memory_folder_io.py` & `CosmoTech-SupplyChain-5.1.0/Supplychain/Generic/memory_folder_io.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.0.1/Supplychain/Generic/simulator_io.py` & `CosmoTech-SupplyChain-5.1.0/Supplychain/Generic/simulator_io.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.0.1/Supplychain/Generic/storage_queue_writer.py` & `CosmoTech-SupplyChain-5.1.0/Supplychain/Generic/storage_queue_writer.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.0.1/Supplychain/Generic/timer.py` & `CosmoTech-SupplyChain-5.1.0/Supplychain/Generic/timer.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.0.1/Supplychain/Protocol/cmaes_optimization_algorithm.py` & `CosmoTech-SupplyChain-5.1.0/Supplychain/Protocol/cmaes_optimization_algorithm.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.0.1/Supplychain/Protocol/default_transformation.py` & `CosmoTech-SupplyChain-5.1.0/Supplychain/Protocol/default_transformation.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.0.1/Supplychain/Protocol/multiprocessing_optimization.py` & `CosmoTech-SupplyChain-5.1.0/Supplychain/Protocol/multiprocessing_optimization.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.0.1/Supplychain/Protocol/objective_functions.py` & `CosmoTech-SupplyChain-5.1.0/Supplychain/Protocol/objective_functions.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.0.1/Supplychain/Protocol/protocol.py` & `CosmoTech-SupplyChain-5.1.0/Supplychain/Protocol/protocol.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.0.1/Supplychain/Run/cmaes_optimization.py` & `CosmoTech-SupplyChain-5.1.0/Supplychain/Run/cmaes_optimization.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.0.1/Supplychain/Run/consumers.py` & `CosmoTech-SupplyChain-5.1.0/Supplychain/Run/consumers.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.0.1/Supplychain/Run/local_sensitivity_analysis_comets.py` & `CosmoTech-SupplyChain-5.1.0/Supplychain/Run/local_sensitivity_analysis_comets.py`

 * *Files 2% similar despite different names*

```diff
@@ -307,14 +307,16 @@
 
         errors = validate_absolute_variations(list_of_variables)
         if errors:
             t.display_message('\n'.join(errors))
             error_message = f"Invalid parameter{'s' if len(errors) > 1 else ''}"
             raise ValueError(error_message)
 
+        t.split("{time_since_last_split:6.4f} ({time_since_start:6.4f}) - Variables creation and validation")
+
         def encoder(parameters):
             """
             Encoder of the task on which the S.A will be performed. The encoder receives a parameter set where
             the attributes of type 'schedule' are separated (see function create_variables). The aim of this encoder is to
             re concatenate the schedules together. For example, if the encoder receives the following parameter set:
             {"transport_lyon": 2,
                 "transport_paris__@__0": 1,
@@ -390,29 +392,33 @@
             encode=encoder,
         )
 
         experiment = co.LocalSensitivityAnalysis(
             task=simulationtask, variables=list_of_variables, n_jobs=-2
         )
 
-        t.display_message("Starting simulations")
+        t.split("{time_since_last_split:6.4f} ({time_since_start:6.4f}) - Experiment initialization")
+
         experiment.run()
-        t.split("Ended simulations : {time_since_start}")
+
+        t.split("{time_since_last_split:6.4f} ({time_since_start:6.4f}) - Simulations")
 
         results = reformat_results(
             experiment.results,
             simulation_name,
             change,
             variation,
             parameter,
             timeinterval,
             initialtimestep,
             finaltimestep,
         )
 
+        t.split("{time_since_last_split:6.4f} ({time_since_start:6.4f}) - Results reformatting")
+
     return results
 
 
 def validate_sa_parameters(
     sensitive_parameter: str,
     change: str,
     variation: float,
```

### Comparing `CosmoTech-SupplyChain-5.0.1/Supplychain/Run/simulation.py` & `CosmoTech-SupplyChain-5.1.0/Supplychain/Run/simulation.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.0.1/Supplychain/Run/simulation_comets.py` & `CosmoTech-SupplyChain-5.1.0/Supplychain/Run/simulation_comets.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.0.1/Supplychain/Run/stochastic_optimization.py` & `CosmoTech-SupplyChain-5.1.0/Supplychain/Run/stochastic_optimization.py`

 * *Files 0% similar despite different names*

```diff
@@ -246,14 +246,17 @@
                 opt.optimization_history
             )
             optimal_decision_variables = opt.results["Optimal variables"]
             optimal_decision_variables_df = self._reformat_decision_variables_results(
                 optimal_decision_variables
             )
 
+            if self.optimization_algorithm == "NGOpt" and self.optim_batch_size == 1:
+                del opt.optimizationalgorithm
+
             t.display_message("Running simple simulation to fill ADX")
             # Put back log level to Info for final simulation
             # Reduce log level to Error during optimization
             logger = CosmoEngine.LoggerManager.GetInstance().GetLogger()
             logger.SetLogLevel(logger.eInfo)
 
         return (
```

### Comparing `CosmoTech-SupplyChain-5.0.1/Supplychain/Run/uncertainty_analysis.py` & `CosmoTech-SupplyChain-5.1.0/Supplychain/Run/uncertainty_analysis.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.0.1/Supplychain/Run/uncertainty_analysis_comets.py` & `CosmoTech-SupplyChain-5.1.0/Supplychain/Run/uncertainty_analysis_comets.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.0.1/Supplychain/Run/uncertainty_analysis_helper_functions.py` & `CosmoTech-SupplyChain-5.1.0/Supplychain/Run/uncertainty_analysis_helper_functions.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.0.1/Supplychain/Schema/adt_column_description.py` & `CosmoTech-SupplyChain-5.1.0/Supplychain/Schema/adt_column_description.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,14 +29,15 @@
                 "SourcingPolicy",
                 "DispatchPolicy",
                 "ReviewPeriod",
                 "FirstReview",
                 "Advance",
                 "Latitude",
                 "Longitude",
+                "IgnoreDownstreamRequiredQuantities",
             ],
             "change": [
                 "StorageUnitCosts",
                 "OrderPoints",
                 "OrderQuantities",
                 "OrderUpToLevels",
                 "SafetyQuantities",
```

### Comparing `CosmoTech-SupplyChain-5.0.1/Supplychain/Schema/default_values.py` & `CosmoTech-SupplyChain-5.1.0/Supplychain/Schema/default_values.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,15 @@
         "SourcingPolicy": "Equidistribution",
         "DispatchPolicy": "Equidistribution",
         "ReviewPeriod": 1,
         "FirstReview": 0,
         "Advance": 0,
         "Latitude": 0.0,
         "Longitude": 0.0,
+        "IgnoreDownstreamRequiredQuantities": False,
         "StorageUnitCosts": {},
         "OrderPoints": {},
         "OrderQuantities": {},
         "OrderUpToLevels": {},
         "SafetyQuantities": {},
         "Demands": {},
         "DemandUncertainties": {},
```

### Comparing `CosmoTech-SupplyChain-5.0.1/Supplychain/Schema/simulator_files_description.py` & `CosmoTech-SupplyChain-5.1.0/Supplychain/Schema/simulator_files_description.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,14 +40,15 @@
         "Advance",
         "LeadTime",
         "SalesForecasts",
         "OrderPointSchedule",
         "OrderQuantitySchedule",
         "SafetyQuantitySchedule",
         "SchedulingStep",
+        "IgnoreDownstreamRequiredQuantities",
     ],
     "CE_Machine": [
         "Name",
         "StockTypeProportion",
         "Groups",
         "OpeningRates",
         "OpeningTimeSchedule",
```

### Comparing `CosmoTech-SupplyChain-5.0.1/Supplychain/Schema/validation_schemas.py` & `CosmoTech-SupplyChain-5.1.0/Supplychain/Schema/validation_schemas.py`

 * *Files 1% similar despite different names*

```diff
@@ -397,14 +397,15 @@
                 },
                 "SalesForecasts": {
                     "type": "object",
                     "patternProperties": {"^[0-9]+$": {"type": "number", "minimum": 0}},
                 },
                 "Latitude": {"type": "number", "minimum": -90, "maximum": 90},
                 "Longitude": {"type": "number", "minimum": -180, "maximum": 180},
+                "IgnoreDownstreamRequiredQuantities": {"type": "boolean"},
             },
             "dependencies": {"InitialValue": ["InitialStock"]},
         },
         "Transport": {
             "$schema": "http://json-schema.org/draft-07/schema#",
             "type": "object",
             "properties": {
```

### Comparing `CosmoTech-SupplyChain-5.0.1/Supplychain/Transform/complete_dict.py` & `CosmoTech-SupplyChain-5.1.0/Supplychain/Transform/complete_dict.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.0.1/Supplychain/Transform/from_dict_to_simulator.py` & `CosmoTech-SupplyChain-5.1.0/Supplychain/Transform/from_dict_to_simulator.py`

 * *Files 1% similar despite different names*

```diff
@@ -530,14 +530,15 @@
                 "SalesForecasts": convert_dict(int, float, stock["SalesForecasts"]),
                 "OrderPointSchedule": convert_dict(int, float, stock["OrderPoints"]),
                 "OrderQuantitySchedule": dict(),
                 "SafetyQuantitySchedule": convert_dict(
                     int, float, stock["SafetyQuantities"]
                 ),
                 "SchedulingStep": self.entity_order.get(stock["id"], -1),
+                "IgnoreDownstreamRequiredQuantities": stock["IgnoreDownstreamRequiredQuantities"],
             }
 
             if stock_item["StockPolicy"] == "OrderPointFixedQuantity":
                 stock_item["OrderQuantitySchedule"] = convert_dict(
                     int, float, stock["OrderQuantities"]
                 )
             elif stock_item["StockPolicy"] == "OrderPointVariableQuantity":
```

### Comparing `CosmoTech-SupplyChain-5.0.1/Supplychain/Transform/from_dict_to_table.py` & `CosmoTech-SupplyChain-5.1.0/Supplychain/Transform/from_dict_to_table.py`

 * *Files 0% similar despite different names*

```diff
@@ -186,15 +186,15 @@
                 fake_event_element = dict()
                 for column_list in fake_row_keys, ['Timestep', ], file_description['event'][event_name]:
                     for key in column_list:
                         fake_event_element[key] = None
                 if self.simulation_id:
                     fake_event_element['SimulationRun'] = self.simulation_id
                 self.write_target_file([fake_event_element, ], event_name, self.simulation_id)
-        self.split("{time_since_last_split:6.4f}({time_since_start:6.4f}) - " + file_name)
+        self.split("{time_since_last_split:6.4f} ({time_since_start:6.4f}) - " + file_name)
 
     def __init__(self,
                  simulation_id: Union[str, None],
                  reader: FolderReader,
                  writer: Union[FolderWriter, None] = None,
                  adx_connector: Union[ADXQueriesWrapper, ADXWrapper, None] = None,
                  keep_duplicate: bool = True):
```

### Comparing `CosmoTech-SupplyChain-5.0.1/Supplychain/Transform/from_table_to_dict.py` & `CosmoTech-SupplyChain-5.1.0/Supplychain/Transform/from_table_to_dict.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.0.1/Supplychain/Transform/from_table_to_dict_old.py` & `CosmoTech-SupplyChain-5.1.0/Supplychain/Transform/from_table_to_dict_old.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.0.1/Supplychain/Transform/patch_dict_with_parameters.py` & `CosmoTech-SupplyChain-5.1.0/Supplychain/Transform/patch_dict_with_parameters.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.0.1/Supplychain/Transform/production_route.py` & `CosmoTech-SupplyChain-5.1.0/Supplychain/Transform/production_route.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.0.1/Supplychain/Validate/validate_dict.py` & `CosmoTech-SupplyChain-5.1.0/Supplychain/Validate/validate_dict.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.0.1/Supplychain/Wrappers/environment_variables.py` & `CosmoTech-SupplyChain-5.1.0/Supplychain/Wrappers/environment_variables.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.0.1/Supplychain/Wrappers/simulator.py` & `CosmoTech-SupplyChain-5.1.0/Supplychain/Wrappers/simulator.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-5.0.1/setup.py` & `CosmoTech-SupplyChain-5.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import setuptools
 
 
-VERSION = "5.0.1"
+VERSION = "5.1.0"
 
 setuptools.setup(
     name='CosmoTech-SupplyChain',
     version=VERSION,
     author='Alexis Fossart',
     author_email='alexis.fossart@cosmotech.com',
     url='https://github.com/Cosmo-Tech/supplychain-python-library<',
```

