# Comparing `tmp/apache-airflow-providers-snowflake-4.4.0rc1.tar.gz` & `tmp/apache-airflow-providers-snowflake-4.4.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-snowflake-4.4.0rc1.tar", last modified: Sat Jul 29 12:09:08 2023, max compression
+gzip compressed data, was "apache-airflow-providers-snowflake-4.4.1rc1.tar", last modified: Fri Aug  4 21:41:41 2023, max compression
```

## Comparing `apache-airflow-providers-snowflake-4.4.0rc1.tar` & `apache-airflow-providers-snowflake-4.4.1rc1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:09:08.761202 apache-airflow-providers-snowflake-4.4.0rc1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-snowflake-4.4.0rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-07-29 12:09:07.000000 apache-airflow-providers-snowflake-4.4.0rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-snowflake-4.4.0rc1/NOTICE
--rw-r--r--   0 root         (0) root         (0)     6044 2023-07-29 12:09:08.761764 apache-airflow-providers-snowflake-4.4.0rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4317 2023-07-29 12:09:07.000000 apache-airflow-providers-snowflake-4.4.0rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:09:08.655883 apache-airflow-providers-snowflake-4.4.0rc1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:09:08.657068 apache-airflow-providers-snowflake-4.4.0rc1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:09:08.694162 apache-airflow-providers-snowflake-4.4.0rc1/airflow/providers/snowflake/
--rw-r--r--   0 root         (0) root         (0)     1578 2023-07-29 12:01:19.000000 apache-airflow-providers-snowflake-4.4.0rc1/airflow/providers/snowflake/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4991 2023-07-29 12:09:07.000000 apache-airflow-providers-snowflake-4.4.0rc1/airflow/providers/snowflake/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:09:08.703082 apache-airflow-providers-snowflake-4.4.0rc1/airflow/providers/snowflake/hooks/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:29.000000 apache-airflow-providers-snowflake-4.4.0rc1/airflow/providers/snowflake/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21801 2023-07-26 06:59:50.000000 apache-airflow-providers-snowflake-4.4.0rc1/airflow/providers/snowflake/hooks/snowflake.py
--rw-r--r--   0 root         (0) root         (0)    12677 2023-07-09 14:40:47.000000 apache-airflow-providers-snowflake-4.4.0rc1/airflow/providers/snowflake/hooks/snowflake_sql_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:09:08.708868 apache-airflow-providers-snowflake-4.4.0rc1/airflow/providers/snowflake/operators/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:29.000000 apache-airflow-providers-snowflake-4.4.0rc1/airflow/providers/snowflake/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)    24878 2023-07-26 06:59:50.000000 apache-airflow-providers-snowflake-4.4.0rc1/airflow/providers/snowflake/operators/snowflake.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:09:08.720597 apache-airflow-providers-snowflake-4.4.0rc1/airflow/providers/snowflake/transfers/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:29.000000 apache-airflow-providers-snowflake-4.4.0rc1/airflow/providers/snowflake/transfers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5765 2023-07-09 14:40:47.000000 apache-airflow-providers-snowflake-4.4.0rc1/airflow/providers/snowflake/transfers/copy_into_snowflake.py
--rw-r--r--   0 root         (0) root         (0)     6054 2023-06-02 11:31:21.000000 apache-airflow-providers-snowflake-4.4.0rc1/airflow/providers/snowflake/transfers/s3_to_snowflake.py
--rw-r--r--   0 root         (0) root         (0)     5098 2023-07-26 06:59:50.000000 apache-airflow-providers-snowflake-4.4.0rc1/airflow/providers/snowflake/transfers/snowflake_to_slack.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:09:08.726145 apache-airflow-providers-snowflake-4.4.0rc1/airflow/providers/snowflake/triggers/
--rw-r--r--   0 root         (0) root         (0)      785 2023-07-05 07:19:39.000000 apache-airflow-providers-snowflake-4.4.0rc1/airflow/providers/snowflake/triggers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4186 2023-07-09 14:40:47.000000 apache-airflow-providers-snowflake-4.4.0rc1/airflow/providers/snowflake/triggers/snowflake_trigger.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:09:08.734576 apache-airflow-providers-snowflake-4.4.0rc1/airflow/providers/snowflake/utils/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:29.000000 apache-airflow-providers-snowflake-4.4.0rc1/airflow/providers/snowflake/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1644 2023-06-01 06:14:29.000000 apache-airflow-providers-snowflake-4.4.0rc1/airflow/providers/snowflake/utils/common.py
--rw-r--r--   0 root         (0) root         (0)     6889 2023-07-09 14:40:47.000000 apache-airflow-providers-snowflake-4.4.0rc1/airflow/providers/snowflake/utils/sql_api_generate_jwt.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:09:08.758540 apache-airflow-providers-snowflake-4.4.0rc1/apache_airflow_providers_snowflake.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6044 2023-07-29 12:09:08.000000 apache-airflow-providers-snowflake-4.4.0rc1/apache_airflow_providers_snowflake.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1299 2023-07-29 12:09:08.000000 apache-airflow-providers-snowflake-4.4.0rc1/apache_airflow_providers_snowflake.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:09:08.000000 apache-airflow-providers-snowflake-4.4.0rc1/apache_airflow_providers_snowflake.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      106 2023-07-29 12:09:08.000000 apache-airflow-providers-snowflake-4.4.0rc1/apache_airflow_providers_snowflake.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:09:08.000000 apache-airflow-providers-snowflake-4.4.0rc1/apache_airflow_providers_snowflake.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      279 2023-07-29 12:09:08.000000 apache-airflow-providers-snowflake-4.4.0rc1/apache_airflow_providers_snowflake.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-07-29 12:09:08.000000 apache-airflow-providers-snowflake-4.4.0rc1/apache_airflow_providers_snowflake.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5011 2023-07-27 05:54:58.000000 apache-airflow-providers-snowflake-4.4.0rc1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     2059 2023-07-29 12:09:08.763589 apache-airflow-providers-snowflake-4.4.0rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1858 2023-07-29 12:09:07.000000 apache-airflow-providers-snowflake-4.4.0rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:41:41.746368 apache-airflow-providers-snowflake-4.4.1rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-snowflake-4.4.1rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-08-04 21:41:40.000000 apache-airflow-providers-snowflake-4.4.1rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-snowflake-4.4.1rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     6044 2023-08-04 21:41:41.746964 apache-airflow-providers-snowflake-4.4.1rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4317 2023-08-04 21:41:40.000000 apache-airflow-providers-snowflake-4.4.1rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:41:41.641469 apache-airflow-providers-snowflake-4.4.1rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:41:41.642672 apache-airflow-providers-snowflake-4.4.1rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:41:41.678819 apache-airflow-providers-snowflake-4.4.1rc1/airflow/providers/snowflake/
+-rw-r--r--   0 root         (0) root         (0)     1578 2023-08-04 21:33:34.000000 apache-airflow-providers-snowflake-4.4.1rc1/airflow/providers/snowflake/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5012 2023-08-04 21:41:40.000000 apache-airflow-providers-snowflake-4.4.1rc1/airflow/providers/snowflake/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:41:41.687801 apache-airflow-providers-snowflake-4.4.1rc1/airflow/providers/snowflake/hooks/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:29.000000 apache-airflow-providers-snowflake-4.4.1rc1/airflow/providers/snowflake/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21801 2023-07-26 06:59:50.000000 apache-airflow-providers-snowflake-4.4.1rc1/airflow/providers/snowflake/hooks/snowflake.py
+-rw-r--r--   0 root         (0) root         (0)    12677 2023-07-09 14:40:47.000000 apache-airflow-providers-snowflake-4.4.1rc1/airflow/providers/snowflake/hooks/snowflake_sql_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:41:41.693593 apache-airflow-providers-snowflake-4.4.1rc1/airflow/providers/snowflake/operators/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:29.000000 apache-airflow-providers-snowflake-4.4.1rc1/airflow/providers/snowflake/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25105 2023-08-04 10:24:22.000000 apache-airflow-providers-snowflake-4.4.1rc1/airflow/providers/snowflake/operators/snowflake.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:41:41.705462 apache-airflow-providers-snowflake-4.4.1rc1/airflow/providers/snowflake/transfers/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:29.000000 apache-airflow-providers-snowflake-4.4.1rc1/airflow/providers/snowflake/transfers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5765 2023-07-09 14:40:47.000000 apache-airflow-providers-snowflake-4.4.1rc1/airflow/providers/snowflake/transfers/copy_into_snowflake.py
+-rw-r--r--   0 root         (0) root         (0)     6054 2023-06-02 11:31:21.000000 apache-airflow-providers-snowflake-4.4.1rc1/airflow/providers/snowflake/transfers/s3_to_snowflake.py
+-rw-r--r--   0 root         (0) root         (0)     5098 2023-07-26 06:59:50.000000 apache-airflow-providers-snowflake-4.4.1rc1/airflow/providers/snowflake/transfers/snowflake_to_slack.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:41:41.711216 apache-airflow-providers-snowflake-4.4.1rc1/airflow/providers/snowflake/triggers/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-07-05 07:19:39.000000 apache-airflow-providers-snowflake-4.4.1rc1/airflow/providers/snowflake/triggers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4186 2023-07-09 14:40:47.000000 apache-airflow-providers-snowflake-4.4.1rc1/airflow/providers/snowflake/triggers/snowflake_trigger.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:41:41.719766 apache-airflow-providers-snowflake-4.4.1rc1/airflow/providers/snowflake/utils/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:29.000000 apache-airflow-providers-snowflake-4.4.1rc1/airflow/providers/snowflake/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1644 2023-06-01 06:14:29.000000 apache-airflow-providers-snowflake-4.4.1rc1/airflow/providers/snowflake/utils/common.py
+-rw-r--r--   0 root         (0) root         (0)     6889 2023-07-09 14:40:47.000000 apache-airflow-providers-snowflake-4.4.1rc1/airflow/providers/snowflake/utils/sql_api_generate_jwt.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:41:41.744024 apache-airflow-providers-snowflake-4.4.1rc1/apache_airflow_providers_snowflake.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6044 2023-08-04 21:41:41.000000 apache-airflow-providers-snowflake-4.4.1rc1/apache_airflow_providers_snowflake.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1299 2023-08-04 21:41:41.000000 apache-airflow-providers-snowflake-4.4.1rc1/apache_airflow_providers_snowflake.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 21:41:41.000000 apache-airflow-providers-snowflake-4.4.1rc1/apache_airflow_providers_snowflake.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      106 2023-08-04 21:41:41.000000 apache-airflow-providers-snowflake-4.4.1rc1/apache_airflow_providers_snowflake.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 21:41:41.000000 apache-airflow-providers-snowflake-4.4.1rc1/apache_airflow_providers_snowflake.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      279 2023-08-04 21:41:41.000000 apache-airflow-providers-snowflake-4.4.1rc1/apache_airflow_providers_snowflake.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-08-04 21:41:41.000000 apache-airflow-providers-snowflake-4.4.1rc1/apache_airflow_providers_snowflake.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5031 2023-08-04 10:24:23.000000 apache-airflow-providers-snowflake-4.4.1rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     2059 2023-08-04 21:41:41.748769 apache-airflow-providers-snowflake-4.4.1rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1858 2023-08-04 21:41:40.000000 apache-airflow-providers-snowflake-4.4.1rc1/setup.py
```

### Comparing `apache-airflow-providers-snowflake-4.4.0rc1/LICENSE` & `apache-airflow-providers-snowflake-4.4.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.4.0rc1/MANIFEST.in` & `apache-airflow-providers-snowflake-4.4.1rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.4.0rc1/PKG-INFO` & `apache-airflow-providers-snowflake-4.4.1rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-snowflake
-Version: 4.4.0rc1
+Version: 4.4.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-snowflake package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-snowflake/4.4.0/
-Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-snowflake/4.4.0/changelog.html
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-snowflake/4.4.1/
+Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-snowflake/4.4.1/changelog.html
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -69,28 +69,28 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-snowflake``
 
-Release: ``4.4.0rc1``
+Release: ``4.4.1rc1``
 
 
 `Snowflake <https://www.snowflake.com/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``snowflake`` provider. All classes for this provider package
 are in ``airflow.providers.snowflake`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-snowflake/4.4.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-snowflake/4.4.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -128,8 +128,8 @@
 ==============================================================================================================  ===============
 `apache-airflow-providers-common-sql <https://airflow.apache.org/docs/apache-airflow-providers-common-sql>`_    ``common.sql``
 `apache-airflow-providers-openlineage <https://airflow.apache.org/docs/apache-airflow-providers-openlineage>`_  ``openlineage``
 `apache-airflow-providers-slack <https://airflow.apache.org/docs/apache-airflow-providers-slack>`_              ``slack``
 ==============================================================================================================  ===============
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-snowflake/4.4.0/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-snowflake/4.4.1/changelog.html>`_.
```

### Comparing `apache-airflow-providers-snowflake-4.4.0rc1/README.rst` & `apache-airflow-providers-snowflake-4.4.1rc1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -32,28 +32,28 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-snowflake``
 
-Release: ``4.4.0rc1``
+Release: ``4.4.1rc1``
 
 
 `Snowflake <https://www.snowflake.com/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``snowflake`` provider. All classes for this provider package
 are in ``airflow.providers.snowflake`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-snowflake/4.4.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-snowflake/4.4.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -91,8 +91,8 @@
 ==============================================================================================================  ===============
 `apache-airflow-providers-common-sql <https://airflow.apache.org/docs/apache-airflow-providers-common-sql>`_    ``common.sql``
 `apache-airflow-providers-openlineage <https://airflow.apache.org/docs/apache-airflow-providers-openlineage>`_  ``openlineage``
 `apache-airflow-providers-slack <https://airflow.apache.org/docs/apache-airflow-providers-slack>`_              ``slack``
 ==============================================================================================================  ===============
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-snowflake/4.4.0/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-snowflake/4.4.1/changelog.html>`_.
```

### Comparing `apache-airflow-providers-snowflake-4.4.0rc1/airflow/providers/snowflake/__init__.py` & `apache-airflow-providers-snowflake-4.4.1rc1/airflow/providers/snowflake/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 from __future__ import annotations
 
 import packaging.version
 
 __all__ = ["__version__"]
 
-__version__ = "4.4.0"
+__version__ = "4.4.1"
 
 try:
     from airflow import __version__ as airflow_version
 except ImportError:
     from airflow.version import version as airflow_version
 
 if packaging.version.parse(packaging.version.parse(airflow_version).base_version) < packaging.version.parse(
```

### Comparing `apache-airflow-providers-snowflake-4.4.0rc1/airflow/providers/snowflake/get_provider_info.py` & `apache-airflow-providers-snowflake-4.4.1rc1/airflow/providers/snowflake/get_provider_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-snowflake",
         "name": "Snowflake",
         "description": "`Snowflake <https://www.snowflake.com/>`__\n",
         "suspended": False,
         "versions": [
+            "4.4.1",
             "4.4.0",
             "4.3.1",
             "4.3.0",
             "4.2.0",
             "4.1.0",
             "4.0.5",
             "4.0.4",
```

### Comparing `apache-airflow-providers-snowflake-4.4.0rc1/airflow/providers/snowflake/hooks/__init__.py` & `apache-airflow-providers-snowflake-4.4.1rc1/airflow/providers/snowflake/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.4.0rc1/airflow/providers/snowflake/hooks/snowflake.py` & `apache-airflow-providers-snowflake-4.4.1rc1/airflow/providers/snowflake/hooks/snowflake.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.4.0rc1/airflow/providers/snowflake/hooks/snowflake_sql_api.py` & `apache-airflow-providers-snowflake-4.4.1rc1/airflow/providers/snowflake/hooks/snowflake_sql_api.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.4.0rc1/airflow/providers/snowflake/operators/__init__.py` & `apache-airflow-providers-snowflake-4.4.1rc1/airflow/providers/snowflake/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.4.0rc1/airflow/providers/snowflake/operators/snowflake.py` & `apache-airflow-providers-snowflake-4.4.1rc1/airflow/providers/snowflake/operators/snowflake.py`

 * *Files 9% similar despite different names*

```diff
@@ -208,26 +208,26 @@
         database: str | None = None,
         role: str | None = None,
         schema: str | None = None,
         authenticator: str | None = None,
         session_parameters: dict | None = None,
         **kwargs,
     ) -> None:
+        if any([warehouse, database, role, schema, authenticator, session_parameters]):
+            hook_params = kwargs.pop("hook_params", {})
+            kwargs["hook_params"] = {
+                "warehouse": warehouse,
+                "database": database,
+                "role": role,
+                "schema": schema,
+                "authenticator": authenticator,
+                "session_parameters": session_parameters,
+                **hook_params,
+            }
         super().__init__(sql=sql, parameters=parameters, conn_id=snowflake_conn_id, **kwargs)
-        self.snowflake_conn_id = snowflake_conn_id
-        self.sql = sql
-        self.autocommit = autocommit
-        self.do_xcom_push = do_xcom_push
-        self.parameters = parameters
-        self.warehouse = warehouse
-        self.database = database
-        self.role = role
-        self.schema = schema
-        self.authenticator = authenticator
-        self.session_parameters = session_parameters
         self.query_ids: list[str] = []
 
 
 class SnowflakeValueCheckOperator(SQLValueCheckOperator):
     """
     Performs a simple check using sql code against a specified value, within a certain level of tolerance.
 
@@ -273,28 +273,28 @@
         database: str | None = None,
         role: str | None = None,
         schema: str | None = None,
         authenticator: str | None = None,
         session_parameters: dict | None = None,
         **kwargs,
     ) -> None:
+        if any([warehouse, database, role, schema, authenticator, session_parameters]):
+            hook_params = kwargs.pop("hook_params", {})
+            kwargs["hook_params"] = {
+                "warehouse": warehouse,
+                "database": database,
+                "role": role,
+                "schema": schema,
+                "authenticator": authenticator,
+                "session_parameters": session_parameters,
+                **hook_params,
+            }
         super().__init__(
             sql=sql, pass_value=pass_value, tolerance=tolerance, conn_id=snowflake_conn_id, **kwargs
         )
-        self.snowflake_conn_id = snowflake_conn_id
-        self.sql = sql
-        self.autocommit = autocommit
-        self.do_xcom_push = do_xcom_push
-        self.parameters = parameters
-        self.warehouse = warehouse
-        self.database = database
-        self.role = role
-        self.schema = schema
-        self.authenticator = authenticator
-        self.session_parameters = session_parameters
         self.query_ids: list[str] = []
 
 
 class SnowflakeIntervalCheckOperator(SQLIntervalCheckOperator):
     """
     Checks that the metrics given as SQL expressions are within tolerance of the ones from days_back before.
 
@@ -348,32 +348,33 @@
         database: str | None = None,
         role: str | None = None,
         schema: str | None = None,
         authenticator: str | None = None,
         session_parameters: dict | None = None,
         **kwargs,
     ) -> None:
+        if any([warehouse, database, role, schema, authenticator, session_parameters]):
+            hook_params = kwargs.pop("hook_params", {})
+            kwargs["hook_params"] = {
+                "warehouse": warehouse,
+                "database": database,
+                "role": role,
+                "schema": schema,
+                "authenticator": authenticator,
+                "session_parameters": session_parameters,
+                **hook_params,
+            }
         super().__init__(
             table=table,
             metrics_thresholds=metrics_thresholds,
             date_filter_column=date_filter_column,
             days_back=days_back,
             conn_id=snowflake_conn_id,
             **kwargs,
         )
-        self.snowflake_conn_id = snowflake_conn_id
-        self.autocommit = autocommit
-        self.do_xcom_push = do_xcom_push
-        self.parameters = parameters
-        self.warehouse = warehouse
-        self.database = database
-        self.role = role
-        self.schema = schema
-        self.authenticator = authenticator
-        self.session_parameters = session_parameters
         self.query_ids: list[str] = []
 
 
 class SnowflakeSqlApiOperator(SQLExecuteQueryOperator):
     """
     Implemented Snowflake SQL API Operator to support multiple SQL statements sequentially,
     which is the behavior of the SnowflakeOperator, the Snowflake SQL API allows submitting
```

### Comparing `apache-airflow-providers-snowflake-4.4.0rc1/airflow/providers/snowflake/transfers/__init__.py` & `apache-airflow-providers-snowflake-4.4.1rc1/airflow/providers/snowflake/transfers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.4.0rc1/airflow/providers/snowflake/transfers/copy_into_snowflake.py` & `apache-airflow-providers-snowflake-4.4.1rc1/airflow/providers/snowflake/transfers/copy_into_snowflake.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.4.0rc1/airflow/providers/snowflake/transfers/s3_to_snowflake.py` & `apache-airflow-providers-snowflake-4.4.1rc1/airflow/providers/snowflake/transfers/s3_to_snowflake.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.4.0rc1/airflow/providers/snowflake/transfers/snowflake_to_slack.py` & `apache-airflow-providers-snowflake-4.4.1rc1/airflow/providers/snowflake/transfers/snowflake_to_slack.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.4.0rc1/airflow/providers/snowflake/triggers/__init__.py` & `apache-airflow-providers-snowflake-4.4.1rc1/airflow/providers/snowflake/triggers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.4.0rc1/airflow/providers/snowflake/triggers/snowflake_trigger.py` & `apache-airflow-providers-snowflake-4.4.1rc1/airflow/providers/snowflake/triggers/snowflake_trigger.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.4.0rc1/airflow/providers/snowflake/utils/__init__.py` & `apache-airflow-providers-snowflake-4.4.1rc1/airflow/providers/snowflake/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.4.0rc1/airflow/providers/snowflake/utils/common.py` & `apache-airflow-providers-snowflake-4.4.1rc1/airflow/providers/snowflake/utils/common.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.4.0rc1/airflow/providers/snowflake/utils/sql_api_generate_jwt.py` & `apache-airflow-providers-snowflake-4.4.1rc1/airflow/providers/snowflake/utils/sql_api_generate_jwt.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.4.0rc1/apache_airflow_providers_snowflake.egg-info/PKG-INFO` & `apache-airflow-providers-snowflake-4.4.1rc1/apache_airflow_providers_snowflake.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-snowflake
-Version: 4.4.0rc1
+Version: 4.4.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-snowflake package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-snowflake/4.4.0/
-Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-snowflake/4.4.0/changelog.html
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-snowflake/4.4.1/
+Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-snowflake/4.4.1/changelog.html
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -69,28 +69,28 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-snowflake``
 
-Release: ``4.4.0rc1``
+Release: ``4.4.1rc1``
 
 
 `Snowflake <https://www.snowflake.com/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``snowflake`` provider. All classes for this provider package
 are in ``airflow.providers.snowflake`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-snowflake/4.4.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-snowflake/4.4.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -128,8 +128,8 @@
 ==============================================================================================================  ===============
 `apache-airflow-providers-common-sql <https://airflow.apache.org/docs/apache-airflow-providers-common-sql>`_    ``common.sql``
 `apache-airflow-providers-openlineage <https://airflow.apache.org/docs/apache-airflow-providers-openlineage>`_  ``openlineage``
 `apache-airflow-providers-slack <https://airflow.apache.org/docs/apache-airflow-providers-slack>`_              ``slack``
 ==============================================================================================================  ===============
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-snowflake/4.4.0/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-snowflake/4.4.1/changelog.html>`_.
```

### Comparing `apache-airflow-providers-snowflake-4.4.0rc1/apache_airflow_providers_snowflake.egg-info/SOURCES.txt` & `apache-airflow-providers-snowflake-4.4.1rc1/apache_airflow_providers_snowflake.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.4.0rc1/pyproject.toml` & `apache-airflow-providers-snowflake-4.4.1rc1/pyproject.toml`

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

### Comparing `apache-airflow-providers-snowflake-4.4.0rc1/setup.cfg` & `apache-airflow-providers-snowflake-4.4.1rc1/setup.cfg`

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
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-snowflake/4.4.0/
-	Changelog=https://airflow.apache.org/docs/apache-airflow-providers-snowflake/4.4.0/changelog.html
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-snowflake/4.4.1/
+	Changelog=https://airflow.apache.org/docs/apache-airflow-providers-snowflake/4.4.1/changelog.html
 	Bug Tracker=https://github.com/apache/airflow/issues
 	Source Code=https://github.com/apache/airflow
 	Slack Chat=https://s.apache.org/airflow-slack
 	Twitter=https://twitter.com/ApacheAirflow
 	YouTube=https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 
 [bdist_wheel]
```

### Comparing `apache-airflow-providers-snowflake-4.4.0rc1/setup.py` & `apache-airflow-providers-snowflake-4.4.1rc1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-snowflake package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "4.4.0"
+version = "4.4.1"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-snowflake setup."""
     setup(
         version=version,
         extras_require={
```

