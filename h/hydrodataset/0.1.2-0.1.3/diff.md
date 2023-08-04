# Comparing `tmp/hydrodataset-0.1.2.tar.gz` & `tmp/hydrodataset-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hydrodataset-0.1.2.tar", last modified: Mon Jul 31 09:38:15 2023, max compression
+gzip compressed data, was "hydrodataset-0.1.3.tar", last modified: Fri Aug  4 10:44:54 2023, max compression
```

## Comparing `hydrodataset-0.1.2.tar` & `hydrodataset-0.1.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:38:15.436135 hydrodataset-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-31 09:38:05.000000 hydrodataset-0.1.2/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-31 09:38:05.000000 hydrodataset-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-31 09:38:05.000000 hydrodataset-0.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8587 2023-07-31 09:38:15.436135 hydrodataset-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7804 2023-07-31 09:38:05.000000 hydrodataset-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:38:15.436135 hydrodataset-0.1.2/hydrodataset/
--rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-07-31 09:38:05.000000 hydrodataset-0.1.2/hydrodataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    64414 2023-07-31 09:38:05.000000 hydrodataset-0.1.2/hydrodataset/camels.py
--rw-r--r--   0 runner    (1001) docker     (123)     9490 2023-07-31 09:38:05.000000 hydrodataset-0.1.2/hydrodataset/caravan.py
--rw-r--r--   0 runner    (1001) docker     (123)    12823 2023-07-31 09:38:05.000000 hydrodataset-0.1.2/hydrodataset/grdc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-07-31 09:38:05.000000 hydrodataset-0.1.2/hydrodataset/hydro_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-07-31 09:38:05.000000 hydrodataset-0.1.2/hydrodataset/hydro_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5239 2023-07-31 09:38:05.000000 hydrodataset-0.1.2/hydrodataset/hysets.py
--rw-r--r--   0 runner    (1001) docker     (123)    14604 2023-07-31 09:38:05.000000 hydrodataset-0.1.2/hydrodataset/lamah.py
--rw-r--r--   0 runner    (1001) docker     (123)    13929 2023-07-31 09:38:05.000000 hydrodataset-0.1.2/hydrodataset/mopex.py
--rw-r--r--   0 runner    (1001) docker     (123)    39072 2023-07-31 09:38:05.000000 hydrodataset-0.1.2/hydrodataset/multi_datasets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:38:15.436135 hydrodataset-0.1.2/hydrodataset.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8587 2023-07-31 09:38:15.000000 hydrodataset-0.1.2/hydrodataset.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-31 09:38:15.000000 hydrodataset-0.1.2/hydrodataset.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-31 09:38:15.000000 hydrodataset-0.1.2/hydrodataset.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 09:38:15.000000 hydrodataset-0.1.2/hydrodataset.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-31 09:38:15.000000 hydrodataset-0.1.2/hydrodataset.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-31 09:38:15.000000 hydrodataset-0.1.2/hydrodataset.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-31 09:38:05.000000 hydrodataset-0.1.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-31 09:38:15.436135 hydrodataset-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-07-31 09:38:05.000000 hydrodataset-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:44:54.259427 hydrodataset-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-08-04 10:44:41.000000 hydrodataset-0.1.3/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-08-04 10:44:41.000000 hydrodataset-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-08-04 10:44:41.000000 hydrodataset-0.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8587 2023-08-04 10:44:54.259427 hydrodataset-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7804 2023-08-04 10:44:41.000000 hydrodataset-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:44:54.259427 hydrodataset-0.1.3/hydrodataset/
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-08-04 10:44:41.000000 hydrodataset-0.1.3/hydrodataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64410 2023-08-04 10:44:41.000000 hydrodataset-0.1.3/hydrodataset/camels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9490 2023-08-04 10:44:41.000000 hydrodataset-0.1.3/hydrodataset/caravan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12823 2023-08-04 10:44:41.000000 hydrodataset-0.1.3/hydrodataset/grdc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-08-04 10:44:41.000000 hydrodataset-0.1.3/hydrodataset/hydro_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-08-04 10:44:41.000000 hydrodataset-0.1.3/hydrodataset/hydro_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5239 2023-08-04 10:44:41.000000 hydrodataset-0.1.3/hydrodataset/hysets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14604 2023-08-04 10:44:41.000000 hydrodataset-0.1.3/hydrodataset/lamah.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13929 2023-08-04 10:44:41.000000 hydrodataset-0.1.3/hydrodataset/mopex.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39072 2023-08-04 10:44:41.000000 hydrodataset-0.1.3/hydrodataset/multi_datasets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:44:54.259427 hydrodataset-0.1.3/hydrodataset.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8587 2023-08-04 10:44:54.000000 hydrodataset-0.1.3/hydrodataset.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-08-04 10:44:54.000000 hydrodataset-0.1.3/hydrodataset.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-08-04 10:44:54.000000 hydrodataset-0.1.3/hydrodataset.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 10:44:54.000000 hydrodataset-0.1.3/hydrodataset.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-08-04 10:44:54.000000 hydrodataset-0.1.3/hydrodataset.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-04 10:44:54.000000 hydrodataset-0.1.3/hydrodataset.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-08-04 10:44:41.000000 hydrodataset-0.1.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-08-04 10:44:54.259427 hydrodataset-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-08-04 10:44:41.000000 hydrodataset-0.1.3/setup.py
```

### Comparing `hydrodataset-0.1.2/LICENSE` & `hydrodataset-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hydrodataset-0.1.2/PKG-INFO` & `hydrodataset-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hydrodataset
-Version: 0.1.2
+Version: 0.1.3
 Summary: A Python package for downloading and reading hydrological datasets
 Home-page: https://github.com/OuyangWenyu/hydrodataset
 Author: Wenyu Ouyang
 Author-email: wenyuouyang@outlook.com
 License: MIT license
 Keywords: hydrodataset
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `hydrodataset-0.1.2/README.md` & `hydrodataset-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `hydrodataset-0.1.2/hydrodataset/__init__.py` & `hydrodataset-0.1.3/hydrodataset/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 Copyright (c) 2021-2022 Wenyu Ouyang. All rights reserved.
 """
 from pathlib import Path
 import os
 
 __author__ = """Wenyu Ouyang"""
 __email__ = "wenyuouyang@outlook.com"
-__version__ = '0.1.2'
+__version__ = '0.1.3'
 
 # we use a .hydrodataset dir to save the setting
 hydrodataset_setting_dir = Path.home().joinpath(".hydrodataset")
 if not hydrodataset_setting_dir.is_dir():
     hydrodataset_setting_dir.mkdir(parents=True)
 hydrodataset_cache_dir = hydrodataset_setting_dir.joinpath("cache")
 if not hydrodataset_cache_dir.is_dir():
```

### Comparing `hydrodataset-0.1.2/hydrodataset/camels.py` & `hydrodataset-0.1.3/hydrodataset/camels.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Author: Wenyu Ouyang
 Date: 2022-01-05 18:01:11
-LastEditTime: 2023-07-31 10:06:56
+LastEditTime: 2023-08-04 18:27:18
 LastEditors: Wenyu Ouyang
 Description: Read Camels Series ("AUStralia", "BRazil", "ChiLe", "GreatBritain", "UnitedStates") datasets
-FilePath: /hydrodataset/hydrodataset/camels.py
+FilePath: \hydrodataset\hydrodataset\camels.py
 Copyright (c) 2021-2022 Wenyu Ouyang. All rights reserved.
 """
 import json
 import warnings
 import collections
 import fnmatch
 import logging
@@ -1500,78 +1500,80 @@
         obj_cols = attrs_df.columns[attrs_df.dtypes == "object"]
         for c in obj_cols:
             attrs_df[c] = attrs_df[c].str.strip().astype(str)
         # unify id to basin
         attrs_df.index.name = "basin"
         # We use xarray dataset to cache all data
         ds_from_df = attrs_df.to_xarray()
-        units = [
-            "degrees",  # gauge_lat
-            "degrees",  # gauge_lon
-            "m",  # elev_mean
-            "m/km",  # slope_mean
-            "km^2",  # area_gages2
-            "km^2",  # area_geospa_fabric
-            "dimensionless",  # geol_1st_class
-            "dimensionless",  # glim_1st_class_frac
-            "dimensionless",  # geol_2nd_class
-            "dimensionless",  # glim_2nd_class_frac
-            "dimensionless",  # carbonate_rocks_frac
-            "dimensionless",  # geol_porostiy
-            "m^2",  # geol_permeability
-            "dimensionless",  # frac_forest
-            "dimensionless",  # lai_max
-            "dimensionless",  # lai_diff
-            "dimensionless",  # gvf_max
-            "dimensionless",  # gvf_diff
-            "dimensionless",  # dom_land_cover_frac
-            "dimensionless",  # dom_land_cover
-            "m",  # root_depth_50
-            "m",  # root_depth_99
-            "mm/day",  # q_mean
-            "dimensionless",  # runoff_ratio
-            "dimensionless",  # slope_fdc
-            "dimensionless",  # baseflow_index
-            "dimensionless",  # stream_elas
-            "mm/day",  # q5
-            "mm/day",  # q95
-            "days/year",  # high_q_freq
-            "day",  # high_q_dur
-            "days/year",  # low_q_freq
-            "day",  # low_q_dur
-            "percent",  # zero_q_freq
-            "dimensionless",  # hfd_mean, day of year
-            "m",  # soil_depth_pelletier
-            "m",  # soil_depth_statsgo
-            "dimensionless",  # soil_porosity
-            "cm/hr",  # soil_conductivity
-            "m",  # max_water_content
-            "percent",  # sand_frac
-            "percent",  # silt_frac
-            "percent",  # clay_frac
-            "percent",  # water_frac
-            "percent",  # organic_frac
-            "percent",  # other_frac
-            "mm/day",  # p_mean
-            "mm/day",  # pet_mean
-            "dimensionless",  # p_seasonality
-            "dimensionless",  # frac_snow
-            "dimensionless",  # aridity
-            "days/year",  # high_prec_freq
-            "day",  # high_prec_dur
-            "dimensionless",  # high_prec_timing, it is season: spring, summer, fall, winter
-            "days/year",  # low_prec_freq
-            "day",  # low_prec_dur
-            "dimensionless",  # low_prec_timing, season
-            "dimensionless",  # huc_02
-            "dimensionless",  # gauge_name
-        ]
+        units_dict = {
+            "gauge_lat": "degrees",
+            "gauge_lon": "degrees",
+            "elev_mean": "m",
+            "slope_mean": "m/km",
+            "area_gages2": "km^2",
+            "area_geospa_fabric": "km^2",
+            "geol_1st_class": "dimensionless",
+            "glim_1st_class_frac": "dimensionless",
+            "geol_2nd_class": "dimensionless",
+            "glim_2nd_class_frac": "dimensionless",
+            "carbonate_rocks_frac": "dimensionless",
+            "geol_porostiy": "dimensionless",
+            "geol_permeability": "m^2",
+            "frac_forest": "dimensionless",
+            "lai_max": "dimensionless",
+            "lai_diff": "dimensionless",
+            "gvf_max": "dimensionless",
+            "gvf_diff": "dimensionless",
+            "dom_land_cover_frac": "dimensionless",
+            "dom_land_cover": "dimensionless",
+            "root_depth_50": "m",
+            "root_depth_99": "m",
+            "q_mean": "mm/day",
+            "runoff_ratio": "dimensionless",
+            "slope_fdc": "dimensionless",
+            "baseflow_index": "dimensionless",
+            "stream_elas": "dimensionless",
+            "q5": "mm/day",
+            "q95": "mm/day",
+            "high_q_freq": "days/year",
+            "high_q_dur": "day",
+            "low_q_freq": "days/year",
+            "low_q_dur": "day",
+            "zero_q_freq": "percent",
+            "hfd_mean": "dimensionless",
+            "soil_depth_pelletier": "m",
+            "soil_depth_statsgo": "m",
+            "soil_porosity": "dimensionless",
+            "soil_conductivity": "cm/hr",
+            "max_water_content": "m",
+            "sand_frac": "percent",
+            "silt_frac": "percent",
+            "clay_frac": "percent",
+            "water_frac": "percent",
+            "organic_frac": "percent",
+            "other_frac": "percent",
+            "p_mean": "mm/day",
+            "pet_mean": "mm/day",
+            "p_seasonality": "dimensionless",
+            "frac_snow": "dimensionless",
+            "aridity": "dimensionless",
+            "high_prec_freq": "days/year",
+            "high_prec_dur": "day",
+            "high_prec_timing": "dimensionless",
+            "low_prec_freq": "days/year",
+            "low_prec_dur": "day",
+            "low_prec_timing": "dimensionless",
+            "huc_02": "dimensionless",
+            "gauge_name": "dimensionless",
+        }
+
         # Assign units to the variables in the Dataset
-        for col, unit in zip(list(ds_from_df), units):
-            ds_from_df[col].attrs["units"] = unit
+        for var_name in units_dict:
+            if var_name in ds_from_df.data_vars:
+                ds_from_df[var_name].attrs["units"] = units_dict[var_name]
         return ds_from_df
 
     def cache_streamflow_xrdataset(self):
         """Save all basins' streamflow data in a netcdf file in the cache directory
 
         TODO: ONLY SUPPORT CAMELS-US now
         """
```

### Comparing `hydrodataset-0.1.2/hydrodataset/caravan.py` & `hydrodataset-0.1.3/hydrodataset/caravan.py`

 * *Files identical despite different names*

### Comparing `hydrodataset-0.1.2/hydrodataset/grdc.py` & `hydrodataset-0.1.3/hydrodataset/grdc.py`

 * *Files identical despite different names*

### Comparing `hydrodataset-0.1.2/hydrodataset/hydro_dataset.py` & `hydrodataset-0.1.3/hydrodataset/hydro_dataset.py`

 * *Files identical despite different names*

### Comparing `hydrodataset-0.1.2/hydrodataset/hydro_utils.py` & `hydrodataset-0.1.3/hydrodataset/hydro_utils.py`

 * *Files identical despite different names*

### Comparing `hydrodataset-0.1.2/hydrodataset/hysets.py` & `hydrodataset-0.1.3/hydrodataset/hysets.py`

 * *Files identical despite different names*

### Comparing `hydrodataset-0.1.2/hydrodataset/lamah.py` & `hydrodataset-0.1.3/hydrodataset/lamah.py`

 * *Files identical despite different names*

### Comparing `hydrodataset-0.1.2/hydrodataset/mopex.py` & `hydrodataset-0.1.3/hydrodataset/mopex.py`

 * *Files identical despite different names*

### Comparing `hydrodataset-0.1.2/hydrodataset/multi_datasets.py` & `hydrodataset-0.1.3/hydrodataset/multi_datasets.py`

 * *Files identical despite different names*

### Comparing `hydrodataset-0.1.2/hydrodataset.egg-info/PKG-INFO` & `hydrodataset-0.1.3/hydrodataset.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hydrodataset
-Version: 0.1.2
+Version: 0.1.3
 Summary: A Python package for downloading and reading hydrological datasets
 Home-page: https://github.com/OuyangWenyu/hydrodataset
 Author: Wenyu Ouyang
 Author-email: wenyuouyang@outlook.com
 License: MIT license
 Keywords: hydrodataset
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `hydrodataset-0.1.2/hydrodataset.egg-info/SOURCES.txt` & `hydrodataset-0.1.3/hydrodataset.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hydrodataset-0.1.2/setup.py` & `hydrodataset-0.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,10 +61,10 @@
     keywords="hydrodataset",
     name="hydrodataset",
     packages=find_packages(include=["hydrodataset", "hydrodataset.*"]),
     setup_requires=setup_requirements,
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/OuyangWenyu/hydrodataset",
-    version='0.1.2',
+    version='0.1.3',
     zip_safe=False,
 )
```

