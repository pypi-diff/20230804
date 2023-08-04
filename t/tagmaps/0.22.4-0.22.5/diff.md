# Comparing `tmp/tagmaps-0.22.4.tar.gz` & `tmp/tagmaps-0.22.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tagmaps-0.22.4.tar", last modified: Fri Jul 21 09:31:09 2023, max compression
+gzip compressed data, was "tagmaps-0.22.5.tar", last modified: Fri Aug  4 06:57:25 2023, max compression
```

## Comparing `tagmaps-0.22.4.tar` & `tagmaps-0.22.5.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-07-21 09:31:09.745502 tagmaps-0.22.4/
--rw-r--r--   0 alex      (1000) alex      (1000)     9421 2023-07-21 09:30:35.000000 tagmaps-0.22.4/CHANGELOG.md
--rwxrwxrwx   0 alex      (1000) alex      (1000)    34940 2019-01-29 10:06:07.000000 tagmaps-0.22.4/LICENSE.md
--rw-r--r--   0 alex      (1000) alex      (1000)      164 2023-05-16 10:04:37.000000 tagmaps-0.22.4/MANIFEST.in
--rw-r--r--   0 alex      (1000) alex      (1000)    12288 2023-07-21 09:31:09.729434 tagmaps-0.22.4/PKG-INFO
--rw-r--r--   0 alex      (1000) alex      (1000)    12137 2023-05-16 10:05:32.000000 tagmaps-0.22.4/README.md
--rw-r--r--   0 alex      (1000) alex      (1000)     2195 2023-07-21 09:30:11.000000 tagmaps-0.22.4/pyproject.toml
--rw-r--r--   0 alex      (1000) alex      (1000)       38 2023-07-21 09:31:09.746506 tagmaps-0.22.4/setup.cfg
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-07-21 09:31:09.268733 tagmaps-0.22.4/src/
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-07-21 09:31:09.421664 tagmaps-0.22.4/src/tagmaps/
--rw-r--r--   0 alex      (1000) alex      (1000)      620 2023-05-16 10:04:38.000000 tagmaps-0.22.4/src/tagmaps/__init__.py
--rw-r--r--   0 alex      (1000) alex      (1000)     5914 2023-05-16 10:04:38.000000 tagmaps-0.22.4/src/tagmaps/__main__.py
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-07-21 09:31:09.660687 tagmaps-0.22.4/src/tagmaps/classes/
--rw-r--r--   0 alex      (1000) alex      (1000)       33 2023-05-16 10:04:38.000000 tagmaps-0.22.4/src/tagmaps/classes/__init__.py
--rw-r--r--   0 alex      (1000) alex      (1000)    17470 2023-07-17 11:20:03.000000 tagmaps-0.22.4/src/tagmaps/classes/alpha_shapes.py
--rw-r--r--   0 alex      (1000) alex      (1000)    41054 2023-05-16 10:04:38.000000 tagmaps-0.22.4/src/tagmaps/classes/cluster.py
--rw-r--r--   0 alex      (1000) alex      (1000)    17232 2023-05-16 10:04:38.000000 tagmaps-0.22.4/src/tagmaps/classes/compile_output.py
--rw-r--r--   0 alex      (1000) alex      (1000)    23633 2023-05-16 10:04:38.000000 tagmaps-0.22.4/src/tagmaps/classes/interface.py
--rw-r--r--   0 alex      (1000) alex      (1000)    17745 2023-05-16 10:04:38.000000 tagmaps-0.22.4/src/tagmaps/classes/load_data.py
--rw-r--r--   0 alex      (1000) alex      (1000)    10479 2023-05-16 10:04:38.000000 tagmaps-0.22.4/src/tagmaps/classes/plotting.py
--rw-r--r--   0 alex      (1000) alex      (1000)    32505 2023-05-16 10:04:38.000000 tagmaps-0.22.4/src/tagmaps/classes/prepare_data.py
--rw-r--r--   0 alex      (1000) alex      (1000)     9578 2023-05-16 10:04:38.000000 tagmaps-0.22.4/src/tagmaps/classes/shared_structure.py
--rw-r--r--   0 alex      (1000) alex      (1000)    21911 2023-05-16 10:04:38.000000 tagmaps-0.22.4/src/tagmaps/classes/utils.py
--rw-r--r--   0 alex      (1000) alex      (1000)       75 2023-05-16 10:04:38.000000 tagmaps-0.22.4/src/tagmaps/classes/write_output.py
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-07-21 09:31:09.674243 tagmaps-0.22.4/src/tagmaps/config/
--rw-r--r--   0 alex      (1000) alex      (1000)       39 2023-05-16 10:04:38.000000 tagmaps-0.22.4/src/tagmaps/config/__init__.py
--rw-r--r--   0 alex      (1000) alex      (1000)    26041 2023-05-16 10:04:38.000000 tagmaps-0.22.4/src/tagmaps/config/config.py
--rw-r--r--   0 alex      (1000) alex      (1000)    31972 2023-05-16 10:04:39.000000 tagmaps-0.22.4/src/tagmaps/matplotlibrc
--rw-r--r--   0 alex      (1000) alex      (1000)    19100 2023-05-16 10:04:39.000000 tagmaps-0.22.4/src/tagmaps/tagmaps_.py
--rw-r--r--   0 alex      (1000) alex      (1000)       46 2023-07-21 09:30:35.000000 tagmaps-0.22.4/src/tagmaps/version.py
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-07-21 09:31:09.464716 tagmaps-0.22.4/src/tagmaps.egg-info/
--rwxrwxrwx   0 alex      (1000) alex      (1000)    12288 2023-07-21 09:31:09.000000 tagmaps-0.22.4/src/tagmaps.egg-info/PKG-INFO
--rwxrwxrwx   0 alex      (1000) alex      (1000)      885 2023-07-21 09:31:09.000000 tagmaps-0.22.4/src/tagmaps.egg-info/SOURCES.txt
--rwxrwxrwx   0 alex      (1000) alex      (1000)        1 2023-07-21 09:31:09.000000 tagmaps-0.22.4/src/tagmaps.egg-info/dependency_links.txt
--rwxrwxrwx   0 alex      (1000) alex      (1000)       50 2023-07-21 09:31:09.000000 tagmaps-0.22.4/src/tagmaps.egg-info/entry_points.txt
--rwxrwxrwx   0 alex      (1000) alex      (1000)      110 2023-07-21 09:31:09.000000 tagmaps-0.22.4/src/tagmaps.egg-info/requires.txt
--rwxrwxrwx   0 alex      (1000) alex      (1000)        8 2023-07-21 09:31:09.000000 tagmaps-0.22.4/src/tagmaps.egg-info/top_level.txt
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-07-21 09:31:09.726434 tagmaps-0.22.4/tests/
--rw-r--r--   0 alex      (1000) alex      (1000)      627 2023-05-16 10:04:39.000000 tagmaps-0.22.4/tests/test_all.py
--rwxrwxrwx   0 alex      (1000) alex      (1000)     3271 2019-02-22 14:26:36.000000 tagmaps-0.22.4/tests/test_emoji.py
--rwxrwxrwx   0 alex      (1000) alex      (1000)      934 2019-01-29 10:06:07.000000 tagmaps-0.22.4/tests/test_post.py
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-08-04 06:57:25.852204 tagmaps-0.22.5/
+-rw-r--r--   0 alex      (1000) alex      (1000)    97811 2023-08-04 06:55:32.000000 tagmaps-0.22.5/CHANGELOG.md
+-rwxrwxrwx   0 alex      (1000) alex      (1000)    34940 2019-01-29 10:06:07.000000 tagmaps-0.22.5/LICENSE.md
+-rw-r--r--   0 alex      (1000) alex      (1000)      164 2023-05-16 10:04:37.000000 tagmaps-0.22.5/MANIFEST.in
+-rw-r--r--   0 alex      (1000) alex      (1000)    12288 2023-08-04 06:57:25.839204 tagmaps-0.22.5/PKG-INFO
+-rw-r--r--   0 alex      (1000) alex      (1000)    12137 2023-05-16 10:05:32.000000 tagmaps-0.22.5/README.md
+-rw-r--r--   0 alex      (1000) alex      (1000)     2204 2023-08-04 06:49:37.000000 tagmaps-0.22.5/pyproject.toml
+-rw-r--r--   0 alex      (1000) alex      (1000)       38 2023-08-04 06:57:25.853036 tagmaps-0.22.5/setup.cfg
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-08-04 06:57:25.469664 tagmaps-0.22.5/src/
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-08-04 06:57:25.610927 tagmaps-0.22.5/src/tagmaps/
+-rw-r--r--   0 alex      (1000) alex      (1000)      620 2023-05-16 10:04:38.000000 tagmaps-0.22.5/src/tagmaps/__init__.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     5914 2023-05-16 10:04:38.000000 tagmaps-0.22.5/src/tagmaps/__main__.py
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-08-04 06:57:25.767921 tagmaps-0.22.5/src/tagmaps/classes/
+-rw-r--r--   0 alex      (1000) alex      (1000)       33 2023-05-16 10:04:38.000000 tagmaps-0.22.5/src/tagmaps/classes/__init__.py
+-rw-r--r--   0 alex      (1000) alex      (1000)    17470 2023-08-04 06:25:10.000000 tagmaps-0.22.5/src/tagmaps/classes/alpha_shapes.py
+-rw-r--r--   0 alex      (1000) alex      (1000)    41054 2023-05-16 10:04:38.000000 tagmaps-0.22.5/src/tagmaps/classes/cluster.py
+-rw-r--r--   0 alex      (1000) alex      (1000)    17232 2023-05-16 10:04:38.000000 tagmaps-0.22.5/src/tagmaps/classes/compile_output.py
+-rw-r--r--   0 alex      (1000) alex      (1000)    23633 2023-05-16 10:04:38.000000 tagmaps-0.22.5/src/tagmaps/classes/interface.py
+-rw-r--r--   0 alex      (1000) alex      (1000)    17826 2023-08-04 06:49:34.000000 tagmaps-0.22.5/src/tagmaps/classes/load_data.py
+-rw-r--r--   0 alex      (1000) alex      (1000)    10479 2023-05-16 10:04:38.000000 tagmaps-0.22.5/src/tagmaps/classes/plotting.py
+-rw-r--r--   0 alex      (1000) alex      (1000)    32505 2023-05-16 10:04:38.000000 tagmaps-0.22.5/src/tagmaps/classes/prepare_data.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     9578 2023-05-16 10:04:38.000000 tagmaps-0.22.5/src/tagmaps/classes/shared_structure.py
+-rw-r--r--   0 alex      (1000) alex      (1000)    21649 2023-08-04 06:49:36.000000 tagmaps-0.22.5/src/tagmaps/classes/utils.py
+-rw-r--r--   0 alex      (1000) alex      (1000)       75 2023-05-16 10:04:38.000000 tagmaps-0.22.5/src/tagmaps/classes/write_output.py
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-08-04 06:57:25.791235 tagmaps-0.22.5/src/tagmaps/config/
+-rw-r--r--   0 alex      (1000) alex      (1000)       39 2023-05-16 10:04:38.000000 tagmaps-0.22.5/src/tagmaps/config/__init__.py
+-rw-r--r--   0 alex      (1000) alex      (1000)    26041 2023-05-16 10:04:38.000000 tagmaps-0.22.5/src/tagmaps/config/config.py
+-rw-r--r--   0 alex      (1000) alex      (1000)    31972 2023-05-16 10:04:39.000000 tagmaps-0.22.5/src/tagmaps/matplotlibrc
+-rw-r--r--   0 alex      (1000) alex      (1000)    19100 2023-05-16 10:04:39.000000 tagmaps-0.22.5/src/tagmaps/tagmaps_.py
+-rwxrwxrwx   0 alex      (1000) alex      (1000)       46 2023-08-04 06:55:54.000000 tagmaps-0.22.5/src/tagmaps/version.py
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-08-04 06:57:25.641492 tagmaps-0.22.5/src/tagmaps.egg-info/
+-rwxrwxrwx   0 alex      (1000) alex      (1000)    12288 2023-08-04 06:57:25.000000 tagmaps-0.22.5/src/tagmaps.egg-info/PKG-INFO
+-rwxrwxrwx   0 alex      (1000) alex      (1000)      885 2023-08-04 06:57:25.000000 tagmaps-0.22.5/src/tagmaps.egg-info/SOURCES.txt
+-rwxrwxrwx   0 alex      (1000) alex      (1000)        1 2023-08-04 06:57:25.000000 tagmaps-0.22.5/src/tagmaps.egg-info/dependency_links.txt
+-rwxrwxrwx   0 alex      (1000) alex      (1000)       50 2023-08-04 06:57:25.000000 tagmaps-0.22.5/src/tagmaps.egg-info/entry_points.txt
+-rwxrwxrwx   0 alex      (1000) alex      (1000)      117 2023-08-04 06:57:25.000000 tagmaps-0.22.5/src/tagmaps.egg-info/requires.txt
+-rwxrwxrwx   0 alex      (1000) alex      (1000)        8 2023-08-04 06:57:25.000000 tagmaps-0.22.5/src/tagmaps.egg-info/top_level.txt
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-08-04 06:57:25.827755 tagmaps-0.22.5/tests/
+-rw-r--r--   0 alex      (1000) alex      (1000)      627 2023-05-16 10:04:39.000000 tagmaps-0.22.5/tests/test_all.py
+-rwxrwxrwx   0 alex      (1000) alex      (1000)     3271 2019-02-22 14:26:36.000000 tagmaps-0.22.5/tests/test_emoji.py
+-rwxrwxrwx   0 alex      (1000) alex      (1000)      934 2019-01-29 10:06:07.000000 tagmaps-0.22.5/tests/test_post.py
```

### Comparing `tagmaps-0.22.4/LICENSE.md` & `tagmaps-0.22.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `tagmaps-0.22.4/PKG-INFO` & `tagmaps-0.22.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tagmaps
-Version: 0.22.4
+Version: 0.22.5
 Summary: Tag Clustering for Tag Maps
 Author-email: Alexander Dunkel <alexander.dunkel@tu-dresden.de>
 License: GNU GPLv3 or any higher
 Project-URL: Homepage, https://github.com/Sieboldianus/TagMaps
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `tagmaps-0.22.4/README.md` & `tagmaps-0.22.5/README.md`

 * *Files identical despite different names*

### Comparing `tagmaps-0.22.4/pyproject.toml` & `tagmaps-0.22.5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 dependencies = [
     "fiona",
     "shapely",
     "pandas>=0.24.2",
     "pyproj>=2.0.0",
     "numpy",
     "matplotlib>=3.0.0",
-    "emoji>=2.0.0",
+    "emoji>=2.7.0, < 3.0.0",
     "hdbscan>=0.8.31",
     "seaborn",
     "scipy",
 ]
 dynamic = ["version"]
 
 [project.readme]
```

### Comparing `tagmaps-0.22.4/src/tagmaps/__init__.py` & `tagmaps-0.22.5/src/tagmaps/__init__.py`

 * *Files identical despite different names*

### Comparing `tagmaps-0.22.4/src/tagmaps/__main__.py` & `tagmaps-0.22.5/src/tagmaps/__main__.py`

 * *Files identical despite different names*

### Comparing `tagmaps-0.22.4/src/tagmaps/classes/alpha_shapes.py` & `tagmaps-0.22.5/src/tagmaps/classes/alpha_shapes.py`

 * *Files identical despite different names*

### Comparing `tagmaps-0.22.4/src/tagmaps/classes/cluster.py` & `tagmaps-0.22.5/src/tagmaps/classes/cluster.py`

 * *Files identical despite different names*

### Comparing `tagmaps-0.22.4/src/tagmaps/classes/compile_output.py` & `tagmaps-0.22.5/src/tagmaps/classes/compile_output.py`

 * *Files identical despite different names*

### Comparing `tagmaps-0.22.4/src/tagmaps/classes/interface.py` & `tagmaps-0.22.5/src/tagmaps/classes/interface.py`

 * *Files identical despite different names*

### Comparing `tagmaps-0.22.4/src/tagmaps/classes/load_data.py` & `tagmaps-0.22.5/src/tagmaps/classes/load_data.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,33 +11,30 @@
 from __future__ import absolute_import
 
 import csv
 import json
 import logging
 import sys
 from decimal import Decimal
-from typing import (IO, Any, Dict, Iterable, Iterator, Optional, OrderedDict,
-                    Set, Tuple)
+from typing import IO, Any, Dict, Iterable, Iterator, Optional, OrderedDict, Set, Tuple
 
 from shapely.geometry import Point
 
 from tagmaps.classes.shared_structure import AnalysisBounds, PostStructure
 from tagmaps.classes.utils import Utils
 
 
-class LoadData():
+class LoadData:
     """Main Class for ingesting data
 
     - will apply basic filters (based on stoplists etc.)
     - Returns CleanedPost
     """
 
-    def __init__(
-            self, cfg, user_variety_input=None,
-            console_reporting=None):
+    def __init__(self, cfg, user_variety_input=None, console_reporting=None):
         """Initializes Load Data structure"""
         if user_variety_input is None:
             user_variety_input = False
         if console_reporting is None:
             console_reporting = False
         self.filelist = self._read_local_files(cfg)
         self.guid_hash = set()  # global list of guids
@@ -67,111 +64,111 @@
         """Main pipeline for reading posts from file
 
         Combine multiple generators to single pipeline
         that is returned for being processed by
         with-statement.
         """
         post_pipeline = self._parse_postlist(
-            self._process_inputfile(
-                self._parse_input_files(count=True)))
+            self._process_inputfile(self._parse_input_files(count=True))
+        )
         return post_pipeline
 
     def __exit__(self, c_type, value, traceback):
         """Contextmanager exit: nothing to do here"""
         return False
 
     def _parse_input_files(self, count: bool = None) -> Iterator[IO[str]]:
         """Loops input input filelist and
         returns opened file handles
         """
         for file_name in self.filelist:
             if count:
                 self.stats.partcount += 1
             self.current_file = file_name.stem
-            yield open(file_name, 'r', newline='', encoding='utf8')
+            yield open(file_name, "r", newline="", encoding="utf8")
 
     def is_intermediate(self):
         """Auto test if intermediate data is present"""
-        post_reader = next(self._process_inputfile(
-            self._parse_input_files(
-                count=False)))
+        post_reader = next(
+            self._process_inputfile(self._parse_input_files(count=False))
+        )
         for post in post_reader:
             pguid = post.get(self.cfg.source_map.post_guid_col)
             if pguid is None and post.get("guid") is not None:
                 # if column name is "guid",
                 # data is likely of type intermediate
-                self.log.info(
-                    "Intermediate data detected.. skipping filtering step.\n")
+                self.log.info("Intermediate data detected.. skipping filtering step.\n")
                 return True
             return False
 
-    def _process_inputfile(
-            self, file_handles: Iterator[IO[str]]) -> Iterator[Any]:
+    def _process_inputfile(self, file_handles: Iterator[IO[str]]) -> Iterator[Any]:
         """File parse for CSV or JSON from open file handle
 
         Output: produces a list of post that can be parsed
         """
         post_reader = []
         for file_handle in file_handles:
             if self.cfg.source_map.file_extension == "csv":
                 post_reader = csv.DictReader(
                     file_handle,
                     delimiter=self.cfg.source_map.delimiter,
                     quotechar=self.cfg.source_map.quote_char,
-                    quoting=self.cfg.source_map.quoting)
+                    quoting=self.cfg.source_map.quoting,
+                )
                 # next(post_list, None)  # skip headerline
             elif self.cfg.source_map.file_extension == "json":
-                post_reader = post_reader + json.loads(
-                    file_handle.read())
+                post_reader = post_reader + json.loads(file_handle.read())
             yield post_reader
 
-    def _parse_postlist(
-            self, post_readers: Iterable[OrderedDict[str, Optional[str]]]):
+    def _parse_postlist(self, post_readers: Iterable[OrderedDict[str, Optional[str]]]):
         """Process posts according to specifications
 
         Returns generator for single record
         """
         # row_num = 0
         msg = None
         for post_reader in post_readers:
             Utils.check_fileheader(
-                post_reader.fieldnames, self.cfg.source_map, self.current_file)
+                post_reader.fieldnames, self.cfg.source_map, self.current_file
+            )
             for post in post_reader:
                 # row_num += 1
                 lbsn_post = self._parse_post(post)
                 if lbsn_post is None:
                     continue
                 else:
                     self.stats.count_glob += 1
                     msg = self._report_progress()
                     # if (row_num % 10 == 0):
                     # modulo: print only once every 10 iterations
                     if self.console_reporting:
-                        print(msg, end='\r')
+                        print(msg, end="\r")
                 yield lbsn_post
         # log last message to file, clean stdout
         if msg and self.console_reporting:
-            print(" " * len(msg), end='\r')
+            print(" " * len(msg), end="\r")
         sys.stdout.flush()
         if self.stats.count_glob == 0:
             raise ValueError(
                 f"No posts found in input data. "
-                f"First file: {next(iter(self.filelist or []), None)}.")
+                f"First file: {next(iter(self.filelist or []), None)}."
+            )
         self.log.info(msg)
 
     def _report_progress(self):
         """Status report"""
         msg = (
-            f'Cleaned input to {len(self.distinct_locations_set):02d} '
-            f'distinct locations from '
-            f'{self.stats.count_glob:02d} posts '
-            f'(File {self.stats.partcount} of {len(self.filelist)}) - '
-            f'Skipped posts: {self.stats.skipped_count} - skipped tags: '
-            f'{self.stats.count_tags_skipped} of '
-            f'{self.stats.count_tags_global}')
+            f"Cleaned input to {len(self.distinct_locations_set):02d} "
+            f"distinct locations from "
+            f"{self.stats.count_glob:02d} posts "
+            f"(File {self.stats.partcount} of {len(self.filelist)}) - "
+            f"Skipped posts: {self.stats.skipped_count} - skipped tags: "
+            f"{self.stats.count_tags_skipped} of "
+            f"{self.stats.count_tags_global}"
+        )
         return msg
 
     def _parse_post(self, post: Dict[str, str]) -> Optional[PostStructure]:
         """Process single post and attach to common structure"""
         # skip duplicates and erroneous entries
         post_guid = post.get(self.cfg.source_map.post_guid_col)
         if post_guid in self.guid_hash:
@@ -179,216 +176,236 @@
             return None
         if post_guid is None:
             raise ValueError(f"Post guid is None: {post}")
         self.guid_hash.add(post_guid)
         origin_id = post.get(self.cfg.source_map.originid_col)
         if origin_id is None:
             origin_id = 0
-        if (self.filter_origin and
-                not origin_id == self.filter_origin):
+        if self.filter_origin and not origin_id == self.filter_origin:
             # optional exclude origin
             self.stats.skipped_count += 1
             return None
         user_guid = post.get(self.cfg.source_map.user_guid_col)
         if user_guid is None:
             raise ValueError(f"User guid is None: {post}")
-        if not self.cfg.ignore_stoplists and \
-                self.cfg.sort_out_user_set is not None \
-                and user_guid in self.cfg.sort_out_user_set:
+        if (
+            not self.cfg.ignore_stoplists
+            and self.cfg.sort_out_user_set is not None
+            and user_guid in self.cfg.sort_out_user_set
+        ):
             return None
         # Continue Parse Post
         lbsn_post = PostStructure(
-            origin_id=int(origin_id), guid=post_guid, user_guid=user_guid)
+            origin_id=int(origin_id), guid=post_guid, user_guid=user_guid
+        )
         lbsn_post.post_url = post.get(self.cfg.source_map.post_url_col)
-        lbsn_post.post_publish_date = \
-            post.get(self.cfg.source_map.post_publish_date_col)
+        lbsn_post.post_publish_date = post.get(
+            self.cfg.source_map.post_publish_date_col
+        )
         # Process Spatial Query first (if skipping necessary)
-        if self.cfg.sort_out_places and \
-                self._is_sortout_place(post):
+        if self.cfg.sort_out_places and self._is_sortout_place(post):
             return None
         lat = None
         lng = None
         if self._is_empty_latlng(post):
             if self.ignore_empty_latlng:
                 pass
             else:
                 return None
         else:
             # assign lat/lng coordinates from dict
             lat, lng = self._correct_placelatlng(
                 post.get(self.cfg.source_map.place_guid_col),
                 post.get(self.cfg.source_map.latitude_col),
-                post.get(self.cfg.source_map.longitude_col)
+                post.get(self.cfg.source_map.longitude_col),
             )
             # update boundary
             self.bounds.upd_latlng_bounds(lat, lng)
             lbsn_post.latitude = lat
             lbsn_post.longitude = lng
         if lat is None or lng is None:
             # Try to substitude place_guid
             # if self.ignore_empty_latlng has been set to True
-            lbsn_post.loc_id = post.get(
-                self.cfg.source_map.place_guid_col)
+            lbsn_post.loc_id = post.get(self.cfg.source_map.place_guid_col)
             if not lbsn_post.loc_id:
-                self.log.warning('Neither coordinates nor place guid found.')
+                self.log.warning("Neither coordinates nor place guid found.")
         else:
             # Note: loc_id not loaded from file
             # create loc_id from lat/lng
-            lbsn_post.loc_id = f'{lat}:{lng}'
+            lbsn_post.loc_id = f"{lat}:{lng}"
         # counting of distinct loc ids
         self.distinct_locations_set.add(lbsn_post.loc_id)
         lbsn_post.loc_name = post.get(self.cfg.source_map.place_name_col)
         # exclude posts outside boundary
-        if (self.cfg.shapefile_intersect or self.cfg.shapefile_exclude) and \
-                self._is_outside_shapebounds(lbsn_post) is True:
+        if (
+            self.cfg.shapefile_intersect or self.cfg.shapefile_exclude
+        ) and self._is_outside_shapebounds(lbsn_post) is True:
             return None
-        if self.cfg.cluster_tags or \
-                self.cfg.cluster_emoji or \
-                self.cfg.topic_modeling:
+        if self.cfg.cluster_tags or self.cfg.cluster_emoji or self.cfg.topic_modeling:
             post_body = post.get(self.cfg.source_map.post_body_col)
             post_title = post.get(self.cfg.source_map.post_title_col)
             if self.cfg.ignore_stoplists:
                 lbsn_post.post_body = post_body
                 lbsn_post.post_title = post_title
             else:
                 if self.cfg.select_tags_set is not None:
                     # if positive filterlist available
                     lbsn_post.post_body = Utils.select_words(
-                        post_body, self.cfg.select_tags_set)
+                        post_body, self.cfg.select_tags_set
+                    )
                     lbsn_post.post_title = Utils.select_words(
-                        post_title, self.cfg.select_tags_set)
+                        post_title, self.cfg.select_tags_set
+                    )
                 else:
                     # check against stoplists
                     lbsn_post.post_body = Utils.remove_stopwords(
-                        post_body, self.cfg.sort_out_always_set)
+                        post_body, self.cfg.sort_out_always_set
+                    )
                     lbsn_post.post_title = Utils.remove_stopwords(
-                        post_title, self.cfg.sort_out_always_set)
+                        post_title, self.cfg.sort_out_always_set
+                    )
         else:
             lbsn_post.post_title = ""
             lbsn_post.post_body = ""
         lbsn_post.post_like_count = self._get_count_frompost(
-            post.get(self.cfg.source_map.post_like_count_col))
+            post.get(self.cfg.source_map.post_like_count_col)
+        )
         lbsn_post.hashtags = set()
         if self.cfg.cluster_tags or self.cfg.topic_modeling:
-            lbsn_post.hashtags = self._get_tags(
-                post.get(self.cfg.source_map.tags_col))
+            lbsn_post.hashtags = self._get_tags(post.get(self.cfg.source_map.tags_col))
         if self.cfg.cluster_emoji:
-            lbsn_post.emoji = self._get_emoji(lbsn_post.post_body)
-            # no merge anymore:
-            # lbsn_post.hashtags = set.union(post_emoji)
-        lbsn_post.post_create_date = \
-            post.get(self.cfg.source_map.post_create_date_col)
+            lbsn_post.emoji = self._get_emoji(post)
+        lbsn_post.post_create_date = post.get(self.cfg.source_map.post_create_date_col)
         lbsn_post.post_views_count = self._get_count_frompost(
-            post.get(self.cfg.source_map.post_views_count_col))
+            post.get(self.cfg.source_map.post_views_count_col)
+        )
         # return parsed post object
         return lbsn_post
 
     @staticmethod
     def _read_local_files(config):
         """Read Local Files according to config parameters
 
         - returns list of file-paths
         """
         input_path = config.input_folder
-        filelist = list(input_path.glob(
-            f'*.{config.source_map.file_extension}'))
+        filelist = list(input_path.glob(f"*.{config.source_map.file_extension}"))
         input_count = len(filelist)
         if input_count == 0:
             raise ValueError(
-                f'No input files *.'
-                f'{config.source_map.file_extension} '
-                f'in ./{input_path.name}/ found.')
+                f"No input files *."
+                f"{config.source_map.file_extension} "
+                f"in ./{input_path.name}/ found."
+            )
         return filelist
 
     @staticmethod
     def _get_count_frompost(count_string: Optional[str]) -> int:
         """Parse post like count field"""
         if count_string and not count_string == "":
             try:
                 photo_likes_int = int(count_string)
                 return photo_likes_int
             except TypeError:
                 logging.getLogger("tagmaps").debug(
-                    f'\nPost like count parser: Type Error: '
-                    f'{type(count_string)} not a valid number format '
-                    f'Returning 0.')
+                    f"\nPost like count parser: Type Error: "
+                    f"{type(count_string)} not a valid number format "
+                    f"Returning 0."
+                )
             except ValueError:
                 logging.getLogger("tagmaps").debug(
-                    f'\nPost like count parser: Value Error: '
-                    f'{count_string} not a valid number. '
-                    f'Returning 0.')
+                    f"\nPost like count parser: Value Error: "
+                    f"{count_string} not a valid number. "
+                    f"Returning 0."
+                )
         return 0
 
-    def _get_emoji(self, post_body: Optional[str]) -> Set[str]:
-        """extract emoji, use selection list if available"""
-        emoji_filtered = Utils.select_emoji(
-            Utils.extract_emoji(post_body), self.cfg.select_emoji_set)
+    def _get_emoji(self, post: Dict[str, str]) -> Set[str]:
+        """Extract emoji from post_body and emoji col,
+        use selection list if available
+        """
+        emoji_body = Utils.select_emoji(
+            Utils.extract_emoji(post.get(self.cfg.source_map.post_body_col)),
+            self.cfg.select_emoji_set,
+        )
+        emoji_col = Utils.select_emoji(post.get(self.cfg.source_map.emoji_col))
+        emoji_filtered = set.union(emoji_body, emoji_col)
         if emoji_filtered:
             self.stats.count_emojis_global += len(emoji_filtered)
         return emoji_filtered
 
     def _get_tags(self, tags_string: Optional[str]) -> Set[str]:
-        """extract tags, apply filter lists if available"""
+        """Extract tags, apply filter lists if available"""
         # base str conversion to set
         tags = set(filter(None, tags_string.lower().split(";")))
         # Filter tags based on two stoplists
         if self.cfg.ignore_stoplists:
             count_tags = len(tags)
             count_skipped = 0
         else:
-            tags, count_tags, count_skipped = \
-                Utils.filter_tags(
-                    tags,
-                    self.cfg.sort_out_always_set,
-                    self.cfg.sort_out_always_instr_set,
-                    self.cfg.select_tags_set
-                )
+            tags, count_tags, count_skipped = Utils.filter_tags(
+                tags,
+                self.cfg.sort_out_always_set,
+                self.cfg.sort_out_always_instr_set,
+                self.cfg.select_tags_set,
+            )
         # update global stats
         self.stats.count_tags_global += count_tags
         self.stats.count_tags_skipped += count_skipped
         return tags
 
     def _correct_placelatlng(
-            self, place_guid_string: Optional[str], lat, lng) -> Tuple[Decimal, Decimal]:
+        self, place_guid_string: Optional[str], lat, lng
+    ) -> Tuple[Decimal, Decimal]:
         """If place corrections available, update lat/lng coordinates
         Needs test: not place_guid_string
         """
-        if (self.cfg.correct_places and not place_guid_string and
-                place_guid_string in self.cfg.correct_place_latlng_dict):
+        if (
+            self.cfg.correct_places
+            and not place_guid_string
+            and place_guid_string in self.cfg.correct_place_latlng_dict
+        ):
             lat = Decimal(
                 # correct lat
-                self.cfg.correct_place_latlng_dict[place_guid_string][0])
+                self.cfg.correct_place_latlng_dict[place_guid_string][0]
+            )
             lng = Decimal(
                 # correct lng
-                self.cfg.correct_place_latlng_dict[place_guid_string][1])
+                self.cfg.correct_place_latlng_dict[place_guid_string][1]
+            )
         else:
             # return original lat/lng
             lat = Decimal(lat)  # original lat
             lng = Decimal(lng)  # original lng
         return lat, lng
 
     def _is_outside_shapebounds(self, post):
-        """Skip all posts outside shapefile """
+        """Skip all posts outside shapefile"""
         # do not expensive spatial check twice:
         if post.loc_id in self.shape_exclude_locid_hash:
             self.stats.skipped_count += 1
             return True
         if post.loc_id not in self.shape_included_locid_hash:
             lng_lat_point = Point(post.longitude, post.latitude)
-            if Utils.check_intersect_polylist(
-                    lng_lat_point, self.cfg.shapefile_intersect,
-                    self.cfg.shapefile_exclude) is False:
+            if (
+                Utils.check_intersect_polylist(
+                    lng_lat_point,
+                    self.cfg.shapefile_intersect,
+                    self.cfg.shapefile_exclude,
+                )
+                is False
+            ):
                 self.stats.skipped_count += 1
                 self.shape_exclude_locid_hash.add(post.loc_id)
                 return True
             self.shape_included_locid_hash.add(post.loc_id)
         return False
 
     def _is_empty_latlng(self, post):
-        """ skip non-geotagged medias"""
+        """skip non-geotagged medias"""
         latitude = post.get(self.cfg.source_map.latitude_col)
         longitude = post.get(self.cfg.source_map.longitude_col)
         if not latitude or not longitude:
             self.stats.count_non_geotagged += 1
             return True
         return False
 
@@ -402,38 +419,31 @@
         return False
 
     def _get_imax(self):
         """User Input to get number of tags to process"""
         if self.cfg.auto_mode:
             return
         if self.cfg.cluster_tags or self.cfg.cluster_emoji:
-            inputtext = \
-                input(f'Files to process: {len(self.filelist)}. \nOptional: '
-                      f'Enter a Number for the variety of tags to process '
-                      f'(default is 1000)\nPress Enter to proceed.. \n')
-            if inputtext is None \
-                    or inputtext == "" \
-                    or not inputtext.isdigit():
+            inputtext = input(
+                f"Files to process: {len(self.filelist)}. \nOptional: "
+                f"Enter a Number for the variety of tags to process "
+                f"(default is 1000)\nPress Enter to proceed.. \n"
+            )
+            if inputtext is None or inputtext == "" or not inputtext.isdigit():
                 return
             self.cfg.max_items = int(inputtext)
 
     def input_stats_report(self):
         """Return input stats"""
-        self.log.info(
-            f'\nTotal post count (PC): '
-            f'{self.stats.count_glob:02d}')
-        self.log.info(
-            f'Total tag count (PTC): '
-            f'{self.stats.count_tags_global}')
-        self.log.info(
-            f'Total emoji count (PEC): '
-            f'{self.stats.count_emojis_global}')
+        self.log.info(f"\nTotal post count (PC): " f"{self.stats.count_glob:02d}")
+        self.log.info(f"Total tag count (PTC): " f"{self.stats.count_tags_global}")
+        self.log.info(f"Total emoji count (PEC): " f"{self.stats.count_emojis_global}")
 
 
-class DataStats():
+class DataStats:
     """Class storing basic data stats"""
 
     def __init__(self):
         """Initialize stats."""
         self.count_glob = 0
         self.partcount = 0
         self.skipped_count = 0
```

### Comparing `tagmaps-0.22.4/src/tagmaps/classes/plotting.py` & `tagmaps-0.22.5/src/tagmaps/classes/plotting.py`

 * *Files identical despite different names*

### Comparing `tagmaps-0.22.4/src/tagmaps/classes/prepare_data.py` & `tagmaps-0.22.5/src/tagmaps/classes/prepare_data.py`

 * *Files identical despite different names*

### Comparing `tagmaps-0.22.4/src/tagmaps/classes/shared_structure.py` & `tagmaps-0.22.5/src/tagmaps/classes/shared_structure.py`

 * *Files identical despite different names*

### Comparing `tagmaps-0.22.4/src/tagmaps/classes/utils.py` & `tagmaps-0.22.5/src/tagmaps/classes/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,139 +19,138 @@
 from collections import namedtuple
 from datetime import timedelta
 from importlib import reload
 from math import asin, cos, radians, sin, sqrt
 from pathlib import Path
 from typing import Dict, Iterable, List, Optional, Set, Tuple, Union
 
-from emoji import distinct_emoji_list
+from emoji.core import distinct_emoji_list, demojize
 import numpy as np
 import pyproj
 import shapely.geometry as geometry
 
 from ..classes.shared_structure import AnalysisBounds, ConfigMap, ItemCounter
 
 
-class Utils():
+class Utils:
     """Collection of various tools and helper functions
 
     Primarily @classmethods and @staticmethods
     """
 
     @staticmethod
-    def check_folder_file(
-            folder_file: Path, create_folder: bool = None) -> Path:
+    def check_folder_file(folder_file: Path, create_folder: bool = None) -> Path:
         """Check if folder exists, optionally create it"""
         if not folder_file.exists():
             pname = "File"
             if folder_file.is_dir():
                 return folder_file
             pname = "Folder"
             if create_folder:
                 Utils.init_dir(folder_file)
                 return folder_file
             raise ValueError(f"{pname} {folder_file} not found.")
         return folder_file
 
     @staticmethod
     def check_fileheader(
-            fieldnames: Iterable[str],
-            source_map: ConfigMap, filename: Optional[str]):
+        fieldnames: Iterable[str], source_map: ConfigMap, filename: Optional[str]
+    ):
         """Checks against existing file columns
         warns if required keys are missing
 
         Args:
             source_map (ConfigMap): Custom headers definition
             Note: the type hint above makes use of forward-references
             defined in PEP 484, as a means to avoid cyclic imports
         """
         header_req = [
             source_map.post_guid_col,
             source_map.user_guid_col,
             source_map.latitude_col,
             source_map.longitude_col,
-            source_map.tags_col]
+            source_map.tags_col,
+        ]
         for header in header_req:
             if header not in fieldnames:
                 raise Warning(
-                    f'File header is missing "{header}"-column, '
-                    f'file: {filename}')
+                    f'File header is missing "{header}"-column, ' f"file: {filename}"
+                )
 
     @staticmethod
     def _count_none(str_list: Union[Dict[str, str], List[str]]) -> int:
         """Return count of list, returns zero for None"""
         if str_list is None:
             return 0
         return len(str_list)
 
     @staticmethod
     def report_listload(list_ref, str_text):
         """Report only if list_ref contains at least 1 entry."""
         entry_count = Utils._count_none(list_ref)
         if entry_count > 0:
-            logging.getLogger("tagmaps").info(
-                f"Loaded {entry_count} {str_text}.")
+            logging.getLogger("tagmaps").info(f"Loaded {entry_count} {str_text}.")
 
     @staticmethod
     def concat_topic(term_list):
         """Concatenate list of terms (e.g. TOPIC) to string"""
-        if any('-' in s for s in term_list):
-            raise ValueError(
-                "No '-' characters supported in topic list terms")
-        topic_name = '-'.join(term_list)
+        if any("-" in s for s in term_list):
+            raise ValueError("No '-' characters supported in topic list terms")
+        topic_name = "-".join(term_list)
         return topic_name
 
     @staticmethod
     def split_topic(term_concat):
         """Split concat topic"""
-        topic_terms = term_concat.split('-')
+        topic_terms = term_concat.split("-")
         return topic_terms
 
     @staticmethod
     def set_proj_dir():
         """Update PROJ_LIB location if not found
 
         Leftover from pyproj < 2.0.0 compatibility,
         PROJ_LIB not needed anymore
         """
-        if not os.environ.get('PROJ_LIB'):
+        if not os.environ.get("PROJ_LIB"):
             local_proj_path = Path.cwd() / "proj"
             if not local_proj_path.exists():
-                raise ValueError("Pyproj 'proj' datadir not found. Either specify "
-                                 "PROJ_LIB environmental variable or copy 'proj' "
-                                 "folder to local path of executable")
-            os.environ['PROJ_LIB'] = str(local_proj_path)
+                raise ValueError(
+                    "Pyproj 'proj' datadir not found. Either specify "
+                    "PROJ_LIB environmental variable or copy 'proj' "
+                    "folder to local path of executable"
+                )
+            os.environ["PROJ_LIB"] = str(local_proj_path)
             pyproj.datadir.set_data_dir(str(local_proj_path))
 
     @staticmethod
-    def get_shapely_bounds(
-            bounds: AnalysisBounds) -> geometry.MultiPoint:
+    def get_shapely_bounds(bounds: AnalysisBounds) -> geometry.MultiPoint:
         """Returns boundary shape from 4 coordinates"""
-        bound_points_shapely = geometry.MultiPoint([
-            (bounds.lim_lng_min, bounds.lim_lat_min),
-            (bounds.lim_lng_max, bounds.lim_lat_max)
-        ])
+        bound_points_shapely = geometry.MultiPoint(
+            [
+                (bounds.lim_lng_min, bounds.lim_lat_min),
+                (bounds.lim_lng_max, bounds.lim_lat_max),
+            ]
+        )
         return bound_points_shapely
 
     @staticmethod
-    def get_best_utmzone(
-            bound_points_shapely: geometry.MultiPoint):
+    def get_best_utmzone(bound_points_shapely: geometry.MultiPoint):
         """Calculate best UTM Zone SRID/EPSG Code
         Args:
         True centroid (coords may be multipoint)"""
         input_lon_center = bound_points_shapely.centroid.coords[0][0]
         input_lat_center = bound_points_shapely.centroid.coords[0][1]
-        epsg_code = Utils._convert_wgs_to_utm(
-            input_lon_center, input_lat_center)
-        crs_proj = f'epsg:{epsg_code}'
+        epsg_code = Utils._convert_wgs_to_utm(input_lon_center, input_lat_center)
+        crs_proj = f"epsg:{epsg_code}"
         return crs_proj, epsg_code
 
     @staticmethod
     def _convert_wgs_to_utm(lon: float, lat: float):
-        """"Return best epsg code for pair
+        """ "Return best epsg code for pair
         of WGS coordinates (lat/lng)
 
         Args:
             lon: latitude
             lat: longitude
 
         Returns:
@@ -161,108 +160,107 @@
         https://gis.stackexchange.com/questions/269518/auto-select-suitable-utm-zone-based-on-grid-intersection/
         https://stackoverflow.com/questions/40132542/get-a-cartesian-projection-accurate-around-a-lat-lng-pair
         https://gis.stackexchange.com/questions/127427/transforming-shapely-polygon-and-multipolygon-objects
         """
 
         utm_band = str((math.floor((lon + 180) / 6) % 60) + 1)
         if len(utm_band) == 1:
-            utm_band = '0'+utm_band
+            utm_band = "0" + utm_band
         if lat >= 0:
-            epsg_code = '326' + utm_band
+            epsg_code = "326" + utm_band
         else:
-            epsg_code = '327' + utm_band
+            epsg_code = "327" + utm_band
         return epsg_code
 
     @staticmethod
     def encode_string(text_s):
         """Encode string in Sha256,
         produce hex
 
         - returns a string of double length,
         containing only hexadecimal digits"""
-        encoded_string = hashlib.sha3_256(
-            text_s.encode("utf8")).hexdigest()
+        encoded_string = hashlib.sha3_256(text_s.encode("utf8")).hexdigest()
         return encoded_string
 
     @staticmethod
     def remove_special_chars(text_s):
         """Removes a list of special chars from string"""
         special_chars = "?.!/;:,[]()'-&#|<>=\""
-        s_cleaned = text_s.translate(
-            {ord(c): " " for c in special_chars})
+        s_cleaned = text_s.translate({ord(c): " " for c in special_chars})
         return s_cleaned
 
     @staticmethod
     def select_words(text_s, selection_list: List[str]) -> str:
         """Filters a string based on a provided
         positive filter list of terms
 
         - removes duplicate terms
         """
         # first remove hyperlinks
         text_s = Utils.remove_hyperlinks(text_s)
         # split string by space character into list
         querywords = text_s.split()
-        resultwords = {word for word in querywords if word.lower()
-                       in selection_list}
-        s_cleaned = ' '.join(resultwords)
+        resultwords = {word for word in querywords if word.lower() in selection_list}
+        s_cleaned = " ".join(resultwords)
         return s_cleaned
 
     @staticmethod
     def select_emoji(
-            input_emoji_set: Set[str],
-            selection_emoji_set: Set[str] = None) -> Set[str]:
-        """Filters a set of emoji based on another set
-        """
+        input_emoji_set: Set[str], selection_emoji_set: Set[str] = None
+    ) -> Set[str]:
+        """Filters a set of emoji based on another set"""
         if selection_emoji_set is None:
             # no filter on empty selection list
             return input_emoji_set
         filtered_emoji_set = {
-            emoji for emoji in input_emoji_set if emoji in selection_emoji_set}
+            emoji for emoji in input_emoji_set if emoji in selection_emoji_set
+        }
         return filtered_emoji_set
 
     @staticmethod
     def remove_stopwords(text_s, stopwords: List[str]) -> str:
         """Removes a list of words from string,
         including hyperlinks (<a></a>) and
         integer numbers (e.g. 2012)
         """
         # first remove hyperlinks
         text_s = Utils.remove_hyperlinks(text_s)
         # split string by space character into list
         querywords = text_s.split()
         # clean list by matching against stopwords
-        resultwords = [word for word in querywords if word.lower()
-                       not in stopwords and not word.isdigit()]
-        s_cleaned = ' '.join(resultwords)
+        resultwords = [
+            word
+            for word in querywords
+            if word.lower() not in stopwords and not word.isdigit()
+        ]
+        s_cleaned = " ".join(resultwords)
         return s_cleaned
 
     @staticmethod
     def remove_hyperlinks(text_s):
         """Regex to remove any hyperlinks from string
 
         Note:
         - anything between <a>xxx</a> will be kept
         """
-        pattern = r'<(a|/a).*?>'
+        pattern = r"<(a|/a).*?>"
         result = re.sub(pattern, "", text_s)
         return result
 
     @staticmethod
     def _is_number(number_s):
         """Check if variable is number (float)"""
         try:
             float(number_s)
             return True
         except ValueError:
             return False
 
     @staticmethod
-    def check_intersect_polylist(
-            latlng_point, polylist, poly_exclude_list=None):
+    def check_intersect_polylist(latlng_point, polylist, poly_exclude_list=None):
         """Checks intersection of Point(lat, lng) against
         list of polygons.
 
         Arguments:
             latlng_point {Fiona Point} -- coordinate
             polylist {list} -- list of polys
             poly_exclude_list {list} -- list of polys to exclude
@@ -293,21 +291,21 @@
         TODO:
         - disables fiona logging, as it (somehow)
           interferes with tag maps logging
           (find better solution)
         """
         # set console view parameters
         # stretch console
-        if platform.system() == 'Windows':
-            os.system('mode con: cols=197 lines=500')
+        if platform.system() == "Windows":
+            os.system("mode con: cols=197 lines=500")
         logging.getLogger("fiona.collection").disabled = True
 
     @staticmethod
     def set_logger(output_folder: Path = None, logging_level=None):
-        """ Set logging handler manually,
+        """Set logging handler manually,
         so we can also print to console while logging to file
         """
         # reset logging in case Jupyter Notebook has
         # captured stdout
         reload(logging)
         # Create or get logger with specific name
         log = logging.getLogger("tagmaps")
@@ -320,104 +318,104 @@
             return log
         if logging_level is None:
             logging_level = logging.INFO
         if output_folder is not None:
             if not output_folder.exists():
                 Utils.init_dir(output_folder)
             # input(f'{type(output_folder)}')
-            __log_file = output_folder / 'log.txt'
-        log.format = '%(message)s'  # type: ignore
-        log.datefmt = ''  # type: ignore
+            __log_file = output_folder / "log.txt"
+        log.format = "%(message)s"  # type: ignore
+        log.datefmt = ""  # type: ignore
         log.setLevel(logging_level)
         # Set Output to Replace in case of
         # encoding issues (console/windows)
         if isinstance(sys.stdout, io.TextIOWrapper):
             # only for console output (not Juypter Notebook stream)
             sys.stdout = io.TextIOWrapper(
-                sys.stdout.detach(), sys.stdout.encoding, 'replace')  # type: ignore
+                sys.stdout.detach(), sys.stdout.encoding, "replace"
+            )  # type: ignore
             log.addHandler(logging.StreamHandler())
             if output_folder is not None:
                 # only log to file in console mode
                 log.addHandler(
-                    logging.FileHandler(__log_file, 'w', 'utf-8'))  # type: ignore
+                    logging.FileHandler(__log_file, "w", "utf-8")
+                )  # type: ignore
         else:
             # log to stdout, not stderr in Jupyter Mode to prevent
             # log.Info messages appear as red boxes
             logging.basicConfig(
-                stream=sys.stdout, format=log.format,  # type: ignore
-                level=logging_level, datefmt=None)
+                stream=sys.stdout,
+                format=log.format,  # type: ignore
+                level=logging_level,
+                datefmt=None,
+            )
             # log.stream = sys.stdout
         # flush once to clear console
         # sys.stdout.flush()
         return log
 
     @staticmethod
     def init_dir(path_folder: Path):
         """Creates local dir if not exists"""
         if not path_folder.exists():
             path_folder.mkdir()
-            print(f'Folder {path_folder.name}/ was created')
+            print(f"Folder {path_folder.name}/ was created")
 
     @staticmethod
     def query_yes_no(question, default="yes"):
         """Ask a yes/no question via raw_input() and return their answer.
 
         "question" is a string that is presented to the user.
         "default" is the presumed answer if the user just hits <Enter>.
             It must be "yes" (the default), "no" or None (meaning
             an answer is required of the user).
 
         The "answer" return value is True for "yes" or False for "no".
         """
-        valid = {"yes": True, "y": True, "ye": True,
-                 "no": False, "n": False}
+        valid = {"yes": True, "y": True, "ye": True, "no": False, "n": False}
         if default is None:
             prompt = " [y/n] "
         elif default == "yes":
             prompt = " [Y/n] "
         elif default == "no":
             prompt = " [y/N] "
         else:
             raise ValueError("invalid default answer: '%s'" % default)
 
         while True:
             sys.stdout.write(question + prompt)
             choice = input().lower()
-            if default is not None and choice == '':
+            if default is not None and choice == "":
                 return valid[default]
             elif choice in valid:
                 return valid[choice]
-            sys.stdout.write(
-                "'yes' or 'no' (or 'y' or 'n').\n")
+            sys.stdout.write("'yes' or 'no' (or 'y' or 'n').\n")
 
     @staticmethod
     def daterange(start_date, end_date):
         """Return time difference between two dates"""
-        for n_val in range(
-                int((end_date - start_date).days)):
+        for n_val in range(int((end_date - start_date).days)):
             yield start_date + timedelta(n_val)
 
     @staticmethod
     def haversine(lon1, lat1, lon2, lat2):
         """
         Calculate the great circle distance between two points
         on the earth (specified in decimal degrees)
         """
         # convert decimal degrees to radians
-        lon1, lat1, lon2, lat2 = map(
-            radians, [lon1, lat1, lon2, lat2])
+        lon1, lat1, lon2, lat2 = map(radians, [lon1, lat1, lon2, lat2])
         # haversine formula
         dlon = lon2 - lon1
         dlat = lat2 - lat1
-        a_value = (sin(dlat/2)**2 + cos(lat1) *
-                   cos(lat2) * sin(dlon/2)**2)
+        a_value = sin(dlat / 2) ** 2 + cos(lat1) * cos(lat2) * sin(dlon / 2) ** 2
         c_value = 2 * asin(sqrt(a_value))
         # Radius of earth in kilometers is 6371
         km_dist = 6371 * c_value
-        m_dist = km_dist*1000
+        m_dist = km_dist * 1000
         return m_dist
 
     @staticmethod
     def get_radians_from_meters(dist):
         """Get approx. distance in radians from meters
 
         Args:
@@ -430,17 +428,17 @@
         - 1 Radian is about 57.2958 degrees.
         - then see:
         https://sciencing.com/convert-distances-degrees-meters-7858322.html
         - Multiply the number of degrees by 111.325
         - To convert this to meters, multiply by 1,000.
           So, 2 degrees is about 222,65 meters.
         """
-        dist = dist/1000
-        degrees_dist = dist/111.325
-        radians_dist = degrees_dist/57.2958
+        dist = dist / 1000
+        degrees_dist = dist / 111.325
+        radians_dist = degrees_dist / 57.2958
         return radians_dist
 
     @staticmethod
     def get_meters_from_radians(dist):
         """Get approx. distance in meters from radians
         distance
 
@@ -460,42 +458,40 @@
         dist = dist * 57.2958
         dist = dist * 111.325
         meters_dist = round(dist * 1000, 1)
         return meters_dist
 
     @staticmethod
     def get_emojiname(emoji_string):
-        """"Tries to get a name representation for
+        """ "Tries to get a name representation for
         emoji. Emoji can either be a single character,
         or a number of characters that construct a grapheme cluster.
         Therefore, unicodedata.name cannot directly be applied.
         For some grapheme clusters, there exists no unicodedata.name
         """
         emoji_name = None
         # first try to get name for whole str
         if len(emoji_string) == 1:
             # if single character
             emoji_name = Utils._get_unicode_name(emoji_string)
         if not emoji_name:
             for char_s in emoji_string:
-                emoji_name = Utils._get_unicode_name(
-                    char_s)
+                emoji_name = Utils._get_unicode_name(char_s)
                 if emoji_name:
                     break
         if not emoji_name:
-            emoji_name = emoji.demojize(emoji_string)
+            emoji_name = demojize(emoji_string)
         if not emoji_name:
-            raise ValueError(f'No name found for {emoji_string}')
+            raise ValueError(f"No name found for {emoji_string}")
         return emoji_name
 
     @staticmethod
     def _get_unicode_name(emoji_string_or_char):
         try:
-            emojiname = unicodedata.name(
-                emoji_string_or_char)
+            emojiname = unicodedata.name(emoji_string_or_char)
             return emojiname
         except ValueError:
             return False
 
     @staticmethod
     def _check_emoji_type(char_unicode):
         """Checks if emoji code point is of specific type,
@@ -504,67 +500,60 @@
         EMOJI MODIFIER, VARIATION SELECTOR
         or ZERO WIDTH modifier
 
         To check: Is this method really needed?
         """
         # name = name(str_emoji)
         try:
-            if unicodedata.name(
-                    char_unicode
-            ).startswith(
-                ("EMOJI MODIFIER",
-                 "VARIATION SELECTOR",
-                 "ZERO WIDTH")
+            if unicodedata.name(char_unicode).startswith(
+                ("EMOJI MODIFIER", "VARIATION SELECTOR", "ZERO WIDTH")
             ):
                 return False
             return True
         except ValueError:
             print(char_unicode)
             return True
 
     @staticmethod
     def extract_emoji(string_with_emoji: Optional[str]) -> Set[str]:
-        """Extract emoji and flags using emoji package
-        """
+        """Extract emoji and flags using emoji package"""
         if not string_with_emoji:
             # empty
             return set()
         return set(distinct_emoji_list(string_with_emoji))
 
     @staticmethod
     def str2bool(str_text):
         """Convert any type of yes no string to
         bool representation"""
-        if str_text.lower() in (
-                'yes', 'true', 't', 'y', '1'):
+        if str_text.lower() in ("yes", "true", "t", "y", "1"):
             return True
-        elif str_text.lower() in (
-                'no', 'false', 'f', 'n', '0'):
+        elif str_text.lower() in ("no", "false", "f", "n", "0"):
             return False
-        raise argparse.ArgumentTypeError(
-            'Boolean value expected.')
+        raise argparse.ArgumentTypeError("Boolean value expected.")
 
     @staticmethod
     def get_rectangle_bounds(points):
         """Get rectangle bounds for numpy.ndarray of point coordinates"""
         RectangleBounds = namedtuple(
-            'RectangleBounds',
-            'lim_lat_min lim_lat_max lim_lng_min lim_lng_max')
+            "RectangleBounds", "lim_lat_min lim_lat_max lim_lng_min lim_lng_max"
+        )
         lim_y_min = np.min(points.T[1])
         lim_y_max = np.max(points.T[1])
         lim_x_min = np.min(points.T[0])
         lim_x_max = np.max(points.T[0])
         return RectangleBounds(lim_y_min, lim_y_max, lim_x_min, lim_x_max)
 
     @staticmethod
-    def filter_tags(taglist: Set[str],
-                    sort_out_always_set: Set[str],
-                    sort_out_always_instr_set: Set[str],
-                    select_tags_set: Set[str] = None
-                    ) -> Tuple[Set[str], int, int]:
+    def filter_tags(
+        taglist: Set[str],
+        sort_out_always_set: Set[str],
+        sort_out_always_instr_set: Set[str],
+        select_tags_set: Set[str] = None,
+    ) -> Tuple[Set[str], int, int]:
         """Filter list of tags based on two stoplists
 
         - also removes numeric items and duplicates
         - extracts only tags with len(s) > 1
         - optionally filters list according to positive selection list
 
         Args:
@@ -592,32 +581,33 @@
                     tags_filtered.add(tag)
                 else:
                     count_skipped += 1
             else:
                 # exclude numbers and those tags
                 # that are in sort_out_always_set
                 # or sort_out_always_instr_set
-                if (len(tag) == 1 or tag == '""'
-                        or tag.isdigit()
-                        or tag in sort_out_always_set):
+                if (
+                    len(tag) == 1
+                    or tag == '""'
+                    or tag.isdigit()
+                    or tag in sort_out_always_set
+                ):
                     count_skipped += 1
                     continue
                 for in_str_partial in sort_out_always_instr_set:
                     if in_str_partial in tag:
                         count_skipped += 1
                         break
                 else:
                     # final else Clause on loop statement
                     tags_filtered.add(tag)
-        return (tags_filtered,
-                count_tags, count_skipped)
+        return (tags_filtered, count_tags, count_skipped)
 
     @staticmethod
-    def get_index_of_item(
-            l_tuple_str: List[ItemCounter], value: Optional[str]) -> int:
+    def get_index_of_item(l_tuple_str: List[ItemCounter], value: Optional[str]) -> int:
         """Get index pos from list of tuples.
 
         Stops iterating through the list as
         soon as it finds the value
         """
         for pos, tuple_str in enumerate(l_tuple_str):
             if tuple_str.name == value:
```

### Comparing `tagmaps-0.22.4/src/tagmaps/config/config.py` & `tagmaps-0.22.5/src/tagmaps/config/config.py`

 * *Files identical despite different names*

### Comparing `tagmaps-0.22.4/src/tagmaps/matplotlibrc` & `tagmaps-0.22.5/src/tagmaps/matplotlibrc`

 * *Files identical despite different names*

### Comparing `tagmaps-0.22.4/src/tagmaps/tagmaps_.py` & `tagmaps-0.22.5/src/tagmaps/tagmaps_.py`

 * *Files identical despite different names*

### Comparing `tagmaps-0.22.4/src/tagmaps.egg-info/PKG-INFO` & `tagmaps-0.22.5/src/tagmaps.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tagmaps
-Version: 0.22.4
+Version: 0.22.5
 Summary: Tag Clustering for Tag Maps
 Author-email: Alexander Dunkel <alexander.dunkel@tu-dresden.de>
 License: GNU GPLv3 or any higher
 Project-URL: Homepage, https://github.com/Sieboldianus/TagMaps
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `tagmaps-0.22.4/src/tagmaps.egg-info/SOURCES.txt` & `tagmaps-0.22.5/src/tagmaps.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tagmaps-0.22.4/tests/test_all.py` & `tagmaps-0.22.5/tests/test_all.py`

 * *Files identical despite different names*

### Comparing `tagmaps-0.22.4/tests/test_emoji.py` & `tagmaps-0.22.5/tests/test_emoji.py`

 * *Files identical despite different names*

### Comparing `tagmaps-0.22.4/tests/test_post.py` & `tagmaps-0.22.5/tests/test_post.py`

 * *Files identical despite different names*

