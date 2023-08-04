# Comparing `tmp/mlh-0.0.7.tar.gz` & `tmp/mlh-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlh-0.0.7.tar", last modified: Wed Aug  2 07:39:09 2023, max compression
+gzip compressed data, was "mlh-0.0.8.tar", last modified: Fri Aug  4 05:21:56 2023, max compression
```

## Comparing `mlh-0.0.7.tar` & `mlh-0.0.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-08-02 07:39:09.351399 mlh-0.0.7/
--rw-rw-rw-   0        0        0     3157 2023-08-02 07:39:09.351399 mlh-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     2582 2023-08-02 05:28:22.000000 mlh-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-08-02 07:39:09.335875 mlh-0.0.7/mlh/
--rw-rw-rw-   0        0        0      269 2023-08-02 06:21:43.000000 mlh-0.0.7/mlh/__init__.py
--rw-rw-rw-   0        0        0     6950 2023-08-02 06:50:30.000000 mlh-0.0.7/mlh/common_utils.py
--rw-rw-rw-   0        0        0     2747 2023-08-02 05:28:22.000000 mlh-0.0.7/mlh/data_from_parquet.py
--rw-rw-rw-   0        0        0     5936 2023-08-02 05:28:22.000000 mlh-0.0.7/mlh/s3_connect.py
--rw-rw-rw-   0        0        0    13566 2023-08-02 06:25:41.000000 mlh-0.0.7/mlh/snowflake_connect.py
--rw-rw-rw-   0        0        0     9675 2023-08-02 06:44:38.000000 mlh-0.0.7/mlh/sqlite_functions.py
--rw-rw-rw-   0        0        0    15840 2023-08-02 06:55:50.000000 mlh-0.0.7/mlh/support.py
--rw-rw-rw-   0        0        0    21100 2023-08-02 07:02:13.000000 mlh-0.0.7/mlh/woe.py
-drwxrwxrwx   0        0        0        0 2023-08-02 07:39:09.351399 mlh-0.0.7/mlh.egg-info/
--rw-rw-rw-   0        0        0     3157 2023-08-02 07:39:09.000000 mlh-0.0.7/mlh.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      306 2023-08-02 07:39:09.000000 mlh-0.0.7/mlh.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-02 07:39:09.000000 mlh-0.0.7/mlh.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       98 2023-08-02 07:39:09.000000 mlh-0.0.7/mlh.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-08-02 07:39:09.000000 mlh-0.0.7/mlh.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-02 07:39:09.351399 mlh-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      845 2023-08-02 07:02:25.000000 mlh-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-04 05:21:56.507063 mlh-0.0.8/
+-rw-rw-rw-   0        0        0     3157 2023-08-04 05:21:56.507063 mlh-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     2582 2023-08-02 05:28:22.000000 mlh-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-08-04 05:21:56.475790 mlh-0.0.8/mlh/
+-rw-rw-rw-   0        0        0      269 2023-08-02 06:21:43.000000 mlh-0.0.8/mlh/__init__.py
+-rw-rw-rw-   0        0        0     6954 2023-08-04 04:57:16.000000 mlh-0.0.8/mlh/common_utils.py
+-rw-rw-rw-   0        0        0     2747 2023-08-02 05:28:22.000000 mlh-0.0.8/mlh/data_from_parquet.py
+-rw-rw-rw-   0        0        0     5936 2023-08-02 05:28:22.000000 mlh-0.0.8/mlh/s3_connect.py
+-rw-rw-rw-   0        0        0    13566 2023-08-02 06:25:41.000000 mlh-0.0.8/mlh/snowflake_connect.py
+-rw-rw-rw-   0        0        0     9675 2023-08-02 06:44:38.000000 mlh-0.0.8/mlh/sqlite_functions.py
+-rw-rw-rw-   0        0        0    15840 2023-08-02 06:55:50.000000 mlh-0.0.8/mlh/support.py
+-rw-rw-rw-   0        0        0    21100 2023-08-02 07:02:13.000000 mlh-0.0.8/mlh/woe.py
+drwxrwxrwx   0        0        0        0 2023-08-04 05:21:56.507063 mlh-0.0.8/mlh.egg-info/
+-rw-rw-rw-   0        0        0     3157 2023-08-04 05:21:56.000000 mlh-0.0.8/mlh.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      306 2023-08-04 05:21:56.000000 mlh-0.0.8/mlh.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-04 05:21:56.000000 mlh-0.0.8/mlh.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       98 2023-08-04 05:21:56.000000 mlh-0.0.8/mlh.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-08-04 05:21:56.000000 mlh-0.0.8/mlh.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-04 05:21:56.507063 mlh-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      845 2023-08-04 04:58:54.000000 mlh-0.0.8/setup.py
```

### Comparing `mlh-0.0.7/PKG-INFO` & `mlh-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlh
-Version: 0.0.7
+Version: 0.0.8
 Summary: This package provides helper utilities for machine learning tasks. One major utility is calculation of weight of evidence
 Home-page: https://github.com/devsahu99/mlh
 Author: Devendra Kumar Sahu
 Author-email: devsahu99@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mlh-0.0.7/README.md` & `mlh-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `mlh-0.0.7/mlh/common_utils.py` & `mlh-0.0.8/mlh/common_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -110,15 +110,15 @@
             input date in the year-quarter format
         ------------------------------------------------------------
         Example:
             cmf = common_utils()
             cmf.Get_Last_N_Quarter_Dates('202310', n=5)
         ------------------------------------------------------------    
         """
-        dt = self.getLastNQuarters(quarterNG, n)
+        dt = self.Get_Last_N_Quarters(quarterNG, n)
         return [self.Get_Quarter_End_Date(x) for x in pd.to_datetime(pd.Series(dt))]
 
     def Date_To_Quarter_Start_Date(self, InputDate):
         """
         This function returns any date to its quarter start date. Helpful in cases where quarterly trends are required
 
         ------------------------------------------------------------
@@ -166,8 +166,8 @@
             writer.book = book
             writer.sheets = dict((ws.title, ws) for ws in book.worksheets)  
             df.to_excel(writer, sheet_name = sheet_name, index=False)
         except:
             writer = pd.ExcelWriter(workbook, engine = 'openpyxl')
             df.to_excel(writer, sheet_name = sheet_name, index=False)
         writer.save()
-        writer.close()
+        writer.close()
```

### Comparing `mlh-0.0.7/mlh/data_from_parquet.py` & `mlh-0.0.8/mlh/data_from_parquet.py`

 * *Files identical despite different names*

### Comparing `mlh-0.0.7/mlh/s3_connect.py` & `mlh-0.0.8/mlh/s3_connect.py`

 * *Files identical despite different names*

### Comparing `mlh-0.0.7/mlh/snowflake_connect.py` & `mlh-0.0.8/mlh/snowflake_connect.py`

 * *Files identical despite different names*

### Comparing `mlh-0.0.7/mlh/sqlite_functions.py` & `mlh-0.0.8/mlh/sqlite_functions.py`

 * *Files identical despite different names*

### Comparing `mlh-0.0.7/mlh/support.py` & `mlh-0.0.8/mlh/support.py`

 * *Files identical despite different names*

### Comparing `mlh-0.0.7/mlh/woe.py` & `mlh-0.0.8/mlh/woe.py`

 * *Files identical despite different names*

### Comparing `mlh-0.0.7/mlh.egg-info/PKG-INFO` & `mlh-0.0.8/mlh.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlh
-Version: 0.0.7
+Version: 0.0.8
 Summary: This package provides helper utilities for machine learning tasks. One major utility is calculation of weight of evidence
 Home-page: https://github.com/devsahu99/mlh
 Author: Devendra Kumar Sahu
 Author-email: devsahu99@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mlh-0.0.7/setup.py` & `mlh-0.0.8/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="mlh",
-    version = '0.0.7',
+    version = '0.0.8',
     author="Devendra Kumar Sahu",
     author_email="devsahu99@gmail.com",
     description="This package provides helper utilities for machine learning tasks. One major utility is calculation of weight of evidence",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/devsahu99/mlh",
     packages=['mlh'],
```

