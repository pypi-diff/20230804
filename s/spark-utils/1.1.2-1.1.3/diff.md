# Comparing `tmp/spark_utils-1.1.2.tar.gz` & `tmp/spark_utils-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spark_utils-1.1.2.tar", max compression
+gzip compressed data, was "spark_utils-1.1.3.tar", max compression
```

## Comparing `spark_utils-1.1.2.tar` & `spark_utils-1.1.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1075 2023-07-25 14:18:04.838493 spark_utils-1.1.2/LICENSE
--rw-r--r--   0        0        0     6766 2023-07-25 14:18:04.838493 spark_utils-1.1.2/README.md
--rw-r--r--   0        0        0      791 2023-07-25 14:18:26.890892 spark_utils-1.1.2/pyproject.toml
--rw-r--r--   0        0        0     1135 2023-07-25 14:18:04.842493 spark_utils-1.1.2/spark_utils/__init__.py
--rw-r--r--   0        0        0       22 2023-07-25 14:18:26.890892 spark_utils-1.1.2/spark_utils/_version.py
--rw-r--r--   0        0        0     1134 2023-07-25 14:18:04.842493 spark_utils-1.1.2/spark_utils/common/__init__.py
--rw-r--r--   0        0        0     4257 2023-07-25 14:18:04.842493 spark_utils-1.1.2/spark_utils/common/functions.py
--rw-r--r--   0        0        0     5977 2023-07-25 14:18:04.842493 spark_utils-1.1.2/spark_utils/common/spark_job_args.py
--rw-r--r--   0        0        0    11709 2023-07-25 14:18:04.842493 spark_utils-1.1.2/spark_utils/common/spark_session_provider.py
--rw-r--r--   0        0        0     3381 2023-07-25 14:18:04.842493 spark_utils-1.1.2/spark_utils/common/spark_sql_utils.py
--rw-r--r--   0        0        0     1449 2023-07-25 14:18:04.842493 spark_utils-1.1.2/spark_utils/common/spark_udf.py
--rw-r--r--   0        0        0     1135 2023-07-25 14:18:04.842493 spark_utils-1.1.2/spark_utils/dataframes/__init__.py
--rw-r--r--   0        0        0    10376 2023-07-25 14:18:04.842493 spark_utils-1.1.2/spark_utils/dataframes/functions.py
--rw-r--r--   0        0        0     2325 2023-07-25 14:18:04.842493 spark_utils-1.1.2/spark_utils/dataframes/models.py
--rw-r--r--   0        0        0     1135 2023-07-25 14:18:04.842493 spark_utils-1.1.2/spark_utils/dataframes/sets/__init__.py
--rw-r--r--   0        0        0     1631 2023-07-25 14:18:04.842493 spark_utils-1.1.2/spark_utils/dataframes/sets/functions.py
--rw-r--r--   0        0        0     1135 2023-07-25 14:18:04.842493 spark_utils-1.1.2/spark_utils/delta_lake/__init__.py
--rw-r--r--   0        0        0     1691 2023-07-25 14:18:04.842493 spark_utils-1.1.2/spark_utils/delta_lake/delta_log.py
--rw-r--r--   0        0        0     5982 2023-07-25 14:18:04.842493 spark_utils-1.1.2/spark_utils/delta_lake/functions.py
--rw-r--r--   0        0        0     1135 2023-07-25 14:18:04.842493 spark_utils-1.1.2/spark_utils/models/__init__.py
--rw-r--r--   0        0        0     1641 2023-07-25 14:18:04.842493 spark_utils-1.1.2/spark_utils/models/hive_metastore_config.py
--rw-r--r--   0        0        0     1318 2023-07-25 14:18:04.842493 spark_utils-1.1.2/spark_utils/models/hive_table.py
--rw-r--r--   0        0        0     1868 2023-07-25 14:18:04.842493 spark_utils-1.1.2/spark_utils/models/job_socket.py
--rw-r--r--   0        0        0     1129 2023-07-25 14:18:04.842493 spark_utils-1.1.2/spark_utils/models/k8s_config.py
--rw-r--r--   0        0        0     7658 1970-01-01 00:00:00.000000 spark_utils-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-08-04 09:44:54.818581 spark_utils-1.1.3/LICENSE
+-rw-r--r--   0        0        0     6766 2023-08-04 09:44:54.818581 spark_utils-1.1.3/README.md
+-rw-r--r--   0        0        0      791 2023-08-04 09:45:18.579633 spark_utils-1.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1135 2023-08-04 09:44:54.822581 spark_utils-1.1.3/spark_utils/__init__.py
+-rw-r--r--   0        0        0       22 2023-08-04 09:45:18.579633 spark_utils-1.1.3/spark_utils/_version.py
+-rw-r--r--   0        0        0     1134 2023-08-04 09:44:54.822581 spark_utils-1.1.3/spark_utils/common/__init__.py
+-rw-r--r--   0        0        0     4257 2023-08-04 09:44:54.822581 spark_utils-1.1.3/spark_utils/common/functions.py
+-rw-r--r--   0        0        0     6347 2023-08-04 09:44:54.822581 spark_utils-1.1.3/spark_utils/common/spark_job_args.py
+-rw-r--r--   0        0        0    11709 2023-08-04 09:44:54.822581 spark_utils-1.1.3/spark_utils/common/spark_session_provider.py
+-rw-r--r--   0        0        0     3381 2023-08-04 09:44:54.822581 spark_utils-1.1.3/spark_utils/common/spark_sql_utils.py
+-rw-r--r--   0        0        0     1449 2023-08-04 09:44:54.822581 spark_utils-1.1.3/spark_utils/common/spark_udf.py
+-rw-r--r--   0        0        0     1135 2023-08-04 09:44:54.822581 spark_utils-1.1.3/spark_utils/dataframes/__init__.py
+-rw-r--r--   0        0        0    10376 2023-08-04 09:44:54.822581 spark_utils-1.1.3/spark_utils/dataframes/functions.py
+-rw-r--r--   0        0        0     2325 2023-08-04 09:44:54.822581 spark_utils-1.1.3/spark_utils/dataframes/models.py
+-rw-r--r--   0        0        0     1135 2023-08-04 09:44:54.822581 spark_utils-1.1.3/spark_utils/dataframes/sets/__init__.py
+-rw-r--r--   0        0        0     1631 2023-08-04 09:44:54.822581 spark_utils-1.1.3/spark_utils/dataframes/sets/functions.py
+-rw-r--r--   0        0        0     1135 2023-08-04 09:44:54.822581 spark_utils-1.1.3/spark_utils/delta_lake/__init__.py
+-rw-r--r--   0        0        0     1691 2023-08-04 09:44:54.822581 spark_utils-1.1.3/spark_utils/delta_lake/delta_log.py
+-rw-r--r--   0        0        0     5982 2023-08-04 09:44:54.822581 spark_utils-1.1.3/spark_utils/delta_lake/functions.py
+-rw-r--r--   0        0        0     1135 2023-08-04 09:44:54.822581 spark_utils-1.1.3/spark_utils/models/__init__.py
+-rw-r--r--   0        0        0     1641 2023-08-04 09:44:54.822581 spark_utils-1.1.3/spark_utils/models/hive_metastore_config.py
+-rw-r--r--   0        0        0     1318 2023-08-04 09:44:54.822581 spark_utils-1.1.3/spark_utils/models/hive_table.py
+-rw-r--r--   0        0        0     1868 2023-08-04 09:44:54.822581 spark_utils-1.1.3/spark_utils/models/job_socket.py
+-rw-r--r--   0        0        0     1129 2023-08-04 09:44:54.822581 spark_utils-1.1.3/spark_utils/models/k8s_config.py
+-rw-r--r--   0        0        0     7658 1970-01-01 00:00:00.000000 spark_utils-1.1.3/PKG-INFO
```

### Comparing `spark_utils-1.1.2/LICENSE` & `spark_utils-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `spark_utils-1.1.2/README.md` & `spark_utils-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `spark_utils-1.1.2/pyproject.toml` & `spark_utils-1.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "spark-utils"
-version = "1.1.2"
+version = "1.1.3"
 description = "Utility classes for comfy Spark job authoriing."
 authors = ["ECCO Sneaks & Data <esdsupport@ecco.com>"]
 maintainers = ['GZU <gzu@ecco.com>', 'JRB <ext-jrb@ecco.com>']
 license = 'MIT'
 readme = "README.md"
 repository = 'https://github.com/SneaksAndData/spark-utils'
```

### Comparing `spark_utils-1.1.2/spark_utils/__init__.py` & `spark_utils-1.1.3/spark_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `spark_utils-1.1.2/spark_utils/common/__init__.py` & `spark_utils-1.1.3/spark_utils/common/__init__.py`

 * *Files identical despite different names*

### Comparing `spark_utils-1.1.2/spark_utils/common/functions.py` & `spark_utils-1.1.3/spark_utils/common/functions.py`

 * *Files identical despite different names*

### Comparing `spark_utils-1.1.2/spark_utils/common/spark_job_args.py` & `spark_utils-1.1.3/spark_utils/common/spark_job_args.py`

 * *Files 3% similar despite different names*

```diff
@@ -94,14 +94,30 @@
         for source in self._parsed_args.source:
             yield JobSocket(*source.split("|"))
 
     def _outputs(self) -> Iterable[JobSocket]:
         for output in self._parsed_args.output:
             yield JobSocket(*output.split("|"))
 
+    @property
+    def sources(self) -> Iterable[JobSocket]:
+        """
+        Returns parsed sources
+        """
+        for source in self._parsed_sources:
+            yield source
+
+    @property
+    def outputs(self) -> Iterable[JobSocket]:
+        """
+        Returns parsed outputs
+        """
+        for output in self._parsed_outputs:
+            yield output
+
     def new_arg(self, *args, **kwargs):
         """
         Adds one or more new arguments
         :param args: argsparse.add_argument(...)
         :return:
         """
         self._parser.add_argument(*args, **kwargs)
```

### Comparing `spark_utils-1.1.2/spark_utils/common/spark_session_provider.py` & `spark_utils-1.1.3/spark_utils/common/spark_session_provider.py`

 * *Files identical despite different names*

### Comparing `spark_utils-1.1.2/spark_utils/common/spark_sql_utils.py` & `spark_utils-1.1.3/spark_utils/common/spark_sql_utils.py`

 * *Files identical despite different names*

### Comparing `spark_utils-1.1.2/spark_utils/common/spark_udf.py` & `spark_utils-1.1.3/spark_utils/common/spark_udf.py`

 * *Files identical despite different names*

### Comparing `spark_utils-1.1.2/spark_utils/dataframes/__init__.py` & `spark_utils-1.1.3/spark_utils/dataframes/__init__.py`

 * *Files identical despite different names*

### Comparing `spark_utils-1.1.2/spark_utils/dataframes/functions.py` & `spark_utils-1.1.3/spark_utils/dataframes/functions.py`

 * *Files identical despite different names*

### Comparing `spark_utils-1.1.2/spark_utils/dataframes/models.py` & `spark_utils-1.1.3/spark_utils/dataframes/models.py`

 * *Files identical despite different names*

### Comparing `spark_utils-1.1.2/spark_utils/dataframes/sets/__init__.py` & `spark_utils-1.1.3/spark_utils/dataframes/sets/__init__.py`

 * *Files identical despite different names*

### Comparing `spark_utils-1.1.2/spark_utils/dataframes/sets/functions.py` & `spark_utils-1.1.3/spark_utils/dataframes/sets/functions.py`

 * *Files identical despite different names*

### Comparing `spark_utils-1.1.2/spark_utils/delta_lake/__init__.py` & `spark_utils-1.1.3/spark_utils/delta_lake/__init__.py`

 * *Files identical despite different names*

### Comparing `spark_utils-1.1.2/spark_utils/delta_lake/delta_log.py` & `spark_utils-1.1.3/spark_utils/delta_lake/delta_log.py`

 * *Files identical despite different names*

### Comparing `spark_utils-1.1.2/spark_utils/delta_lake/functions.py` & `spark_utils-1.1.3/spark_utils/delta_lake/functions.py`

 * *Files identical despite different names*

### Comparing `spark_utils-1.1.2/spark_utils/models/__init__.py` & `spark_utils-1.1.3/spark_utils/models/__init__.py`

 * *Files identical despite different names*

### Comparing `spark_utils-1.1.2/spark_utils/models/hive_metastore_config.py` & `spark_utils-1.1.3/spark_utils/models/hive_metastore_config.py`

 * *Files identical despite different names*

### Comparing `spark_utils-1.1.2/spark_utils/models/hive_table.py` & `spark_utils-1.1.3/spark_utils/models/hive_table.py`

 * *Files identical despite different names*

### Comparing `spark_utils-1.1.2/spark_utils/models/job_socket.py` & `spark_utils-1.1.3/spark_utils/models/job_socket.py`

 * *Files identical despite different names*

### Comparing `spark_utils-1.1.2/spark_utils/models/k8s_config.py` & `spark_utils-1.1.3/spark_utils/models/k8s_config.py`

 * *Files identical despite different names*

### Comparing `spark_utils-1.1.2/PKG-INFO` & `spark_utils-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spark-utils
-Version: 1.1.2
+Version: 1.1.3
 Summary: Utility classes for comfy Spark job authoriing.
 Home-page: https://github.com/SneaksAndData/spark-utils
 License: MIT
 Author: ECCO Sneaks & Data
 Author-email: esdsupport@ecco.com
 Maintainer: GZU
 Maintainer-email: gzu@ecco.com
```

