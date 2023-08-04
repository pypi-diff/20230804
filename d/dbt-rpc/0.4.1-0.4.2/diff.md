# Comparing `tmp/dbt-rpc-0.4.1.tar.gz` & `tmp/dbt-rpc-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-rpc-0.4.1.tar", last modified: Tue May  9 19:01:17 2023, max compression
+gzip compressed data, was "dbt-rpc-0.4.2.tar", last modified: Fri Aug  4 18:43:52 2023, max compression
```

## Comparing `dbt-rpc-0.4.1.tar` & `dbt-rpc-0.4.2.tar`

### file list

```diff
@@ -1,57 +1,41 @@
-drwxr-xr-x   0 chenyuli   (502) staff       (20)        0 2023-05-09 19:01:17.295311 dbt-rpc-0.4.1/
--rw-r--r--   0 chenyuli   (502) staff       (20)    11344 2022-07-20 21:30:31.000000 dbt-rpc-0.4.1/LICENSE.md
--rw-r--r--   0 chenyuli   (502) staff       (20)      860 2023-05-09 19:01:17.295141 dbt-rpc-0.4.1/PKG-INFO
--rw-r--r--   0 chenyuli   (502) staff       (20)     1864 2023-05-09 18:24:11.000000 dbt-rpc-0.4.1/README.md
-drwxr-xr-x   0 chenyuli   (502) staff       (20)        0 2023-05-09 19:01:17.278730 dbt-rpc-0.4.1/dbt_rpc/
--rw-r--r--   0 chenyuli   (502) staff       (20)        0 2022-07-20 21:30:31.000000 dbt-rpc-0.4.1/dbt_rpc/__init__.py
--rw-r--r--   0 chenyuli   (502) staff       (20)    17375 2023-05-09 18:24:31.000000 dbt-rpc-0.4.1/dbt_rpc/__main__.py
-drwxr-xr-x   0 chenyuli   (502) staff       (20)        0 2023-05-09 19:01:17.280374 dbt-rpc-0.4.1/dbt_rpc/contracts/
--rw-r--r--   0 chenyuli   (502) staff       (20)    23370 2023-05-09 19:01:03.000000 dbt-rpc-0.4.1/dbt_rpc/contracts/rpc.py
-drwxr-xr-x   0 chenyuli   (502) staff       (20)        0 2023-05-09 19:01:17.280602 dbt-rpc-0.4.1/dbt_rpc/parser/
--rw-r--r--   0 chenyuli   (502) staff       (20)     1966 2023-05-09 18:24:11.000000 dbt-rpc-0.4.1/dbt_rpc/parser/rpc.py
-drwxr-xr-x   0 chenyuli   (502) staff       (20)        0 2023-05-09 19:01:17.284076 dbt-rpc-0.4.1/dbt_rpc/rpc/
--rw-r--r--   0 chenyuli   (502) staff       (20)     1992 2022-07-20 21:30:31.000000 dbt-rpc-0.4.1/dbt_rpc/rpc/__init__.py
--rw-r--r--   0 chenyuli   (502) staff       (20)     8811 2023-05-09 19:01:03.000000 dbt-rpc-0.4.1/dbt_rpc/rpc/builtins.py
--rw-r--r--   0 chenyuli   (502) staff       (20)     2259 2022-07-20 21:30:31.000000 dbt-rpc-0.4.1/dbt_rpc/rpc/error.py
--rw-r--r--   0 chenyuli   (502) staff       (20)     3926 2023-05-09 19:01:03.000000 dbt-rpc-0.4.1/dbt_rpc/rpc/gc.py
--rw-r--r--   0 chenyuli   (502) staff       (20)     6024 2023-05-09 18:24:11.000000 dbt-rpc-0.4.1/dbt_rpc/rpc/logger.py
--rw-r--r--   0 chenyuli   (502) staff       (20)     5133 2023-05-09 18:24:11.000000 dbt-rpc-0.4.1/dbt_rpc/rpc/method.py
--rw-r--r--   0 chenyuli   (502) staff       (20)     4374 2023-05-09 18:24:31.000000 dbt-rpc-0.4.1/dbt_rpc/rpc/node_runners.py
--rw-r--r--   0 chenyuli   (502) staff       (20)     4869 2023-05-09 19:01:03.000000 dbt-rpc-0.4.1/dbt_rpc/rpc/response_manager.py
--rw-r--r--   0 chenyuli   (502) staff       (20)    19107 2023-05-09 18:24:31.000000 dbt-rpc-0.4.1/dbt_rpc/rpc/task_handler.py
--rw-r--r--   0 chenyuli   (502) staff       (20)     2694 2023-05-09 19:01:03.000000 dbt-rpc-0.4.1/dbt_rpc/rpc/task_handler_protocol.py
--rw-r--r--   0 chenyuli   (502) staff       (20)     9510 2023-05-09 19:01:03.000000 dbt-rpc-0.4.1/dbt_rpc/rpc/task_manager.py
-drwxr-xr-x   0 chenyuli   (502) staff       (20)        0 2023-05-09 19:01:17.285959 dbt-rpc-0.4.1/dbt_rpc/task/
--rw-r--r--   0 chenyuli   (502) staff       (20)        0 2023-05-01 23:43:40.000000 dbt-rpc-0.4.1/dbt_rpc/task/__init__.py
--rw-r--r--   0 chenyuli   (502) staff       (20)     1569 2023-05-09 18:24:31.000000 dbt-rpc-0.4.1/dbt_rpc/task/base.py
--rw-r--r--   0 chenyuli   (502) staff       (20)     5059 2023-05-09 18:24:31.000000 dbt-rpc-0.4.1/dbt_rpc/task/cli.py
--rw-r--r--   0 chenyuli   (502) staff       (20)      976 2023-05-09 18:24:31.000000 dbt-rpc-0.4.1/dbt_rpc/task/deps.py
--rw-r--r--   0 chenyuli   (502) staff       (20)    10644 2023-05-09 18:24:31.000000 dbt-rpc-0.4.1/dbt_rpc/task/project_commands.py
--rw-r--r--   0 chenyuli   (502) staff       (20)     6222 2023-05-09 18:24:11.000000 dbt-rpc-0.4.1/dbt_rpc/task/server.py
--rw-r--r--   0 chenyuli   (502) staff       (20)     7375 2023-05-09 18:24:11.000000 dbt-rpc-0.4.1/dbt_rpc/task/sql_commands.py
-drwxr-xr-x   0 chenyuli   (502) staff       (20)        0 2023-05-09 19:01:17.280179 dbt-rpc-0.4.1/dbt_rpc.egg-info/
--rw-r--r--   0 chenyuli   (502) staff       (20)      860 2023-05-09 19:01:17.000000 dbt-rpc-0.4.1/dbt_rpc.egg-info/PKG-INFO
--rw-r--r--   0 chenyuli   (502) staff       (20)     1129 2023-05-09 19:01:17.000000 dbt-rpc-0.4.1/dbt_rpc.egg-info/SOURCES.txt
--rw-r--r--   0 chenyuli   (502) staff       (20)        1 2023-05-09 19:01:17.000000 dbt-rpc-0.4.1/dbt_rpc.egg-info/dependency_links.txt
--rw-r--r--   0 chenyuli   (502) staff       (20)       50 2023-05-09 19:01:17.000000 dbt-rpc-0.4.1/dbt_rpc.egg-info/entry_points.txt
--rw-r--r--   0 chenyuli   (502) staff       (20)        1 2022-07-20 22:27:25.000000 dbt-rpc-0.4.1/dbt_rpc.egg-info/not-zip-safe
--rw-r--r--   0 chenyuli   (502) staff       (20)       34 2023-05-09 19:01:17.000000 dbt-rpc-0.4.1/dbt_rpc.egg-info/requires.txt
--rw-r--r--   0 chenyuli   (502) staff       (20)        8 2023-05-09 19:01:17.000000 dbt-rpc-0.4.1/dbt_rpc.egg-info/top_level.txt
--rw-r--r--   0 chenyuli   (502) staff       (20)       38 2023-05-09 19:01:17.295373 dbt-rpc-0.4.1/setup.cfg
--rw-r--r--   0 chenyuli   (502) staff       (20)     1413 2023-05-09 19:01:03.000000 dbt-rpc-0.4.1/setup.py
-drwxr-xr-x   0 chenyuli   (502) staff       (20)        0 2023-05-09 19:01:17.294876 dbt-rpc-0.4.1/tests/
--rw-r--r--   0 chenyuli   (502) staff       (20)     5803 2023-02-14 23:05:02.000000 dbt-rpc-0.4.1/tests/test_build.py
--rw-r--r--   0 chenyuli   (502) staff       (20)     2763 2023-04-06 22:01:40.000000 dbt-rpc-0.4.1/tests/test_compile.py
--rw-r--r--   0 chenyuli   (502) staff       (20)     1284 2023-05-09 18:24:31.000000 dbt-rpc-0.4.1/tests/test_compile_sql.py
--rw-r--r--   0 chenyuli   (502) staff       (20)     1154 2022-07-23 23:11:05.000000 dbt-rpc-0.4.1/tests/test_concurrency.py
--rw-r--r--   0 chenyuli   (502) staff       (20)     5955 2022-07-20 21:30:31.000000 dbt-rpc-0.4.1/tests/test_deps.py
--rw-r--r--   0 chenyuli   (502) staff       (20)     1071 2023-05-09 16:38:54.000000 dbt-rpc-0.4.1/tests/test_list.py
--rw-r--r--   0 chenyuli   (502) staff       (20)    12604 2023-05-09 18:24:11.000000 dbt-rpc-0.4.1/tests/test_management.py
--rw-r--r--   0 chenyuli   (502) staff       (20)      502 2023-05-03 14:55:51.000000 dbt-rpc-0.4.1/tests/test_reload.py
--rw-r--r--   0 chenyuli   (502) staff       (20)     4500 2022-07-23 23:11:26.000000 dbt-rpc-0.4.1/tests/test_run.py
--rw-r--r--   0 chenyuli   (502) staff       (20)     3018 2022-07-20 21:30:31.000000 dbt-rpc-0.4.1/tests/test_run_operation.py
--rw-r--r--   0 chenyuli   (502) staff       (20)      562 2022-09-14 22:22:50.000000 dbt-rpc-0.4.1/tests/test_run_sql.py
--rw-r--r--   0 chenyuli   (502) staff       (20)     3517 2022-07-20 21:30:31.000000 dbt-rpc-0.4.1/tests/test_seed.py
--rw-r--r--   0 chenyuli   (502) staff       (20)     4638 2022-07-20 21:30:31.000000 dbt-rpc-0.4.1/tests/test_snapshots.py
--rw-r--r--   0 chenyuli   (502) staff       (20)     6387 2022-07-20 21:30:31.000000 dbt-rpc-0.4.1/tests/test_source_freshness.py
--rw-r--r--   0 chenyuli   (502) staff       (20)     3242 2022-07-20 21:30:31.000000 dbt-rpc-0.4.1/tests/test_test.py
+drwxr-xr-x   0 gerda      (501) staff       (20)        0 2023-08-04 18:43:52.890037 dbt-rpc-0.4.2/
+-rw-r--r--   0 gerda      (501) staff       (20)    11344 2021-11-25 19:15:34.000000 dbt-rpc-0.4.2/LICENSE.md
+-rw-r--r--   0 gerda      (501) staff       (20)      882 2023-08-04 18:43:52.889754 dbt-rpc-0.4.2/PKG-INFO
+-rw-r--r--   0 gerda      (501) staff       (20)     1864 2023-04-03 13:46:18.000000 dbt-rpc-0.4.2/README.md
+drwxr-xr-x   0 gerda      (501) staff       (20)        0 2023-08-04 18:43:52.869654 dbt-rpc-0.4.2/dbt_rpc/
+-rw-r--r--   0 gerda      (501) staff       (20)        0 2021-11-25 19:15:34.000000 dbt-rpc-0.4.2/dbt_rpc/__init__.py
+-rw-r--r--   0 gerda      (501) staff       (20)    17375 2023-08-04 18:43:38.000000 dbt-rpc-0.4.2/dbt_rpc/__main__.py
+drwxr-xr-x   0 gerda      (501) staff       (20)        0 2023-08-04 18:43:52.875011 dbt-rpc-0.4.2/dbt_rpc/contracts/
+-rw-r--r--   0 gerda      (501) staff       (20)    23318 2023-08-04 18:43:38.000000 dbt-rpc-0.4.2/dbt_rpc/contracts/rpc.py
+drwxr-xr-x   0 gerda      (501) staff       (20)        0 2023-08-04 18:43:52.875720 dbt-rpc-0.4.2/dbt_rpc/parser/
+-rw-r--r--   0 gerda      (501) staff       (20)     1966 2023-07-27 21:16:32.000000 dbt-rpc-0.4.2/dbt_rpc/parser/rpc.py
+drwxr-xr-x   0 gerda      (501) staff       (20)        0 2023-08-04 18:43:52.884609 dbt-rpc-0.4.2/dbt_rpc/rpc/
+-rw-r--r--   0 gerda      (501) staff       (20)     1992 2021-11-25 19:15:34.000000 dbt-rpc-0.4.2/dbt_rpc/rpc/__init__.py
+-rw-r--r--   0 gerda      (501) staff       (20)     8814 2023-08-04 18:43:38.000000 dbt-rpc-0.4.2/dbt_rpc/rpc/builtins.py
+-rw-r--r--   0 gerda      (501) staff       (20)     2259 2021-11-25 19:15:34.000000 dbt-rpc-0.4.2/dbt_rpc/rpc/error.py
+-rw-r--r--   0 gerda      (501) staff       (20)     3926 2023-07-27 22:52:19.000000 dbt-rpc-0.4.2/dbt_rpc/rpc/gc.py
+-rw-r--r--   0 gerda      (501) staff       (20)     6024 2023-08-01 18:05:20.000000 dbt-rpc-0.4.2/dbt_rpc/rpc/logger.py
+-rw-r--r--   0 gerda      (501) staff       (20)     5133 2023-07-27 21:16:32.000000 dbt-rpc-0.4.2/dbt_rpc/rpc/method.py
+-rw-r--r--   0 gerda      (501) staff       (20)     4374 2023-08-04 18:43:38.000000 dbt-rpc-0.4.2/dbt_rpc/rpc/node_runners.py
+-rw-r--r--   0 gerda      (501) staff       (20)     4869 2023-08-01 19:54:44.000000 dbt-rpc-0.4.2/dbt_rpc/rpc/response_manager.py
+-rw-r--r--   0 gerda      (501) staff       (20)    19111 2023-08-04 18:43:38.000000 dbt-rpc-0.4.2/dbt_rpc/rpc/task_handler.py
+-rw-r--r--   0 gerda      (501) staff       (20)     2694 2023-07-27 22:52:19.000000 dbt-rpc-0.4.2/dbt_rpc/rpc/task_handler_protocol.py
+-rw-r--r--   0 gerda      (501) staff       (20)     9510 2023-08-04 18:43:38.000000 dbt-rpc-0.4.2/dbt_rpc/rpc/task_manager.py
+drwxr-xr-x   0 gerda      (501) staff       (20)        0 2023-08-04 18:43:52.888973 dbt-rpc-0.4.2/dbt_rpc/task/
+-rw-r--r--   0 gerda      (501) staff       (20)        0 2021-11-25 19:15:34.000000 dbt-rpc-0.4.2/dbt_rpc/task/__init__.py
+-rw-r--r--   0 gerda      (501) staff       (20)     1102 2023-08-04 18:43:38.000000 dbt-rpc-0.4.2/dbt_rpc/task/base.py
+-rw-r--r--   0 gerda      (501) staff       (20)     5226 2023-08-04 18:43:38.000000 dbt-rpc-0.4.2/dbt_rpc/task/cli.py
+-rw-r--r--   0 gerda      (501) staff       (20)      976 2023-08-04 18:43:38.000000 dbt-rpc-0.4.2/dbt_rpc/task/deps.py
+-rw-r--r--   0 gerda      (501) staff       (20)    11005 2023-08-04 18:43:38.000000 dbt-rpc-0.4.2/dbt_rpc/task/project_commands.py
+-rw-r--r--   0 gerda      (501) staff       (20)     6222 2023-08-01 18:05:20.000000 dbt-rpc-0.4.2/dbt_rpc/task/server.py
+-rw-r--r--   0 gerda      (501) staff       (20)     7375 2023-07-27 21:16:32.000000 dbt-rpc-0.4.2/dbt_rpc/task/sql_commands.py
+drwxr-xr-x   0 gerda      (501) staff       (20)        0 2023-08-04 18:43:52.874462 dbt-rpc-0.4.2/dbt_rpc.egg-info/
+-rw-r--r--   0 gerda      (501) staff       (20)      882 2023-08-04 18:43:52.000000 dbt-rpc-0.4.2/dbt_rpc.egg-info/PKG-INFO
+-rw-r--r--   0 gerda      (501) staff       (20)      790 2023-08-04 18:43:52.000000 dbt-rpc-0.4.2/dbt_rpc.egg-info/SOURCES.txt
+-rw-r--r--   0 gerda      (501) staff       (20)        1 2023-08-04 18:43:52.000000 dbt-rpc-0.4.2/dbt_rpc.egg-info/dependency_links.txt
+-rw-r--r--   0 gerda      (501) staff       (20)       51 2023-08-04 18:43:52.000000 dbt-rpc-0.4.2/dbt_rpc.egg-info/entry_points.txt
+-rw-r--r--   0 gerda      (501) staff       (20)        1 2022-02-01 20:12:38.000000 dbt-rpc-0.4.2/dbt_rpc.egg-info/not-zip-safe
+-rw-r--r--   0 gerda      (501) staff       (20)       41 2023-08-04 18:43:52.000000 dbt-rpc-0.4.2/dbt_rpc.egg-info/requires.txt
+-rw-r--r--   0 gerda      (501) staff       (20)        8 2023-08-04 18:43:52.000000 dbt-rpc-0.4.2/dbt_rpc.egg-info/top_level.txt
+-rw-r--r--   0 gerda      (501) staff       (20)       38 2023-08-04 18:43:52.890167 dbt-rpc-0.4.2/setup.cfg
+-rw-r--r--   0 gerda      (501) staff       (20)     1420 2023-08-04 18:43:44.000000 dbt-rpc-0.4.2/setup.py
```

### Comparing `dbt-rpc-0.4.1/LICENSE.md` & `dbt-rpc-0.4.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `dbt-rpc-0.4.1/PKG-INFO` & `dbt-rpc-0.4.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.2
 Name: dbt-rpc
-Version: 0.4.1
+Version: 0.4.2
 Summary:  A JSON RPC server that provides an interface to programmically interact with dbt projects. 
 Home-page: https://github.com/dbt-labs/dbt-rpc
 Author: dbt Labs
 Author-email: info@dbtlabs.com
+License: UNKNOWN
+Description:  A JSON RPC server that provides an interface to programmically interact with dbt projects. 
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.6.3
-License-File: LICENSE.md
-
- A JSON RPC server that provides an interface to programmically interact with dbt projects.
```

### Comparing `dbt-rpc-0.4.1/README.md` & `dbt-rpc-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `dbt-rpc-0.4.1/dbt_rpc/__main__.py` & `dbt-rpc-0.4.2/dbt_rpc/__main__.py`

 * *Files identical despite different names*

### Comparing `dbt-rpc-0.4.1/dbt_rpc/contracts/rpc.py` & `dbt-rpc-0.4.2/dbt_rpc/contracts/rpc.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,27 +14,25 @@
     RunResultsArtifact,
     TimingInfo,
     CatalogArtifact,
     CatalogResults,
     ExecutionResult,
     FreshnessExecutionResultArtifact,
     FreshnessResult,
-    RunOperationResult,
-    RunOperationResultsArtifact,
     RunExecutionResult,
 )
 from dbt.contracts.util import VersionedSchema, schema_version
 from dbt.exceptions import DbtInternalError
 from dbt.logger import LogMessage
 from dbt.utils import restrict_to
 
-
 TaskTags = Optional[Dict[str, Any]]
 TaskID = uuid.UUID
 
+
 # Inputs
 
 
 @dataclass
 class RPCParameters(dbtClassMixin):
     task_tags: TaskTags
     timeout: Optional[float]
@@ -83,14 +81,15 @@
     threads: Optional[int] = None
     models: Union[None, str, List[str]] = None
     select: Union[None, str, List[str]] = None
     exclude: Union[None, str, List[str]] = None
     selector: Optional[str] = None
     state: Optional[str] = None
     defer: Optional[bool] = None
+    favor_state: Optional[bool] = None
 
 
 @dataclass
 class RPCSnapshotParameters(RPCParameters):
     threads: Optional[int] = None
     select: Union[None, str, List[str]] = None
     exclude: Union[None, str, List[str]] = None
@@ -100,14 +99,15 @@
 
 @dataclass
 class RPCTestParameters(RPCCompileParameters):
     data: bool = False
     schema: bool = False
     state: Optional[str] = None
     defer: Optional[bool] = None
+    favor_state: Optional[bool] = None
 
 
 @dataclass
 class RPCSeedParameters(RPCParameters):
     threads: Optional[int] = None
     select: Union[None, str, List[str]] = None
     exclude: Union[None, str, List[str]] = None
@@ -127,14 +127,15 @@
     resource_types: Optional[List[str]] = None
     select: Union[None, str, List[str]] = None
     threads: Optional[int] = None
     exclude: Union[None, str, List[str]] = None
     selector: Optional[str] = None
     state: Optional[str] = None
     defer: Optional[bool] = None
+    favor_state: Optional[bool] = None
 
 
 @dataclass
 class RPCCliParameters(RPCParameters):
     cli: str
 
 
@@ -306,69 +307,63 @@
             elapsed_time=self.elapsed_time,
             args=self.args,
         )
         writable.write(path)
 
     @classmethod
     def from_local_result(
-        cls,
-        base: RunExecutionResult,
-        logs: List[LogMessage],
+            cls,
+            base: RunExecutionResult,
+            logs: List[LogMessage],
     ) -> "RemoteExecutionResult":
         return cls(
             generated_at=base.generated_at,
             results=base.results,
             elapsed_time=base.elapsed_time,
             args=base.args,
             logs=logs,
         )
 
 
 @dataclass
-class ResultTable(dbtClassMixin):
-    column_names: List[str]
-    rows: List[Any]
-
-
-@dataclass
-@schema_version("remote-run-operation-result", 1)
-class RemoteRunOperationResult(RunOperationResult, RemoteResult):
-    generated_at: datetime = field(default_factory=datetime.utcnow)
+@schema_version("poll-remote-run-operation-result", 1)
+class RunOperationCompleteResult(
+    RemoteExecutionResult,
+):
+    success: bool = field(default_factory=bool)
 
     @classmethod
     def from_local_result(
-        cls,
-        base: RunOperationResultsArtifact,
-        logs: List[LogMessage],
-    ) -> "RemoteRunOperationResult":
+            cls,
+            base: RunExecutionResult,
+            logs: List[LogMessage],
+    ) -> "RemoteExecutionResult":
         return cls(
-            generated_at=base.metadata.generated_at,
+            generated_at=base.generated_at,
             results=base.results,
             elapsed_time=base.elapsed_time,
-            success=base.success,
             logs=logs,
+            success=base.success,
         )
 
-    def write(self, path: str):
-        writable = RunOperationResultsArtifact.from_success(
-            success=self.success,
-            generated_at=self.generated_at,
-            elapsed_time=self.elapsed_time,
-        )
-        writable.write(path)
+
+@dataclass
+class ResultTable(dbtClassMixin):
+    column_names: List[str]
+    rows: List[Any]
 
 
 @dataclass
 @schema_version("remote-freshness-result", 1)
 class RemoteFreshnessResult(FreshnessResult, RemoteResult):
     @classmethod
     def from_local_result(
-        cls,
-        base: FreshnessResult,
-        logs: List[LogMessage],
+            cls,
+            base: FreshnessResult,
+            logs: List[LogMessage],
     ) -> "RemoteFreshnessResult":
         return cls(
             metadata=base.metadata,
             results=base.results,
             elapsed_time=base.elapsed_time,
             logs=logs,
         )
@@ -387,15 +382,14 @@
 
 RPCResult = Union[
     RemoteCompileResult,
     RemoteExecutionResult,
     RemoteFreshnessResult,
     RemoteCatalogResults,
     RemoteDepsResult,
-    RemoteRunOperationResult,
 ]
 
 
 # GC types
 
 
 class GCResultState(StrEnum):
@@ -567,19 +561,19 @@
     state: TaskHandlerState = field(
         metadata=restrict_to(TaskHandlerState.Success, TaskHandlerState.Failed),
     )
     generated_at: datetime = field(default_factory=datetime.utcnow)
 
     @classmethod
     def from_result(
-        cls: Type["PollRemoteEmptyCompleteResult"],
-        base: RemoteDepsResult,
-        tags: TaskTags,
-        timing: TaskTiming,
-        logs: List[LogMessage],
+            cls: Type["PollRemoteEmptyCompleteResult"],
+            base: RemoteDepsResult,
+            tags: TaskTags,
+            timing: TaskTiming,
+            logs: List[LogMessage],
     ) -> "PollRemoteEmptyCompleteResult":
         return cls(
             logs=logs,
             tags=tags,
             state=timing.state,
             start=timing.start,
             end=timing.end,
@@ -604,19 +598,19 @@
 ):
     state: TaskHandlerState = field(
         metadata=restrict_to(TaskHandlerState.Success, TaskHandlerState.Failed),
     )
 
     @classmethod
     def from_result(
-        cls: Type["PollExecuteCompleteResult"],
-        base: RemoteExecutionResult,
-        tags: TaskTags,
-        timing: TaskTiming,
-        logs: List[LogMessage],
+            cls: Type["PollExecuteCompleteResult"],
+            base: RemoteExecutionResult,
+            tags: TaskTags,
+            timing: TaskTiming,
+            logs: List[LogMessage],
     ) -> "PollExecuteCompleteResult":
         return cls(
             results=base.results,
             elapsed_time=base.elapsed_time,
             logs=logs,
             tags=tags,
             state=timing.state,
@@ -624,126 +618,126 @@
             end=timing.end,
             elapsed=timing.elapsed,
             generated_at=base.generated_at,
         )
 
 
 @dataclass
-@schema_version("poll-remote-compile-result", 1)
-class PollCompileCompleteResult(
-    RemoteCompileResult,
+@schema_version("poll-remote-execution-result", 1)
+class PollRunOperationCompleteResult(
+    RunOperationCompleteResult,
     PollResult,
 ):
     state: TaskHandlerState = field(
         metadata=restrict_to(TaskHandlerState.Success, TaskHandlerState.Failed),
     )
 
     @classmethod
     def from_result(
-        cls: Type["PollCompileCompleteResult"],
-        base: RemoteCompileResult,
-        tags: TaskTags,
-        timing: TaskTiming,
-        logs: List[LogMessage],
-    ) -> "PollCompileCompleteResult":
+            cls: Type["PollRunOperationCompleteResult"],
+            base: RemoteExecutionResult,
+            tags: TaskTags,
+            timing: TaskTiming,
+            logs: List[LogMessage],
+    ) -> "PollRunOperationCompleteResult":
         return cls(
-            raw_sql=base.raw_sql,
-            compiled_sql=base.compiled_sql,
-            node=base.node,
-            timing=base.timing,
+            results=base.results,
+            elapsed_time=base.elapsed_time,
             logs=logs,
             tags=tags,
             state=timing.state,
             start=timing.start,
             end=timing.end,
             elapsed=timing.elapsed,
             generated_at=base.generated_at,
+            success=base.success,
         )
 
 
 @dataclass
-@schema_version("poll-remote-run-result", 1)
-class PollRunCompleteResult(
-    RemoteRunResult,
+@schema_version("poll-remote-compile-result", 1)
+class PollCompileCompleteResult(
+    RemoteCompileResult,
     PollResult,
 ):
     state: TaskHandlerState = field(
         metadata=restrict_to(TaskHandlerState.Success, TaskHandlerState.Failed),
     )
 
     @classmethod
     def from_result(
-        cls: Type["PollRunCompleteResult"],
-        base: RemoteRunResult,
-        tags: TaskTags,
-        timing: TaskTiming,
-        logs: List[LogMessage],
-    ) -> "PollRunCompleteResult":
+            cls: Type["PollCompileCompleteResult"],
+            base: RemoteCompileResult,
+            tags: TaskTags,
+            timing: TaskTiming,
+            logs: List[LogMessage],
+    ) -> "PollCompileCompleteResult":
         return cls(
             raw_sql=base.raw_sql,
             compiled_sql=base.compiled_sql,
             node=base.node,
             timing=base.timing,
             logs=logs,
-            table=base.table,
             tags=tags,
             state=timing.state,
             start=timing.start,
             end=timing.end,
             elapsed=timing.elapsed,
             generated_at=base.generated_at,
         )
 
 
 @dataclass
-@schema_version("poll-remote-run-operation-result", 1)
-class PollRunOperationCompleteResult(
-    RemoteRunOperationResult,
+@schema_version("poll-remote-run-result", 1)
+class PollRunCompleteResult(
+    RemoteRunResult,
     PollResult,
 ):
     state: TaskHandlerState = field(
         metadata=restrict_to(TaskHandlerState.Success, TaskHandlerState.Failed),
     )
 
     @classmethod
     def from_result(
-        cls: Type["PollRunOperationCompleteResult"],
-        base: RemoteRunOperationResult,
-        tags: TaskTags,
-        timing: TaskTiming,
-        logs: List[LogMessage],
-    ) -> "PollRunOperationCompleteResult":
+            cls: Type["PollRunCompleteResult"],
+            base: RemoteRunResult,
+            tags: TaskTags,
+            timing: TaskTiming,
+            logs: List[LogMessage],
+    ) -> "PollRunCompleteResult":
         return cls(
-            success=base.success,
-            results=base.results,
-            generated_at=base.generated_at,
-            elapsed_time=base.elapsed_time,
+            raw_sql=base.raw_sql,
+            compiled_sql=base.compiled_sql,
+            node=base.node,
+            timing=base.timing,
             logs=logs,
+            table=base.table,
             tags=tags,
             state=timing.state,
             start=timing.start,
             end=timing.end,
             elapsed=timing.elapsed,
+            generated_at=base.generated_at,
         )
 
 
 @dataclass
 @schema_version("poll-remote-catalog-result", 1)
 class PollCatalogCompleteResult(RemoteCatalogResults, PollResult):
     state: TaskHandlerState = field(
         metadata=restrict_to(TaskHandlerState.Success, TaskHandlerState.Failed),
     )
 
     @classmethod
     def from_result(
-        cls: Type["PollCatalogCompleteResult"],
-        base: RemoteCatalogResults,
-        tags: TaskTags,
-        timing: TaskTiming,
-        logs: List[LogMessage],
+            cls: Type["PollCatalogCompleteResult"],
+            base: RemoteCatalogResults,
+            tags: TaskTags,
+            timing: TaskTiming,
+            logs: List[LogMessage],
     ) -> "PollCatalogCompleteResult":
         return cls(
             nodes=base.nodes,
             sources=base.sources,
             generated_at=base.generated_at,
             errors=base.errors,
             _compile_results=base._compile_results,
@@ -767,19 +761,19 @@
 class PollGetManifestResult(GetManifestResult, PollResult):
     state: TaskHandlerState = field(
         metadata=restrict_to(TaskHandlerState.Success, TaskHandlerState.Failed),
     )
 
     @classmethod
     def from_result(
-        cls: Type["PollGetManifestResult"],
-        base: GetManifestResult,
-        tags: TaskTags,
-        timing: TaskTiming,
-        logs: List[LogMessage],
+            cls: Type["PollGetManifestResult"],
+            base: GetManifestResult,
+            tags: TaskTags,
+            timing: TaskTiming,
+            logs: List[LogMessage],
     ) -> "PollGetManifestResult":
         return cls(
             manifest=base.manifest,
             logs=logs,
             tags=tags,
             state=timing.state,
             start=timing.start,
@@ -794,19 +788,19 @@
     state: TaskHandlerState = field(
         metadata=restrict_to(TaskHandlerState.Success,
                              TaskHandlerState.Failed),
     )
 
     @classmethod
     def from_result(
-        cls: Type['PollListResult'],
-        base: RemoteListResults,
-        tags: TaskTags,
-        timing: TaskTiming,
-        logs: List[LogMessage],
+            cls: Type['PollListResult'],
+            base: RemoteListResults,
+            tags: TaskTags,
+            timing: TaskTiming,
+            logs: List[LogMessage],
     ) -> 'PollListResult':
         return cls(
             output=base.output,
             logs=logs,
             tags=tags,
             state=timing.state,
             start=timing.start,
@@ -820,19 +814,19 @@
 class PollFreshnessResult(RemoteFreshnessResult, PollResult):
     state: TaskHandlerState = field(
         metadata=restrict_to(TaskHandlerState.Success, TaskHandlerState.Failed),
     )
 
     @classmethod
     def from_result(
-        cls: Type["PollFreshnessResult"],
-        base: RemoteFreshnessResult,
-        tags: TaskTags,
-        timing: TaskTiming,
-        logs: List[LogMessage],
+            cls: Type["PollFreshnessResult"],
+            base: RemoteFreshnessResult,
+            tags: TaskTags,
+            timing: TaskTiming,
+            logs: List[LogMessage],
     ) -> "PollFreshnessResult":
         return cls(
             logs=logs,
             tags=tags,
             state=timing.state,
             start=timing.start,
             end=timing.end,
```

### Comparing `dbt-rpc-0.4.1/dbt_rpc/parser/rpc.py` & `dbt-rpc-0.4.2/dbt_rpc/parser/rpc.py`

 * *Files identical despite different names*

### Comparing `dbt-rpc-0.4.1/dbt_rpc/rpc/__init__.py` & `dbt-rpc-0.4.2/dbt_rpc/rpc/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-rpc-0.4.1/dbt_rpc/rpc/builtins.py` & `dbt-rpc-0.4.2/dbt_rpc/rpc/builtins.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,17 @@
 import signal
 from datetime import datetime
 from typing import Type, Union, Any, List, Dict
 
 import dbt.exceptions
 from dbt_rpc.contracts.rpc import (
     PollListResult,
+    PollRunOperationCompleteResult,
     RemoteListResults,
+    RunOperationCompleteResult,
     TaskTags,
     StatusParameters,
     ReloadParameters,
     LastParse,
     GCParameters,
     GCResult,
     GetManifestResult,
@@ -22,27 +24,25 @@
     PSResult,
     RemoteExecutionResult,
     RemoteFreshnessResult,
     RemoteRunResult,
     RemoteCompileResult,
     RemoteCatalogResults,
     RemoteDepsResult,
-    RemoteRunOperationResult,
     PollParameters,
     PollResult,
     PollInProgressResult,
     PollKilledResult,
     PollExecuteCompleteResult,
     PollGetManifestResult,
     PollRunCompleteResult,
     PollCompileCompleteResult,
     PollCatalogCompleteResult,
     PollFreshnessResult,
     PollRemoteEmptyCompleteResult,
-    PollRunOperationCompleteResult,
     TaskHandlerState,
     TaskTiming,
 )
 from dbt.logger import LogMessage
 from dbt_rpc.rpc.error import dbt_error, RPCException
 from dbt_rpc.rpc.method import RemoteBuiltinMethod
 from dbt_rpc.rpc.task_handler import RequestTaskHandler
@@ -145,40 +145,40 @@
     cls: Type[
         Union[
             PollExecuteCompleteResult,
             PollRunCompleteResult,
             PollCompileCompleteResult,
             PollCatalogCompleteResult,
             PollRemoteEmptyCompleteResult,
-            PollRunOperationCompleteResult,
             PollGetManifestResult,
             PollFreshnessResult,
             PollListResult,
+            PollRunOperationCompleteResult
         ]
     ]
 
     if isinstance(result, RemoteExecutionResult):
         cls = PollExecuteCompleteResult
     # order matters here, as RemoteRunResult subclasses RemoteCompileResult
     elif isinstance(result, RemoteRunResult):
         cls = PollRunCompleteResult
     elif isinstance(result, RemoteCompileResult):
         cls = PollCompileCompleteResult
     elif isinstance(result, RemoteCatalogResults):
         cls = PollCatalogCompleteResult
     elif isinstance(result, RemoteDepsResult):
         cls = PollRemoteEmptyCompleteResult
-    elif isinstance(result, RemoteRunOperationResult):
-        cls = PollRunOperationCompleteResult
     elif isinstance(result, GetManifestResult):
         cls = PollGetManifestResult
     elif isinstance(result, RemoteFreshnessResult):
         cls = PollFreshnessResult
     elif isinstance(result, RemoteListResults):
         cls = PollListResult
+    elif isinstance(result, RunOperationCompleteResult):
+        cls = PollRunOperationCompleteResult
     else:
         raise dbt.exceptions.DbtInternalError(
             "got invalid result in poll_complete: {}".format(result)
         )
     return cls.from_result(result, tags, timing, logs)
```

### Comparing `dbt-rpc-0.4.1/dbt_rpc/rpc/error.py` & `dbt-rpc-0.4.2/dbt_rpc/rpc/error.py`

 * *Files identical despite different names*

### Comparing `dbt-rpc-0.4.1/dbt_rpc/rpc/gc.py` & `dbt-rpc-0.4.2/dbt_rpc/rpc/gc.py`

 * *Files identical despite different names*

### Comparing `dbt-rpc-0.4.1/dbt_rpc/rpc/logger.py` & `dbt-rpc-0.4.2/dbt_rpc/rpc/logger.py`

 * *Files identical despite different names*

### Comparing `dbt-rpc-0.4.1/dbt_rpc/rpc/method.py` & `dbt-rpc-0.4.2/dbt_rpc/rpc/method.py`

 * *Files identical despite different names*

### Comparing `dbt-rpc-0.4.1/dbt_rpc/rpc/node_runners.py` & `dbt-rpc-0.4.2/dbt_rpc/rpc/node_runners.py`

 * *Files identical despite different names*

### Comparing `dbt-rpc-0.4.1/dbt_rpc/rpc/response_manager.py` & `dbt-rpc-0.4.2/dbt_rpc/rpc/response_manager.py`

 * *Files identical despite different names*

### Comparing `dbt-rpc-0.4.1/dbt_rpc/rpc/task_handler.py` & `dbt-rpc-0.4.2/dbt_rpc/rpc/task_handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,15 +80,15 @@
         # reload the active plugin
         load_plugin(self.task.config.credentials.type)
         # register it
         register_adapter(self.task.config)
 
     def task_exec(self) -> None:
         """task_exec runs first inside the child process"""
-        if type(self.task) != RemoteListTask:
+        if type(self.task) is not RemoteListTask:
             # TODO: find another solution for this.. in theory it stops us from
             # being able to kill RemoteListTask processes
             signal.signal(signal.SIGTERM, sigterm_handler)
         # the first thing we do in a new process: push logging back over our
         # queue
         handler = QueueLogHandler(self.queue)
         with handler.applicationbound():
```

### Comparing `dbt-rpc-0.4.1/dbt_rpc/rpc/task_handler_protocol.py` & `dbt-rpc-0.4.2/dbt_rpc/rpc/task_handler_protocol.py`

 * *Files identical despite different names*

### Comparing `dbt-rpc-0.4.1/dbt_rpc/rpc/task_manager.py` & `dbt-rpc-0.4.2/dbt_rpc/rpc/task_manager.py`

 * *Files identical despite different names*

### Comparing `dbt-rpc-0.4.1/dbt_rpc/task/cli.py` & `dbt-rpc-0.4.2/dbt_rpc/task/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import abc
 import shlex
 from dbt.clients.yaml_helper import Dumper, yaml  # noqa: F401
-from typing import Type, Optional
+from typing import Type, Optional, AbstractSet
 
 from dbt_rpc.contracts.rpc import RPCCliParameters
 
 from dbt_rpc.rpc.method import (
     RemoteMethod,
     RemoteManifestMethod,
     Parameters,
@@ -137,7 +137,10 @@
 
     def interpret_results(self, results):
         if self.real_task is None:
             # I don't know what happened, but it was surely some flavor of
             # failure
             return False
         return self.real_task.interpret_results(results)
+
+    def defer_to_manifest(self, adapter, selected_uids: AbstractSet[str]):
+        return self.real_task.defer_to_manifest(self, adapter, selected_uids)
```

### Comparing `dbt-rpc-0.4.1/dbt_rpc/task/deps.py` & `dbt-rpc-0.4.2/dbt_rpc/task/deps.py`

 * *Files identical despite different names*

### Comparing `dbt-rpc-0.4.1/dbt_rpc/task/project_commands.py` & `dbt-rpc-0.4.2/dbt_rpc/task/project_commands.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,49 +1,48 @@
 import json
 from datetime import datetime
 from pathlib import Path
 from typing import List, Optional, Union
 
-from dbt.flags import get_flags
 from dbt.contracts.graph.manifest import WritableManifest
+from dbt.exceptions import DbtRuntimeError
+from dbt.flags import get_flags
+from dbt.task.base import BaseTask
+from dbt.task.build import BuildTask
+from dbt.task.compile import CompileTask
+from dbt.task.freshness import FreshnessTask
+from dbt.task.generate import GenerateTask
+from dbt.task.list import ListTask
+from dbt.task.run import RunTask
+from dbt.task.run_operation import RunOperationTask
+from dbt.task.seed import SeedTask
+from dbt.task.snapshot import SnapshotTask
+from dbt.task.test import TestTask
+
 from dbt_rpc.contracts.rpc import (
     GetManifestParameters,
     GetManifestResult,
     RPCCompileParameters,
     RPCDocsGenerateParameters,
     RPCRunParameters,
     RPCRunOperationParameters,
     RPCSeedParameters,
     RPCTestParameters,
     RemoteCatalogResults,
     RemoteExecutionResult,
     RemoteListResults,
-    RemoteRunOperationResult,
     RPCSnapshotParameters,
     RPCSourceFreshnessParameters,
     RPCListParameters,
     RPCBuildParameters,
+    RunOperationCompleteResult,
 )
-from dbt.exceptions import DbtRuntimeError
 from dbt_rpc.rpc.method import (
     Parameters, RemoteManifestMethod
 )
-
-from dbt.task.base import BaseTask
-from dbt.task.compile import CompileTask
-from dbt.task.freshness import FreshnessTask
-from dbt.task.generate import GenerateTask
-from dbt.task.run import RunTask
-from dbt.task.run_operation import RunOperationTask
-from dbt.task.seed import SeedTask
-from dbt.task.snapshot import SnapshotTask
-from dbt.task.test import TestTask
-from dbt.task.list import ListTask
-from dbt.task.build import BuildTask
-
 from .base import RPCTask
 from .cli import HasCLI
 
 
 class RPCCommandTask(
     RPCTask[Parameters],
     HasCLI[Parameters, RemoteExecutionResult],
@@ -106,14 +105,18 @@
 
         if params.threads is not None:
             self.args.threads = params.threads
         if params.defer is None:
             self.args.defer = get_flags().DEFER
         else:
             self.args.defer = params.defer
+        if params.favor_state is None:
+            self.args.favor_state = False
+        else:
+            self.args.favor_state = params.favor_state
 
         self.args.state = state_path(params.state)
         self.set_previous_state()
 
 
 class RemoteSeedProjectTask(RPCCommandTask[RPCSeedParameters], SeedTask):
     METHOD_NAME = 'seed'
@@ -179,16 +182,16 @@
             errors=errors,
             logs=[],
         )
 
 
 class RemoteRunOperationTask(
     RunOperationTask,
-    RemoteManifestMethod[RPCRunOperationParameters, RemoteRunOperationResult],
-    HasCLI[RPCRunOperationParameters, RemoteRunOperationResult],
+    RemoteManifestMethod[RPCRunOperationParameters, RunOperationCompleteResult],
+    HasCLI[RPCRunOperationParameters, RunOperationCompleteResult],
 ):
     METHOD_NAME = 'run-operation'
 
     def __init__(self, args, config, manifest):
         super().__init__(args, config)
         RemoteManifestMethod.__init__(
             self, args, config, manifest  # type: ignore
@@ -207,21 +210,22 @@
             return self.args.args
         else:
             return RunOperationTask._get_kwargs(self)
 
     def _runtime_initialize(self):
         return RunOperationTask._runtime_initialize(self)
 
-    def handle_request(self) -> RemoteRunOperationResult:
+    def handle_request(self) -> RunOperationCompleteResult:
         base = RunOperationTask.run(self)
-        result = RemoteRunOperationResult.from_local_result(base=base, logs=[])
+        base.generated_at = datetime.utcnow()
+        result = RunOperationCompleteResult.from_local_result(base=base, logs=[])
         return result
 
-    def interpret_results(self, results):
-        return results.success
+    # def interpret_results(self, results):
+    #     return results[].success
 
 
 class RemoteSnapshotTask(RPCCommandTask[RPCSnapshotParameters], SnapshotTask):
     METHOD_NAME = 'snapshot'
 
     def set_args(self, params: RPCSnapshotParameters) -> None:
         # select has an argparse `dest` value of `models`.
@@ -331,10 +335,14 @@
 
         if params.threads is not None:
             self.args.threads = params.threads
         if params.defer is None:
             self.args.defer = get_flags().DEFER
         else:
             self.args.defer = params.defer
+        if params.favor_state is None:
+            self.args.favor_state = False
+        else:
+            self.args.favor_state = params.favor_state
 
         self.args.state = state_path(params.state)
         self.set_previous_state()
```

### Comparing `dbt-rpc-0.4.1/dbt_rpc/task/server.py` & `dbt-rpc-0.4.2/dbt_rpc/task/server.py`

 * *Files identical despite different names*

### Comparing `dbt-rpc-0.4.1/dbt_rpc/task/sql_commands.py` & `dbt-rpc-0.4.2/dbt_rpc/task/sql_commands.py`

 * *Files identical despite different names*

### Comparing `dbt-rpc-0.4.1/dbt_rpc.egg-info/PKG-INFO` & `dbt-rpc-0.4.2/dbt_rpc.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.2
 Name: dbt-rpc
-Version: 0.4.1
+Version: 0.4.2
 Summary:  A JSON RPC server that provides an interface to programmically interact with dbt projects. 
 Home-page: https://github.com/dbt-labs/dbt-rpc
 Author: dbt Labs
 Author-email: info@dbtlabs.com
+License: UNKNOWN
+Description:  A JSON RPC server that provides an interface to programmically interact with dbt projects. 
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.6.3
-License-File: LICENSE.md
-
- A JSON RPC server that provides an interface to programmically interact with dbt projects.
```

### Comparing `dbt-rpc-0.4.1/setup.py` & `dbt-rpc-0.4.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 
 package_name = "dbt-rpc"
-package_version = "0.4.1"
+package_version = "0.4.2"
 description = """ A JSON RPC server that provides an interface to programmically interact with dbt projects. """
 
 
 setup(
     name=package_name,
     version=package_version,
     description=description,
@@ -24,15 +24,15 @@
     include_package_data=True,
     test_suite="tests",
     entry_points={
         "console_scripts": [
             "dbt-rpc = dbt_rpc.__main__:main",
         ],
     },
-    install_requires=["json-rpc>=1.14,<2", "dbt-core>=1.5.0"],
+    install_requires=["json-rpc>=1.14,<2", "dbt-core>=1.5.0,<1.6.0"],
     zip_safe=False,
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: Microsoft :: Windows",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: POSIX :: Linux",
```

