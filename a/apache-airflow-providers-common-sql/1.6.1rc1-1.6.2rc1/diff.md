# Comparing `tmp/apache-airflow-providers-common-sql-1.6.1rc1.tar.gz` & `tmp/apache-airflow-providers-common-sql-1.6.2rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-common-sql-1.6.1rc1.tar", last modified: Sat Jul 29 12:08:15 2023, max compression
+gzip compressed data, was "apache-airflow-providers-common-sql-1.6.2rc1.tar", last modified: Fri Aug  4 21:40:58 2023, max compression
```

## Comparing `apache-airflow-providers-common-sql-1.6.1rc1.tar` & `apache-airflow-providers-common-sql-1.6.2rc1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:15.344153 apache-airflow-providers-common-sql-1.6.1rc1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-common-sql-1.6.1rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-07-29 12:08:14.000000 apache-airflow-providers-common-sql-1.6.1rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-common-sql-1.6.1rc1/NOTICE
--rw-r--r--   0 root         (0) root         (0)     5566 2023-07-29 12:08:15.344852 apache-airflow-providers-common-sql-1.6.1rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3861 2023-07-29 12:08:14.000000 apache-airflow-providers-common-sql-1.6.1rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:15.254916 apache-airflow-providers-common-sql-1.6.1rc1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:15.256070 apache-airflow-providers-common-sql-1.6.1rc1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:15.257141 apache-airflow-providers-common-sql-1.6.1rc1/airflow/providers/common/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:15.292983 apache-airflow-providers-common-sql-1.6.1rc1/airflow/providers/common/sql/
--rw-r--r--   0 root         (0) root         (0)     1579 2023-07-29 12:01:19.000000 apache-airflow-providers-common-sql-1.6.1rc1/airflow/providers/common/sql/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2620 2023-07-29 12:08:14.000000 apache-airflow-providers-common-sql-1.6.1rc1/airflow/providers/common/sql/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:15.299054 apache-airflow-providers-common-sql-1.6.1rc1/airflow/providers/common/sql/hooks/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-common-sql-1.6.1rc1/airflow/providers/common/sql/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    24869 2023-07-26 06:59:50.000000 apache-airflow-providers-common-sql-1.6.1rc1/airflow/providers/common/sql/hooks/sql.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:15.306104 apache-airflow-providers-common-sql-1.6.1rc1/airflow/providers/common/sql/operators/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-common-sql-1.6.1rc1/airflow/providers/common/sql/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)    46908 2023-07-26 06:59:50.000000 apache-airflow-providers-common-sql-1.6.1rc1/airflow/providers/common/sql/operators/sql.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:15.312673 apache-airflow-providers-common-sql-1.6.1rc1/airflow/providers/common/sql/sensors/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-common-sql-1.6.1rc1/airflow/providers/common/sql/sensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4726 2023-06-05 12:50:36.000000 apache-airflow-providers-common-sql-1.6.1rc1/airflow/providers/common/sql/sensors/sql.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:15.341060 apache-airflow-providers-common-sql-1.6.1rc1/apache_airflow_providers_common_sql.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5566 2023-07-29 12:08:15.000000 apache-airflow-providers-common-sql-1.6.1rc1/apache_airflow_providers_common_sql.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      855 2023-07-29 12:08:15.000000 apache-airflow-providers-common-sql-1.6.1rc1/apache_airflow_providers_common_sql.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:08:15.000000 apache-airflow-providers-common-sql-1.6.1rc1/apache_airflow_providers_common_sql.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      107 2023-07-29 12:08:15.000000 apache-airflow-providers-common-sql-1.6.1rc1/apache_airflow_providers_common_sql.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:08:15.000000 apache-airflow-providers-common-sql-1.6.1rc1/apache_airflow_providers_common_sql.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      120 2023-07-29 12:08:15.000000 apache-airflow-providers-common-sql-1.6.1rc1/apache_airflow_providers_common_sql.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-07-29 12:08:15.000000 apache-airflow-providers-common-sql-1.6.1rc1/apache_airflow_providers_common_sql.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5011 2023-07-27 05:54:58.000000 apache-airflow-providers-common-sql-1.6.1rc1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1970 2023-07-29 12:08:15.347635 apache-airflow-providers-common-sql-1.6.1rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1782 2023-07-29 12:08:14.000000 apache-airflow-providers-common-sql-1.6.1rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:40:58.024927 apache-airflow-providers-common-sql-1.6.2rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-common-sql-1.6.2rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-08-04 21:40:56.000000 apache-airflow-providers-common-sql-1.6.2rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-common-sql-1.6.2rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     5566 2023-08-04 21:40:58.025505 apache-airflow-providers-common-sql-1.6.2rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3861 2023-08-04 21:40:56.000000 apache-airflow-providers-common-sql-1.6.2rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:40:57.943530 apache-airflow-providers-common-sql-1.6.2rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:40:57.944697 apache-airflow-providers-common-sql-1.6.2rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:40:57.945738 apache-airflow-providers-common-sql-1.6.2rc1/airflow/providers/common/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:40:57.978421 apache-airflow-providers-common-sql-1.6.2rc1/airflow/providers/common/sql/
+-rw-r--r--   0 root         (0) root         (0)     1579 2023-08-04 21:33:34.000000 apache-airflow-providers-common-sql-1.6.2rc1/airflow/providers/common/sql/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2641 2023-08-04 21:40:56.000000 apache-airflow-providers-common-sql-1.6.2rc1/airflow/providers/common/sql/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:40:57.984055 apache-airflow-providers-common-sql-1.6.2rc1/airflow/providers/common/sql/hooks/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-common-sql-1.6.2rc1/airflow/providers/common/sql/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24869 2023-07-26 06:59:50.000000 apache-airflow-providers-common-sql-1.6.2rc1/airflow/providers/common/sql/hooks/sql.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:40:57.989944 apache-airflow-providers-common-sql-1.6.2rc1/airflow/providers/common/sql/operators/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-common-sql-1.6.2rc1/airflow/providers/common/sql/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    47157 2023-08-04 19:44:14.000000 apache-airflow-providers-common-sql-1.6.2rc1/airflow/providers/common/sql/operators/sql.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:40:57.996311 apache-airflow-providers-common-sql-1.6.2rc1/airflow/providers/common/sql/sensors/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-common-sql-1.6.2rc1/airflow/providers/common/sql/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4726 2023-06-05 12:50:36.000000 apache-airflow-providers-common-sql-1.6.2rc1/airflow/providers/common/sql/sensors/sql.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:40:58.022182 apache-airflow-providers-common-sql-1.6.2rc1/apache_airflow_providers_common_sql.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5566 2023-08-04 21:40:57.000000 apache-airflow-providers-common-sql-1.6.2rc1/apache_airflow_providers_common_sql.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      855 2023-08-04 21:40:57.000000 apache-airflow-providers-common-sql-1.6.2rc1/apache_airflow_providers_common_sql.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 21:40:57.000000 apache-airflow-providers-common-sql-1.6.2rc1/apache_airflow_providers_common_sql.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      107 2023-08-04 21:40:57.000000 apache-airflow-providers-common-sql-1.6.2rc1/apache_airflow_providers_common_sql.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 21:40:57.000000 apache-airflow-providers-common-sql-1.6.2rc1/apache_airflow_providers_common_sql.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      120 2023-08-04 21:40:57.000000 apache-airflow-providers-common-sql-1.6.2rc1/apache_airflow_providers_common_sql.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-08-04 21:40:57.000000 apache-airflow-providers-common-sql-1.6.2rc1/apache_airflow_providers_common_sql.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5031 2023-08-04 10:24:23.000000 apache-airflow-providers-common-sql-1.6.2rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1970 2023-08-04 21:40:58.027302 apache-airflow-providers-common-sql-1.6.2rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1782 2023-08-04 21:40:56.000000 apache-airflow-providers-common-sql-1.6.2rc1/setup.py
```

### Comparing `apache-airflow-providers-common-sql-1.6.1rc1/LICENSE` & `apache-airflow-providers-common-sql-1.6.2rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-common-sql-1.6.1rc1/MANIFEST.in` & `apache-airflow-providers-common-sql-1.6.2rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-common-sql-1.6.1rc1/PKG-INFO` & `apache-airflow-providers-common-sql-1.6.2rc1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-common-sql
-Version: 1.6.1rc1
+Version: 1.6.2rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-common-sql package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-common-sql/1.6.1/
-Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-common-sql/1.6.1/changelog.html
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-common-sql/1.6.2/
+Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-common-sql/1.6.2/changelog.html
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -68,28 +68,28 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-common-sql``
 
-Release: ``1.6.1rc1``
+Release: ``1.6.2rc1``
 
 
 `Common SQL Provider <https://en.wikipedia.org/wiki/SQL>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``common.sql`` provider. All classes for this provider package
 are in ``airflow.providers.common.sql`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-common-sql/1.6.1/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-common-sql/1.6.2/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -123,8 +123,8 @@
 ==============================================================================================================  ===============
 Dependent package                                                                                               Extra
 ==============================================================================================================  ===============
 `apache-airflow-providers-openlineage <https://airflow.apache.org/docs/apache-airflow-providers-openlineage>`_  ``openlineage``
 ==============================================================================================================  ===============
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-common-sql/1.6.1/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-common-sql/1.6.2/changelog.html>`_.
```

### Comparing `apache-airflow-providers-common-sql-1.6.1rc1/README.rst` & `apache-airflow-providers-common-sql-1.6.2rc1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -32,28 +32,28 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-common-sql``
 
-Release: ``1.6.1rc1``
+Release: ``1.6.2rc1``
 
 
 `Common SQL Provider <https://en.wikipedia.org/wiki/SQL>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``common.sql`` provider. All classes for this provider package
 are in ``airflow.providers.common.sql`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-common-sql/1.6.1/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-common-sql/1.6.2/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -87,8 +87,8 @@
 ==============================================================================================================  ===============
 Dependent package                                                                                               Extra
 ==============================================================================================================  ===============
 `apache-airflow-providers-openlineage <https://airflow.apache.org/docs/apache-airflow-providers-openlineage>`_  ``openlineage``
 ==============================================================================================================  ===============
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-common-sql/1.6.1/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-common-sql/1.6.2/changelog.html>`_.
```

### Comparing `apache-airflow-providers-common-sql-1.6.1rc1/airflow/providers/common/sql/__init__.py` & `apache-airflow-providers-common-sql-1.6.2rc1/airflow/providers/common/sql/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 from __future__ import annotations
 
 import packaging.version
 
 __all__ = ["__version__"]
 
-__version__ = "1.6.1"
+__version__ = "1.6.2"
 
 try:
     from airflow import __version__ as airflow_version
 except ImportError:
     from airflow.version import version as airflow_version
 
 if packaging.version.parse(packaging.version.parse(airflow_version).base_version) < packaging.version.parse(
```

### Comparing `apache-airflow-providers-common-sql-1.6.1rc1/airflow/providers/common/sql/get_provider_info.py` & `apache-airflow-providers-common-sql-1.6.2rc1/airflow/providers/common/sql/get_provider_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-common-sql",
         "name": "Common SQL",
         "description": "`Common SQL Provider <https://en.wikipedia.org/wiki/SQL>`__\n",
         "suspended": False,
         "versions": [
+            "1.6.2",
             "1.6.1",
             "1.6.0",
             "1.5.2",
             "1.5.1",
             "1.5.0",
             "1.4.0",
             "1.3.4",
```

### Comparing `apache-airflow-providers-common-sql-1.6.1rc1/airflow/providers/common/sql/hooks/__init__.py` & `apache-airflow-providers-common-sql-1.6.2rc1/airflow/providers/common/sql/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-common-sql-1.6.1rc1/airflow/providers/common/sql/hooks/sql.py` & `apache-airflow-providers-common-sql-1.6.2rc1/airflow/providers/common/sql/hooks/sql.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-common-sql-1.6.1rc1/airflow/providers/common/sql/operators/__init__.py` & `apache-airflow-providers-common-sql-1.6.2rc1/airflow/providers/common/sql/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-common-sql-1.6.1rc1/airflow/providers/common/sql/operators/sql.py` & `apache-airflow-providers-common-sql-1.6.2rc1/airflow/providers/common/sql/operators/sql.py`

 * *Files 0% similar despite different names*

```diff
@@ -200,14 +200,16 @@
     :param sql: the SQL code or string pointing to a template file to be executed (templated).
         File must have a '.sql' extension.
     :param autocommit: (optional) if True, each command is automatically committed (default: False).
     :param parameters: (optional) the parameters to render the SQL query with.
     :param handler: (optional) the function that will be applied to the cursor (default: fetch_all_handler).
     :param split_statements: (optional) if split single SQL string into statements. By default, defers
         to the default value in the ``run`` method of the configured hook.
+    :param conn_id: the connection ID used to connect to the database
+    :param database: name of database which overwrite the defined one in connection
     :param return_last: (optional) return the result of only last statement (default: True).
     :param show_return_value_in_logs: (optional) if true operator output will be printed to the task log.
         Use with caution. It's not recommended to dump large datasets to the log. (default: False).
 
     .. seealso::
         For more information on how to use this operator, take a look at the guide:
         :ref:`howto/operator:SQLExecuteQueryOperator`
@@ -221,20 +223,22 @@
     def __init__(
         self,
         *,
         sql: str | list[str],
         autocommit: bool = False,
         parameters: Mapping | Iterable | None = None,
         handler: Callable[[Any], Any] = fetch_all_handler,
+        conn_id: str | None = None,
+        database: str | None = None,
         split_statements: bool | None = None,
         return_last: bool = True,
         show_return_value_in_logs: bool = False,
         **kwargs,
     ) -> None:
-        super().__init__(**kwargs)
+        super().__init__(conn_id=conn_id, database=database, **kwargs)
         self.sql = sql
         self.autocommit = autocommit
         self.parameters = parameters
         self.handler = handler
         self.split_statements = split_statements
         self.return_last = return_last
         self.show_return_value_in_logs = show_return_value_in_logs
@@ -899,16 +903,16 @@
         ".hql",
         ".sql",
     )
     template_fields_renderers = {"sql1": "sql", "sql2": "sql"}
     ui_color = "#fff7e6"
 
     ratio_formulas = {
-        "max_over_min": lambda cur, ref: float(max(cur, ref)) / min(cur, ref),
-        "relative_diff": lambda cur, ref: float(abs(cur - ref)) / ref,
+        "max_over_min": lambda cur, ref: max(cur, ref) / min(cur, ref),
+        "relative_diff": lambda cur, ref: abs(cur - ref) / ref,
     }
 
     def __init__(
         self,
         *,
         table: str,
         metrics_thresholds: dict[str, int],
```

### Comparing `apache-airflow-providers-common-sql-1.6.1rc1/airflow/providers/common/sql/sensors/__init__.py` & `apache-airflow-providers-common-sql-1.6.2rc1/airflow/providers/common/sql/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-common-sql-1.6.1rc1/airflow/providers/common/sql/sensors/sql.py` & `apache-airflow-providers-common-sql-1.6.2rc1/airflow/providers/common/sql/sensors/sql.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-common-sql-1.6.1rc1/apache_airflow_providers_common_sql.egg-info/PKG-INFO` & `apache-airflow-providers-common-sql-1.6.2rc1/apache_airflow_providers_common_sql.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-common-sql
-Version: 1.6.1rc1
+Version: 1.6.2rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-common-sql package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-common-sql/1.6.1/
-Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-common-sql/1.6.1/changelog.html
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-common-sql/1.6.2/
+Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-common-sql/1.6.2/changelog.html
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -68,28 +68,28 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-common-sql``
 
-Release: ``1.6.1rc1``
+Release: ``1.6.2rc1``
 
 
 `Common SQL Provider <https://en.wikipedia.org/wiki/SQL>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``common.sql`` provider. All classes for this provider package
 are in ``airflow.providers.common.sql`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-common-sql/1.6.1/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-common-sql/1.6.2/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -123,8 +123,8 @@
 ==============================================================================================================  ===============
 Dependent package                                                                                               Extra
 ==============================================================================================================  ===============
 `apache-airflow-providers-openlineage <https://airflow.apache.org/docs/apache-airflow-providers-openlineage>`_  ``openlineage``
 ==============================================================================================================  ===============
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-common-sql/1.6.1/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-common-sql/1.6.2/changelog.html>`_.
```

### Comparing `apache-airflow-providers-common-sql-1.6.1rc1/apache_airflow_providers_common_sql.egg-info/SOURCES.txt` & `apache-airflow-providers-common-sql-1.6.2rc1/apache_airflow_providers_common_sql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-common-sql-1.6.1rc1/pyproject.toml` & `apache-airflow-providers-common-sql-1.6.2rc1/pyproject.toml`

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

### Comparing `apache-airflow-providers-common-sql-1.6.1rc1/setup.cfg` & `apache-airflow-providers-common-sql-1.6.2rc1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -23,16 +23,16 @@
 	License :: OSI Approved :: Apache Software License
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	Topic :: System :: Monitoring
 project_urls = 
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-common-sql/1.6.1/
-	Changelog=https://airflow.apache.org/docs/apache-airflow-providers-common-sql/1.6.1/changelog.html
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-common-sql/1.6.2/
+	Changelog=https://airflow.apache.org/docs/apache-airflow-providers-common-sql/1.6.2/changelog.html
 	Bug Tracker=https://github.com/apache/airflow/issues
 	Source Code=https://github.com/apache/airflow
 	Slack Chat=https://s.apache.org/airflow-slack
 	Twitter=https://twitter.com/ApacheAirflow
 	YouTube=https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 
 [bdist_wheel]
```

### Comparing `apache-airflow-providers-common-sql-1.6.1rc1/setup.py` & `apache-airflow-providers-common-sql-1.6.2rc1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-common-sql package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "1.6.1"
+version = "1.6.2"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-common-sql setup."""
     setup(
         version=version,
         extras_require={
```

