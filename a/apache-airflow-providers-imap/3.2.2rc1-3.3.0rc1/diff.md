# Comparing `tmp/apache-airflow-providers-imap-3.2.2rc1.tar.gz` & `tmp/apache-airflow-providers-imap-3.3.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-imap-3.2.2rc1.tar", last modified: Tue Jun 20 11:42:20 2023, max compression
+gzip compressed data, was "apache-airflow-providers-imap-3.3.0rc1.tar", last modified: Fri Aug  4 21:41:17 2023, max compression
```

## Comparing `apache-airflow-providers-imap-3.2.2rc1.tar` & `apache-airflow-providers-imap-3.3.0rc1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:20.226959 apache-airflow-providers-imap-3.2.2rc1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-imap-3.2.2rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:42:19.000000 apache-airflow-providers-imap-3.2.2rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-imap-3.2.2rc1/NOTICE
--rw-r--r--   0 root         (0) root         (0)    10402 2023-06-20 11:42:20.228169 apache-airflow-providers-imap-3.2.2rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8880 2023-06-20 11:42:19.000000 apache-airflow-providers-imap-3.2.2rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:20.147596 apache-airflow-providers-imap-3.2.2rc1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:20.148910 apache-airflow-providers-imap-3.2.2rc1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:20.187214 apache-airflow-providers-imap-3.2.2rc1/airflow/providers/imap/
--rw-r--r--   0 root         (0) root         (0)     1529 2023-06-20 11:01:09.000000 apache-airflow-providers-imap-3.2.2rc1/airflow/providers/imap/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2618 2023-06-20 11:42:19.000000 apache-airflow-providers-imap-3.2.2rc1/airflow/providers/imap/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:20.193153 apache-airflow-providers-imap-3.2.2rc1/airflow/providers/imap/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-imap-3.2.2rc1/airflow/providers/imap/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14090 2023-06-01 06:14:28.000000 apache-airflow-providers-imap-3.2.2rc1/airflow/providers/imap/hooks/imap.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:20.198967 apache-airflow-providers-imap-3.2.2rc1/airflow/providers/imap/sensors/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-imap-3.2.2rc1/airflow/providers/imap/sensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3054 2023-06-01 06:14:28.000000 apache-airflow-providers-imap-3.2.2rc1/airflow/providers/imap/sensors/imap_attachment.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:20.223903 apache-airflow-providers-imap-3.2.2rc1/apache_airflow_providers_imap.egg-info/
--rw-r--r--   0 root         (0) root         (0)    10402 2023-06-20 11:42:20.000000 apache-airflow-providers-imap-3.2.2rc1/apache_airflow_providers_imap.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      693 2023-06-20 11:42:20.000000 apache-airflow-providers-imap-3.2.2rc1/apache_airflow_providers_imap.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:42:20.000000 apache-airflow-providers-imap-3.2.2rc1/apache_airflow_providers_imap.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      101 2023-06-20 11:42:20.000000 apache-airflow-providers-imap-3.2.2rc1/apache_airflow_providers_imap.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:42:20.000000 apache-airflow-providers-imap-3.2.2rc1/apache_airflow_providers_imap.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       27 2023-06-20 11:42:20.000000 apache-airflow-providers-imap-3.2.2rc1/apache_airflow_providers_imap.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:42:20.000000 apache-airflow-providers-imap-3.2.2rc1/apache_airflow_providers_imap.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-imap-3.2.2rc1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1817 2023-06-20 11:42:20.230574 apache-airflow-providers-imap-3.2.2rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1626 2023-06-20 11:42:19.000000 apache-airflow-providers-imap-3.2.2rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:41:17.873464 apache-airflow-providers-imap-3.3.0rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-imap-3.3.0rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-08-04 21:41:16.000000 apache-airflow-providers-imap-3.3.0rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-imap-3.3.0rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     4394 2023-08-04 21:41:17.874018 apache-airflow-providers-imap-3.3.0rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2764 2023-08-04 21:41:16.000000 apache-airflow-providers-imap-3.3.0rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:41:17.802392 apache-airflow-providers-imap-3.3.0rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:41:17.803547 apache-airflow-providers-imap-3.3.0rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:41:17.835532 apache-airflow-providers-imap-3.3.0rc1/airflow/providers/imap/
+-rw-r--r--   0 root         (0) root         (0)     1573 2023-08-04 21:33:34.000000 apache-airflow-providers-imap-3.3.0rc1/airflow/providers/imap/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4200 2023-08-04 21:41:16.000000 apache-airflow-providers-imap-3.3.0rc1/airflow/providers/imap/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:41:17.841344 apache-airflow-providers-imap-3.3.0rc1/airflow/providers/imap/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-imap-3.3.0rc1/airflow/providers/imap/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15241 2023-08-04 19:44:14.000000 apache-airflow-providers-imap-3.3.0rc1/airflow/providers/imap/hooks/imap.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:41:17.847041 apache-airflow-providers-imap-3.3.0rc1/airflow/providers/imap/sensors/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-imap-3.3.0rc1/airflow/providers/imap/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3054 2023-06-01 06:14:28.000000 apache-airflow-providers-imap-3.3.0rc1/airflow/providers/imap/sensors/imap_attachment.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:41:17.871279 apache-airflow-providers-imap-3.3.0rc1/apache_airflow_providers_imap.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4394 2023-08-04 21:41:17.000000 apache-airflow-providers-imap-3.3.0rc1/apache_airflow_providers_imap.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      693 2023-08-04 21:41:17.000000 apache-airflow-providers-imap-3.3.0rc1/apache_airflow_providers_imap.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 21:41:17.000000 apache-airflow-providers-imap-3.3.0rc1/apache_airflow_providers_imap.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      101 2023-08-04 21:41:17.000000 apache-airflow-providers-imap-3.3.0rc1/apache_airflow_providers_imap.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 21:41:17.000000 apache-airflow-providers-imap-3.3.0rc1/apache_airflow_providers_imap.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       27 2023-08-04 21:41:17.000000 apache-airflow-providers-imap-3.3.0rc1/apache_airflow_providers_imap.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-08-04 21:41:17.000000 apache-airflow-providers-imap-3.3.0rc1/apache_airflow_providers_imap.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5031 2023-08-04 10:24:23.000000 apache-airflow-providers-imap-3.3.0rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1911 2023-08-04 21:41:17.875895 apache-airflow-providers-imap-3.3.0rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1626 2023-08-04 21:41:16.000000 apache-airflow-providers-imap-3.3.0rc1/setup.py
```

### Comparing `apache-airflow-providers-imap-3.2.2rc1/LICENSE` & `apache-airflow-providers-imap-3.3.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-imap-3.2.2rc1/MANIFEST.in` & `apache-airflow-providers-imap-3.3.0rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-imap-3.2.2rc1/airflow/providers/imap/__init__.py` & `apache-airflow-providers-imap-3.3.0rc1/airflow/providers/imap/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,18 +24,20 @@
 #
 from __future__ import annotations
 
 import packaging.version
 
 __all__ = ["__version__"]
 
-__version__ = "3.2.2"
+__version__ = "3.3.0"
 
 try:
     from airflow import __version__ as airflow_version
 except ImportError:
     from airflow.version import version as airflow_version
 
-if packaging.version.parse(airflow_version) < packaging.version.parse("2.4.0"):
+if packaging.version.parse(packaging.version.parse(airflow_version).base_version) < packaging.version.parse(
+    "2.4.0"
+):
     raise RuntimeError(
         f"The package `apache-airflow-providers-imap:{__version__}` requires Apache Airflow 2.4.0+"  # NOQA: E501
     )
```

### Comparing `apache-airflow-providers-imap-3.2.2rc1/airflow/providers/imap/hooks/__init__.py` & `apache-airflow-providers-imap-3.3.0rc1/airflow/providers/imap/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-imap-3.2.2rc1/airflow/providers/imap/hooks/imap.py` & `apache-airflow-providers-imap-3.3.0rc1/airflow/providers/imap/hooks/imap.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,24 +12,25 @@
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 """
-This module provides everything to be able to search in mails for a specific attachment
-and also to download it.
+This module provides everything to search mail for a specific attachment and download it.
+
 It uses the imaplib library that is already integrated in python 3.
 """
 from __future__ import annotations
 
 import email
 import imaplib
 import os
 import re
+import ssl
 from typing import Any, Iterable
 
 from airflow.exceptions import AirflowException
 from airflow.hooks.base import BaseHook
 from airflow.models.connection import Connection
 from airflow.utils.log.logging_mixin import LoggingMixin
 
@@ -74,24 +75,46 @@
             conn = self.get_connection(self.imap_conn_id)
             self.mail_client = self._build_client(conn)
             self.mail_client.login(conn.login, conn.password)
 
         return self
 
     def _build_client(self, conn: Connection) -> imaplib.IMAP4_SSL | imaplib.IMAP4:
-        IMAP: type[imaplib.IMAP4_SSL] | type[imaplib.IMAP4]
-        if conn.extra_dejson.get("use_ssl", True):
-            IMAP = imaplib.IMAP4_SSL
-        else:
-            IMAP = imaplib.IMAP4
-
-        if conn.port:
-            mail_client = IMAP(conn.host, conn.port)
+        mail_client: imaplib.IMAP4_SSL | imaplib.IMAP4
+        use_ssl = conn.extra_dejson.get("use_ssl", True)
+        if use_ssl:
+            from airflow.configuration import conf
+
+            extra_ssl_context = conn.extra_dejson.get("ssl_context", None)
+            if extra_ssl_context:
+                ssl_context_string = extra_ssl_context
+            else:
+                ssl_context_string = conf.get("imap", "SSL_CONTEXT", fallback=None)
+            if ssl_context_string is None:
+                ssl_context_string = conf.get("email", "SSL_CONTEXT", fallback=None)
+            if ssl_context_string is None:
+                ssl_context_string = "default"
+            if ssl_context_string == "default":
+                ssl_context = ssl.create_default_context()
+            elif ssl_context_string == "none":
+                ssl_context = None
+            else:
+                raise RuntimeError(
+                    f"The email.ssl_context configuration variable must "
+                    f"be set to 'default' or 'none' and is '{ssl_context_string}'."
+                )
+            if conn.port:
+                mail_client = imaplib.IMAP4_SSL(conn.host, conn.port, ssl_context=ssl_context)
+            else:
+                mail_client = imaplib.IMAP4_SSL(conn.host, ssl_context=ssl_context)
         else:
-            mail_client = IMAP(conn.host)
+            if conn.port:
+                mail_client = imaplib.IMAP4(conn.host, conn.port)
+            else:
+                mail_client = imaplib.IMAP4(conn.host)
 
         return mail_client
 
     def has_mail_attachment(
         self, name: str, *, check_regex: bool = False, mail_folder: str = "INBOX", mail_filter: str = "All"
     ) -> bool:
         """
```

### Comparing `apache-airflow-providers-imap-3.2.2rc1/airflow/providers/imap/sensors/__init__.py` & `apache-airflow-providers-imap-3.3.0rc1/airflow/providers/imap/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-imap-3.2.2rc1/airflow/providers/imap/sensors/imap_attachment.py` & `apache-airflow-providers-imap-3.3.0rc1/airflow/providers/imap/sensors/imap_attachment.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-imap-3.2.2rc1/apache_airflow_providers_imap.egg-info/SOURCES.txt` & `apache-airflow-providers-imap-3.3.0rc1/apache_airflow_providers_imap.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-imap-3.2.2rc1/pyproject.toml` & `apache-airflow-providers-imap-3.3.0rc1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -13,19 +13,21 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 [tool.black]
 line-length = 110
 target-version = ['py37', 'py38', 'py39', 'py310']
-# The build system section is needed in order to workaround the side-effect introduced by recent
-# setup tools version. The recent setuptools version update (64.0.0) broke paths of editable installations
-# and we have to pin it to 63.4.3 version
-# The problem is tracked (and this limitation might be removed if it is solved) in:
-# https://github.com/pypa/setuptools/issues/3548
+
+# Editable installs are currently broken using setuptools 64.0.0 and above. The problem is tracked in
+# https://github.com/pypa/setuptools/issues/3548. We're also discussing how we could potentially fix
+# this problem on our end in issue https://github.com/apache/airflow/issues/30764. Until then we need
+# to use one of the following workarounds locally for editable installs:
+# 1) Pin setuptools <= 63.4.3 below in the [build-system] section.
+# 2) Include your airflow source code directory in PYTHONPATH.
 [build-system]
 requires = ['setuptools==67.2.0']
 build-backend = "setuptools.build_meta"
 
 [project]
 requires-python = ">=3.8"
 
@@ -35,15 +37,16 @@
 extend-exclude = [
     ".eggs",
     "airflow/_vendor/*",
     "airflow/providers/google/ads/_vendor/*",
     # The files generated by stubgen aren't 100% valid syntax it turns out, and we don't ship them, so we can
     # ignore them in ruff
     "airflow/providers/common/sql/*/*.pyi",
-    "airflow/migrations/versions/*.py"
+    "airflow/migrations/versions/*.py",
+    "tests/dags/test_imports.py",
 ]
 
 extend-select = [
     "I", # Missing required import (auto-fixable)
     "UP", # Pyupgrade
     "RUF100", # Unused noqa (auto-fixable)
 
@@ -67,14 +70,16 @@
     "D212",
     "D213",
     "D214",
     "D215",
     "E731",
 ]
 
+namespace-packages = ["airflow/providers"]
+
 [tool.pytest.ini_options]
 # * Disable `flaky` plugin for pytest. This plugin conflicts with `rerunfailures` because provide same marker.
 # * Disable `nose` builtin plugin for pytest. This feature deprecated in 7.2 and will be removed in pytest>=8
 # * And we focus on use native pytest capabilities rather than adopt another frameworks.
 addopts = "-rasl --verbosity=2 -p no:flaky -p no:nose --asyncio-mode=strict"
 norecursedirs = [
     ".eggs",
@@ -93,54 +98,29 @@
     "ignore::DeprecationWarning:flask_appbuilder.widgets",
     # https://github.com/dpgaspar/Flask-AppBuilder/pull/1940
     "ignore::DeprecationWarning:flask_sqlalchemy",
     # https://github.com/dpgaspar/Flask-AppBuilder/pull/1903
     "ignore::DeprecationWarning:apispec.utils",
 ]
 python_files = [
-    "*.py",
+    "test_*.py",
+    "example_*.py",
 ]
 testpaths = [
     "tests",
 ]
 
 [tool.ruff.isort]
-known-first-party = ["airflow", "airflow_breeze", "docker_tests", "docs", "kubernetes_tests", "tests"]
 required-imports = ["from __future__ import annotations"]
 combine-as-imports = true
 
-# TODO: for now, https://github.com/charliermarsh/ruff/issues/1817
-known-third-party = [
-    "asana",
-    "atlassian",
-    "celery",
-    "cloudant",
-    "databricks",
-    "datadog",
-    "docker",
-    "elasticsearch",
-    "github",
-    "google",
-    "grpc",
-    "jenkins",
-    "mysql",
-    "neo4j",
-    "papermill",
-    "redis",
-    "sendgrid",
-    "snowflake",
-    "telegram",
-    "trino",
-]
-
 [tool.ruff.per-file-ignores]
 "airflow/models/__init__.py" = ["F401"]
 "airflow/models/sqla_models.py" = ["F401"]
 
-
 # The test_python.py is needed because adding __future__.annotations breaks runtime checks that are
 # needed for the test to work
 "tests/decorators/test_python.py" = ["I002"]
 
 # The Pydantic representations of SqlAlchemy Models are not parsed well with Pydantic
 # when __future__.annotations is used so we need to skip them from upgrading
 "airflow/serialization/pydantic/*.py" = ["I002"]
```

### Comparing `apache-airflow-providers-imap-3.2.2rc1/setup.cfg` & `apache-airflow-providers-imap-3.3.0rc1/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -23,15 +23,16 @@
 	License :: OSI Approved :: Apache Software License
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	Topic :: System :: Monitoring
 project_urls = 
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-imap/3.2.2/
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-imap/3.3.0/
+	Changelog=https://airflow.apache.org/docs/apache-airflow-providers-imap/3.3.0/changelog.html
 	Bug Tracker=https://github.com/apache/airflow/issues
 	Source Code=https://github.com/apache/airflow
 	Slack Chat=https://s.apache.org/airflow-slack
 	Twitter=https://twitter.com/ApacheAirflow
 	YouTube=https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 
 [bdist_wheel]
```

### Comparing `apache-airflow-providers-imap-3.2.2rc1/setup.py` & `apache-airflow-providers-imap-3.3.0rc1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-imap package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "3.2.2"
+version = "3.3.0"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-imap setup."""
     setup(
         version=version,
         extras_require={},
```

