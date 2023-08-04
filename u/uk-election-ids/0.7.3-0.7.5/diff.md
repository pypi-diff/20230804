# Comparing `tmp/uk_election_ids-0.7.3.tar.gz` & `tmp/uk_election_ids-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uk_election_ids-0.7.3.tar", last modified: Wed Apr 12 20:06:20 2023, max compression
+gzip compressed data, was "uk_election_ids-0.7.5.tar", last modified: Fri Aug  4 08:03:29 2023, max compression
```

## Comparing `uk_election_ids-0.7.3.tar` & `uk_election_ids-0.7.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:06:20.256075 uk_election_ids-0.7.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-12 20:06:09.000000 uk_election_ids-0.7.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-12 20:06:09.000000 uk_election_ids-0.7.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-04-12 20:06:20.256075 uk_election_ids-0.7.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-04-12 20:06:09.000000 uk_election_ids-0.7.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 20:06:20.256075 uk_election_ids-0.7.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-04-12 20:06:09.000000 uk_election_ids-0.7.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:06:20.256075 uk_election_ids-0.7.3/uk_election_ids/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 20:06:09.000000 uk_election_ids-0.7.3/uk_election_ids/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:06:20.256075 uk_election_ids-0.7.3/uk_election_ids/data/
--rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-04-12 20:06:09.000000 uk_election_ids-0.7.3/uk_election_ids/data/id_requirements.json
--rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-04-12 20:06:09.000000 uk_election_ids-0.7.3/uk_election_ids/data/voting_systems.json
--rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-04-12 20:06:09.000000 uk_election_ids-0.7.3/uk_election_ids/datapackage.py
--rw-r--r--   0 runner    (1001) docker     (123)    13999 2023-04-12 20:06:09.000000 uk_election_ids-0.7.3/uk_election_ids/election_ids.py
--rw-r--r--   0 runner    (1001) docker     (123)     4580 2023-04-12 20:06:09.000000 uk_election_ids-0.7.3/uk_election_ids/metadata_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-04-12 20:06:09.000000 uk_election_ids-0.7.3/uk_election_ids/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-04-12 20:06:09.000000 uk_election_ids-0.7.3/uk_election_ids/slugger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:06:20.256075 uk_election_ids-0.7.3/uk_election_ids.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-04-12 20:06:20.000000 uk_election_ids-0.7.3/uk_election_ids.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-04-12 20:06:20.000000 uk_election_ids-0.7.3/uk_election_ids.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 20:06:20.000000 uk_election_ids-0.7.3/uk_election_ids.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-12 20:06:20.000000 uk_election_ids-0.7.3/uk_election_ids.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-12 20:06:20.000000 uk_election_ids-0.7.3/uk_election_ids.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 08:03:29.630542 uk_election_ids-0.7.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-08-04 08:03:14.000000 uk_election_ids-0.7.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-04 08:03:14.000000 uk_election_ids-0.7.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-08-04 08:03:29.630542 uk_election_ids-0.7.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-08-04 08:03:14.000000 uk_election_ids-0.7.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 08:03:29.630542 uk_election_ids-0.7.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-08-04 08:03:14.000000 uk_election_ids-0.7.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 08:03:29.626542 uk_election_ids-0.7.5/uk_election_ids/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 08:03:14.000000 uk_election_ids-0.7.5/uk_election_ids/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 08:03:29.630542 uk_election_ids-0.7.5/uk_election_ids/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-08-04 08:03:14.000000 uk_election_ids-0.7.5/uk_election_ids/data/id_requirements.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-08-04 08:03:14.000000 uk_election_ids-0.7.5/uk_election_ids/data/voting_systems.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-08-04 08:03:14.000000 uk_election_ids-0.7.5/uk_election_ids/datapackage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13999 2023-08-04 08:03:14.000000 uk_election_ids-0.7.5/uk_election_ids/election_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4580 2023-08-04 08:03:14.000000 uk_election_ids-0.7.5/uk_election_ids/metadata_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-08-04 08:03:14.000000 uk_election_ids-0.7.5/uk_election_ids/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-08-04 08:03:14.000000 uk_election_ids-0.7.5/uk_election_ids/slugger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 08:03:29.630542 uk_election_ids-0.7.5/uk_election_ids.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-08-04 08:03:29.000000 uk_election_ids-0.7.5/uk_election_ids.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-08-04 08:03:29.000000 uk_election_ids-0.7.5/uk_election_ids.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 08:03:29.000000 uk_election_ids-0.7.5/uk_election_ids.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-08-04 08:03:29.000000 uk_election_ids-0.7.5/uk_election_ids.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-04 08:03:29.000000 uk_election_ids-0.7.5/uk_election_ids.egg-info/top_level.txt
```

### Comparing `uk_election_ids-0.7.3/LICENSE` & `uk_election_ids-0.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `uk_election_ids-0.7.3/PKG-INFO` & `uk_election_ids-0.7.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uk_election_ids
-Version: 0.7.3
+Version: 0.7.5
 Summary: Create Democracy Club Election Identifiers
 Home-page: https://github.com/DemocracyClub/uk-election-ids/
 Author: chris48s
 License: MIT
 Project-URL: Documentation, https://democracyclub.github.io/uk-election-ids/
 Project-URL: Source, https://github.com/DemocracyClub/uk-election-ids/
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `uk_election_ids-0.7.3/README.md` & `uk_election_ids-0.7.5/README.md`

 * *Files identical despite different names*

### Comparing `uk_election_ids-0.7.3/setup.py` & `uk_election_ids-0.7.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
             return f.read()
     except IOError:
         return ""
 
 
 setup(
     name="uk_election_ids",
-    version="0.7.3",
+    version="0.7.5",
     author="chris48s",
     license="MIT",
     url="https://github.com/DemocracyClub/uk-election-ids/",
     packages=["uk_election_ids"],
     package_data={"uk_election_ids": ["data/*.json"]},
     description="Create Democracy Club Election Identifiers",
     long_description=_get_description(),
```

### Comparing `uk_election_ids-0.7.3/uk_election_ids/data/id_requirements.json` & `uk_election_ids-0.7.5/uk_election_ids/data/id_requirements.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.984375%*

 * *Differences: {"'id_type'": "{'pilot-2019': {'name': '2019 voter ID pilot scheme'}}"}*

```diff
@@ -179,11 +179,11 @@
         "EFA-2002": {
             "name": "Electoral Fraud (Northern Ireland) Act 2002"
         },
         "pilot-2018": {
             "name": "2018 voter ID pilot scheme"
         },
         "pilot-2019": {
-            "name": "2018 voter ID pilot scheme"
+            "name": "2019 voter ID pilot scheme"
         }
     }
 }
```

### Comparing `uk_election_ids-0.7.3/uk_election_ids/data/voting_systems.json` & `uk_election_ids-0.7.5/uk_election_ids/data/voting_systems.json`

 * *Files identical despite different names*

### Comparing `uk_election_ids-0.7.3/uk_election_ids/datapackage.py` & `uk_election_ids-0.7.5/uk_election_ids/datapackage.py`

 * *Files identical despite different names*

### Comparing `uk_election_ids-0.7.3/uk_election_ids/election_ids.py` & `uk_election_ids-0.7.5/uk_election_ids/election_ids.py`

 * *Files identical despite different names*

### Comparing `uk_election_ids-0.7.3/uk_election_ids/metadata_tools.py` & `uk_election_ids-0.7.5/uk_election_ids/metadata_tools.py`

 * *Files identical despite different names*

### Comparing `uk_election_ids-0.7.3/uk_election_ids/parser.py` & `uk_election_ids-0.7.5/uk_election_ids/parser.py`

 * *Files identical despite different names*

### Comparing `uk_election_ids-0.7.3/uk_election_ids/slugger.py` & `uk_election_ids-0.7.5/uk_election_ids/slugger.py`

 * *Files identical despite different names*

### Comparing `uk_election_ids-0.7.3/uk_election_ids.egg-info/PKG-INFO` & `uk_election_ids-0.7.5/uk_election_ids.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uk-election-ids
-Version: 0.7.3
+Version: 0.7.5
 Summary: Create Democracy Club Election Identifiers
 Home-page: https://github.com/DemocracyClub/uk-election-ids/
 Author: chris48s
 License: MIT
 Project-URL: Documentation, https://democracyclub.github.io/uk-election-ids/
 Project-URL: Source, https://github.com/DemocracyClub/uk-election-ids/
 Classifier: License :: OSI Approved :: MIT License
```

