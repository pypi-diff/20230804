# Comparing `tmp/dbt-airflow-factory-0.32.0.tar.gz` & `tmp/dbt-airflow-factory-0.33.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-airflow-factory-0.32.0.tar", last modified: Wed Jul  5 07:11:01 2023, max compression
+gzip compressed data, was "dbt-airflow-factory-0.33.0.tar", last modified: Fri Aug  4 10:41:46 2023, max compression
```

## Comparing `dbt-airflow-factory-0.32.0.tar` & `dbt-airflow-factory-0.33.0.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 07:11:01.827899 dbt-airflow-factory-0.32.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-05 07:10:58.000000 dbt-airflow-factory-0.32.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-07-05 07:11:01.827899 dbt-airflow-factory-0.32.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-07-05 07:10:58.000000 dbt-airflow-factory-0.32.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 07:11:01.823899 dbt-airflow-factory-0.32.0/dbt_airflow_factory/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-05 07:10:58.000000 dbt-airflow-factory-0.32.0/dbt_airflow_factory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5576 2023-07-05 07:10:58.000000 dbt-airflow-factory-0.32.0/dbt_airflow_factory/airflow_dag_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 07:11:01.823899 dbt-airflow-factory-0.32.0/dbt_airflow_factory/bash/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 07:10:58.000000 dbt-airflow-factory-0.32.0/dbt_airflow_factory/bash/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-07-05 07:10:58.000000 dbt-airflow-factory-0.32.0/dbt_airflow_factory/bash/bash_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-05 07:10:58.000000 dbt-airflow-factory-0.32.0/dbt_airflow_factory/bash/bash_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-05 07:10:58.000000 dbt-airflow-factory-0.32.0/dbt_airflow_factory/bash/bash_parameters_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     4824 2023-07-05 07:10:58.000000 dbt-airflow-factory-0.32.0/dbt_airflow_factory/builder_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-07-05 07:10:58.000000 dbt-airflow-factory-0.32.0/dbt_airflow_factory/config_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-05 07:10:58.000000 dbt-airflow-factory-0.32.0/dbt_airflow_factory/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-07-05 07:10:58.000000 dbt-airflow-factory-0.32.0/dbt_airflow_factory/dbt_parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 07:11:01.823899 dbt-airflow-factory-0.32.0/dbt_airflow_factory/ecs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 07:10:58.000000 dbt-airflow-factory-0.32.0/dbt_airflow_factory/ecs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-07-05 07:10:58.000000 dbt-airflow-factory-0.32.0/dbt_airflow_factory/ecs/ecs_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-05 07:10:58.000000 dbt-airflow-factory-0.32.0/dbt_airflow_factory/ecs/ecs_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-05 07:10:58.000000 dbt-airflow-factory-0.32.0/dbt_airflow_factory/ecs/ecs_parameters_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-07-05 07:10:58.000000 dbt-airflow-factory-0.32.0/dbt_airflow_factory/ingestion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 07:11:01.827899 dbt-airflow-factory-0.32.0/dbt_airflow_factory/k8s/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 07:10:58.000000 dbt-airflow-factory-0.32.0/dbt_airflow_factory/k8s/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-07-05 07:10:58.000000 dbt-airflow-factory-0.32.0/dbt_airflow_factory/k8s/k8s_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6041 2023-07-05 07:10:58.000000 dbt-airflow-factory-0.32.0/dbt_airflow_factory/k8s/k8s_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-07-05 07:10:58.000000 dbt-airflow-factory-0.32.0/dbt_airflow_factory/k8s/k8s_parameters_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 07:11:01.827899 dbt-airflow-factory-0.32.0/dbt_airflow_factory/notifications/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 07:10:58.000000 dbt-airflow-factory-0.32.0/dbt_airflow_factory/notifications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-07-05 07:10:58.000000 dbt-airflow-factory-0.32.0/dbt_airflow_factory/notifications/handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-07-05 07:10:58.000000 dbt-airflow-factory-0.32.0/dbt_airflow_factory/operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3897 2023-07-05 07:10:58.000000 dbt-airflow-factory-0.32.0/dbt_airflow_factory/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 07:11:01.827899 dbt-airflow-factory-0.32.0/dbt_airflow_factory/tasks_builder/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 07:10:58.000000 dbt-airflow-factory-0.32.0/dbt_airflow_factory/tasks_builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7734 2023-07-05 07:10:58.000000 dbt-airflow-factory-0.32.0/dbt_airflow_factory/tasks_builder/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-05 07:10:58.000000 dbt-airflow-factory-0.32.0/dbt_airflow_factory/tasks_builder/parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 07:11:01.823899 dbt-airflow-factory-0.32.0/dbt_airflow_factory.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-07-05 07:11:01.000000 dbt-airflow-factory-0.32.0/dbt_airflow_factory.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-07-05 07:11:01.000000 dbt-airflow-factory-0.32.0/dbt_airflow_factory.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 07:11:01.000000 dbt-airflow-factory-0.32.0/dbt_airflow_factory.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 07:11:01.000000 dbt-airflow-factory-0.32.0/dbt_airflow_factory.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-05 07:11:01.000000 dbt-airflow-factory-0.32.0/dbt_airflow_factory.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-05 07:11:01.000000 dbt-airflow-factory-0.32.0/dbt_airflow_factory.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-05 07:10:58.000000 dbt-airflow-factory-0.32.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-05 07:11:01.827899 dbt-airflow-factory-0.32.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-07-05 07:10:58.000000 dbt-airflow-factory-0.32.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:41:46.978485 dbt-airflow-factory-0.33.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-04 10:41:45.000000 dbt-airflow-factory-0.33.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4116 2023-08-04 10:41:46.978485 dbt-airflow-factory-0.33.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-08-04 10:41:45.000000 dbt-airflow-factory-0.33.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:41:46.974485 dbt-airflow-factory-0.33.0/dbt_airflow_factory/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-08-04 10:41:45.000000 dbt-airflow-factory-0.33.0/dbt_airflow_factory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5576 2023-08-04 10:41:45.000000 dbt-airflow-factory-0.33.0/dbt_airflow_factory/airflow_dag_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:41:46.978485 dbt-airflow-factory-0.33.0/dbt_airflow_factory/bash/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 10:41:45.000000 dbt-airflow-factory-0.33.0/dbt_airflow_factory/bash/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-08-04 10:41:45.000000 dbt-airflow-factory-0.33.0/dbt_airflow_factory/bash/bash_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-08-04 10:41:45.000000 dbt-airflow-factory-0.33.0/dbt_airflow_factory/bash/bash_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-08-04 10:41:45.000000 dbt-airflow-factory-0.33.0/dbt_airflow_factory/bash/bash_parameters_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4909 2023-08-04 10:41:45.000000 dbt-airflow-factory-0.33.0/dbt_airflow_factory/builder_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-08-04 10:41:45.000000 dbt-airflow-factory-0.33.0/dbt_airflow_factory/config_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-08-04 10:41:45.000000 dbt-airflow-factory-0.33.0/dbt_airflow_factory/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-08-04 10:41:45.000000 dbt-airflow-factory-0.33.0/dbt_airflow_factory/dbt_parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:41:46.978485 dbt-airflow-factory-0.33.0/dbt_airflow_factory/ecs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 10:41:45.000000 dbt-airflow-factory-0.33.0/dbt_airflow_factory/ecs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-08-04 10:41:45.000000 dbt-airflow-factory-0.33.0/dbt_airflow_factory/ecs/ecs_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-08-04 10:41:45.000000 dbt-airflow-factory-0.33.0/dbt_airflow_factory/ecs/ecs_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-08-04 10:41:45.000000 dbt-airflow-factory-0.33.0/dbt_airflow_factory/ecs/ecs_parameters_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-08-04 10:41:45.000000 dbt-airflow-factory-0.33.0/dbt_airflow_factory/ingestion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:41:46.978485 dbt-airflow-factory-0.33.0/dbt_airflow_factory/k8s/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 10:41:45.000000 dbt-airflow-factory-0.33.0/dbt_airflow_factory/k8s/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-08-04 10:41:45.000000 dbt-airflow-factory-0.33.0/dbt_airflow_factory/k8s/k8s_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6041 2023-08-04 10:41:45.000000 dbt-airflow-factory-0.33.0/dbt_airflow_factory/k8s/k8s_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-08-04 10:41:45.000000 dbt-airflow-factory-0.33.0/dbt_airflow_factory/k8s/k8s_parameters_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:41:46.978485 dbt-airflow-factory-0.33.0/dbt_airflow_factory/notifications/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 10:41:45.000000 dbt-airflow-factory-0.33.0/dbt_airflow_factory/notifications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-08-04 10:41:45.000000 dbt-airflow-factory-0.33.0/dbt_airflow_factory/notifications/handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-08-04 10:41:45.000000 dbt-airflow-factory-0.33.0/dbt_airflow_factory/operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3897 2023-08-04 10:41:45.000000 dbt-airflow-factory-0.33.0/dbt_airflow_factory/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:41:46.978485 dbt-airflow-factory-0.33.0/dbt_airflow_factory/tasks_builder/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 10:41:45.000000 dbt-airflow-factory-0.33.0/dbt_airflow_factory/tasks_builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7849 2023-08-04 10:41:45.000000 dbt-airflow-factory-0.33.0/dbt_airflow_factory/tasks_builder/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-08-04 10:41:45.000000 dbt-airflow-factory-0.33.0/dbt_airflow_factory/tasks_builder/parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:41:46.974485 dbt-airflow-factory-0.33.0/dbt_airflow_factory.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4116 2023-08-04 10:41:46.000000 dbt-airflow-factory-0.33.0/dbt_airflow_factory.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-08-04 10:41:46.000000 dbt-airflow-factory-0.33.0/dbt_airflow_factory.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 10:41:46.000000 dbt-airflow-factory-0.33.0/dbt_airflow_factory.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 10:41:46.000000 dbt-airflow-factory-0.33.0/dbt_airflow_factory.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-08-04 10:41:46.000000 dbt-airflow-factory-0.33.0/dbt_airflow_factory.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-04 10:41:46.000000 dbt-airflow-factory-0.33.0/dbt_airflow_factory.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-08-04 10:41:45.000000 dbt-airflow-factory-0.33.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-08-04 10:41:46.978485 dbt-airflow-factory-0.33.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-08-04 10:41:45.000000 dbt-airflow-factory-0.33.0/setup.py
```

### Comparing `dbt-airflow-factory-0.32.0/LICENSE` & `dbt-airflow-factory-0.33.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt-airflow-factory-0.32.0/PKG-INFO` & `dbt-airflow-factory-0.33.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,98 +1,100 @@
 Metadata-Version: 2.1
 Name: dbt-airflow-factory
-Version: 0.32.0
+Version: 0.33.0
 Summary: Library to convert DBT manifest metadata to Airflow tasks
 Home-page: https://github.com/getindata/dbt-airflow-factory/
 Author: Piotr Pekala
 Author-email: piotr.pekala@getindata.com
 License: Apache Software License (Apache 2.0)
-Description: # DBT Airflow Factory
-        
-        [![Python Version](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue)](https://github.com/getindata/dbt-airflow-factory)
-        [![PyPI Version](https://badge.fury.io/py/dbt-airflow-factory.svg)](https://pypi.org/project/dbt-airflow-factory/)
-        [![Downloads](https://pepy.tech/badge/dbt-airflow-factory)](https://pepy.tech/project/dbt-airflow-factory)
-        [![Maintainability](https://api.codeclimate.com/v1/badges/47fd3570c858b6c166ad/maintainability)](https://codeclimate.com/github/getindata/dbt-airflow-factory/maintainability)
-        [![Test Coverage](https://api.codeclimate.com/v1/badges/47fd3570c858b6c166ad/test_coverage)](https://codeclimate.com/github/getindata/dbt-airflow-factory/test_coverage)
-        [![Documentation Status](https://readthedocs.org/projects/dbt-airflow-factory/badge/?version=latest)](https://dbt-airflow-factory.readthedocs.io/en/latest/?badge=latest)
-        
-        Library to convert DBT manifest metadata to Airflow tasks
-        
-        ## Documentation
-        
-        Read the full documentation at [https://dbt-airflow-factory.readthedocs.io/](https://dbt-airflow-factory.readthedocs.io/en/latest/index.html)
-        
-        ## Installation
-        
-        Use the package manager [pip][pip] to install the library:
-        
-        ```bash
-        pip install dbt-airflow-factory
-        ```
-        
-        ## Usage
-        
-        The library is expected to be used inside an Airflow environment with a Kubernetes image referencing **dbt**.
-        
-        **dbt-airflow-factory**'s main task is to parse `manifest.json` and create Airflow DAG out of it. It also reads config
-        files from `config` directory and therefore is highly customizable (e.g., user can set path to `manifest.json`).
-        
-        To start, create a directory with a following structure, where `manifest.json` is a file generated by **dbt**:
-        ```
-        .
-        ├── config
-        │   ├── base
-        │   │   ├── airflow.yml
-        │   │   ├── dbt.yml
-        │   │   └── k8s.yml
-        │   └── dev
-        │       └── dbt.yml
-        ├── dag.py
-        └── manifest.json
-        ```
-        
-        Then, put the following code into `dag.py`:
-        ```python
-        from dbt_airflow_factory.airflow_dag_factory import AirflowDagFactory
-        from os import path
-        
-        dag = AirflowDagFactory(path.dirname(path.abspath(__file__)), "dev").create()
-        ```
-        
-        When uploaded to Airflow DAGs directory, it will get picked up by Airflow, parse `manifest.json` and prepare a DAG to run.
-        
-        ### Configuration files
-        
-        It is best to look up the example configuration files in [tests directory][tests] to get a glimpse of correct configs.
-        
-        You can use [Airflow template variables][airflow-vars] in your `dbt.yml` and `k8s.yml` files, as long as they are inside
-        quotation marks:
-        ```yaml
-        target: "{{ var.value.env }}"
-        some_other_field: "{{ ds_nodash }}"
-        ```
-        
-        Analogously, you can use `"{{ var.value.VARIABLE_NAME }}"` in `airflow.yml`, but only the Airflow variable getter.
-        Any other Airflow template variables will not work in `airflow.yml`.
-        
-        ### Creation of the directory with data-pipelines-cli
-        
-        **DBT Airflow Factory** works best in tandem with [data-pipelines-cli][dp-cli] tool. **dp** not only prepares directory
-        for the library to digest, but also automates Docker image building and pushes generated directory to the cloud storage
-        of your choice.
-        
-        [airflow-vars]: https://airflow.apache.org/docs/apache-airflow/stable/templates-ref.html#variables
-        [dp-cli]: https://pypi.org/project/data-pipelines-cli/
-        [pip]: https://pip.pypa.io/en/stable/
-        [tests]: https://github.com/getindata/dbt-airflow-factory/tree/develop/tests/config
-        
 Keywords: dbt airflow manifest parser python
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 Provides-Extra: docs
+License-File: LICENSE
+
+# DBT Airflow Factory
+
+[![Python Version](https://img.shields.io/badge/python-3.9%20%7C%203.10%20%7C%203.11-blue)](https://github.com/getindata/dbt-airflow-factory)
+[![PyPI Version](https://badge.fury.io/py/dbt-airflow-factory.svg)](https://pypi.org/project/dbt-airflow-factory/)
+[![Downloads](https://pepy.tech/badge/dbt-airflow-factory)](https://pepy.tech/project/dbt-airflow-factory)
+[![Maintainability](https://api.codeclimate.com/v1/badges/47fd3570c858b6c166ad/maintainability)](https://codeclimate.com/github/getindata/dbt-airflow-factory/maintainability)
+[![Test Coverage](https://api.codeclimate.com/v1/badges/47fd3570c858b6c166ad/test_coverage)](https://codeclimate.com/github/getindata/dbt-airflow-factory/test_coverage)
+[![Documentation Status](https://readthedocs.org/projects/dbt-airflow-factory/badge/?version=latest)](https://dbt-airflow-factory.readthedocs.io/en/latest/?badge=latest)
+
+Library to convert DBT manifest metadata to Airflow tasks
+
+## Documentation
+
+Read the full documentation at [https://dbt-airflow-factory.readthedocs.io/](https://dbt-airflow-factory.readthedocs.io/en/latest/index.html)
+
+## Installation
+
+Use the package manager [pip][pip] to install the library:
+
+```bash
+pip install dbt-airflow-factory
+```
+
+## Usage
+
+The library is expected to be used inside an Airflow environment with a Kubernetes image referencing **dbt**.
+
+**dbt-airflow-factory**'s main task is to parse `manifest.json` and create Airflow DAG out of it. It also reads config
+files from `config` directory and therefore is highly customizable (e.g., user can set path to `manifest.json`).
+
+To start, create a directory with a following structure, where `manifest.json` is a file generated by **dbt**:
+```
+.
+├── config
+│   ├── base
+│   │   ├── airflow.yml
+│   │   ├── dbt.yml
+│   │   └── k8s.yml
+│   └── dev
+│       └── dbt.yml
+├── dag.py
+└── manifest.json
+```
+
+Then, put the following code into `dag.py`:
+```python
+from dbt_airflow_factory.airflow_dag_factory import AirflowDagFactory
+from os import path
+
+dag = AirflowDagFactory(path.dirname(path.abspath(__file__)), "dev").create()
+```
+
+When uploaded to Airflow DAGs directory, it will get picked up by Airflow, parse `manifest.json` and prepare a DAG to run.
+
+### Configuration files
+
+It is best to look up the example configuration files in [tests directory][tests] to get a glimpse of correct configs.
+
+You can use [Airflow template variables][airflow-vars] in your `dbt.yml` and `k8s.yml` files, as long as they are inside
+quotation marks:
+```yaml
+target: "{{ var.value.env }}"
+some_other_field: "{{ ds_nodash }}"
+```
+
+Analogously, you can use `"{{ var.value.VARIABLE_NAME }}"` in `airflow.yml`, but only the Airflow variable getter.
+Any other Airflow template variables will not work in `airflow.yml`.
+
+### Creation of the directory with data-pipelines-cli
+
+**DBT Airflow Factory** works best in tandem with [data-pipelines-cli][dp-cli] tool. **dp** not only prepares directory
+for the library to digest, but also automates Docker image building and pushes generated directory to the cloud storage
+of your choice.
+
+[airflow-vars]: https://airflow.apache.org/docs/apache-airflow/stable/templates-ref.html#variables
+[dp-cli]: https://pypi.org/project/data-pipelines-cli/
+[pip]: https://pip.pypa.io/en/stable/
+[tests]: https://github.com/getindata/dbt-airflow-factory/tree/develop/tests/config
+
+
```

### Comparing `dbt-airflow-factory-0.32.0/README.md` & `dbt-airflow-factory-0.33.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # DBT Airflow Factory
 
-[![Python Version](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue)](https://github.com/getindata/dbt-airflow-factory)
+[![Python Version](https://img.shields.io/badge/python-3.9%20%7C%203.10%20%7C%203.11-blue)](https://github.com/getindata/dbt-airflow-factory)
 [![PyPI Version](https://badge.fury.io/py/dbt-airflow-factory.svg)](https://pypi.org/project/dbt-airflow-factory/)
 [![Downloads](https://pepy.tech/badge/dbt-airflow-factory)](https://pepy.tech/project/dbt-airflow-factory)
 [![Maintainability](https://api.codeclimate.com/v1/badges/47fd3570c858b6c166ad/maintainability)](https://codeclimate.com/github/getindata/dbt-airflow-factory/maintainability)
 [![Test Coverage](https://api.codeclimate.com/v1/badges/47fd3570c858b6c166ad/test_coverage)](https://codeclimate.com/github/getindata/dbt-airflow-factory/test_coverage)
 [![Documentation Status](https://readthedocs.org/projects/dbt-airflow-factory/badge/?version=latest)](https://dbt-airflow-factory.readthedocs.io/en/latest/?badge=latest)
 
 Library to convert DBT manifest metadata to Airflow tasks
```

### Comparing `dbt-airflow-factory-0.32.0/dbt_airflow_factory/airflow_dag_factory.py` & `dbt-airflow-factory-0.33.0/dbt_airflow_factory/airflow_dag_factory.py`

 * *Files identical despite different names*

### Comparing `dbt-airflow-factory-0.32.0/dbt_airflow_factory/bash/bash_operator.py` & `dbt-airflow-factory-0.33.0/dbt_airflow_factory/bash/bash_operator.py`

 * *Files identical despite different names*

### Comparing `dbt-airflow-factory-0.32.0/dbt_airflow_factory/builder_factory.py` & `dbt-airflow-factory-0.33.0/dbt_airflow_factory/builder_factory.py`

 * *Files 4% similar despite different names*

```diff
@@ -79,14 +79,15 @@
         )
 
     def _create_tasks_airflow_config(self) -> TasksBuildingParameters:
         return TasksBuildingParameters(
             self.airflow_config.get("use_task_group", False),
             self.airflow_config.get("show_ephemeral_models", True),
             self.airflow_config.get("enable_project_dependencies", False),
+            self.airflow_config.get("check_all_deps_for_multiple_deps_tests", True),
         )
 
     def _create_operator_builder(
         self, type: str, dbt_params: DbtExecutionEnvironmentParameters
     ) -> DbtRunOperatorBuilder:
         if type == "k8s":
             return KubernetesPodOperatorBuilder(
```

### Comparing `dbt-airflow-factory-0.32.0/dbt_airflow_factory/config_utils.py` & `dbt-airflow-factory-0.33.0/dbt_airflow_factory/config_utils.py`

 * *Files identical despite different names*

### Comparing `dbt-airflow-factory-0.32.0/dbt_airflow_factory/dbt_parameters.py` & `dbt-airflow-factory-0.33.0/dbt_airflow_factory/dbt_parameters.py`

 * *Files identical despite different names*

### Comparing `dbt-airflow-factory-0.32.0/dbt_airflow_factory/ecs/ecs_operator.py` & `dbt-airflow-factory-0.33.0/dbt_airflow_factory/ecs/ecs_operator.py`

 * *Files identical despite different names*

### Comparing `dbt-airflow-factory-0.32.0/dbt_airflow_factory/ingestion.py` & `dbt-airflow-factory-0.33.0/dbt_airflow_factory/ingestion.py`

 * *Files identical despite different names*

### Comparing `dbt-airflow-factory-0.32.0/dbt_airflow_factory/k8s/k8s_operator.py` & `dbt-airflow-factory-0.33.0/dbt_airflow_factory/k8s/k8s_operator.py`

 * *Files identical despite different names*

### Comparing `dbt-airflow-factory-0.32.0/dbt_airflow_factory/k8s/k8s_parameters.py` & `dbt-airflow-factory-0.33.0/dbt_airflow_factory/k8s/k8s_parameters.py`

 * *Files identical despite different names*

### Comparing `dbt-airflow-factory-0.32.0/dbt_airflow_factory/k8s/k8s_parameters_loader.py` & `dbt-airflow-factory-0.33.0/dbt_airflow_factory/k8s/k8s_parameters_loader.py`

 * *Files identical despite different names*

### Comparing `dbt-airflow-factory-0.32.0/dbt_airflow_factory/notifications/handler.py` & `dbt-airflow-factory-0.33.0/dbt_airflow_factory/notifications/handler.py`

 * *Files identical despite different names*

### Comparing `dbt-airflow-factory-0.32.0/dbt_airflow_factory/operator.py` & `dbt-airflow-factory-0.33.0/dbt_airflow_factory/operator.py`

 * *Files identical despite different names*

### Comparing `dbt-airflow-factory-0.32.0/dbt_airflow_factory/tasks.py` & `dbt-airflow-factory-0.33.0/dbt_airflow_factory/tasks.py`

 * *Files identical despite different names*

### Comparing `dbt-airflow-factory-0.32.0/dbt_airflow_factory/tasks_builder/builder.py` & `dbt-airflow-factory-0.33.0/dbt_airflow_factory/tasks_builder/builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -166,14 +166,15 @@
         manifest = self._load_dbt_manifest(manifest_path)
         dbt_airflow_graph: DbtManifestGraph = create_tasks_graph(
             manifest,
             GraphConfiguration(
                 gateway_config=self.gateway_config,
                 enable_dags_dependencies=self.airflow_config.enable_dags_dependencies,
                 show_ephemeral_models=self.airflow_config.show_ephemeral_models,
+                check_all_deps_for_multiple_deps_tests=self.airflow_config.check_all_deps_for_multiple_deps_tests,
             ),
         )
         tasks_with_context = self._create_tasks_from_graph(dbt_airflow_graph)
         logging.info(f"Created {str(tasks_with_context.length())} tasks groups")
         return tasks_with_context
 
     def _create_dag_sensor(self, node: Dict[str, Any]) -> ModelExecutionTask:
```

### Comparing `dbt-airflow-factory-0.32.0/dbt_airflow_factory.egg-info/PKG-INFO` & `dbt-airflow-factory-0.33.0/dbt_airflow_factory.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,98 +1,100 @@
 Metadata-Version: 2.1
 Name: dbt-airflow-factory
-Version: 0.32.0
+Version: 0.33.0
 Summary: Library to convert DBT manifest metadata to Airflow tasks
 Home-page: https://github.com/getindata/dbt-airflow-factory/
 Author: Piotr Pekala
 Author-email: piotr.pekala@getindata.com
 License: Apache Software License (Apache 2.0)
-Description: # DBT Airflow Factory
-        
-        [![Python Version](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue)](https://github.com/getindata/dbt-airflow-factory)
-        [![PyPI Version](https://badge.fury.io/py/dbt-airflow-factory.svg)](https://pypi.org/project/dbt-airflow-factory/)
-        [![Downloads](https://pepy.tech/badge/dbt-airflow-factory)](https://pepy.tech/project/dbt-airflow-factory)
-        [![Maintainability](https://api.codeclimate.com/v1/badges/47fd3570c858b6c166ad/maintainability)](https://codeclimate.com/github/getindata/dbt-airflow-factory/maintainability)
-        [![Test Coverage](https://api.codeclimate.com/v1/badges/47fd3570c858b6c166ad/test_coverage)](https://codeclimate.com/github/getindata/dbt-airflow-factory/test_coverage)
-        [![Documentation Status](https://readthedocs.org/projects/dbt-airflow-factory/badge/?version=latest)](https://dbt-airflow-factory.readthedocs.io/en/latest/?badge=latest)
-        
-        Library to convert DBT manifest metadata to Airflow tasks
-        
-        ## Documentation
-        
-        Read the full documentation at [https://dbt-airflow-factory.readthedocs.io/](https://dbt-airflow-factory.readthedocs.io/en/latest/index.html)
-        
-        ## Installation
-        
-        Use the package manager [pip][pip] to install the library:
-        
-        ```bash
-        pip install dbt-airflow-factory
-        ```
-        
-        ## Usage
-        
-        The library is expected to be used inside an Airflow environment with a Kubernetes image referencing **dbt**.
-        
-        **dbt-airflow-factory**'s main task is to parse `manifest.json` and create Airflow DAG out of it. It also reads config
-        files from `config` directory and therefore is highly customizable (e.g., user can set path to `manifest.json`).
-        
-        To start, create a directory with a following structure, where `manifest.json` is a file generated by **dbt**:
-        ```
-        .
-        ├── config
-        │   ├── base
-        │   │   ├── airflow.yml
-        │   │   ├── dbt.yml
-        │   │   └── k8s.yml
-        │   └── dev
-        │       └── dbt.yml
-        ├── dag.py
-        └── manifest.json
-        ```
-        
-        Then, put the following code into `dag.py`:
-        ```python
-        from dbt_airflow_factory.airflow_dag_factory import AirflowDagFactory
-        from os import path
-        
-        dag = AirflowDagFactory(path.dirname(path.abspath(__file__)), "dev").create()
-        ```
-        
-        When uploaded to Airflow DAGs directory, it will get picked up by Airflow, parse `manifest.json` and prepare a DAG to run.
-        
-        ### Configuration files
-        
-        It is best to look up the example configuration files in [tests directory][tests] to get a glimpse of correct configs.
-        
-        You can use [Airflow template variables][airflow-vars] in your `dbt.yml` and `k8s.yml` files, as long as they are inside
-        quotation marks:
-        ```yaml
-        target: "{{ var.value.env }}"
-        some_other_field: "{{ ds_nodash }}"
-        ```
-        
-        Analogously, you can use `"{{ var.value.VARIABLE_NAME }}"` in `airflow.yml`, but only the Airflow variable getter.
-        Any other Airflow template variables will not work in `airflow.yml`.
-        
-        ### Creation of the directory with data-pipelines-cli
-        
-        **DBT Airflow Factory** works best in tandem with [data-pipelines-cli][dp-cli] tool. **dp** not only prepares directory
-        for the library to digest, but also automates Docker image building and pushes generated directory to the cloud storage
-        of your choice.
-        
-        [airflow-vars]: https://airflow.apache.org/docs/apache-airflow/stable/templates-ref.html#variables
-        [dp-cli]: https://pypi.org/project/data-pipelines-cli/
-        [pip]: https://pip.pypa.io/en/stable/
-        [tests]: https://github.com/getindata/dbt-airflow-factory/tree/develop/tests/config
-        
 Keywords: dbt airflow manifest parser python
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 Provides-Extra: docs
+License-File: LICENSE
+
+# DBT Airflow Factory
+
+[![Python Version](https://img.shields.io/badge/python-3.9%20%7C%203.10%20%7C%203.11-blue)](https://github.com/getindata/dbt-airflow-factory)
+[![PyPI Version](https://badge.fury.io/py/dbt-airflow-factory.svg)](https://pypi.org/project/dbt-airflow-factory/)
+[![Downloads](https://pepy.tech/badge/dbt-airflow-factory)](https://pepy.tech/project/dbt-airflow-factory)
+[![Maintainability](https://api.codeclimate.com/v1/badges/47fd3570c858b6c166ad/maintainability)](https://codeclimate.com/github/getindata/dbt-airflow-factory/maintainability)
+[![Test Coverage](https://api.codeclimate.com/v1/badges/47fd3570c858b6c166ad/test_coverage)](https://codeclimate.com/github/getindata/dbt-airflow-factory/test_coverage)
+[![Documentation Status](https://readthedocs.org/projects/dbt-airflow-factory/badge/?version=latest)](https://dbt-airflow-factory.readthedocs.io/en/latest/?badge=latest)
+
+Library to convert DBT manifest metadata to Airflow tasks
+
+## Documentation
+
+Read the full documentation at [https://dbt-airflow-factory.readthedocs.io/](https://dbt-airflow-factory.readthedocs.io/en/latest/index.html)
+
+## Installation
+
+Use the package manager [pip][pip] to install the library:
+
+```bash
+pip install dbt-airflow-factory
+```
+
+## Usage
+
+The library is expected to be used inside an Airflow environment with a Kubernetes image referencing **dbt**.
+
+**dbt-airflow-factory**'s main task is to parse `manifest.json` and create Airflow DAG out of it. It also reads config
+files from `config` directory and therefore is highly customizable (e.g., user can set path to `manifest.json`).
+
+To start, create a directory with a following structure, where `manifest.json` is a file generated by **dbt**:
+```
+.
+├── config
+│   ├── base
+│   │   ├── airflow.yml
+│   │   ├── dbt.yml
+│   │   └── k8s.yml
+│   └── dev
+│       └── dbt.yml
+├── dag.py
+└── manifest.json
+```
+
+Then, put the following code into `dag.py`:
+```python
+from dbt_airflow_factory.airflow_dag_factory import AirflowDagFactory
+from os import path
+
+dag = AirflowDagFactory(path.dirname(path.abspath(__file__)), "dev").create()
+```
+
+When uploaded to Airflow DAGs directory, it will get picked up by Airflow, parse `manifest.json` and prepare a DAG to run.
+
+### Configuration files
+
+It is best to look up the example configuration files in [tests directory][tests] to get a glimpse of correct configs.
+
+You can use [Airflow template variables][airflow-vars] in your `dbt.yml` and `k8s.yml` files, as long as they are inside
+quotation marks:
+```yaml
+target: "{{ var.value.env }}"
+some_other_field: "{{ ds_nodash }}"
+```
+
+Analogously, you can use `"{{ var.value.VARIABLE_NAME }}"` in `airflow.yml`, but only the Airflow variable getter.
+Any other Airflow template variables will not work in `airflow.yml`.
+
+### Creation of the directory with data-pipelines-cli
+
+**DBT Airflow Factory** works best in tandem with [data-pipelines-cli][dp-cli] tool. **dp** not only prepares directory
+for the library to digest, but also automates Docker image building and pushes generated directory to the cloud storage
+of your choice.
+
+[airflow-vars]: https://airflow.apache.org/docs/apache-airflow/stable/templates-ref.html#variables
+[dp-cli]: https://pypi.org/project/data-pipelines-cli/
+[pip]: https://pip.pypa.io/en/stable/
+[tests]: https://github.com/getindata/dbt-airflow-factory/tree/develop/tests/config
+
+
```

### Comparing `dbt-airflow-factory-0.32.0/dbt_airflow_factory.egg-info/SOURCES.txt` & `dbt-airflow-factory-0.33.0/dbt_airflow_factory.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbt-airflow-factory-0.32.0/setup.cfg` & `dbt-airflow-factory-0.33.0/setup.cfg`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [bumpversion]
-current_version = 0.32.0
+current_version = 0.33.0
 
 [bumpversion:file:setup.py]
 
 [bumpversion:file:dbt_airflow_factory/__init__.py]
 
 [flake8]
 exclude = .git,__pycache__,build,dist,docs/source/conf.py
-max-line-length = 100
+max-line-length = 120
 extend-ignore = E203
 
 [mypy]
 ignore_missing_imports = True
 follow_imports = silent
 strict_optional = True
 no_implicit_optional = True
```

### Comparing `dbt-airflow-factory-0.32.0/setup.py` & `dbt-airflow-factory-0.33.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,49 +3,48 @@
 from setuptools import find_packages, setup
 
 with open("README.md") as f:
     README = f.read()
 
 # Runtime Requirements.
 INSTALL_REQUIRES = [
-    "pytimeparse==1.1.8",
-    "dbt-graph-builder>=0.3.0",
+    "pytimeparse>=1.1, <2",
+    "dbt-graph-builder>=0.6.3, <2",
+    "apache-airflow[kubernetes,slack]>=2.5, <3",
+    "apache-airflow-providers-airbyte>=3.1, <4",
 ]
 
 # Dev Requirements
 EXTRA_REQUIRE = {
     "tests": [
         "pytest>=6.2.2, <7.0.0",
         "pytest-cov>=2.8.0, <3.0.0",
         "tox==3.21.1",
         "pre-commit==2.9.3",
-        "pandas==1.2.5",
-        "apache-airflow[kubernetes,slack]==2.5.2",
-        "apache-airflow-providers-airbyte==3.1.0",
+        "pandas>=1.2.5, <2.0.0",
     ],
     "docs": [
         "sphinx==4.3.1",
         "sphinx-rtd-theme==1.0.0",
         "sphinx-click>=3.0,<3.1",
         "myst-parser>=0.16, <0.17",
         "docutils<0.17",
     ],
 }
 
 setup(
     name="dbt-airflow-factory",
-    version="0.32.0",
+    version="0.33.0",
     description="Library to convert DBT manifest metadata to Airflow tasks",
     long_description=README,
     long_description_content_type="text/markdown",
     license="Apache Software License (Apache 2.0)",
     python_requires=">=3",
     classifiers=[
         "Development Status :: 3 - Alpha",
-        "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
     ],
     keywords="dbt airflow manifest parser python",
     author="Piotr Pekala",
     author_email="piotr.pekala@getindata.com",
```

