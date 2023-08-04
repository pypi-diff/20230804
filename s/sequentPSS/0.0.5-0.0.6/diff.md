# Comparing `tmp/sequentPSS-0.0.5.tar.gz` & `tmp/sequentPSS-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sequentPSS-0.0.5.tar", last modified: Fri Aug  4 21:29:55 2023, max compression
+gzip compressed data, was "sequentPSS-0.0.6.tar", last modified: Fri Aug  4 21:48:17 2023, max compression
```

## Comparing `sequentPSS-0.0.5.tar` & `sequentPSS-0.0.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-08-04 21:29:55.921934 sequentPSS-0.0.5/
--rw-rw-rw-   0        0        0      159 2023-08-03 20:55:03.000000 sequentPSS-0.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0      274 2023-08-04 21:29:55.920937 sequentPSS-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0       93 2023-08-03 03:13:22.000000 sequentPSS-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-08-04 21:29:55.860440 sequentPSS-0.0.5/sequentPSS/
--rw-rw-rw-   0        0        0       27 2023-08-03 22:30:45.000000 sequentPSS-0.0.5/sequentPSS/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-04 21:29:55.914298 sequentPSS-0.0.5/sequentPSS/sampleData/
--rw-rw-rw-   0        0        0     1040 2023-08-02 16:41:16.000000 sequentPSS-0.0.5/sequentPSS/sampleData/O1.txt
--rw-rw-rw-   0        0        0     1040 2023-08-02 16:43:05.000000 sequentPSS-0.0.5/sequentPSS/sampleData/O2.txt
--rw-rw-rw-   0        0        0     1040 2023-08-02 16:39:01.000000 sequentPSS-0.0.5/sequentPSS/sampleData/O3.txt
--rw-rw-rw-   0        0        0   946401 2023-08-03 22:13:09.000000 sequentPSS-0.0.5/sequentPSS/sampleData/concatenated_df.csv
--rw-rw-rw-   0        0        0    10982 2023-08-04 21:26:43.000000 sequentPSS-0.0.5/sequentPSS/sequentPSS.py
-drwxrwxrwx   0        0        0        0 2023-08-04 21:29:55.899338 sequentPSS-0.0.5/sequentPSS.egg-info/
--rw-rw-rw-   0        0        0      274 2023-08-04 21:29:54.000000 sequentPSS-0.0.5/sequentPSS.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      376 2023-08-04 21:29:55.000000 sequentPSS-0.0.5/sequentPSS.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-04 21:29:54.000000 sequentPSS-0.0.5/sequentPSS.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-08-04 21:29:55.000000 sequentPSS-0.0.5/sequentPSS.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-08-04 21:29:55.000000 sequentPSS-0.0.5/sequentPSS.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-04 21:29:55.922932 sequentPSS-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1455 2023-08-04 21:29:50.000000 sequentPSS-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-04 21:48:17.707091 sequentPSS-0.0.6/
+-rw-rw-rw-   0        0        0      159 2023-08-03 20:55:03.000000 sequentPSS-0.0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0      274 2023-08-04 21:48:17.706095 sequentPSS-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0       93 2023-08-03 03:13:22.000000 sequentPSS-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-08-04 21:48:17.654234 sequentPSS-0.0.6/sequentPSS/
+-rw-rw-rw-   0        0        0       27 2023-08-03 22:30:45.000000 sequentPSS-0.0.6/sequentPSS/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-04 21:48:17.700112 sequentPSS-0.0.6/sequentPSS/sampleData/
+-rw-rw-rw-   0        0        0     1040 2023-08-02 16:41:16.000000 sequentPSS-0.0.6/sequentPSS/sampleData/O1.txt
+-rw-rw-rw-   0        0        0     1040 2023-08-02 16:43:05.000000 sequentPSS-0.0.6/sequentPSS/sampleData/O2.txt
+-rw-rw-rw-   0        0        0     1040 2023-08-02 16:39:01.000000 sequentPSS-0.0.6/sequentPSS/sampleData/O3.txt
+-rw-rw-rw-   0        0        0   946401 2023-08-04 21:37:05.000000 sequentPSS-0.0.6/sequentPSS/sampleData/concatenated_df.csv
+-rw-rw-rw-   0        0        0    10985 2023-08-04 21:45:53.000000 sequentPSS-0.0.6/sequentPSS/sequentPSS.py
+drwxrwxrwx   0        0        0        0 2023-08-04 21:48:17.688143 sequentPSS-0.0.6/sequentPSS.egg-info/
+-rw-rw-rw-   0        0        0      274 2023-08-04 21:48:16.000000 sequentPSS-0.0.6/sequentPSS.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      376 2023-08-04 21:48:17.000000 sequentPSS-0.0.6/sequentPSS.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-04 21:48:16.000000 sequentPSS-0.0.6/sequentPSS.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2023-08-04 21:48:17.000000 sequentPSS-0.0.6/sequentPSS.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-08-04 21:48:17.000000 sequentPSS-0.0.6/sequentPSS.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-04 21:48:17.708091 sequentPSS-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1455 2023-08-04 21:47:43.000000 sequentPSS-0.0.6/setup.py
```

### Comparing `sequentPSS-0.0.5/sequentPSS/sampleData/O1.txt` & `sequentPSS-0.0.6/sequentPSS/sampleData/O1.txt`

 * *Files identical despite different names*

### Comparing `sequentPSS-0.0.5/sequentPSS/sampleData/O2.txt` & `sequentPSS-0.0.6/sequentPSS/sampleData/O2.txt`

 * *Files identical despite different names*

### Comparing `sequentPSS-0.0.5/sequentPSS/sampleData/O3.txt` & `sequentPSS-0.0.6/sequentPSS/sampleData/O3.txt`

 * *Files identical despite different names*

### Comparing `sequentPSS-0.0.5/sequentPSS/sampleData/concatenated_df.csv` & `sequentPSS-0.0.6/sequentPSS/sampleData/concatenated_df.csv`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-,uniq_num,p1,p2,p3,y1,y2,y3
+,uniq_num,x1,x2,x3,y1,y2,y3
 0,0,2,1,2,187,121,19
 1,0,2,1,2,31.9,27,7
 2,0,2,1,2,192.1,168,15
 3,0,2,1,2,1056.9,275,34
 4,0,2,1,2,995.9,363,15
 5,0,2,1,2,838,355,15
 6,0,2,1,2,761.6,321,24
```

### Comparing `sequentPSS-0.0.5/sequentPSS/sequentPSS.py` & `sequentPSS-0.0.6/sequentPSS/sequentPSS.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from SALib.analyze import fast
 from SALib.analyze import rbd_fast
 from SALib.analyze import delta
 
 
 # ## data
 
-# In[52]:
+# In[225]:
 
 
 # change path to relative path - only for publishing
 current_directory = os.path.dirname(os.path.abspath(__file__))
 os.chdir(current_directory)
 
 path = "./sampleData/concatenated_df.csv"
@@ -36,56 +36,56 @@
 O2 = sorted(np.loadtxt(oPath + "O2.txt"))
 O3 = sorted(np.loadtxt(oPath + "O3.txt"))
 
 
 
 # ## simulation code
 
-# In[53]:
+# In[226]:
 
 
-def simple_Simulation(p1: 'int', p2: 'int', p3: 'int', n = 10):
+def simple_Simulation(x1: 'int', x2: 'int', x3: 'int', n = 10):
     '''
     to make simple simulation
     
     Parameters
     ----------
-    p1 : parameter 1. range: 1 to 5
-    p2 : parameter 2. range: 1 to 5
-    p3 : parameter 3. range: 1 to 5
+    x1 : parameter 1. range: 1 to 5
+    x2 : parameter 2. range: 1 to 5
+    x3 : parameter 3. range: 1 to 5
     n : the number of simulation runs
 
     Returns
     -------
     DataFrame
         A comma-separated values (csv) file is returned as two-dimensional
         data structure with labeled axes.
 
     Examples
     --------
-    >>> simple_Simulation(p1 = 1, p2 = 3, p3 = 2, n = 11)
+    >>> simple_Simulation(x1 = 1, x2 = 3, x3 = 2, n = 11)
     '''
     
     global simul_data # globally declare
    
     # select data
-    condition = (simul_data['p1'] == p1) & (simul_data['p2'] == p2) & (simul_data['p3'] == p3)
+    condition = (simul_data['x1'] == x1) & (simul_data['x2'] == x2) & (simul_data['x3'] == x3)
     filtered_df = simul_data[condition]
     
     dfs = []
     for i in range(n): # now, extracts by #n
         
         uniq_num = random2.choice(pd.unique(filtered_df['uniq_num']))
         chosen_df = filtered_df[filtered_df['uniq_num'] == uniq_num] #filter only uniq_num
     
         # now make new simulation data
         new_data = {
-            'p1': [chosen_df['p1'].iloc[0]],
-            'p2': [chosen_df['p2'].iloc[0]],
-            'p3': [chosen_df['p3'].iloc[0]],
+            'x1': [chosen_df['x1'].iloc[0]],
+            'x2': [chosen_df['x2'].iloc[0]],
+            'x3': [chosen_df['x3'].iloc[0]],
             'y1': [sorted(chosen_df['y1'].tolist())],
             'y2': [sorted(chosen_df['y2'].tolist())],
             'y3': [sorted(chosen_df['y3'].tolist())]
         }
         
         chosen_df = pd.DataFrame(new_data)
 
@@ -104,66 +104,66 @@
 
     
     return result_df
 
 
 # ## 1) preprocessing (1) - Determine a criterions for calibration
 
-# In[54]:
+# In[228]:
 
 
 # run multiple simulations
 
-def multiple_simple_simulation(p1_list, p2_list, p3_list, M = 150, u = 0.1, k = 3):
+def multiple_simple_simulation(x1_list, x2_list, x3_list, M = 150, u = 0.1, k = 3):
     '''
     to make simple simulation results df by multiple parameters
     
     Parameters
     ----------
-    p1: parameter 1. range: 1 to 5
-    p2: parameter 2. range: 1 to 5
-    p3: parameter 3. range: 1 to 5
+    x1: parameter 1. range: 1 to 5
+    x2: parameter 2. range: 1 to 5
+    x3: parameter 3. range: 1 to 5
     M: MonteCarlo index (default:100, too low:low accuracy, too high:computational intensity) 
     u = leniency index (default:0.1, too low:overfit, too high:uncertainty)
     k = the number of parameters (3)
 
     Returns
     -------
     DataFrame
         A comma-separated values (csv) file is returned as two-dimensional
         data structure with labeled axes.
 
     Examples
     --------
-    >>> multi_simul_df = multiple_simple_simulation(p1_list, p2_list, p3_list, M = 150, u = 0.1, k = 3)
+    >>> multi_simul_df = multiple_simple_simulation(x1_list, x2_list, x3_list, M = 150, u = 0.1, k = 3)
     '''    
     
     global simple_Simulation
     
     # list for saving all results dfs
     prep1_dfs = []
     
     for i in range(M*(2*k + 2)): #1200 times
         # set parameter space
-        p_1 = random2.choice(p1_list)
-        p_2 = random2.choice(p2_list)
-        p_3 = random2.choice(p3_list)
+        x_1 = random2.choice(x1_list)
+        x_2 = random2.choice(x2_list)
+        x_3 = random2.choice(x3_list)
 
         # run model and save
-        tem_prep1_data = simple_Simulation(p1 = p_1, p2 = p_2, p3 = p_3, n = 1)
+        tem_prep1_data = simple_Simulation(x1 = x_1, x2 = x_2, x3 = x_3, n = 1)
 
         # append temporal result to list
         prep1_dfs.append(tem_prep1_data)
 
     result_df = pd.concat(prep1_dfs, axis=0, ignore_index=True)
 
     return result_df
 
 
-# In[55]:
+# In[229]:
 
 
 # Preprocessing (1): determining a criterion for calibration
 
 #def prep1_criterion():
 
 def prep1_criterion(O_list, multi_simul_df, u, k):
@@ -195,15 +195,15 @@
     
     # --- func for RMSE calculation ---
     def rmse(actual, predicted):
         return np.sqrt(np.mean((np.array(actual) - np.array(predicted))**2))
 
 
     # --- add combinations of y ---
-    comb_columns = [col for col in multi_simul_df_temp.columns if col.startswith('p')] # if the comlumn name starts with p
+    comb_columns = [col for col in multi_simul_df_temp.columns if col.startswith('x')] # if the comlumn name starts with x
     multi_simul_df_temp['comb'] = multi_simul_df_temp[comb_columns].apply(lambda row: list(row), axis=1)
 
     
     # --- add new columns of rmse between y columns and O_list ---
     for i, col in enumerate(multi_simul_df_temp.columns):
         if col.startswith('y'):
             col_name = 'rmse_O' + col[1:]
@@ -246,15 +246,15 @@
     return rmse_sel_df, multi_simul_df_temp
     
     
 
 
 # ## 2) preprocessing (2) - Sorting Y and X
 
-# In[206]:
+# In[230]:
 
 
 def sorting_Y(multi_simul_df_rmse_sel):
     '''
     Count the cases where 'rmse' is smaller than 'rmse_sel'. If the counts are higher, that 'y' is calibrated first.
     
     Parameters
@@ -296,15 +296,15 @@
     sorted_y_seq_df = result_df.sort_values(by='count', ascending=False)
 
     print('The order of Ys:', sorted_y_seq_df['y'].to_list())
     
     return result_df
 
 
-# In[221]:
+# In[231]:
 
 
 def sorting_X(problem: dict, multi_simul_df_rmse_sel, GSA = 'RBD-FAST'):
     
     '''
     
     Sobol: Sobol’ Sensitivity Analysis
@@ -356,8 +356,7 @@
     print('The order of Xs:', sorted_x_seq_df['Xs'].to_list())
     
     
     return si_df
 
 
 
-
```

### Comparing `sequentPSS-0.0.5/setup.py` & `sequentPSS-0.0.6/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name = 'sequentPSS',
-    version = '0.0.5',
+    version = '0.0.6',
     description = "algorithm for sequential parameter searching with GSA",
     url = 'https://github.com/MG-Choi/sequentPSS',
     author = 'MoongiChoi',
     author_email = 'u1316663@utah.edu',
     packages = find_packages(),
     package_data = {'sequentPSS': ['sampleData/concatenated_df.csv', 'sampleData/O1.txt', 'sampleData/O2.txt', 'sampleData/O3.txt']},
     include_package_data = True,
```

