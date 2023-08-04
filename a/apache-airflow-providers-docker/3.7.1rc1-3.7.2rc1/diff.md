# Comparing `tmp/apache-airflow-providers-docker-3.7.1rc1.tar.gz` & `tmp/apache-airflow-providers-docker-3.7.2rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-docker-3.7.1rc1.tar", last modified: Tue Jun 20 11:41:56 2023, max compression
+gzip compressed data, was "apache-airflow-providers-docker-3.7.2rc1.tar", last modified: Fri Aug  4 21:41:03 2023, max compression
```

## Comparing `apache-airflow-providers-docker-3.7.1rc1.tar` & `apache-airflow-providers-docker-3.7.2rc1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:56.415472 apache-airflow-providers-docker-3.7.1rc1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-docker-3.7.1rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:41:55.000000 apache-airflow-providers-docker-3.7.1rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-docker-3.7.1rc1/NOTICE
--rw-r--r--   0 root         (0) root         (0)    17405 2023-06-20 11:41:56.416806 apache-airflow-providers-docker-3.7.1rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    15877 2023-06-20 11:41:55.000000 apache-airflow-providers-docker-3.7.1rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:56.308576 apache-airflow-providers-docker-3.7.1rc1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:56.310018 apache-airflow-providers-docker-3.7.1rc1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:56.352270 apache-airflow-providers-docker-3.7.1rc1/airflow/providers/docker/
--rw-r--r--   0 root         (0) root         (0)     1531 2023-06-20 11:01:09.000000 apache-airflow-providers-docker-3.7.1rc1/airflow/providers/docker/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:56.360181 apache-airflow-providers-docker-3.7.1rc1/airflow/providers/docker/decorators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-docker-3.7.1rc1/airflow/providers/docker/decorators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6805 2023-06-01 06:14:28.000000 apache-airflow-providers-docker-3.7.1rc1/airflow/providers/docker/decorators/docker.py
--rw-r--r--   0 root         (0) root         (0)     3280 2023-06-20 11:41:55.000000 apache-airflow-providers-docker-3.7.1rc1/airflow/providers/docker/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:56.367660 apache-airflow-providers-docker-3.7.1rc1/airflow/providers/docker/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-docker-3.7.1rc1/airflow/providers/docker/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7940 2023-06-02 11:31:21.000000 apache-airflow-providers-docker-3.7.1rc1/airflow/providers/docker/hooks/docker.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:56.382129 apache-airflow-providers-docker-3.7.1rc1/airflow/providers/docker/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-docker-3.7.1rc1/airflow/providers/docker/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)    23414 2023-06-08 05:42:54.000000 apache-airflow-providers-docker-3.7.1rc1/airflow/providers/docker/operators/docker.py
--rw-r--r--   0 root         (0) root         (0)     9636 2023-06-02 11:31:21.000000 apache-airflow-providers-docker-3.7.1rc1/airflow/providers/docker/operators/docker_swarm.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:56.412192 apache-airflow-providers-docker-3.7.1rc1/apache_airflow_providers_docker.egg-info/
--rw-r--r--   0 root         (0) root         (0)    17405 2023-06-20 11:41:56.000000 apache-airflow-providers-docker-3.7.1rc1/apache_airflow_providers_docker.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      861 2023-06-20 11:41:56.000000 apache-airflow-providers-docker-3.7.1rc1/apache_airflow_providers_docker.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:41:56.000000 apache-airflow-providers-docker-3.7.1rc1/apache_airflow_providers_docker.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      103 2023-06-20 11:41:56.000000 apache-airflow-providers-docker-3.7.1rc1/apache_airflow_providers_docker.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:41:56.000000 apache-airflow-providers-docker-3.7.1rc1/apache_airflow_providers_docker.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       63 2023-06-20 11:41:56.000000 apache-airflow-providers-docker-3.7.1rc1/apache_airflow_providers_docker.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:41:56.000000 apache-airflow-providers-docker-3.7.1rc1/apache_airflow_providers_docker.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-docker-3.7.1rc1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1867 2023-06-20 11:41:56.419389 apache-airflow-providers-docker-3.7.1rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1638 2023-06-20 11:41:55.000000 apache-airflow-providers-docker-3.7.1rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:41:03.406999 apache-airflow-providers-docker-3.7.2rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-docker-3.7.2rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-08-04 21:41:02.000000 apache-airflow-providers-docker-3.7.2rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-docker-3.7.2rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     4443 2023-08-04 21:41:03.407724 apache-airflow-providers-docker-3.7.2rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2805 2023-08-04 21:41:02.000000 apache-airflow-providers-docker-3.7.2rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:41:03.315339 apache-airflow-providers-docker-3.7.2rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:41:03.316325 apache-airflow-providers-docker-3.7.2rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:41:03.351298 apache-airflow-providers-docker-3.7.2rc1/airflow/providers/docker/
+-rw-r--r--   0 root         (0) root         (0)     1575 2023-08-04 21:33:34.000000 apache-airflow-providers-docker-3.7.2rc1/airflow/providers/docker/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:41:03.358707 apache-airflow-providers-docker-3.7.2rc1/airflow/providers/docker/decorators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-docker-3.7.2rc1/airflow/providers/docker/decorators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6806 2023-06-29 05:49:30.000000 apache-airflow-providers-docker-3.7.2rc1/airflow/providers/docker/decorators/docker.py
+-rw-r--r--   0 root         (0) root         (0)     3301 2023-08-04 21:41:02.000000 apache-airflow-providers-docker-3.7.2rc1/airflow/providers/docker/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:41:03.365745 apache-airflow-providers-docker-3.7.2rc1/airflow/providers/docker/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-docker-3.7.2rc1/airflow/providers/docker/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7940 2023-06-02 11:31:21.000000 apache-airflow-providers-docker-3.7.2rc1/airflow/providers/docker/hooks/docker.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:41:03.376606 apache-airflow-providers-docker-3.7.2rc1/airflow/providers/docker/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-docker-3.7.2rc1/airflow/providers/docker/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    23409 2023-08-04 10:24:22.000000 apache-airflow-providers-docker-3.7.2rc1/airflow/providers/docker/operators/docker.py
+-rw-r--r--   0 root         (0) root         (0)     9637 2023-06-29 05:49:30.000000 apache-airflow-providers-docker-3.7.2rc1/airflow/providers/docker/operators/docker_swarm.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 21:41:03.404133 apache-airflow-providers-docker-3.7.2rc1/apache_airflow_providers_docker.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4443 2023-08-04 21:41:03.000000 apache-airflow-providers-docker-3.7.2rc1/apache_airflow_providers_docker.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      861 2023-08-04 21:41:03.000000 apache-airflow-providers-docker-3.7.2rc1/apache_airflow_providers_docker.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 21:41:03.000000 apache-airflow-providers-docker-3.7.2rc1/apache_airflow_providers_docker.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      103 2023-08-04 21:41:03.000000 apache-airflow-providers-docker-3.7.2rc1/apache_airflow_providers_docker.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 21:41:03.000000 apache-airflow-providers-docker-3.7.2rc1/apache_airflow_providers_docker.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       63 2023-08-04 21:41:03.000000 apache-airflow-providers-docker-3.7.2rc1/apache_airflow_providers_docker.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-08-04 21:41:03.000000 apache-airflow-providers-docker-3.7.2rc1/apache_airflow_providers_docker.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5031 2023-08-04 10:24:23.000000 apache-airflow-providers-docker-3.7.2rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1963 2023-08-04 21:41:03.410053 apache-airflow-providers-docker-3.7.2rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1638 2023-08-04 21:41:02.000000 apache-airflow-providers-docker-3.7.2rc1/setup.py
```

### Comparing `apache-airflow-providers-docker-3.7.1rc1/LICENSE` & `apache-airflow-providers-docker-3.7.2rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-docker-3.7.1rc1/MANIFEST.in` & `apache-airflow-providers-docker-3.7.2rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-docker-3.7.1rc1/airflow/providers/docker/__init__.py` & `apache-airflow-providers-docker-3.7.2rc1/airflow/providers/docker/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,18 +24,20 @@
 #
 from __future__ import annotations
 
 import packaging.version
 
 __all__ = ["__version__"]
 
-__version__ = "3.7.1"
+__version__ = "3.7.2"
 
 try:
     from airflow import __version__ as airflow_version
 except ImportError:
     from airflow.version import version as airflow_version
 
-if packaging.version.parse(airflow_version) < packaging.version.parse("2.4.0"):
+if packaging.version.parse(packaging.version.parse(airflow_version).base_version) < packaging.version.parse(
+    "2.4.0"
+):
     raise RuntimeError(
         f"The package `apache-airflow-providers-docker:{__version__}` requires Apache Airflow 2.4.0+"  # NOQA: E501
     )
```

### Comparing `apache-airflow-providers-docker-3.7.1rc1/airflow/providers/docker/decorators/__init__.py` & `apache-airflow-providers-docker-3.7.2rc1/airflow/providers/docker/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-docker-3.7.1rc1/airflow/providers/docker/decorators/docker.py` & `apache-airflow-providers-docker-3.7.2rc1/airflow/providers/docker/decorators/docker.py`

 * *Files 2% similar despite different names*

```diff
@@ -146,15 +146,16 @@
 
 def docker_task(
     python_callable: Callable | None = None,
     multiple_outputs: bool | None = None,
     **kwargs,
 ) -> TaskDecorator:
     """
-    Python operator decorator. Wraps a function into an Airflow operator.
+    Python operator decorator; wraps a function into an Airflow operator.
+
     Also accepts any argument that DockerOperator will via ``kwargs``. Can be reused in a single DAG.
 
     :param python_callable: Function to decorate
     :param multiple_outputs: If set, function return value will be unrolled to multiple XCom values.
         Dict will unroll to XCom values with keys as XCom keys. Defaults to False.
     """
     return task_decorator_factory(
```

### Comparing `apache-airflow-providers-docker-3.7.1rc1/airflow/providers/docker/get_provider_info.py` & `apache-airflow-providers-docker-3.7.2rc1/airflow/providers/docker/get_provider_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-docker",
         "name": "Docker",
         "description": "`Docker <https://docs.docker.com/install/>`__\n",
         "suspended": False,
         "versions": [
+            "3.7.2",
             "3.7.1",
             "3.7.0",
             "3.6.0",
             "3.5.1",
             "3.5.0",
             "3.4.0",
             "3.3.0",
```

### Comparing `apache-airflow-providers-docker-3.7.1rc1/airflow/providers/docker/hooks/__init__.py` & `apache-airflow-providers-docker-3.7.2rc1/airflow/providers/docker/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-docker-3.7.1rc1/airflow/providers/docker/hooks/docker.py` & `apache-airflow-providers-docker-3.7.2rc1/airflow/providers/docker/hooks/docker.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-docker-3.7.1rc1/airflow/providers/docker/operators/__init__.py` & `apache-airflow-providers-docker-3.7.2rc1/airflow/providers/docker/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-docker-3.7.1rc1/airflow/providers/docker/operators/docker.py` & `apache-airflow-providers-docker-3.7.2rc1/airflow/providers/docker/operators/docker.py`

 * *Files 1% similar despite different names*

```diff
@@ -370,15 +370,15 @@
             host_config=self.cli.create_host_config(
                 auto_remove=False,
                 mounts=target_mounts,
                 network_mode=self.network_mode,
                 shm_size=self.shm_size,
                 dns=self.dns,
                 dns_search=self.dns_search,
-                cpu_shares=int(round(self.cpus * 1024)),
+                cpu_shares=round(self.cpus * 1024),
                 port_bindings=self.port_bindings,
                 mem_limit=self.mem_limit,
                 cap_add=self.cap_add,
                 extra_hosts=self.extra_hosts,
                 privileged=self.privileged,
                 device_requests=self.device_requests,
                 log_config=LogConfig(config=docker_log_config),
```

### Comparing `apache-airflow-providers-docker-3.7.1rc1/airflow/providers/docker/operators/docker_swarm.py` & `apache-airflow-providers-docker-3.7.2rc1/airflow/providers/docker/operators/docker_swarm.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 if TYPE_CHECKING:
     from airflow.utils.context import Context
 
 
 class DockerSwarmOperator(DockerOperator):
     """
     Execute a command as an ephemeral docker swarm service.
+
     Example use-case - Using Docker Swarm orchestration to make one-time
     scripts highly available.
 
     A temporary directory is created on the host and
     mounted into a container to allow storing files
     that together exceed the default disk size of 10GB in a container.
     The path to the mounted directory can be accessed
```

### Comparing `apache-airflow-providers-docker-3.7.1rc1/apache_airflow_providers_docker.egg-info/SOURCES.txt` & `apache-airflow-providers-docker-3.7.2rc1/apache_airflow_providers_docker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-docker-3.7.1rc1/pyproject.toml` & `apache-airflow-providers-docker-3.7.2rc1/pyproject.toml`

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

### Comparing `apache-airflow-providers-docker-3.7.1rc1/setup.cfg` & `apache-airflow-providers-docker-3.7.2rc1/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -23,15 +23,16 @@
 	License :: OSI Approved :: Apache Software License
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	Topic :: System :: Monitoring
 project_urls = 
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-docker/3.7.1/
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-docker/3.7.2/
+	Changelog=https://airflow.apache.org/docs/apache-airflow-providers-docker/3.7.2/changelog.html
 	Bug Tracker=https://github.com/apache/airflow/issues
 	Source Code=https://github.com/apache/airflow
 	Slack Chat=https://s.apache.org/airflow-slack
 	Twitter=https://twitter.com/ApacheAirflow
 	YouTube=https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 
 [bdist_wheel]
```

### Comparing `apache-airflow-providers-docker-3.7.1rc1/setup.py` & `apache-airflow-providers-docker-3.7.2rc1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-docker package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "3.7.1"
+version = "3.7.2"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-docker setup."""
     setup(
         version=version,
         extras_require={},
```

