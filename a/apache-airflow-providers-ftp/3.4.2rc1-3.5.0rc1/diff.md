# Comparing `tmp/apache-airflow-providers-ftp-3.4.2rc1.tar.gz` & `tmp/apache-airflow-providers-ftp-3.5.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-ftp-3.4.2rc1.tar", last modified: Tue Jun 20 11:42:03 2023, max compression
+gzip compressed data, was "apache-airflow-providers-ftp-3.5.0rc1.tar", last modified: Fri Aug  4 21:41:06 2023, max compression
```

## Comparing `apache-airflow-providers-ftp-3.4.2rc1.tar` & `apache-airflow-providers-ftp-3.5.0rc1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:03.623457 apache-airflow-providers-ftp-3.4.2rc1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-ftp-3.4.2rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:42:02.000000 apache-airflow-providers-ftp-3.4.2rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-ftp-3.4.2rc1/NOTICE
--rw-r--r--   0 root         (0) root         (0)    10296 2023-06-20 11:42:03.624667 apache-airflow-providers-ftp-3.4.2rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8777 2023-06-20 11:42:02.000000 apache-airflow-providers-ftp-3.4.2rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:03.540377 apache-airflow-providers-ftp-3.4.2rc1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:03.541702 apache-airflow-providers-ftp-3.4.2rc1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:03.577906 apache-airflow-providers-ftp-3.4.2rc1/airflow/providers/ftp/
--rw-r--r--   0 root         (0) root         (0)     1528 2023-06-20 11:01:09.000000 apache-airflow-providers-ftp-3.4.2rc1/airflow/providers/ftp/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2765 2023-06-20 11:42:02.000000 apache-airflow-providers-ftp-3.4.2rc1/airflow/providers/ftp/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:03.583570 apache-airflow-providers-ftp-3.4.2rc1/airflow/providers/ftp/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-ftp-3.4.2rc1/airflow/providers/ftp/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9846 2023-06-02 11:31:21.000000 apache-airflow-providers-ftp-3.4.2rc1/airflow/providers/ftp/hooks/ftp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:03.589324 apache-airflow-providers-ftp-3.4.2rc1/airflow/providers/ftp/operators/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-ftp-3.4.2rc1/airflow/providers/ftp/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6079 2023-06-02 11:31:21.000000 apache-airflow-providers-ftp-3.4.2rc1/airflow/providers/ftp/operators/ftp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:03.595048 apache-airflow-providers-ftp-3.4.2rc1/airflow/providers/ftp/sensors/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-ftp-3.4.2rc1/airflow/providers/ftp/sensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3364 2023-06-02 11:31:21.000000 apache-airflow-providers-ftp-3.4.2rc1/airflow/providers/ftp/sensors/ftp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:03.620290 apache-airflow-providers-ftp-3.4.2rc1/apache_airflow_providers_ftp.egg-info/
--rw-r--r--   0 root         (0) root         (0)    10296 2023-06-20 11:42:03.000000 apache-airflow-providers-ftp-3.4.2rc1/apache_airflow_providers_ftp.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      750 2023-06-20 11:42:03.000000 apache-airflow-providers-ftp-3.4.2rc1/apache_airflow_providers_ftp.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:42:03.000000 apache-airflow-providers-ftp-3.4.2rc1/apache_airflow_providers_ftp.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      100 2023-06-20 11:42:03.000000 apache-airflow-providers-ftp-3.4.2rc1/apache_airflow_providers_ftp.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:42:03.000000 apache-airflow-providers-ftp-3.4.2rc1/apache_airflow_providers_ftp.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       27 2023-06-20 11:42:03.000000 apache-airflow-providers-ftp-3.4.2rc1/apache_airflow_providers_ftp.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:42:03.000000 apache-airflow-providers-ftp-3.4.2rc1/apache_airflow_providers_ftp.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-ftp-3.4.2rc1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1811 2023-06-20 11:42:03.626640 apache-airflow-providers-ftp-3.4.2rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1620 2023-06-20 11:42:02.000000 apache-airflow-providers-ftp-3.4.2rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:41:06.801802 apache-airflow-providers-ftp-3.5.0rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-ftp-3.5.0rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-08-04 21:41:05.000000 apache-airflow-providers-ftp-3.5.0rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-ftp-3.5.0rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     5444 2023-08-04 21:41:06.802375 apache-airflow-providers-ftp-3.5.0rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3790 2023-08-04 21:41:05.000000 apache-airflow-providers-ftp-3.5.0rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:41:06.724097 apache-airflow-providers-ftp-3.5.0rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:41:06.725152 apache-airflow-providers-ftp-3.5.0rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:41:06.759046 apache-airflow-providers-ftp-3.5.0rc1/airflow/providers/ftp/
+-rw-r--r--   0 root         (0) root         (0)     1572 2023-08-04 21:33:34.000000 apache-airflow-providers-ftp-3.5.0rc1/airflow/providers/ftp/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2786 2023-08-04 21:41:05.000000 apache-airflow-providers-ftp-3.5.0rc1/airflow/providers/ftp/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:41:06.764593 apache-airflow-providers-ftp-3.5.0rc1/airflow/providers/ftp/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-ftp-3.5.0rc1/airflow/providers/ftp/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9788 2023-06-29 05:49:30.000000 apache-airflow-providers-ftp-3.5.0rc1/airflow/providers/ftp/hooks/ftp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:41:06.770158 apache-airflow-providers-ftp-3.5.0rc1/airflow/providers/ftp/operators/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-ftp-3.5.0rc1/airflow/providers/ftp/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8151 2023-08-04 10:24:22.000000 apache-airflow-providers-ftp-3.5.0rc1/airflow/providers/ftp/operators/ftp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:41:06.775764 apache-airflow-providers-ftp-3.5.0rc1/airflow/providers/ftp/sensors/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-ftp-3.5.0rc1/airflow/providers/ftp/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3364 2023-06-02 11:31:21.000000 apache-airflow-providers-ftp-3.5.0rc1/airflow/providers/ftp/sensors/ftp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:41:06.799308 apache-airflow-providers-ftp-3.5.0rc1/apache_airflow_providers_ftp.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5444 2023-08-04 21:41:06.000000 apache-airflow-providers-ftp-3.5.0rc1/apache_airflow_providers_ftp.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      750 2023-08-04 21:41:06.000000 apache-airflow-providers-ftp-3.5.0rc1/apache_airflow_providers_ftp.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 21:41:06.000000 apache-airflow-providers-ftp-3.5.0rc1/apache_airflow_providers_ftp.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      100 2023-08-04 21:41:06.000000 apache-airflow-providers-ftp-3.5.0rc1/apache_airflow_providers_ftp.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 21:41:06.000000 apache-airflow-providers-ftp-3.5.0rc1/apache_airflow_providers_ftp.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       79 2023-08-04 21:41:06.000000 apache-airflow-providers-ftp-3.5.0rc1/apache_airflow_providers_ftp.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-08-04 21:41:06.000000 apache-airflow-providers-ftp-3.5.0rc1/apache_airflow_providers_ftp.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5031 2023-08-04 10:24:23.000000 apache-airflow-providers-ftp-3.5.0rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1904 2023-08-04 21:41:06.804284 apache-airflow-providers-ftp-3.5.0rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1675 2023-08-04 21:41:05.000000 apache-airflow-providers-ftp-3.5.0rc1/setup.py
```

### Comparing `apache-airflow-providers-ftp-3.4.2rc1/LICENSE` & `apache-airflow-providers-ftp-3.5.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-ftp-3.4.2rc1/MANIFEST.in` & `apache-airflow-providers-ftp-3.5.0rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-ftp-3.4.2rc1/airflow/providers/ftp/__init__.py` & `apache-airflow-providers-ftp-3.5.0rc1/airflow/providers/ftp/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,18 +24,20 @@
 #
 from __future__ import annotations
 
 import packaging.version
 
 __all__ = ["__version__"]
 
-__version__ = "3.4.2"
+__version__ = "3.5.0"
 
 try:
     from airflow import __version__ as airflow_version
 except ImportError:
     from airflow.version import version as airflow_version
 
-if packaging.version.parse(airflow_version) < packaging.version.parse("2.4.0"):
+if packaging.version.parse(packaging.version.parse(airflow_version).base_version) < packaging.version.parse(
+    "2.4.0"
+):
     raise RuntimeError(
         f"The package `apache-airflow-providers-ftp:{__version__}` requires Apache Airflow 2.4.0+"  # NOQA: E501
     )
```

### Comparing `apache-airflow-providers-ftp-3.4.2rc1/airflow/providers/ftp/get_provider_info.py` & `apache-airflow-providers-ftp-3.5.0rc1/airflow/providers/ftp/get_provider_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-ftp",
         "name": "File Transfer Protocol (FTP)",
         "description": "`File Transfer Protocol (FTP) <https://tools.ietf.org/html/rfc114>`__\n",
         "suspended": False,
         "versions": [
+            "3.5.0",
             "3.4.2",
             "3.4.1",
             "3.4.0",
             "3.3.1",
             "3.3.0",
             "3.2.0",
             "3.1.0",
```

### Comparing `apache-airflow-providers-ftp-3.4.2rc1/airflow/providers/ftp/hooks/__init__.py` & `apache-airflow-providers-ftp-3.5.0rc1/airflow/providers/ftp/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-ftp-3.4.2rc1/airflow/providers/ftp/hooks/ftp.py` & `apache-airflow-providers-ftp-3.5.0rc1/airflow/providers/ftp/hooks/ftp.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,26 +61,22 @@
             pasv = params.extra_dejson.get("passive", True)
             self.conn = ftplib.FTP(params.host, params.login, params.password)
             self.conn.set_pasv(pasv)
 
         return self.conn
 
     def close_conn(self):
-        """
-        Closes the connection. An error will occur if the
-        connection was not ever opened.
-        """
+        """Closes the connection; an error will occur if the connection was never opened."""
         conn = self.conn
         conn.quit()
         self.conn = None
 
     def describe_directory(self, path: str) -> dict:
         """
-        Returns a dictionary of {filename: {attributes}} for all files
-        on the remote system (where the MLSD command is supported).
+        Return a dictionary of {filename: {attributes}} for all files on a remote system which supports MLSD.
 
         :param path: full path to the remote directory
         """
         conn = self.get_conn()
         conn.cwd(path)
         files = dict(conn.mlsd())
         return files
```

### Comparing `apache-airflow-providers-ftp-3.4.2rc1/airflow/providers/ftp/operators/__init__.py` & `apache-airflow-providers-ftp-3.5.0rc1/airflow/providers/ftp/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-ftp-3.4.2rc1/airflow/providers/ftp/operators/ftp.py` & `apache-airflow-providers-ftp-3.5.0rc1/airflow/providers/ftp/operators/ftp.py`

 * *Files 22% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 """This module contains FTP operator."""
 from __future__ import annotations
 
 import os
+import socket
+from ftplib import FTP_PORT
 from functools import cached_property
 from pathlib import Path
 from typing import Any, Sequence
 
 from airflow.models import BaseOperator
 from airflow.providers.ftp.hooks.ftp import FTPHook, FTPSHook
 
@@ -33,16 +35,16 @@
     PUT = "put"
     GET = "get"
 
 
 class FTPFileTransmitOperator(BaseOperator):
     """
     FTPFileTransmitOperator for transferring files from remote host to local or vice a versa.
-    This operator uses an FTPHook to open ftp transport channel that serve as basis
-    for file transfer.
+
+    This operator uses an FTPHook to open ftp transport channel that serve as basis for file transfer.
 
     .. seealso::
         For more information on how to use this operator, take a look at the guide:
         :ref:`howto/operator:FTPFileTransmitOperator`
 
     :param ftp_conn_id: :ref:`ftp connection id<howto/connection:ftp>`
         from airflow Connections.
@@ -131,20 +133,80 @@
                     self.hook.create_directory(remote_folder)
                 file_msg = f"from {_local_filepath} to {_remote_filepath}"
                 self.log.info("Starting to transfer file %s", file_msg)
                 self.hook.store_file(_remote_filepath, _local_filepath)
 
         return self.local_filepath
 
+    def get_openlineage_facets_on_start(self):
+        """
+        Returns OpenLineage datasets with following naming structure:
+                input: file://hostname/path
+                output file://<conn.host>:<conn.port>/path.
+        """
+        from openlineage.client.run import Dataset
+
+        from airflow.providers.openlineage.extractors import OperatorLineage
+
+        scheme = "file"
+
+        local_host = socket.gethostname()
+        try:
+            local_host = socket.gethostbyname(local_host)
+        except Exception as e:
+            self.log.warning(
+                f"Failed to resolve local hostname. Using the hostname got by socket.gethostbyname() without resolution. {e}",  # noqa: E501
+                exc_info=True,
+            )
+
+        conn = self.hook.get_conn()
+        remote_host = conn.host
+        remote_port = conn.port
+
+        if isinstance(self.local_filepath, str):
+            local_filepath = [self.local_filepath]
+        else:
+            local_filepath = self.local_filepath
+        if isinstance(self.remote_filepath, str):
+            remote_filepath = [self.remote_filepath]
+        else:
+            remote_filepath = self.remote_filepath
+
+        local_datasets = [
+            Dataset(namespace=self._get_namespace(scheme, local_host, None, path), name=path)
+            for path in local_filepath
+        ]
+        remote_datasets = [
+            Dataset(namespace=self._get_namespace(scheme, remote_host, remote_port, path), name=path)
+            for path in remote_filepath
+        ]
+
+        if self.operation.lower() == FTPOperation.GET:
+            inputs = remote_datasets
+            outputs = local_datasets
+        else:
+            inputs = local_datasets
+            outputs = remote_datasets
+
+        return OperatorLineage(
+            inputs=inputs,
+            outputs=outputs,
+        )
+
+    def _get_namespace(self, scheme, host, port, path) -> str:
+        port = port or FTP_PORT
+        authority = f"{host}:{port}"
+        return f"{scheme}://{authority}"
+
 
 class FTPSFileTransmitOperator(FTPFileTransmitOperator):
     """
     FTPSFileTransmitOperator for transferring files from remote host to local or vice a versa.
-    This operator uses an FTPSHook to open ftps transport channel that serve as basis
-    for file transfer.
+
+    This operator uses an FTPSHook to open ftps transport channel that serve as basis for file transfer.
 
     .. seealso::
         For more information on how to use this operator, take a look at the guide:
         :ref:`howto/operator:FTPSFileTransmitOperator`
     """
 
     @cached_property
```

### Comparing `apache-airflow-providers-ftp-3.4.2rc1/airflow/providers/ftp/sensors/__init__.py` & `apache-airflow-providers-ftp-3.5.0rc1/airflow/providers/ftp/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-ftp-3.4.2rc1/airflow/providers/ftp/sensors/ftp.py` & `apache-airflow-providers-ftp-3.5.0rc1/airflow/providers/ftp/sensors/ftp.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-ftp-3.4.2rc1/apache_airflow_providers_ftp.egg-info/SOURCES.txt` & `apache-airflow-providers-ftp-3.5.0rc1/apache_airflow_providers_ftp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-ftp-3.4.2rc1/pyproject.toml` & `apache-airflow-providers-ftp-3.5.0rc1/pyproject.toml`

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

### Comparing `apache-airflow-providers-ftp-3.4.2rc1/setup.cfg` & `apache-airflow-providers-ftp-3.5.0rc1/setup.cfg`

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
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-ftp/3.4.2/
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-ftp/3.5.0/
+	Changelog=https://airflow.apache.org/docs/apache-airflow-providers-ftp/3.5.0/changelog.html
 	Bug Tracker=https://github.com/apache/airflow/issues
 	Source Code=https://github.com/apache/airflow
 	Slack Chat=https://s.apache.org/airflow-slack
 	Twitter=https://twitter.com/ApacheAirflow
 	YouTube=https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 
 [bdist_wheel]
```

### Comparing `apache-airflow-providers-ftp-3.4.2rc1/setup.py` & `apache-airflow-providers-ftp-3.5.0rc1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,22 +22,22 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-ftp package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "3.4.2"
+version = "3.5.0"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-ftp setup."""
     setup(
         version=version,
-        extras_require={},
+        extras_require={"openlineage": ["apache-airflow-providers-openlineage"]},
         packages=find_namespace_packages(
             include=[
                 "airflow.providers.ftp",
                 "airflow.providers.ftp.*",
                 "airflow.providers.ftp_vendor",
                 "airflow.providers.ftp_vendor.*",
             ],
```

