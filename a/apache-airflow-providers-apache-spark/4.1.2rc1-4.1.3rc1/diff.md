# Comparing `tmp/apache-airflow-providers-apache-spark-4.1.2rc1.tar.gz` & `tmp/apache-airflow-providers-apache-spark-4.1.3rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-apache-spark-4.1.2rc1.tar", last modified: Sat Jul 29 12:08:04 2023, max compression
+gzip compressed data, was "apache-airflow-providers-apache-spark-4.1.3rc1.tar", last modified: Fri Aug  4 21:40:46 2023, max compression
```

## Comparing `apache-airflow-providers-apache-spark-4.1.2rc1.tar` & `apache-airflow-providers-apache-spark-4.1.3rc1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:04.723019 apache-airflow-providers-apache-spark-4.1.2rc1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-spark-4.1.2rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-07-29 12:08:03.000000 apache-airflow-providers-apache-spark-4.1.2rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-spark-4.1.2rc1/NOTICE
--rw-r--r--   0 root         (0) root         (0)     5594 2023-07-29 12:08:04.723680 apache-airflow-providers-apache-spark-4.1.2rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3900 2023-07-29 12:08:03.000000 apache-airflow-providers-apache-spark-4.1.2rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:04.634056 apache-airflow-providers-apache-spark-4.1.2rc1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:04.635118 apache-airflow-providers-apache-spark-4.1.2rc1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:04.636143 apache-airflow-providers-apache-spark-4.1.2rc1/airflow/providers/apache/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:04.666849 apache-airflow-providers-apache-spark-4.1.2rc1/airflow/providers/apache/spark/
--rw-r--r--   0 root         (0) root         (0)     1581 2023-07-29 12:01:19.000000 apache-airflow-providers-apache-spark-4.1.2rc1/airflow/providers/apache/spark/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3688 2023-07-29 12:08:03.000000 apache-airflow-providers-apache-spark-4.1.2rc1/airflow/providers/apache/spark/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:04.681199 apache-airflow-providers-apache-spark-4.1.2rc1/airflow/providers/apache/spark/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-spark-4.1.2rc1/airflow/providers/apache/spark/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11356 2023-06-29 05:49:30.000000 apache-airflow-providers-apache-spark-4.1.2rc1/airflow/providers/apache/spark/hooks/spark_jdbc.py
--rw-r--r--   0 root         (0) root         (0)     6753 2023-06-01 07:44:14.000000 apache-airflow-providers-apache-spark-4.1.2rc1/airflow/providers/apache/spark/hooks/spark_jdbc_script.py
--rw-r--r--   0 root         (0) root         (0)     7037 2023-06-29 05:49:30.000000 apache-airflow-providers-apache-spark-4.1.2rc1/airflow/providers/apache/spark/hooks/spark_sql.py
--rw-r--r--   0 root         (0) root         (0)    28687 2023-07-26 06:59:50.000000 apache-airflow-providers-apache-spark-4.1.2rc1/airflow/providers/apache/spark/hooks/spark_submit.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:04.692959 apache-airflow-providers-apache-spark-4.1.2rc1/airflow/providers/apache/spark/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-spark-4.1.2rc1/airflow/providers/apache/spark/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9935 2023-06-29 05:49:30.000000 apache-airflow-providers-apache-spark-4.1.2rc1/airflow/providers/apache/spark/operators/spark_jdbc.py
--rw-r--r--   0 root         (0) root         (0)     4508 2023-06-01 07:44:14.000000 apache-airflow-providers-apache-spark-4.1.2rc1/airflow/providers/apache/spark/operators/spark_sql.py
--rw-r--r--   0 root         (0) root         (0)     8370 2023-06-29 05:49:30.000000 apache-airflow-providers-apache-spark-4.1.2rc1/airflow/providers/apache/spark/operators/spark_submit.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:04.720342 apache-airflow-providers-apache-spark-4.1.2rc1/apache_airflow_providers_apache_spark.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5594 2023-07-29 12:08:04.000000 apache-airflow-providers-apache-spark-4.1.2rc1/apache_airflow_providers_apache_spark.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1074 2023-07-29 12:08:04.000000 apache-airflow-providers-apache-spark-4.1.2rc1/apache_airflow_providers_apache_spark.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:08:04.000000 apache-airflow-providers-apache-spark-4.1.2rc1/apache_airflow_providers_apache_spark.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      109 2023-07-29 12:08:04.000000 apache-airflow-providers-apache-spark-4.1.2rc1/apache_airflow_providers_apache_spark.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:08:04.000000 apache-airflow-providers-apache-spark-4.1.2rc1/apache_airflow_providers_apache_spark.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      102 2023-07-29 12:08:04.000000 apache-airflow-providers-apache-spark-4.1.2rc1/apache_airflow_providers_apache_spark.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-07-29 12:08:04.000000 apache-airflow-providers-apache-spark-4.1.2rc1/apache_airflow_providers_apache_spark.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5011 2023-07-27 05:54:58.000000 apache-airflow-providers-apache-spark-4.1.2rc1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1976 2023-07-29 12:08:04.725683 apache-airflow-providers-apache-spark-4.1.2rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1744 2023-07-29 12:08:03.000000 apache-airflow-providers-apache-spark-4.1.2rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:40:46.135375 apache-airflow-providers-apache-spark-4.1.3rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-spark-4.1.3rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-08-04 21:40:45.000000 apache-airflow-providers-apache-spark-4.1.3rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-spark-4.1.3rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     5594 2023-08-04 21:40:46.135906 apache-airflow-providers-apache-spark-4.1.3rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3900 2023-08-04 21:40:45.000000 apache-airflow-providers-apache-spark-4.1.3rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:40:46.048141 apache-airflow-providers-apache-spark-4.1.3rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:40:46.049292 apache-airflow-providers-apache-spark-4.1.3rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:40:46.050266 apache-airflow-providers-apache-spark-4.1.3rc1/airflow/providers/apache/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:40:46.081304 apache-airflow-providers-apache-spark-4.1.3rc1/airflow/providers/apache/spark/
+-rw-r--r--   0 root         (0) root         (0)     1581 2023-08-04 21:33:34.000000 apache-airflow-providers-apache-spark-4.1.3rc1/airflow/providers/apache/spark/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3709 2023-08-04 21:40:45.000000 apache-airflow-providers-apache-spark-4.1.3rc1/airflow/providers/apache/spark/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:40:46.095656 apache-airflow-providers-apache-spark-4.1.3rc1/airflow/providers/apache/spark/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-spark-4.1.3rc1/airflow/providers/apache/spark/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11492 2023-08-04 10:24:22.000000 apache-airflow-providers-apache-spark-4.1.3rc1/airflow/providers/apache/spark/hooks/spark_jdbc.py
+-rw-r--r--   0 root         (0) root         (0)     6753 2023-06-01 07:44:14.000000 apache-airflow-providers-apache-spark-4.1.3rc1/airflow/providers/apache/spark/hooks/spark_jdbc_script.py
+-rw-r--r--   0 root         (0) root         (0)     7037 2023-06-29 05:49:30.000000 apache-airflow-providers-apache-spark-4.1.3rc1/airflow/providers/apache/spark/hooks/spark_sql.py
+-rw-r--r--   0 root         (0) root         (0)    28687 2023-07-26 06:59:50.000000 apache-airflow-providers-apache-spark-4.1.3rc1/airflow/providers/apache/spark/hooks/spark_submit.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:40:46.107202 apache-airflow-providers-apache-spark-4.1.3rc1/airflow/providers/apache/spark/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-spark-4.1.3rc1/airflow/providers/apache/spark/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9935 2023-06-29 05:49:30.000000 apache-airflow-providers-apache-spark-4.1.3rc1/airflow/providers/apache/spark/operators/spark_jdbc.py
+-rw-r--r--   0 root         (0) root         (0)     4508 2023-06-01 07:44:14.000000 apache-airflow-providers-apache-spark-4.1.3rc1/airflow/providers/apache/spark/operators/spark_sql.py
+-rw-r--r--   0 root         (0) root         (0)     8370 2023-06-29 05:49:30.000000 apache-airflow-providers-apache-spark-4.1.3rc1/airflow/providers/apache/spark/operators/spark_submit.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:40:46.133107 apache-airflow-providers-apache-spark-4.1.3rc1/apache_airflow_providers_apache_spark.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5594 2023-08-04 21:40:45.000000 apache-airflow-providers-apache-spark-4.1.3rc1/apache_airflow_providers_apache_spark.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1074 2023-08-04 21:40:46.000000 apache-airflow-providers-apache-spark-4.1.3rc1/apache_airflow_providers_apache_spark.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 21:40:45.000000 apache-airflow-providers-apache-spark-4.1.3rc1/apache_airflow_providers_apache_spark.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      109 2023-08-04 21:40:45.000000 apache-airflow-providers-apache-spark-4.1.3rc1/apache_airflow_providers_apache_spark.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 21:40:45.000000 apache-airflow-providers-apache-spark-4.1.3rc1/apache_airflow_providers_apache_spark.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      102 2023-08-04 21:40:45.000000 apache-airflow-providers-apache-spark-4.1.3rc1/apache_airflow_providers_apache_spark.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-08-04 21:40:45.000000 apache-airflow-providers-apache-spark-4.1.3rc1/apache_airflow_providers_apache_spark.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5031 2023-08-04 10:24:23.000000 apache-airflow-providers-apache-spark-4.1.3rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1976 2023-08-04 21:40:46.137691 apache-airflow-providers-apache-spark-4.1.3rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1744 2023-08-04 21:40:45.000000 apache-airflow-providers-apache-spark-4.1.3rc1/setup.py
```

### Comparing `apache-airflow-providers-apache-spark-4.1.2rc1/LICENSE` & `apache-airflow-providers-apache-spark-4.1.3rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-spark-4.1.2rc1/MANIFEST.in` & `apache-airflow-providers-apache-spark-4.1.3rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-spark-4.1.2rc1/PKG-INFO` & `apache-airflow-providers-apache-spark-4.1.3rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-apache-spark
-Version: 4.1.2rc1
+Version: 4.1.3rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-apache-spark package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-spark/4.1.2/
-Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-apache-spark/4.1.2/changelog.html
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-spark/4.1.3/
+Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-apache-spark/4.1.3/changelog.html
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -67,28 +67,28 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-apache-spark``
 
-Release: ``4.1.2rc1``
+Release: ``4.1.3rc1``
 
 
 `Apache Spark <https://spark.apache.org/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``apache.spark`` provider. All classes for this provider package
 are in ``airflow.providers.apache.spark`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apache-spark/4.1.2/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apache-spark/4.1.3/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -122,8 +122,8 @@
 ======================================================================================================================  ===================
 Dependent package                                                                                                       Extra
 ======================================================================================================================  ===================
 `apache-airflow-providers-cncf-kubernetes <https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes>`_  ``cncf.kubernetes``
 ======================================================================================================================  ===================
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-apache-spark/4.1.2/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-apache-spark/4.1.3/changelog.html>`_.
```

### Comparing `apache-airflow-providers-apache-spark-4.1.2rc1/README.rst` & `apache-airflow-providers-apache-spark-4.1.3rc1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -32,28 +32,28 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-apache-spark``
 
-Release: ``4.1.2rc1``
+Release: ``4.1.3rc1``
 
 
 `Apache Spark <https://spark.apache.org/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``apache.spark`` provider. All classes for this provider package
 are in ``airflow.providers.apache.spark`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apache-spark/4.1.2/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apache-spark/4.1.3/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -87,8 +87,8 @@
 ======================================================================================================================  ===================
 Dependent package                                                                                                       Extra
 ======================================================================================================================  ===================
 `apache-airflow-providers-cncf-kubernetes <https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes>`_  ``cncf.kubernetes``
 ======================================================================================================================  ===================
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-apache-spark/4.1.2/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-apache-spark/4.1.3/changelog.html>`_.
```

### Comparing `apache-airflow-providers-apache-spark-4.1.2rc1/airflow/providers/apache/spark/__init__.py` & `apache-airflow-providers-apache-spark-4.1.3rc1/airflow/providers/apache/spark/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 from __future__ import annotations
 
 import packaging.version
 
 __all__ = ["__version__"]
 
-__version__ = "4.1.2"
+__version__ = "4.1.3"
 
 try:
     from airflow import __version__ as airflow_version
 except ImportError:
     from airflow.version import version as airflow_version
 
 if packaging.version.parse(packaging.version.parse(airflow_version).base_version) < packaging.version.parse(
```

### Comparing `apache-airflow-providers-apache-spark-4.1.2rc1/airflow/providers/apache/spark/get_provider_info.py` & `apache-airflow-providers-apache-spark-4.1.3rc1/airflow/providers/apache/spark/get_provider_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-apache-spark",
         "name": "Apache Spark",
         "description": "`Apache Spark <https://spark.apache.org/>`__\n",
         "suspended": False,
         "versions": [
+            "4.1.3",
             "4.1.2",
             "4.1.1",
             "4.1.0",
             "4.0.1",
             "4.0.0",
             "3.0.0",
             "2.1.3",
```

### Comparing `apache-airflow-providers-apache-spark-4.1.2rc1/airflow/providers/apache/spark/hooks/__init__.py` & `apache-airflow-providers-apache-spark-4.1.3rc1/airflow/providers/apache/spark/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-spark-4.1.2rc1/airflow/providers/apache/spark/hooks/spark_jdbc.py` & `apache-airflow-providers-apache-spark-4.1.3rc1/airflow/providers/apache/spark/hooks/spark_jdbc.py`

 * *Files 1% similar despite different names*

```diff
@@ -177,14 +177,16 @@
             )
         return conn_data
 
     def _build_jdbc_application_arguments(self, jdbc_conn: dict[str, Any]) -> Any:
         arguments = []
         arguments += ["-cmdType", self._cmd_type]
         if self._jdbc_connection["url"]:
+            if "?" in jdbc_conn["conn_prefix"]:
+                raise ValueError("The jdbc extra conn_prefix should not contain a '?'")
             arguments += [
                 "-url",
                 f"{jdbc_conn['conn_prefix']}{jdbc_conn['url']}/{jdbc_conn['schema']}",
             ]
         if self._jdbc_connection["user"]:
             arguments += ["-user", self._jdbc_connection["user"]]
         if self._jdbc_connection["password"]:
```

### Comparing `apache-airflow-providers-apache-spark-4.1.2rc1/airflow/providers/apache/spark/hooks/spark_jdbc_script.py` & `apache-airflow-providers-apache-spark-4.1.3rc1/airflow/providers/apache/spark/hooks/spark_jdbc_script.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-spark-4.1.2rc1/airflow/providers/apache/spark/hooks/spark_sql.py` & `apache-airflow-providers-apache-spark-4.1.3rc1/airflow/providers/apache/spark/hooks/spark_sql.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-spark-4.1.2rc1/airflow/providers/apache/spark/hooks/spark_submit.py` & `apache-airflow-providers-apache-spark-4.1.3rc1/airflow/providers/apache/spark/hooks/spark_submit.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-spark-4.1.2rc1/airflow/providers/apache/spark/operators/__init__.py` & `apache-airflow-providers-apache-spark-4.1.3rc1/airflow/providers/apache/spark/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-spark-4.1.2rc1/airflow/providers/apache/spark/operators/spark_jdbc.py` & `apache-airflow-providers-apache-spark-4.1.3rc1/airflow/providers/apache/spark/operators/spark_jdbc.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-spark-4.1.2rc1/airflow/providers/apache/spark/operators/spark_sql.py` & `apache-airflow-providers-apache-spark-4.1.3rc1/airflow/providers/apache/spark/operators/spark_sql.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-spark-4.1.2rc1/airflow/providers/apache/spark/operators/spark_submit.py` & `apache-airflow-providers-apache-spark-4.1.3rc1/airflow/providers/apache/spark/operators/spark_submit.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-spark-4.1.2rc1/apache_airflow_providers_apache_spark.egg-info/PKG-INFO` & `apache-airflow-providers-apache-spark-4.1.3rc1/apache_airflow_providers_apache_spark.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-apache-spark
-Version: 4.1.2rc1
+Version: 4.1.3rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-apache-spark package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-spark/4.1.2/
-Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-apache-spark/4.1.2/changelog.html
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-spark/4.1.3/
+Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-apache-spark/4.1.3/changelog.html
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -67,28 +67,28 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-apache-spark``
 
-Release: ``4.1.2rc1``
+Release: ``4.1.3rc1``
 
 
 `Apache Spark <https://spark.apache.org/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``apache.spark`` provider. All classes for this provider package
 are in ``airflow.providers.apache.spark`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apache-spark/4.1.2/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apache-spark/4.1.3/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -122,8 +122,8 @@
 ======================================================================================================================  ===================
 Dependent package                                                                                                       Extra
 ======================================================================================================================  ===================
 `apache-airflow-providers-cncf-kubernetes <https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes>`_  ``cncf.kubernetes``
 ======================================================================================================================  ===================
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-apache-spark/4.1.2/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-apache-spark/4.1.3/changelog.html>`_.
```

### Comparing `apache-airflow-providers-apache-spark-4.1.2rc1/apache_airflow_providers_apache_spark.egg-info/SOURCES.txt` & `apache-airflow-providers-apache-spark-4.1.3rc1/apache_airflow_providers_apache_spark.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-spark-4.1.2rc1/pyproject.toml` & `apache-airflow-providers-apache-spark-4.1.3rc1/pyproject.toml`

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

### Comparing `apache-airflow-providers-apache-spark-4.1.2rc1/setup.cfg` & `apache-airflow-providers-apache-spark-4.1.3rc1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -23,16 +23,16 @@
 	License :: OSI Approved :: Apache Software License
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	Topic :: System :: Monitoring
 project_urls = 
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-apache-spark/4.1.2/
-	Changelog=https://airflow.apache.org/docs/apache-airflow-providers-apache-spark/4.1.2/changelog.html
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-apache-spark/4.1.3/
+	Changelog=https://airflow.apache.org/docs/apache-airflow-providers-apache-spark/4.1.3/changelog.html
 	Bug Tracker=https://github.com/apache/airflow/issues
 	Source Code=https://github.com/apache/airflow
 	Slack Chat=https://s.apache.org/airflow-slack
 	Twitter=https://twitter.com/ApacheAirflow
 	YouTube=https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 
 [bdist_wheel]
```

### Comparing `apache-airflow-providers-apache-spark-4.1.2rc1/setup.py` & `apache-airflow-providers-apache-spark-4.1.3rc1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-apache-spark package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "4.1.2"
+version = "4.1.3"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-apache-spark setup."""
     setup(
         version=version,
         extras_require={"cncf.kubernetes": ["apache-airflow-providers-cncf-kubernetes>=7.4.0"]},
```

