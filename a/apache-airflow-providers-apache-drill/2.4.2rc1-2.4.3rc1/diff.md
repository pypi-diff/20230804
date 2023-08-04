# Comparing `tmp/apache-airflow-providers-apache-drill-2.4.2rc1.tar.gz` & `tmp/apache-airflow-providers-apache-drill-2.4.3rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-apache-drill-2.4.2rc1.tar", last modified: Sat Jul 29 12:07:53 2023, max compression
+gzip compressed data, was "apache-airflow-providers-apache-drill-2.4.3rc1.tar", last modified: Fri Aug  4 21:40:37 2023, max compression
```

## Comparing `apache-airflow-providers-apache-drill-2.4.2rc1.tar` & `apache-airflow-providers-apache-drill-2.4.3rc1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:07:53.339467 apache-airflow-providers-apache-drill-2.4.2rc1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-drill-2.4.2rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-07-29 12:07:52.000000 apache-airflow-providers-apache-drill-2.4.2rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-drill-2.4.2rc1/NOTICE
--rw-r--r--   0 root         (0) root         (0)     5714 2023-07-29 12:07:53.340090 apache-airflow-providers-apache-drill-2.4.2rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4025 2023-07-29 12:07:52.000000 apache-airflow-providers-apache-drill-2.4.2rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:07:53.266945 apache-airflow-providers-apache-drill-2.4.2rc1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:07:53.267946 apache-airflow-providers-apache-drill-2.4.2rc1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:07:53.269070 apache-airflow-providers-apache-drill-2.4.2rc1/airflow/providers/apache/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:07:53.301790 apache-airflow-providers-apache-drill-2.4.2rc1/airflow/providers/apache/drill/
--rw-r--r--   0 root         (0) root         (0)     1581 2023-07-29 12:01:19.000000 apache-airflow-providers-apache-drill-2.4.2rc1/airflow/providers/apache/drill/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2757 2023-07-29 12:07:52.000000 apache-airflow-providers-apache-drill-2.4.2rc1/airflow/providers/apache/drill/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:07:53.307588 apache-airflow-providers-apache-drill-2.4.2rc1/airflow/providers/apache/drill/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-drill-2.4.2rc1/airflow/providers/apache/drill/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3660 2023-06-01 07:44:14.000000 apache-airflow-providers-apache-drill-2.4.2rc1/airflow/providers/apache/drill/hooks/drill.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:07:53.313272 apache-airflow-providers-apache-drill-2.4.2rc1/airflow/providers/apache/drill/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-drill-2.4.2rc1/airflow/providers/apache/drill/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2346 2023-07-16 17:25:26.000000 apache-airflow-providers-apache-drill-2.4.2rc1/airflow/providers/apache/drill/operators/drill.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:07:53.336782 apache-airflow-providers-apache-drill-2.4.2rc1/apache_airflow_providers_apache_drill.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5714 2023-07-29 12:07:53.000000 apache-airflow-providers-apache-drill-2.4.2rc1/apache_airflow_providers_apache_drill.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      792 2023-07-29 12:07:53.000000 apache-airflow-providers-apache-drill-2.4.2rc1/apache_airflow_providers_apache_drill.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:07:53.000000 apache-airflow-providers-apache-drill-2.4.2rc1/apache_airflow_providers_apache_drill.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      109 2023-07-29 12:07:53.000000 apache-airflow-providers-apache-drill-2.4.2rc1/apache_airflow_providers_apache_drill.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:07:53.000000 apache-airflow-providers-apache-drill-2.4.2rc1/apache_airflow_providers_apache_drill.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      149 2023-07-29 12:07:53.000000 apache-airflow-providers-apache-drill-2.4.2rc1/apache_airflow_providers_apache_drill.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-07-29 12:07:53.000000 apache-airflow-providers-apache-drill-2.4.2rc1/apache_airflow_providers_apache_drill.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5011 2023-07-27 05:54:58.000000 apache-airflow-providers-apache-drill-2.4.2rc1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     2041 2023-07-29 12:07:53.342061 apache-airflow-providers-apache-drill-2.4.2rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1727 2023-07-29 12:07:52.000000 apache-airflow-providers-apache-drill-2.4.2rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:40:37.478341 apache-airflow-providers-apache-drill-2.4.3rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-drill-2.4.3rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-08-04 21:40:36.000000 apache-airflow-providers-apache-drill-2.4.3rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-drill-2.4.3rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     5714 2023-08-04 21:40:37.478901 apache-airflow-providers-apache-drill-2.4.3rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4025 2023-08-04 21:40:36.000000 apache-airflow-providers-apache-drill-2.4.3rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:40:37.380637 apache-airflow-providers-apache-drill-2.4.3rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:40:37.381959 apache-airflow-providers-apache-drill-2.4.3rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:40:37.383293 apache-airflow-providers-apache-drill-2.4.3rc1/airflow/providers/apache/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:40:37.430619 apache-airflow-providers-apache-drill-2.4.3rc1/airflow/providers/apache/drill/
+-rw-r--r--   0 root         (0) root         (0)     1581 2023-08-04 21:33:34.000000 apache-airflow-providers-apache-drill-2.4.3rc1/airflow/providers/apache/drill/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2778 2023-08-04 21:40:36.000000 apache-airflow-providers-apache-drill-2.4.3rc1/airflow/providers/apache/drill/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:40:37.438827 apache-airflow-providers-apache-drill-2.4.3rc1/airflow/providers/apache/drill/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-drill-2.4.3rc1/airflow/providers/apache/drill/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4149 2023-08-04 10:24:22.000000 apache-airflow-providers-apache-drill-2.4.3rc1/airflow/providers/apache/drill/hooks/drill.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:40:37.445840 apache-airflow-providers-apache-drill-2.4.3rc1/airflow/providers/apache/drill/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-drill-2.4.3rc1/airflow/providers/apache/drill/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2346 2023-07-16 17:25:26.000000 apache-airflow-providers-apache-drill-2.4.3rc1/airflow/providers/apache/drill/operators/drill.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:40:37.475566 apache-airflow-providers-apache-drill-2.4.3rc1/apache_airflow_providers_apache_drill.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5714 2023-08-04 21:40:37.000000 apache-airflow-providers-apache-drill-2.4.3rc1/apache_airflow_providers_apache_drill.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      792 2023-08-04 21:40:37.000000 apache-airflow-providers-apache-drill-2.4.3rc1/apache_airflow_providers_apache_drill.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 21:40:37.000000 apache-airflow-providers-apache-drill-2.4.3rc1/apache_airflow_providers_apache_drill.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      109 2023-08-04 21:40:37.000000 apache-airflow-providers-apache-drill-2.4.3rc1/apache_airflow_providers_apache_drill.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 21:40:37.000000 apache-airflow-providers-apache-drill-2.4.3rc1/apache_airflow_providers_apache_drill.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      149 2023-08-04 21:40:37.000000 apache-airflow-providers-apache-drill-2.4.3rc1/apache_airflow_providers_apache_drill.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-08-04 21:40:37.000000 apache-airflow-providers-apache-drill-2.4.3rc1/apache_airflow_providers_apache_drill.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5031 2023-08-04 10:24:23.000000 apache-airflow-providers-apache-drill-2.4.3rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     2041 2023-08-04 21:40:37.480942 apache-airflow-providers-apache-drill-2.4.3rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1727 2023-08-04 21:40:36.000000 apache-airflow-providers-apache-drill-2.4.3rc1/setup.py
```

### Comparing `apache-airflow-providers-apache-drill-2.4.2rc1/LICENSE` & `apache-airflow-providers-apache-drill-2.4.3rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-drill-2.4.2rc1/MANIFEST.in` & `apache-airflow-providers-apache-drill-2.4.3rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-drill-2.4.2rc1/PKG-INFO` & `apache-airflow-providers-apache-drill-2.4.3rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-apache-drill
-Version: 2.4.2rc1
+Version: 2.4.3rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-apache-drill package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-drill/2.4.2/
-Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-apache-drill/2.4.2/changelog.html
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-drill/2.4.3/
+Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-apache-drill/2.4.3/changelog.html
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
 
 
 Package ``apache-airflow-providers-apache-drill``
 
-Release: ``2.4.2rc1``
+Release: ``2.4.3rc1``
 
 
 `Apache Drill <https://drill.apache.org/>`__.
 
 
 Provider package
 ----------------
 
 This is a provider package for ``apache.drill`` provider. All classes for this provider package
 are in ``airflow.providers.apache.drill`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apache-drill/2.4.2/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apache-drill/2.4.3/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -123,8 +123,8 @@
 ============================================================================================================  ==============
 Dependent package                                                                                             Extra
 ============================================================================================================  ==============
 `apache-airflow-providers-common-sql <https://airflow.apache.org/docs/apache-airflow-providers-common-sql>`_  ``common.sql``
 ============================================================================================================  ==============
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-apache-drill/2.4.2/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-apache-drill/2.4.3/changelog.html>`_.
```

### Comparing `apache-airflow-providers-apache-drill-2.4.2rc1/README.rst` & `apache-airflow-providers-apache-drill-2.4.3rc1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -32,28 +32,28 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-apache-drill``
 
-Release: ``2.4.2rc1``
+Release: ``2.4.3rc1``
 
 
 `Apache Drill <https://drill.apache.org/>`__.
 
 
 Provider package
 ----------------
 
 This is a provider package for ``apache.drill`` provider. All classes for this provider package
 are in ``airflow.providers.apache.drill`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apache-drill/2.4.2/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apache-drill/2.4.3/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -88,8 +88,8 @@
 ============================================================================================================  ==============
 Dependent package                                                                                             Extra
 ============================================================================================================  ==============
 `apache-airflow-providers-common-sql <https://airflow.apache.org/docs/apache-airflow-providers-common-sql>`_  ``common.sql``
 ============================================================================================================  ==============
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-apache-drill/2.4.2/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-apache-drill/2.4.3/changelog.html>`_.
```

### Comparing `apache-airflow-providers-apache-drill-2.4.2rc1/airflow/providers/apache/drill/__init__.py` & `apache-airflow-providers-apache-drill-2.4.3rc1/airflow/providers/apache/drill/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 from __future__ import annotations
 
 import packaging.version
 
 __all__ = ["__version__"]
 
-__version__ = "2.4.2"
+__version__ = "2.4.3"
 
 try:
     from airflow import __version__ as airflow_version
 except ImportError:
     from airflow.version import version as airflow_version
 
 if packaging.version.parse(packaging.version.parse(airflow_version).base_version) < packaging.version.parse(
```

### Comparing `apache-airflow-providers-apache-drill-2.4.2rc1/airflow/providers/apache/drill/get_provider_info.py` & `apache-airflow-providers-apache-drill-2.4.3rc1/airflow/providers/apache/drill/get_provider_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-apache-drill",
         "name": "Apache Drill",
         "description": "`Apache Drill <https://drill.apache.org/>`__.\n",
         "suspended": False,
         "versions": [
+            "2.4.3",
             "2.4.2",
             "2.4.1",
             "2.4.0",
             "2.3.2",
             "2.3.1",
             "2.3.0",
             "2.2.1",
```

### Comparing `apache-airflow-providers-apache-drill-2.4.2rc1/airflow/providers/apache/drill/hooks/__init__.py` & `apache-airflow-providers-apache-drill-2.4.3rc1/airflow/providers/apache/drill/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-drill-2.4.2rc1/airflow/providers/apache/drill/hooks/drill.py` & `apache-airflow-providers-apache-drill-2.4.3rc1/airflow/providers/apache/drill/hooks/drill.py`

 * *Files 16% similar despite different names*

```diff
@@ -45,21 +45,22 @@
     hook_name = "Drill"
     supports_autocommit = False
 
     def get_conn(self) -> Connection:
         """Establish a connection to Drillbit."""
         conn_md = self.get_connection(getattr(self, self.conn_name_attr))
         creds = f"{conn_md.login}:{conn_md.password}@" if conn_md.login else ""
-        if "/" in conn_md.host or "&" in conn_md.host:
-            raise ValueError("Drill host should not contain '/&' characters")
-        engine = create_engine(
-            f'{conn_md.extra_dejson.get("dialect_driver", "drill+sadrill")}://{creds}'
+        database_url = (
+            f"{conn_md.extra_dejson.get('dialect_driver', 'drill+sadrill')}://{creds}"
             f"{conn_md.host}:{conn_md.port}/"
             f'{conn_md.extra_dejson.get("storage_plugin", "dfs")}'
         )
+        if "?" in database_url:
+            raise ValueError("Drill database_url should not contain a '?'")
+        engine = create_engine(database_url)
 
         self.log.info(
             "Connected to the Drillbit at %s:%s as user %s", conn_md.host, conn_md.port, conn_md.login
         )
         return engine.raw_connection()
 
     def get_uri(self) -> str:
@@ -73,18 +74,24 @@
         if conn_md.port is not None:
             host += f":{conn_md.port}"
         conn_type = conn_md.conn_type or "drill"
         dialect_driver = conn_md.extra_dejson.get("dialect_driver", "drill+sadrill")
         storage_plugin = conn_md.extra_dejson.get("storage_plugin", "dfs")
         return f"{conn_type}://{host}/{storage_plugin}?dialect_driver={dialect_driver}"
 
-    def set_autocommit(self, conn: Connection, autocommit: bool) -> NotImplementedError:
+    # The superclass DbApiHook's method implementation has a return type `None` and mypy fails saying
+    # return type `NotImplementedError` is incompatible with it. Hence, we ignore the mypy error here.
+    def set_autocommit(  # type: ignore[override]
+        self, conn: Connection, autocommit: bool
+    ) -> NotImplementedError:
         raise NotImplementedError("There are no transactions in Drill.")
 
-    def insert_rows(
+    # The superclass DbApiHook's method implementation has a return type `None` and mypy fails saying
+    # return type `NotImplementedError` is incompatible with it. Hence, we ignore the mypy error here.
+    def insert_rows(  # type: ignore[override]
         self,
         table: str,
         rows: Iterable[tuple[str]],
         target_fields: Iterable[str] | None = None,
         commit_every: int = 1000,
         replace: bool = False,
         **kwargs: Any,
```

### Comparing `apache-airflow-providers-apache-drill-2.4.2rc1/airflow/providers/apache/drill/operators/__init__.py` & `apache-airflow-providers-apache-drill-2.4.3rc1/airflow/providers/apache/drill/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-drill-2.4.2rc1/airflow/providers/apache/drill/operators/drill.py` & `apache-airflow-providers-apache-drill-2.4.3rc1/airflow/providers/apache/drill/operators/drill.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-drill-2.4.2rc1/apache_airflow_providers_apache_drill.egg-info/PKG-INFO` & `apache-airflow-providers-apache-drill-2.4.3rc1/apache_airflow_providers_apache_drill.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-apache-drill
-Version: 2.4.2rc1
+Version: 2.4.3rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-apache-drill package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-drill/2.4.2/
-Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-apache-drill/2.4.2/changelog.html
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-drill/2.4.3/
+Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-apache-drill/2.4.3/changelog.html
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
 
 
 Package ``apache-airflow-providers-apache-drill``
 
-Release: ``2.4.2rc1``
+Release: ``2.4.3rc1``
 
 
 `Apache Drill <https://drill.apache.org/>`__.
 
 
 Provider package
 ----------------
 
 This is a provider package for ``apache.drill`` provider. All classes for this provider package
 are in ``airflow.providers.apache.drill`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apache-drill/2.4.2/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-apache-drill/2.4.3/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -123,8 +123,8 @@
 ============================================================================================================  ==============
 Dependent package                                                                                             Extra
 ============================================================================================================  ==============
 `apache-airflow-providers-common-sql <https://airflow.apache.org/docs/apache-airflow-providers-common-sql>`_  ``common.sql``
 ============================================================================================================  ==============
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-apache-drill/2.4.2/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-apache-drill/2.4.3/changelog.html>`_.
```

### Comparing `apache-airflow-providers-apache-drill-2.4.2rc1/apache_airflow_providers_apache_drill.egg-info/SOURCES.txt` & `apache-airflow-providers-apache-drill-2.4.3rc1/apache_airflow_providers_apache_drill.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-drill-2.4.2rc1/pyproject.toml` & `apache-airflow-providers-apache-drill-2.4.3rc1/pyproject.toml`

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

### Comparing `apache-airflow-providers-apache-drill-2.4.2rc1/setup.cfg` & `apache-airflow-providers-apache-drill-2.4.3rc1/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -23,16 +23,16 @@
 	License :: OSI Approved :: Apache Software License
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	Topic :: System :: Monitoring
 project_urls = 
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-apache-drill/2.4.2/
-	Changelog=https://airflow.apache.org/docs/apache-airflow-providers-apache-drill/2.4.2/changelog.html
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-apache-drill/2.4.3/
+	Changelog=https://airflow.apache.org/docs/apache-airflow-providers-apache-drill/2.4.3/changelog.html
 	Bug Tracker=https://github.com/apache/airflow/issues
 	Source Code=https://github.com/apache/airflow
 	Slack Chat=https://s.apache.org/airflow-slack
 	Twitter=https://twitter.com/ApacheAirflow
 	YouTube=https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 
 [bdist_wheel]
```

### Comparing `apache-airflow-providers-apache-drill-2.4.2rc1/setup.py` & `apache-airflow-providers-apache-drill-2.4.3rc1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-apache-drill package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "2.4.2"
+version = "2.4.3"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-apache-drill setup."""
     setup(
         version=version,
         extras_require={"common.sql": ["apache-airflow-providers-common-sql"]},
```

