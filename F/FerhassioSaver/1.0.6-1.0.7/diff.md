# Comparing `tmp/FerhassioSaver-1.0.6.tar.gz` & `tmp/FerhassioSaver-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FerhassioSaver-1.0.6.tar", last modified: Wed Oct 26 09:37:32 2022, max compression
+gzip compressed data, was "FerhassioSaver-1.0.7.tar", last modified: Fri Aug  4 12:17:47 2023, max compression
```

## Comparing `FerhassioSaver-1.0.6.tar` & `FerhassioSaver-1.0.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2022-10-26 09:37:32.849247 FerhassioSaver-1.0.6/
--rw-rw-rw-   0        0        0     1091 2022-10-24 11:32:37.000000 FerhassioSaver-1.0.6/LICENSE
--rw-rw-rw-   0        0        0     1756 2022-10-26 09:37:32.849247 FerhassioSaver-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     1380 2022-10-25 10:03:05.000000 FerhassioSaver-1.0.6/README.md
--rw-rw-rw-   0        0        0      478 2022-10-26 09:36:20.000000 FerhassioSaver-1.0.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-10-26 09:37:32.849247 FerhassioSaver-1.0.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2022-10-26 09:37:32.844545 FerhassioSaver-1.0.6/src/
-drwxrwxrwx   0        0        0        0 2022-10-26 09:37:32.848405 FerhassioSaver-1.0.6/src/FerhassioSaver.egg-info/
--rw-rw-rw-   0        0        0     1756 2022-10-26 09:37:32.000000 FerhassioSaver-1.0.6/src/FerhassioSaver.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      238 2022-10-26 09:37:32.000000 FerhassioSaver-1.0.6/src/FerhassioSaver.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-10-26 09:37:32.000000 FerhassioSaver-1.0.6/src/FerhassioSaver.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2022-10-26 09:37:32.000000 FerhassioSaver-1.0.6/src/FerhassioSaver.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4559 2022-10-26 09:36:20.000000 FerhassioSaver-1.0.6/src/FerhassioSaver.py
--rw-rw-rw-   0        0        0        0 2022-10-24 10:54:11.000000 FerhassioSaver-1.0.6/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-04 12:17:47.721210 FerhassioSaver-1.0.7/
+-rw-rw-rw-   0        0        0     1091 2023-08-04 12:12:07.000000 FerhassioSaver-1.0.7/LICENSE
+-rw-rw-rw-   0        0        0     1759 2023-08-04 12:17:47.720214 FerhassioSaver-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1380 2023-08-04 12:12:07.000000 FerhassioSaver-1.0.7/README.md
+-rw-rw-rw-   0        0        0      481 2023-08-04 12:15:00.000000 FerhassioSaver-1.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-04 12:17:47.721210 FerhassioSaver-1.0.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-04 12:17:47.708246 FerhassioSaver-1.0.7/src/
+drwxrwxrwx   0        0        0        0 2023-08-04 12:17:47.719216 FerhassioSaver-1.0.7/src/FerhassioSaver.egg-info/
+-rw-rw-rw-   0        0        0     1759 2023-08-04 12:17:47.000000 FerhassioSaver-1.0.7/src/FerhassioSaver.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      238 2023-08-04 12:17:47.000000 FerhassioSaver-1.0.7/src/FerhassioSaver.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-04 12:17:47.000000 FerhassioSaver-1.0.7/src/FerhassioSaver.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-08-04 12:17:47.000000 FerhassioSaver-1.0.7/src/FerhassioSaver.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4666 2023-08-04 12:15:00.000000 FerhassioSaver-1.0.7/src/FerhassioSaver.py
+-rw-rw-rw-   0        0        0        0 2023-08-04 12:12:07.000000 FerhassioSaver-1.0.7/src/__init__.py
```

### Comparing `FerhassioSaver-1.0.6/LICENSE` & `FerhassioSaver-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `FerhassioSaver-1.0.6/PKG-INFO` & `FerhassioSaver-1.0.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: FerhassioSaver
-Version: 1.0.6
+Version: 1.0.7
 Summary: Python-arango wrapper
-Author-email: Ferhassio <michael@itiva.ge>
+Author-email: Ferhassio <ferhassio@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Ferhassio Saver
 
 *Arango wrapper for 
 https://github.com/ArangoDB-Community/python-arango*
```

### Comparing `FerhassioSaver-1.0.6/README.md` & `FerhassioSaver-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `FerhassioSaver-1.0.6/src/FerhassioSaver.egg-info/PKG-INFO` & `FerhassioSaver-1.0.7/src/FerhassioSaver.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: FerhassioSaver
-Version: 1.0.6
+Version: 1.0.7
 Summary: Python-arango wrapper
-Author-email: Ferhassio <michael@itiva.ge>
+Author-email: Ferhassio <ferhassio@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Ferhassio Saver
 
 *Arango wrapper for 
 https://github.com/ArangoDB-Community/python-arango*
```

### Comparing `FerhassioSaver-1.0.6/src/FerhassioSaver.py` & `FerhassioSaver-1.0.7/src/FerhassioSaver.py`

 * *Files 10% similar despite different names*

```diff
@@ -70,31 +70,32 @@
                                             f"RETURN doc")
             fetched_data = [document for document in job]
         else:
             raise AttributeError
 
         return fetched_data
 
-    def load_data(self, json_list: list, chunk_size: int, on_duplicate = 'replace') -> None:
+    def load_data(self, json_list: list, chunk_size: int, on_duplicate: str = 'replace', overwrite: bool = False) -> None:
         """
         Save to ArangoDB
         :param chunk_size: Chunk size for worker
         :param json_list: List of jsons from page
+        :param overwrite: Overwrite data in dab or not
         :param on_duplicate: replace(default), update, ignore
         :return: None
         """
         self.workers_count = 0
         self.time_spent = 0
 
         transaction_start_time = time.time()
 
         chunk_generator = [json_list[i:i + chunk_size] for i in range(0, len(json_list), chunk_size)]
 
         for chunk in chunk_generator:
-            self.async_coll.import_bulk(chunk, on_duplicate=on_duplicate)
+            self.async_coll.import_bulk(chunk, on_duplicate=on_duplicate, overwrite=overwrite)
             self.workers_count += 1
 
         transaction_end_time = time.time()
         self.time_spent += round(transaction_end_time - transaction_start_time, 5)
 
     def load_once(self, doc: dict, overwrite_mode='update') -> None:
         """
```

