# Comparing `tmp/pyroscopegriddingcpu-0.0.0.7.tar.gz` & `tmp/pyroscopegriddingcpu-0.0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyroscopegriddingcpu-0.0.0.7.tar", last modified: Wed Jul 12 19:43:35 2023, max compression
+gzip compressed data, was "pyroscopegriddingcpu-0.0.0.8.tar", last modified: Fri Aug  4 08:22:12 2023, max compression
```

## Comparing `pyroscopegriddingcpu-0.0.0.7.tar` & `pyroscopegriddingcpu-0.0.0.8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 19:43:35.211325 pyroscopegriddingcpu-0.0.0.7/
--rw-rw-rw-   0        0        0     1077 2023-04-06 22:17:54.000000 pyroscopegriddingcpu-0.0.0.7/LICENSE.txt
--rw-rw-rw-   0        0        0    11069 2023-07-12 19:43:35.210325 pyroscopegriddingcpu-0.0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     9962 2023-04-06 22:20:54.000000 pyroscopegriddingcpu-0.0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-07-12 19:43:35.158266 pyroscopegriddingcpu-0.0.0.7/pyroscopegriddingcpu/
--rw-rw-rw-   0        0        0      247 2023-07-12 16:34:35.000000 pyroscopegriddingcpu-0.0.0.7/pyroscopegriddingcpu/__init__.py
--rw-rw-rw-   0        0        0     3506 2023-07-12 16:24:51.000000 pyroscopegriddingcpu-0.0.0.7/pyroscopegriddingcpu/fileparser.py
--rw-rw-rw-   0        0        0    10325 2023-07-12 19:41:52.000000 pyroscopegriddingcpu-0.0.0.7/pyroscopegriddingcpu/filter_data.py
--rw-rw-rw-   0        0        0    30817 2023-07-12 16:27:22.000000 pyroscopegriddingcpu-0.0.0.7/pyroscopegriddingcpu/grid_ncf.py
--rw-rw-rw-   0        0        0     6305 2023-07-12 19:42:57.000000 pyroscopegriddingcpu-0.0.0.7/pyroscopegriddingcpu/gridding.py
--rw-rw-rw-   0        0        0    25955 2023-07-12 19:25:35.000000 pyroscopegriddingcpu-0.0.0.7/pyroscopegriddingcpu/gtools.py
--rw-rw-rw-   0        0        0     9373 2023-07-12 16:33:56.000000 pyroscopegriddingcpu-0.0.0.7/pyroscopegriddingcpu/naming_conventions.py
--rw-rw-rw-   0        0        0    13976 2023-07-12 16:33:50.000000 pyroscopegriddingcpu-0.0.0.7/pyroscopegriddingcpu/sat_data_input.py
--rw-rw-rw-   0        0        0     6275 2023-07-12 15:44:36.000000 pyroscopegriddingcpu-0.0.0.7/pyroscopegriddingcpu/solar_zenith.py
--rw-rw-rw-   0        0        0     5191 2023-07-12 19:12:34.000000 pyroscopegriddingcpu-0.0.0.7/pyroscopegriddingcpu/time_conv.py
-drwxrwxrwx   0        0        0        0 2023-07-12 19:43:35.207365 pyroscopegriddingcpu-0.0.0.7/pyroscopegriddingcpu.egg-info/
--rw-rw-rw-   0        0        0    11069 2023-07-12 19:43:34.000000 pyroscopegriddingcpu-0.0.0.7/pyroscopegriddingcpu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      650 2023-07-12 19:43:34.000000 pyroscopegriddingcpu-0.0.0.7/pyroscopegriddingcpu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 19:43:34.000000 pyroscopegriddingcpu-0.0.0.7/pyroscopegriddingcpu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       74 2023-07-12 19:43:34.000000 pyroscopegriddingcpu-0.0.0.7/pyroscopegriddingcpu.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       84 2023-07-12 19:43:34.000000 pyroscopegriddingcpu-0.0.0.7/pyroscopegriddingcpu.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-07-12 19:43:34.000000 pyroscopegriddingcpu-0.0.0.7/pyroscopegriddingcpu.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-12 19:43:35.212322 pyroscopegriddingcpu-0.0.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1914 2023-07-12 19:43:27.000000 pyroscopegriddingcpu-0.0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-04 08:22:12.343379 pyroscopegriddingcpu-0.0.0.8/
+-rw-rw-rw-   0        0        0     1077 2023-04-06 22:17:54.000000 pyroscopegriddingcpu-0.0.0.8/LICENSE.txt
+-rw-rw-rw-   0        0        0    11069 2023-08-04 08:22:12.342380 pyroscopegriddingcpu-0.0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     9962 2023-04-06 22:20:54.000000 pyroscopegriddingcpu-0.0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-08-04 08:22:12.310379 pyroscopegriddingcpu-0.0.0.8/pyroscopegriddingcpu/
+-rw-rw-rw-   0        0        0      247 2023-07-12 16:34:35.000000 pyroscopegriddingcpu-0.0.0.8/pyroscopegriddingcpu/__init__.py
+-rw-rw-rw-   0        0        0     3506 2023-07-12 16:24:51.000000 pyroscopegriddingcpu-0.0.0.8/pyroscopegriddingcpu/fileparser.py
+-rw-rw-rw-   0        0        0    10376 2023-08-04 06:12:38.000000 pyroscopegriddingcpu-0.0.0.8/pyroscopegriddingcpu/filter_data.py
+-rw-rw-rw-   0        0        0    30819 2023-08-04 07:48:04.000000 pyroscopegriddingcpu-0.0.0.8/pyroscopegriddingcpu/grid_ncf.py
+-rw-rw-rw-   0        0        0     6305 2023-07-12 19:42:57.000000 pyroscopegriddingcpu-0.0.0.8/pyroscopegriddingcpu/gridding.py
+-rw-rw-rw-   0        0        0    25955 2023-07-12 19:25:35.000000 pyroscopegriddingcpu-0.0.0.8/pyroscopegriddingcpu/gtools.py
+-rw-rw-rw-   0        0        0     9373 2023-07-12 16:33:56.000000 pyroscopegriddingcpu-0.0.0.8/pyroscopegriddingcpu/naming_conventions.py
+-rw-rw-rw-   0        0        0    13976 2023-07-12 16:33:50.000000 pyroscopegriddingcpu-0.0.0.8/pyroscopegriddingcpu/sat_data_input.py
+-rw-rw-rw-   0        0        0     6275 2023-07-12 15:44:36.000000 pyroscopegriddingcpu-0.0.0.8/pyroscopegriddingcpu/solar_zenith.py
+-rw-rw-rw-   0        0        0     5191 2023-07-12 19:12:34.000000 pyroscopegriddingcpu-0.0.0.8/pyroscopegriddingcpu/time_conv.py
+drwxrwxrwx   0        0        0        0 2023-08-04 08:22:12.341380 pyroscopegriddingcpu-0.0.0.8/pyroscopegriddingcpu.egg-info/
+-rw-rw-rw-   0        0        0    11069 2023-08-04 08:22:12.000000 pyroscopegriddingcpu-0.0.0.8/pyroscopegriddingcpu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      650 2023-08-04 08:22:12.000000 pyroscopegriddingcpu-0.0.0.8/pyroscopegriddingcpu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-04 08:22:12.000000 pyroscopegriddingcpu-0.0.0.8/pyroscopegriddingcpu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       74 2023-08-04 08:22:12.000000 pyroscopegriddingcpu-0.0.0.8/pyroscopegriddingcpu.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       84 2023-08-04 08:22:12.000000 pyroscopegriddingcpu-0.0.0.8/pyroscopegriddingcpu.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-08-04 08:22:12.000000 pyroscopegriddingcpu-0.0.0.8/pyroscopegriddingcpu.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-04 08:22:12.344380 pyroscopegriddingcpu-0.0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1914 2023-08-04 08:21:50.000000 pyroscopegriddingcpu-0.0.0.8/setup.py
```

### Comparing `pyroscopegriddingcpu-0.0.0.7/LICENSE.txt` & `pyroscopegriddingcpu-0.0.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyroscopegriddingcpu-0.0.0.7/PKG-INFO` & `pyroscopegriddingcpu-0.0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyroscopegriddingcpu
-Version: 0.0.0.7
+Version: 0.0.0.8
 Summary: Data fusion package for transforming L2 satellite to L3 spatial-temporal gridded data
 Home-page: https://github.com/jwei-openscapes/aerosol-data-fusion
 Author: Sally Zhao, Neil Gutkin
 Author-email: zhaosally0@gmail.com
 License: MIT
 Keywords: data fusion,satellite,L2,L3
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `pyroscopegriddingcpu-0.0.0.7/README.md` & `pyroscopegriddingcpu-0.0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `pyroscopegriddingcpu-0.0.0.7/pyroscopegriddingcpu/fileparser.py` & `pyroscopegriddingcpu-0.0.0.8/pyroscopegriddingcpu/fileparser.py`

 * *Files identical despite different names*

### Comparing `pyroscopegriddingcpu-0.0.0.7/pyroscopegriddingcpu/filter_data.py` & `pyroscopegriddingcpu-0.0.0.8/pyroscopegriddingcpu/filter_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -146,14 +146,16 @@
         
         lat1 = np.array(lat1) * float(geo['scale_factor'][0]) + float(geo['add_offset'][0])
         lat.append(lat1)
         lon1 = np.array(lon1) * float(geo['scale_factor'][1]) + float(geo['add_offset'][1])
         lon.append(lon1)
         #phy_vars1 = np.array(phy_vars1) * float(phy['scale_factor'][p]) + float(phy['add_offset'][p])
         #phy_vars1[phy_vars1 == 0] = 0.5
+        
+        phy_vars1 = np.array(phy_vars1) * float(phy['scale_factor'][0]) + float(phy['add_offset'][0])
         phy_vars.append(phy_vars1)
 
         #print("phyvars1: ", len(phy_vars1))
         
         #print(phy_vars1)
 
         # metadata attributes
@@ -166,15 +168,15 @@
                 #store
                 m[key] = phy[key][p]
             
 
         metadata.append(m)
 
     # scale factors
-    phy_vars = np.array(phy_vars) * float(phy['scale_factor'][0]) + float(phy['add_offset'][0])
+    phy_vars = np.array(phy_vars)
     for p in phy_vars:
         pass
         #print("FINAL MAXES HDF:", p.max())
     #print("latitude:", len(lat))
     #print("Physical:", len(phy_vars))
     print("Metadata: ", metadata)
```

### Comparing `pyroscopegriddingcpu-0.0.0.7/pyroscopegriddingcpu/grid_ncf.py` & `pyroscopegriddingcpu-0.0.0.8/pyroscopegriddingcpu/grid_ncf.py`

 * *Files 1% similar despite different names*

```diff
@@ -423,16 +423,16 @@
                         #leogeo_stats["Mean"].append(np.flipud(rotated)) #for leogeo calculation later
                         print("STATISTIC ERROR")
                     
                     #print(np.flipud(rotated))
                     
                     #manually set to fill_value
                     rotated = np.array(rotated)
-                    rotated[rotated > meta[j]["valid_range"][1]+1] = -800#meta[j]["_FillValue"]
-                    rotated[rotated < meta[j]["valid_range"][0]-1] = -800 #meta[j]["_FillValue"]
+                    #rotated[rotated > meta[j]["valid_range"][1]+1] = -800#meta[j]["_FillValue"]
+                    #rotated[rotated < meta[j]["valid_range"][0]-1] = -800 #meta[j]["_FillValue"]
                     
                     final_input = np.flipud(rotated)#.astype(np.short)
                     final_input = final_input #/meta[j]["scale_factor"]
                     #curr_sensor_value = values[index]
                     #values[index][0, :, :] = values[index][0, :, :].astype(np.short)
                     values[index][0, :, :] = final_input 
                     values[index][0, :, :] = values[index][0, :, :].astype("f4")
```

### Comparing `pyroscopegriddingcpu-0.0.0.7/pyroscopegriddingcpu/gridding.py` & `pyroscopegriddingcpu-0.0.0.8/pyroscopegriddingcpu/gridding.py`

 * *Files identical despite different names*

### Comparing `pyroscopegriddingcpu-0.0.0.7/pyroscopegriddingcpu/gtools.py` & `pyroscopegriddingcpu-0.0.0.8/pyroscopegriddingcpu/gtools.py`

 * *Files identical despite different names*

### Comparing `pyroscopegriddingcpu-0.0.0.7/pyroscopegriddingcpu/naming_conventions.py` & `pyroscopegriddingcpu-0.0.0.8/pyroscopegriddingcpu/naming_conventions.py`

 * *Files identical despite different names*

### Comparing `pyroscopegriddingcpu-0.0.0.7/pyroscopegriddingcpu/sat_data_input.py` & `pyroscopegriddingcpu-0.0.0.8/pyroscopegriddingcpu/sat_data_input.py`

 * *Files identical despite different names*

### Comparing `pyroscopegriddingcpu-0.0.0.7/pyroscopegriddingcpu/solar_zenith.py` & `pyroscopegriddingcpu-0.0.0.8/pyroscopegriddingcpu/solar_zenith.py`

 * *Files identical despite different names*

### Comparing `pyroscopegriddingcpu-0.0.0.7/pyroscopegriddingcpu/time_conv.py` & `pyroscopegriddingcpu-0.0.0.8/pyroscopegriddingcpu/time_conv.py`

 * *Files identical despite different names*

### Comparing `pyroscopegriddingcpu-0.0.0.7/pyroscopegriddingcpu.egg-info/PKG-INFO` & `pyroscopegriddingcpu-0.0.0.8/pyroscopegriddingcpu.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyroscopegriddingcpu
-Version: 0.0.0.7
+Version: 0.0.0.8
 Summary: Data fusion package for transforming L2 satellite to L3 spatial-temporal gridded data
 Home-page: https://github.com/jwei-openscapes/aerosol-data-fusion
 Author: Sally Zhao, Neil Gutkin
 Author-email: zhaosally0@gmail.com
 License: MIT
 Keywords: data fusion,satellite,L2,L3
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `pyroscopegriddingcpu-0.0.0.7/pyroscopegriddingcpu.egg-info/SOURCES.txt` & `pyroscopegriddingcpu-0.0.0.8/pyroscopegriddingcpu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyroscopegriddingcpu-0.0.0.7/setup.py` & `pyroscopegriddingcpu-0.0.0.8/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 # Setting up
 setup(
     name = 'pyroscopegriddingcpu',         # Package name
     packages = ['pyroscopegriddingcpu'],   
-    version = '0.0.0.7',      # Initial version
+    version = '0.0.0.8',      # Initial version
     license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
     description = 'Data fusion package for transforming L2 satellite to L3 spatial-temporal gridded data',  
     long_description = long_description,
     long_description_content_type='text/markdown',
     author = 'Sally Zhao, Neil Gutkin',                 
     author_email = 'zhaosally0@gmail.com',     
     url = 'https://github.com/jwei-openscapes/aerosol-data-fusion',   # github repository
```

