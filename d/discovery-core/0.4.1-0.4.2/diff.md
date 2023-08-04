# Comparing `tmp/discovery-core-0.4.1.tar.gz` & `tmp/discovery-core-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discovery-core-0.4.1.tar", last modified: Wed Aug  2 16:53:42 2023, max compression
+gzip compressed data, was "discovery-core-0.4.2.tar", last modified: Fri Aug  4 20:25:59 2023, max compression
```

## Comparing `discovery-core-0.4.1.tar` & `discovery-core-0.4.2.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-02 16:53:42.092922 discovery-core-0.4.1/
--rwxr-xr-x   0 doatridge   (503) staff       (20)     1087 2023-06-28 23:35:32.000000 discovery-core-0.4.1/LICENSE.txt
--rwxr-xr-x   0 doatridge   (503) staff       (20)       65 2023-06-28 23:35:32.000000 discovery-core-0.4.1/MANIFEST.in
--rw-r--r--   0 doatridge   (503) staff       (20)    14094 2023-08-02 16:53:42.093353 discovery-core-0.4.1/PKG-INFO
--rw-r--r--   0 doatridge   (503) staff       (20)    13130 2023-06-28 23:35:32.000000 discovery-core-0.4.1/README.rst
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-02 16:53:42.070923 discovery-core-0.4.1/discovery_core.egg-info/
--rw-r--r--   0 doatridge   (503) staff       (20)    14094 2023-08-02 16:53:41.000000 discovery-core-0.4.1/discovery_core.egg-info/PKG-INFO
--rw-r--r--   0 doatridge   (503) staff       (20)     1092 2023-08-02 16:53:42.000000 discovery-core-0.4.1/discovery_core.egg-info/SOURCES.txt
--rw-r--r--   0 doatridge   (503) staff       (20)        1 2023-08-02 16:53:41.000000 discovery-core-0.4.1/discovery_core.egg-info/dependency_links.txt
--rw-r--r--   0 doatridge   (503) staff       (20)       13 2023-08-02 16:53:41.000000 discovery-core-0.4.1/discovery_core.egg-info/top_level.txt
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-02 16:53:42.071259 discovery-core-0.4.1/ds_core/
--rw-r--r--   0 doatridge   (503) staff       (20)       73 2023-08-02 16:53:22.000000 discovery-core-0.4.1/ds_core/__init__.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-02 16:53:42.073087 discovery-core-0.4.1/ds_core/components/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.4.1/ds_core/components/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)    63432 2023-08-02 16:51:55.000000 discovery-core-0.4.1/ds_core/components/abstract_component.py
--rw-r--r--   0 doatridge   (503) staff       (20)    25922 2023-08-01 22:47:24.000000 discovery-core-0.4.1/ds_core/components/core_commons.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-02 16:53:42.075191 discovery-core-0.4.1/ds_core/handlers/
--rwxr-xr-x   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.4.1/ds_core/handlers/__init__.py
--rwxr-xr-x   0 doatridge   (503) staff       (20)    15258 2023-05-02 21:09:52.000000 discovery-core-0.4.1/ds_core/handlers/abstract_handlers.py
--rw-r--r--   0 doatridge   (503) staff       (20)     8143 2023-07-17 17:55:59.000000 discovery-core-0.4.1/ds_core/handlers/pyarrow_handlers.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-02 16:53:42.076175 discovery-core-0.4.1/ds_core/intent/
--rwxr-xr-x   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.4.1/ds_core/intent/__init__.py
--rwxr-xr-x   0 doatridge   (503) staff       (20)    11255 2023-06-29 15:15:01.000000 discovery-core-0.4.1/ds_core/intent/abstract_intent.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-02 16:53:42.079167 discovery-core-0.4.1/ds_core/properties/
--rwxr-xr-x   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.4.1/ds_core/properties/__init__.py
--rwxr-xr-x   0 doatridge   (503) staff       (20)    65710 2023-06-29 23:15:54.000000 discovery-core-0.4.1/ds_core/properties/abstract_properties.py
--rwxr-xr-x   0 doatridge   (503) staff       (20)     2996 2022-09-22 17:31:08.000000 discovery-core-0.4.1/ds_core/properties/decorator_patterns.py
--rw-r--r--   0 doatridge   (503) staff       (20)    11271 2023-06-29 15:15:01.000000 discovery-core-0.4.1/ds_core/properties/property_manager.py
--rwxr-xr-x   0 doatridge   (503) staff       (20)      110 2023-08-02 16:53:42.094467 discovery-core-0.4.1/setup.cfg
--rwxr-xr-x   0 doatridge   (503) staff       (20)     2085 2023-07-03 17:06:43.000000 discovery-core-0.4.1/setup.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-02 16:53:42.080159 discovery-core-0.4.1/test/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-06-29 15:06:28.000000 discovery-core-0.4.1/test/__init__.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-02 16:53:42.082672 discovery-core-0.4.1/test/components/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.4.1/test/components/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)    31457 2023-08-01 20:07:50.000000 discovery-core-0.4.1/test/components/abstract_component_test.py
--rw-r--r--   0 doatridge   (503) staff       (20)    20699 2023-08-01 22:48:11.000000 discovery-core-0.4.1/test/components/commons_test.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-02 16:53:42.085876 discovery-core-0.4.1/test/handlers/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.4.1/test/handlers/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)    11054 2023-06-29 16:24:13.000000 discovery-core-0.4.1/test/handlers/connector_contract_test.py
--rw-r--r--   0 doatridge   (503) staff       (20)     2560 2023-06-29 16:24:13.000000 discovery-core-0.4.1/test/handlers/handler_factory_test.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-02 16:53:42.088615 discovery-core-0.4.1/test/intent/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.4.1/test/intent/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)     2899 2023-07-12 16:01:36.000000 discovery-core-0.4.1/test/intent/abstract_intent_test.py
--rw-r--r--   0 doatridge   (503) staff       (20)     7100 2023-07-12 17:46:55.000000 discovery-core-0.4.1/test/intent/pyarrow_intent_model.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-02 16:53:42.091931 discovery-core-0.4.1/test/properties/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.4.1/test/properties/__init__.py
--rwxr-xr-x   0 doatridge   (503) staff       (20)    36169 2023-06-29 23:15:54.000000 discovery-core-0.4.1/test/properties/abstract_properties_manager_test.py
--rwxr-xr-x   0 doatridge   (503) staff       (20)     9513 2023-06-29 16:47:52.000000 discovery-core-0.4.1/test/properties/property_manager_test.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-04 20:25:59.025672 discovery-core-0.4.2/
+-rwxr-xr-x   0 doatridge   (503) staff       (20)     1087 2023-06-28 23:35:32.000000 discovery-core-0.4.2/LICENSE.txt
+-rwxr-xr-x   0 doatridge   (503) staff       (20)       65 2023-06-28 23:35:32.000000 discovery-core-0.4.2/MANIFEST.in
+-rw-r--r--   0 doatridge   (503) staff       (20)    14094 2023-08-04 20:25:59.025864 discovery-core-0.4.2/PKG-INFO
+-rw-r--r--   0 doatridge   (503) staff       (20)    13130 2023-06-28 23:35:32.000000 discovery-core-0.4.2/README.rst
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-04 20:25:59.015284 discovery-core-0.4.2/discovery_core.egg-info/
+-rw-r--r--   0 doatridge   (503) staff       (20)    14094 2023-08-04 20:25:58.000000 discovery-core-0.4.2/discovery_core.egg-info/PKG-INFO
+-rw-r--r--   0 doatridge   (503) staff       (20)     1092 2023-08-04 20:25:58.000000 discovery-core-0.4.2/discovery_core.egg-info/SOURCES.txt
+-rw-r--r--   0 doatridge   (503) staff       (20)        1 2023-08-04 20:25:58.000000 discovery-core-0.4.2/discovery_core.egg-info/dependency_links.txt
+-rw-r--r--   0 doatridge   (503) staff       (20)       13 2023-08-04 20:25:58.000000 discovery-core-0.4.2/discovery_core.egg-info/top_level.txt
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-04 20:25:59.015644 discovery-core-0.4.2/ds_core/
+-rw-r--r--   0 doatridge   (503) staff       (20)       73 2023-08-02 16:54:47.000000 discovery-core-0.4.2/ds_core/__init__.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-04 20:25:59.016866 discovery-core-0.4.2/ds_core/components/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.4.2/ds_core/components/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    63432 2023-08-02 16:51:55.000000 discovery-core-0.4.2/ds_core/components/abstract_component.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    26586 2023-08-04 18:24:32.000000 discovery-core-0.4.2/ds_core/components/core_commons.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-04 20:25:59.018172 discovery-core-0.4.2/ds_core/handlers/
+-rwxr-xr-x   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.4.2/ds_core/handlers/__init__.py
+-rwxr-xr-x   0 doatridge   (503) staff       (20)    15258 2023-05-02 21:09:52.000000 discovery-core-0.4.2/ds_core/handlers/abstract_handlers.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     8143 2023-07-17 17:55:59.000000 discovery-core-0.4.2/ds_core/handlers/pyarrow_handlers.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-04 20:25:59.018815 discovery-core-0.4.2/ds_core/intent/
+-rwxr-xr-x   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.4.2/ds_core/intent/__init__.py
+-rwxr-xr-x   0 doatridge   (503) staff       (20)    11255 2023-06-29 15:15:01.000000 discovery-core-0.4.2/ds_core/intent/abstract_intent.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-04 20:25:59.020616 discovery-core-0.4.2/ds_core/properties/
+-rwxr-xr-x   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.4.2/ds_core/properties/__init__.py
+-rwxr-xr-x   0 doatridge   (503) staff       (20)    65710 2023-06-29 23:15:54.000000 discovery-core-0.4.2/ds_core/properties/abstract_properties.py
+-rwxr-xr-x   0 doatridge   (503) staff       (20)     2996 2022-09-22 17:31:08.000000 discovery-core-0.4.2/ds_core/properties/decorator_patterns.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    11271 2023-06-29 15:15:01.000000 discovery-core-0.4.2/ds_core/properties/property_manager.py
+-rwxr-xr-x   0 doatridge   (503) staff       (20)      110 2023-08-04 20:25:59.026448 discovery-core-0.4.2/setup.cfg
+-rwxr-xr-x   0 doatridge   (503) staff       (20)     2085 2023-07-03 17:06:43.000000 discovery-core-0.4.2/setup.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-04 20:25:59.020976 discovery-core-0.4.2/test/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-06-29 15:06:28.000000 discovery-core-0.4.2/test/__init__.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-04 20:25:59.022114 discovery-core-0.4.2/test/components/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.4.2/test/components/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    31457 2023-08-01 20:07:50.000000 discovery-core-0.4.2/test/components/abstract_component_test.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    21160 2023-08-04 18:29:25.000000 discovery-core-0.4.2/test/components/commons_test.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-04 20:25:59.023163 discovery-core-0.4.2/test/handlers/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.4.2/test/handlers/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    11054 2023-06-29 16:24:13.000000 discovery-core-0.4.2/test/handlers/connector_contract_test.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     2560 2023-06-29 16:24:13.000000 discovery-core-0.4.2/test/handlers/handler_factory_test.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-04 20:25:59.024306 discovery-core-0.4.2/test/intent/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.4.2/test/intent/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     2899 2023-07-12 16:01:36.000000 discovery-core-0.4.2/test/intent/abstract_intent_test.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     7100 2023-07-12 17:46:55.000000 discovery-core-0.4.2/test/intent/pyarrow_intent_model.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-04 20:25:59.025372 discovery-core-0.4.2/test/properties/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.4.2/test/properties/__init__.py
+-rwxr-xr-x   0 doatridge   (503) staff       (20)    36169 2023-06-29 23:15:54.000000 discovery-core-0.4.2/test/properties/abstract_properties_manager_test.py
+-rwxr-xr-x   0 doatridge   (503) staff       (20)     9513 2023-06-29 16:47:52.000000 discovery-core-0.4.2/test/properties/property_manager_test.py
```

### Comparing `discovery-core-0.4.1/LICENSE.txt` & `discovery-core-0.4.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `discovery-core-0.4.1/PKG-INFO` & `discovery-core-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discovery-core
-Version: 0.4.1
+Version: 0.4.2
 Summary: Augmented Intent Single Task Adaptive Components
 Home-page: http://github.com/gigas64/discovery-core
 Author: Gigas64
 Author-email: gigas64@opengrass.net
 License: BSD
 Keywords: Foundation SDK Machine learning AI component intent data science
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `discovery-core-0.4.1/README.rst` & `discovery-core-0.4.2/README.rst`

 * *Files identical despite different names*

### Comparing `discovery-core-0.4.1/discovery_core.egg-info/PKG-INFO` & `discovery-core-0.4.2/discovery_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discovery-core
-Version: 0.4.1
+Version: 0.4.2
 Summary: Augmented Intent Single Task Adaptive Components
 Home-page: http://github.com/gigas64/discovery-core
 Author: Gigas64
 Author-email: gigas64@opengrass.net
 License: BSD
 Keywords: Foundation SDK Machine learning AI component intent data science
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `discovery-core-0.4.1/discovery_core.egg-info/SOURCES.txt` & `discovery-core-0.4.2/discovery_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `discovery-core-0.4.1/ds_core/components/abstract_component.py` & `discovery-core-0.4.2/ds_core/components/abstract_component.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.4.1/ds_core/components/core_commons.py` & `discovery-core-0.4.2/ds_core/components/core_commons.py`

 * *Files 2% similar despite different names*

```diff
@@ -195,14 +195,30 @@
                 rtn_counter[rtn_counter.index(max(rtn_counter))] -= 1
         rtn_seq = []
         for i in range(len(seq)):
             rtn_seq += [seq[i]] * rtn_counter[i]
         return rtn_seq
 
     @staticmethod
+    def list_search(seq: list, value: [int,float,str], low: int=None, high: int=None):
+        """ A binary search for a value in a list sequence between two index"""
+        low = low if isinstance(low, int) else 0
+        high = high if isinstance(high, int) else len(seq)
+        if high >= low:
+            mid = int((high + low) / 2)
+            if seq[mid] == value:
+                return mid
+            elif seq[mid] > value:
+                return CoreCommons.list_search(seq, value, low, mid - 1)
+            else:
+                return CoreCommons.list_search(seq, value, mid + 1, high)
+        else:
+            return -1
+
+    @staticmethod
     def list_standardize(seq: list, precision: int=None) -> list:
         """standardise a numeric list"""
         if not isinstance(seq, list):
             raise ValueError("The sequence must be of type 'list'")
         if not all(isinstance(x, (int, float)) for x in seq):
             raise ValueError("The sequence must be a list of numeric values")
         precision = precision if isinstance(precision, int) else 5
@@ -270,15 +286,15 @@
 
         :param data: the Canonical data to get the column headers from
         :param d_types: (optional) a list of pyarrow DataTypes of the columns headers
         :param headers: (optional) a list of header strings to select from the columns headers
         :param regex: (optional) a regular expression to search from the columns headers
         :param drop: (optional) reverses the selection and drops the selected column headers
         :return: a filtered list of headers
-        :return:
+        :return: pa.Table
         """
         return data.select(CoreCommons.filter_headers(data=data, headers=headers, d_types=d_types, regex=regex,
                                                       drop=drop))
 
     @staticmethod
     def table_append(t1: pa.Table, t2: pa.Table):
         """ appends all the columns in t2 to t1 """
```

### Comparing `discovery-core-0.4.1/ds_core/handlers/abstract_handlers.py` & `discovery-core-0.4.2/ds_core/handlers/abstract_handlers.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.4.1/ds_core/handlers/pyarrow_handlers.py` & `discovery-core-0.4.2/ds_core/handlers/pyarrow_handlers.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.4.1/ds_core/intent/abstract_intent.py` & `discovery-core-0.4.2/ds_core/intent/abstract_intent.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.4.1/ds_core/properties/abstract_properties.py` & `discovery-core-0.4.2/ds_core/properties/abstract_properties.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.4.1/ds_core/properties/decorator_patterns.py` & `discovery-core-0.4.2/ds_core/properties/decorator_patterns.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.4.1/ds_core/properties/property_manager.py` & `discovery-core-0.4.2/ds_core/properties/property_manager.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.4.1/setup.py` & `discovery-core-0.4.2/setup.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.4.1/test/components/abstract_component_test.py` & `discovery-core-0.4.2/test/components/abstract_component_test.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.4.1/test/components/commons_test.py` & `discovery-core-0.4.2/test/components/commons_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -195,14 +195,16 @@
         result = CoreCommons.filter_headers(tbl, headers=['num','int','string'], d_types=[pa.bool_(), pa.string()])
         self.assertCountEqual(['string'], result)
 
     def test_filter_columns(self):
         tbl = pq.read_table("../_data/sample_types.parquet")
         result = CoreCommons.filter_columns(tbl, headers=['num', 'date', 'string'], regex='t', d_types=[pa.string()])
         self.assertCountEqual(['string'], result.column_names)
+        result = CoreCommons.filter_columns(tbl, headers='num')
+        self.assertCountEqual(['num'], result.column_names)
 
     def test_list_formatter(self):
         sample = {'A': [1,2], 'B': [1,2], 'C': [1,2]}
         result = CoreCommons.list_formatter(sample)
         self.assertEqual(list("ABC"), result)
         result = CoreCommons.list_formatter(sample.keys())
         self.assertEqual(list("ABC"), result)
@@ -221,23 +223,31 @@
         sample = 2784.45612367432
         self.assertEqual((14, 10), CoreCommons.precision_scale(sample))
         sample = -3.72
         self.assertEqual((3, 2), CoreCommons.precision_scale(sample))
         sample = -4
         self.assertEqual((1, 0), CoreCommons.precision_scale(sample))
 
-
     def test_list_dup(self):
         seq = ['A', 'B', 'B', 'C', 'C', 'D']
         result = CoreCommons.list_dup(seq=seq)
         self.assertCountEqual(['B', 'C'], result)
         seq = ['A', 'B', 'C', 'D']
         result = CoreCommons.list_dup(seq=seq)
         self.assertCountEqual([], result)
 
+    def tests_list_beta_find(self):
+        seq = ['A', 'B', 'C', 'D', 'E']
+        result = CoreCommons.list_search(seq, 'A')
+        self.assertEqual(0, result)
+        result = CoreCommons.list_search(seq, 'C')
+        self.assertEqual(2, result)
+        result = CoreCommons.list_search(seq, 'E')
+        self.assertEqual(4, result)
+
     def test_list_standardize(self):
         seq = [100, 75, 50, 25, 0]
         result = CoreCommons.list_standardize(seq=seq)
         self.assertEqual(0.0, result[2])
         self.assertEqual(0.0, result[1] + result[3])
         self.assertEqual(0.0, result[0] + result[4])
```

### Comparing `discovery-core-0.4.1/test/handlers/connector_contract_test.py` & `discovery-core-0.4.2/test/handlers/connector_contract_test.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.4.1/test/handlers/handler_factory_test.py` & `discovery-core-0.4.2/test/handlers/handler_factory_test.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.4.1/test/intent/abstract_intent_test.py` & `discovery-core-0.4.2/test/intent/abstract_intent_test.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.4.1/test/intent/pyarrow_intent_model.py` & `discovery-core-0.4.2/test/intent/pyarrow_intent_model.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.4.1/test/properties/abstract_properties_manager_test.py` & `discovery-core-0.4.2/test/properties/abstract_properties_manager_test.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.4.1/test/properties/property_manager_test.py` & `discovery-core-0.4.2/test/properties/property_manager_test.py`

 * *Files identical despite different names*

