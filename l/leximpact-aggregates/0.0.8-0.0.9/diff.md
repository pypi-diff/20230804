# Comparing `tmp/leximpact-aggregates-0.0.8.tar.gz` & `tmp/leximpact-aggregates-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "leximpact-aggregates-0.0.8.tar", max compression
+gzip compressed data, was "leximpact-aggregates-0.0.9.tar", max compression
```

## Comparing `leximpact-aggregates-0.0.8.tar` & `leximpact-aggregates-0.0.9.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       22 2022-05-20 12:47:26.516438 leximpact-aggregates-0.0.8/leximpact_aggregates/__init__.py
--rw-r--r--   0        0        0     2162 2022-05-20 10:28:30.482574 leximpact-aggregates-0.0.8/leximpact_aggregates/_nbdev.py
--rw-r--r--   0        0        0    20461 2022-05-20 12:47:26.516438 leximpact-aggregates-0.0.8/leximpact_aggregates/aggregate.py
--rw-r--r--   0        0        0     6283 2022-05-20 10:28:30.482574 leximpact-aggregates-0.0.8/leximpact_aggregates/aggregates_pote.py
--rw-r--r--   0        0        0     1611 2022-05-10 12:34:57.618232 leximpact-aggregates-0.0.8/leximpact_aggregates/pyramide_ages.py
--rw-r--r--   0        0        0      728 2022-05-20 12:47:26.520438 leximpact-aggregates-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      844 2022-05-20 14:04:40.345375 leximpact-aggregates-0.0.8/setup.py
--rw-r--r--   0        0        0      805 2022-05-20 14:04:40.345581 leximpact-aggregates-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0       22 2022-05-31 16:27:47.225532 leximpact-aggregates-0.0.9/leximpact_aggregates/__init__.py
+-rw-r--r--   0        0        0     2185 2022-05-31 16:27:47.225532 leximpact-aggregates-0.0.9/leximpact_aggregates/_nbdev.py
+-rw-r--r--   0        0        0    20461 2022-05-31 16:27:47.225532 leximpact-aggregates-0.0.9/leximpact_aggregates/aggregate.py
+-rw-r--r--   0        0        0     6399 2022-05-31 16:27:47.225532 leximpact-aggregates-0.0.9/leximpact_aggregates/aggregates_pote.py
+-rw-r--r--   0        0        0     1611 2022-05-31 16:27:47.225532 leximpact-aggregates-0.0.9/leximpact_aggregates/pyramide_ages.py
+-rw-r--r--   0        0        0      728 2022-05-31 16:27:47.225532 leximpact-aggregates-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      844 2022-05-31 16:28:12.292216 leximpact-aggregates-0.0.9/setup.py
+-rw-r--r--   0        0        0      805 2022-05-31 16:28:12.292417 leximpact-aggregates-0.0.9/PKG-INFO
```

### Comparing `leximpact-aggregates-0.0.8/leximpact_aggregates/_nbdev.py` & `leximpact-aggregates-0.0.9/leximpact_aggregates/_nbdev.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,16 +14,16 @@
     "Reference": "aggregate.ipynb",
     "Data": "aggregate.ipynb",
     "LabelKey": "aggregate.ipynb",
     "Aggregate": "aggregate.ipynb",
     "AggregateManager": "aggregate.ipynb",
     "config": "pyramide_ages.ipynb",
     "extraction_date": "aggregates_from_pote.ipynb",
-    "pote_extractions_folder": "aggregates_from_pote.ipynb",
-    "pote_quantiles": "aggregates_from_pote.ipynb",
+    "csv_pote_extractions_folder": "aggregates_from_pote.ipynb",
+    "calib_copulas_and_quantile_folder": "aggregates_from_pote.ipynb",
     "of_vars": "aggregates_from_pote.ipynb",
     "df_dgfip": "aggregates_from_pote.ipynb",
     "pote_var_to_dict": "aggregates_from_pote.ipynb",
     "metadata": "aggregates_from_pote.ipynb",
     "ref_pote_2018": "aggregates_from_pote.ipynb",
     "ref_pote_2019": "aggregates_from_pote.ipynb",
     "labels": "aggregates_from_pote.ipynb",
```

### Comparing `leximpact-aggregates-0.0.8/leximpact_aggregates/aggregate.py` & `leximpact-aggregates-0.0.9/leximpact_aggregates/aggregate.py`

 * *Files identical despite different names*

### Comparing `leximpact-aggregates-0.0.8/leximpact_aggregates/aggregates_pote.py` & `leximpact-aggregates-0.0.9/leximpact_aggregates/aggregates_pote.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: notebooks/aggregates_from_pote.ipynb (unless otherwise specified).
 
 __all__ = [
     "config",
     "tc",
     "extraction_date",
-    "pote_extractions_folder",
-    "pote_quantiles",
+    "csv_pote_extractions_folder",
+    "calib_copulas_and_quantile_folder",
     "of_vars",
     "df_dgfip",
     "pote_var_to_dict",
     "metadata",
     "ref_pote_2018",
     "ref_pote_2019",
     "labels",
@@ -54,16 +54,17 @@
 
 
 # yaml = YAML()  # typ='unsafe' for testing
 
 extraction_date = time.strftime("%Y-%m-%d")
 
 # Cell
-pote_extractions_folder = config.get("DATASETS") + "20220427-ExtractionAll/data/"
-pote_quantiles = config.get("DATASETS") + "20220519-ExtractQuantiles/data/"
+csv_pote_extractions_folder = config.get("DATASETS") + "20220427-ExtractionAll/data/"
+calib_copulas_and_quantile_folder = "/mnt/data-out/leximpact/casd-anonimyzed/"
+# pote_quantiles = config.get("DATASETS") + "20220530-ExtractQuantiles/data/"
 
 # Cell
 of_vars = openfisca_variables
 
 # Cell
 
 df_dgfip = pd.read_excel("Colonnes_POTE_2019.xlsx", skiprows=1)
@@ -166,18 +167,18 @@
 pd.set_option("display.max_colwidth", 80)
 pd.options.display.float_format = "{:,.7f}".format
 
 liste_des_variables_csg_2018 = pd.read_csv(
     config.get("DATASETS") + "agregats_des_variables_csg-POTE_2018.csv"
 )
 liste_des_variables_csg_2019 = pd.read_csv(
-    pote_extractions_folder + "/agregats_POTE_2019.csv"
+    csv_pote_extractions_folder + "/agregats_POTE_2019.csv"
 )
 liste_des_variables_revenus_2019 = pd.read_csv(
-    pote_extractions_folder + "/agregats_POTE_revenus_rici_2019.csv"
+    csv_pote_extractions_folder + "/agregats_POTE_revenus_rici_2019.csv"
 )
 
 pote = {
     "2019": [liste_des_variables_csg_2019, liste_des_variables_revenus_2019],
     "2018": [liste_des_variables_csg_2018],
 }
```

### Comparing `leximpact-aggregates-0.0.8/leximpact_aggregates/pyramide_ages.py` & `leximpact-aggregates-0.0.9/leximpact_aggregates/pyramide_ages.py`

 * *Files identical despite different names*

### Comparing `leximpact-aggregates-0.0.8/pyproject.toml` & `leximpact-aggregates-0.0.9/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "leximpact-aggregates"
-version = "0.0.8"
+version = "0.0.9"
 description = "Store aggregates of french data."
 authors = ["LexImpact"]
 license = "AGPL-3.0"
 #packages = [
 #    { include = "leximpact_aggregates" },
 #    { include = "aggregates/**/*.yaml" },
 #]
```

### Comparing `leximpact-aggregates-0.0.8/setup.py` & `leximpact-aggregates-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
  'nbdev>=1.2.2,<2.0.0',
  'openpyxl>=3.0.9,<4.0.0',
  'pre-commit>=2.17.0,<3.0.0',
  'pydantic>=1.9.0,<2.0.0']
 
 setup_kwargs = {
     'name': 'leximpact-aggregates',
-    'version': '0.0.8',
+    'version': '0.0.9',
     'description': 'Store aggregates of french data.',
     'long_description': None,
     'author': 'LexImpact',
     'author_email': None,
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `leximpact-aggregates-0.0.8/PKG-INFO` & `leximpact-aggregates-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: leximpact-aggregates
-Version: 0.0.8
+Version: 0.0.9
 Summary: Store aggregates of french data.
 License: AGPL-3.0
 Author: LexImpact
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```
