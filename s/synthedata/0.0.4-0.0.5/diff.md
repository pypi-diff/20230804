# Comparing `tmp/synthedata-0.0.4.tar.gz` & `tmp/synthedata-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/synthedata-0.0.4.tar", last modified: Mon Jul 31 15:49:56 2023, max compression
+gzip compressed data, was "dist/synthedata-0.0.5.tar", last modified: Fri Aug  4 18:47:09 2023, max compression
```

## Comparing `synthedata-0.0.4.tar` & `synthedata-0.0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 annli      (501) staff       (20)        0 2023-07-31 15:49:56.036948 synthedata-0.0.4/
--rw-r--r--   0 annli      (501) staff       (20)     8768 2023-07-31 15:49:56.036666 synthedata-0.0.4/PKG-INFO
--rw-r--r--   0 annli      (501) staff       (20)     7176 2023-05-25 20:34:45.000000 synthedata-0.0.4/README.md
--rw-r--r--   0 annli      (501) staff       (20)       38 2023-07-31 15:49:56.037053 synthedata-0.0.4/setup.cfg
--rw-r--r--   0 annli      (501) staff       (20)      662 2023-07-31 15:49:47.000000 synthedata-0.0.4/setup.py
-drwxr-xr-x   0 annli      (501) staff       (20)        0 2023-07-31 15:49:56.033922 synthedata-0.0.4/synthedata/
--rw-r--r--   0 annli      (501) staff       (20)       18 2023-05-25 20:33:58.000000 synthedata-0.0.4/synthedata/__init__.py
--rw-r--r--   0 annli      (501) staff       (20)    32184 2023-07-31 15:43:32.000000 synthedata-0.0.4/synthedata/data_creator.py
-drwxr-xr-x   0 annli      (501) staff       (20)        0 2023-07-31 15:49:56.035673 synthedata-0.0.4/synthedata.egg-info/
--rw-r--r--   0 annli      (501) staff       (20)     8768 2023-07-31 15:49:55.000000 synthedata-0.0.4/synthedata.egg-info/PKG-INFO
--rw-r--r--   0 annli      (501) staff       (20)      204 2023-07-31 15:49:56.000000 synthedata-0.0.4/synthedata.egg-info/SOURCES.txt
--rw-r--r--   0 annli      (501) staff       (20)        1 2023-07-31 15:49:55.000000 synthedata-0.0.4/synthedata.egg-info/dependency_links.txt
--rw-r--r--   0 annli      (501) staff       (20)       11 2023-07-31 15:49:55.000000 synthedata-0.0.4/synthedata.egg-info/top_level.txt
+drwxr-xr-x   0 annli      (501) staff       (20)        0 2023-08-04 18:47:09.357787 synthedata-0.0.5/
+-rw-r--r--   0 annli      (501) staff       (20)     8768 2023-08-04 18:47:09.357342 synthedata-0.0.5/PKG-INFO
+-rw-r--r--   0 annli      (501) staff       (20)     7176 2023-05-25 20:34:45.000000 synthedata-0.0.5/README.md
+-rw-r--r--   0 annli      (501) staff       (20)       38 2023-08-04 18:47:09.358004 synthedata-0.0.5/setup.cfg
+-rw-r--r--   0 annli      (501) staff       (20)      662 2023-08-04 18:38:38.000000 synthedata-0.0.5/setup.py
+drwxr-xr-x   0 annli      (501) staff       (20)        0 2023-08-04 18:47:09.351648 synthedata-0.0.5/synthedata/
+-rw-r--r--   0 annli      (501) staff       (20)       18 2023-05-25 20:33:58.000000 synthedata-0.0.5/synthedata/__init__.py
+-rw-r--r--   0 annli      (501) staff       (20)    33531 2023-08-04 18:36:02.000000 synthedata-0.0.5/synthedata/data_creator.py
+drwxr-xr-x   0 annli      (501) staff       (20)        0 2023-08-04 18:47:09.355675 synthedata-0.0.5/synthedata.egg-info/
+-rw-r--r--   0 annli      (501) staff       (20)     8768 2023-08-04 18:47:09.000000 synthedata-0.0.5/synthedata.egg-info/PKG-INFO
+-rw-r--r--   0 annli      (501) staff       (20)      204 2023-08-04 18:47:09.000000 synthedata-0.0.5/synthedata.egg-info/SOURCES.txt
+-rw-r--r--   0 annli      (501) staff       (20)        1 2023-08-04 18:47:09.000000 synthedata-0.0.5/synthedata.egg-info/dependency_links.txt
+-rw-r--r--   0 annli      (501) staff       (20)       11 2023-08-04 18:47:09.000000 synthedata-0.0.5/synthedata.egg-info/top_level.txt
```

### Comparing `synthedata-0.0.4/PKG-INFO` & `synthedata-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synthedata
-Version: 0.0.4
+Version: 0.0.5
 Summary: A synthetic data creator package
 Home-page: https://github.com/fau-syn-data/synthetic-data.git
 Author: BACS_group1
 Author-email: fausyndata@gmail.com
 License: UNKNOWN
 Description: ﻿# Welcome to StackEdit!
```

### Comparing `synthedata-0.0.4/README.md` & `synthedata-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `synthedata-0.0.4/setup.py` & `synthedata-0.0.5/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="synthedata",
-    version="0.0.4",
+    version="0.0.5",
     author="BACS_group1",
     author_email="fausyndata@gmail.com",
     description="A synthetic data creator package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/fau-syn-data/synthetic-data.git",
     #packages=setuptools.find_packages(),
```

### Comparing `synthedata-0.0.4/synthedata/data_creator.py` & `synthedata-0.0.5/synthedata/data_creator.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,20 +115,23 @@
             temp = 'col' + str(len(self.df.columns) + i)
             i += 1
         return temp
 
     def binarize_column(self, column_name, limit):
         '''This function binarizes the column of the dataframe based on the input limit.'''
         self.df[column_name]=(self.df[column_name] < limit).astype(int)
+        return self
 
     def categorize_column(self, column_name, limits):
         '''This function replaces numerical values in a column with generic categories.
         The limits set the lower and upper boudaries for the categories. The upper limit of the first category is the lower limit of the second and so on.
         '''
+        limits = sorted(list(set(limits)))
         self.df[column_name] = pd.cut(self.df[column_name], bins= limits, labels= ["class_" + str(i + 1) for i in range(len(limits) - 1)] )
+        return self
         
     def add_var(self, var_name:str, data_generation_function:Callable, features:list or dict=None,
                 noise=True, outliers=True, nas=True):
         '''This function adds a new variable as column to the dataframe of the class instance. It requires a name for the new column and a callable function as input.
         The features are the column names that are to be interpreted locally relative to the dataframe. They can be passed as a list or as a dictionary.
         By default None values will be added for any function, noise and outliers will only be added to the new variable if it is a numerical column.'''
         with warnings.catch_warnings():
@@ -221,59 +224,82 @@
             n = size=len(self.df.index)
             if n == 0:
                 n = 10000
         if var_name is None:
             var_name = self.generate_name()
         return n, var_name
 
-    def add_nominal(self, n:int=None, var_name:str=None, topic: Literal["gender"] = "gender"):
+    def add_nominal(self, n:int=None, var_name:str=None, topic: Literal["gender", "random"] = "random"):
         '''Adds a nominal column to the dataframe. So far only a distribution for gender is implemented.
         Possible extensions include e.g., generic nominal values, race distribution.'''
         n, var_name = self.check_inputs(n, var_name)
-        if topic=="gender":
+        if topic=="random":
+            p1 = np.random.uniform(0.1, 0.6)
+            p2 = np.random.uniform(0.1, 0.9-p1)
+            p3 = 1 - p1 - p2
+            return self.add_var(var_name, lambda: np.random.choice(['category_1','category_2', 'category_3'], n, p=[p1, p2, p3]), [])
+        elif topic=="gender":
             return self.add_var(var_name, lambda: np.random.choice(['male','female', 'diverse'], n, p=[0.45, 0.45, 0.1]), [])
         else: return self
 
-    def add_ordinal(self, n:int=None, var_name:str=None, topic: Literal["grades"] = "grades"):
-        '''Adds an ordinal column to the dataframe. So far only a distribution for grades is implemented.'''        
+    def add_ordinal(self, n:int=None, var_name:str=None, topic: Literal["grades", "random"] = "random"):
+        '''Adds an ordinal column to the dataframe. So far only a distribution for grades is implemented.'''
         n, var_name = self.check_inputs(n, var_name)
-        if topic=="grades":
+        if topic=="random":
+            p1 = np.random.uniform(0.1, 0.6)
+            p2 = np.random.uniform(0.1, 0.9-p1)
+            p3 = 1 - p1 - p2
+            return self.add_var(var_name, lambda: np.random.choice(['low','medium', 'high'], n, p=[p1, p2, p3]), [])
+        elif topic=="grades":
             return self.add_var(var_name, lambda:
                                 np.clip(
                                     np.around(
                                         np.random.normal(loc=2.5, scale=1, size=n)
                                         ), 1, 6).astype(int),
                                 [])
         else: return self
 
-
-    def add_interval(self, n:int=None, var_name:str=None, topic: Literal["IQ"] = "IQ"):
-        '''Adds an interval column to the dataframe. So far only a distribution for IQ is implemented.'''        
+    def add_interval(self, n:int=None, var_name:str=None, topic: Literal["IQ", "random"] = "random"):
+        '''Adds an interval column to the dataframe. So far only a distribution for IQ is implemented.'''
         n, var_name = self.check_inputs(n, var_name)
-        if topic=="IQ":
+        if topic=="random":
+            p1 = np.random.uniform(100, 2000)
+            p2 = np.random.uniform(1, 0.3*p1)
+            return self.add_var(var_name, lambda:
+                                np.clip(
+                                    np.around(
+                                        np.random.normal(loc=p1, scale=p2, size=n)
+                                        ), 0.3*p1, 1.7*p1).astype(int),
+                                [])
+        elif topic=="IQ":
             return self.add_var(var_name, lambda:
                                 np.clip(
                                     np.around(
                                         np.random.normal(loc=100, scale=15, size=n)
                                         ), 10, 250).astype(int),
                                 [])
         else: return self
 
-    def add_ratio(self, n:int=None, var_name:str=None, topic: Literal["revenue"] = "revenue"):
-        '''Adds a ratio column to the dataframe. So far only a distribution for revenue is implemented.'''        
+    def add_ratio(self, n:int=None, var_name:str=None, topic: Literal["revenue", "random"] = "random"):
+        '''Adds a ratio column to the dataframe. So far only a distribution for revenue is implemented.'''
         n, var_name = self.check_inputs(n, var_name)
-        if topic=="revenue":
+        if topic=="random":
+            p1 = np.random.uniform(-200, 200)
+            p2 = np.random.uniform(1, 300)
+            return self.add_var(var_name, lambda: np.around(np.random.normal(loc=p1, scale=p2, size=n)).astype(int),[])
+        elif topic=="revenue":
             return self.add_var(var_name, lambda:
                                 np.clip(
                                   np.around(
                                         np.random.lognormal(np.log(1000000.00), 0.75, size=n), 2
                                         ), 0.00, 572754000000.00),
                                 [])
         else: return self
 
+
     def gen_target(self, var_name="target", dependency_rate = 0.1, mandatory_features = [], bias = []):
         '''Generates the target and biased target column for the datafame.
         The mandatory features and the features for the bias get passed as list of strings of their respective names.'''
         categorical_mapping = {}
         features_for_target = []
         biased_columns = []
         features_for_target.clear()
```

### Comparing `synthedata-0.0.4/synthedata.egg-info/PKG-INFO` & `synthedata-0.0.5/synthedata.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synthedata
-Version: 0.0.4
+Version: 0.0.5
 Summary: A synthetic data creator package
 Home-page: https://github.com/fau-syn-data/synthetic-data.git
 Author: BACS_group1
 Author-email: fausyndata@gmail.com
 License: UNKNOWN
 Description: ﻿# Welcome to StackEdit!
```

