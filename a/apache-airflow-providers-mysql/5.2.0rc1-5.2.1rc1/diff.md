# Comparing `tmp/apache-airflow-providers-mysql-5.2.0rc1.tar.gz` & `tmp/apache-airflow-providers-mysql-5.2.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-mysql-5.2.0rc1.tar", last modified: Sat Jul 29 12:08:45 2023, max compression
+gzip compressed data, was "apache-airflow-providers-mysql-5.2.1rc1.tar", last modified: Fri Aug  4 21:41:25 2023, max compression
```

## Comparing `apache-airflow-providers-mysql-5.2.0rc1.tar` & `apache-airflow-providers-mysql-5.2.1rc1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:45.227311 apache-airflow-providers-mysql-5.2.0rc1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-mysql-5.2.0rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-07-29 12:08:44.000000 apache-airflow-providers-mysql-5.2.0rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-mysql-5.2.0rc1/NOTICE
--rw-r--r--   0 root         (0) root         (0)     6423 2023-07-29 12:08:45.228022 apache-airflow-providers-mysql-5.2.0rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4603 2023-07-29 12:08:44.000000 apache-airflow-providers-mysql-5.2.0rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:45.133757 apache-airflow-providers-mysql-5.2.0rc1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:45.134899 apache-airflow-providers-mysql-5.2.0rc1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:45.169049 apache-airflow-providers-mysql-5.2.0rc1/airflow/providers/mysql/
--rw-r--r--   0 root         (0) root         (0)     1574 2023-07-29 12:01:19.000000 apache-airflow-providers-mysql-5.2.0rc1/airflow/providers/mysql/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3790 2023-07-29 12:08:44.000000 apache-airflow-providers-mysql-5.2.0rc1/airflow/providers/mysql/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:45.174888 apache-airflow-providers-mysql-5.2.0rc1/airflow/providers/mysql/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-mysql-5.2.0rc1/airflow/providers/mysql/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12988 2023-07-26 06:59:50.000000 apache-airflow-providers-mysql-5.2.0rc1/airflow/providers/mysql/hooks/mysql.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:45.181079 apache-airflow-providers-mysql-5.2.0rc1/airflow/providers/mysql/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-mysql-5.2.0rc1/airflow/providers/mysql/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2987 2023-07-16 17:25:26.000000 apache-airflow-providers-mysql-5.2.0rc1/airflow/providers/mysql/operators/mysql.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:45.195588 apache-airflow-providers-mysql-5.2.0rc1/airflow/providers/mysql/transfers/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-mysql-5.2.0rc1/airflow/providers/mysql/transfers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3269 2023-07-05 07:19:39.000000 apache-airflow-providers-mysql-5.2.0rc1/airflow/providers/mysql/transfers/presto_to_mysql.py
--rw-r--r--   0 root         (0) root         (0)     3558 2023-06-01 06:14:28.000000 apache-airflow-providers-mysql-5.2.0rc1/airflow/providers/mysql/transfers/s3_to_mysql.py
--rw-r--r--   0 root         (0) root         (0)     3251 2023-07-05 07:19:39.000000 apache-airflow-providers-mysql-5.2.0rc1/airflow/providers/mysql/transfers/trino_to_mysql.py
--rw-r--r--   0 root         (0) root         (0)     6455 2023-06-08 05:42:54.000000 apache-airflow-providers-mysql-5.2.0rc1/airflow/providers/mysql/transfers/vertica_to_mysql.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:45.224156 apache-airflow-providers-mysql-5.2.0rc1/apache_airflow_providers_mysql.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6423 2023-07-29 12:08:45.000000 apache-airflow-providers-mysql-5.2.0rc1/apache_airflow_providers_mysql.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      955 2023-07-29 12:08:45.000000 apache-airflow-providers-mysql-5.2.0rc1/apache_airflow_providers_mysql.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:08:45.000000 apache-airflow-providers-mysql-5.2.0rc1/apache_airflow_providers_mysql.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      102 2023-07-29 12:08:45.000000 apache-airflow-providers-mysql-5.2.0rc1/apache_airflow_providers_mysql.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:08:45.000000 apache-airflow-providers-mysql-5.2.0rc1/apache_airflow_providers_mysql.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      421 2023-07-29 12:08:45.000000 apache-airflow-providers-mysql-5.2.0rc1/apache_airflow_providers_mysql.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-07-29 12:08:45.000000 apache-airflow-providers-mysql-5.2.0rc1/apache_airflow_providers_mysql.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5011 2023-07-27 05:54:58.000000 apache-airflow-providers-mysql-5.2.0rc1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1987 2023-07-29 12:08:45.230492 apache-airflow-providers-mysql-5.2.0rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2087 2023-07-29 12:08:44.000000 apache-airflow-providers-mysql-5.2.0rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:41:25.637020 apache-airflow-providers-mysql-5.2.1rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-mysql-5.2.1rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-08-04 21:41:24.000000 apache-airflow-providers-mysql-5.2.1rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-mysql-5.2.1rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     6477 2023-08-04 21:41:25.637621 apache-airflow-providers-mysql-5.2.1rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4657 2023-08-04 21:41:24.000000 apache-airflow-providers-mysql-5.2.1rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:41:25.534779 apache-airflow-providers-mysql-5.2.1rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:41:25.535758 apache-airflow-providers-mysql-5.2.1rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:41:25.574882 apache-airflow-providers-mysql-5.2.1rc1/airflow/providers/mysql/
+-rw-r--r--   0 root         (0) root         (0)     1574 2023-08-04 21:33:34.000000 apache-airflow-providers-mysql-5.2.1rc1/airflow/providers/mysql/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3803 2023-08-04 21:41:24.000000 apache-airflow-providers-mysql-5.2.1rc1/airflow/providers/mysql/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:41:25.582336 apache-airflow-providers-mysql-5.2.1rc1/airflow/providers/mysql/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-mysql-5.2.1rc1/airflow/providers/mysql/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12988 2023-07-26 06:59:50.000000 apache-airflow-providers-mysql-5.2.1rc1/airflow/providers/mysql/hooks/mysql.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:41:25.589048 apache-airflow-providers-mysql-5.2.1rc1/airflow/providers/mysql/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-mysql-5.2.1rc1/airflow/providers/mysql/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2987 2023-07-16 17:25:26.000000 apache-airflow-providers-mysql-5.2.1rc1/airflow/providers/mysql/operators/mysql.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:41:25.605973 apache-airflow-providers-mysql-5.2.1rc1/airflow/providers/mysql/transfers/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-mysql-5.2.1rc1/airflow/providers/mysql/transfers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3269 2023-07-05 07:19:39.000000 apache-airflow-providers-mysql-5.2.1rc1/airflow/providers/mysql/transfers/presto_to_mysql.py
+-rw-r--r--   0 root         (0) root         (0)     3558 2023-06-01 06:14:28.000000 apache-airflow-providers-mysql-5.2.1rc1/airflow/providers/mysql/transfers/s3_to_mysql.py
+-rw-r--r--   0 root         (0) root         (0)     3251 2023-07-05 07:19:39.000000 apache-airflow-providers-mysql-5.2.1rc1/airflow/providers/mysql/transfers/trino_to_mysql.py
+-rw-r--r--   0 root         (0) root         (0)     6455 2023-06-08 05:42:54.000000 apache-airflow-providers-mysql-5.2.1rc1/airflow/providers/mysql/transfers/vertica_to_mysql.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:41:25.633814 apache-airflow-providers-mysql-5.2.1rc1/apache_airflow_providers_mysql.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6477 2023-08-04 21:41:25.000000 apache-airflow-providers-mysql-5.2.1rc1/apache_airflow_providers_mysql.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      955 2023-08-04 21:41:25.000000 apache-airflow-providers-mysql-5.2.1rc1/apache_airflow_providers_mysql.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 21:41:25.000000 apache-airflow-providers-mysql-5.2.1rc1/apache_airflow_providers_mysql.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      102 2023-08-04 21:41:25.000000 apache-airflow-providers-mysql-5.2.1rc1/apache_airflow_providers_mysql.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 21:41:25.000000 apache-airflow-providers-mysql-5.2.1rc1/apache_airflow_providers_mysql.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      421 2023-08-04 21:41:25.000000 apache-airflow-providers-mysql-5.2.1rc1/apache_airflow_providers_mysql.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-08-04 21:41:25.000000 apache-airflow-providers-mysql-5.2.1rc1/apache_airflow_providers_mysql.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5031 2023-08-04 10:24:23.000000 apache-airflow-providers-mysql-5.2.1rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     2019 2023-08-04 21:41:25.639525 apache-airflow-providers-mysql-5.2.1rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2055 2023-08-04 21:41:24.000000 apache-airflow-providers-mysql-5.2.1rc1/setup.py
```

### Comparing `apache-airflow-providers-mysql-5.2.0rc1/LICENSE` & `apache-airflow-providers-mysql-5.2.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-mysql-5.2.0rc1/MANIFEST.in` & `apache-airflow-providers-mysql-5.2.1rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-mysql-5.2.0rc1/PKG-INFO` & `apache-airflow-providers-mysql-5.2.1rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-mysql
-Version: 5.2.0rc1
+Version: 5.2.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-mysql package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-mysql/5.2.0/
-Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-mysql/5.2.0/changelog.html
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-mysql/5.2.1/
+Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-mysql/5.2.1/changelog.html
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -73,28 +73,28 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-mysql``
 
-Release: ``5.2.0rc1``
+Release: ``5.2.1rc1``
 
 
 `MySQL <https://www.mysql.com/products/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``mysql`` provider. All classes for this provider package
 are in ``airflow.providers.mysql`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-mysql/5.2.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-mysql/5.2.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -107,14 +107,15 @@
 
 =======================================  ==================
 PIP package                              Version required
 =======================================  ==================
 ``apache-airflow``                       ``>=2.4.0``
 ``apache-airflow-providers-common-sql``  ``>=1.3.1``
 ``mysqlclient``                          ``>=1.3.6``
+``mysql-connector-python``               ``>=8.0.11``
 =======================================  ==================
 
 Cross provider package dependencies
 -----------------------------------
 
 Those are dependencies that might be needed in order to use all the features of the package.
 You need to install the specified provider packages in order to use them.
@@ -134,8 +135,8 @@
 `apache-airflow-providers-openlineage <https://airflow.apache.org/docs/apache-airflow-providers-openlineage>`_  ``openlineage``
 `apache-airflow-providers-presto <https://airflow.apache.org/docs/apache-airflow-providers-presto>`_            ``presto``
 `apache-airflow-providers-trino <https://airflow.apache.org/docs/apache-airflow-providers-trino>`_              ``trino``
 `apache-airflow-providers-vertica <https://airflow.apache.org/docs/apache-airflow-providers-vertica>`_          ``vertica``
 ==============================================================================================================  ===============
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-mysql/5.2.0/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-mysql/5.2.1/changelog.html>`_.
```

### Comparing `apache-airflow-providers-mysql-5.2.0rc1/README.rst` & `apache-airflow-providers-mysql-5.2.1rc1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -32,28 +32,28 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-mysql``
 
-Release: ``5.2.0rc1``
+Release: ``5.2.1rc1``
 
 
 `MySQL <https://www.mysql.com/products/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``mysql`` provider. All classes for this provider package
 are in ``airflow.providers.mysql`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-mysql/5.2.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-mysql/5.2.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -66,14 +66,15 @@
 
 =======================================  ==================
 PIP package                              Version required
 =======================================  ==================
 ``apache-airflow``                       ``>=2.4.0``
 ``apache-airflow-providers-common-sql``  ``>=1.3.1``
 ``mysqlclient``                          ``>=1.3.6``
+``mysql-connector-python``               ``>=8.0.11``
 =======================================  ==================
 
 Cross provider package dependencies
 -----------------------------------
 
 Those are dependencies that might be needed in order to use all the features of the package.
 You need to install the specified provider packages in order to use them.
@@ -93,8 +94,8 @@
 `apache-airflow-providers-openlineage <https://airflow.apache.org/docs/apache-airflow-providers-openlineage>`_  ``openlineage``
 `apache-airflow-providers-presto <https://airflow.apache.org/docs/apache-airflow-providers-presto>`_            ``presto``
 `apache-airflow-providers-trino <https://airflow.apache.org/docs/apache-airflow-providers-trino>`_              ``trino``
 `apache-airflow-providers-vertica <https://airflow.apache.org/docs/apache-airflow-providers-vertica>`_          ``vertica``
 ==============================================================================================================  ===============
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-mysql/5.2.0/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-mysql/5.2.1/changelog.html>`_.
```

### Comparing `apache-airflow-providers-mysql-5.2.0rc1/airflow/providers/mysql/__init__.py` & `apache-airflow-providers-mysql-5.2.1rc1/airflow/providers/mysql/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 from __future__ import annotations
 
 import packaging.version
 
 __all__ = ["__version__"]
 
-__version__ = "5.2.0"
+__version__ = "5.2.1"
 
 try:
     from airflow import __version__ as airflow_version
 except ImportError:
     from airflow.version import version as airflow_version
 
 if packaging.version.parse(packaging.version.parse(airflow_version).base_version) < packaging.version.parse(
```

### Comparing `apache-airflow-providers-mysql-5.2.0rc1/airflow/providers/mysql/get_provider_info.py` & `apache-airflow-providers-mysql-5.2.1rc1/airflow/providers/mysql/get_provider_info.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-mysql",
         "name": "MySQL",
         "description": "`MySQL <https://www.mysql.com/products/>`__\n",
         "suspended": False,
         "versions": [
+            "5.2.1",
             "5.2.0",
             "5.1.1",
             "5.1.0",
             "5.0.0",
             "4.0.2",
             "4.0.1",
             "4.0.0",
@@ -54,14 +55,15 @@
             "1.0.1",
             "1.0.0",
         ],
         "dependencies": [
             "apache-airflow>=2.4.0",
             "apache-airflow-providers-common-sql>=1.3.1",
             "mysqlclient>=1.3.6",
+            "mysql-connector-python>=8.0.11",
         ],
         "integrations": [
             {
                 "integration-name": "MySQL",
                 "external-doc-url": "https://www.mysql.com/",
                 "how-to-guide": ["/docs/apache-airflow-providers-mysql/operators.rst"],
                 "logo": "/integration-logos/mysql/MySQL.png",
@@ -93,11 +95,9 @@
                 "target-integration-name": "MySQL",
                 "python-module": "airflow.providers.mysql.transfers.trino_to_mysql",
             },
         ],
         "connection-types": [
             {"hook-class-name": "airflow.providers.mysql.hooks.mysql.MySqlHook", "connection-type": "mysql"}
         ],
-        "additional-extras": [
-            {"name": "mysql-connector-python", "dependencies": ["mysql-connector-python>=8.0.11"]}
-        ],
+        "additional-extras": [{"name": "mysql-connector-python", "dependencies": []}],
     }
```

### Comparing `apache-airflow-providers-mysql-5.2.0rc1/airflow/providers/mysql/hooks/__init__.py` & `apache-airflow-providers-mysql-5.2.1rc1/airflow/providers/mysql/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-mysql-5.2.0rc1/airflow/providers/mysql/hooks/mysql.py` & `apache-airflow-providers-mysql-5.2.1rc1/airflow/providers/mysql/hooks/mysql.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-mysql-5.2.0rc1/airflow/providers/mysql/operators/__init__.py` & `apache-airflow-providers-mysql-5.2.1rc1/airflow/providers/mysql/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-mysql-5.2.0rc1/airflow/providers/mysql/operators/mysql.py` & `apache-airflow-providers-mysql-5.2.1rc1/airflow/providers/mysql/operators/mysql.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-mysql-5.2.0rc1/airflow/providers/mysql/transfers/__init__.py` & `apache-airflow-providers-mysql-5.2.1rc1/airflow/providers/mysql/transfers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-mysql-5.2.0rc1/airflow/providers/mysql/transfers/presto_to_mysql.py` & `apache-airflow-providers-mysql-5.2.1rc1/airflow/providers/mysql/transfers/presto_to_mysql.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-mysql-5.2.0rc1/airflow/providers/mysql/transfers/s3_to_mysql.py` & `apache-airflow-providers-mysql-5.2.1rc1/airflow/providers/mysql/transfers/s3_to_mysql.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-mysql-5.2.0rc1/airflow/providers/mysql/transfers/trino_to_mysql.py` & `apache-airflow-providers-mysql-5.2.1rc1/airflow/providers/mysql/transfers/trino_to_mysql.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-mysql-5.2.0rc1/airflow/providers/mysql/transfers/vertica_to_mysql.py` & `apache-airflow-providers-mysql-5.2.1rc1/airflow/providers/mysql/transfers/vertica_to_mysql.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-mysql-5.2.0rc1/apache_airflow_providers_mysql.egg-info/PKG-INFO` & `apache-airflow-providers-mysql-5.2.1rc1/apache_airflow_providers_mysql.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-mysql
-Version: 5.2.0rc1
+Version: 5.2.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-mysql package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-mysql/5.2.0/
-Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-mysql/5.2.0/changelog.html
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-mysql/5.2.1/
+Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-mysql/5.2.1/changelog.html
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -73,28 +73,28 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-mysql``
 
-Release: ``5.2.0rc1``
+Release: ``5.2.1rc1``
 
 
 `MySQL <https://www.mysql.com/products/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``mysql`` provider. All classes for this provider package
 are in ``airflow.providers.mysql`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-mysql/5.2.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-mysql/5.2.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -107,14 +107,15 @@
 
 =======================================  ==================
 PIP package                              Version required
 =======================================  ==================
 ``apache-airflow``                       ``>=2.4.0``
 ``apache-airflow-providers-common-sql``  ``>=1.3.1``
 ``mysqlclient``                          ``>=1.3.6``
+``mysql-connector-python``               ``>=8.0.11``
 =======================================  ==================
 
 Cross provider package dependencies
 -----------------------------------
 
 Those are dependencies that might be needed in order to use all the features of the package.
 You need to install the specified provider packages in order to use them.
@@ -134,8 +135,8 @@
 `apache-airflow-providers-openlineage <https://airflow.apache.org/docs/apache-airflow-providers-openlineage>`_  ``openlineage``
 `apache-airflow-providers-presto <https://airflow.apache.org/docs/apache-airflow-providers-presto>`_            ``presto``
 `apache-airflow-providers-trino <https://airflow.apache.org/docs/apache-airflow-providers-trino>`_              ``trino``
 `apache-airflow-providers-vertica <https://airflow.apache.org/docs/apache-airflow-providers-vertica>`_          ``vertica``
 ==============================================================================================================  ===============
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-mysql/5.2.0/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-mysql/5.2.1/changelog.html>`_.
```

### Comparing `apache-airflow-providers-mysql-5.2.0rc1/apache_airflow_providers_mysql.egg-info/SOURCES.txt` & `apache-airflow-providers-mysql-5.2.1rc1/apache_airflow_providers_mysql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-mysql-5.2.0rc1/pyproject.toml` & `apache-airflow-providers-mysql-5.2.1rc1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -99,14 +99,15 @@
     # https://github.com/dpgaspar/Flask-AppBuilder/pull/1940
     "ignore::DeprecationWarning:flask_sqlalchemy",
     # https://github.com/dpgaspar/Flask-AppBuilder/pull/1903
     "ignore::DeprecationWarning:apispec.utils",
 ]
 python_files = [
     "test_*.py",
+    "example_*.py",
 ]
 testpaths = [
     "tests",
 ]
 
 [tool.ruff.isort]
 required-imports = ["from __future__ import annotations"]
```

### Comparing `apache-airflow-providers-mysql-5.2.0rc1/setup.cfg` & `apache-airflow-providers-mysql-5.2.1rc1/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -23,16 +23,16 @@
 	License :: OSI Approved :: Apache Software License
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	Topic :: System :: Monitoring
 project_urls = 
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-mysql/5.2.0/
-	Changelog=https://airflow.apache.org/docs/apache-airflow-providers-mysql/5.2.0/changelog.html
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-mysql/5.2.1/
+	Changelog=https://airflow.apache.org/docs/apache-airflow-providers-mysql/5.2.1/changelog.html
 	Bug Tracker=https://github.com/apache/airflow/issues
 	Source Code=https://github.com/apache/airflow
 	Slack Chat=https://s.apache.org/airflow-slack
 	Twitter=https://twitter.com/ApacheAirflow
 	YouTube=https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 
 [bdist_wheel]
@@ -45,14 +45,15 @@
 packages = find:
 setup_requires = 
 	setuptools
 	wheel
 install_requires = 
 	apache-airflow-providers-common-sql>=1.3.1.dev0
 	apache-airflow>=2.4.0.dev0
+	mysql-connector-python>=8.0.11
 	mysqlclient>=1.3.6
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.mysql.get_provider_info:get_provider_info
 
 [files]
```

### Comparing `apache-airflow-providers-mysql-5.2.0rc1/setup.py` & `apache-airflow-providers-mysql-5.2.1rc1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,29 +22,29 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-mysql package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "5.2.0"
+version = "5.2.1"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-mysql setup."""
     setup(
         version=version,
         extras_require={
             "amazon": ["apache-airflow-providers-amazon"],
             "common.sql": ["apache-airflow-providers-common-sql"],
             "openlineage": ["apache-airflow-providers-openlineage"],
             "presto": ["apache-airflow-providers-presto"],
             "trino": ["apache-airflow-providers-trino"],
             "vertica": ["apache-airflow-providers-vertica"],
-            "mysql-connector-python": ["mysql-connector-python>=8.0.11"],
+            "mysql-connector-python": [],
         },
         packages=find_namespace_packages(
             include=[
                 "airflow.providers.mysql",
                 "airflow.providers.mysql.*",
                 "airflow.providers.mysql_vendor",
                 "airflow.providers.mysql_vendor.*",
```

