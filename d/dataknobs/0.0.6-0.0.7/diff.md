# Comparing `tmp/dataknobs-0.0.6.tar.gz` & `tmp/dataknobs-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataknobs-0.0.6.tar", max compression
+gzip compressed data, was "dataknobs-0.0.7.tar", max compression
```

## Comparing `dataknobs-0.0.6.tar` & `dataknobs-0.0.7.tar`

### file list

```diff
@@ -1,39 +1,40 @@
--rw-r--r--   0        0        0     1065 2023-02-10 14:57:51.288106 dataknobs-0.0.6/LICENSE
--rw-r--r--   0        0        0     2189 2023-04-07 02:48:31.052502 dataknobs-0.0.6/README.md
--rw-r--r--   0        0        0        0 2023-02-10 14:59:17.454505 dataknobs-0.0.6/dataknobs/__init__.py
--rw-r--r--   0        0        0        0 2023-02-10 14:59:17.448758 dataknobs-0.0.6/dataknobs/structures/__init__.py
--rw-r--r--   0        0        0     1984 2023-02-10 14:59:17.453600 dataknobs-0.0.6/dataknobs/structures/conditional_dict.py
--rw-r--r--   0        0        0     2244 2023-04-07 02:48:31.054139 dataknobs-0.0.6/dataknobs/structures/document.py
--rw-r--r--   0        0        0     2846 2023-05-15 16:49:57.176743 dataknobs-0.0.6/dataknobs/structures/record_store.py
--rw-r--r--   0        0        0    16152 2023-04-07 02:48:31.055468 dataknobs-0.0.6/dataknobs/structures/tree.py
--rw-r--r--   0        0        0        0 2023-02-10 14:59:17.460301 dataknobs-0.0.6/dataknobs/utils/__init__.py
--rw-r--r--   0        0        0    10016 2023-04-07 02:48:31.055899 dataknobs-0.0.6/dataknobs/utils/elasticsearch_utils.py
--rw-r--r--   0        0        0     8677 2023-02-10 14:59:17.470241 dataknobs-0.0.6/dataknobs/utils/emoji_utils.py
--rw-r--r--   0        0        0     2317 2023-04-19 15:41:48.056711 dataknobs-0.0.6/dataknobs/utils/file_utils.py
--rw-r--r--   0        0        0    17695 2023-03-10 01:33:33.971598 dataknobs-0.0.6/dataknobs/utils/json_paths.py.002
--rw-r--r--   0        0        0    17767 2023-03-11 21:00:19.316119 dataknobs-0.0.6/dataknobs/utils/json_paths.py.del
--rw-r--r--   0        0        0    40729 2023-04-29 20:00:19.391504 dataknobs-0.0.6/dataknobs/utils/json_utils.py
--rw-r--r--   0        0        0    20296 2023-02-18 17:25:48.681883 dataknobs-0.0.6/dataknobs/utils/json_utils.py.000
--rw-r--r--   0        0        0    56727 2023-03-08 20:22:00.908582 dataknobs-0.0.6/dataknobs/utils/json_utils.py.001
--rw-r--r--   0        0        0    56710 2023-03-09 18:53:43.696089 dataknobs-0.0.6/dataknobs/utils/json_utils.py.002
--rw-r--r--   0        0        0    38844 2023-03-12 02:44:32.369267 dataknobs-0.0.6/dataknobs/utils/json_utils.py.003
--rw-r--r--   0        0        0    39879 2023-03-22 16:43:44.020177 dataknobs-0.0.6/dataknobs/utils/json_utils.py.004
--rw-r--r--   0        0        0    14351 2023-02-10 14:59:17.456062 dataknobs-0.0.6/dataknobs/utils/pandas_utils.py
--rw-r--r--   0        0        0     9134 2023-03-13 17:34:48.816244 dataknobs-0.0.6/dataknobs/utils/path_group.py.no-add
--rw-r--r--   0        0        0    11853 2023-03-11 22:32:17.644075 dataknobs-0.0.6/dataknobs/utils/path_sorter.py.del
--rw-r--r--   0        0        0    13283 2023-02-10 14:59:17.466209 dataknobs-0.0.6/dataknobs/utils/requests_utils.py
--rw-r--r--   0        0        0     3782 2023-02-10 14:59:17.458516 dataknobs-0.0.6/dataknobs/utils/resource_utils.py
--rw-r--r--   0        0        0    13186 2023-02-10 14:59:17.469429 dataknobs-0.0.6/dataknobs/utils/sql_utils.py
--rw-r--r--   0        0        0    24066 2023-05-08 19:59:02.942710 dataknobs-0.0.6/dataknobs/utils/stats_utils.py
--rw-r--r--   0        0        0     1425 2023-04-07 02:48:31.057298 dataknobs-0.0.6/dataknobs/utils/subprocess_utils.py
--rw-r--r--   0        0        0     3104 2023-02-10 14:59:17.468140 dataknobs-0.0.6/dataknobs/utils/xml_utils.py
--rw-r--r--   0        0        0     2878 2023-02-10 14:59:17.477011 dataknobs-0.0.6/dataknobs/xization/0.readme.txt
--rw-r--r--   0        0        0        0 2023-02-10 14:59:17.477662 dataknobs-0.0.6/dataknobs/xization/__init__.py
--rw-r--r--   0        0        0    23741 2023-04-07 02:48:31.058125 dataknobs-0.0.6/dataknobs/xization/annotations.py
--rw-r--r--   0        0        0    32223 2023-04-07 02:48:31.059013 dataknobs-0.0.6/dataknobs/xization/authorities.py
--rw-r--r--   0        0        0    24670 2023-04-07 02:48:31.059440 dataknobs-0.0.6/dataknobs/xization/lexicon.py
--rw-r--r--   0        0        0    27391 2023-04-07 02:48:31.060348 dataknobs-0.0.6/dataknobs/xization/masking_tokenizer.py
--rw-r--r--   0        0        0    14226 2023-02-10 14:59:17.476141 dataknobs-0.0.6/dataknobs/xization/normalize.py
--rw-r--r--   0        0        0      834 2023-05-15 16:49:57.177027 dataknobs-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     3313 1970-01-01 00:00:00.000000 dataknobs-0.0.6/setup.py
--rw-r--r--   0        0        0     3138 1970-01-01 00:00:00.000000 dataknobs-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-02-10 14:57:51.288106 dataknobs-0.0.7/LICENSE
+-rw-r--r--   0        0        0     2189 2023-04-07 02:48:31.052502 dataknobs-0.0.7/README.md
+-rw-r--r--   0        0        0        0 2023-02-10 14:59:17.454505 dataknobs-0.0.7/dataknobs/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-10 14:59:17.448758 dataknobs-0.0.7/dataknobs/structures/__init__.py
+-rw-r--r--   0        0        0     1984 2023-02-10 14:59:17.453600 dataknobs-0.0.7/dataknobs/structures/conditional_dict.py
+-rw-r--r--   0        0        0     2244 2023-04-07 02:48:31.054139 dataknobs-0.0.7/dataknobs/structures/document.py
+-rw-r--r--   0        0        0     2846 2023-05-15 16:49:57.176743 dataknobs-0.0.7/dataknobs/structures/record_store.py
+-rw-r--r--   0        0        0    16152 2023-04-07 02:48:31.055468 dataknobs-0.0.7/dataknobs/structures/tree.py
+-rw-r--r--   0        0        0        0 2023-02-10 14:59:17.460301 dataknobs-0.0.7/dataknobs/utils/__init__.py
+-rw-r--r--   0        0        0    10016 2023-04-07 02:48:31.055899 dataknobs-0.0.7/dataknobs/utils/elasticsearch_utils.py
+-rw-r--r--   0        0        0     8677 2023-02-10 14:59:17.470241 dataknobs-0.0.7/dataknobs/utils/emoji_utils.py
+-rw-r--r--   0        0        0     2697 2023-08-03 23:16:33.443798 dataknobs-0.0.7/dataknobs/utils/file_utils.py
+-rw-r--r--   0        0        0    17695 2023-03-10 01:33:33.971598 dataknobs-0.0.7/dataknobs/utils/json_paths.py.002
+-rw-r--r--   0        0        0    17767 2023-03-11 21:00:19.316119 dataknobs-0.0.7/dataknobs/utils/json_paths.py.del
+-rw-r--r--   0        0        0    40761 2023-08-03 23:16:33.444305 dataknobs-0.0.7/dataknobs/utils/json_utils.py
+-rw-r--r--   0        0        0    20296 2023-02-18 17:25:48.681883 dataknobs-0.0.7/dataknobs/utils/json_utils.py.000
+-rw-r--r--   0        0        0    56727 2023-03-08 20:22:00.908582 dataknobs-0.0.7/dataknobs/utils/json_utils.py.001
+-rw-r--r--   0        0        0    56710 2023-03-09 18:53:43.696089 dataknobs-0.0.7/dataknobs/utils/json_utils.py.002
+-rw-r--r--   0        0        0    38844 2023-03-12 02:44:32.369267 dataknobs-0.0.7/dataknobs/utils/json_utils.py.003
+-rw-r--r--   0        0        0    39879 2023-03-22 16:43:44.020177 dataknobs-0.0.7/dataknobs/utils/json_utils.py.004
+-rw-r--r--   0        0        0    14351 2023-02-10 14:59:17.456062 dataknobs-0.0.7/dataknobs/utils/pandas_utils.py
+-rw-r--r--   0        0        0     9134 2023-03-13 17:34:48.816244 dataknobs-0.0.7/dataknobs/utils/path_group.py.no-add
+-rw-r--r--   0        0        0    11853 2023-03-11 22:32:17.644075 dataknobs-0.0.7/dataknobs/utils/path_sorter.py.del
+-rw-r--r--   0        0        0    13283 2023-02-10 14:59:17.466209 dataknobs-0.0.7/dataknobs/utils/requests_utils.py
+-rw-r--r--   0        0        0     3782 2023-02-10 14:59:17.458516 dataknobs-0.0.7/dataknobs/utils/resource_utils.py
+-rw-r--r--   0        0        0    13529 2023-08-03 23:16:33.444696 dataknobs-0.0.7/dataknobs/utils/sql_utils.py
+-rw-r--r--   0        0        0    24066 2023-05-08 19:59:02.942710 dataknobs-0.0.7/dataknobs/utils/stats_utils.py
+-rw-r--r--   0        0        0     1425 2023-04-07 02:48:31.057298 dataknobs-0.0.7/dataknobs/utils/subprocess_utils.py
+-rw-r--r--   0        0        0     3104 2023-02-10 14:59:17.468140 dataknobs-0.0.7/dataknobs/utils/xml_utils.py
+-rw-r--r--   0        0        0     2878 2023-02-10 14:59:17.477011 dataknobs-0.0.7/dataknobs/xization/0.readme.txt
+-rw-r--r--   0        0        0        0 2023-02-10 14:59:17.477662 dataknobs-0.0.7/dataknobs/xization/__init__.py
+-rw-r--r--   0        0        0    47317 2023-08-03 23:16:33.445227 dataknobs-0.0.7/dataknobs/xization/annotations.py
+-rw-r--r--   0        0        0    24071 2023-07-07 20:44:22.174208 dataknobs-0.0.7/dataknobs/xization/annotations.py.000
+-rw-r--r--   0        0        0    31640 2023-08-03 23:16:33.445734 dataknobs-0.0.7/dataknobs/xization/authorities.py
+-rw-r--r--   0        0        0    24670 2023-04-07 02:48:31.059440 dataknobs-0.0.7/dataknobs/xization/lexicon.py
+-rw-r--r--   0        0        0    27391 2023-04-07 02:48:31.060348 dataknobs-0.0.7/dataknobs/xization/masking_tokenizer.py
+-rw-r--r--   0        0        0    14226 2023-02-10 14:59:17.476141 dataknobs-0.0.7/dataknobs/xization/normalize.py
+-rw-r--r--   0        0        0      834 2023-08-03 23:16:33.447817 dataknobs-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     3313 1970-01-01 00:00:00.000000 dataknobs-0.0.7/setup.py
+-rw-r--r--   0        0        0     3138 1970-01-01 00:00:00.000000 dataknobs-0.0.7/PKG-INFO
```

### Comparing `dataknobs-0.0.6/LICENSE` & `dataknobs-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `dataknobs-0.0.6/README.md` & `dataknobs-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `dataknobs-0.0.6/dataknobs/structures/conditional_dict.py` & `dataknobs-0.0.7/dataknobs/structures/conditional_dict.py`

 * *Files identical despite different names*

### Comparing `dataknobs-0.0.6/dataknobs/structures/document.py` & `dataknobs-0.0.7/dataknobs/structures/document.py`

 * *Files identical despite different names*

### Comparing `dataknobs-0.0.6/dataknobs/structures/record_store.py` & `dataknobs-0.0.7/dataknobs/structures/record_store.py`

 * *Files identical despite different names*

### Comparing `dataknobs-0.0.6/dataknobs/structures/tree.py` & `dataknobs-0.0.7/dataknobs/structures/tree.py`

 * *Files identical despite different names*

### Comparing `dataknobs-0.0.6/dataknobs/utils/elasticsearch_utils.py` & `dataknobs-0.0.7/dataknobs/utils/elasticsearch_utils.py`

 * *Files identical despite different names*

### Comparing `dataknobs-0.0.6/dataknobs/utils/emoji_utils.py` & `dataknobs-0.0.7/dataknobs/utils/emoji_utils.py`

 * *Files identical despite different names*

### Comparing `dataknobs-0.0.6/dataknobs/utils/file_utils.py` & `dataknobs-0.0.7/dataknobs/utils/file_utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -71,7 +71,21 @@
         mode = 'wt'
     else:
         open_fn = open
         mode = 'w'
     with open_fn(outfile, mode=mode, encoding='utf-8') as f:
         for line in sorted(lines):
             print(line, file=f)
+
+
+def is_gzip_file(filepath: str) -> bool:
+    '''
+    Determine whether the file at filepath is gzipped.
+    :param filepath: The path to the file
+    :return: True if the file is gzipped
+    '''
+    is_gzip = False
+    if os.path.exists(filepath):
+        with open(filepath, 'rb') as f:
+            b = f.read(3)
+            is_gzip = (b == b'\x1f\x8b\x08')
+    return is_gzip
```

### Comparing `dataknobs-0.0.6/dataknobs/utils/json_paths.py.002` & `dataknobs-0.0.7/dataknobs/utils/json_paths.py.002`

 * *Files identical despite different names*

### Comparing `dataknobs-0.0.6/dataknobs/utils/json_paths.py.del` & `dataknobs-0.0.7/dataknobs/utils/json_paths.py.del`

 * *Files identical despite different names*

### Comparing `dataknobs-0.0.6/dataknobs/utils/json_utils.py` & `dataknobs-0.0.7/dataknobs/utils/json_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import io
 import json_stream.requests
 import os
 import pandas as pd
 import re
 import requests
 import dataknobs.structures.tree as dk_tree
+import dataknobs.utils.file_utils as dk_futils
 from abc import ABC, abstractmethod
 from collections import defaultdict
 from typing import Any, Callable, Dict, List, Set, Tuple, Union
 
 
 ELT_IDX_RE = re.compile(r'^(.*)\[(.*)\]$')
 FLATTEN_IDX_RE = re.compile(r'\[(\d+)\]')
@@ -27,15 +28,15 @@
     :param json_data: The json data (url, file_path, or str)
     :param visitor_fn: The visitor_fn(item, path) to call, where
         item is each json item's value and path is the tuple of
         elements identifying the path to the item.
     :param timeout: The requests timeout (in seconds)
     '''
     if os.path.exists(json_data):
-        if json_data.endswith('.gz') or '.gz?' in json_data:
+        if dk_futils.is_gzip_file(json_data):
             with gzip.open(json_data, 'rt', encoding='utf-8') as f:
                 json_stream.visit(f, visitor_fn)
         else:
             with open(json_data, 'r', encoding='utf-8') as f:
                 json_stream.visit(f, visitor_fn)
     elif json_data.startswith('http'):
         with requests.get(json_data, stream=True, timeout=timeout) as response:
```

### Comparing `dataknobs-0.0.6/dataknobs/utils/json_utils.py.000` & `dataknobs-0.0.7/dataknobs/utils/json_utils.py.000`

 * *Files identical despite different names*

### Comparing `dataknobs-0.0.6/dataknobs/utils/json_utils.py.001` & `dataknobs-0.0.7/dataknobs/utils/json_utils.py.001`

 * *Files identical despite different names*

### Comparing `dataknobs-0.0.6/dataknobs/utils/json_utils.py.002` & `dataknobs-0.0.7/dataknobs/utils/json_utils.py.002`

 * *Files identical despite different names*

### Comparing `dataknobs-0.0.6/dataknobs/utils/json_utils.py.003` & `dataknobs-0.0.7/dataknobs/utils/json_utils.py.003`

 * *Files identical despite different names*

### Comparing `dataknobs-0.0.6/dataknobs/utils/json_utils.py.004` & `dataknobs-0.0.7/dataknobs/utils/json_utils.py.004`

 * *Files identical despite different names*

### Comparing `dataknobs-0.0.6/dataknobs/utils/pandas_utils.py` & `dataknobs-0.0.7/dataknobs/utils/pandas_utils.py`

 * *Files identical despite different names*

### Comparing `dataknobs-0.0.6/dataknobs/utils/path_group.py.no-add` & `dataknobs-0.0.7/dataknobs/utils/path_group.py.no-add`

 * *Files identical despite different names*

### Comparing `dataknobs-0.0.6/dataknobs/utils/path_sorter.py.del` & `dataknobs-0.0.7/dataknobs/utils/path_sorter.py.del`

 * *Files identical despite different names*

### Comparing `dataknobs-0.0.6/dataknobs/utils/requests_utils.py` & `dataknobs-0.0.7/dataknobs/utils/requests_utils.py`

 * *Files identical despite different names*

### Comparing `dataknobs-0.0.6/dataknobs/utils/resource_utils.py` & `dataknobs-0.0.7/dataknobs/utils/resource_utils.py`

 * *Files identical despite different names*

### Comparing `dataknobs-0.0.6/dataknobs/utils/sql_utils.py` & `dataknobs-0.0.7/dataknobs/utils/sql_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,25 +131,34 @@
     def _do_get_table_names(self) -> List[str]:
         '''
         Do the work of getting table names.
         '''
         return self.tables_df['table_name'].tolist()
 
     @lru_cache(maxsize=2)
-    def query(self, query: str) -> pd.DataFrame:
+    def query(
+            self,
+            query: str,
+            params: Dict[str, Any] = None,
+    ) -> pd.DataFrame:
         '''
         Submit a query, returning the results as a dataframe.
 
         :param query: The sql query to execute
+        :param params: Parameters to safely inject into the query string, where
+            each parameter "param" has the form "%(param)s" in the query string
         :return: A dataframe with the results
         '''
         df = None
         with self.get_conn() as conn:
             with conn.cursor() as curs:
-                curs.execute(query)
+                if params is None:
+                    curs.execute(query)
+                else:
+                    curs.execute(query, params)
                 df = pd.DataFrame(
                     curs.fetchall(),
                     columns=[
                         desc[0] for desc in curs.description
                     ]
                 )
         return df
```

### Comparing `dataknobs-0.0.6/dataknobs/utils/stats_utils.py` & `dataknobs-0.0.7/dataknobs/utils/stats_utils.py`

 * *Files identical despite different names*

### Comparing `dataknobs-0.0.6/dataknobs/utils/subprocess_utils.py` & `dataknobs-0.0.7/dataknobs/utils/subprocess_utils.py`

 * *Files identical despite different names*

### Comparing `dataknobs-0.0.6/dataknobs/utils/xml_utils.py` & `dataknobs-0.0.7/dataknobs/utils/xml_utils.py`

 * *Files identical despite different names*

### Comparing `dataknobs-0.0.6/dataknobs/xization/0.readme.txt` & `dataknobs-0.0.7/dataknobs/xization/0.readme.txt`

 * *Files identical despite different names*

### Comparing `dataknobs-0.0.6/dataknobs/xization/annotations.py` & `dataknobs-0.0.7/dataknobs/xization/annotations.py.000`

 * *Files 1% similar despite different names*

```diff
@@ -219,14 +219,25 @@
         '''
         Get the annotations as a pandas dataframe.
         '''
         if self._df is None:
             self._df = self._build_df()
         return self._df
 
+    def clear(self):
+        ''' Clear/empty out all annotations '''
+        self._df = None
+        self._annotations_list = None
+
+    def is_empty(self) -> bool:
+        return (
+            (self._df is None or len(self._df) == 0) and
+            (self._annotations_list is None or len(self._annotations_list) == 0)
+        )
+
     def add_dict(self, annotation: Dict[str, Any]):
         '''
         Add the annotation dict.
         '''
         self.ann_row_dicts.append(annotation)
 
     def add_dicts(self, annotations: List[Dict[str, Any]]):
```

### Comparing `dataknobs-0.0.6/dataknobs/xization/authorities.py` & `dataknobs-0.0.7/dataknobs/xization/authorities.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 import pandas as pd
 import re
-import dataknobs.structures.document as dk_doc
-import dataknobs.xization.annotations as dk_anns
+import dataknobs.xization.annotations as dk_annots
 from abc import ABC, abstractmethod
 from typing import Any, Callable, Dict, List, Set, Union
 
 
 # Key annotation column name constants
 KEY_AUTH_ID_COL = 'auth_id'
 
 
-class DerivedFieldGroups(dk_anns.DerivedAnnotationColumns):
+class DerivedFieldGroups(dk_annots.DerivedAnnotationColumns):
     '''
     Defines derived column types:
       * "field_type" -- The column holding they type of field of an annotation row
       * "field_group" -- The column holding the group number(s) of the field
       * "field_record" -- The column holding record number(s) of the field
     '''
     
@@ -41,15 +40,15 @@
         '''
         self.field_type_suffix = field_type_suffix
         self.field_group_suffix = field_group_suffix
         self.field_record_suffix = field_record_suffix
 
     def get_col_value(
             self,
-            metadata: dk_anns.AnnotationsMetaData,
+            metadata: dk_annots.AnnotationsMetaData,
             col_type: str,
             row: pd.Series,
             missing: str = None,
     ) -> str:
         '''
         Get the value of the column in the given row derived from col_type,
         where col_type is one of:
@@ -125,27 +124,27 @@
         value; or a field type, group, or record, get the name of the derived
         field record column.
         '''
         field = self.unpack_field(field_value)
         return f'{field}{self.field_record_suffix}'
 
 
-class AuthorityAnnotationsMetaData(dk_anns.AnnotationsMetaData):
+class AuthorityAnnotationsMetaData(dk_annots.AnnotationsMetaData):
     '''
     An extension of AnnotationsMetaData that adds an 'auth_id_col' to the
     standard (key) annotation columns (attributes).
     '''
     def __init__(
             self,
-            start_pos_col: str = dk_anns.KEY_START_POS_COL,
-            end_pos_col: str = dk_anns.KEY_END_POS_COL,
-            text_col: str = dk_anns.KEY_TEXT_COL,
-            ann_type_col: str = dk_anns.KEY_ANN_TYPE_COL,
+            start_pos_col: str = dk_annots.KEY_START_POS_COL,
+            end_pos_col: str = dk_annots.KEY_END_POS_COL,
+            text_col: str = dk_annots.KEY_TEXT_COL,
+            ann_type_col: str = dk_annots.KEY_ANN_TYPE_COL,
             auth_id_col: str = KEY_AUTH_ID_COL,
-            sort_fields: List[str] = (dk_anns.KEY_START_POS_COL, dk_anns.KEY_END_POS_COL),
+            sort_fields: List[str] = (dk_annots.KEY_START_POS_COL, dk_annots.KEY_END_POS_COL),
             sort_fields_ascending: List[bool] = (True, False),
             **kwargs
     ):
         '''
         Initialize with key (and more) column names and info.
 
         Key column types:
@@ -182,15 +181,15 @@
 
     @property
     def auth_id_col(self) -> str:
         ''' Get the column name for the auth_id '''
         return self.data[KEY_AUTH_ID_COL]
 
 
-class AuthorityAnnotationsBuilder(dk_anns.AnnotationsBuilder):
+class AuthorityAnnotationsBuilder(dk_annots.AnnotationsBuilder):
     '''
     An extension of an AnnotationsBuilder that adds the 'auth_id' column.
     '''
 
     def __init__(
             self,
             metadata: AuthorityAnnotationsMetaData=None,
@@ -261,15 +260,15 @@
         :param is_id: True if value is an ID
         :return: The applicable authority dataframe rows.
         '''
         col = self.df.index if is_id else self.df[self.name]
         return self.df[col == value]
 
 
-class Authority(ABC):
+class Authority(dk_annots.Annotator):
     '''
     A class for managing and defining tabular authoritative data for e.g.,
     taxonomies, etc., and using them to annotate instances within text.
     '''
     def __init__(
             self,
             name:str,
@@ -287,15 +286,15 @@
         :param authdata: The authority data
         :param field_groups: The derived field groups to use
         :param anns_validator: fn(auth, anns_dict_list) that returns True if
            the list of annotation row dicts are valid to be added as
            annotations for a single match or "entity".
         :param parent_auth: This authority's parent authority (if any)
         '''
-        self._name = name
+        super().__init__(name)
         self.anns_builder = (
             auth_anns_builder if auth_anns_builder is not None
             else AuthorityAnnotationsBuilder()
         )
         self.authdata = authdata
         self.field_groups = (
             field_groups if field_groups is not None
@@ -306,22 +305,14 @@
 
     @property
     def metadata(self) -> AuthorityAnnotationsMetaData:
         ''' Get the meta-data '''
         return self.anns_builder.metadata
 
     @property
-    def name(self) -> str:
-        '''
-        Get the name of this authority, which is usually the name or type
-        of entities defined herein.
-        '''
-        return self._name
-
-    @property
     def parent(self) -> 'Authority':
         '''
         Get this authority's parent, or None.
         '''
         return self._parent
 
     @abstractmethod
@@ -329,60 +320,55 @@
         '''
         Determine whether the given value is in this authority.
         :param value: A possible authority value.
         :return: True if the value is a valid entity value.
         '''
         raise NotImplementedError
 
-    def annotate_text(
+    def annotate_input(
             self,
-            doctext: Union[dk_doc.Text, str],
-            annotations: dk_anns.Annotations = None,
-    ) -> dk_anns.Annotations:
+            text_obj: Union[dk_annots.AnnotatedText, str],
+            **kwargs,
+    ) -> dk_annots.Annotations:
         '''
         Find and annotate this authority's entities in the document text
         as dictionaries like:
         [
             {
                 'input_id': <id>,
                 'start_pos': <start_char_pos>,
                 'end_pos': <end_char_pos>,
                 'entity_text': <entity_text>,
                 'ann_type': <authority_name>,
                 '<auth_id>': <auth_value_id_or_canonical_form>,
                 'confidence': <confidence_if_available>,
             },
         ]
-        :param doctext: The text to process.
-        :param annotations: The annotations object to add annotations to
-        :return: The given or a new Annotations instance
-        '''
-        if doctext is not None:
-            if isinstance(doctext, str) and len(doctext.strip()) > 0:
-                doctext = dk_doc.Text(
-                    doctext,
-                    AuthorityAnnotationsMetaData(),
+        :param text_obj: The text object or string to process.
+        :return: An Annotations instance
+        '''
+        if text_obj is not None:
+            if isinstance(text_obj, str) and len(text_obj.strip()) > 0:
+                text_obj = dk_annots.AnnotatedText(
+                    text_obj,
+                    annots_metadata = self.metadata,
                 )
-        if doctext is not None:
-            if annotations is None:
-                annotations = dk_anns.Annotations(self.metadata)
-            annotations = self.add_annotations(doctext, annotations)
+        if text_obj is not None:
+            annotations = self.add_annotations(text_obj)
         return annotations
 
     @abstractmethod
     def add_annotations(
             self,
-            doctext: dk_doc.Text,
-            annotations: dk_anns.Annotations,
-    ) -> dk_anns.Annotations:
+            text_obj: dk_annots.AnnotatedText,
+    ) -> dk_annots.Annotations:
         '''
         Method to do the work of finding, validating, and adding annotations.
-        :param doctext: The text to process.
-        :param annotations: The annotations object to add annotations to
-        :return: The given or a new Annotations instance
+        :param text_obj: The annotated text object to process and add annotations.
+        :return: The added Annotations
         '''
         raise NotImplementedError
 
     def validate_ann_dicts(self, ann_dicts: List[Dict[str, Any]]) -> bool:
         '''
         The annotation row dictionaries are valid if:
           * They are non-empty
@@ -397,16 +383,16 @@
                     self.anns_validator is None or
                     self.anns_validator(self, ann_dicts)
                 )
         )
 
     def compose(
             self,
-            annotations: dk_anns.Annotations,
-    ) -> dk_anns.Annotations:
+            annotations: dk_annots.Annotations,
+    ) -> dk_annots.Annotations:
         '''
         Compose annotations into groups.
         :param annotations: The annotations
         :return: composed annotations
         '''
         return annotations
 
@@ -471,29 +457,29 @@
             self.auth = auth
             self.ann_row_dicts = ann_row_dicts
             self._row_accessor = None  # AnnotationsRowAccessor
             self._anns = None  # Annotations
             self._atts = None  # Dict[str, str]
     
         @property
-        def row_accessor(self) -> dk_anns.AnnotationsRowAccessor:
+        def row_accessor(self) -> dk_annots.AnnotationsRowAccessor:
             '''
             Get the row accessor for this instance's annotations.
             '''
             if self._row_accessor is None:
-                self._row_accessor = dk_anns.AnnotationsRowAccessor(
+                self._row_accessor = dk_annots.AnnotationsRowAccessor(
                     self.auth.metadata, derived_cols=self.auth.field_groups
                 )
             return self._row_accessor
     
         @property
-        def anns(self) -> dk_anns.Annotations:
+        def anns(self) -> dk_annots.Annotations:
             ''' Get this instance's annotation rows as an annotations object '''
             if self._anns is None:
-                self._anns = dk_anns.Annotations(self.auth.metadata)
+                self._anns = dk_annots.Annotations(self.auth.metadata)
                 for row_dict in self.ann_row_dicts:
                     self._anns.add_dict(row_dict)
             return self._anns
     
         @property
         def df(self) -> pd.DataFrame:
             ''' Get the annotation's dataframe '''
@@ -711,24 +697,22 @@
         :return: None if the value is not a valid entity value; otherwise,
             return the re.Match object.
         '''
         return self.regex.match(str(value))
 
     def add_annotations(
             self,
-            doctext: dk_doc.Text,
-            annotations: dk_anns.Annotations,
-    ) -> dk_anns.Annotations:
-        '''
-        Method to do the work of finding and adding annotations.
-        :param doctext: The text to process.
-        :param annotations: The annotations object to add annotations to
-        :return: The given or a new Annotations instance
+            text_obj: dk_annots.AnnotatedText,
+    ) -> dk_annots.Annotations:
         '''
-        for match in re.finditer(self.regex, doctext.text):
+        Method to do the work of finding, validating, and adding annotations.
+        :param text_obj: The annotated text object to process and add annotations.
+        :return: The added Annotations
+        '''
+        for match in re.finditer(self.regex, text_obj.text):
             ann_dicts = list()
             if match.lastindex is not None:
                 if len(self.regex.groupindex) > 0:  # we have named groups
                     for group_name, group_num in self.regex.groupindex.items():
                         group_text = match.group(group_num)
                         kwargs = {
                             self.field_groups.get_field_type_col(self.name): group_name
@@ -758,16 +742,16 @@
                     start_pos=match.start(),
                     end_pos=match.end(),
                     entity_text=match.group(),
                     auth_value_id=self.get_canonical_form(match.group(), self.name),
                 ))
             if self.validate_ann_dicts(ann_dicts):
                 # Add non-empty, valid annotation dicts to the result
-                annotations.add_dicts(ann_dicts)
-        return annotations
+                text_obj.annotations.add_dicts(ann_dicts)
+        return text_obj.annotations
 
     def get_canonical_form(self, entity_text:str, entity_type:str) -> Any:
         if self.canonical_fn is not None:
             entity_text = self.canonical_fn(entity_text, entity_type)
         return entity_text
 
 
@@ -825,19 +809,17 @@
         for auth in self.auths:
             if auth.has_value(value):
                 return True
         return False
 
     def add_annotations(
             self,
-            doctext: dk_doc.Text,
-            annotations: dk_anns.Annotations,
-    ) -> dk_anns.Annotations:
-        '''
-        Method to do the work of finding and adding annotations.
-        :param doctext: The text to process.
-        :param annotations: The annotations object to add annotations to
-        :return: The given or a new Annotations instance
+            text_obj: dk_annots.AnnotatedText,
+    ) -> dk_annots.Annotations:
+        '''
+        Method to do the work of finding, validating, and adding annotations.
+        :param text_obj: The annotated text object to process and add annotations.
+        :return: The added Annotations
         '''
         for auth in self.auths:
-            auth.annotate_text(doctext, annotations)
-        return annotations
+            auth.annotate_input(text_obj)
+        return text_obj.annotations
```

### Comparing `dataknobs-0.0.6/dataknobs/xization/lexicon.py` & `dataknobs-0.0.7/dataknobs/xization/lexicon.py`

 * *Files identical despite different names*

### Comparing `dataknobs-0.0.6/dataknobs/xization/masking_tokenizer.py` & `dataknobs-0.0.7/dataknobs/xization/masking_tokenizer.py`

 * *Files identical despite different names*

### Comparing `dataknobs-0.0.6/dataknobs/xization/normalize.py` & `dataknobs-0.0.7/dataknobs/xization/normalize.py`

 * *Files identical despite different names*

### Comparing `dataknobs-0.0.6/pyproject.toml` & `dataknobs-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dataknobs"
-version = "0.0.6"
+version = "0.0.7"
 description = "Useful implementations of data structures and design patterns for AI knowledge bases."
 authors = ["Spence Koehler <KoehlerSB747@gmail.com>"]
 readme = "README.md"
 packages = [{include = "dataknobs"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `dataknobs-0.0.6/setup.py` & `dataknobs-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
  'psycopg2-binary>=2.9.3,<3.0.0',
  'python-dotenv>=0.21.0,<0.22.0',
  'requests>=2.28.1,<3.0.0',
  'scikit-learn>=1.2.1,<2.0.0']
 
 setup_kwargs = {
     'name': 'dataknobs',
-    'version': '0.0.6',
+    'version': '0.0.7',
     'description': 'Useful implementations of data structures and design patterns for AI knowledge bases.',
     'long_description': 'DataKnobs\n=============================\n\n## Description\n\nUseful implementations of data structures and design patterns for knowledge bases and AI, or the knobs and levers for fine-tuning and leveraging your data.\n\nThis repo also serves as a template or sandbox for development, experimentation, and testing of general data structures, algorithms, and utilities for DS, AI, ML, and NLP.\n\nProvides connectors for other popular text and data processing packages like:\n  * numpy and pandas\n  * nltk\n  * wordnet\n  * postgres\n  * elasticsearch\n\n## General project information\n\nThe purpose of this project is:\n\n  * To provide dependable implementations of useful data structures.\n  * To show examples of design patterns and ways to apply AI concepts.\n  * To prototype tools for delivering a robust DS/AI/ML/NLP utilities library package.\n  * To facilitate interactive development, demonstration, visualization, and testing of the library components via jupter notebooks and/or scripts.\n\n## Installation and Usage\n\n```bash/python\n% pip install dataknobs\n% python\n>>> import dataknobs as dk\n>>> ...\n```\n\n\n## Development\n\n### Development machine prerequisites\n\nThe following minimum configuration should exist for development:\n\n  * tox\n  * pyenv\n     * pyenv install 3.9\n  * poetry\n\nWith optional:\n\n  * docker\n  * bash\n\nBy convention, a data directory can be leveraged for development that is mounted as a shared volumne in Docker as /data. This has the default of $HOME/data, but can be overridden with the DATADIR environment variable.\n\n\n### Development quickstart guide\n\n  * In a terminal, clone the repo and cd into the project directory.\n\n#### Testing\n\n  * Tests and Lint: "tox"\n  * Just unit tests: "tox -e tests"\n  * Just lint: "tox -e lint"\n\n#### Using docker\n\n  * Development:\n```\n% tox -e dev\n# poetry shell\n# python\n```\n\n  * Notebook:\n    * execute "tox -e nb"\n      * copy/paste url into browser\n\n#### Using virtual environments\n\n  * Development:\n    * Manual: source ".project_vars", poetry install, poetry shell\n    * Automated: execute "bin/start_dev.sh"  (requires "/bin/bash" on your machine)\n\n  * Notebook:\n    * execute "bin/start_notebook.sh"\n      * copy/paste url into browser\n',
     'author': 'Spence Koehler',
     'author_email': 'KoehlerSB747@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `dataknobs-0.0.6/PKG-INFO` & `dataknobs-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataknobs
-Version: 0.0.6
+Version: 0.0.7
 Summary: Useful implementations of data structures and design patterns for AI knowledge bases.
 Author: Spence Koehler
 Author-email: KoehlerSB747@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

