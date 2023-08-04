# Comparing `tmp/apache-airflow-providers-openlineage-1.0.0rc1.tar.gz` & `tmp/apache-airflow-providers-openlineage-1.0.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-openlineage-1.0.0rc1.tar", last modified: Sat Jul 29 12:08:49 2023, max compression
+gzip compressed data, was "apache-airflow-providers-openlineage-1.0.1rc1.tar", last modified: Fri Aug  4 21:41:28 2023, max compression
```

## Comparing `apache-airflow-providers-openlineage-1.0.0rc1.tar` & `apache-airflow-providers-openlineage-1.0.1rc1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:49.878147 apache-airflow-providers-openlineage-1.0.0rc1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-openlineage-1.0.0rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-07-29 12:08:48.000000 apache-airflow-providers-openlineage-1.0.0rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-openlineage-1.0.0rc1/NOTICE
--rw-r--r--   0 root         (0) root         (0)     5806 2023-07-29 12:08:49.878673 apache-airflow-providers-openlineage-1.0.0rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4121 2023-07-29 12:08:48.000000 apache-airflow-providers-openlineage-1.0.0rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:49.773138 apache-airflow-providers-openlineage-1.0.0rc1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:49.774433 apache-airflow-providers-openlineage-1.0.0rc1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:49.811232 apache-airflow-providers-openlineage-1.0.0rc1/airflow/providers/openlineage/
--rw-r--r--   0 root         (0) root         (0)     1580 2023-07-29 12:01:19.000000 apache-airflow-providers-openlineage-1.0.0rc1/airflow/providers/openlineage/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:49.826250 apache-airflow-providers-openlineage-1.0.0rc1/airflow/providers/openlineage/extractors/
--rw-r--r--   0 root         (0) root         (0)     1081 2023-06-01 06:14:28.000000 apache-airflow-providers-openlineage-1.0.0rc1/airflow/providers/openlineage/extractors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4568 2023-07-27 05:54:58.000000 apache-airflow-providers-openlineage-1.0.0rc1/airflow/providers/openlineage/extractors/base.py
--rw-r--r--   0 root         (0) root         (0)     2735 2023-07-27 05:54:58.000000 apache-airflow-providers-openlineage-1.0.0rc1/airflow/providers/openlineage/extractors/bash.py
--rw-r--r--   0 root         (0) root         (0)     7806 2023-07-27 05:54:58.000000 apache-airflow-providers-openlineage-1.0.0rc1/airflow/providers/openlineage/extractors/manager.py
--rw-r--r--   0 root         (0) root         (0)     3270 2023-07-27 05:54:58.000000 apache-airflow-providers-openlineage-1.0.0rc1/airflow/providers/openlineage/extractors/python.py
--rw-r--r--   0 root         (0) root         (0)     2054 2023-07-29 12:08:48.000000 apache-airflow-providers-openlineage-1.0.0rc1/airflow/providers/openlineage/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:49.843215 apache-airflow-providers-openlineage-1.0.0rc1/airflow/providers/openlineage/plugins/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-openlineage-1.0.0rc1/airflow/providers/openlineage/plugins/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12484 2023-07-27 05:54:58.000000 apache-airflow-providers-openlineage-1.0.0rc1/airflow/providers/openlineage/plugins/adapter.py
--rw-r--r--   0 root         (0) root         (0)     2218 2023-07-27 05:54:58.000000 apache-airflow-providers-openlineage-1.0.0rc1/airflow/providers/openlineage/plugins/facets.py
--rw-r--r--   0 root         (0) root         (0)     7256 2023-07-05 07:19:39.000000 apache-airflow-providers-openlineage-1.0.0rc1/airflow/providers/openlineage/plugins/listener.py
--rw-r--r--   0 root         (0) root         (0)     2356 2023-07-05 07:19:39.000000 apache-airflow-providers-openlineage-1.0.0rc1/airflow/providers/openlineage/plugins/macros.py
--rw-r--r--   0 root         (0) root         (0)     1688 2023-07-05 07:19:39.000000 apache-airflow-providers-openlineage-1.0.0rc1/airflow/providers/openlineage/plugins/openlineage.py
--rw-r--r--   0 root         (0) root         (0)    11218 2023-07-27 05:54:58.000000 apache-airflow-providers-openlineage-1.0.0rc1/airflow/providers/openlineage/sqlparser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:49.851742 apache-airflow-providers-openlineage-1.0.0rc1/airflow/providers/openlineage/utils/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-openlineage-1.0.0rc1/airflow/providers/openlineage/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7038 2023-07-27 05:54:58.000000 apache-airflow-providers-openlineage-1.0.0rc1/airflow/providers/openlineage/utils/sql.py
--rw-r--r--   0 root         (0) root         (0)    13269 2023-07-27 05:54:58.000000 apache-airflow-providers-openlineage-1.0.0rc1/airflow/providers/openlineage/utils/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:49.875542 apache-airflow-providers-openlineage-1.0.0rc1/apache_airflow_providers_openlineage.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5806 2023-07-29 12:08:49.000000 apache-airflow-providers-openlineage-1.0.0rc1/apache_airflow_providers_openlineage.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1316 2023-07-29 12:08:49.000000 apache-airflow-providers-openlineage-1.0.0rc1/apache_airflow_providers_openlineage.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:08:49.000000 apache-airflow-providers-openlineage-1.0.0rc1/apache_airflow_providers_openlineage.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      217 2023-07-29 12:08:49.000000 apache-airflow-providers-openlineage-1.0.0rc1/apache_airflow_providers_openlineage.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:08:49.000000 apache-airflow-providers-openlineage-1.0.0rc1/apache_airflow_providers_openlineage.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      203 2023-07-29 12:08:49.000000 apache-airflow-providers-openlineage-1.0.0rc1/apache_airflow_providers_openlineage.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-07-29 12:08:49.000000 apache-airflow-providers-openlineage-1.0.0rc1/apache_airflow_providers_openlineage.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5011 2023-07-27 05:54:58.000000 apache-airflow-providers-openlineage-1.0.0rc1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     2198 2023-07-29 12:08:49.880511 apache-airflow-providers-openlineage-1.0.0rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1721 2023-07-29 12:08:48.000000 apache-airflow-providers-openlineage-1.0.0rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:41:28.918074 apache-airflow-providers-openlineage-1.0.1rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-openlineage-1.0.1rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-08-04 21:41:27.000000 apache-airflow-providers-openlineage-1.0.1rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-openlineage-1.0.1rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     5806 2023-08-04 21:41:28.918956 apache-airflow-providers-openlineage-1.0.1rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4121 2023-08-04 21:41:27.000000 apache-airflow-providers-openlineage-1.0.1rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:41:28.802473 apache-airflow-providers-openlineage-1.0.1rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:41:28.803773 apache-airflow-providers-openlineage-1.0.1rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:41:28.841940 apache-airflow-providers-openlineage-1.0.1rc1/airflow/providers/openlineage/
+-rw-r--r--   0 root         (0) root         (0)     1580 2023-08-04 21:33:34.000000 apache-airflow-providers-openlineage-1.0.1rc1/airflow/providers/openlineage/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:41:28.855989 apache-airflow-providers-openlineage-1.0.1rc1/airflow/providers/openlineage/extractors/
+-rw-r--r--   0 root         (0) root         (0)     1081 2023-06-01 06:14:28.000000 apache-airflow-providers-openlineage-1.0.1rc1/airflow/providers/openlineage/extractors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4831 2023-08-04 19:44:14.000000 apache-airflow-providers-openlineage-1.0.1rc1/airflow/providers/openlineage/extractors/base.py
+-rw-r--r--   0 root         (0) root         (0)     2735 2023-07-27 05:54:58.000000 apache-airflow-providers-openlineage-1.0.1rc1/airflow/providers/openlineage/extractors/bash.py
+-rw-r--r--   0 root         (0) root         (0)     7806 2023-07-27 05:54:58.000000 apache-airflow-providers-openlineage-1.0.1rc1/airflow/providers/openlineage/extractors/manager.py
+-rw-r--r--   0 root         (0) root         (0)     3270 2023-07-27 05:54:58.000000 apache-airflow-providers-openlineage-1.0.1rc1/airflow/providers/openlineage/extractors/python.py
+-rw-r--r--   0 root         (0) root         (0)     4850 2023-08-04 21:41:27.000000 apache-airflow-providers-openlineage-1.0.1rc1/airflow/providers/openlineage/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:41:28.873537 apache-airflow-providers-openlineage-1.0.1rc1/airflow/providers/openlineage/plugins/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-openlineage-1.0.1rc1/airflow/providers/openlineage/plugins/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12484 2023-07-27 05:54:58.000000 apache-airflow-providers-openlineage-1.0.1rc1/airflow/providers/openlineage/plugins/adapter.py
+-rw-r--r--   0 root         (0) root         (0)     2218 2023-07-27 05:54:58.000000 apache-airflow-providers-openlineage-1.0.1rc1/airflow/providers/openlineage/plugins/facets.py
+-rw-r--r--   0 root         (0) root         (0)     7256 2023-07-05 07:19:39.000000 apache-airflow-providers-openlineage-1.0.1rc1/airflow/providers/openlineage/plugins/listener.py
+-rw-r--r--   0 root         (0) root         (0)     2356 2023-07-05 07:19:39.000000 apache-airflow-providers-openlineage-1.0.1rc1/airflow/providers/openlineage/plugins/macros.py
+-rw-r--r--   0 root         (0) root         (0)     1986 2023-08-04 20:15:26.000000 apache-airflow-providers-openlineage-1.0.1rc1/airflow/providers/openlineage/plugins/openlineage.py
+-rw-r--r--   0 root         (0) root         (0)    11220 2023-08-04 10:24:22.000000 apache-airflow-providers-openlineage-1.0.1rc1/airflow/providers/openlineage/sqlparser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:41:28.882160 apache-airflow-providers-openlineage-1.0.1rc1/airflow/providers/openlineage/utils/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-openlineage-1.0.1rc1/airflow/providers/openlineage/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7038 2023-07-27 05:54:58.000000 apache-airflow-providers-openlineage-1.0.1rc1/airflow/providers/openlineage/utils/sql.py
+-rw-r--r--   0 root         (0) root         (0)    13516 2023-08-04 19:44:14.000000 apache-airflow-providers-openlineage-1.0.1rc1/airflow/providers/openlineage/utils/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:41:28.913214 apache-airflow-providers-openlineage-1.0.1rc1/apache_airflow_providers_openlineage.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5806 2023-08-04 21:41:28.000000 apache-airflow-providers-openlineage-1.0.1rc1/apache_airflow_providers_openlineage.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1316 2023-08-04 21:41:28.000000 apache-airflow-providers-openlineage-1.0.1rc1/apache_airflow_providers_openlineage.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 21:41:28.000000 apache-airflow-providers-openlineage-1.0.1rc1/apache_airflow_providers_openlineage.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      217 2023-08-04 21:41:28.000000 apache-airflow-providers-openlineage-1.0.1rc1/apache_airflow_providers_openlineage.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 21:41:28.000000 apache-airflow-providers-openlineage-1.0.1rc1/apache_airflow_providers_openlineage.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      203 2023-08-04 21:41:28.000000 apache-airflow-providers-openlineage-1.0.1rc1/apache_airflow_providers_openlineage.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-08-04 21:41:28.000000 apache-airflow-providers-openlineage-1.0.1rc1/apache_airflow_providers_openlineage.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5031 2023-08-04 10:24:23.000000 apache-airflow-providers-openlineage-1.0.1rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     2198 2023-08-04 21:41:28.921712 apache-airflow-providers-openlineage-1.0.1rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1721 2023-08-04 21:41:27.000000 apache-airflow-providers-openlineage-1.0.1rc1/setup.py
```

### Comparing `apache-airflow-providers-openlineage-1.0.0rc1/LICENSE` & `apache-airflow-providers-openlineage-1.0.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-openlineage-1.0.0rc1/MANIFEST.in` & `apache-airflow-providers-openlineage-1.0.1rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-openlineage-1.0.0rc1/PKG-INFO` & `apache-airflow-providers-openlineage-1.0.1rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-openlineage
-Version: 1.0.0rc1
+Version: 1.0.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-openlineage package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-openlineage/1.0.0/
-Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-openlineage/1.0.0/changelog.html
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-openlineage/1.0.1/
+Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-openlineage/1.0.1/changelog.html
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
 
 
 Package ``apache-airflow-providers-openlineage``
 
-Release: ``1.0.0rc1``
+Release: ``1.0.1rc1``
 
 
 `OpenLineage <https://openlineage.io/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``openlineage`` provider. All classes for this provider package
 are in ``airflow.providers.openlineage`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-openlineage/1.0.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-openlineage/1.0.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -125,8 +125,8 @@
 ============================================================================================================  ==============
 Dependent package                                                                                             Extra
 ============================================================================================================  ==============
 `apache-airflow-providers-common-sql <https://airflow.apache.org/docs/apache-airflow-providers-common-sql>`_  ``common.sql``
 ============================================================================================================  ==============
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-openlineage/1.0.0/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-openlineage/1.0.1/changelog.html>`_.
```

### Comparing `apache-airflow-providers-openlineage-1.0.0rc1/README.rst` & `apache-airflow-providers-openlineage-1.0.1rc1/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -32,28 +32,28 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-openlineage``
 
-Release: ``1.0.0rc1``
+Release: ``1.0.1rc1``
 
 
 `OpenLineage <https://openlineage.io/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``openlineage`` provider. All classes for this provider package
 are in ``airflow.providers.openlineage`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-openlineage/1.0.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-openlineage/1.0.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -90,8 +90,8 @@
 ============================================================================================================  ==============
 Dependent package                                                                                             Extra
 ============================================================================================================  ==============
 `apache-airflow-providers-common-sql <https://airflow.apache.org/docs/apache-airflow-providers-common-sql>`_  ``common.sql``
 ============================================================================================================  ==============
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-openlineage/1.0.0/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-openlineage/1.0.1/changelog.html>`_.
```

### Comparing `apache-airflow-providers-openlineage-1.0.0rc1/airflow/providers/openlineage/__init__.py` & `apache-airflow-providers-openlineage-1.0.1rc1/airflow/providers/openlineage/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 from __future__ import annotations
 
 import packaging.version
 
 __all__ = ["__version__"]
 
-__version__ = "1.0.0"
+__version__ = "1.0.1"
 
 try:
     from airflow import __version__ as airflow_version
 except ImportError:
     from airflow.version import version as airflow_version
 
 if packaging.version.parse(packaging.version.parse(airflow_version).base_version) < packaging.version.parse(
```

### Comparing `apache-airflow-providers-openlineage-1.0.0rc1/airflow/providers/openlineage/extractors/__init__.py` & `apache-airflow-providers-openlineage-1.0.1rc1/airflow/providers/openlineage/extractors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-openlineage-1.0.0rc1/airflow/providers/openlineage/extractors/base.py` & `apache-airflow-providers-openlineage-1.0.1rc1/airflow/providers/openlineage/extractors/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -82,14 +82,20 @@
         """
         return []
 
     def extract(self) -> OperatorLineage | None:
         # OpenLineage methods are optional - if there's no method, return None
         try:
             return self._get_openlineage_facets(self.operator.get_openlineage_facets_on_start)  # type: ignore
+        except ImportError:
+            self.log.error(
+                "OpenLineage provider method failed to import OpenLineage integration. "
+                "This should not happen. Please report this bug to developers."
+            )
+            return None
         except AttributeError:
             return None
 
     def extract_on_complete(self, task_instance) -> OperatorLineage | None:
         if task_instance.state == TaskInstanceState.FAILED:
             on_failed = getattr(self.operator, "get_openlineage_facets_on_failure", None)
             if on_failed and callable(on_failed):
```

### Comparing `apache-airflow-providers-openlineage-1.0.0rc1/airflow/providers/openlineage/extractors/bash.py` & `apache-airflow-providers-openlineage-1.0.1rc1/airflow/providers/openlineage/extractors/bash.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-openlineage-1.0.0rc1/airflow/providers/openlineage/extractors/manager.py` & `apache-airflow-providers-openlineage-1.0.1rc1/airflow/providers/openlineage/extractors/manager.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-openlineage-1.0.0rc1/airflow/providers/openlineage/extractors/python.py` & `apache-airflow-providers-openlineage-1.0.1rc1/airflow/providers/openlineage/extractors/python.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-openlineage-1.0.0rc1/airflow/providers/openlineage/plugins/__init__.py` & `apache-airflow-providers-openlineage-1.0.1rc1/airflow/providers/openlineage/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-openlineage-1.0.0rc1/airflow/providers/openlineage/plugins/adapter.py` & `apache-airflow-providers-openlineage-1.0.1rc1/airflow/providers/openlineage/plugins/adapter.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-openlineage-1.0.0rc1/airflow/providers/openlineage/plugins/facets.py` & `apache-airflow-providers-openlineage-1.0.1rc1/airflow/providers/openlineage/plugins/facets.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-openlineage-1.0.0rc1/airflow/providers/openlineage/plugins/listener.py` & `apache-airflow-providers-openlineage-1.0.1rc1/airflow/providers/openlineage/plugins/listener.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-openlineage-1.0.0rc1/airflow/providers/openlineage/plugins/macros.py` & `apache-airflow-providers-openlineage-1.0.1rc1/airflow/providers/openlineage/plugins/macros.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-openlineage-1.0.0rc1/airflow/providers/openlineage/plugins/openlineage.py` & `apache-airflow-providers-openlineage-1.0.1rc1/airflow/providers/openlineage/plugins/openlineage.py`

 * *Files 17% similar despite different names*

```diff
@@ -21,26 +21,32 @@
 from airflow.configuration import conf
 from airflow.plugins_manager import AirflowPlugin
 from airflow.providers.openlineage.plugins.macros import lineage_parent_id, lineage_run_id
 
 
 def _is_disabled() -> bool:
     return (
-        conf.getboolean("openlineage", "disabled")
+        conf.getboolean("openlineage", "disabled", fallback=False)
         or os.getenv("OPENLINEAGE_DISABLED", "false").lower() == "true"
+        or (
+            conf.get("openlineage", "transport", fallback="") == ""
+            and conf.get("openlineage", "config_path", fallback="") == ""
+            and os.getenv("OPENLINEAGE_URL", "") == ""
+            and os.getenv("OPENLINEAGE_CONFIG", "") == ""
+        )
     )
 
 
 class OpenLineageProviderPlugin(AirflowPlugin):
     """
     Listener that emits numerous Events.
 
     OpenLineage Plugin provides listener that emits OL events on DAG start,
     complete and failure and TaskInstances start, complete and failure.
     """
 
     name = "OpenLineageProviderPlugin"
-    macros = [lineage_run_id, lineage_parent_id]
     if not _is_disabled():
         from airflow.providers.openlineage.plugins.listener import OpenLineageListener
 
+        macros = [lineage_run_id, lineage_parent_id]
         listeners = [OpenLineageListener()]
```

### Comparing `apache-airflow-providers-openlineage-1.0.0rc1/airflow/providers/openlineage/sqlparser.py` & `apache-airflow-providers-openlineage-1.0.1rc1/airflow/providers/openlineage/sqlparser.py`

 * *Files 0% similar despite different names*

```diff
@@ -287,10 +287,10 @@
         hierarchy: TablesHierarchy = {}
         for table in tables:
             if is_cross_db:
                 db = table.database or database
             else:
                 db = None
             schemas = hierarchy.setdefault(normalize_name(db) if db else db, {})
-            tables = schemas.setdefault(normalize_name(table.schema) if table.schema else db, [])
+            tables = schemas.setdefault(normalize_name(table.schema) if table.schema else None, [])
             tables.append(table.name)
         return hierarchy
```

### Comparing `apache-airflow-providers-openlineage-1.0.0rc1/airflow/providers/openlineage/utils/__init__.py` & `apache-airflow-providers-openlineage-1.0.1rc1/airflow/providers/openlineage/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-openlineage-1.0.0rc1/airflow/providers/openlineage/utils/sql.py` & `apache-airflow-providers-openlineage-1.0.1rc1/airflow/providers/openlineage/utils/sql.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-openlineage-1.0.0rc1/airflow/providers/openlineage/utils/utils.py` & `apache-airflow-providers-openlineage-1.0.1rc1/airflow/providers/openlineage/utils/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 import datetime
 import json
 import logging
 import os
 from contextlib import suppress
 from functools import wraps
-from typing import TYPE_CHECKING, Any
+from typing import TYPE_CHECKING, Any, Iterable
 from urllib.parse import parse_qsl, urlencode, urlparse, urlunparse
 
 import attrs
 from attrs import asdict
 
 # TODO: move this maybe to Airflow's logic?
 from openlineage.client.utils import RedactMixin
@@ -410,7 +410,14 @@
     )
     return isinstance(source_var, str) and source_var.lower() not in ("true", "1", "t")
 
 
 def get_filtered_unknown_operator_keys(operator: BaseOperator) -> dict:
     not_required_keys = {"dag", "task_group"}
     return {attr: value for attr, value in operator.__dict__.items() if attr not in not_required_keys}
+
+
+def normalize_sql(sql: str | Iterable[str]):
+    if isinstance(sql, str):
+        sql = [stmt for stmt in sql.split(";") if stmt != ""]
+    sql = [obj for stmt in sql for obj in stmt.split(";") if obj != ""]
+    return ";\n".join(sql)
```

### Comparing `apache-airflow-providers-openlineage-1.0.0rc1/apache_airflow_providers_openlineage.egg-info/PKG-INFO` & `apache-airflow-providers-openlineage-1.0.1rc1/apache_airflow_providers_openlineage.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-openlineage
-Version: 1.0.0rc1
+Version: 1.0.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-openlineage package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-openlineage/1.0.0/
-Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-openlineage/1.0.0/changelog.html
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-openlineage/1.0.1/
+Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-openlineage/1.0.1/changelog.html
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
 
 
 Package ``apache-airflow-providers-openlineage``
 
-Release: ``1.0.0rc1``
+Release: ``1.0.1rc1``
 
 
 `OpenLineage <https://openlineage.io/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``openlineage`` provider. All classes for this provider package
 are in ``airflow.providers.openlineage`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-openlineage/1.0.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-openlineage/1.0.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -125,8 +125,8 @@
 ============================================================================================================  ==============
 Dependent package                                                                                             Extra
 ============================================================================================================  ==============
 `apache-airflow-providers-common-sql <https://airflow.apache.org/docs/apache-airflow-providers-common-sql>`_  ``common.sql``
 ============================================================================================================  ==============
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-openlineage/1.0.0/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-openlineage/1.0.1/changelog.html>`_.
```

### Comparing `apache-airflow-providers-openlineage-1.0.0rc1/apache_airflow_providers_openlineage.egg-info/SOURCES.txt` & `apache-airflow-providers-openlineage-1.0.1rc1/apache_airflow_providers_openlineage.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-openlineage-1.0.0rc1/pyproject.toml` & `apache-airflow-providers-openlineage-1.0.1rc1/pyproject.toml`

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

### Comparing `apache-airflow-providers-openlineage-1.0.0rc1/setup.cfg` & `apache-airflow-providers-openlineage-1.0.1rc1/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -23,16 +23,16 @@
 	License :: OSI Approved :: Apache Software License
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	Topic :: System :: Monitoring
 project_urls = 
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-openlineage/1.0.0/
-	Changelog=https://airflow.apache.org/docs/apache-airflow-providers-openlineage/1.0.0/changelog.html
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-openlineage/1.0.1/
+	Changelog=https://airflow.apache.org/docs/apache-airflow-providers-openlineage/1.0.1/changelog.html
 	Bug Tracker=https://github.com/apache/airflow/issues
 	Source Code=https://github.com/apache/airflow
 	Slack Chat=https://s.apache.org/airflow-slack
 	Twitter=https://twitter.com/ApacheAirflow
 	YouTube=https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 
 [bdist_wheel]
```

### Comparing `apache-airflow-providers-openlineage-1.0.0rc1/setup.py` & `apache-airflow-providers-openlineage-1.0.1rc1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-openlineage package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "1.0.0"
+version = "1.0.1"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-openlineage setup."""
     setup(
         version=version,
         extras_require={"common.sql": ["apache-airflow-providers-common-sql"]},
```

