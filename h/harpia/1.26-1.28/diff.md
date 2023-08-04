# Comparing `tmp/harpia-1.26.tar.gz` & `tmp/harpia-1.28.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "harpia-1.26.tar", last modified: Fri Aug  4 19:47:17 2023, max compression
+gzip compressed data, was "harpia-1.28.tar", last modified: Fri Aug  4 20:08:32 2023, max compression
```

## Comparing `harpia-1.26.tar` & `harpia-1.28.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-08-04 19:47:17.391504 harpia-1.26/
--rw-rw-rw-   0        0        0     1080 2023-07-31 03:26:07.000000 harpia-1.26/LICENSE
--rw-rw-rw-   0        0        0      554 2023-08-04 19:47:17.391504 harpia-1.26/PKG-INFO
--rw-rw-rw-   0        0        0       22 2023-07-31 03:26:07.000000 harpia-1.26/README.md
-drwxrwxrwx   0        0        0        0 2023-08-04 19:47:17.310804 harpia-1.26/harpia/
--rw-rw-rw-   0        0        0     1141 2023-07-31 03:26:07.000000 harpia-1.26/harpia/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-04 19:47:17.321933 harpia-1.26/harpia/tropomi/
--rw-rw-rw-   0        0        0     1137 2023-07-31 03:26:07.000000 harpia-1.26/harpia/tropomi/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-04 19:47:17.330939 harpia-1.26/harpia/tropomi/no2/
--rw-rw-rw-   0        0        0     1242 2023-08-02 17:39:12.000000 harpia-1.26/harpia/tropomi/no2/__init__.py
--rw-rw-rw-   0        0        0     6734 2023-07-31 04:10:19.000000 harpia-1.26/harpia/tropomi/no2/converter.py
--rw-rw-rw-   0        0        0     3181 2023-08-02 02:48:42.000000 harpia-1.26/harpia/tropomi/no2/cp_completion.py
--rw-rw-rw-   0        0        0     7037 2023-08-04 19:45:07.000000 harpia-1.26/harpia/tropomi/no2/imputation.py
--rw-rw-rw-   0        0        0     5689 2023-08-04 19:37:00.000000 harpia-1.26/harpia/tropomi/no2/kriging.py
-drwxrwxrwx   0        0        0        0 2023-08-04 19:47:17.310804 harpia-1.26/harpia/tropomi/no2/lib/
-drwxrwxrwx   0        0        0        0 2023-08-04 19:47:17.361228 harpia-1.26/harpia/tropomi/no2/lib/random_missing_indices/
--rw-rw-rw-   0        0        0 33554168 2023-07-29 01:01:49.000000 harpia-1.26/harpia/tropomi/no2/lib/random_missing_indices/random_indices_20190101_20200101_025_0.5_0.1.npy
--rw-rw-rw-   0        0        0  8366192 2023-07-29 17:57:48.000000 harpia-1.26/harpia/tropomi/no2/lib/random_missing_indices/random_indices_20190101_20200101_050_0.5_0.1.npy
-drwxrwxrwx   0        0        0        0 2023-08-04 19:47:17.391504 harpia-1.26/harpia/tropomi/no2/lib/raster_templates/
--rw-rw-rw-   0        0        0  7844566 2023-07-31 03:26:07.000000 harpia-1.26/harpia/tropomi/no2/lib/raster_templates/raster_template_130w60w20n55n_005.tif
--rw-rw-rw-   0        0        0  1970880 2023-07-31 03:26:07.000000 harpia-1.26/harpia/tropomi/no2/lib/raster_templates/raster_template_130w60w20n55n_010.tif
--rw-rw-rw-   0        0        0   317616 2023-07-31 03:26:07.000000 harpia-1.26/harpia/tropomi/no2/lib/raster_templates/raster_template_130w60w20n55n_025.tif
--rw-rw-rw-   0        0        0    78826 2023-07-31 03:26:07.000000 harpia-1.26/harpia/tropomi/no2/lib/raster_templates/raster_template_130w60w20n55n_050.tif
--rw-rw-rw-   0        0        0    19984 2023-07-31 03:26:07.000000 harpia-1.26/harpia/tropomi/no2/lib/raster_templates/raster_template_130w60w20n55n_100.tif
--rw-rw-rw-   0        0        0     5883 2023-08-01 05:28:02.000000 harpia-1.26/harpia/tropomi/no2/utils.py
-drwxrwxrwx   0        0        0        0 2023-08-04 19:47:17.321933 harpia-1.26/harpia.egg-info/
--rw-rw-rw-   0        0        0      554 2023-08-04 19:47:17.000000 harpia-1.26/harpia.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      991 2023-08-04 19:47:17.000000 harpia-1.26/harpia.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-04 19:47:17.000000 harpia-1.26/harpia.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-08-04 19:47:17.000000 harpia-1.26/harpia.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-08-04 19:47:17.000000 harpia-1.26/harpia.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-04 19:47:17.391504 harpia-1.26/setup.cfg
--rw-rw-rw-   0        0        0     2226 2023-08-04 19:45:45.000000 harpia-1.26/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-04 20:08:32.183551 harpia-1.28/
+-rw-rw-rw-   0        0        0     1080 2023-07-31 03:26:07.000000 harpia-1.28/LICENSE
+-rw-rw-rw-   0        0        0      554 2023-08-04 20:08:32.183551 harpia-1.28/PKG-INFO
+-rw-rw-rw-   0        0        0       22 2023-07-31 03:26:07.000000 harpia-1.28/README.md
+drwxrwxrwx   0        0        0        0 2023-08-04 20:08:32.072797 harpia-1.28/harpia/
+-rw-rw-rw-   0        0        0     1141 2023-07-31 03:26:07.000000 harpia-1.28/harpia/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-04 20:08:32.087418 harpia-1.28/harpia/tropomi/
+-rw-rw-rw-   0        0        0     1137 2023-07-31 03:26:07.000000 harpia-1.28/harpia/tropomi/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-04 20:08:32.103106 harpia-1.28/harpia/tropomi/no2/
+-rw-rw-rw-   0        0        0     1242 2023-08-02 17:39:12.000000 harpia-1.28/harpia/tropomi/no2/__init__.py
+-rw-rw-rw-   0        0        0     6734 2023-07-31 04:10:19.000000 harpia-1.28/harpia/tropomi/no2/converter.py
+-rw-rw-rw-   0        0        0     3181 2023-08-02 02:48:42.000000 harpia-1.28/harpia/tropomi/no2/cp_completion.py
+-rw-rw-rw-   0        0        0     7079 2023-08-04 20:07:15.000000 harpia-1.28/harpia/tropomi/no2/imputation.py
+-rw-rw-rw-   0        0        0     5605 2023-08-04 20:05:49.000000 harpia-1.28/harpia/tropomi/no2/kriging.py
+drwxrwxrwx   0        0        0        0 2023-08-04 20:08:32.062692 harpia-1.28/harpia/tropomi/no2/lib/
+drwxrwxrwx   0        0        0        0 2023-08-04 20:08:32.153391 harpia-1.28/harpia/tropomi/no2/lib/random_missing_indices/
+-rw-rw-rw-   0        0        0 33554168 2023-07-29 01:01:49.000000 harpia-1.28/harpia/tropomi/no2/lib/random_missing_indices/random_indices_20190101_20200101_025_0.5_0.1.npy
+-rw-rw-rw-   0        0        0  8366192 2023-07-29 17:57:48.000000 harpia-1.28/harpia/tropomi/no2/lib/random_missing_indices/random_indices_20190101_20200101_050_0.5_0.1.npy
+drwxrwxrwx   0        0        0        0 2023-08-04 20:08:32.183551 harpia-1.28/harpia/tropomi/no2/lib/raster_templates/
+-rw-rw-rw-   0        0        0  7844566 2023-07-31 03:26:07.000000 harpia-1.28/harpia/tropomi/no2/lib/raster_templates/raster_template_130w60w20n55n_005.tif
+-rw-rw-rw-   0        0        0  1970880 2023-07-31 03:26:07.000000 harpia-1.28/harpia/tropomi/no2/lib/raster_templates/raster_template_130w60w20n55n_010.tif
+-rw-rw-rw-   0        0        0   317616 2023-07-31 03:26:07.000000 harpia-1.28/harpia/tropomi/no2/lib/raster_templates/raster_template_130w60w20n55n_025.tif
+-rw-rw-rw-   0        0        0    78826 2023-07-31 03:26:07.000000 harpia-1.28/harpia/tropomi/no2/lib/raster_templates/raster_template_130w60w20n55n_050.tif
+-rw-rw-rw-   0        0        0    19984 2023-07-31 03:26:07.000000 harpia-1.28/harpia/tropomi/no2/lib/raster_templates/raster_template_130w60w20n55n_100.tif
+-rw-rw-rw-   0        0        0     5883 2023-08-01 05:28:02.000000 harpia-1.28/harpia/tropomi/no2/utils.py
+drwxrwxrwx   0        0        0        0 2023-08-04 20:08:32.087418 harpia-1.28/harpia.egg-info/
+-rw-rw-rw-   0        0        0      554 2023-08-04 20:08:32.000000 harpia-1.28/harpia.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      991 2023-08-04 20:08:32.000000 harpia-1.28/harpia.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-04 20:08:32.000000 harpia-1.28/harpia.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-08-04 20:08:32.000000 harpia-1.28/harpia.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-08-04 20:08:32.000000 harpia-1.28/harpia.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-04 20:08:32.183551 harpia-1.28/setup.cfg
+-rw-rw-rw-   0        0        0     2226 2023-08-04 20:08:08.000000 harpia-1.28/setup.py
```

### Comparing `harpia-1.26/LICENSE` & `harpia-1.28/LICENSE`

 * *Files identical despite different names*

### Comparing `harpia-1.26/PKG-INFO` & `harpia-1.28/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: harpia
-Version: 1.26
+Version: 1.28
 Summary: A Python Package for Development
 Home-page: https://github.com/rmsolgi/harpia.git
 Author: Ryan Solgi
 Author-email: ryan.solgi@gmail.com
 Maintainer: Ryan Solgi
 Keywords: harpia
 Classifier: Programming Language :: Python :: 3
```

### Comparing `harpia-1.26/harpia/__init__.py` & `harpia-1.28/harpia/__init__.py`

 * *Files identical despite different names*

### Comparing `harpia-1.26/harpia/tropomi/__init__.py` & `harpia-1.28/harpia/tropomi/__init__.py`

 * *Files identical despite different names*

### Comparing `harpia-1.26/harpia/tropomi/no2/__init__.py` & `harpia-1.28/harpia/tropomi/no2/__init__.py`

 * *Files identical despite different names*

### Comparing `harpia-1.26/harpia/tropomi/no2/converter.py` & `harpia-1.28/harpia/tropomi/no2/converter.py`

 * *Files identical despite different names*

### Comparing `harpia-1.26/harpia/tropomi/no2/cp_completion.py` & `harpia-1.28/harpia/tropomi/no2/cp_completion.py`

 * *Files identical despite different names*

### Comparing `harpia-1.26/harpia/tropomi/no2/imputation.py` & `harpia-1.28/harpia/tropomi/no2/imputation.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
         file_name="TC_results_"+start_date+'_'+end_date+'_'+resolution+'_'+qa_value+'_'+added_missing_ratio+'_'+str(rank)+'.pickle'
         writing_file=os.path.join(writing_directory, file_name)
         with open(writing_file, 'wb') as file:
             pickle.dump(results_dict,file)
         
     return results_dict
 
-def kriging(kriging_type,prediction_interval,raster_directory,start_date,end_date,resolution,qa_value,added_missing_ratio, writing_directory=None, partitioning=False):
+def kriging(kriging_type,prediction_interval,raster_directory,start_date,end_date,resolution,qa_value,added_missing_ratio, writing_directory=None, partitioning=False, variogram_model='linear'):
     
     random_indices_name="random_indices_"+start_date+'_'+end_date+'_'+resolution+'_'+qa_value+'_'+added_missing_ratio+'.npy'
     data, existed_dates, missed_dates=hp.utils.raster_to_array(raster_directory,start_date,end_date,resolution,qa_value)
     data=hp.utils.add_nans(data) #### nan values must be added before any change in the data values 
     data=hp.utils.molec_per_cm2(data)
     #mask=hp.utils.make_mask(data)  IT MUST NOT USE BECAUSE IT INCLUDE NAN VALUES TOO. 
     mask=np.ones(data.shape)
@@ -66,15 +66,15 @@
     
     raw_observations=cut_data[cut_random_indices]
     data_array=(data-np.nanmin(data))/(np.nanmax(data)-np.nanmin(data))
     cut_data_array=data_array[prediction_interval[0]:prediction_interval[1],:,:]
     normalized_observations=cut_data_array[cut_random_indices]
     start=time.time()
     
-    reterived_array=hp.kriging.run_kriging(cut_data_array,cut_mask,resolution, kriging_type, partitioning)
+    reterived_array=hp.kriging.run_kriging(cut_data_array,cut_mask,resolution, kriging_type,variogram_model, partitioning)
     
     end=time.time()
     
     normalized_predictions=reterived_array[cut_random_indices]
     raw_reterived_array=reterived_array*(np.nanmax(data)-np.nanmin(data))+np.nanmin(data)
     raw_predictions=raw_reterived_array[cut_random_indices]
     
@@ -90,15 +90,15 @@
         writing_file=os.path.join(writing_directory, file_name)
         with open(writing_file, 'wb') as file:
             pickle.dump(results_dict,file)
             
     return results_dict
 
 
-def custum_kriging(k_rows,k_cols,prediction_interval,raster_directory,start_date,end_date,resolution,qa_value,added_missing_ratio, writing_directory=None, kriging_type='ordinary', variogram_model='linear'):
+def custom_kriging(k_rows,k_cols,prediction_interval,raster_directory,start_date,end_date,resolution,qa_value,added_missing_ratio, writing_directory=None, kriging_type='ordinary', variogram_model='linear'):
     
     random_indices_name="random_indices_"+start_date+'_'+end_date+'_'+resolution+'_'+qa_value+'_'+added_missing_ratio+'.npy'
     data, existed_dates, missed_dates=hp.utils.raster_to_array(raster_directory,start_date,end_date,resolution,qa_value)
     data=hp.utils.add_nans(data) #### nan values must be added before any change in the data values 
     data=hp.utils.molec_per_cm2(data)
     #mask=hp.utils.make_mask(data)  IT MUST NOT USE BECAUSE IT INCLUDE NAN VALUES TOO. 
     mask=np.ones(data.shape)
```

### Comparing `harpia-1.26/harpia/tropomi/no2/kriging.py` & `harpia-1.28/harpia/tropomi/no2/kriging.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     
     
     return mask
 ##############################################################################
 ##############################################################################
 ##############################################################################
 
-def kriging_helper(array,mask,kriging_type='ordinary', variogram_model='linear'):
+def kriging_helper(array,mask,kriging_type, variogram_model):
     
     
     one_indices=np.where(mask==1)
     y_array=one_indices[0]
     x_array=one_indices[1]
     
     
@@ -64,15 +64,15 @@
    
     return z
 
 ##############################################################################
 ##############################################################################
 ##############################################################################
   
-def main_kriging(data, predict_indices,kriging_type='ordinary', variogram_model='linear'): #data must have negative and nan values as they are
+def main_kriging(data, predict_indices,kriging_type, variogram_model): #data must have negative and nan values as they are
     
     
     mask=kriging.make_mask(data,predict_indices)
     
     #data_array=(data-np.nanmin(data))/(np.nanmax(data)-np.nanmin(data))
     k_data=copy.deepcopy(data)
     
@@ -105,48 +105,48 @@
             
             
             k_data[:,(row_size*i):(row_size*(i+1)),(column_size*j):(column_size*(j+1))]=data_array
         #print(i)
     return k_data  
 
     
-def run_kriging_helper_custom(data,random_mask,rows, cols, kriging_type='ordinary', variogram_model='linear'):
+def run_kriging_helper_custom(data,random_mask,rows, cols, kriging_type, variogram_model):
     k_data=copy.deepcopy(data)
     for i in range(len(rows)-1):
         for j in range(len(cols)-1):
             data_array=data[:,rows[i]:rows[i+1],cols[j]:cols[j+1]]
             mask_array=random_mask[:,rows[i]:rows[i+1],cols[j]:cols[j+1]]
     
             random_indices=np.where(mask_array==0)
-            z=kriging.main_kriging(data_array.copy(),random_indices,kriging_type)
+            z=kriging.main_kriging(data_array.copy(),random_indices,kriging_type,variogram_model)
             
             data_array[random_indices]=z
             k_data[:,rows[i]:rows[i+1],cols[j]:cols[j+1]]=data_array
             
     return k_data
 ##############################################################################
 ##############################################################################
 ##############################################################################
 
 
-def run_kriging(data,random_mask,resolution, kriging_type='ordinary', partitioning=False, variogram_model='linear'):
+def run_kriging(data,random_mask,resolution, kriging_type, variogram_model, partitioning=False):
     if resolution=='050':
         k_data=kriging.run_kriging_helper(data,random_mask,1,1,70,140,kriging_type, variogram_model)
     elif resolution=='025':
         if partitioning:
             k_data=kriging.run_kriging_helper(data,random_mask,3,1,47,281,kriging_type,variogram_model)
         else:
             k_data=kriging.run_kriging_helper(data,random_mask,1,1,141,281,kriging_type,variogram_model)
     else:
         raise "resolution is not recognized"
     return k_data
 
 
 ##############################################################################
 
-def run_custom_kriging(data,random_mask,resolution, rows, cols, kriging_type='ordinary', variogram_model='linear'): #rows and cols determines the partitioning
+def run_custom_kriging(data,random_mask,resolution, rows, cols, kriging_type, variogram_model): #rows and cols determines the partitioning
     k_data=kriging.run_kriging_helper_custom(data,random_mask,rows, cols, kriging_type, variogram_model)
     return k_data
```

### Comparing `harpia-1.26/harpia/tropomi/no2/lib/random_missing_indices/random_indices_20190101_20200101_025_0.5_0.1.npy` & `harpia-1.28/harpia/tropomi/no2/lib/random_missing_indices/random_indices_20190101_20200101_025_0.5_0.1.npy`

 * *Files identical despite different names*

### Comparing `harpia-1.26/harpia/tropomi/no2/lib/random_missing_indices/random_indices_20190101_20200101_050_0.5_0.1.npy` & `harpia-1.28/harpia/tropomi/no2/lib/random_missing_indices/random_indices_20190101_20200101_050_0.5_0.1.npy`

 * *Files identical despite different names*

### Comparing `harpia-1.26/harpia/tropomi/no2/lib/raster_templates/raster_template_130w60w20n55n_005.tif` & `harpia-1.28/harpia/tropomi/no2/lib/raster_templates/raster_template_130w60w20n55n_005.tif`

 * *Files identical despite different names*

### Comparing `harpia-1.26/harpia/tropomi/no2/lib/raster_templates/raster_template_130w60w20n55n_010.tif` & `harpia-1.28/harpia/tropomi/no2/lib/raster_templates/raster_template_130w60w20n55n_010.tif`

 * *Files identical despite different names*

### Comparing `harpia-1.26/harpia/tropomi/no2/lib/raster_templates/raster_template_130w60w20n55n_025.tif` & `harpia-1.28/harpia/tropomi/no2/lib/raster_templates/raster_template_130w60w20n55n_025.tif`

 * *Files identical despite different names*

### Comparing `harpia-1.26/harpia/tropomi/no2/lib/raster_templates/raster_template_130w60w20n55n_050.tif` & `harpia-1.28/harpia/tropomi/no2/lib/raster_templates/raster_template_130w60w20n55n_050.tif`

 * *Files identical despite different names*

### Comparing `harpia-1.26/harpia/tropomi/no2/lib/raster_templates/raster_template_130w60w20n55n_100.tif` & `harpia-1.28/harpia/tropomi/no2/lib/raster_templates/raster_template_130w60w20n55n_100.tif`

 * *Files identical despite different names*

### Comparing `harpia-1.26/harpia/tropomi/no2/utils.py` & `harpia-1.28/harpia/tropomi/no2/utils.py`

 * *Files identical despite different names*

### Comparing `harpia-1.26/harpia.egg-info/PKG-INFO` & `harpia-1.28/harpia.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: harpia
-Version: 1.26
+Version: 1.28
 Summary: A Python Package for Development
 Home-page: https://github.com/rmsolgi/harpia.git
 Author: Ryan Solgi
 Author-email: ryan.solgi@gmail.com
 Maintainer: Ryan Solgi
 Keywords: harpia
 Classifier: Programming Language :: Python :: 3
```

### Comparing `harpia-1.26/harpia.egg-info/SOURCES.txt` & `harpia-1.28/harpia.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `harpia-1.26/setup.py` & `harpia-1.28/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="harpia",
-    version="1.26",
+    version="1.28",
     author="Ryan Solgi",
     author_email="ryan.solgi@gmail.com",
     maintainer='Ryan Solgi',
     description="A Python Package for Development",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/rmsolgi/harpia.git",
```

