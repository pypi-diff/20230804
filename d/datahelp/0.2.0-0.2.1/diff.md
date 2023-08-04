# Comparing `tmp/datahelp-0.2.0.tar.gz` & `tmp/datahelp-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datahelp-0.2.0.tar", last modified: Wed Jul 26 09:23:30 2023, max compression
+gzip compressed data, was "datahelp-0.2.1.tar", last modified: Fri Aug  4 09:11:07 2023, max compression
```

## Comparing `datahelp-0.2.0.tar` & `datahelp-0.2.1.tar`

### file list

```diff
@@ -1,22 +1,21 @@
-drwxr-xr-x   0 shak      (1000) shak      (1000)        0 2023-07-26 09:23:30.513308 datahelp-0.2.0/
--rw-r--r--   0 shak      (1000) shak      (1000)     1067 2023-07-19 21:51:44.000000 datahelp-0.2.0/LICENSE.txt
--rw-r--r--   0 shak      (1000) shak      (1000)     3772 2023-07-26 09:23:30.513308 datahelp-0.2.0/PKG-INFO
--rw-r--r--   0 shak      (1000) shak      (1000)     3327 2023-07-23 19:35:11.000000 datahelp-0.2.0/README.md
-drwxr-xr-x   0 shak      (1000) shak      (1000)        0 2023-07-26 09:23:30.513308 datahelp-0.2.0/datahelp/
--rw-r--r--   0 shak      (1000) shak      (1000)       22 2023-07-23 19:01:46.000000 datahelp-0.2.0/datahelp/__init__.py
--rw-r--r--   0 shak      (1000) shak      (1000)     4634 2023-07-23 15:41:42.000000 datahelp-0.2.0/datahelp/create_project.py
--rw-r--r--   0 shak      (1000) shak      (1000)    11106 2023-07-23 19:56:09.000000 datahelp-0.2.0/datahelp/eda.py
--rw-r--r--   0 shak      (1000) shak      (1000)     5003 2023-07-22 22:04:55.000000 datahelp-0.2.0/datahelp/feature_engineering.py
--rw-r--r--   0 shak      (1000) shak      (1000)     4231 2023-07-22 22:00:28.000000 datahelp-0.2.0/datahelp/modelling.py
--rw-r--r--   0 shak      (1000) shak      (1000)     7248 2023-07-23 19:55:05.000000 datahelp-0.2.0/datahelp/timeseries.py
--rw-r--r--   0 shak      (1000) shak      (1000)     1042 2023-07-22 23:17:03.000000 datahelp-0.2.0/datahelp/utils.py
--rw-r--r--   0 shak      (1000) shak      (1000)      745 2023-07-19 21:38:45.000000 datahelp-0.2.0/datahelp/visualize.py
-drwxr-xr-x   0 shak      (1000) shak      (1000)        0 2023-07-26 09:23:30.513308 datahelp-0.2.0/datahelp.egg-info/
--rw-r--r--   0 shak      (1000) shak      (1000)     3772 2023-07-26 09:23:30.000000 datahelp-0.2.0/datahelp.egg-info/PKG-INFO
--rw-r--r--   0 shak      (1000) shak      (1000)      395 2023-07-26 09:23:30.000000 datahelp-0.2.0/datahelp.egg-info/SOURCES.txt
--rw-r--r--   0 shak      (1000) shak      (1000)        1 2023-07-26 09:23:30.000000 datahelp-0.2.0/datahelp.egg-info/dependency_links.txt
--rw-r--r--   0 shak      (1000) shak      (1000)       65 2023-07-26 09:23:30.000000 datahelp-0.2.0/datahelp.egg-info/requires.txt
--rw-r--r--   0 shak      (1000) shak      (1000)        9 2023-07-26 09:23:30.000000 datahelp-0.2.0/datahelp.egg-info/top_level.txt
--rw-r--r--   0 shak      (1000) shak      (1000)      941 2023-07-26 09:20:48.000000 datahelp-0.2.0/pyproject.toml
--rw-r--r--   0 shak      (1000) shak      (1000)       79 2023-07-26 09:23:30.513308 datahelp-0.2.0/setup.cfg
--rw-r--r--   0 shak      (1000) shak      (1000)     1039 2023-07-26 09:22:49.000000 datahelp-0.2.0/setup.py
+drwxr-xr-x   0 shak      (1000) shak      (1000)        0 2023-08-04 09:11:07.892546 datahelp-0.2.1/
+-rw-r--r--   0 shak      (1000) shak      (1000)     1067 2023-07-19 21:51:44.000000 datahelp-0.2.1/LICENSE.txt
+-rw-r--r--   0 shak      (1000) shak      (1000)     3856 2023-08-04 09:11:07.892546 datahelp-0.2.1/PKG-INFO
+-rw-r--r--   0 shak      (1000) shak      (1000)     3414 2023-07-27 13:28:38.000000 datahelp-0.2.1/README.md
+drwxr-xr-x   0 shak      (1000) shak      (1000)        0 2023-08-04 09:11:07.892546 datahelp-0.2.1/datahelp/
+-rw-r--r--   0 shak      (1000) shak      (1000)       22 2023-07-27 06:19:05.000000 datahelp-0.2.1/datahelp/__init__.py
+-rw-r--r--   0 shak      (1000) shak      (1000)     4634 2023-07-27 06:19:05.000000 datahelp-0.2.1/datahelp/create_project.py
+-rw-r--r--   0 shak      (1000) shak      (1000)    10988 2023-07-27 13:13:11.000000 datahelp-0.2.1/datahelp/eda.py
+-rw-r--r--   0 shak      (1000) shak      (1000)     5003 2023-07-27 06:19:05.000000 datahelp-0.2.1/datahelp/feature_engineering.py
+-rw-r--r--   0 shak      (1000) shak      (1000)     4231 2023-08-04 09:06:08.000000 datahelp-0.2.1/datahelp/modelling.py
+-rw-r--r--   0 shak      (1000) shak      (1000)     7241 2023-07-27 06:19:05.000000 datahelp-0.2.1/datahelp/timeseries.py
+-rw-r--r--   0 shak      (1000) shak      (1000)     1042 2023-07-27 06:19:05.000000 datahelp-0.2.1/datahelp/utils.py
+-rw-r--r--   0 shak      (1000) shak      (1000)      745 2023-07-27 06:19:05.000000 datahelp-0.2.1/datahelp/visualize.py
+drwxr-xr-x   0 shak      (1000) shak      (1000)        0 2023-08-04 09:11:07.892546 datahelp-0.2.1/datahelp.egg-info/
+-rw-r--r--   0 shak      (1000) shak      (1000)     3856 2023-08-04 09:11:07.000000 datahelp-0.2.1/datahelp.egg-info/PKG-INFO
+-rw-r--r--   0 shak      (1000) shak      (1000)      380 2023-08-04 09:11:07.000000 datahelp-0.2.1/datahelp.egg-info/SOURCES.txt
+-rw-r--r--   0 shak      (1000) shak      (1000)        1 2023-08-04 09:11:07.000000 datahelp-0.2.1/datahelp.egg-info/dependency_links.txt
+-rw-r--r--   0 shak      (1000) shak      (1000)       65 2023-08-04 09:11:07.000000 datahelp-0.2.1/datahelp.egg-info/requires.txt
+-rw-r--r--   0 shak      (1000) shak      (1000)        9 2023-08-04 09:11:07.000000 datahelp-0.2.1/datahelp.egg-info/top_level.txt
+-rw-r--r--   0 shak      (1000) shak      (1000)       79 2023-08-04 09:11:07.892546 datahelp-0.2.1/setup.cfg
+-rw-r--r--   0 shak      (1000) shak      (1000)     1039 2023-08-04 09:11:00.000000 datahelp-0.2.1/setup.py
```

### Comparing `datahelp-0.2.0/LICENSE.txt` & `datahelp-0.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `datahelp-0.2.0/PKG-INFO` & `datahelp-0.2.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datahelp
-Version: 0.2.0
+Version: 0.2.1
 Summary: Data science library for data science / data analysis teams
 Home-page: https://github.com/datahelp
 Author: Meshack Kitonga
 Author-email: dev.kitonga@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
@@ -22,23 +22,23 @@
 
 datahelp offers the following key features:
 
 1. **Project Management:** datahelp simplifies the creation of standard data science project structures. With a single function call, you can generate a well-organized project directory with predefined folders for datasets, processed data, raw data, outputs, models, scripts, notebooks, and more.
 
 2. **Model Saving and Loading:** datahelp provides easy-to-use functions for saving and loading trained machine learning models. It supports various formats such as joblib, pickle, and keras, enabling seamless integration with different model types.
 
-3. **Data Exploration and Visualization:** The library includes functions for data exploration, summary statistics, and visualization. You can quickly generate feature importances plots and visualize missing data to gain insights into your datasets.
+3. **Data Exploration and Visualization:** The library includes functions for data exploration, summary statistics, and visualization. You can quickly generate feature vi plots and visualize missing data to gain insights into your datasets.
 
 4. **Feature Engineering:** datahelp includes methods for handling missing data and noise in your datasets. It offers functions for dropping missing columns based on a specified threshold and detecting outliers using Tukey's Interquartile Range (IQR) method.
 
 5. **Model Evaluation and Cross-Validation:** datahelp provides tools to evaluate model performance, including functions to calculate accuracy, F1-score, precision, recall, and generate classification reports. It also supports cross-validation for model evaluation.
 
 6. **Scaling and Normalization:** The library offers functions for min-max scaling and z-score normalization of data to bring features to a common scale.
 
-## Getting Started
+## Quickstart
 
 To use datahelp in your data science projects, you can install it via pip:
 
 ```bash
 pip install datahelp
 ```
 
@@ -59,14 +59,17 @@
 
 cat_count = dh.eda.get_cat_counts(df)
 cat_count
 
 missing = dh.eda.display_missing(df)
 missing
 ```
+## Lins
+Project: https://github.com/kimxons/datahelp
+PyPi: https://pypi.python.org/pypi/dataehlp/
 
 ## Documentation
 
 For detailed usage instructions and API reference, please refer to the official documentation at [https://datahelp-docs.example.com](https://datahelp-docs.example.com)
 
 ## Contribution
```

### Comparing `datahelp-0.2.0/README.md` & `datahelp-0.2.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 
 datahelp offers the following key features:
 
 1. **Project Management:** datahelp simplifies the creation of standard data science project structures. With a single function call, you can generate a well-organized project directory with predefined folders for datasets, processed data, raw data, outputs, models, scripts, notebooks, and more.
 
 2. **Model Saving and Loading:** datahelp provides easy-to-use functions for saving and loading trained machine learning models. It supports various formats such as joblib, pickle, and keras, enabling seamless integration with different model types.
 
-3. **Data Exploration and Visualization:** The library includes functions for data exploration, summary statistics, and visualization. You can quickly generate feature importances plots and visualize missing data to gain insights into your datasets.
+3. **Data Exploration and Visualization:** The library includes functions for data exploration, summary statistics, and visualization. You can quickly generate feature vi plots and visualize missing data to gain insights into your datasets.
 
 4. **Feature Engineering:** datahelp includes methods for handling missing data and noise in your datasets. It offers functions for dropping missing columns based on a specified threshold and detecting outliers using Tukey's Interquartile Range (IQR) method.
 
 5. **Model Evaluation and Cross-Validation:** datahelp provides tools to evaluate model performance, including functions to calculate accuracy, F1-score, precision, recall, and generate classification reports. It also supports cross-validation for model evaluation.
 
 6. **Scaling and Normalization:** The library offers functions for min-max scaling and z-score normalization of data to bring features to a common scale.
 
-## Getting Started
+## Quickstart
 
 To use datahelp in your data science projects, you can install it via pip:
 
 ```bash
 pip install datahelp
 ```
 
@@ -43,14 +43,17 @@
 
 cat_count = dh.eda.get_cat_counts(df)
 cat_count
 
 missing = dh.eda.display_missing(df)
 missing
 ```
+## Lins
+Project: https://github.com/kimxons/datahelp
+PyPi: https://pypi.python.org/pypi/dataehlp/
 
 ## Documentation
 
 For detailed usage instructions and API reference, please refer to the official documentation at [https://datahelp-docs.example.com](https://datahelp-docs.example.com)
 
 ## Contribution
```

### Comparing `datahelp-0.2.0/datahelp/create_project.py` & `datahelp-0.2.1/datahelp/create_project.py`

 * *Files identical despite different names*

### Comparing `datahelp-0.2.0/datahelp/eda.py` & `datahelp-0.2.1/datahelp/eda.py`

 * *Files 6% similar despite different names*

```diff
@@ -76,41 +76,41 @@
         raise TypeError("df must be a pandas DataFrame or Series")
 
     cat_vars = get_cat_vars(df)
     counts = {var: df[var].value_counts().shape[0] for var in cat_vars}
     return pd.DataFrame({"Feature": list(counts.keys()), "Unique Count": list(counts.values())})
 
 
-def plot_feature_importance(importances: np.ndarray, feature_names: list) -> None:
+def plot_feature_importance(vi: np.ndarray, feature_names: list) -> None:
     """
     Plots the feature importance as a bar chart.
 
     Parameters:
     -----------
-    importances : numpy ndarray
-        The feature importances from a trained model.
+    vi : numpy ndarray
+        The feature vi from a trained model.
     feature_names : list of str
-        The names of the features in the same order as the importances.
+        The names of the features in the same order as the vi.
 
     Returns:
     --------
     None
     """
-    if not isinstance(importances, np.ndarray) or not isinstance(feature_names, list):
-        raise TypeError("importances should be a numpy ndarray and feature_names should be a list.")
+    if not isinstance(vi, np.ndarray) or not isinstance(feature_names, list):
+        raise TypeError("vi should be a numpy ndarray and feature_names should be a list.")
 
-    if len(importances) != len(feature_names):
-        raise ValueError("importances and feature_names should have the same length.")
+    if len(vi) != len(feature_names):
+        raise ValueError("vi and feature_names should have the same length.")
 
-    sorted_indices = importances.argsort()[::-1]
-    plt.bar(range(len(importances)), importances[sorted_indices])
-    plt.xticks(range(len(importances)), np.array(feature_names)[sorted_indices], rotation=90)
+    sorted_indices = vi.argsort()[::-1]
+    plt.bar(range(len(vi)), vi[sorted_indices])
+    plt.xticks(range(len(vi)), np.array(feature_names)[sorted_indices], rotation=90)
     plt.xlabel("Feature")
     plt.ylabel("Importance")
-    plt.title("Feature Importances")
+    plt.title("Feature vi")
     plt.show()
 
 
 def feature_summary(df: Union[pd.DataFrame, pd.Series], visualize: bool = False) -> None:
     """
     Provides a summary of the features in a pandas DataFrame.
 
@@ -327,15 +327,15 @@
     if index:
         if train_data[index].nunique() == train_data.shape[0]:
             print('Id field is unique.')
         else:
             print('Id field is not unique')
 
         if len(np.intersect1d(train_data[index].values, test_data[index].values)) == 0:
-            print('Train and test sets have distinct Ids.') 
+            print('Train and test sets have distinct Ids.')
         else:
             print('Train and test sets IDs are the same.')
 
         print('\n')
         plt.plot(train_data.groupby(col).count()[[index]], 'o-', label='train')
         plt.plot(test_data.groupby(col).count()[[index]], 'o-', label='test')
         plt.title('Train and test instances overlap.')
```

### Comparing `datahelp-0.2.0/datahelp/feature_engineering.py` & `datahelp-0.2.1/datahelp/feature_engineering.py`

 * *Files identical despite different names*

### Comparing `datahelp-0.2.0/datahelp/modelling.py` & `datahelp-0.2.1/datahelp/modelling.py`

 * *Files identical despite different names*

### Comparing `datahelp-0.2.0/datahelp/timeseries.py` & `datahelp-0.2.1/datahelp/timeseries.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,16 +38,16 @@
     """
     # Function implementation remains unchanged
     pass
 
 
 def extract_time_info(data=None, time_cols=None, subset=None, drop=True):
     """
-    Returns time information in a pandas DataFrame as a new set of columns 
-    added to the original data frame. For extracting DateTime features, 
+    Returns time information in a pandas DataFrame as a new set of columns
+    added to the original data frame. For extracting DateTime features,
     use extract_date_info function.
 
     Parameters:
     -----------
     data: DataFrame or named Series
         The data set to extract time information from.
 
@@ -66,15 +66,15 @@
     """
     # Function implementation remains unchanged
     pass
 
 
 def get_time_elapsed(data=None, date_cols=None, by='s', col_name=None):
     """
-    Calculates the time elapsed between two specified date columns 
+    Calculates the time elapsed between two specified date columns
     and returns the value in either seconds (s), minutes (m), or hours (h).
 
     Parameters:
     -----------
     data: DataFrame or named Series.
         The data where the Date features are located.
 
@@ -96,26 +96,26 @@
     pass
 
 
 def get_period_of_day(date_col=None):
     """
     Returns a list of the time of the day as regards to mornings, afternoons, or evenings.
     Hour of the day that falls between [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12] are mapped to mornings,
-    [13, 14, 15, 16] are mapped to afternoons, and [17, 18, 19, 20, 21, 22, 23] are mapped to evenings. 
+    [13, 14, 15, 16] are mapped to afternoons, and [17, 18, 19, 20, 21, 22, 23] are mapped to evenings.
 
     Parameters:
     ------------
     date_col: Series, 1-D DataFrame
         The datetime feature.
 
     Returns:
     ----------
     Series of mapped values.
     """
-    def _map_hours(x):   
+    def _map_hours(x):
         if x in [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12]:
             return 'morning'
         elif x in [13, 14, 15, 16]:
             return 'afternoon'
         else:
             return 'evening'
```

### Comparing `datahelp-0.2.0/datahelp/utils.py` & `datahelp-0.2.1/datahelp/utils.py`

 * *Files identical despite different names*

### Comparing `datahelp-0.2.0/datahelp/visualize.py` & `datahelp-0.2.1/datahelp/visualize.py`

 * *Files identical despite different names*

### Comparing `datahelp-0.2.0/datahelp.egg-info/PKG-INFO` & `datahelp-0.2.1/datahelp.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datahelp
-Version: 0.2.0
+Version: 0.2.1
 Summary: Data science library for data science / data analysis teams
 Home-page: https://github.com/datahelp
 Author: Meshack Kitonga
 Author-email: dev.kitonga@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
@@ -22,23 +22,23 @@
 
 datahelp offers the following key features:
 
 1. **Project Management:** datahelp simplifies the creation of standard data science project structures. With a single function call, you can generate a well-organized project directory with predefined folders for datasets, processed data, raw data, outputs, models, scripts, notebooks, and more.
 
 2. **Model Saving and Loading:** datahelp provides easy-to-use functions for saving and loading trained machine learning models. It supports various formats such as joblib, pickle, and keras, enabling seamless integration with different model types.
 
-3. **Data Exploration and Visualization:** The library includes functions for data exploration, summary statistics, and visualization. You can quickly generate feature importances plots and visualize missing data to gain insights into your datasets.
+3. **Data Exploration and Visualization:** The library includes functions for data exploration, summary statistics, and visualization. You can quickly generate feature vi plots and visualize missing data to gain insights into your datasets.
 
 4. **Feature Engineering:** datahelp includes methods for handling missing data and noise in your datasets. It offers functions for dropping missing columns based on a specified threshold and detecting outliers using Tukey's Interquartile Range (IQR) method.
 
 5. **Model Evaluation and Cross-Validation:** datahelp provides tools to evaluate model performance, including functions to calculate accuracy, F1-score, precision, recall, and generate classification reports. It also supports cross-validation for model evaluation.
 
 6. **Scaling and Normalization:** The library offers functions for min-max scaling and z-score normalization of data to bring features to a common scale.
 
-## Getting Started
+## Quickstart
 
 To use datahelp in your data science projects, you can install it via pip:
 
 ```bash
 pip install datahelp
 ```
 
@@ -59,14 +59,17 @@
 
 cat_count = dh.eda.get_cat_counts(df)
 cat_count
 
 missing = dh.eda.display_missing(df)
 missing
 ```
+## Lins
+Project: https://github.com/kimxons/datahelp
+PyPi: https://pypi.python.org/pypi/dataehlp/
 
 ## Documentation
 
 For detailed usage instructions and API reference, please refer to the official documentation at [https://datahelp-docs.example.com](https://datahelp-docs.example.com)
 
 ## Contribution
```

### Comparing `datahelp-0.2.0/setup.py` & `datahelp-0.2.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name="datahelp",
-    version="0.2.0",
+    version="0.2.1",
     license="MIT",
     description="Data science library for data science / data analysis teams",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Meshack Kitonga",
     author_email="dev.kitonga@gmail.com",
     url="https://github.com/datahelp",
```

