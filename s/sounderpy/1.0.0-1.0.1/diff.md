# Comparing `tmp/sounderpy-1.0.0.tar.gz` & `tmp/sounderpy-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sounderpy-1.0.0.tar", last modified: Mon Jul 17 03:59:02 2023, max compression
+gzip compressed data, was "sounderpy-1.0.1.tar", last modified: Fri Aug  4 20:37:45 2023, max compression
```

## Comparing `sounderpy-1.0.0.tar` & `sounderpy-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 03:59:02.346273 sounderpy-1.0.0/
--rw-rw-rw-   0        0        0     1094 2023-07-17 00:45:12.000000 sounderpy-1.0.0/LICENSE.txt
--rw-rw-rw-   0        0        0     3344 2023-07-17 03:59:02.342227 sounderpy-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     2768 2023-07-17 03:48:02.000000 sounderpy-1.0.0/README.md
--rw-rw-rw-   0        0        0      650 2023-07-17 03:52:56.000000 sounderpy-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-17 03:59:02.346273 sounderpy-1.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-17 03:59:02.287835 sounderpy-1.0.0/src/
-drwxrwxrwx   0        0        0        0 2023-07-17 03:59:02.316582 sounderpy-1.0.0/src/sounderpy/
--rw-rw-rw-   0        0        0      470 2023-07-17 02:33:17.000000 sounderpy-1.0.0/src/sounderpy/__init__.py
--rw-rw-rw-   0        0        0    47632 2023-07-17 03:52:27.000000 sounderpy-1.0.0/src/sounderpy/sounderpy.py
-drwxrwxrwx   0        0        0        0 2023-07-17 03:59:02.339351 sounderpy-1.0.0/src/sounderpy.egg-info/
--rw-rw-rw-   0        0        0     3344 2023-07-17 03:59:02.000000 sounderpy-1.0.0/src/sounderpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      237 2023-07-17 03:59:02.000000 sounderpy-1.0.0/src/sounderpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 03:59:02.000000 sounderpy-1.0.0/src/sounderpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-07-17 03:59:02.000000 sounderpy-1.0.0/src/sounderpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-04 20:37:45.830464 sounderpy-1.0.1/
+-rw-rw-rw-   0        0        0     1094 2023-07-17 00:45:12.000000 sounderpy-1.0.1/LICENSE.txt
+-rw-rw-rw-   0        0        0     4884 2023-08-04 20:37:45.822953 sounderpy-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4072 2023-08-03 23:53:29.000000 sounderpy-1.0.1/README.md
+-rw-rw-rw-   0        0        0     1070 2023-08-03 23:48:20.000000 sounderpy-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-04 20:37:45.830464 sounderpy-1.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-04 20:37:45.678139 sounderpy-1.0.1/src/
+drwxrwxrwx   0        0        0        0 2023-08-04 20:37:45.735021 sounderpy-1.0.1/src/sounderpy/
+-rw-rw-rw-   0        0        0      771 2023-08-04 00:37:17.000000 sounderpy-1.0.1/src/sounderpy/__init__.py
+-rw-rw-rw-   0        0        0    71924 2023-08-04 00:41:38.000000 sounderpy-1.0.1/src/sounderpy/sounderpy.py
+drwxrwxrwx   0        0        0        0 2023-08-04 20:37:45.771072 sounderpy-1.0.1/src/sounderpy.egg-info/
+drwxrwxrwx   0        0        0        0 2023-08-04 20:37:45.819707 sounderpy-1.0.1/src/sounderpy.egg-info/.ipynb_checkpoints/
+-rw-rw-rw-   0        0        0     3604 2023-07-27 02:15:00.000000 sounderpy-1.0.1/src/sounderpy.egg-info/.ipynb_checkpoints/PKG-INFO-checkpoint
+-rw-rw-rw-   0        0        0      273 2023-07-27 02:15:00.000000 sounderpy-1.0.1/src/sounderpy.egg-info/.ipynb_checkpoints/SOURCES-checkpoint.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 02:15:00.000000 sounderpy-1.0.1/src/sounderpy.egg-info/.ipynb_checkpoints/dependency_links-checkpoint.txt
+-rw-rw-rw-   0        0        0      137 2023-07-27 02:15:00.000000 sounderpy-1.0.1/src/sounderpy.egg-info/.ipynb_checkpoints/requires-checkpoint.txt
+-rw-rw-rw-   0        0        0       10 2023-07-27 02:15:00.000000 sounderpy-1.0.1/src/sounderpy.egg-info/.ipynb_checkpoints/top_level-checkpoint.txt
+-rw-rw-rw-   0        0        0     4884 2023-08-04 20:37:45.000000 sounderpy-1.0.1/src/sounderpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      607 2023-08-04 20:37:45.000000 sounderpy-1.0.1/src/sounderpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-04 20:37:45.000000 sounderpy-1.0.1/src/sounderpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      137 2023-08-04 20:37:45.000000 sounderpy-1.0.1/src/sounderpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-08-04 20:37:45.000000 sounderpy-1.0.1/src/sounderpy.egg-info/top_level.txt
```

### Comparing `sounderpy-1.0.0/LICENSE.txt` & `sounderpy-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sounderpy-1.0.0/PKG-INFO` & `sounderpy-1.0.1/src/sounderpy.egg-info/.ipynb_checkpoints/PKG-INFO-checkpoint`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 Metadata-Version: 2.1
 Name: sounderpy
 Version: 1.0.0
 Summary: VERTICAL PROFILE DATA RETRIEVAL TOOL
 Author-email: Kyle J Gillett <gille3kj@cmich.edu>
 Project-URL: Homepage, https://github.com/kylejgillett/sounderpy/tree/main
 Project-URL: Documentation, https://github.com/kylejgillett/sounderpy/blob/main/DOCUMENTATION.md
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Scientific/Engineering :: Atmospheric Science
+Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10.0
+Classifier: License :: OSI Approved :: MIT License
+Requires-Python: >=3.1
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # sounderpy
 
 ## WELCOME! thank you for visiting SounderPy!
 This script is used to access vertical profile data for calculations or plotting of a vertical profile (sounding).
```

### Comparing `sounderpy-1.0.0/src/sounderpy/sounderpy.py` & `sounderpy-1.0.1/src/sounderpy/sounderpy.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,140 +1,127 @@
-import cdsapi
-from sys import exit
+# BUILT IN
+from datetime import datetime, timedelta
+import time
+import csv
+import sys
 import requests
-from   metpy.units  import units
-import metpy.calc   as mpcalc
-import xarray as xr
 from urllib.request import urlopen
+import warnings
+# OTHER
+import cdsapi
+import pandas as pd
+import xarray as xr
 import numpy as np
-import numpy.ma       as ma
-from siphon.catalog   import TDSCatalog
-from siphon.ncss      import NCSS
+import numpy.ma as ma
 from scipy import interpolate
-import cartopy.crs as ccrs
+# MATPLOTLIB
+import matplotlib.pyplot as plt
+from mpl_toolkits.axes_grid1.inset_locator import inset_axes
+# METPY
+import metpy.calc as mpcalc
+from metpy.units import units
+from metpy.plots import SkewT, Hodograph
+# SIPHON 
+from siphon.catalog import TDSCatalog
+from siphon.ncss import NCSS
 from siphon.simplewebservice.wyoming import WyomingUpperAir
 from siphon.simplewebservice.iastate import IAStateUpperAir
-from datetime         import datetime
-import time
-import pandas as pd
+from siphon.simplewebservice.igra2 import IGRAUpperAir
 
-version = 'v1.0.0'
-version_date = 'July 17, 2023'
+version = 'v2.0.0'
+version_date = 'August 6th, 2023'
 
 
 '''
         VERTICAL PROFILE DATA RETRIEVAL TOOL
         ------------------------------------
-        
-        This script it used to access vertical profile data for calculations or plotting of a vertical profile (sounding)
-        This script is capable of accessing data from the ECMWF CDS (ERA5 reanalysis), the unidata THREDDS TDS (RAP reanalysis & real time),
-        the University of Wyoming RAOB profile archive (observed), the Iowa State University's RAOB archive (observed) or a manually uploaded
-        .txt file of sounding data.
+        This script it used to access vertical profile data for calculations or plotting of a vertical profile (sounding).
         
         RELEASE
         -------
-        Version: 1.0.0 | July, 17, 2023
+        Version: 2.0.0 | August 6th, 2023
+        
+        DOCUMENTATION
+        -------
+        GiHub Wiki: https://github.com/kylejgillett/sounderpy/wiki
 
         COPYRIGHT
         ---------
         Created by Kyle J Gillett (@wxkylegillett) 2023
 
 '''
 
 
 
 citation_text = f"""
 ## ------------------ VERTICAL PROFILE DATA RETRIEVAL TOOL ------------------------ ##
-##                           {version} | {version_date}                                  ##
+##                           {version} | {version_date}                              ##
 ##                             (C) KYLE J GILLETT                                   ##
-##         THIS TOOL CAN LOAD RAOB, RAP, RUC, ERA5 AND VERTICAL PROFILE DATA        ##
-##  CALL THE FUNCTION '.get_docs()' TO PRINT SIMPLE DOCUMENTATION FOR THIS PACKAGE  ##
+##  THIS TOOL LOADS RAOB, IGRA, RAP, RUC, ERA5, RAP-ANALYSIS, & BUFKIT PROFILE DATA ##
 ## -------------------- THANK YOU FOR USING THIS PACKAGE -------------------------- ##
 """
 print(citation_text)
 
 
 
 
 
 
 
 
-
-
 #################################################################################################################################################
 #                                                      GET_MODEL_DATA() FUNCTION                                                                 
 #################################################################################################################################################
 
 def get_model_data(method, latlon, year, month, day, hour, domain='point'):
     st = time.time()
     
     '''
     get_model_data(method, domain, latlons, year, month, day, hour)
 
-    function used to access model profile data from the ERA5, RAP or RUC
-
-    PARAMETERS
-    ----------
-      name      dtype  required  example         explanation 
-      method:    str,    yes,    'rap-ruc'       model data source: 'rap-ruc', 'era5' 
-      latlon:    list,   yes,    [42.3, -97.3]   ordered list of lat, lon points 
-      year:      str,    yes,    '2014'          4 digit year (UTC)
-      month:     str,    yes,    '06'            2 digit month (UTC)
-      day:       str,    yes,    '16'            2 digit day (UTC)
-      hour:      str,    yes,    '20'            2 digit hour (UTC)
-      domain:    str,    no,     'point'         default='point', single lat/lon 'point' or 'map' for lat/lon box *under dev.
-
-    RETURNS
-    -------
-      raw_data: for ERA5, an xarray.Dataset of ERA5 reanalysis data or
-      raw_data: for RAP/RUC, a netCDF4._netCDF4.Dataset of RAP/RUC reanalysis data
-
-    EXAMPLES
-    --------
-      raw_data = spy.get_model_data('rap', 'point', [42.3, -97.3], '2014', '06', '16', '18')
-      raw_data = spy.get_model_data('era5', 'point', [42.3, -97.3], '2014', '06', '16', '18')
-
-    note: method 'rap-ruc' will try for RAP data first, if the data is not availible, then it will try for RUC data
+    function used to access model reanalysis profile data from the ERA5, RAP or RUC or realtime RAP analysis data
     
     COPYRIGHT
-    ---------
-       Created by Kyle J Gillett (@wxkylegillett) 2023
+    Created by Kyle J Gillett (@wxkylegillett) 2023
 
     '''
     
+    if method not in ['era', 'era5', 'ERA', 'ERA5', 'rap', 'ruc', 'rap-ruc', 'RAP', 'RUC', 'RAP-RUC', 'rap-now', 'RAP-NOW', 'RAP-now']:
+        warnings.filterwarnings("ignore")
+        sys.exit("Invalid 'method' kwarg. Valid methods inlcude ['era5', 'rap-ruc', 'rap-now']")
+    
     global latlon1, source, year1, month1, day1, hour1
     latlon1 = latlon
-    source = str.upper(method)
     year1  = year
     month1 = month
     day1   = day
     hour1  = hour
-
                  #lat            #lat           #lon               #lon
     latlons = [latlon[0] + .5, latlon[0] - .5, latlon[1] - .5, latlon[1] + .5]
 
     
+    
+    
+    
     ######################################################## ERA5 FUNCTION ###################################################################
     if method in ['era', 'era5', 'ERA', 'ERA5']:
-
+        source = 'ERA5'
         print(f'-- ERA5 REANALYSIS DATA ACCESS FUNCTION --\n------------------------------------------')
 
         dataset_presLvls = 'reanalysis-era5-pressure-levels'
         dataset_singleLvls = 'reanalysis-era5-single-levels'
         download_flag = 'false' 
 
         if domain == 'point':
             latlon_list = [latlons[0], latlons[2], latlons[1], latlons[3]]
         elif domain == 'map':
             latlon_list = [latlons[0]+10, latlons[2]-10, latlons[1]-10, latlons[3]+10]
-        else:
-            latlon_list = [9999, 9999, 9999, 9999] 
-            print('[!] FUNCTION ERROR [!]\n[!] method str must be point, or map, this code will now end [!]')
-            exit()
+        else: 
+            warnings.filterwarnings("ignore")
+            sys.exit("'domain' kwarg must be 'point' or 'map'")
 
         # SET UP CALL FOR PRESSURE LEVEL DATA 
         c = cdsapi.Client()
         params = {
                 'product_type':'reanalysis',
                 'variable': ['temperature', 'geopotential', 'relative humidity', 'U WIND COMPONENT', 'V WIND COMPONENT', 'vertical_velocity'],
                 'pressure_level': [
@@ -189,28 +176,29 @@
         raw_data = xr.merge([ds,ds2])
         print('- COMPLETE -')
         elapsed_time = time.time() - st
         print('RUNTIME:', time.strftime("%H:%M:%S", time.gmtime(elapsed_time)))
         return raw_data
 
 
+    
+    
 
     ######################################################## RAP FUNCTION ###################################################################
     if method in ['rap', 'ruc', 'rap-ruc', 'RAP', 'RUC', 'RAP-RUC']:
-
+        
         print(f'-- RAP REANALYSIS DATA ACCESS FUNCTION --\n-----------------------------------------')
 
         if domain == 'point':
             latlon_list = [latlons[2],latlons[3],latlons[1],latlons[0]]
         elif domain == 'map':
             latlon_list = [latlons[2]-10 ,latlons[3]+10,latlons[1]-10,latlons[0]+10]
         else:
-            latlon_list = [9999, 9999, 9999, 9999] 
-            print('[!] FUNCTION ERROR [!]\n[!] method str must be point, or map, this code will now end [!]')
-            exit()
+            warnings.filterwarnings("ignore")
+            sys.exit("'domain' kwarg must be 'point' or 'map'")
 
         urls = {
         'RAP_13km' : 'https://www.ncei.noaa.gov/thredds/ncss/model-rap130/'+str(year)+str(month)+'/'+str(year)+str(month)+str(day)+'/rap_130_'+str(year)+str(month)+str(day)+'_'+str(hour)+'00_000.grb2',
         'RAP_13km_old' : 'https://www.ncdc.noaa.gov/thredds/ncss/model-rap130-old/'+str(year)+str(month)+'/'+str(year)+str(month)+str(day)+'/rap_130_'+str(year)+str(month)+str(day)+'_'+str(hour)+'00_000.grb2',
             
         'RAP_13km_anl' : 'https://www.ncei.noaa.gov/thredds/ncss/model-rap130anl/'+str(year)+str(month)+'/'+str(year)+str(month)+str(day)+'/rap_130_'+str(year)+str(month)+str(day)+'_'+str(hour)+'00_000.grb2',
         'RAP_13km_anl_old' : 'https://www.ncdc.noaa.gov/thredds/ncss/model-rap130anl-old/'+str(year)+str(month)+'/'+str(year)+str(month)+str(day)+'/rap_130_'+str(year)+str(month)+str(day)+'_'+str(hour)+'00_000.grb2',
@@ -238,15 +226,17 @@
                 except:
                     pass
         except:
             pass
         try:
             data = NCSS(url_to_use)
         except:
-            print('[!] ERROR [!]\nNCSS URL FAILED -- THIS HAPPENS WHEN A BAD REQUEST IS MADE. POSSIBLE ERRORS: \n> CHECK TO MAKE SURE YOU ENTERED THE CORRECT DATES.\n> NOTE: DATA IS NOT AVAILIABLE FOR EVERY DATE\n> THIS CATALOG OFTEN EXPERIENCES MISSING DATA/OUTAGES\n> MAKE SURE DATES ARE STRINGS -- MONTH, DAY AND HOUR MUST BE TWO DIGITS (EX: 18, 06, 00)')
+            warnings.filterwarnings("ignore")
+            sys.exit('NCSS URL FAILED -- THIS HAPPENS WHEN A BAD REQUEST IS MADE.\n> CHECK TO MAKE SURE YOU ENTERED THE CORRECT DATES.\n> NOTE: DATA IS NOT AVAILIABLE FOR EVERY DATE\n> THIS CATALOG OFTEN EXPERIENCES MISSING DATA/OUTAGES\n> MAKE SURE DATES ARE STRINGS -- MONTH, DAY AND HOUR MUST BE TWO DIGITS (EX: 18, 06, 00)')
+            
             pass
         query = data.query()
         # Subsets by data
         if source == 'rap':
             query.variables('Pressure_surface',
                         'Geopotential_height_isobaric', 'Geopotential_height_surface',
                         'Temperature_isobaric', 'Temperature_height_above_ground',
@@ -268,156 +258,456 @@
         raw_data = data.get_data(query)
 
         print('- COMPLETE -')
         
         elapsed_time = time.time() - st
         print('RUNTIME:', time.strftime("%H:%M:%S", time.gmtime(elapsed_time)))
         return raw_data
-
-    else:
-        print("[!] ERROR [!]\n[!] You may have entered an invalid method.\nValid methods include 'RAP' or 'ERA5'")
     
     
     
+    ######################################################## RAP-NOW FUNCTION ###################################################################
+    
+    if method in ['rap-now', 'RAP-NOW', 'RAP-now']:
+
+        print(f'-- RAP REANALYSIS DATA ACCESS FUNCTION --\n-----------------------------------------')
+
+        if domain == 'point':
+            latlon_list = [latlons[2],latlons[3],latlons[1],latlons[0]]
+        elif domain == 'map':
+            latlon_list = [latlons[2]-10 ,latlons[3]+10,latlons[1]-10,latlons[0]+10]
+        else:
+            warnings.filterwarnings("ignore")
+            sys.exit("'domain' kwarg must be 'point' or 'map'")
+
+        url = 'http://thredds.ucar.edu/thredds/catalog/grib/NCEP/RAP/CONUS_13km/latest.xml'
+        try:
+            cat = TDSCatalog('http://thredds.ucar.edu/thredds/catalog/grib/NCEP/RAP/CONUS_13km/latest.xml')
+            source = 'RAP ANALYSIS'
+        except:
+            sys.exit("NCSS URL FAILED -- THIS HAPPENS WHEN A BAD REQUEST IS MADE. RAP Analysis data may not be available at this time.")
+            pass
+        # set up query     
+        latest_ds = list(cat.datasets.values())[0]
+        ncss = NCSS(latest_ds.access_urls['NetcdfSubset'])
+        query = ncss.query()
+        # Find start time
+        start_time = ncss.metadata.time_span['begin']
+        fcst_date = datetime.strptime(start_time, '%Y-%m-%dT%H:%M:%SZ')
+        year1  = fcst_date.strftime('%Y')
+        month1 = fcst_date.strftime('%m')
+        day1   = fcst_date.strftime('%d')
+        hour1  = fcst_date.strftime('%H')
+        # Subsets by time
+        query.time(fcst_date).accept('netcdf4')
+        # Subsets by data
+        query.variables('MSLP_MAPS_System_Reduction_msl',
+                'Pressure_surface',
+                'Geopotential_height_isobaric',
+                'Temperature_isobaric',
+                'Relative_humidity_isobaric',
+                'Temperature_height_above_ground',
+                'Relative_humidity_height_above_ground',
+                'u-component_of_wind_height_above_ground', 'v-component_of_wind_height_above_ground', 
+                'u-component_of_wind_isobaric', 'v-component_of_wind_isobaric',
+                'Vertical_velocity_pressure_isobaric',
+                'Convective_available_potential_energy_surface',
+                'Storm_relative_helicity_height_above_ground_layer',
+                'U-Component_Storm_Motion_height_above_ground_layer',
+                'V-Component_Storm_Motion_height_above_ground_layer').add_lonlat()
+
+        # Subsets by area
+        query.lonlat_box(latlon_list[0], latlon_list[1], latlon_list[2], latlon_list[3])
+        # Gets data
+        raw_data = ncss.get_data(query)
+
+        print('- COMPLETE -')
+        
+        elapsed_time = time.time() - st
+        print('RUNTIME:', time.strftime("%H:%M:%S", time.gmtime(elapsed_time)))
+        return raw_data
+
+    
+    
     
     
     
     
 ##################################################################################################################################################
 #                                                     GET_OBS_DATA() FUNCTION                                                                    #
 ##################################################################################################################################################
 
 def get_obs_data(station, year, month, day, hour):
+    
     st = time.time()
+    
     """
     get_obs_data(station, year, month, day, hour)
 
     function used to access and parse RAOB profile data
     this function will search both UW & ISU for desired station and date
-
-    PARAMETERS
-    ----------
-      name      dtype  required  example         explanation 
-      station:   str,    yes,    'OAX'           3 digit RAOB station identifier
-      year:      str,    yes,    '2014'          4 digit year (UTC)
-      month:     str,    yes,    '06'            2 digit month (UTC)
-      day:       str,    yes,    '16'            2 digit day (UTC)
-      hour:      str,    yes,    '18'            2 digit hour (UTC)
-
-    RETURNS
-    -------
-      clean_data: a dict of cleaned profile data ready to use for plotting
-
-    EXAMPLES
-    --------
-      clean_data = spy.get_obs_data('OAX', '2014', '06', '16', '18')
         
     COPYRIGHT
-    ---------
-      Created by Kyle J Gillett (@wxkylegillett) 2023
+    Created by Kyle J Gillett (@wxkylegillett) 2023
     
     """
     
+    print(f'-- OBSERVED DATA ACCESS FUNCTION --\n-----------------------------------')
+    
     global station1, source, year1, month1, day1, hour1
     source = 'obs'
     station1 = station
     year1  = year
     month1 = month
     day1   = day
     hour1  = hour
-    RAOB_STATIONS = pd.read_csv(f'https://raw.githubusercontent.com/kylejgillett/sounderpy/main/RAOB-STATIONS.txt', skiprows=7, skipinitialspace = True)
-    
+    RAOB_STATIONS = pd.read_csv(f'https://raw.githubusercontent.com/kylejgillett/sounderpy/main/txt_files/RAOB-STATIONS.txt', skiprows=7, skipinitialspace = True)
+    IGRA_STATIONS = pd.read_csv(f'https://raw.githubusercontent.com/kylejgillett/sounderpy/main/txt_files/IGRA-STATIONS.txt', skiprows=7, skipinitialspace = True)
     
     dt = datetime(int(year), int(month), int(day), int(hour)) 
     got_data = False
-    for i in range(1, 11):
-        try: 
-            df = WyomingUpperAir.request_data(dt, station)
-            got_data = True
-            if got_data == True:
-                print(f'FOUND RAOB: {station} on {month}/{day}/{year} at {hour}z')
-                break
-        except:
-            if i == 10:
-                print('NO DATA FOR THIS STATION & DATE IN THE UW ARCHIVE, TRYING IEM...')
-                got_data = False          
-        pass
-    if got_data == False: 
+    
+    if RAOB_STATIONS['ICAO'].str.contains(station, na=False, case=True).sum() >= 1:
         for i in range(1, 11):
             try: 
-                df = IAStateUpperAir.request_data(dt, station)
+                df = WyomingUpperAir.request_data(dt, station)
                 got_data = True
                 if got_data == True:
-                    print(f'FOUND RAOB: {station} on {month}/{day}/{year} at {hour}z')
+                    print(f'FOUND RAOB: {station} on {month}/{day}/{year} at {hour}z | From UW')
                     break
             except:
                 if i == 10:
-                    print(f'[!] OPERATION FAILED [!]\n There is likely no available data for station {station} on {month}/{day}/{year} at {hour}z\nPlease make sure you entered a valid station ID and date\nor try a different time, date, or station')
+                    print('NO DATA FOR THIS STATION & DATE IN THE UW ARCHIVE, TRYING IEM...')
                     got_data = False          
             pass
- 
-    if got_data == True:
-        station = RAOB_STATIONS['ICAO'][np.where(RAOB_STATIONS['ICAO'].str.contains(station, na=False, case=True))[0]].values[0]
         
-        new_keys = ['p', 'z', 'T', 'Td', 'u', 'v']
-        old_keys = ['pressure', 'height', 'temperature', 'dewpoint', 'u_wind', 'v_wind'] # 'latitude', 'longitude']
-        units_list = ['hPa', 'meter', 'degC', 'degC', 'kt', 'kt']
-        clean_data = {}
-        non_dups = np.concatenate(([True], np.diff(df.to_dict('list')['pressure']) != 0))
-        for old_key, new_key, unit in zip (old_keys, new_keys, units_list):
-            clean_data[new_key] = np.array(df.to_dict('list')[old_key])[non_dups]*units(unit)
-        clean_data['station_info'] = [RAOB_STATIONS[RAOB_STATIONS['ICAO']==station]['ICAO'].values[0],
-                                      RAOB_STATIONS[RAOB_STATIONS['ICAO']==station]['NAME'].values[0],
-                                      RAOB_STATIONS[RAOB_STATIONS['ICAO']==station]['LOC'].values[0],
-                                      raob_latlon(station),
-                                      RAOB_STATIONS[RAOB_STATIONS['ICAO']==station]['EL(m)'].values[0]]
-        try:
-            slc = (len(clean_data['p']) - np.where(clean_data['p']<=98.*units('hPa'))[0][0])
-            for key in new_keys:
-                clean_data[key] = clean_data[key][:-slc]
-        except:
-            pass
-        elapsed_time = time.time() - st
-        print('RUNTIME:', time.strftime("%H:%M:%S", time.gmtime(elapsed_time)))
-        return clean_data    
+        if got_data == False: 
+            for i in range(1, 11):
+                try: 
+                    df = IAStateUpperAir.request_data(dt, station)
+                    got_data = True
+                    if got_data == True:
+                        print(f'FOUND RAOB: {station} on {month}/{day}/{year} at {hour}z | From IEM')
+                        break
+                except:
+                    if i == 10:
+                        warnings.filterwarnings("ignore")
+                        sys.exit(f"There is likely no available data for station {station} on {month}/{day}/{year} at {hour}z\nPlease make sure you entered a valid station ID and date\nor try a different time, date, or station")
+                        got_data = False          
+                pass
+
+        if got_data == True:
+            station = RAOB_STATIONS['ICAO'][np.where(RAOB_STATIONS['ICAO'].str.contains(station, na=False, case=True))[0]].values[0].strip()
+
+            new_keys = ['p', 'z', 'T', 'Td', 'u', 'v']
+            old_keys = ['pressure', 'height', 'temperature', 'dewpoint', 'u_wind', 'v_wind'] # 'latitude', 'longitude']
+            units_list = ['hPa', 'meter', 'degC', 'degC', 'kt', 'kt']
+            clean_data = {}
+            non_dups = np.concatenate(([True], np.diff(df.to_dict('list')['pressure']) != 0))
+            for old_key, new_key, unit in zip (old_keys, new_keys, units_list):
+                clean_data[new_key] = np.array(df.to_dict('list')[old_key])[non_dups]*units(unit)
+            clean_data['site_info'] = {
+                'site-id'   : RAOB_STATIONS[RAOB_STATIONS['ICAO']==station]['ICAO'].values[0],
+                'site-name' : RAOB_STATIONS[RAOB_STATIONS['ICAO']==station]['NAME'].values[0],
+                'site-lctn' : RAOB_STATIONS[RAOB_STATIONS['ICAO']==station]['LOC'].values[0],
+                'site-latlon' : raob_latlon(station),
+                'site-elv'  : RAOB_STATIONS[RAOB_STATIONS['ICAO']==station]['EL(m)'].values[0],
+                'source'    : 'RAOB',
+                'model'     : 'no-model',
+                'fcst-hour' : 'no-fcst-hour',
+                'run-time'  : ['no-run-time'],
+                'valid-time': [year, month, day, hour]}
+            
+            try:
+                slc = (len(clean_data['p']) - np.where(clean_data['p']<=98.*units('hPa'))[0][0])
+                for key in new_keys:
+                    clean_data[key] = clean_data[key][:-slc]
+            except:
+                pass
+            elapsed_time = time.time() - st
+            print('RUNTIME:', time.strftime("%H:%M:%S", time.gmtime(elapsed_time)))
+            return clean_data 
+
+            
+    elif IGRA_STATIONS['ID'].str.contains(station, na=False, case=True).sum() >= 1:
+        for i in range(1, 3):
+            try: 
+                df = IGRAUpperAir.request_data(dt, station)
+                got_data = True
+                if got_data == True:
+                    print(f'FOUND DATA: {station} on {month}/{day}/{year} at {hour}z | From IGRAv2')
+                    break
+            except:
+                if i == 3:
+                    warnings.filterwarnings("ignore")
+                    sys.exit(f"There is likely no available data for station {station} on {month}/{day}/{year} at {hour}z\nPlease make sure you entered a valid station ID and date\nor try a different time, date, or station")
+                    got_data = False        
+        if got_data == True:
+            station = IGRA_STATIONS['ID'][np.where(IGRA_STATIONS['ID'].str.contains(station, na=False, case=True))[0]].values[0].strip()
+            
+            head = df[1]
+            df = df[0]
+            new_keys = ['p', 'z', 'T', 'Td', 'u', 'v']
+            old_keys = ['pressure', 'height', 'temperature', 'dewpoint', 'u_wind', 'v_wind'] # 'latitude', 'longitude']
+            units_list = ['hPa', 'meter', 'degC', 'degC', 'kt', 'kt']
+            clean_data = {}
+            zflag=np.array(df['zflag'])
+            pflag=np.array(df['pflag'])
+            tflag=np.array(df['tflag'])
+            for old_key, new_key, unit in zip (old_keys, new_keys, units_list):
+                clean_data[new_key] = np.array(df.to_dict('list')[old_key])[zflag+pflag+tflag>=4]*units(unit)
+            clean_data['site_info'] = {
+                    'site-id'   : IGRA_STATIONS[IGRA_STATIONS['ID']==station]['ID'].str.strip().values[0],
+                    'site-name' : IGRA_STATIONS[IGRA_STATIONS['ID']==station]['NAME'].str.strip().values[0],
+                    'site-lctn' : 'no-site-location',
+                    'site-latlon' : igra_latlon(station),
+                    'site-elv'  : IGRA_STATIONS[IGRA_STATIONS['ID']==station]['EL(m)'].values[0],
+                    'source'    : 'IGRA',
+                    'model'     : 'no-model',
+                    'fcst-hour' : 'no-fcst-hour',
+                    'run-time'  : ['no-run-time'],
+                    'valid-time': [year, month, day, hour]}
+            
+            clean_data['u'] = clean_data['u']*1.94384
+            clean_data['v'] = clean_data['v']*1.94384
+            elapsed_time = time.time() - st
+            print('RUNTIME:', time.strftime("%H:%M:%S", time.gmtime(elapsed_time)))
+            return clean_data     
+
+        else: 
+            warnings.filterwarnings("ignore")
+            sys.exit(f"There is likely no available data for station {station} on {month}/{day}/{year} at {hour}z\nPlease make sure you entered a valid station ID and date\nor try a different time, date, or station")
+        
+    else:
+        warnings.filterwarnings("ignore")
+        sys.exit(f"There is likely no available data for station {station} on {month}/{day}/{year} at {hour}z\nPlease make sure you entered a valid station ID and date\nor try a different time, date, or station")
+    
+
+    
 
     
     
     
     
     
     
+##################################################################################################################################################
+#                                                    GET_BUFKIT_DATA() FUNCTION                                                                   #
+##################################################################################################################################################
+    
+def get_bufkit_data(model, station, fcst_hour, run_year=None, run_month=None, run_day=None, run_hour=None):
+    st = time.time()
+    
+    '''
+    function used to load and parse BUFKIT sounding data
+
+    COPYRIGHT
+    Created by Kyle J Gillett (@wxkylegillett) 2023
+
+    '''
+    print(f'-- BUFKIT DATA ACCESS FUNCTION --\n---------------------------------')
+    model = str.lower(model)
+    
+    # GET MOST-RECENT RUNS FROM PSU SERVERS 
+    if run_year == None:
+        if model not in ['gfs', 'nam', 'namnest', 'rap', 'hrrr', 'sref', 'hiresw']:
+            sys.exit("NOT A VALID MODEL -- VALID MODELS ARE ['GFS', 'NAM', 'NAMNEST', 'RAP', 'HRRR', 'SREF', 'HIRESW']")
+        if model == 'gfs':
+            model3 = 'gfs3' 
+        else:
+            model3 = model
+        data_conn = f'http://www.meteo.psu.edu/bufkit/data/{model.upper()}/{model3}_{station.lower()}.buf'
+        
+    # GET ARCHIVE DATA FROM THE IEM SERVERS. CORRECT GFS & NAM MODEL NAMES     
+    else:
+        if model not in ['gfs', 'nam', 'namnest', 'rap', 'hrrr']:
+            sys.exit("NOT A VALID MODEL -- VALID MODELS ARE ['GFS', 'NAM', 'NAMNEST', 'RAP', 'HRRR']")
+        if model == 'namnest':
+            model == 'nam4km'
+        if model == 'gfs':
+            model3 = 'gfs3' 
+        else:
+            model3 = model
+        data_conn = f'https://mtarchive.geol.iastate.edu/{run_year}/{run_month}/{run_day}/bufkit/{run_hour}/{model}/{model3}_{station.lower()}.buf'  
+
+        
+    # GET BUFKIT FILE 
+    # CONVERT LINES OF BYTES TO STRINGS 
+    buf_file = urlopen(data_conn)
+    buf_file = [str(line).replace("b'", "").replace("\\r\\n'", "") for line in buf_file]
+    
+    BUFKIT_STATIONS = pd.read_csv(f'https://raw.githubusercontent.com/kylejgillett/sounderpy/main/txt_files/BUFKIT-STATIONS-MASTER.csv', skiprows=7, skipinitialspace = True)
+    
+    station = BUFKIT_STATIONS['ID'][np.where(BUFKIT_STATIONS['ID'].str.contains(station, na=False, case=True))[0]].values[0]
+    
+    # Create temp data list and record trigger
+    tmp_data, sounding_headers, derived_headers = [], '', ''
+    recordSounding = False
+    
+    run_time = buf_file[4][buf_file[4].index('TIME') + 7:(buf_file[4].index('TIME')+9)+9]
+    run_dt = datetime(int(f'20{run_time[0:2]}'), int(run_time[2:4]), int(run_time[4:6]), int(run_time[7:9])) 
+    fct_dt = run_dt + timedelta(hours = fcst_hour)
+    stp_dt = fct_dt + timedelta(hours = 1)
+    
+    # Loop over each line in data file
+    for line in buf_file:
+        # Find start of sounding data
+        if f'TIME = {fct_dt.strftime("%Y")[2:4]}{fct_dt.strftime("%m")}{fct_dt.strftime("%d")}/{fct_dt.strftime("%H")}00' in line:
+            recordSounding=True  
+        if 'SNPARM' in line:
+            sounding_headers=line[line.index('=')+2:].replace(' ', '').split(';')
+        if 'STNPRM' in line:
+            derived_headers=line[line.index('=')+2:].replace(' ', '').split(';')
+        # Append data line to temp data list
+        if recordSounding:
+            tmp_data.append(line)
+        # Break out of loop when end key reached
+        if f'TIME = {stp_dt.strftime("%Y")[2:4]}{stp_dt.strftime("%m")}{stp_dt.strftime("%d")}/{stp_dt.strftime("%H")}00' in line:
+            tmp_data.pop(-1)
+            break
+
+    station_headers=['STID', 'STNM', 'TIME', 'SLAT', 'SLON', 'SELV', 'STIM']
+    tmp_str=''
+    recordStationInfo, recordDerivedQty, recordSoundingQty = False, False, True
+    station_metadata, derived_data, sounding_data = [], [], []
+
+    for line in tmp_data:
+        # Check for station infromation
+        if recordStationInfo and line=='':
+            # Break values up to only be seperated by one whitespace
+            station_info=(tmp_str.replace(' = ', ' '))
+
+            # Split values into list
+            station_info=station_info.split(' ')
+
+            # Remove label values
+            station_info=[x for x in station_info if x not in station_headers]
+            while '' in station_info:
+                station_info.remove('')
+
+            # Add to main list
+            station_metadata.append(station_info)
+
+            # Reset temp vars
+            tmp_str=''
+            recordStationInfo=False
+
+        if any(var in line for var in station_headers):
+            recordStationInfo=True
+            tmp_str+=(' ' + line)
+
+        # Check for derived sounding quantities
+        if recordDerivedQty==True and line=='':
+            # Break values up to only be seperated by one whitespace
+            derived_qty=(tmp_str.replace(' = ', ' '))
+            # Split values into list
+            derived_qty=derived_qty.split(' ')
+            # Remove non-numeric values
+            derived_qty=[x for x in derived_qty if x not in derived_headers]
+            while '' in derived_qty:
+                derived_qty.remove('')
+            # Add to main list
+            derived_data.append(derived_qty)
+            # Reset temp vars
+            tmp_str=''
+            recordDerivedQty=False
+        if any(var in line for var in derived_headers):
+            recordDerivedQty=True
+            tmp_str+=(' ' + line)
+        # Check for sounding quantities
+        if any(var in line for var in sounding_headers):
+            recordSoundingQty=True
+        if recordSoundingQty and line=='':
+            level_list=[]
+            # Split data string into values
+            data_list=tmp_str.split(' ')
+            # Remove empty indices
+            while '' in data_list:
+                data_list.remove('')
+            # Break data up into pressure levels
+            for i in range(0, len(data_list), len(sounding_headers)):
+                level_list.append(data_list[i:len(sounding_headers)+i])
+        elif recordSoundingQty:
+            if any(var in line for var in sounding_headers)==False:
+                tmp_str+=(' ' + line)
+
+    p = []
+    z = []
+    T = []
+    Td = []
+    ws = []
+    wd = []
+
+    if model in ['GFS', 'gfs']:
+        for i in range(0, len(level_list)):
+            p.append(float(level_list[i][0]))
+            z.append(float(level_list[i][8]))
+            T.append(float(level_list[i][1]))
+            Td.append(float(level_list[i][3]))
+            ws.append(float(level_list[i][6]))
+            wd.append(float(level_list[i][5]))  
+    else:
+        for i in range(0, len(level_list)):
+            p.append(float(level_list[i][0]))
+            z.append(float(level_list[i][9]))
+            T.append(float(level_list[i][1]))
+            Td.append(float(level_list[i][3]))
+            ws.append(float(level_list[i][6]))
+            wd.append(float(level_list[i][5])) 
+    u = list(mpcalc.wind_components(ws*units.kts, wd*units.degrees)[0].m)
+    v = list(mpcalc.wind_components(ws*units.kts, wd*units.degrees)[1].m)
+    
+    def find_nearest(array, value):
+        array = np.asarray(array)
+        nearest_idx = (np.abs(array - value)).argmin()
+        return nearest_idx
+    
+    hPa100 = find_nearest(p, 50)
+
+    clean_data = {}
+    lists = [p[0:hPa100], z[0:hPa100], T[0:hPa100], Td[0:hPa100], u[0:hPa100], v[0:hPa100]]
+    keys = ['p', 'z', 'T', 'Td', 'u', 'v']
+    units_list = ['hPa', 'meter', 'degC', 'degC', 'kt', 'kt']
+    for key, lst, unit in zip(keys, lists, units_list):
+        clean_data[key] = lst*units(unit) 
+    
+    clean_data['site_info'] = {
+                'site-id'   : BUFKIT_STATIONS[BUFKIT_STATIONS['ID']==station]['ID'].str.strip().values[0],
+                'site-name' : BUFKIT_STATIONS[BUFKIT_STATIONS['ID']==station]['NAME'].str.strip().values[0],
+                'site-lctn' : BUFKIT_STATIONS[BUFKIT_STATIONS['ID']==station]['LOC'].str.strip().values[0],
+                'site-latlon' : [BUFKIT_STATIONS[BUFKIT_STATIONS['ID']==station]['LAT'].values[0], BUFKIT_STATIONS[BUFKIT_STATIONS['ID']==station]['LAT'].values[0]],
+                'site-elv'  : BUFKIT_STATIONS[BUFKIT_STATIONS['ID']==station]['EL(m)'].values[0],
+                'source'    : 'BUFKIT',
+                'model'     : str.upper(model),
+                'fcst-hour' : f'F0{fcst_hour}',
+                'run-time'  : [run_dt.strftime("%Y"), run_dt.strftime("%m"), run_dt.strftime("%d"), run_dt.strftime("%H")],
+                'valid-time': [fct_dt.strftime("%Y"), fct_dt.strftime("%m"), fct_dt.strftime("%d"), fct_dt.strftime("%H")]} 
+    
+    elapsed_time = time.time() - st
+    print('RUNTIME:', time.strftime("%H:%M:%S", time.gmtime(elapsed_time)))
+    return clean_data
     
     
     
     
 
     
 ##################################################################################################################################################
 #                                                        PARSE_DATA() FUNCTION                                                                   #
 ##################################################################################################################################################
 
     
 def parse_data(raw_data):
+    
     st = time.time()
+    
     '''
-    parse_data() [function, used to parse sounding data after using a get_data() function]
+    function used to parse sounding data after using a get_model_data() function
 
-    PARAMETERS
-    ----------
-     name          dtype      required   explanation 
-     raw_data:     dataset,   required,  xr.DataSet containing ERA5 renalaysis data
-    
-    RETURNS
-    -------
-     name         dtype    explanation 
-     clean_data   dict,    cleaned profile data with units in a dict format. 
-    
     COPYRIGHT
-    ---------
     Created by Kyle J Gillett (@wxkylegillett) 2023
 
     '''
     
     if str(type(raw_data)) == "<class 'xarray.core.dataset.Dataset'>":
         
         print(f'-- ERA5 REANALYSIS DATA PARSE FUNCTION --\n------------------------------------------')
@@ -452,53 +742,87 @@
         }
 
 
     
     
     
     if str(type(raw_data)) == "<class 'netCDF4._netCDF4.Dataset'>":
-
-        print(f'-- RAP REANALYSIS DATA PARSE FUNCTION --\n------------------------------------------')
-
+            
+            print(f'-- RAP REANALYSIS DATA PARSE FUNCTION --\n------------------------------------------')
+            if "Geopotential_height_surface" in raw_data.variables.keys():
     
-        vert_data = {
-            'vert_T' : (ma.getdata(raw_data.variables['Temperature_isobaric'][0,:,:,:]-273.15)),
-            'vert_p' : (np.array([100, 125, 150, 175, 200, 225, 250, 275, 300, 325, 350, 375, 400, 425, 450, 475, 500, 525, 550, 575, 600, 625, 650, 675, 700, 725, 750, 775, 800, 825, 850, 875, 900, 925, 950, 975, 1000])),
-            'vert_z' : (ma.getdata(raw_data.variables['Geopotential_height_isobaric'][0,:,:,:])),
-            'vert_rh': (ma.getdata(raw_data.variables['Relative_humidity_isobaric'][0,:,:,:])),
-            'vert_u' : (ma.getdata(raw_data.variables['u-component_of_wind_isobaric'][0,:,:,:]*1.94384)),
-            'vert_v' : (ma.getdata(raw_data.variables['v-component_of_wind_isobaric'][0,:,:,:]*1.94384)),
-            'vert_w' : (ma.getdata(raw_data.variables['Vertical_velocity_pressure_isobaric'][0,:,:,:])),
-            'vert_Td': (mpcalc.dewpoint_from_relative_humidity(
-                (ma.getdata(raw_data.variables['Temperature_isobaric'][0,:,:,:]-273.15))*units.degC, 
-                (ma.getdata(raw_data.variables['Relative_humidity_isobaric'][0,:,:,:])*units.percent))).m,
-        } 
-
-        sfc_data = {
-            'sfc_T' : (ma.getdata(raw_data.variables['Temperature_height_above_ground'][0,0,:,:]-273.15)),
-            'sfc_p' : (ma.getdata(raw_data.variables['Pressure_surface'][0,:,:]/100)),
-            'sfc_z' : (ma.getdata(raw_data.variables['Geopotential_height_surface'][0,:,:])),
-            'sfc_rh': (ma.getdata(raw_data.variables['Relative_humidity_height_above_ground'][0,0,:,:])),
-            'sfc_u' : (ma.getdata(raw_data.variables['u-component_of_wind_height_above_ground'][0,0,:,:]*1.94384)),
-            'sfc_v' : (ma.getdata(raw_data.variables['v-component_of_wind_height_above_ground'][0,0,:,:]*1.94384)),
-            'sfc_Td': (mpcalc.dewpoint_from_relative_humidity(
-                (ma.getdata(raw_data.variables['Temperature_height_above_ground'][0,0,:,:]-273.15))*units.degC, 
-                (ma.getdata(raw_data.variables['Relative_humidity_height_above_ground'][0,0,:,:])*units.percent))).m,
-        } 
+                vert_data = {
+                    'vert_T' : (ma.getdata(raw_data.variables['Temperature_isobaric'][0,:,:,:]-273.15)),
+                    'vert_p' : (np.array([100, 125, 150, 175, 200, 225, 250, 275, 300, 325, 350, 375, 400, 425, 450, 475, 500, 525, 550, 575, 600, 625, 650, 675, 700, 725, 750, 775, 800, 825, 850, 875, 900, 925, 950, 975, 1000])),
+                    'vert_z' : (ma.getdata(raw_data.variables['Geopotential_height_isobaric'][0,:,:,:])),
+                    'vert_rh': (ma.getdata(raw_data.variables['Relative_humidity_isobaric'][0,:,:,:])),
+                    'vert_u' : (ma.getdata(raw_data.variables['u-component_of_wind_isobaric'][0,:,:,:]*1.94384)),
+                    'vert_v' : (ma.getdata(raw_data.variables['v-component_of_wind_isobaric'][0,:,:,:]*1.94384)),
+                    'vert_w' : (ma.getdata(raw_data.variables['Vertical_velocity_pressure_isobaric'][0,:,:,:])),
+                    'vert_Td': (mpcalc.dewpoint_from_relative_humidity(
+                        (ma.getdata(raw_data.variables['Temperature_isobaric'][0,:,:,:]-273.15))*units.degC, 
+                        (ma.getdata(raw_data.variables['Relative_humidity_isobaric'][0,:,:,:])*units.percent))).m,
+                } 
+
+                sfc_data = {
+                    'sfc_T' : (ma.getdata(raw_data.variables['Temperature_height_above_ground'][0,0,:,:]-273.15)),
+                    'sfc_p' : (ma.getdata(raw_data.variables['Pressure_surface'][0,:,:]/100)),
+                    'sfc_z' : (ma.getdata(raw_data.variables['Geopotential_height_surface'][0,:,:])),
+                    'sfc_rh': (ma.getdata(raw_data.variables['Relative_humidity_height_above_ground'][0,0,:,:])),
+                    'sfc_u' : (ma.getdata(raw_data.variables['u-component_of_wind_height_above_ground'][0,0,:,:]*1.94384)),
+                    'sfc_v' : (ma.getdata(raw_data.variables['v-component_of_wind_height_above_ground'][0,0,:,:]*1.94384)),
+                    'sfc_Td': (mpcalc.dewpoint_from_relative_humidity(
+                        (ma.getdata(raw_data.variables['Temperature_height_above_ground'][0,0,:,:]-273.15))*units.degC, 
+                        (ma.getdata(raw_data.variables['Relative_humidity_height_above_ground'][0,0,:,:])*units.percent))).m,
+                } 
+
+                latlon_data = {
+                'data_lat'    : (ma.getdata(1000*(raw_data.variables[raw_data.variables['Pressure_surface'].dimensions[1]][:]))),
+                'data_lon'    : (ma.getdata(1000*(raw_data.variables[raw_data.variables['Pressure_surface'].dimensions[2]][:]))),
+                'data_latnum' : (ma.getdata(1000*(raw_data.variables[raw_data.variables['Pressure_surface'].dimensions[1]][:]))).shape[0],
+                'data_lonnum' : (ma.getdata(1000*(raw_data.variables[raw_data.variables['Pressure_surface'].dimensions[2]][:]))).shape[0]
+                }
 
-        latlon_data = {
-        'data_lat'    : (ma.getdata(1000*(raw_data.variables[raw_data.variables['Pressure_surface'].dimensions[1]][:]))),
-        'data_lon'    : (ma.getdata(1000*(raw_data.variables[raw_data.variables['Pressure_surface'].dimensions[2]][:]))),
-        'data_latnum' : (ma.getdata(1000*(raw_data.variables[raw_data.variables['Pressure_surface'].dimensions[1]][:]))).shape[0],
-        'data_lonnum' : (ma.getdata(1000*(raw_data.variables[raw_data.variables['Pressure_surface'].dimensions[2]][:]))).shape[0]
-        }
-    
-    
-    
-        
+            else: 
+                vert_data = {
+                'vert_T' : (ma.getdata(raw_data.variables['Temperature_isobaric'][0,:,:,:]-273.15)),
+                'vert_p' : (np.array([100, 125, 150, 175, 200, 225, 250, 275, 300, 325, 350, 375, 400, 425, 450, 475, 500, 525, 550, 575, 600, 625, 650, 675, 700, 725, 750, 775, 800, 825, 850, 875, 900, 925, 950, 975, 1000])),
+                'vert_z' : (ma.getdata(raw_data.variables['Geopotential_height_isobaric'][0,:,:,:])),
+                'vert_rh': (ma.getdata(raw_data.variables['Relative_humidity_isobaric'][0,:,:,:])),
+                'vert_u' : (ma.getdata(raw_data.variables['u-component_of_wind_isobaric'][0,:,:,:]*1.94384)),
+                'vert_v' : (ma.getdata(raw_data.variables['v-component_of_wind_isobaric'][0,:,:,:]*1.94384)),
+                'vert_w' : (ma.getdata(raw_data.variables['Vertical_velocity_pressure_isobaric'][0,:,:,:])),
+                'vert_Td': (mpcalc.dewpoint_from_relative_humidity(
+                    (ma.getdata(raw_data.variables['Temperature_isobaric'][0,:,:,:]-273.15))*units.degC, 
+                    (ma.getdata(raw_data.variables['Relative_humidity_isobaric'][0,:,:,:])*units.percent))).m,
+            } 
+                
+                sfc_data = {
+                'sfc_T' : (ma.getdata(raw_data.variables['Temperature_height_above_ground'][0,0,:,:]-273.15)),
+                'sfc_p' : (ma.getdata(raw_data.variables['Pressure_surface'][0,:,:]/100)),
+                #'sfc_z' : (ma.getdata(raw_data.variables['Geopotential_height_surface'][0,:,:])),
+                'sfc_rh': (ma.getdata(raw_data.variables['Relative_humidity_height_above_ground'][0,0,:,:])),
+                'sfc_u' : (ma.getdata(raw_data.variables['u-component_of_wind_height_above_ground'][0,0,:,:]*1.94384)),
+                'sfc_v' : (ma.getdata(raw_data.variables['v-component_of_wind_height_above_ground'][0,0,:,:]*1.94384)),
+                'sfc_Td': (mpcalc.dewpoint_from_relative_humidity(
+                    (ma.getdata(raw_data.variables['Temperature_height_above_ground'][0,0,:,:]-273.15))*units.degC, 
+                    (ma.getdata(raw_data.variables['Relative_humidity_height_above_ground'][0,0,:,:])*units.percent))).m,
+                } 
+                sfc_data['sfc_z'] = np.zeros(sfc_data['sfc_p'].shape)
+                for i in range(0,sfc_data['sfc_p'].shape[0]):
+                    for j in range(0,sfc_data['sfc_p'].shape[1]):
+                        sfc_data['sfc_z'][i,j]=np.interp([sfc_data['sfc_p'][i,j]],vert_data['vert_p'],vert_data['vert_z'][:,i,j])[0]
+                        vert_data['vert_z'][:,i,j]=vert_data['vert_z'][:,i,j]-sfc_data['sfc_z'][i,j]
+    
+                latlon_data = {
+                'data_lat'    : (ma.getdata(1000*(raw_data.variables[raw_data.variables['Pressure_surface'].dimensions[1]][:]))),
+                'data_lon'    : (ma.getdata(1000*(raw_data.variables[raw_data.variables['Pressure_surface'].dimensions[2]][:]))),
+                'data_latnum' : (ma.getdata(1000*(raw_data.variables[raw_data.variables['Pressure_surface'].dimensions[1]][:]))).shape[0],
+                'data_lonnum' : (ma.getdata(1000*(raw_data.variables[raw_data.variables['Pressure_surface'].dimensions[2]][:]))).shape[0]
+                }
         
     # NOW THAT DATA IS PARSED AND IN THE SAME FORMAT, CLEAN IT UP:    
     
     def get_sfc_index(height_arr):
         i = 0
         while i < len(height_arr):
             if height_arr[i] >= 0:
@@ -511,15 +835,14 @@
         i = 0
         while i < len(mod_arr):
             mod_arr[i] = arr[i + sfc_index]
             i = i + 1
         mod_arr = np.insert(mod_arr, 0, sfc_val)
         return mod_arr
     
-    crs = ccrs.PlateCarree()
     clons, clats = np.meshgrid(latlon_data['data_lon'], latlon_data['data_lat'])
     tlons = clons 
     tlats = clats
     def haversine(lon_arr, lat_arr, lon_point, lat_point): 
         distance = 6371*(2*np.arcsin(np.sqrt(np.sin((np.radians(lat_arr)-np.radians(lat_point))/2)**2 + np.cos(np.radians(lat_point)) * np.cos(np.radians(lat_arr)) * np.sin((np.radians(lon_arr)-np.radians(lon_point))/2)**2)))
         return distance
     location_index = np.where(haversine(tlons,tlats,latlon1[1],latlon1[0]) == np.min(haversine(tlons,tlats,latlon1[1],latlon1[0])))
@@ -543,42 +866,50 @@
     new_keys = ['T', 'Td', 'rh', 'u', 'v', 'z', 'p']
     sfc_keys = ['sfc_T', 'sfc_Td', 'sfc_rh', 'sfc_u', 'sfc_v', 'sfc_z', 'sfc_p']
     vert_keys = ['vert_T', 'vert_Td', 'vert_rh', 'vert_u', 'vert_v', 'vert_z', 'vert_p']
     
     for vert_key, sfc_key, new_key in zip(vert_keys, sfc_keys, new_keys):
         sb_dict[new_key] = make_sfc_based(vert_loc_idx[vert_key],  sfc_loc_idx[sfc_key],  sfc_index)
     sb_dict['w'] = make_sfc_based(vert_loc_idx['vert_w'],  vert_loc_idx['vert_w'][0],  sfc_index)
-    # if sb_dict['p'][0] < sb_dict['p'][1]:
-    #     sb_dict['p'][0] = sb_dict['p'][0] + 25
     
     # Interpolates data
     dz = 250 
     soundingtop_hght = sb_dict['z'][-1]
     toplvl      = int(soundingtop_hght/dz)*dz
     numlvls     = int(toplvl/dz)
     interp_lvls = np.linspace(0,toplvl,numlvls+1)
     
     keys = ['T', 'Td', 'rh', 'u', 'v', 'z', 'p', 'w']
     units_list = ['degC', 'degC', 'percent', 'kt', 'kt', 'm', 'hPa']
     interp_dict = {}
     zeros_dict  = {}
-    final_profile  = {}
+    clean_data  = {}
     
     for key in keys:
         interp_dict[key] = (interpolate.interp1d(sb_dict['z'], sb_dict[key]))
         zeros_dict[key]  = np.zeros((len(interp_lvls)))
         for zeros_arr in zeros_dict.values():
             zeros_dict[key][0] = sb_dict[key][0]
         for i in range(1,len(zeros_dict[key]),1):
             zeros_dict[key][i] = interp_dict[key](dz*i)
     for i, unit, key in zip(range(0, len(units_list)), units_list, keys):
-        final_profile[key] = zeros_dict[key]*units(unit)
-    final_profile['w'] = zeros_dict['w']/units('sec') 
-    final_profile['zAGL'] = final_profile['z'] + surface_height*units.m
-    clean_data = final_profile 
+        clean_data[key] = zeros_dict[key]*units(unit)
+    clean_data['w'] = zeros_dict['w']/units('sec') 
+    clean_data['zAGL'] = clean_data['z'] + surface_height*units.m
+    clean_data['site_info'] = {
+                'site-id'   : 'no-site-idea',
+                'site-name' : 'no-site-name',
+                'site-lctn' : 'no-site-location',
+                'site-latlon' : [latlon1[0], latlon1[1]],
+                'site-elv'  : surface_height,
+                'source'    : 'Model Reanalysis',
+                'model'     : source,
+                'fcst-hour' : 'F00',
+                'run-time'  : [year1, month1, day1, hour1],
+                'valid-time': [year1, month1, day1, hour1]}
     
     print('- COMPLETE -')
     elapsed_time = time.time() - st
     print('RUNTIME:', time.strftime("%H:%M:%S", time.gmtime(elapsed_time)))
     return clean_data
 
 
@@ -587,49 +918,25 @@
 
 
 
 ##################################################################################################################################################
 #                                                       METPY_SOUNDING() FUNCTION                                                                #
 ##################################################################################################################################################
 
-def metpy_sounding(clean_data):
-    st = time.time()
-    import matplotlib.pyplot as plt
-    import metpy.calc as mpcalc
-    from metpy.plots import add_metpy_logo, SkewT, Hodograph
-    from mpl_toolkits.axes_grid1.inset_locator import inset_axes
-    from metpy.units import units
-    
+def __metpy_sounding(clean_data):
+    st = time.time()   
     
     '''
-        metpy_sounding(clean_data)
-
         this function inputs cleaned profile data through a slightly modified MetPy sounding plot script. 
 
-        PARAMETERS
-        ----------
-        name         dtype    required   example      explanation 
-        clean_data:  dict,      yes,    clean_data    a dict of cleaned profile data acquired from the above functions. 
-
-        RETURNS
-        -------
-        img: MetPy Sounding Plot
-
-        EXAMPLES
-        --------
-        spy.metpy_sounding(clean_sounding)
-
         COPYRIGHT
-        ---------
         Created by Kyle J Gillett (@wxkylegillett) 2023
-
     '''
     
     fig = plt.figure(figsize=(16, 12), edgecolor="#04253a")
-    add_metpy_logo(fig, 80, 80)
     skew = SkewT(fig, rotation=45)
     fig.set_facecolor('#ffffff')        
     skew.ax.set_facecolor('#ffffff')                                                    # set facecolor to white                         
     skew.plot(clean_data['p'], clean_data['T'], 'r', lw=3)                              # plot T
     skew.plot(clean_data['p'], clean_data['Td'], 'g', lw=3)                             # plot Td
     interval = np.logspace(2.113, 3, 30) * units.hPa                                    # Arrange wind barbs for best fit
     idx = mpcalc.resample_nn_1d(clean_data['p'], interval)                              # Resample wind barbs for bes
@@ -639,19 +946,27 @@
     plt.xticks(fontsize=13)                                                             # define x axis tick mark size
     plt.yticks(fontsize=13, ha='left')                                                  # define y axis tick mark size
     plt.tick_params(axis="x",direction="in", pad=-12)                                   # move x ticks in
     plt.tick_params(axis="y",direction="in", pad=-7)                                    # move y ticks in
     plt.xlabel("  ", fontsize=12)                                                       # remove x axis label
     plt.ylabel("  ", fontsize=12)                                                       # remove y axis label
     # ADD A SIMPLE PLOT TITLE
-    if source == 'obs':
-        plt.title(f"{clean_data['station_info'][0]} |  VALID: {month1}/{day1}/{year1} {hour1}Z  |  {clean_data['station_info'][3][0]}, {clean_data['station_info'][3][1]}",loc='left', weight='bold', fontsize=15)
+    if clean_data['site_info']['source'] in ['RAOB', 'IGRA']:
+        plt.title(f"{clean_data['site_info']['site-id']} | VALID: {clean_data['site_info']['valid-time'][1]}/{clean_data['site_info']['valid-time'][2]}/{clean_data['site_info']['valid-time'][0]} {clean_data['site_info']['valid-time'][3]}Z  |  {clean_data['site_info']['site-latlon'][0]}, {clean_data['site_info']['site-latlon'][1]}",loc='left', weight='bold', fontsize=15)
+         
+    elif clean_data['site_info']['source'] == 'BUFKIT':
+        plt.title(f"{clean_data['site_info']['run-time'][3]}Z {clean_data['site_info']['model']} {clean_data['site_info']['fcst-hour']} | VALID: {clean_data['site_info']['valid-time'][1]}/{clean_data['site_info']['valid-time'][2]}/{clean_data['site_info']['valid-time'][0]} {clean_data['site_info']['valid-time'][3]}Z | {clean_data['site_info']['site-id']} ",
+                  loc='left', weight='bold', fontsize=15)
+          
     else:
-        plt.title(f'{source} F00  |  VALID: {month1}/{day1}/{year1} {hour1}Z  |  {latlon1}',loc='left', weight='bold', fontsize=15)
+        plt.title(f"{clean_data['site_info']['run-time'][3]}Z {clean_data['site_info']['model']} {clean_data['site_info']['fcst-hour']} | VALID: {clean_data['site_info']['valid-time'][1]}/{clean_data['site_info']['valid-time'][2]}/{clean_data['site_info']['valid-time'][0]} {clean_data['site_info']['valid-time'][3]}Z | {clean_data['site_info']['site-latlon'][0]}, {clean_data['site_info']['site-latlon'][1]}",
+                  loc='left', weight='bold', fontsize=15)
+    
     plt.title("POWERED BY METPY & SOUNDERPY", fontsize=12, alpha=0.5, weight='bold', color='blue', loc='right')
+   
     # Set some better labels than the default
     skew.ax.set_xlabel(f"Temperature ({clean_data['T'].units:~P})")
     skew.ax.set_ylabel(f"Pressure ({clean_data['p'].units:~P})")
     # Calculate LCL height and plot as black dot. Because `p`'s first value is
     # ~1000 mb and its last value is ~250 mb, the `0` index is selected for
     # `p`, `T`, and `Td` to lift the parcel from the surface. If `p` was inverted,
     # i.e. start from low value, 250 mb, to a high value, 1000 mb, the `-1` index
@@ -733,81 +1048,141 @@
     hodo_plot = h.plot_colormapped(u_hodo, v_hodo, z_hodo, lw=4)  # Plot a line colored by wind speed
     plt.xticks(np.arange(0,0,1))
     plt.yticks(np.arange(0,0,1))
     for i in range(10,120,10):
         h.ax.annotate(str(i),(i,0),xytext=(0,2),textcoords='offset pixels',clip_on=True,fontsize=10,weight='bold',alpha=0.3,zorder=0)
     for i in range(10,120,10):
         h.ax.annotate(str(i),(0,i),xytext=(0,2),textcoords='offset pixels',clip_on=True,fontsize=10,weight='bold',alpha=0.3,zorder=0)
-    # Show the plot
-    plt.show()
     elapsed_time = time.time() - st
     print('RUNTIME:', time.strftime("%H:%M:%S", time.gmtime(elapsed_time)))
+    return plt
+
+
+def metpy_sounding(clean_data, method='show', filename='sounderpy_sounding'):
+    if method == 'show':
+        __metpy_sounding(clean_data).show()
+    elif method == 'save':
+        __metpy_sounding(clean_data).savefig(filename)
     
     
+
     
     
     
     
     
-
-##################################################################################################################################################
-#                                                           GET_DOCS() FUNCTION                                                                  #
 ##################################################################################################################################################
- 
-def get_docs():
-    docs_text = f"""
-## ------------ VERTICAL PROFILE DATA RETRIEVAL TOOL DOCUMENTATION ----------------
-## check out the full documentation here: https://github.com/kylejgillett/sounderpy/blob/main/DOCUMENTATION.md
-## 
-## SounderPy can access and parse data from:
-## > ECMWF CDS ERA5 reanalysis [1940-present] *note: you must set up an account through the CDS to unlock ERA5 data. 
-##    (see: https://cds.climate.copernicus.eu/api-how-to)
-## > UNIDATA THREDDS TDS RAP reanalysis [2005-present]
-## > UNIDATA THREDDS TDS RUC reanalysis [2005-2020]
-## > The University of Wyoming RAOB archive [1973-present, depending on station]
-## > Iowa State University's RAOB archive [1945-present, depending on station]
-##
-##
-## COPYRIGHT
-## ---------
-## Created by Kyle J Gillett (@wxkylegillett) 2023
-##
-## Version: {version} | {version_date}
-## --------------------------------------------------------------------------------
-##
-## TOOLS INCLUDED IN THIS PACKAGE:
-## -------------------------------
-## get_docs(): [function, prints quick documentation for this package]
-##
-## get_model_data(method, domain, latlons, year, month, day, hour): [function, used to access model sounding data] - returns raw_data 
-##
-## get_obs_data(station, year, month, day, hour): [function, used to access RAOB sounding data] - returns clean_data 
-##
-## parse_data(raw_data) [function, used to parse sounding data after using a get_model_data() function] - returns clean_data
-##
-## metpy_sounding(clean_data)  [function, used to metpy's skewt plotting functions to create a quick sounding 
-##                                of the parsed data the original script from MetPy is found here: 
-##                                https://unidata.github.io/MetPy/latest/tutorials/upperair_soundings.html
-## metar_latlon(metar_site) [function, get lat-lon pair for a metar site] - returns list of lat/lon pair
-##
-## raob_latlon(raob_site) [function, get lat-lon pair for a raob site] - returns list of lat/lon pair
-##
-##
-## EXAMPLES:
-##     >>> import sounderpy as spy
-##     >>> raw_data   = spy.get_model_data('rap', [43.45, -84.57], '2014', '06', '16', '21')   
-##     >>> clean_data = spy.parse_data(raw_data)
-##     >>> spy.metpy_sounding(clean_data)
-"""
-    print(docs_text)
+#                                                       METPY_HODOGRAPH() FUNCTION                                                                #
+#################################################################################################################################################
+
+    
+def __metpy_hodograph(clean_data):
+    
+    st = time.time()   
+    '''
+        metpy_hodograph(clean_data)
+
+        this function inputs cleaned profile data through a slightly modified MetPy sounding plot script. 
 
+        COPYRIGHT
+        Created by Kyle J Gillett (@wxkylegillett) 2023
+    '''
+    
+    # Create a hodograph
+    fig = plt.figure(figsize=(16, 12), edgecolor="#04253a")
+    ax = plt.subplot()
+    h = Hodograph(ax, component_range=100)
+    
+    # ADD A SIMPLE PLOT TITLE
+    if clean_data['site_info']['source'] in ['RAOB', 'IGRA']:
+        plt.title(f"{clean_data['site_info']['site-id']} | VALID: {clean_data['site_info']['valid-time'][1]}/{clean_data['site_info']['valid-time'][2]}/{clean_data['site_info']['valid-time'][0]} {clean_data['site_info']['valid-time'][3]}Z  |  {clean_data['site_info']['site-latlon'][0]}, {clean_data['site_info']['site-latlon'][1]}",loc='left', weight='bold', fontsize=15)
+         
+    elif clean_data['site_info']['source'] == 'BUFKIT':
+        plt.title(f"{clean_data['site_info']['run-time'][3]}Z {clean_data['site_info']['model']} {clean_data['site_info']['fcst-hour']} | VALID: {clean_data['site_info']['valid-time'][1]}/{clean_data['site_info']['valid-time'][2]}/{clean_data['site_info']['valid-time'][0]} {clean_data['site_info']['valid-time'][3]}Z | {clean_data['site_info']['site-id']} ",
+                  loc='left', weight='bold', fontsize=15)
+          
+    else:
+        plt.title(f"{clean_data['site_info']['run-time'][3]}Z {clean_data['site_info']['model']} {clean_data['site_info']['fcst-hour']} | VALID: {clean_data['site_info']['valid-time'][1]}/{clean_data['site_info']['valid-time'][2]}/{clean_data['site_info']['valid-time'][0]} {clean_data['site_info']['valid-time'][3]}Z | {clean_data['site_info']['site-latlon'][0]}, {clean_data['site_info']['site-latlon'][1]}",
+                  loc='left', weight='bold', fontsize=15)
     
+    plt.title("POWERED BY METPY & SOUNDERPY", fontsize=12, alpha=0.5, weight='bold', color='blue', loc='right')
+    
+    # determine max height of wind data to plot on hodograph in km (if hodo_layer = 9, 0-9km u and v are plotted)
+    hodo_layer = int(12)
+    # remove nan values from base wind u and v component arrays to find min & max values.
+    u_clean = clean_data['u'].magnitude[np.logical_not(np.isnan(clean_data['u'].magnitude))]
+    v_clean = clean_data['v'].magnitude[np.logical_not(np.isnan(clean_data['v'].magnitude))]
+    # restructure u and v, p, ws and z data arrays based on corrected u and v arrays and hodo_layer depth
+    p_hodo, u_hodo, v_hodo, z_hodo = mpcalc.get_layer(clean_data['p'], clean_data['u'], clean_data['v'], clean_data['z'], depth=hodo_layer*units.km)
+    x_min = u_hodo.min().m
+    y_min = v_hodo.min().m
+    x_max = u_hodo.max().m
+    y_max = v_hodo.max().m
+    # if statements to determine approprate x axis and y axis limits (to change dynamically with the data)
+    if y_max >= 0:
+        y_Maxlimit = (y_max + 15)
+    if y_max < 0:
+        y_Maxlimit = (y_max + 15)
+
+    if x_max >= 0:
+        x_Maxlimit = (x_max + 15)
+    if x_max < 0:
+        x_Maxlimit = (x_max + 15)
+
+    if y_min >= 0:
+        y_Minlimit = (y_min - 40)
+    if y_min < 0:
+        y_Minlimit = (y_min - 40)
+
+    if x_min >= 0:
+        x_Minlimit = (x_min - 40)
+    if x_min < 0:
+        x_Minlimit = (x_min - 40)
+
+    try:
+        h.ax.set_xlim(x_Minlimit, x_Maxlimit)                                  
+        h.ax.set_ylim(y_Minlimit, y_Maxlimit)                             
+    except:
+        pass
+    h.add_grid(increment=20, color='black', linestyle='-', linewidth=1.5, alpha=0.3)   
+    h.add_grid(increment=10, color='silver', linewidth=1, linestyle='--', alpha=0.5) 
+    ax.set_xlim(-65,65)
+    ax.set_ylim(-65,65)
+    fig.set_facecolor('#ffffff')        
+    h.ax.set_facecolor('#ffffff')
+    h.ax.set_facecolor('#ffffff')                                      
+    h.ax.set_box_aspect(1)                          
+    h.ax.set_yticklabels([])
+    h.ax.set_xticklabels([])
+    h.ax.set_xticks([])
+    h.ax.set_yticks([])
+    h.ax.set_xlabel(' ')
+    h.ax.set_ylabel(' ')
+    hodo_plot = h.plot_colormapped(u_hodo, v_hodo, z_hodo, lw=6)  # Plot a line colored by wind speed
+    plt.xticks(np.arange(0,0,1))
+    plt.yticks(np.arange(0,0,1))
+    for i in range(10,120,10):
+        h.ax.annotate(str(i),(i,0),xytext=(0,2),textcoords='offset pixels',clip_on=True,fontsize=10,weight='bold',alpha=0.3,zorder=0)
+    for i in range(10,120,10):
+        h.ax.annotate(str(i),(0,i),xytext=(0,2),textcoords='offset pixels',clip_on=True,fontsize=10,weight='bold',alpha=0.3,zorder=0)
+
+    elapsed_time = time.time() - st
+    print('RUNTIME:', time.strftime("%H:%M:%S", time.gmtime(elapsed_time)))
+    return plt
+
 
+def metpy_hodograph(clean_data, method='show', filename='sounderpy_hodograph'):
+    if method == 'show':
+        __metpy_hodograph(clean_data).show()
+    elif method == 'save':
+        __metpy_hodograph(clean_data).savefig(filename)
     
     
+    
+
 
     
     
 ##################################################################################################################################################
 #                                                      SOUNDERPY HELPER FUCNTIONS                                                                #
 ##################################################################################################################################################
 '''
@@ -818,25 +1193,14 @@
 '''
     
 ####################################################### DATA INTERPOLATION ################################################################# 
 def interp_data(variable, heights, step=100):
     
     '''
         interpolate vertical profile over vertical height array
-        
-        PARAMETERS
-        ----------
-        name        dtype    required    explanation 
-        variable:   array    yes         the data to be interpolated. Must be same length as height array
-        heights:    array    yes         heights corresponding to the vertical profile used to interpolate
-        step:       int      no          resolution of interpolation. Default is 100 (recommended value is 100)
-        
-        RETURNS
-        -------
-        varinterp:  array,  array of interpolated data 
     '''
     
     try:
         variable.units
         variable = variable.m
     except:
         variable = variable
@@ -856,23 +1220,14 @@
     
 ########################################################## FIND NEAREST ####################################################################### 
 def find_nearest(array, value):
     
     '''
         search through an array to find the index of the value nearest to a given value
         
-        PARAMETERS
-        ----------
-        name         dtype                        required    explanation 
-        array        array of ints or floats      yes         the array of data search through to 'find the nearest'
-        value        int or float (same as array) yes         the value used to campare against the array of data
-        
-        RETURNS
-        -------
-        nearest_idx:  int,  index of the data array that corresponds with the nearest value to the given value. 
     '''
     
     array = np.asarray(array)
     nearest_idx = (np.abs(array - value)).argmin()
     return nearest_idx
 
     
@@ -881,24 +1236,16 @@
 ##################################################### MAKE SURFACED BASED #################################################################### 
 
 def get_sfc_index(height_arr):
     
     """
         This function takes an array of height values and finds the index before the first positive value
 
-        PARAMETERS
-        ----------
-        name         dtype         required     explanation 
-        height_arr   array         yes          array of height values
-        RETURNS
-        -------
-        index:       int     indicating the index just before the first positive height value. If -1 is returned,
-               a positive index could not be found.
-    
     """
+    
     i = 0
     # Search the array for the sfc index
     while i < len(height_arr):
         if height_arr[i] >= 0:
             return i
         else:
             i += 1
@@ -910,25 +1257,14 @@
 
 def make_sfc_based(arr, sfc_val, sfc_index):
     
     """
         takes an array and a valid index in that array, then returns a copy of the
         array beginning at the provided index i.e., chops off below-ground values
 
-        PARAMETERS
-        ----------
-        name       dtype         required     explanation 
-        arr        array         yes          the array to manipulate
-        sfc_val    int or float  yes          the value that corresponds to the true surface value
-        sfc_index  int           yes          index indicating where the true sfc is (where copying occurs) (found via get_sfc_index())
-
-        RETURNS
-        -------
-        mod_arr:   array   array of values from arr[index:len(arr)]
-    
     """
 
     # Initialize an empty numpy array as the modified array
     mod_arr = np.empty(len(arr) - sfc_index)
     # Insert the sfc and higher values into the modified array
     i = 0
     while i < len(mod_arr):
@@ -943,27 +1279,17 @@
     
 def make_sfc_based_3D(arr, sfc_arr):
     
     '''
         takes a 3D array of mandatory level data and a 2D array of surface data, 
         appends the surface data onto the mandatory level array, and returns a single array
         of both surface and mandatory level data
-
-
-        PARAMETERS
-        ----------
-        name       dtype         required     explanation 
-        arr        3D array      yes          the 3D vertical profile(s) array to manipulate
-        sfc_arr    2D array      yes          the true surface values to be added to the vertical profile(s)
-
-        RETURNS
-        -------
-        mod_arr:   array   array of values from arr[index:len(arr)]
-    
+        
     '''
+    
     mod_arr = np.zeros((np.shape(arr)[0]+1,np.shape(arr)[1],np.shape(arr)[2]))
     for j in range(np.shape(arr)[1]):
         for k in range(np.shape(arr)[2]):
             mod_arr[0,j,k] = sfc_arr[j,k]
             mod_arr[1:,j,k] = arr[:,j,k]
     return mod_arr
 
@@ -975,22 +1301,14 @@
 
 def metar_latlon(metar_site):
     
     '''
         takes a METAR site id such as 'KMBS', searches over 9000 station IDs  and returns
         a list including the lat/lon for the METAR site
 
-        PARAMETERS
-        ----------
-        name        dtype    required   example   explanation 
-        metar_site  str      yes        'KMBS'    4 digit METAR site id
-
-        RETURNS
-        -------
-        latlon:     list      lat lon pair for requested METAR site in a list
     '''
     
     def dms2dd(degrees, minutes, direction):
         dd = float(degrees) + float(minutes) / 60
         if direction == "S" or direction == "W":
             dd *= -1
         return dd
@@ -1012,42 +1330,195 @@
 
             if icao:
                 stations[icao] = {"name": station, "lat": lat, "lon": lon, "altitude": altitude, "country": country}
     try:
         latlon = [np.round(stations.get(metar_site)['lat'],2), np.round(stations.get(metar_site)['lon'],2)]
         return latlon
     except:
-        print('[!] ERROR [!]\nMETAR site lat/lon not available')
+        sys.exit("NO METAR SITE FOUND FOR THAT ID -- Make sure you entered a valid METAR ID -- Make sure you entered the METAR ID as a string, ex: 'KMOP'")
         pass
+
+    
+#################################################### FIND BUFKIT SITE LATLON ##################################################################  
     
+def bufkit_latlon(bufkit_site):
     
+    '''
+        takes a BUFKIT site id such as 'KMOP', searches over 1200 station IDs and returns
+        a list including the lat/lon for the BUFKIT site
+
+    '''
+    BUFKIT_STATIONS = pd.read_csv(f'https://raw.githubusercontent.com/kylejgillett/sounderpy/main/txt_files/BUFKIT-STATIONS-MASTER.csv', skiprows=7, skipinitialspace = True)
+    try:
+        station = BUFKIT_STATIONS['ID'][np.where(BUFKIT_STATIONS['ID'].str.contains(bufkit_site, na=False, case=True))[0]].values[0]
+
+        lat = (BUFKIT_STATIONS[BUFKIT_STATIONS['ID']==station]['LAT'].values[0])
+        lon = (BUFKIT_STATIONS[BUFKIT_STATIONS['ID']==station]['LON'].values[0])
+        return [lat, lon]
     
+    except:
+        sys.exit("NO BUFKIT SITE FOUND FOR THAT ID -- Make sure you entered a valid BUFKIT ID -- Make sure you entered the BUFKIT ID as a string, ex: 'KMOP'")
+        pass
     
     
 #################################################### FIND RAOB SITE LATLON ##################################################################    
     
 def raob_latlon(raob_site):
+    
+    '''
+        takes a RAOB site id such as 'DTX', searches over 9000 station IDs  and returns
+        a list including the lat/lon for the RAOB site
 
+    '''
+    
     def dms2dd(degrees, direction):
         dd = float(degrees)
         if direction == "S" or direction == "W":
             dd *= -1
         return dd
-    RAOB_STATIONS = pd.read_csv(f'https://raw.githubusercontent.com/kylejgillett/sounderpy/main/RAOB-STATIONS.txt', skiprows=7, skipinitialspace = True)
+    RAOB_STATIONS = pd.read_csv(f'https://raw.githubusercontent.com/kylejgillett/sounderpy/main/txt_files/RAOB-STATIONS.txt', skiprows=7, skipinitialspace = True)
     try:
         station = RAOB_STATIONS['ICAO'][np.where(RAOB_STATIONS['ICAO'].str.contains(raob_site, na=False, case=True))[0]].values[0]
 
         lat = dms2dd(RAOB_STATIONS[RAOB_STATIONS['ICAO']==station]['LAT'].values[0], RAOB_STATIONS[RAOB_STATIONS['ICAO']==station]['A'].values[0])
         lon = dms2dd(RAOB_STATIONS[RAOB_STATIONS['ICAO']==station]['LON'].values[0], RAOB_STATIONS[RAOB_STATIONS['ICAO']==station]['B'].values[0])
         return [lat, lon]
     
     except:
-        print("[!] ERROR [!]\n[!] NO RAOB SITE FOUND FOR THAT ID[!]\n > Make sure you entered a valid RAOB ID\n > Make sure you entered the RAOB ID as a string, ex: 'DTX'")
+        sys.exit("NO RAOB SITE FOUND FOR THAT ID -- Make sure you entered a valid RAOB ID -- Make sure you entered the RAOB ID as a string, ex: 'DTX'")
+        pass
+    
+
+    
+    
+    
+    
+#################################################### FIND IGRA SITE LATLON ##################################################################  
+
+def igra_latlon(igra_site):
+    
+    '''
+        takes a IGRA2 site id such as 'GMM00010393', searches nearly 3000 station IDs  and returns
+        a list including the lat/lon for the IGRA2 site
+    '''
+    
+    
+    IGRA_STATIONS = pd.read_csv(f'https://raw.githubusercontent.com/kylejgillett/sounderpy/main/txt_files/IGRA-STATIONS.txt', skiprows=7, skipinitialspace = True)
+    try:
+        station = IGRA_STATIONS['ID'][np.where(IGRA_STATIONS['ID'].str.contains(igra_site, na=False, case=True))[0]].values[0]
+
+        lat = np.round(IGRA_STATIONS[IGRA_STATIONS['ID']==station]['LAT'].values[0], 2)
+        lon = np.round(IGRA_STATIONS[IGRA_STATIONS['ID']==station]['LON'].values[0], 2)
+        return [lat, lon]
+    
+    except:
+        sys.exit("NO IGRAv2 SITE FOUND FOR THAT ID -- Make sure you entered a valid IGRAv2 ID -- Make sure you entered the RAOB ID as a string, ex: 'GMM00010393'")
+        pass
+
+    
+    
+    
+    
+    
+######################################################### BUOY SITE LATLON ####################################################################     
+def buoy_latlon(buoy_site):
+    
+    '''
+        takes a BUOY/CMAN site id such as '41001', searches through a number of station IDs and returns
+        a list including the lat/lon for the BUOY/CMAN  site
+
+    '''
+
+    def dms2dd(degrees, direction):
+        dd = float(degrees)
+        if direction == "S" or direction == "W":
+            dd *= -1
+        return dd
+    BUOY_STATIONS = pd.read_csv('https://raw.githubusercontent.com/kylejgillett/sounderpy/main/txt_files/BUOY-STATIONS.txt', skiprows=7, skipinitialspace = True)
+    try:
+        station = BUOY_STATIONS['ID'][np.where(BUOY_STATIONS['ID'].str.contains(buoy_site, na=False, case=True))[0]].values[0]
+
+        lat = dms2dd(BUOY_STATIONS[BUOY_STATIONS['ID']==station]['LAT'].values[0], BUOY_STATIONS[BUOY_STATIONS['ID']==station]['A'].values[0])
+        lon = dms2dd(BUOY_STATIONS[BUOY_STATIONS['ID']==station]['LON'].values[0], BUOY_STATIONS[BUOY_STATIONS['ID']==station]['B'].values[0])
+        return [lat, lon]
+    
+    except:
+        sys.exit("NO BUOY SITE FOUND FOR THAT ID -- Make sure you entered a valid BUOY ID -- Make sure you entered the BUOY ID as a string, ex: '41001'")
         pass
     
+
+    
+    
+    
+    
+########################################################### TO CM1 FILE ####################################################################     
+
+def to_cm1(clean_data, filename=None):
+    '''
+    function, creates CM1 input sounding file for CM1 integration
+
+    COPYRIGHT
+    Created by Kyle J Gillett (@wxkylegillett) 2023 & Kelton Halbert 2021
+    
+    Derived from Kelton Halbert / Leigh Orf via github: 
+    
+    https://github.com/leighorf/LOFS-read/blob/master/bin/sndmod
+    
+    '''
+    
+    
+    if filename == None:
+        filename = f'sounderpy_data'
+    else:
+        filename = filename
+    outfile = open(filename, 'w')
+    num_lines = len(list(clean_data.items())[0][1])
+    delimiter=''
+    
+    clean_data['theta'] = mpcalc.potential_temperature(clean_data['p'], clean_data['T'])
+    clean_data['relhm'] = mpcalc.relative_humidity_from_dewpoint(clean_data['T'], clean_data['Td'])
+    clean_data['mixrt'] = mpcalc.mixing_ratio_from_relative_humidity(clean_data['p'], clean_data['T'], clean_data['relhm'])
+    
+    for idx in range(num_lines):
+            line_str = ""
+            line_str += "%12s" % str(format(np.around(clean_data["z"][idx].m, 6), "0.6f")) + delimiter + str("\t")
+            line_str += "%12s" % str(format(np.around(clean_data["theta"][idx].m, 6), "0.6f")) + delimiter + str("\t")
+            line_str += "%12s" % str(format(np.around(clean_data["mixrt"][idx].m, 6), "0.6f")) + delimiter + str("\t")
+            line_str += "%12s" % str(format(np.around(clean_data["u"][idx].m, 6), "0.6f")) + delimiter + str("\t")
+            line_str += "%12s" % str(format(np.around(clean_data["v"][idx].m, 6), "0.6f")) + str("\n")
+            outfile.write(line_str)
+        
+    outfile.close()
+
+    
+
+    
+    
+    
+    
+########################################################### TO CSV FILE ####################################################################      
+def to_csv(clean_data, filename=None):
+    '''
+    function, creates CSV file of sounding data
+    
+    COPYRIGHT
+    Created by Kyle J Gillett (@wxkylegillett) 2023
+    '''
+    
+    if filename == None:
+        filename = f'sounderpy_data.csv'
+    else:
+        filename = filename
+    no_units = {}
+    for key in ['p', 'z', 'T', 'Td', 'u', 'v']:
+            no_units[key] = clean_data[key].m
+    with open(filename, "w") as csvfile:
+        writer = csv.writer(csvfile)
+        writer.writerow(no_units.keys())
+        writer.writerows(zip(*no_units.values()))
```

