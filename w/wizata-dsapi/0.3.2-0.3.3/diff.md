# Comparing `tmp/wizata-dsapi-0.3.2.tar.gz` & `tmp/wizata-dsapi-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wizata-dsapi-0.3.2.tar", last modified: Fri Aug  4 12:44:56 2023, max compression
+gzip compressed data, was "wizata-dsapi-0.3.3.tar", last modified: Fri Aug  4 13:45:33 2023, max compression
```

## Comparing `wizata-dsapi-0.3.2.tar` & `wizata-dsapi-0.3.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 wizata.jph   (502) staff       (20)        0 2023-08-04 12:44:56.205997 wizata-dsapi-0.3.2/
--rw-r--r--   0 wizata.jph   (502) staff       (20)    11356 2023-07-20 17:32:08.000000 wizata-dsapi-0.3.2/LICENSE.txt
--rw-r--r--   0 wizata.jph   (502) staff       (20)      169 2023-08-04 12:44:56.205883 wizata-dsapi-0.3.2/PKG-INFO
--rw-r--r--   0 wizata.jph   (502) staff       (20)      315 2023-07-20 17:32:08.000000 wizata-dsapi-0.3.2/README.rst
--rw-r--r--   0 wizata.jph   (502) staff       (20)       38 2023-08-04 12:44:56.206038 wizata-dsapi-0.3.2/setup.cfg
--rw-r--r--   0 wizata.jph   (502) staff       (20)     1203 2023-08-04 12:44:52.000000 wizata-dsapi-0.3.2/setup.py
-drwxr-xr-x   0 wizata.jph   (502) staff       (20)        0 2023-08-04 12:44:56.204827 wizata-dsapi-0.3.2/wizata_dsapi/
--rw-r--r--   0 wizata.jph   (502) staff       (20)     1029 2023-08-04 10:57:55.000000 wizata-dsapi-0.3.2/wizata_dsapi/__init__.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)      605 2023-07-20 17:32:08.000000 wizata-dsapi-0.3.2/wizata_dsapi/api_dto.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)     5173 2023-08-04 12:44:52.000000 wizata-dsapi-0.3.2/wizata_dsapi/context.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)     5588 2023-07-20 17:32:08.000000 wizata-dsapi-0.3.2/wizata_dsapi/dataframe_toolkit.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)     5933 2023-07-20 17:32:08.000000 wizata-dsapi-0.3.2/wizata_dsapi/datapoint.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)     1815 2023-07-20 17:32:08.000000 wizata-dsapi-0.3.2/wizata_dsapi/ds_dataframe.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)     2772 2023-07-20 17:32:08.000000 wizata-dsapi-0.3.2/wizata_dsapi/dsapi_json_encoder.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)    14533 2023-08-04 10:57:55.000000 wizata-dsapi-0.3.2/wizata_dsapi/execution.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)     3711 2023-07-20 17:32:08.000000 wizata-dsapi-0.3.2/wizata_dsapi/experiment.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)    10306 2023-08-02 08:42:21.000000 wizata-dsapi-0.3.2/wizata_dsapi/mlmodel.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)     1552 2023-07-20 17:32:08.000000 wizata-dsapi-0.3.2/wizata_dsapi/model_toolkit.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)    18380 2023-08-02 08:42:21.000000 wizata-dsapi-0.3.2/wizata_dsapi/pipeline.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)     2067 2023-07-20 17:32:08.000000 wizata-dsapi-0.3.2/wizata_dsapi/plot.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)    17759 2023-07-20 17:32:08.000000 wizata-dsapi-0.3.2/wizata_dsapi/request.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)     8485 2023-07-20 17:32:08.000000 wizata-dsapi-0.3.2/wizata_dsapi/script.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)     7110 2023-07-31 10:14:43.000000 wizata-dsapi-0.3.2/wizata_dsapi/template.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)     2517 2023-07-20 17:32:08.000000 wizata-dsapi-0.3.2/wizata_dsapi/twin.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)     4675 2023-08-02 08:42:21.000000 wizata-dsapi-0.3.2/wizata_dsapi/twinregistration.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)      471 2023-07-20 17:32:08.000000 wizata-dsapi-0.3.2/wizata_dsapi/wizard_function.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)    57650 2023-07-31 10:14:43.000000 wizata-dsapi-0.3.2/wizata_dsapi/wizata_dsapi_client.py
-drwxr-xr-x   0 wizata.jph   (502) staff       (20)        0 2023-08-04 12:44:56.205699 wizata-dsapi-0.3.2/wizata_dsapi.egg-info/
--rw-r--r--   0 wizata.jph   (502) staff       (20)      169 2023-08-04 12:44:56.000000 wizata-dsapi-0.3.2/wizata_dsapi.egg-info/PKG-INFO
--rw-r--r--   0 wizata.jph   (502) staff       (20)      754 2023-08-04 12:44:56.000000 wizata-dsapi-0.3.2/wizata_dsapi.egg-info/SOURCES.txt
--rw-r--r--   0 wizata.jph   (502) staff       (20)        1 2023-08-04 12:44:56.000000 wizata-dsapi-0.3.2/wizata_dsapi.egg-info/dependency_links.txt
--rw-r--r--   0 wizata.jph   (502) staff       (20)      555 2023-08-04 12:44:56.000000 wizata-dsapi-0.3.2/wizata_dsapi.egg-info/requires.txt
--rw-r--r--   0 wizata.jph   (502) staff       (20)       13 2023-08-04 12:44:56.000000 wizata-dsapi-0.3.2/wizata_dsapi.egg-info/top_level.txt
+drwxr-xr-x   0 wizata.jph   (502) staff       (20)        0 2023-08-04 13:45:33.706030 wizata-dsapi-0.3.3/
+-rw-r--r--   0 wizata.jph   (502) staff       (20)    11356 2023-07-20 17:32:08.000000 wizata-dsapi-0.3.3/LICENSE.txt
+-rw-r--r--   0 wizata.jph   (502) staff       (20)      169 2023-08-04 13:45:33.705913 wizata-dsapi-0.3.3/PKG-INFO
+-rw-r--r--   0 wizata.jph   (502) staff       (20)      315 2023-07-20 17:32:08.000000 wizata-dsapi-0.3.3/README.rst
+-rw-r--r--   0 wizata.jph   (502) staff       (20)       38 2023-08-04 13:45:33.706071 wizata-dsapi-0.3.3/setup.cfg
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     1203 2023-08-04 13:45:28.000000 wizata-dsapi-0.3.3/setup.py
+drwxr-xr-x   0 wizata.jph   (502) staff       (20)        0 2023-08-04 13:45:33.704642 wizata-dsapi-0.3.3/wizata_dsapi/
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     1029 2023-08-04 10:57:55.000000 wizata-dsapi-0.3.3/wizata_dsapi/__init__.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)      605 2023-07-20 17:32:08.000000 wizata-dsapi-0.3.3/wizata_dsapi/api_dto.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     5172 2023-08-04 13:45:28.000000 wizata-dsapi-0.3.3/wizata_dsapi/context.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     5588 2023-07-20 17:32:08.000000 wizata-dsapi-0.3.3/wizata_dsapi/dataframe_toolkit.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     5933 2023-07-20 17:32:08.000000 wizata-dsapi-0.3.3/wizata_dsapi/datapoint.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     1815 2023-07-20 17:32:08.000000 wizata-dsapi-0.3.3/wizata_dsapi/ds_dataframe.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     2772 2023-07-20 17:32:08.000000 wizata-dsapi-0.3.3/wizata_dsapi/dsapi_json_encoder.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)    14533 2023-08-04 10:57:55.000000 wizata-dsapi-0.3.3/wizata_dsapi/execution.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     3711 2023-07-20 17:32:08.000000 wizata-dsapi-0.3.3/wizata_dsapi/experiment.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)    10306 2023-08-02 08:42:21.000000 wizata-dsapi-0.3.3/wizata_dsapi/mlmodel.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     1552 2023-07-20 17:32:08.000000 wizata-dsapi-0.3.3/wizata_dsapi/model_toolkit.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)    18380 2023-08-02 08:42:21.000000 wizata-dsapi-0.3.3/wizata_dsapi/pipeline.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     2067 2023-07-20 17:32:08.000000 wizata-dsapi-0.3.3/wizata_dsapi/plot.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)    17759 2023-07-20 17:32:08.000000 wizata-dsapi-0.3.3/wizata_dsapi/request.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     8485 2023-07-20 17:32:08.000000 wizata-dsapi-0.3.3/wizata_dsapi/script.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     7110 2023-07-31 10:14:43.000000 wizata-dsapi-0.3.3/wizata_dsapi/template.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     2517 2023-07-20 17:32:08.000000 wizata-dsapi-0.3.3/wizata_dsapi/twin.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     4675 2023-08-02 08:42:21.000000 wizata-dsapi-0.3.3/wizata_dsapi/twinregistration.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)      471 2023-07-20 17:32:08.000000 wizata-dsapi-0.3.3/wizata_dsapi/wizard_function.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)    57650 2023-07-31 10:14:43.000000 wizata-dsapi-0.3.3/wizata_dsapi/wizata_dsapi_client.py
+drwxr-xr-x   0 wizata.jph   (502) staff       (20)        0 2023-08-04 13:45:33.705743 wizata-dsapi-0.3.3/wizata_dsapi.egg-info/
+-rw-r--r--   0 wizata.jph   (502) staff       (20)      169 2023-08-04 13:45:33.000000 wizata-dsapi-0.3.3/wizata_dsapi.egg-info/PKG-INFO
+-rw-r--r--   0 wizata.jph   (502) staff       (20)      754 2023-08-04 13:45:33.000000 wizata-dsapi-0.3.3/wizata_dsapi.egg-info/SOURCES.txt
+-rw-r--r--   0 wizata.jph   (502) staff       (20)        1 2023-08-04 13:45:33.000000 wizata-dsapi-0.3.3/wizata_dsapi.egg-info/dependency_links.txt
+-rw-r--r--   0 wizata.jph   (502) staff       (20)      555 2023-08-04 13:45:33.000000 wizata-dsapi-0.3.3/wizata_dsapi.egg-info/requires.txt
+-rw-r--r--   0 wizata.jph   (502) staff       (20)       13 2023-08-04 13:45:33.000000 wizata-dsapi-0.3.3/wizata_dsapi.egg-info/top_level.txt
```

### Comparing `wizata-dsapi-0.3.2/LICENSE.txt` & `wizata-dsapi-0.3.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.3.2/setup.py` & `wizata-dsapi-0.3.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='wizata-dsapi',
-    version='0.3.2',
+    version='0.3.3',
     description='Wizata Data Science Toolkit',
     author='Wizata S.A.',
     author_email='info@wizata.com',
     packages=['wizata_dsapi'],
     install_requires=[
         'dill==0.3.6',
         'pandas==1.5.3',
```

### Comparing `wizata-dsapi-0.3.2/wizata_dsapi/__init__.py` & `wizata-dsapi-0.3.3/wizata_dsapi/__init__.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.3.2/wizata_dsapi/api_dto.py` & `wizata-dsapi-0.3.3/wizata_dsapi/api_dto.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.3.2/wizata_dsapi/context.py` & `wizata-dsapi-0.3.3/wizata_dsapi/context.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,33 +20,34 @@
         self.models = {}
         self.dataframes = {}
         self.properties = {}
         self.plots = {}
 
         self.__key_mapping = None
         self.__primary_key = None
+        self.__temporary_dataframe = None
 
         self.__new_plot = None
         self.__new_model = None
 
     @property
     def dataframe(self):
         if self.__primary_key is not None and self.__key_mapping is not None and self.__primary_key in self.__key_mapping and self.__key_mapping[self.__primary_key] in self.dataframes:
             return self.dataframes[self.__key_mapping[self.__primary_key]]
-        elif len(self.dataframes) > 0:
-            first_key = list(self.dataframes.keys())[0]
-            return self.dataframes[first_key]
+        elif self.__temporary_dataframe is not None:
+            return self.__temporary_dataframe
+        else:
+            return None
 
     @dataframe.setter
     def dataframe(self, df: pandas.DataFrame):
         if self.__primary_key is not None and self.__key_mapping is not None and self.__primary_key in self.__key_mapping and self.__key_mapping[self.__primary_key] in self.dataframes:
             self.dataframes[self.__key_mapping[self.__primary_key]] = df
-        elif len(self.dataframes) > 0:
-            first_key = list(self.dataframes.keys())[0]
-            self.dataframes[first_key] = df
+        else:
+            self.__temporary_dataframe = df
 
     def append(self, key: str, obj, overwrite: bool = True):
         """
         append an object (pandas.Dataframe or any properties)
         :param key: dictionary identifier - name inside your pipeline.
         :param obj: ML Model, Dataframe or any properties (must be JSON serializable type).
         :param overwrite: by default - allow modifying an existing object. can be set to false.
@@ -127,14 +128,15 @@
         """
         reset context between step execution - remove all step info, but keep all data.
         """
         self.__new_plot = None
         self.__new_model = None
         self.__key_mapping = None
         self.__primary_key = None
+        self.__temporary_dataframe = None
 
     def _set_mapping(self, key_mapping: dict, primary_key: str):
         """
         set step mapping between pipeline names and step name
         """
         self.__key_mapping = key_mapping
         self.__primary_key = primary_key
```

### Comparing `wizata-dsapi-0.3.2/wizata_dsapi/dataframe_toolkit.py` & `wizata-dsapi-0.3.3/wizata_dsapi/dataframe_toolkit.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.3.2/wizata_dsapi/datapoint.py` & `wizata-dsapi-0.3.3/wizata_dsapi/datapoint.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.3.2/wizata_dsapi/ds_dataframe.py` & `wizata-dsapi-0.3.3/wizata_dsapi/ds_dataframe.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.3.2/wizata_dsapi/dsapi_json_encoder.py` & `wizata-dsapi-0.3.3/wizata_dsapi/dsapi_json_encoder.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.3.2/wizata_dsapi/execution.py` & `wizata-dsapi-0.3.3/wizata_dsapi/execution.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.3.2/wizata_dsapi/experiment.py` & `wizata-dsapi-0.3.3/wizata_dsapi/experiment.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.3.2/wizata_dsapi/mlmodel.py` & `wizata-dsapi-0.3.3/wizata_dsapi/mlmodel.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.3.2/wizata_dsapi/model_toolkit.py` & `wizata-dsapi-0.3.3/wizata_dsapi/model_toolkit.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.3.2/wizata_dsapi/pipeline.py` & `wizata-dsapi-0.3.3/wizata_dsapi/pipeline.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.3.2/wizata_dsapi/plot.py` & `wizata-dsapi-0.3.3/wizata_dsapi/plot.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.3.2/wizata_dsapi/request.py` & `wizata-dsapi-0.3.3/wizata_dsapi/request.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.3.2/wizata_dsapi/script.py` & `wizata-dsapi-0.3.3/wizata_dsapi/script.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.3.2/wizata_dsapi/template.py` & `wizata-dsapi-0.3.3/wizata_dsapi/template.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.3.2/wizata_dsapi/twin.py` & `wizata-dsapi-0.3.3/wizata_dsapi/twin.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.3.2/wizata_dsapi/twinregistration.py` & `wizata-dsapi-0.3.3/wizata_dsapi/twinregistration.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.3.2/wizata_dsapi/wizata_dsapi_client.py` & `wizata-dsapi-0.3.3/wizata_dsapi/wizata_dsapi_client.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.3.2/wizata_dsapi.egg-info/SOURCES.txt` & `wizata-dsapi-0.3.3/wizata_dsapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.3.2/wizata_dsapi.egg-info/requires.txt` & `wizata-dsapi-0.3.3/wizata_dsapi.egg-info/requires.txt`

 * *Files identical despite different names*

