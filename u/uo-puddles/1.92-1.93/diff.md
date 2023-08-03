# Comparing `tmp/uo_puddles-1.92.tar.gz` & `tmp/uo_puddles-1.93.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uo_puddles-1.92.tar", last modified: Thu Aug  3 22:00:40 2023, max compression
+gzip compressed data, was "uo_puddles-1.93.tar", last modified: Thu Aug  3 22:07:46 2023, max compression
```

## Comparing `uo_puddles-1.92.tar` & `uo_puddles-1.93.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 22:00:40.542038 uo_puddles-1.92/
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-08-03 22:00:31.000000 uo_puddles-1.92/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-08-03 22:00:40.542038 uo_puddles-1.92/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-03 22:00:31.000000 uo_puddles-1.92/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-08-03 22:00:31.000000 uo_puddles-1.92/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 22:00:40.546038 uo_puddles-1.92/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-08-03 22:00:31.000000 uo_puddles-1.92/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 22:00:40.542038 uo_puddles-1.92/uo_puddles/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-08-03 22:00:31.000000 uo_puddles-1.92/uo_puddles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19518 2023-08-03 22:00:31.000000 uo_puddles-1.92/uo_puddles/cis423.py
--rw-r--r--   0 runner    (1001) docker     (123)    26639 2023-08-03 22:00:31.000000 uo_puddles-1.92/uo_puddles/good_ai.py
--rw-r--r--   0 runner    (1001) docker     (123)    24737 2023-08-03 22:00:31.000000 uo_puddles-1.92/uo_puddles/good_ai_22.py
--rw-r--r--   0 runner    (1001) docker     (123)    10936 2023-08-03 22:00:31.000000 uo_puddles-1.92/uo_puddles/gremcat_df.py
--rw-r--r--   0 runner    (1001) docker     (123)     5676 2023-08-03 22:00:31.000000 uo_puddles-1.92/uo_puddles/gremcat_oo.py
--rw-r--r--   0 runner    (1001) docker     (123)    21533 2023-08-03 22:00:31.000000 uo_puddles-1.92/uo_puddles/mlops.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 22:00:40.542038 uo_puddles-1.92/uo_puddles.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-08-03 22:00:40.000000 uo_puddles-1.92/uo_puddles.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-08-03 22:00:40.000000 uo_puddles-1.92/uo_puddles.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 22:00:40.000000 uo_puddles-1.92/uo_puddles.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-03 22:00:40.000000 uo_puddles-1.92/uo_puddles.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 22:07:46.590498 uo_puddles-1.93/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-08-03 22:07:35.000000 uo_puddles-1.93/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-08-03 22:07:46.590498 uo_puddles-1.93/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-03 22:07:35.000000 uo_puddles-1.93/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-08-03 22:07:35.000000 uo_puddles-1.93/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 22:07:46.590498 uo_puddles-1.93/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-08-03 22:07:35.000000 uo_puddles-1.93/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 22:07:46.586498 uo_puddles-1.93/uo_puddles/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-08-03 22:07:35.000000 uo_puddles-1.93/uo_puddles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19518 2023-08-03 22:07:35.000000 uo_puddles-1.93/uo_puddles/cis423.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26639 2023-08-03 22:07:35.000000 uo_puddles-1.93/uo_puddles/good_ai.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24737 2023-08-03 22:07:35.000000 uo_puddles-1.93/uo_puddles/good_ai_22.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10936 2023-08-03 22:07:35.000000 uo_puddles-1.93/uo_puddles/gremcat_df.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5676 2023-08-03 22:07:35.000000 uo_puddles-1.93/uo_puddles/gremcat_oo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21624 2023-08-03 22:07:35.000000 uo_puddles-1.93/uo_puddles/mlops.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 22:07:46.586498 uo_puddles-1.93/uo_puddles.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-08-03 22:07:46.000000 uo_puddles-1.93/uo_puddles.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-08-03 22:07:46.000000 uo_puddles-1.93/uo_puddles.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 22:07:46.000000 uo_puddles-1.93/uo_puddles.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-03 22:07:46.000000 uo_puddles-1.93/uo_puddles.egg-info/top_level.txt
```

### Comparing `uo_puddles-1.92/LICENSE.txt` & `uo_puddles-1.93/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `uo_puddles-1.92/setup.py` & `uo_puddles-1.93/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="uo_puddles",
-    version="1.92",    #also change pypi_version variable at top of library
+    version="1.93",    #also change pypi_version variable at top of library
     author="Stephen Fickas",
     author_email="stephenfickas@gmail.com",
     description="for cis423 class",
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         "Programming Language :: Python :: 3",
```

### Comparing `uo_puddles-1.92/uo_puddles/cis423.py` & `uo_puddles-1.93/uo_puddles/cis423.py`

 * *Files identical despite different names*

### Comparing `uo_puddles-1.92/uo_puddles/good_ai.py` & `uo_puddles-1.93/uo_puddles/good_ai.py`

 * *Files identical despite different names*

### Comparing `uo_puddles-1.92/uo_puddles/good_ai_22.py` & `uo_puddles-1.93/uo_puddles/good_ai_22.py`

 * *Files identical despite different names*

### Comparing `uo_puddles-1.92/uo_puddles/gremcat_df.py` & `uo_puddles-1.93/uo_puddles/gremcat_df.py`

 * *Files identical despite different names*

### Comparing `uo_puddles-1.92/uo_puddles/gremcat_oo.py` & `uo_puddles-1.93/uo_puddles/gremcat_oo.py`

 * *Files identical despite different names*

### Comparing `uo_puddles-1.92/uo_puddles/mlops.py` & `uo_puddles-1.93/uo_puddles/mlops.py`

 * *Files 2% similar despite different names*

```diff
@@ -442,25 +442,26 @@
 
 titanic_transformer = Pipeline(steps=[
     ('gender', CustomMappingTransformer('Gender', {'Male': 0, 'Female': 1})),
     ('class', CustomMappingTransformer('Class', {'Crew': 0, 'C3': 1, 'C2': 2, 'C1': 3})),
     ('ohe', CustomOHETransformer(target_column='Joined')),
     ('age', CustomTukeyTransformer(target_column='Age', fence='outer')), #from chapter 4
     ('fare', CustomTukeyTransformer(target_column='Fare', fence='outer')), #from chapter 4
-    ('scale', CustomRobustTransformer()),  #from chapter 5
+    ('scale_age', CustomRobustTransformer('Age')),  #from chapter 5
+    ('scale_fare', CustomRobustTransformer('Fare')),  #from chapter 5
     ('imputer', KNNImputer(n_neighbors=5, weights="uniform", add_indicator=False))  #from chapter 6
     ], verbose=True)
 
 customer_transformer = Pipeline(steps=[
     ('os', CustomOHETransformer(target_column='OS')),
     ('isp', CustomOHETransformer(target_column='ISP')),
     ('level', CustomMappingTransformer('Experience Level', {'low': 0, 'medium': 1, 'high':2})),
     ('gender', CustomMappingTransformer('Gender', {'Male': 0, 'Female': 1})),
     ('time spent', CustomTukeyTransformer('Time Spent', 'inner')),  #from chapter 4
-    ('scale', CustomRobustTransformer()), #from chapter 5
+    ('scale', CustomRobustTransformer('Time Spent')), #from chapter 5
     ('imputer', KNNImputer(n_neighbors=5, weights="uniform", add_indicator=False))  #from chapter 6
     ], verbose=True)
 
 
 def dataset_setup(full_table, label_column_name, the_transformer, rs, ts=.2):
   feature_table = full_table.drop(columns=label_column_name)
   labels = full_table[label_column_name].to_list()
```

