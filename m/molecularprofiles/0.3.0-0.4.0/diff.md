# Comparing `tmp/molecularprofiles-0.3.0.tar.gz` & `tmp/molecularprofiles-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "molecularprofiles-0.3.0.tar", last modified: Wed Apr 19 08:12:54 2023, max compression
+gzip compressed data, was "molecularprofiles-0.4.0.tar", last modified: Fri Aug  4 15:02:02 2023, max compression
```

## Comparing `molecularprofiles-0.3.0.tar` & `molecularprofiles-0.4.0.tar`

### file list

```diff
@@ -1,24 +1,23 @@
-drwxr-xr-x   0 mdalchen   (501) staff       (20)        0 2023-04-19 08:12:54.383834 molecularprofiles-0.3.0/
--rw-r--r--   0 mdalchen   (501) staff       (20)     1474 2022-11-22 15:24:35.000000 molecularprofiles-0.3.0/LICENSE
--rw-r--r--   0 mdalchen   (501) staff       (20)     2654 2023-04-19 08:12:54.383550 molecularprofiles-0.3.0/PKG-INFO
--rw-r--r--   0 mdalchen   (501) staff       (20)      450 2023-02-01 16:41:16.000000 molecularprofiles-0.3.0/README.md
--rw-r--r--   0 mdalchen   (501) staff       (20)     1656 2023-04-19 08:01:37.000000 molecularprofiles-0.3.0/pyproject.toml
--rw-r--r--   0 mdalchen   (501) staff       (20)       38 2023-04-19 08:12:54.383919 molecularprofiles-0.3.0/setup.cfg
-drwxr-xr-x   0 mdalchen   (501) staff       (20)        0 2023-04-19 08:12:54.371595 molecularprofiles-0.3.0/src/
-drwxr-xr-x   0 mdalchen   (501) staff       (20)        0 2023-04-19 08:12:54.373057 molecularprofiles-0.3.0/src/molecularprofiles/
--rwxr-xr-x   0 mdalchen   (501) staff       (20)      195 2023-04-19 08:02:09.000000 molecularprofiles-0.3.0/src/molecularprofiles/__init__.py
--rwxr-xr-x   0 mdalchen   (501) staff       (20)    19996 2023-04-19 08:02:40.000000 molecularprofiles-0.3.0/src/molecularprofiles/molecularprofiles.py
-drwxr-xr-x   0 mdalchen   (501) staff       (20)        0 2023-04-19 08:12:54.382873 molecularprofiles-0.3.0/src/molecularprofiles/utils/
--rw-r--r--   0 mdalchen   (501) staff       (20)       27 2023-02-03 15:27:32.000000 molecularprofiles-0.3.0/src/molecularprofiles/utils/__init__.py
--rwxr-xr-x   0 mdalchen   (501) staff       (20)     1257 2023-04-19 08:01:37.000000 molecularprofiles-0.3.0/src/molecularprofiles/utils/constants.py
--rwxr-xr-x   0 mdalchen   (501) staff       (20)    16618 2023-04-19 08:02:40.000000 molecularprofiles-0.3.0/src/molecularprofiles/utils/grib_utils.py
--rwxr-xr-x   0 mdalchen   (501) staff       (20)    10506 2023-04-19 08:01:37.000000 molecularprofiles-0.3.0/src/molecularprofiles/utils/humidity.py
--rw-r--r--   0 mdalchen   (501) staff       (20)      327 2023-02-03 15:27:32.000000 molecularprofiles-0.3.0/src/molecularprofiles/utils/mdps_log.conf
--rwxr-xr-x   0 mdalchen   (501) staff       (20)    10235 2023-04-19 08:01:37.000000 molecularprofiles-0.3.0/src/molecularprofiles/utils/observatory.py
--rw-r--r--   0 mdalchen   (501) staff       (20)    14698 2023-04-19 08:02:40.000000 molecularprofiles-0.3.0/src/molecularprofiles/utils/rayleigh.py
-drwxr-xr-x   0 mdalchen   (501) staff       (20)        0 2023-04-19 08:12:54.375210 molecularprofiles-0.3.0/src/molecularprofiles.egg-info/
--rw-r--r--   0 mdalchen   (501) staff       (20)     2654 2023-04-19 08:12:54.000000 molecularprofiles-0.3.0/src/molecularprofiles.egg-info/PKG-INFO
--rw-r--r--   0 mdalchen   (501) staff       (20)      621 2023-04-19 08:12:54.000000 molecularprofiles-0.3.0/src/molecularprofiles.egg-info/SOURCES.txt
--rw-r--r--   0 mdalchen   (501) staff       (20)        1 2023-04-19 08:12:54.000000 molecularprofiles-0.3.0/src/molecularprofiles.egg-info/dependency_links.txt
--rw-r--r--   0 mdalchen   (501) staff       (20)      205 2023-04-19 08:12:54.000000 molecularprofiles-0.3.0/src/molecularprofiles.egg-info/requires.txt
--rw-r--r--   0 mdalchen   (501) staff       (20)       18 2023-04-19 08:12:54.000000 molecularprofiles-0.3.0/src/molecularprofiles.egg-info/top_level.txt
+drwxr-xr-x   0 mdalchen   (501) staff       (20)        0 2023-08-04 15:02:02.306022 molecularprofiles-0.4.0/
+-rw-r--r--   0 mdalchen   (501) staff       (20)     1474 2022-11-22 15:24:35.000000 molecularprofiles-0.4.0/LICENSE
+-rw-r--r--   0 mdalchen   (501) staff       (20)     2654 2023-08-04 15:02:02.305789 molecularprofiles-0.4.0/PKG-INFO
+-rw-r--r--   0 mdalchen   (501) staff       (20)      450 2023-02-01 16:41:16.000000 molecularprofiles-0.4.0/README.md
+-rw-r--r--   0 mdalchen   (501) staff       (20)     1638 2023-07-21 08:41:06.000000 molecularprofiles-0.4.0/pyproject.toml
+-rw-r--r--   0 mdalchen   (501) staff       (20)       38 2023-08-04 15:02:02.306097 molecularprofiles-0.4.0/setup.cfg
+drwxr-xr-x   0 mdalchen   (501) staff       (20)        0 2023-08-04 15:02:02.298661 molecularprofiles-0.4.0/src/
+drwxr-xr-x   0 mdalchen   (501) staff       (20)        0 2023-08-04 15:02:02.300267 molecularprofiles-0.4.0/src/molecularprofiles/
+-rwxr-xr-x   0 mdalchen   (501) staff       (20)      195 2023-07-31 16:15:37.000000 molecularprofiles-0.4.0/src/molecularprofiles/__init__.py
+-rwxr-xr-x   0 mdalchen   (501) staff       (20)    15793 2023-07-21 11:49:42.000000 molecularprofiles-0.4.0/src/molecularprofiles/molecularprofiles.py
+drwxr-xr-x   0 mdalchen   (501) staff       (20)        0 2023-08-04 15:02:02.305204 molecularprofiles-0.4.0/src/molecularprofiles/utils/
+-rw-r--r--   0 mdalchen   (501) staff       (20)       27 2023-02-03 15:27:32.000000 molecularprofiles-0.4.0/src/molecularprofiles/utils/__init__.py
+-rwxr-xr-x   0 mdalchen   (501) staff       (20)     1257 2023-04-19 08:01:37.000000 molecularprofiles-0.4.0/src/molecularprofiles/utils/constants.py
+-rwxr-xr-x   0 mdalchen   (501) staff       (20)     9107 2023-07-31 16:22:51.000000 molecularprofiles-0.4.0/src/molecularprofiles/utils/grib_utils.py
+-rwxr-xr-x   0 mdalchen   (501) staff       (20)    10490 2023-07-21 08:41:06.000000 molecularprofiles-0.4.0/src/molecularprofiles/utils/humidity.py
+-rw-r--r--   0 mdalchen   (501) staff       (20)      327 2023-02-03 15:27:32.000000 molecularprofiles-0.4.0/src/molecularprofiles/utils/mdps_log.conf
+-rw-r--r--   0 mdalchen   (501) staff       (20)    14694 2023-07-21 08:41:06.000000 molecularprofiles-0.4.0/src/molecularprofiles/utils/rayleigh.py
+drwxr-xr-x   0 mdalchen   (501) staff       (20)        0 2023-08-04 15:02:02.302035 molecularprofiles-0.4.0/src/molecularprofiles.egg-info/
+-rw-r--r--   0 mdalchen   (501) staff       (20)     2654 2023-08-04 15:02:02.000000 molecularprofiles-0.4.0/src/molecularprofiles.egg-info/PKG-INFO
+-rw-r--r--   0 mdalchen   (501) staff       (20)      578 2023-08-04 15:02:02.000000 molecularprofiles-0.4.0/src/molecularprofiles.egg-info/SOURCES.txt
+-rw-r--r--   0 mdalchen   (501) staff       (20)        1 2023-08-04 15:02:02.000000 molecularprofiles-0.4.0/src/molecularprofiles.egg-info/dependency_links.txt
+-rw-r--r--   0 mdalchen   (501) staff       (20)      193 2023-08-04 15:02:02.000000 molecularprofiles-0.4.0/src/molecularprofiles.egg-info/requires.txt
+-rw-r--r--   0 mdalchen   (501) staff       (20)       18 2023-08-04 15:02:02.000000 molecularprofiles-0.4.0/src/molecularprofiles.egg-info/top_level.txt
```

### Comparing `molecularprofiles-0.3.0/LICENSE` & `molecularprofiles-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `molecularprofiles-0.3.0/PKG-INFO` & `molecularprofiles-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molecularprofiles
-Version: 0.3.0
+Version: 0.4.0
 Summary: Meteorological data analysis suite
 Author-email: Pere Munar Adrover <pere.munar@uab.cat>, Markus Gaug <markus.gaug@uab.cat>, Scott Griffiths <sgriffiths@ifae.es>, Georgios Voutsinas <georgios.voutsinas@unige.ch>, Mykhailo Dalchenko <mykhailo.dalchenko@unige.ch>
 License: Copyright (c) 2020, Molecularprofiles Project
         
         Redistribution and use in source and binary forms, with or withoutmodification, are permitted provided that the following conditions are met:
         
         1. Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
```

### Comparing `molecularprofiles-0.3.0/pyproject.toml` & `molecularprofiles-0.4.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 requires-python = ">=3.8"
 
 dependencies = [
     "numpy",
     "scipy",
     "astropy",
     "pygrib",
-    "statsmodels"
 ]
 
 [project.urls]
 Home = "https://gitlab.cta-observatory.org/cta-array-elements/ccf/mdps"
 
 [tool.setuptools]
 include-package-data = true
```

### Comparing `molecularprofiles-0.3.0/src/molecularprofiles/molecularprofiles.py` & `molecularprofiles-0.4.0/src/molecularprofiles/molecularprofiles.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,17 +7,18 @@
 Further developed and mainted by
 Mykhailo Dalchenko (mykhailo.dalchenko@unige.ch) and
 Georgios Voutsinas (georgios.voutsinas@unige.ch)
 """
 
 import os
 import logging
+import json
 
 import astropy.units as u
-from astropy.table import Table
+from astropy.table import Table, vstack
 import numpy as np
 from scipy.interpolate import interp1d
 
 from molecularprofiles.utils.grib_utils import get_grib_file_data, extend_grib_data
 from molecularprofiles.utils.constants import (
     DENSITY_SCALE_HEIGHT,
     N0_AIR,
@@ -54,27 +55,22 @@
     write_corsika:              prints the data into a txt file which format is compliant with the input card
                                 for the CORSIKA air shower simulation software
     create_mdp:                 creates an altitude profile of the molecular number density
     rayleigh_extinction:        creates a file, in format to be directly fed to simtel simulation, with the
                                 extinction per altitude bin for wavelengths from 200 to 1000 nm
     """
 
-    def __init__(self, data_file, data_server="server", observatory="north"):
+    def __init__(self, data_file):
         """
         Constructor
 
         :param data_file: txt file containing the data (string)
-        :param data_server: label to be put in some of the output plots (string)
-        :param observatory: valid options are: "north", "south", "other"
-
         """
 
         self.data_file = data_file
-        self.data_server = data_server
-        self.observatory = observatory
 
     # =============================================================================================================
     # Private functions
     # =============================================================================================================
     def _interpolate_cubic(self, x_param, y_param, new_x_param):
         func = interp1d(x_param, y_param, kind="cubic", fill_value="extrapolate")
         return func(new_x_param)
@@ -195,21 +191,22 @@
         rayleigh = Rayleigh(wavelength, C, P, T, RH)
         return rayleigh.refractive_index
 
     # =======================================================================================================
     # printing functions:
     # =======================================================================================================
 
-    def write_corsika(self, outfile, co2_concentration):
+    def write_corsika(self, outfile, co2_concentration, upper_atmosphere=None):
         """
         Write an output file in the style of a CORSIKA atmospheric configuration file:
 
         alt (km)     rho (g/cm^3)   thick (g/cm^2)   (n-1)
         """
-        height = np.arange(0.0, 27000.0, 1000) * u.m
+
+        height = np.arange(0.0, 46000.0, 1000) * u.m
         temperature = (
             self._interpolate_cubic(
                 self.stat_description["avg"]["Altitude"],
                 self.stat_description["avg"]["Temperature"],
                 height,
             )
             * self.stat_description["avg"]["Temperature"].unit
@@ -246,173 +243,65 @@
         rel_refractive_index = (
             self._refractive_index(
                 pressure, temperature, relative_humidity, 350.0 * u.nm, co2_concentration
             )
             - 1.0
         )
 
-        with open(outfile, "w") as f:
-
-            f.write("# Atmospheric Model ECMWF year/month/day   hour h\n")  # .format(**datedict))
-            f.write(
-                "#Col. #1          #2           #3            #4        [ #5 ]        [ #6 ]       [ # 7 ]\n"
-            )
-            f.write(
-                "# Alt [km]    rho [g/cm^3] thick [g/cm^2]    n-1        T [k]       p [mbar]      pw / p\n"
-            )
-
-            for i in np.arange(len(height)):
-
-                outdict = {
-                    "height": height[i].to_value(u.km),
-                    "rho": density[i].to_value(u.g / u.cm**3),
-                    "thick": thickness[i].to_value(u.g / u.cm**2),
-                    "nm1": rel_refractive_index[i],
-                    "T": temperature[i].to_value(u.K),
-                    "p": pressure[i].to_value(u.mbar),
-                    "pw/p": rel_water_vapor_pressure[i],
-                }
-                f.write(
-                    "  {height:7.3f}     {rho:5.5E}  {thick:5.5E}  {nm1:5.5E}  {T:5.5E}  {p:5.5E}  {pw/p:5.5E}\n".format(
-                        **outdict
-                    )
-                )
-
-            # concatenate the dummy values of MagicWinter starting from 50.0 km
-            f.write(
-                "   27.000     2.96567e-05  1.96754e+01  6.84513e-06  223.70  1.90428e+01  0.00000e+00\n"
-            )
-
-            f.write(
-                "   28.000     2.52913e-05  1.69341e+01  5.83752e-06  225.69  1.63842e+01  0.00000e+00\n"
-            )
-
-            f.write(
-                "   29.000     2.15935e-05  1.45949e+01  4.98403e-06  227.75  1.41164e+01  0.00000e+00\n"
-            )
-
-            f.write(
-                "   30.000     1.84554e-05  1.25967e+01  4.25972e-06  229.92  1.21798e+01  0.00000e+00\n"
-            )
-
-            f.write(
-                "   32.000     1.35171e-05  9.42594e+00  3.11990e-06  234.75  9.10824e+00  0.00000e+00\n"
-            )
-
-            f.write(
-                "   34.000     9.93769e-06  7.09977e+00  2.29374e-06  240.36  6.85638e+00  0.00000e+00\n"
-            )
-
-            f.write(
-                "   36.000     7.35111e-06  5.38483e+00  1.69672e-06  246.30  5.19717e+00  0.00000e+00\n"
-            )
-
-            f.write(
-                "   38.000     5.47808e-06  4.11190e+00  1.26441e-06  252.24  3.96630e+00  0.00000e+00\n"
-            )
-
-            f.write(
-                "   40.000     4.11643e-06  3.15961e+00  9.50121e-07  257.79  3.04599e+00  0.00000e+00\n"
-            )
-
-            f.write(
-                "   42.000     3.12126e-06  2.44097e+00  7.20424e-07  262.51  2.35189e+00  0.00000e+00\n"
-            )
-
-            f.write(
-                "   44.000     2.38908e-06  1.89362e+00  5.51429e-07  265.91  1.82354e+00  0.00000e+00\n"
-            )
-
-            f.write(
-                "   46.000     1.84598e-06  1.47276e+00  4.26075e-07  267.52  1.41753e+00  0.00000e+00\n"
-            )
+        corsika_input_table = Table()
+        tables = []
 
-            f.write(
-                "   48.000     1.43779e-06  1.14626e+00  3.31858e-07  267.20  1.10275e+00  0.00000e+00\n"
-            )
-
-            f.write(
-                "   50.000     1.09738e-06  8.72656e-01   2.53289e-07   266.34   8.38955e-01  0.00000e+00\n"
-            )
-            f.write(
-                "   55.000     5.99974e-07  4.61036e-01   1.38481e-07   257.19   4.42930e-01  0.00000e+00\n"
-            )
-            f.write(
-                "   60.000     3.25544e-07  2.36175e-01   7.51395e-08   242.81   2.26896e-01  0.00000e+00\n"
-            )
-            f.write(
-                "   65.000     1.70152e-07  1.15918e-01   3.92732e-08   227.93   1.11324e-01  0.00000e+00\n"
-            )
-            f.write(
-                "   70.000     8.43368e-08  5.45084e-02   1.94660e-08   215.90   5.22651e-02  0.00000e+00\n"
-            )
-            f.write(
-                "   75.000     3.95973e-08  2.48012e-02   9.13953e-09   208.66   2.37169e-02  0.00000e+00\n"
-            )
-            f.write(
-                "   80.000     1.79635e-08  1.10899e-02   4.14618e-09   205.11   1.05760e-02  0.00000e+00\n"
-            )
-            f.write(
-                "   85.000     8.03691e-09  4.91583e-03   1.85502e-09   202.12   4.66284e-03  0.00000e+00\n"
-            )
-            f.write(
-                "   90.000     3.59602e-09  2.15599e-03   8.30003e-10   196.26   2.02583e-03  0.00000e+00\n"
-            )
-            f.write(
-                "   95.000     1.59871e-09  9.21029e-04   3.69000e-10   187.55   8.60656e-04  0.00000e+00\n"
-            )
-            f.write(
-                "  100.000     6.73608e-10  3.82814e-04   1.55477e-10   185.38   3.58448e-04  0.00000e+00\n"
-            )
-            f.write(
-                "  105.000     2.69097e-10  1.61973e-04   6.21108e-11   197.19   1.52311e-04  0.00000e+00\n"
-            )
-            f.write(
-                "  110.000     1.09021e-10  7.37110e-05   2.51634e-11   224.14   7.01416e-05  0.00000e+00\n"
-            )
-            f.write(
-                "  115.000     4.71300e-11  3.70559e-05   1.08782e-11   268.51   3.63251e-05  0.00000e+00\n"
-            )
-            f.write(
-                "  120.000     2.23479e-11  2.05900e-05   5.15817e-12   333.43   2.13890e-05  0.00000e+00\n"
-            )
+        for i in np.arange(len(height)):
+            outdict = {
+                "height": height[i].to(u.km),
+                "rho": density[i].to(u.g / u.cm**3),
+                "thick": thickness[i].decompose().to(u.g / u.cm**2),
+                "nm1": rel_refractive_index[i],
+                "T": temperature[i],
+                "p": pressure[i],
+                "pw/p": rel_water_vapor_pressure[i],
+            }
+            tables.append(outdict)
+        # Merge ECMWF profile with upper atmospheric profile
+        if upper_atmosphere:
+            upper_atmosphere_table = Table.read(upper_atmosphere, format="ascii.ecsv")
+            tables.append(upper_atmosphere_table)
+        corsika_input_table = vstack(tables)
+        corsika_input_table.write(outfile, overwrite=True)
 
     def create_mdp(self, mdp_file):
         """
         Write an output file with the molecular number density per height
         """
 
         heights = (
             np.arange(0.0, 27000.0, 1000) * u.m
         )  # FIXME: The hardcoded value 27 reflects the current ceiling of GDAS data (26km a.s.l.). Shouldn't be hardcoded and in general the binning and limits should be considered.
-        with open(mdp_file, "w") as f:
-
-            number_density = (
-                self._interpolate_cubic(
-                    self.stat_description["avg"]["Altitude"],
-                    self.stat_description["avg"]["Density"],
-                    heights,
-                )
-                * self.stat_description["avg"]["Density"].unit
-            )
-            for i, height in enumerate(heights):
-                file_line = [str(height), "\t", str(number_density[i]), "\n"]
-                f.writelines(file_line)
+        number_density = (
+            self._interpolate_cubic(
+                self.stat_description["avg"]["Altitude"],
+                self.stat_description["avg"]["Density"],
+                heights,
+            )
+            * self.stat_description["avg"]["Density"].unit
+        )
+        t = Table([heights, number_density], names=["height", "number density"])
+        t.write(mdp_file, overwrite=True)
 
     def rayleigh_extinction(self, rayleigh_extinction_file, co2_concentration):
         """
         Calculates the integral optical depth due to Rayleigh scattering
         per altitude bins as a function of wavelength.
         The optical depth (AOD) for an altitude h over the observatory will be given by
         the integral of the monochromatic volume coefficient beta, with integration limits
         h_obs up to h.
 
-        returns:
+        Returns:
         --------
-            File with integral optical depth per height bin per wavelength bin. The format is the same with MODTRAN files.
+            Ecsv file with integral optical depth per height bin per wavelength bin. The data model is the same with MODTRAN files.
         """
 
         # For now we work for La Palma site. We will most probably have to find an average
         # altitude for each site. h_obs should become an attribute of observatory class.
         height_obs = 2158
         height = (
             np.array(
@@ -477,20 +366,32 @@
                 bin_centers,
             )
             * self.stat_description["avg"]["Pressure"].unit
         )
         wavelength_range = np.arange(200, 1001, 1) * u.nm
 
         # Here is a schoolkid's, homemade numerical integration. Though it gives reasonable results.
-        with open(rayleigh_extinction_file, "w") as f:
-            for wavelength in wavelength_range:
-                aod = 0
-                file_line = [str(wavelength.to(u.nm)).split(" ")[0], "\t"]
-                for P, T, RH, dh in zip(pressure, temperature, relative_humidity, bin_widths):
-                    rayleigh = Rayleigh(wavelength, co2_concentration, P, T, RH)
-                    beta = rayleigh.beta
-                    aod += dh * beta
-                    file_line += [f"{aod:.6f}", "\t"]
-                file_line += ["\n"]
-                f.writelines(file_line)
-
+        rayleigh_extinction_table = Table()
+        tables = []
+        for wavelength in wavelength_range:
+            aod = 0
+            l = []
+            optical_depth = []
+            l.append(wavelength)
+            file_line = []
+            file_line.append(wavelength.to_value())
+            for P, T, RH, dh in zip(pressure, temperature, relative_humidity, bin_widths):
+                rayleigh = Rayleigh(wavelength, co2_concentration, P, T, RH)
+                beta = rayleigh.beta
+                aod += dh * beta
+                optical_depth.append(aod.to_value())
+            optical_depth_column = np.array([optical_depth])
+            height_column = np.array([height])
+            extinction_per_wavelength = Table(
+                [l, height_column, optical_depth_column],
+                names=("wavelength", "altitude", "AOD"),
+                units=(u.nm, u.m, u.dimensionless_unscaled),
+            )
+            tables.append(extinction_per_wavelength)
+        rayleigh_extinction_table = vstack(tables)
+        rayleigh_extinction_table.write(rayleigh_extinction_file, overwrite=True)
         return rayleigh_extinction_file
```

### Comparing `molecularprofiles-0.3.0/src/molecularprofiles/utils/constants.py` & `molecularprofiles-0.4.0/src/molecularprofiles/utils/constants.py`

 * *Files identical despite different names*

### Comparing `molecularprofiles-0.3.0/src/molecularprofiles/utils/humidity.py` & `molecularprofiles-0.4.0/src/molecularprofiles/utils/humidity.py`

 * *Files 0% similar despite different names*

```diff
@@ -138,33 +138,34 @@
     res[mask] = (
         np.exp(
             1.2378847e-5 / u.K**2 * T[mask] ** 2
             - 1.9121316e-2 / u.K * T[mask]
             + 33.93711047
             - 6343.1645 * u.K / T[mask]
         )
-        * u.Pa
+        / 100.0
+        # * u.Pa
     )
 
     theta = (373.16 * u.K / T[~mask]).to_value()  # ratio of steam point (100 deg C) to temperature
     res[~mask] = (
         np.power(
             10,
             (
                 -7.90298 * (theta - 1)
                 + 5.02808 * np.log10(theta)
                 - 1.3816e-7 * (np.power(10, 11.344 * (1 - 1 / theta)) - 1)
                 + 8.1328e-3 * (np.power(10, -3.49149 * (theta - 1)) - 1)
                 + np.log10(1013.246)
             ),
         )
-        * u.hPa
+        # * u.hPa
     )
 
-    return res
+    return res * u.hPa
 
 
 # TODO: Check this function and write unit test
 def saturation_vapor_pressure_over_water(temperature):
     """
     Calculates the vapor pressure at saturation over water.
 
@@ -338,9 +339,8 @@
         Relative humidity
 
     Returns
     -------
     astropy.units.Quantity
         Water vapor partial pressure
     """
-    # water vapor pressure: e = h * E(temp)
     return relative_humidity.to(u.dimensionless_unscaled) * saturation_vapor_pressure(temperature)
```

### Comparing `molecularprofiles-0.3.0/src/molecularprofiles/utils/rayleigh.py` & `molecularprofiles-0.4.0/src/molecularprofiles/utils/rayleigh.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,16 +71,16 @@
             Relative humidity [%]
         """
         # check inputs for bad values
         if np.any(wavelength < 200 * u.nm) or np.any(wavelength > 4000 * u.nm):
             raise ValueError("Wavelength range only from 200 nm - 4 micrometer allowed.")
         if np.any(pressure < 0 * u.hPa) or np.any(pressure > 1400 * u.hPa):
             raise ValueError("Pressure only in range 0 - 1400 hPa allowed.")
-        if np.any(temperature < 180 * u.K) or np.any(temperature > 373.15 * u.K):
-            raise ValueError("Temperatures only in range 180 - 373 K allowed.")
+        if np.any(temperature < 150 * u.K) or np.any(temperature > 400 * u.K):
+            raise ValueError("Temperatures only in range 150 - 400 K allowed.")
         # if np.any(relative_humidity < 0) or np.any(relative_humidity > 100 * u.percent):
         #    raise ValueError("Relative humity must lie between 0 - 100.")
         # FIXME: Relative humidity can exceed 100%, in case of supersaturated air.
         # The maximum limit should be thought better. However relative humidity cannot go negative.
         # If we receive negative values it is most probably due to interpolation problems.
         # Till we fix these issues it is better to comment out the minimum limit.
         if co2_bkg < 200 or co2_bkg > 1000:
@@ -180,15 +180,14 @@
         """
         return (
             (self.molecular_number_density * self.scattering_cross_section).decompose().to(1 / u.km)
         )
 
     @functools.cached_property
     def refractive_index(self):
-
         """
         Ciddor formula for calculation of refractive index in moist air.
         The obtained refractive index is precise to 1e-7.
 
         Returns
         -------
         float
```

### Comparing `molecularprofiles-0.3.0/src/molecularprofiles.egg-info/PKG-INFO` & `molecularprofiles-0.4.0/src/molecularprofiles.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molecularprofiles
-Version: 0.3.0
+Version: 0.4.0
 Summary: Meteorological data analysis suite
 Author-email: Pere Munar Adrover <pere.munar@uab.cat>, Markus Gaug <markus.gaug@uab.cat>, Scott Griffiths <sgriffiths@ifae.es>, Georgios Voutsinas <georgios.voutsinas@unige.ch>, Mykhailo Dalchenko <mykhailo.dalchenko@unige.ch>
 License: Copyright (c) 2020, Molecularprofiles Project
         
         Redistribution and use in source and binary forms, with or withoutmodification, are permitted provided that the following conditions are met:
         
         1. Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
```

### Comparing `molecularprofiles-0.3.0/src/molecularprofiles.egg-info/SOURCES.txt` & `molecularprofiles-0.4.0/src/molecularprofiles.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -9,9 +9,8 @@
 src/molecularprofiles.egg-info/requires.txt
 src/molecularprofiles.egg-info/top_level.txt
 src/molecularprofiles/utils/__init__.py
 src/molecularprofiles/utils/constants.py
 src/molecularprofiles/utils/grib_utils.py
 src/molecularprofiles/utils/humidity.py
 src/molecularprofiles/utils/mdps_log.conf
-src/molecularprofiles/utils/observatory.py
 src/molecularprofiles/utils/rayleigh.py
```

