# Comparing `tmp/dtintegrations-0.5.1.tar.gz` & `tmp/dtintegrations-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dtintegrations-0.5.1.tar", last modified: Thu Feb 10 14:02:57 2022, max compression
+gzip compressed data, was "dtintegrations-0.6.0.tar", last modified: Fri Aug  4 13:33:02 2023, max compression
```

## Comparing `dtintegrations-0.5.1.tar` & `dtintegrations-0.6.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-10 14:02:57.052890 dtintegrations-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (121)     1092 2022-02-10 14:02:45.000000 dtintegrations-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     3221 2022-02-10 14:02:57.056890 dtintegrations-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2306 2022-02-10 14:02:45.000000 dtintegrations-0.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-10 14:02:57.052890 dtintegrations-0.5.1/dtintegrations/
--rw-r--r--   0 runner    (1001) docker     (121)      147 2022-02-10 14:02:45.000000 dtintegrations-0.5.1/dtintegrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-10 14:02:57.052890 dtintegrations-0.5.1/dtintegrations/data_connector/
--rw-r--r--   0 runner    (1001) docker     (121)       81 2022-02-10 14:02:45.000000 dtintegrations-0.5.1/dtintegrations/data_connector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5808 2022-02-10 14:02:45.000000 dtintegrations-0.5.1/dtintegrations/data_connector/http_push.py
--rw-r--r--   0 runner    (1001) docker     (121)      942 2022-02-10 14:02:45.000000 dtintegrations-0.5.1/dtintegrations/data_connector/metadata.py
--rw-r--r--   0 runner    (1001) docker     (121)     3262 2022-02-10 14:02:45.000000 dtintegrations-0.5.1/dtintegrations/outputs.py
--rw-r--r--   0 runner    (1001) docker     (121)     2439 2022-02-10 14:02:45.000000 dtintegrations-0.5.1/dtintegrations/provider.py
--rw-r--r--   0 runner    (1001) docker     (121)     1218 2022-02-10 14:02:45.000000 dtintegrations-0.5.1/dtintegrations/request.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-10 14:02:57.052890 dtintegrations-0.5.1/dtintegrations.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3221 2022-02-10 14:02:56.000000 dtintegrations-0.5.1/dtintegrations.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      458 2022-02-10 14:02:56.000000 dtintegrations-0.5.1/dtintegrations.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-10 14:02:56.000000 dtintegrations-0.5.1/dtintegrations.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      156 2022-02-10 14:02:56.000000 dtintegrations-0.5.1/dtintegrations.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-02-10 14:02:56.000000 dtintegrations-0.5.1/dtintegrations.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1179 2022-02-10 14:02:57.056890 dtintegrations-0.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       92 2022-02-10 14:02:45.000000 dtintegrations-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:33:02.688609 dtintegrations-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-08-04 13:32:51.000000 dtintegrations-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-08-04 13:33:02.688609 dtintegrations-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-08-04 13:32:51.000000 dtintegrations-0.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:33:02.688609 dtintegrations-0.6.0/dtintegrations/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-08-04 13:32:51.000000 dtintegrations-0.6.0/dtintegrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:33:02.688609 dtintegrations-0.6.0/dtintegrations/data_connector/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-08-04 13:32:51.000000 dtintegrations-0.6.0/dtintegrations/data_connector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5808 2023-08-04 13:32:51.000000 dtintegrations-0.6.0/dtintegrations/data_connector/http_push.py
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-08-04 13:32:51.000000 dtintegrations-0.6.0/dtintegrations/data_connector/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-08-04 13:32:51.000000 dtintegrations-0.6.0/dtintegrations/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-08-04 13:32:51.000000 dtintegrations-0.6.0/dtintegrations/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-08-04 13:32:51.000000 dtintegrations-0.6.0/dtintegrations/request.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:33:02.688609 dtintegrations-0.6.0/dtintegrations.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-08-04 13:33:02.000000 dtintegrations-0.6.0/dtintegrations.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-08-04 13:33:02.000000 dtintegrations-0.6.0/dtintegrations.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 13:33:02.000000 dtintegrations-0.6.0/dtintegrations.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-08-04 13:33:02.000000 dtintegrations-0.6.0/dtintegrations.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-04 13:33:02.000000 dtintegrations-0.6.0/dtintegrations.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-08-04 13:33:02.692609 dtintegrations-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-08-04 13:32:51.000000 dtintegrations-0.6.0/setup.py
```

### Comparing `dtintegrations-0.5.1/LICENSE` & `dtintegrations-0.6.0/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2021 Disruptive Technologies Research AS
+Copyright (c) 2023 Disruptive Technologies Research AS
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `dtintegrations-0.5.1/PKG-INFO` & `dtintegrations-0.6.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 Metadata-Version: 2.1
 Name: dtintegrations
-Version: 0.5.1
+Version: 0.6.0
 Summary: Disruptive Technologies Python Integrations.
 Home-page: https://github.com/disruptive-technologies/disruptive-dataconnector
 Author: Disruptive Technologies Research AS
 Author-email: developer-support@disruptive-technologies.com
-License: UNKNOWN
 Keywords: disruptive,technologies,dt,integration,api
-Platform: UNKNOWN
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # Disruptive Technologies Python Integrations
 
 ![build](https://github.com/disruptive-technologies/python-integrations/actions/workflows/build.yml/badge.svg)
@@ -44,15 +42,15 @@
 
 ```sh
 pip install .
 ```
 
 ### Requirements
 
-- Python 3.7, 3.8, 3.9, 3.10
+- Python 3.8, 3.9, 3.10, 3.11
 
 ## Usage
 Currently, the main functionality of this package is validating requests forwarded by a [Data Connector](https://developer.disruptive-technologies.com/docs/data-connectors/introduction-to-data-connector).  
 
 The following example shows this for a [Google Cloud Function](https://cloud.google.com/functions).
 ```python
 from dtintegrations import data_connector, provider
@@ -95,9 +93,7 @@
 make lint
 ```
 
 Build the package distribution:
 ```
 make build
 ```
-
-
```

### Comparing `dtintegrations-0.5.1/README.md` & `dtintegrations-0.6.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 ```sh
 pip install .
 ```
 
 ### Requirements
 
-- Python 3.7, 3.8, 3.9, 3.10
+- Python 3.8, 3.9, 3.10, 3.11
 
 ## Usage
 Currently, the main functionality of this package is validating requests forwarded by a [Data Connector](https://developer.disruptive-technologies.com/docs/data-connectors/introduction-to-data-connector).  
 
 The following example shows this for a [Google Cloud Function](https://cloud.google.com/functions).
 ```python
 from dtintegrations import data_connector, provider
```

### Comparing `dtintegrations-0.5.1/dtintegrations/data_connector/http_push.py` & `dtintegrations-0.6.0/dtintegrations/data_connector/http_push.py`

 * *Files identical despite different names*

### Comparing `dtintegrations-0.5.1/dtintegrations/data_connector/metadata.py` & `dtintegrations-0.6.0/dtintegrations/data_connector/metadata.py`

 * *Files identical despite different names*

### Comparing `dtintegrations-0.5.1/dtintegrations/outputs.py` & `dtintegrations-0.6.0/dtintegrations/outputs.py`

 * *Files identical despite different names*

### Comparing `dtintegrations-0.5.1/dtintegrations/provider.py` & `dtintegrations-0.6.0/dtintegrations/provider.py`

 * *Files identical despite different names*

### Comparing `dtintegrations-0.5.1/dtintegrations/request.py` & `dtintegrations-0.6.0/dtintegrations/request.py`

 * *Files identical despite different names*

### Comparing `dtintegrations-0.5.1/dtintegrations.egg-info/PKG-INFO` & `dtintegrations-0.6.0/dtintegrations.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 Metadata-Version: 2.1
 Name: dtintegrations
-Version: 0.5.1
+Version: 0.6.0
 Summary: Disruptive Technologies Python Integrations.
 Home-page: https://github.com/disruptive-technologies/disruptive-dataconnector
 Author: Disruptive Technologies Research AS
 Author-email: developer-support@disruptive-technologies.com
-License: UNKNOWN
 Keywords: disruptive,technologies,dt,integration,api
-Platform: UNKNOWN
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # Disruptive Technologies Python Integrations
 
 ![build](https://github.com/disruptive-technologies/python-integrations/actions/workflows/build.yml/badge.svg)
@@ -44,15 +42,15 @@
 
 ```sh
 pip install .
 ```
 
 ### Requirements
 
-- Python 3.7, 3.8, 3.9, 3.10
+- Python 3.8, 3.9, 3.10, 3.11
 
 ## Usage
 Currently, the main functionality of this package is validating requests forwarded by a [Data Connector](https://developer.disruptive-technologies.com/docs/data-connectors/introduction-to-data-connector).  
 
 The following example shows this for a [Google Cloud Function](https://cloud.google.com/functions).
 ```python
 from dtintegrations import data_connector, provider
@@ -95,9 +93,7 @@
 make lint
 ```
 
 Build the package distribution:
 ```
 make build
 ```
-
-
```

### Comparing `dtintegrations-0.5.1/setup.cfg` & `dtintegrations-0.6.0/setup.cfg`

 * *Files 25% similar despite different names*

```diff
@@ -15,25 +15,24 @@
 	api
 license_file = LICENSE
 classifiers = 
 	Natural Language :: English
 	License :: OSI Approved :: MIT License
 	Development Status :: 3 - Alpha
 	Intended Audience :: Developers
-	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Operating System :: OS Independent
 
 [options]
-python_requires = >=3.7
+python_requires = >=3.8
 install_requires = 
-	pyjwt >= 2.0.0, < 3.0.0
-	disruptive >= 0.6.0
+	disruptive >= 1.6.0
 packages = find:
 
 [options.packages.find]
 exclude = 
 	tests
 	tests.*
```

