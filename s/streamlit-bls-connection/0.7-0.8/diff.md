# Comparing `tmp/streamlit_bls_connection-0.7.tar.gz` & `tmp/streamlit_bls_connection-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit_bls_connection-0.7.tar", last modified: Sun Jul 30 01:43:15 2023, max compression
+gzip compressed data, was "streamlit_bls_connection-0.8.tar", last modified: Fri Aug  4 01:41:40 2023, max compression
```

## Comparing `streamlit_bls_connection-0.7.tar` & `streamlit_bls_connection-0.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-30 01:43:15.689288 streamlit_bls_connection-0.7/
--rw-rw-rw-   0        0        0     1089 2023-07-29 16:30:01.000000 streamlit_bls_connection-0.7/LICENSE
--rw-rw-rw-   0        0        0     4452 2023-07-30 01:43:15.689288 streamlit_bls_connection-0.7/PKG-INFO
--rw-rw-rw-   0        0        0     3562 2023-07-30 01:36:49.000000 streamlit_bls_connection-0.7/README.md
--rw-rw-rw-   0        0        0      389 2023-07-30 01:42:35.000000 streamlit_bls_connection-0.7/pyproject.toml
--rw-rw-rw-   0        0        0       86 2023-07-30 01:43:15.690286 streamlit_bls_connection-0.7/setup.cfg
--rw-rw-rw-   0        0        0     1188 2023-07-30 01:42:17.000000 streamlit_bls_connection-0.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-30 01:43:15.649024 streamlit_bls_connection-0.7/streamlit_bls_connection/
--rw-rw-rw-   0        0        0       65 2023-07-29 16:22:24.000000 streamlit_bls_connection-0.7/streamlit_bls_connection/__init__.py
--rw-rw-rw-   0        0        0     3601 2023-07-30 01:29:28.000000 streamlit_bls_connection-0.7/streamlit_bls_connection/bls_connection.py
--rw-rw-rw-   0        0        0       33 2023-07-30 01:42:56.000000 streamlit_bls_connection-0.7/streamlit_bls_connection/version.py
-drwxrwxrwx   0        0        0        0 2023-07-30 01:43:15.689288 streamlit_bls_connection-0.7/streamlit_bls_connection.egg-info/
--rw-rw-rw-   0        0        0     4452 2023-07-30 01:43:15.000000 streamlit_bls_connection-0.7/streamlit_bls_connection.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      406 2023-07-30 01:43:15.000000 streamlit_bls_connection-0.7/streamlit_bls_connection.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-30 01:43:15.000000 streamlit_bls_connection-0.7/streamlit_bls_connection.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2023-07-30 01:43:15.000000 streamlit_bls_connection-0.7/streamlit_bls_connection.egg-info/requires.txt
--rw-rw-rw-   0        0        0       25 2023-07-30 01:43:15.000000 streamlit_bls_connection-0.7/streamlit_bls_connection.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-04 01:41:40.057410 streamlit_bls_connection-0.8/
+-rw-rw-rw-   0        0        0     1089 2023-07-29 16:30:01.000000 streamlit_bls_connection-0.8/LICENSE
+-rw-rw-rw-   0        0        0     4624 2023-08-04 01:41:40.057410 streamlit_bls_connection-0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     3728 2023-08-04 01:40:35.000000 streamlit_bls_connection-0.8/README.md
+-rw-rw-rw-   0        0        0      389 2023-08-04 00:49:28.000000 streamlit_bls_connection-0.8/pyproject.toml
+-rw-rw-rw-   0        0        0       86 2023-08-04 01:41:40.058418 streamlit_bls_connection-0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1190 2023-08-04 00:53:47.000000 streamlit_bls_connection-0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-04 01:41:40.007788 streamlit_bls_connection-0.8/streamlit_bls_connection/
+-rw-rw-rw-   0        0        0       65 2023-07-29 16:22:24.000000 streamlit_bls_connection-0.8/streamlit_bls_connection/__init__.py
+-rw-rw-rw-   0        0        0    11270 2023-07-31 16:29:21.000000 streamlit_bls_connection-0.8/streamlit_bls_connection/bls_connection.py
+-rw-rw-rw-   0        0        0       33 2023-08-04 00:47:07.000000 streamlit_bls_connection-0.8/streamlit_bls_connection/version.py
+drwxrwxrwx   0        0        0        0 2023-08-04 01:41:40.056399 streamlit_bls_connection-0.8/streamlit_bls_connection.egg-info/
+-rw-rw-rw-   0        0        0     4624 2023-08-04 01:41:39.000000 streamlit_bls_connection-0.8/streamlit_bls_connection.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      406 2023-08-04 01:41:39.000000 streamlit_bls_connection-0.8/streamlit_bls_connection.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-04 01:41:39.000000 streamlit_bls_connection-0.8/streamlit_bls_connection.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-08-04 01:41:39.000000 streamlit_bls_connection-0.8/streamlit_bls_connection.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2023-08-04 01:41:39.000000 streamlit_bls_connection-0.8/streamlit_bls_connection.egg-info/top_level.txt
```

### Comparing `streamlit_bls_connection-0.7/LICENSE` & `streamlit_bls_connection-0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit_bls_connection-0.7/PKG-INFO` & `streamlit_bls_connection-0.8/streamlit_bls_connection.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: streamlit_bls_connection
-Version: 0.7
+Name: streamlit-bls-connection
+Version: 0.8
 Summary: A package to fetch Bureau of Labor Statistics data using Streamlit
 Home-page: https://github.com/tonyhollaar/
-Download-URL: https://github.com/tonyhollaar/streamlit_bls_connection/archive/refs/tags/v4.tar.gz
+Download-URL: https://github.com/tonyhollaar/streamlit_bls_connection/archive/refs/tags/v0.8.tar.gz
 Author: Tony Hollaar
 Author-email: thollaar@gmail.com
 License: MIT
 Keywords: streamlit,api,bls
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
@@ -33,34 +33,38 @@
 ## How to use `streamlit-bls-connection`
 To run the Streamlit app locally on your machine, follow these steps:
 
 ### Installation
 1. Install the `streamlit-bls-connection` package and its dependencies by running the following command in your terminal or command prompt:
 
 ```bash
-pip install streamlit-bls-connection
+pip install streamlit_bls_connection
 ```
 
 ### Create .py file
 2. Create a new Python script  with your favorite text editor (e.g., VSCode, Spyder, Notepad++), name it `app.py` and copy/paste below code and save changes.
 ```python
 import streamlit as st
 from streamlit_bls_connection import BLSConnection
 
 # Step 1: Setup connection to US Bureau of Labor Statistics
-connection = BLSConnection("bls_connection")
+conn = st.experimental_connection('bls', type=BLSConnection)
 
-# Step 2: Define Input parameters for the API call
+# Step 2: Define input parameters
 # Tip: one or multiple Series ID's* can be retrieved
+# find Series ID's on www.bls.gov > DATA TOOLS
 seriesids_list = ['APU000074714', 'APU000072610']
-start_year_str = '2014'  # start of date range
-end_year_str = '2023'    # end of date range
+start_year_str = '2014' # start of date range
+end_year_str = '2023'   # end of date range
 
 # Step 3: Fetch data using the custom connection
-dataframes_dict = connection.query(seriesids_list, start_year_str, end_year_str)
+dataframes_dict = connection.query(seriesids_list,
+                                   start_year_str, 
+                                   end_year_str,
+                                   api_key = None)
 
 # Step 4: Create dataframes
 gas_df = dataframes_dict['APU000074714']
 electricity_df = dataframes_dict['APU000072610']
 
 # Step 5: Show Dataframes in Streamlit
 st.dataframe(gas_df)
```

### Comparing `streamlit_bls_connection-0.7/README.md` & `streamlit_bls_connection-0.8/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -13,34 +13,38 @@
 ## How to use `streamlit-bls-connection`
 To run the Streamlit app locally on your machine, follow these steps:
 
 ### Installation
 1. Install the `streamlit-bls-connection` package and its dependencies by running the following command in your terminal or command prompt:
 
 ```bash
-pip install streamlit-bls-connection
+pip install streamlit_bls_connection
 ```
 
 ### Create .py file
 2. Create a new Python script  with your favorite text editor (e.g., VSCode, Spyder, Notepad++), name it `app.py` and copy/paste below code and save changes.
 ```python
 import streamlit as st
 from streamlit_bls_connection import BLSConnection
 
 # Step 1: Setup connection to US Bureau of Labor Statistics
-connection = BLSConnection("bls_connection")
+conn = st.experimental_connection('bls', type=BLSConnection)
 
-# Step 2: Define Input parameters for the API call
+# Step 2: Define input parameters
 # Tip: one or multiple Series ID's* can be retrieved
+# find Series ID's on www.bls.gov > DATA TOOLS
 seriesids_list = ['APU000074714', 'APU000072610']
-start_year_str = '2014'  # start of date range
-end_year_str = '2023'    # end of date range
+start_year_str = '2014' # start of date range
+end_year_str = '2023'   # end of date range
 
 # Step 3: Fetch data using the custom connection
-dataframes_dict = connection.query(seriesids_list, start_year_str, end_year_str)
+dataframes_dict = connection.query(seriesids_list,
+                                   start_year_str, 
+                                   end_year_str,
+                                   api_key = None)
 
 # Step 4: Create dataframes
 gas_df = dataframes_dict['APU000074714']
 electricity_df = dataframes_dict['APU000072610']
 
 # Step 5: Show Dataframes in Streamlit
 st.dataframe(gas_df)
```

### Comparing `streamlit_bls_connection-0.7/setup.py` & `streamlit_bls_connection-0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='streamlit_bls_connection',
-    version='0.7',
+    version='0.8',
     license='MIT',  
     description='A package to fetch Bureau of Labor Statistics data using Streamlit',
     long_description=long_description,  
     long_description_content_type='text/markdown',
     author='Tony Hollaar',
     author_email='thollaar@gmail.com',
     url='https://github.com/tonyhollaar/',
-    download_url='https://github.com/tonyhollaar/streamlit_bls_connection/archive/refs/tags/v4.tar.gz',
+    download_url='https://github.com/tonyhollaar/streamlit_bls_connection/archive/refs/tags/v0.8.tar.gz',
     packages=find_packages(),
     keywords=['streamlit', 'api', 'bls'],  # <-- Comma added here
     install_requires=[
         'streamlit',
         'requests',
         'pandas',
     ],
```

### Comparing `streamlit_bls_connection-0.7/streamlit_bls_connection.egg-info/PKG-INFO` & `streamlit_bls_connection-0.8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: streamlit-bls-connection
-Version: 0.7
+Name: streamlit_bls_connection
+Version: 0.8
 Summary: A package to fetch Bureau of Labor Statistics data using Streamlit
 Home-page: https://github.com/tonyhollaar/
-Download-URL: https://github.com/tonyhollaar/streamlit_bls_connection/archive/refs/tags/v4.tar.gz
+Download-URL: https://github.com/tonyhollaar/streamlit_bls_connection/archive/refs/tags/v0.8.tar.gz
 Author: Tony Hollaar
 Author-email: thollaar@gmail.com
 License: MIT
 Keywords: streamlit,api,bls
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
@@ -33,34 +33,38 @@
 ## How to use `streamlit-bls-connection`
 To run the Streamlit app locally on your machine, follow these steps:
 
 ### Installation
 1. Install the `streamlit-bls-connection` package and its dependencies by running the following command in your terminal or command prompt:
 
 ```bash
-pip install streamlit-bls-connection
+pip install streamlit_bls_connection
 ```
 
 ### Create .py file
 2. Create a new Python script  with your favorite text editor (e.g., VSCode, Spyder, Notepad++), name it `app.py` and copy/paste below code and save changes.
 ```python
 import streamlit as st
 from streamlit_bls_connection import BLSConnection
 
 # Step 1: Setup connection to US Bureau of Labor Statistics
-connection = BLSConnection("bls_connection")
+conn = st.experimental_connection('bls', type=BLSConnection)
 
-# Step 2: Define Input parameters for the API call
+# Step 2: Define input parameters
 # Tip: one or multiple Series ID's* can be retrieved
+# find Series ID's on www.bls.gov > DATA TOOLS
 seriesids_list = ['APU000074714', 'APU000072610']
-start_year_str = '2014'  # start of date range
-end_year_str = '2023'    # end of date range
+start_year_str = '2014' # start of date range
+end_year_str = '2023'   # end of date range
 
 # Step 3: Fetch data using the custom connection
-dataframes_dict = connection.query(seriesids_list, start_year_str, end_year_str)
+dataframes_dict = connection.query(seriesids_list,
+                                   start_year_str, 
+                                   end_year_str,
+                                   api_key = None)
 
 # Step 4: Create dataframes
 gas_df = dataframes_dict['APU000074714']
 electricity_df = dataframes_dict['APU000072610']
 
 # Step 5: Show Dataframes in Streamlit
 st.dataframe(gas_df)
```

