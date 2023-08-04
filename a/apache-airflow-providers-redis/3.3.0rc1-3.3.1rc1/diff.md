# Comparing `tmp/apache-airflow-providers-redis-3.3.0rc1.tar.gz` & `tmp/apache-airflow-providers-redis-3.3.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-redis-3.3.0rc1.tar", last modified: Sat Jul 29 12:09:00 2023, max compression
+gzip compressed data, was "apache-airflow-providers-redis-3.3.1rc1.tar", last modified: Fri Aug  4 21:41:34 2023, max compression
```

## Comparing `apache-airflow-providers-redis-3.3.0rc1.tar` & `apache-airflow-providers-redis-3.3.1rc1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:09:00.031960 apache-airflow-providers-redis-3.3.0rc1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-redis-3.3.0rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-07-29 12:08:58.000000 apache-airflow-providers-redis-3.3.0rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-redis-3.3.0rc1/NOTICE
--rw-r--r--   0 root         (0) root         (0)     4384 2023-07-29 12:09:00.032626 apache-airflow-providers-redis-3.3.0rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2750 2023-07-29 12:08:58.000000 apache-airflow-providers-redis-3.3.0rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:59.929772 apache-airflow-providers-redis-3.3.0rc1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:59.931310 apache-airflow-providers-redis-3.3.0rc1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:59.971091 apache-airflow-providers-redis-3.3.0rc1/airflow/providers/redis/
--rw-r--r--   0 root         (0) root         (0)     1574 2023-07-29 12:01:19.000000 apache-airflow-providers-redis-3.3.0rc1/airflow/providers/redis/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2686 2023-07-29 12:08:58.000000 apache-airflow-providers-redis-3.3.0rc1/airflow/providers/redis/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:59.977186 apache-airflow-providers-redis-3.3.0rc1/airflow/providers/redis/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-redis-3.3.0rc1/airflow/providers/redis/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2945 2023-06-02 11:31:21.000000 apache-airflow-providers-redis-3.3.0rc1/airflow/providers/redis/hooks/redis.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:59.984895 apache-airflow-providers-redis-3.3.0rc1/airflow/providers/redis/log/
--rw-r--r--   0 root         (0) root         (0)      787 2023-07-26 06:59:50.000000 apache-airflow-providers-redis-3.3.0rc1/airflow/providers/redis/log/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3641 2023-07-26 06:59:50.000000 apache-airflow-providers-redis-3.3.0rc1/airflow/providers/redis/log/redis_task_handler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:08:59.991024 apache-airflow-providers-redis-3.3.0rc1/airflow/providers/redis/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-redis-3.3.0rc1/airflow/providers/redis/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2097 2023-06-02 11:31:21.000000 apache-airflow-providers-redis-3.3.0rc1/airflow/providers/redis/operators/redis_publish.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:09:00.001303 apache-airflow-providers-redis-3.3.0rc1/airflow/providers/redis/sensors/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-redis-3.3.0rc1/airflow/providers/redis/sensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1585 2023-06-02 11:31:21.000000 apache-airflow-providers-redis-3.3.0rc1/airflow/providers/redis/sensors/redis_key.py
--rw-r--r--   0 root         (0) root         (0)     2586 2023-06-02 11:31:21.000000 apache-airflow-providers-redis-3.3.0rc1/airflow/providers/redis/sensors/redis_pub_sub.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 12:09:00.028927 apache-airflow-providers-redis-3.3.0rc1/apache_airflow_providers_redis.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4384 2023-07-29 12:08:59.000000 apache-airflow-providers-redis-3.3.0rc1/apache_airflow_providers_redis.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      937 2023-07-29 12:08:59.000000 apache-airflow-providers-redis-3.3.0rc1/apache_airflow_providers_redis.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:08:59.000000 apache-airflow-providers-redis-3.3.0rc1/apache_airflow_providers_redis.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      102 2023-07-29 12:08:59.000000 apache-airflow-providers-redis-3.3.0rc1/apache_airflow_providers_redis.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 12:08:59.000000 apache-airflow-providers-redis-3.3.0rc1/apache_airflow_providers_redis.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       40 2023-07-29 12:08:59.000000 apache-airflow-providers-redis-3.3.0rc1/apache_airflow_providers_redis.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-07-29 12:08:59.000000 apache-airflow-providers-redis-3.3.0rc1/apache_airflow_providers_redis.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5011 2023-07-27 05:54:58.000000 apache-airflow-providers-redis-3.3.0rc1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1932 2023-07-29 12:09:00.034847 apache-airflow-providers-redis-3.3.0rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1632 2023-07-29 12:08:58.000000 apache-airflow-providers-redis-3.3.0rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:41:34.663300 apache-airflow-providers-redis-3.3.1rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-redis-3.3.1rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-08-04 21:41:33.000000 apache-airflow-providers-redis-3.3.1rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-redis-3.3.1rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     4384 2023-08-04 21:41:34.663931 apache-airflow-providers-redis-3.3.1rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2750 2023-08-04 21:41:33.000000 apache-airflow-providers-redis-3.3.1rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:41:34.570393 apache-airflow-providers-redis-3.3.1rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:41:34.571553 apache-airflow-providers-redis-3.3.1rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:41:34.607362 apache-airflow-providers-redis-3.3.1rc1/airflow/providers/redis/
+-rw-r--r--   0 root         (0) root         (0)     1574 2023-08-04 21:33:34.000000 apache-airflow-providers-redis-3.3.1rc1/airflow/providers/redis/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2707 2023-08-04 21:41:33.000000 apache-airflow-providers-redis-3.3.1rc1/airflow/providers/redis/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:41:34.612912 apache-airflow-providers-redis-3.3.1rc1/airflow/providers/redis/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-redis-3.3.1rc1/airflow/providers/redis/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2945 2023-06-02 11:31:21.000000 apache-airflow-providers-redis-3.3.1rc1/airflow/providers/redis/hooks/redis.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:41:34.618810 apache-airflow-providers-redis-3.3.1rc1/airflow/providers/redis/log/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-07-26 06:59:50.000000 apache-airflow-providers-redis-3.3.1rc1/airflow/providers/redis/log/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3641 2023-07-26 06:59:50.000000 apache-airflow-providers-redis-3.3.1rc1/airflow/providers/redis/log/redis_task_handler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:41:34.625314 apache-airflow-providers-redis-3.3.1rc1/airflow/providers/redis/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-redis-3.3.1rc1/airflow/providers/redis/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2097 2023-06-02 11:31:21.000000 apache-airflow-providers-redis-3.3.1rc1/airflow/providers/redis/operators/redis_publish.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:41:34.635533 apache-airflow-providers-redis-3.3.1rc1/airflow/providers/redis/sensors/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-redis-3.3.1rc1/airflow/providers/redis/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1585 2023-06-02 11:31:21.000000 apache-airflow-providers-redis-3.3.1rc1/airflow/providers/redis/sensors/redis_key.py
+-rw-r--r--   0 root         (0) root         (0)     2660 2023-08-04 10:24:22.000000 apache-airflow-providers-redis-3.3.1rc1/airflow/providers/redis/sensors/redis_pub_sub.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:41:34.660987 apache-airflow-providers-redis-3.3.1rc1/apache_airflow_providers_redis.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4384 2023-08-04 21:41:34.000000 apache-airflow-providers-redis-3.3.1rc1/apache_airflow_providers_redis.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      937 2023-08-04 21:41:34.000000 apache-airflow-providers-redis-3.3.1rc1/apache_airflow_providers_redis.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 21:41:34.000000 apache-airflow-providers-redis-3.3.1rc1/apache_airflow_providers_redis.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      102 2023-08-04 21:41:34.000000 apache-airflow-providers-redis-3.3.1rc1/apache_airflow_providers_redis.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 21:41:34.000000 apache-airflow-providers-redis-3.3.1rc1/apache_airflow_providers_redis.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       40 2023-08-04 21:41:34.000000 apache-airflow-providers-redis-3.3.1rc1/apache_airflow_providers_redis.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-08-04 21:41:34.000000 apache-airflow-providers-redis-3.3.1rc1/apache_airflow_providers_redis.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5031 2023-08-04 10:24:23.000000 apache-airflow-providers-redis-3.3.1rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1932 2023-08-04 21:41:34.666038 apache-airflow-providers-redis-3.3.1rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1632 2023-08-04 21:41:33.000000 apache-airflow-providers-redis-3.3.1rc1/setup.py
```

### Comparing `apache-airflow-providers-redis-3.3.0rc1/LICENSE` & `apache-airflow-providers-redis-3.3.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-redis-3.3.0rc1/MANIFEST.in` & `apache-airflow-providers-redis-3.3.1rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-redis-3.3.0rc1/PKG-INFO` & `apache-airflow-providers-redis-3.3.1rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-redis
-Version: 3.3.0rc1
+Version: 3.3.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-redis package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-redis/3.3.0/
-Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-redis/3.3.0/changelog.html
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-redis/3.3.1/
+Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-redis/3.3.1/changelog.html
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -66,28 +66,28 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-redis``
 
-Release: ``3.3.0rc1``
+Release: ``3.3.1rc1``
 
 
 `Redis <https://redis.io/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``redis`` provider. All classes for this provider package
 are in ``airflow.providers.redis`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-redis/3.3.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-redis/3.3.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -102,8 +102,8 @@
 PIP package         Version required
 ==================  ==================
 ``apache-airflow``  ``>=2.4.0``
 ``redis``           ``>=3.2.0``
 ==================  ==================
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-redis/3.3.0/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-redis/3.3.1/changelog.html>`_.
```

### Comparing `apache-airflow-providers-redis-3.3.0rc1/README.rst` & `apache-airflow-providers-redis-3.3.1rc1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -32,28 +32,28 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-redis``
 
-Release: ``3.3.0rc1``
+Release: ``3.3.1rc1``
 
 
 `Redis <https://redis.io/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``redis`` provider. All classes for this provider package
 are in ``airflow.providers.redis`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-redis/3.3.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-redis/3.3.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -68,8 +68,8 @@
 PIP package         Version required
 ==================  ==================
 ``apache-airflow``  ``>=2.4.0``
 ``redis``           ``>=3.2.0``
 ==================  ==================
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-redis/3.3.0/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-redis/3.3.1/changelog.html>`_.
```

### Comparing `apache-airflow-providers-redis-3.3.0rc1/airflow/providers/redis/__init__.py` & `apache-airflow-providers-redis-3.3.1rc1/airflow/providers/redis/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 from __future__ import annotations
 
 import packaging.version
 
 __all__ = ["__version__"]
 
-__version__ = "3.3.0"
+__version__ = "3.3.1"
 
 try:
     from airflow import __version__ as airflow_version
 except ImportError:
     from airflow.version import version as airflow_version
 
 if packaging.version.parse(packaging.version.parse(airflow_version).base_version) < packaging.version.parse(
```

### Comparing `apache-airflow-providers-redis-3.3.0rc1/airflow/providers/redis/get_provider_info.py` & `apache-airflow-providers-redis-3.3.1rc1/airflow/providers/redis/get_provider_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-redis",
         "name": "Redis",
         "description": "`Redis <https://redis.io/>`__\n",
         "suspended": False,
         "versions": [
+            "3.3.1",
             "3.3.0",
             "3.2.1",
             "3.2.0",
             "3.1.0",
             "3.0.0",
             "2.0.4",
             "2.0.3",
```

### Comparing `apache-airflow-providers-redis-3.3.0rc1/airflow/providers/redis/hooks/__init__.py` & `apache-airflow-providers-redis-3.3.1rc1/airflow/providers/redis/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-redis-3.3.0rc1/airflow/providers/redis/hooks/redis.py` & `apache-airflow-providers-redis-3.3.1rc1/airflow/providers/redis/hooks/redis.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-redis-3.3.0rc1/airflow/providers/redis/log/__init__.py` & `apache-airflow-providers-redis-3.3.1rc1/airflow/providers/redis/log/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-redis-3.3.0rc1/airflow/providers/redis/log/redis_task_handler.py` & `apache-airflow-providers-redis-3.3.1rc1/airflow/providers/redis/log/redis_task_handler.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-redis-3.3.0rc1/airflow/providers/redis/operators/__init__.py` & `apache-airflow-providers-redis-3.3.1rc1/airflow/providers/redis/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-redis-3.3.0rc1/airflow/providers/redis/operators/redis_publish.py` & `apache-airflow-providers-redis-3.3.1rc1/airflow/providers/redis/operators/redis_publish.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-redis-3.3.0rc1/airflow/providers/redis/sensors/__init__.py` & `apache-airflow-providers-redis-3.3.1rc1/airflow/providers/redis/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-redis-3.3.0rc1/airflow/providers/redis/sensors/redis_key.py` & `apache-airflow-providers-redis-3.3.1rc1/airflow/providers/redis/sensors/redis_key.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-redis-3.3.0rc1/airflow/providers/redis/sensors/redis_pub_sub.py` & `apache-airflow-providers-redis-3.3.1rc1/airflow/providers/redis/sensors/redis_pub_sub.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 from __future__ import annotations
 
+from functools import cached_property
 from typing import TYPE_CHECKING, Sequence
 
 from airflow.providers.redis.hooks.redis import RedisHook
 from airflow.sensors.base import BaseSensorOperator
 
 if TYPE_CHECKING:
     from airflow.utils.context import Context
@@ -37,28 +38,30 @@
     template_fields: Sequence[str] = ("channels",)
     ui_color = "#f0eee4"
 
     def __init__(self, *, channels: list[str] | str, redis_conn_id: str, **kwargs) -> None:
         super().__init__(**kwargs)
         self.channels = channels
         self.redis_conn_id = redis_conn_id
-        self.pubsub = RedisHook(redis_conn_id=self.redis_conn_id).get_conn().pubsub()
-        self.pubsub.subscribe(self.channels)
+
+    @cached_property
+    def pubsub(self):
+        return RedisHook(redis_conn_id=self.redis_conn_id).get_conn().pubsub()
 
     def poke(self, context: Context) -> bool:
         """
         Check for message on subscribed channels and write to xcom the message with key ``message``.
 
         An example of message ``{'type': 'message', 'pattern': None, 'channel': b'test', 'data': b'hello'}``
 
         :param context: the context object
         :return: ``True`` if message (with type 'message') is available or ``False`` if not
         """
         self.log.info("RedisPubSubSensor checking for message on channels: %s", self.channels)
-
+        self.pubsub.subscribe(self.channels)
         message = self.pubsub.get_message()
         self.log.info("Message %s from channel %s", message, self.channels)
 
         # Process only message types
         if message and message["type"] == "message":
 
             context["ti"].xcom_push(key="message", value=message)
```

### Comparing `apache-airflow-providers-redis-3.3.0rc1/apache_airflow_providers_redis.egg-info/PKG-INFO` & `apache-airflow-providers-redis-3.3.1rc1/apache_airflow_providers_redis.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-redis
-Version: 3.3.0rc1
+Version: 3.3.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-redis package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-redis/3.3.0/
-Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-redis/3.3.0/changelog.html
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-redis/3.3.1/
+Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-redis/3.3.1/changelog.html
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -66,28 +66,28 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-redis``
 
-Release: ``3.3.0rc1``
+Release: ``3.3.1rc1``
 
 
 `Redis <https://redis.io/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``redis`` provider. All classes for this provider package
 are in ``airflow.providers.redis`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-redis/3.3.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-redis/3.3.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
@@ -102,8 +102,8 @@
 PIP package         Version required
 ==================  ==================
 ``apache-airflow``  ``>=2.4.0``
 ``redis``           ``>=3.2.0``
 ==================  ==================
 
 The changelog for the provider package can be found in the
-`changelog <https://airflow.apache.org/docs/apache-airflow-providers-redis/3.3.0/changelog.html>`_.
+`changelog <https://airflow.apache.org/docs/apache-airflow-providers-redis/3.3.1/changelog.html>`_.
```

### Comparing `apache-airflow-providers-redis-3.3.0rc1/apache_airflow_providers_redis.egg-info/SOURCES.txt` & `apache-airflow-providers-redis-3.3.1rc1/apache_airflow_providers_redis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-redis-3.3.0rc1/pyproject.toml` & `apache-airflow-providers-redis-3.3.1rc1/pyproject.toml`

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

### Comparing `apache-airflow-providers-redis-3.3.0rc1/setup.cfg` & `apache-airflow-providers-redis-3.3.1rc1/setup.cfg`

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
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-redis/3.3.0/
-	Changelog=https://airflow.apache.org/docs/apache-airflow-providers-redis/3.3.0/changelog.html
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-redis/3.3.1/
+	Changelog=https://airflow.apache.org/docs/apache-airflow-providers-redis/3.3.1/changelog.html
 	Bug Tracker=https://github.com/apache/airflow/issues
 	Source Code=https://github.com/apache/airflow
 	Slack Chat=https://s.apache.org/airflow-slack
 	Twitter=https://twitter.com/ApacheAirflow
 	YouTube=https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 
 [bdist_wheel]
```

### Comparing `apache-airflow-providers-redis-3.3.0rc1/setup.py` & `apache-airflow-providers-redis-3.3.1rc1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-redis package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "3.3.0"
+version = "3.3.1"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-redis setup."""
     setup(
         version=version,
         extras_require={},
```

