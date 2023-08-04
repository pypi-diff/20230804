# Comparing `tmp/mastsel-1.1.tar.gz` & `tmp/mastsel-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mastsel-1.1.tar", last modified: Fri Jul  7 08:51:38 2023, max compression
+gzip compressed data, was "mastsel-1.2.tar", last modified: Fri Aug  4 10:03:12 2023, max compression
```

## Comparing `mastsel-1.1.tar` & `mastsel-1.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:51:38.713973 mastsel-1.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:51:38.709973 mastsel-1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:51:38.709973 mastsel-1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-07 08:51:22.000000 mastsel-1.1/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-07-07 08:51:22.000000 mastsel-1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-07 08:51:22.000000 mastsel-1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-07 08:51:22.000000 mastsel-1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-07-07 08:51:38.709973 mastsel-1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-07-07 08:51:22.000000 mastsel-1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:51:38.709973 mastsel-1.1/mastsel/
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-07-07 08:51:22.000000 mastsel-1.1/mastsel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-07 08:51:38.000000 mastsel-1.1/mastsel/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-07-07 08:51:22.000000 mastsel-1.1/mastsel/ini_to_yaml.py
--rw-r--r--   0 runner    (1001) docker     (123)    20442 2023-07-07 08:51:22.000000 mastsel-1.1/mastsel/mavisFormulas.py
--rw-r--r--   0 runner    (1001) docker     (123)    45142 2023-07-07 08:51:22.000000 mastsel-1.1/mastsel/mavisLO.py
--rw-r--r--   0 runner    (1001) docker     (123)     6165 2023-07-07 08:51:22.000000 mastsel-1.1/mastsel/mavisParams.py
--rw-r--r--   0 runner    (1001) docker     (123)     6033 2023-07-07 08:51:22.000000 mastsel-1.1/mastsel/mavisParamsOld.py
--rw-r--r--   0 runner    (1001) docker     (123)    13216 2023-07-07 08:51:22.000000 mastsel-1.1/mastsel/mavisPsf.py
--rw-r--r--   0 runner    (1001) docker     (123)     7956 2023-07-07 08:51:22.000000 mastsel-1.1/mastsel/mavisUtilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:51:38.709973 mastsel-1.1/mastsel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-07-07 08:51:38.000000 mastsel-1.1/mastsel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-07-07 08:51:38.000000 mastsel-1.1/mastsel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 08:51:38.000000 mastsel-1.1/mastsel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-07 08:51:38.000000 mastsel-1.1/mastsel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-07 08:51:38.000000 mastsel-1.1/mastsel.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:51:38.709973 mastsel-1.1/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-07-07 08:51:22.000000 mastsel-1.1/notebooks/MAVIS-CONVOLUTION-TEST.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     9842 2023-07-07 08:51:22.000000 mastsel-1.1/notebooks/MAVIS-CONVOLUTION.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    10266 2023-07-07 08:51:22.000000 mastsel-1.1/notebooks/MAVIS.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    10100 2023-07-07 08:51:22.000000 mastsel-1.1/notebooks/MAVIS2.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     3929 2023-07-07 08:51:22.000000 mastsel-1.1/notebooks/MAVIS3.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     7064 2023-07-07 08:51:22.000000 mastsel-1.1/notebooks/MAVIS_INT_REC.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-07-07 08:51:22.000000 mastsel-1.1/notebooks/MAVIS_MAIN.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-07 08:51:22.000000 mastsel-1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 08:51:38.713973 mastsel-1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:51:38.709973 mastsel-1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     8749 2023-07-07 08:51:22.000000 mastsel-1.1/tests/allTests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:03:12.164282 mastsel-1.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:03:12.152282 mastsel-1.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:03:12.156282 mastsel-1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-08-04 10:02:52.000000 mastsel-1.2/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-08-04 10:02:52.000000 mastsel-1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-08-04 10:02:52.000000 mastsel-1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-04 10:02:52.000000 mastsel-1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-08-04 10:03:12.164282 mastsel-1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-08-04 10:02:52.000000 mastsel-1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:03:12.160282 mastsel-1.2/mastsel/
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-08-04 10:02:53.000000 mastsel-1.2/mastsel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-08-04 10:03:11.000000 mastsel-1.2/mastsel/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-08-04 10:02:53.000000 mastsel-1.2/mastsel/ini_to_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20482 2023-08-04 10:02:53.000000 mastsel-1.2/mastsel/mavisFormulas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48118 2023-08-04 10:02:53.000000 mastsel-1.2/mastsel/mavisLO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6165 2023-08-04 10:02:53.000000 mastsel-1.2/mastsel/mavisParams.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6033 2023-08-04 10:02:53.000000 mastsel-1.2/mastsel/mavisParamsOld.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13498 2023-08-04 10:02:53.000000 mastsel-1.2/mastsel/mavisPsf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9155 2023-08-04 10:02:53.000000 mastsel-1.2/mastsel/mavisUtilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:03:12.160282 mastsel-1.2/mastsel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-08-04 10:03:11.000000 mastsel-1.2/mastsel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-08-04 10:03:12.000000 mastsel-1.2/mastsel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 10:03:11.000000 mastsel-1.2/mastsel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-08-04 10:03:11.000000 mastsel-1.2/mastsel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-04 10:03:11.000000 mastsel-1.2/mastsel.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:03:12.164282 mastsel-1.2/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-08-04 10:02:53.000000 mastsel-1.2/notebooks/MAVIS-CONVOLUTION-TEST.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     9842 2023-08-04 10:02:53.000000 mastsel-1.2/notebooks/MAVIS-CONVOLUTION.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    10266 2023-08-04 10:02:53.000000 mastsel-1.2/notebooks/MAVIS.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    10100 2023-08-04 10:02:53.000000 mastsel-1.2/notebooks/MAVIS2.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     3929 2023-08-04 10:02:53.000000 mastsel-1.2/notebooks/MAVIS3.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     7064 2023-08-04 10:02:53.000000 mastsel-1.2/notebooks/MAVIS_INT_REC.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-08-04 10:02:53.000000 mastsel-1.2/notebooks/MAVIS_MAIN.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-08-04 10:02:53.000000 mastsel-1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 10:03:12.164282 mastsel-1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:03:12.164282 mastsel-1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7450 2023-08-04 10:02:53.000000 mastsel-1.2/tests/allTests.py
```

### Comparing `mastsel-1.1/.github/workflows/publish.yml` & `mastsel-1.2/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `mastsel-1.1/.gitignore` & `mastsel-1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `mastsel-1.1/LICENSE` & `mastsel-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mastsel-1.1/PKG-INFO` & `mastsel-1.2/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: mastsel
-Version: 1.1
+Version: 1.2
 Summary: Asterism Selection for MAVIS instrument
 Author-email: Fabio Rossi <fabio.rossi@inaf.it>
 License: MIT License
 Project-URL: repository, https://github.com/astro-tiptop/MASTSEL
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: gpu
 License-File: LICENSE
 
 # MASTSEL
 
 This library was developed with 2 goals: support the Asterism Selection for
```

### Comparing `mastsel-1.1/README.md` & `mastsel-1.2/README.md`

 * *Files identical despite different names*

### Comparing `mastsel-1.1/mastsel/ini_to_yaml.py` & `mastsel-1.2/mastsel/ini_to_yaml.py`

 * *Files identical despite different names*

### Comparing `mastsel-1.1/mastsel/mavisFormulas.py` & `mastsel-1.2/mastsel/mavisFormulas.py`

 * *Files 0% similar despite different names*

```diff
@@ -435,7 +435,9 @@
                              truncatedMeanComponents(2),
                              truncatedVarianceComponents(0),
                              truncatedVarianceComponents(1),
                              truncatedVarianceComponents(2)
                            ] )
 
     return _MavisFormulas
+
+_mavisFormulas = createMavisFormulary()
```

### Comparing `mastsel-1.1/mastsel/mavisLO.py` & `mastsel-1.2/mastsel/mavisLO.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,21 +5,22 @@
 if not gpuEnabled:
     cp = np
 else:
     import cupy as cp
 
 from mastsel.mavisUtilities import *
 from mastsel.mavisFormulas import *
+from mastsel.mavisFormulas import _mavisFormulas
+
 import functools
 import multiprocessing as mp
 from configparser import ConfigParser
 import yaml
 import os
 
-
 class MavisLO(object):
     
     def check_section_key(self, primary):
         if self.configType == 'ini':
             return self.config.has_section(primary)
         elif self.configType == 'yml':
             return primary in self.my_yaml_dict.keys()
@@ -102,15 +103,17 @@
         self.WindowRadiusWCoG_LO    = self.get_config_value('sensor_LO','WindowRadiusWCoG')
         self.sigmaRON_LO            = self.get_config_value('sensor_LO','SigmaRON')
         if self.sigmaRON_LO == 0:
             self.sigmaRON_LO = 1e-6
         self.ExcessNoiseFactor_LO   = self.get_config_value('sensor_LO','ExcessNoiseFactor')
         self.Dark_LO                = self.get_config_value('sensor_LO','Dark')
         self.skyBackground_LO       = self.get_config_value('sensor_LO','SkyBackground')
+        # this is called t in MAVIS AOM formulas
         self.ThresholdWCoG_LO       = self.get_config_value('sensor_LO','ThresholdWCoG')
+        # this is called v (nu greek letter) in MAVIS AOM formulas
         self.NewValueThrPix_LO      = self.get_config_value('sensor_LO','NewValueThrPix')
 
         
         if self.check_config_key('sensor_LO','noNoise'):
             self.noNoise = self.get_config_value('sensor_LO','noNoise')
         else:
             self.noNoise = False
@@ -120,25 +123,29 @@
         self.SensorFrameRate_LO     = self.get_config_value('RTC','SensorFrameRate_LO')
         self.loopDelaySteps_LO      = self.get_config_value('RTC','LoopDelaySteps_LO')
         self.LoopGain_LO            = self.get_config_value('RTC','LoopGain_LO')
 
         defaultCompute = 'GPU'
         defaultIntegralDiscretization1 = 1000
         defaultIntegralDiscretization2 = 4000
+        defaultSimpleVarianceComputation = True
         self.computationPlatform =defaultCompute
         self.integralDiscretization1 = defaultIntegralDiscretization1
         self.integralDiscretization2 = defaultIntegralDiscretization2
-        
+        self.simpleVarianceComputation = defaultSimpleVarianceComputation
+
         if self.check_section_key('COMPUTATION'):
             if self.check_config_key('COMPUTATION','platform'):
                 self.computationPlatform    = self.get_config_value('COMPUTATION','platform')
             if self.check_config_key('COMPUTATION','integralDiscretization1'):
                 self.integralDiscretization1 = self.get_config_value('COMPUTATION','integralDiscretization1')
             if self.check_config_key('COMPUTATION','integralDiscretization2'):
                 self.integralDiscretization2 = self.get_config_value('COMPUTATION','integralDiscretization2')
+            if self.check_config_key('COMPUTATION','simpleVarianceComputation'):
+                self.simpleVarianceComputation = self.get_config_value('COMPUTATION','simpleVarianceComputation')
 
         if self.check_config_key('atmosphere','r0_Value') and self.check_config_key('atmosphere','Seeing'):
             print('%%%%%%%% ATTENTION %%%%%%%%')
             print('You must provide r0_Value or Seeing value, not both, ')
             print('Seeing parameter will be used, r0_Value will be discarded!\n')
 
         if self.check_config_key('atmosphere','Seeing'):
@@ -170,32 +177,39 @@
         else:
             self.wSpeed = self.get_config_value('atmosphere','WindSpeed')
             self.WindSpeed = (np.dot( np.power(np.asarray(self.wSpeed), 5.0/3.0), np.asarray(self.Cn2Weights) ) / np.sum( np.asarray(self.Cn2Weights) ) ) ** (3.0/5.0)
 
         #
         # END OF SETTING PARAMETERS READ FROM FILE       
         #
-        
+       
         airmass = 1/np.cos(self.ZenithAngle*np.pi/180)
         self.r0_Value = self.r0_Value * airmass**(-3.0/5.0)
                  
 #        self.mutex = None
         self.imax = 30
         self.zmin = 0.03
         self.zmax = 30
         self.integrationPoints = self.integralDiscretization1
         self.psdIntegrationPoints = self.integralDiscretization2
         self.largeGridSize = 200
         self.downsample_factor = 4
+        # this is N_W in the simplified variance formulas
         self.smallGridSize = 2*self.WindowRadiusWCoG_LO
         self.p_offset = 1.0 # 1/4 pixel on medium grid
         self.mediumGridSize = int(self.largeGridSize/self.downsample_factor)
         self.mediumShape = (self.mediumGridSize,self.mediumGridSize)
         self.mediumPixelScale = self.PixelScale_LO/self.downsample_factor
-        self.MavisFormulas = createMavisFormulary()
+
+        # diffraction limited FWHM - full aperture
+        self.diffNGS_FWHM_mas = self.SensingWavelength_LO/(self.TelescopeDiameter)*radiansToArcsecs*1000
+        # diffraction limited FWHM - one aperture
+        self.subapNGS_FWHM_mas = self.SensingWavelength_LO/(self.TelescopeDiameter/self.NumberLenslets[0])*radiansToArcsecs*1000
+
+        self.MavisFormulas = _mavisFormulas
         self.zernikeCov_rh1 = self.MavisFormulas.getFormulaRhs('ZernikeCovarianceD')
         self.zernikeCov_lh1 = self.MavisFormulas.getFormulaLhs('ZernikeCovarianceD')
         self.sTurbPSDTip, self.sTurbPSDTilt = self.specializedTurbFuncs()
         self.fCValue = self.specializedC_coefficient()
         self.fTipS_LO, self.fTiltS_LO = self.specializedNoiseFuncs()
         self.fTipS, self.fTiltS = self.specializedWindFuncs()
         self.specializedCovExprs = self.buildSpecializedCovFunctions()
@@ -425,74 +439,102 @@
         paramsAndRanges = [( 'f_k', gaussianPoints, 0.0, 0.0, 'provided' )]
         lh = sp.Function('B')(getSymbolByName(aFunction, 'f_k'))
         xplot1, zplot1 = self.mIt.IntegralEval(lh, aIntegral, paramsAndRanges, [ (self.integrationPoints//2, 'linear'), (self.imax, 'linear')], 'raw')
         ssx, s0 = self.mIt.functionEval(expr0, paramsAndRanges )
         zplot1 = zplot1 + s0
         lh = sp.Function('B')(getSymbolByName(expr1, 'f_k'))
         ssx, zplot2 = self.mIt.functionEval(expr1, paramsAndRanges )
+        # magic number 10 here is due to the fact that more than 10 photons flux can be approximated witha gaussian distribution
         rr = np.where(gaussianPoints + self.Dark_LO/self.SensorFrameRate_LO < 10.0, zplot1, zplot2)
         rr = rr.reshape((self.smallGridSize,self.smallGridSize))
         return ssx, rr
 
     
     def meanVarSigma(self, gaussianPoints):
         xplot1, mu_ktr_array = self.compute2DMeanVar( self.aFunctionM, self.expr0M, gaussianPoints, self.aFunctionMGauss)
         xplot2, var_ktr_array = self.compute2DMeanVar( self.aFunctionV, self.expr0V, gaussianPoints, self.aFunctionVGauss)
         var_ktr_array = var_ktr_array - mu_ktr_array**2
         sigma_ktr_array = np.sqrt(var_ktr_array.astype(np.float32))
         return mu_ktr_array, var_ktr_array, sigma_ktr_array
 
-        
-    def computeBias(self, aNGS_flux, aNGS_SR_LO, aNGS_FWHM_mas):
-        gridSpanArcsec= self.mediumPixelScale*self.largeGridSize/1000
-        gridSpanRad = gridSpanArcsec/radiansToArcsecs
-        
-        # diffraction limited FWHM - full aperture
-        diffNGS_FWHM_mas = self.SensingWavelength_LO/(self.TelescopeDiameter)*radiansToArcsecs*1000
-        # diffraction limited FWHM - one sub-aperture
-        subapNGS_FWHM_mas = self.SensingWavelength_LO/(self.TelescopeDiameter/self.NumberLenslets[0])*radiansToArcsecs*1000
+    def sigmaTotXX(self, sigma_ph_xx, sigma_ron_xx):
+        return (1.0/self.N_sa_tot_LO) * ( sigma_ph_xx + sigma_ron_xx)
+        # * self.PixelScale_LO**2
+
+
+    def simplifiedComputeBiasAndVariance(self, aNGS_flux, aNGS_SR_LO, aNGS_FWHM_mas):
+        # aNGS_flux is provided in photons/s
+        FWHM_coeff = np.sqrt(np.abs(aNGS_FWHM_mas**2 - self.diffNGS_FWHM_mas**2 ))
+        aNGS_FWHM_mas_mod = np.sqrt( FWHM_coeff**2 + self.subapNGS_FWHM_mas**2 )
+        # print('             aNGS_FWHM_mas_mod',aNGS_FWHM_mas_mod)
+        back = self.skyBackground_LO/self.SensorFrameRate_LO
+        N_T = aNGS_FWHM_mas_mod/self.PixelScale_LO
+        # print('             N_T',N_T)
+        N_W = self.smallGridSize
+        # print('             N_W',N_W)
+        N_D = self.subapNGS_FWHM_mas/self.PixelScale_LO
+        sigma_e = np.sqrt( self.ExcessNoiseFactor_LO * (self.Dark_LO / self.SensorFrameRate_LO + back) + self.sigmaRON_LO**2 )
+        # print('             sigma_e',sigma_e)
+        sigma_ph_fwhm = 0.25*self.ExcessNoiseFactor_LO*(1.0/(2.0*np.log(2.0)*aNGS_flux/self.SensorFrameRate_LO)) * ((N_T)*((N_T**2+N_W**2)/(2*N_T**2+N_W**2))) ** 2
+        # print('             sigma_ph_fwhm',sigma_ph_fwhm)
+        sigma_ron_fwhm = 0.25*(np.pi/(32.0*(np.log(2.0)**2))) * ( (sigma_e/(aNGS_flux/self.SensorFrameRate_LO)) * (N_T**2+N_W**2) ) ** 2
+        # print('             sigma_ron_fwhm',sigma_ron_fwhm)
+        sigma_ph_sr = (1.0/aNGS_SR_LO) * sigma_ph_fwhm
+        sigma_ron_sr = (1.0/aNGS_SR_LO)**2 * sigma_ron_fwhm
+        sigma_tot_fwhm = self.sigmaTotXX(sigma_ph_fwhm, sigma_ron_fwhm)
+        sigma_tot_sr = self.sigmaTotXX(sigma_ph_sr, sigma_ron_sr)
+        sigma_tot = (N_D/N_T)**2 * sigma_tot_sr + ( 1.0 - (N_D/N_T)**2 ) * sigma_tot_fwhm
+        varx = vary = sigma_tot
+        mux = muy = 0
+        bias = N_W**2/(N_W**2+N_T**2)
+        return (bias,(mux,muy),(varx,vary))
+
+
+    def computeBiasAndVariance(self, aNGS_flux, aNGS_SR_LO, aNGS_FWHM_mas):
+        # aNGS_flux is provided in photons/s
+
         # increment of FWHM given by the partial correction
-        FWHM_coeff = np.sqrt(np.abs(aNGS_FWHM_mas**2 - diffNGS_FWHM_mas**2 ))
+        FWHM_coeff = np.sqrt(np.abs(aNGS_FWHM_mas**2 - self.diffNGS_FWHM_mas**2 ))
         # estimated FWHM on a sub-aperture 
-        aNGS_FWHM_mas_mod = np.sqrt( FWHM_coeff**2 + subapNGS_FWHM_mas**2 )
+        aNGS_FWHM_mas_mod = np.sqrt( FWHM_coeff**2 + self.subapNGS_FWHM_mas**2 )
         asigma = aNGS_FWHM_mas_mod/sigmaToFWHM/self.mediumPixelScale
             
         xCoords=np.asarray(np.linspace(-self.largeGridSize/2.0+0.5, self.largeGridSize/2.0-0.5, self.largeGridSize), dtype=np.float32)
         yCoords=np.asarray(np.linspace(-self.largeGridSize/2.0+0.5, self.largeGridSize/2.0-0.5, self.largeGridSize), dtype=np.float32)
         xGrid, yGrid = np.meshgrid( xCoords, yCoords, sparse=False, copy=True)
         
         loD = self.SensingWavelength_LO/self.TelescopeDiameter*radiansToArcsecs*1000
        
-        if aNGS_FWHM_mas >= 2*diffNGS_FWHM_mas:
+        if aNGS_FWHM_mas >= 2*self.diffNGS_FWHM_mas and not self.LoopGain_LO=='test':
             if self.verbose:
-                print('mavisLO.computeBias, FWHM (',aNGS_FWHM_mas,') is larger than 2 times the diffraction.')
+                print('mavisLO.computeBiasVariance, FWHM (',aNGS_FWHM_mas,') is larger than 2 times the diffraction.')
             # if correction is low we consider that there is a seeing limited like PSF
             g2d = simple2Dgaussian( xGrid, yGrid, 0, 0, asigma)
             g2d = g2d * aNGS_flux/self.SensorFrameRate_LO * 1 / np.sum(g2d)
             peakValue = np.max(g2d)
-        elif aNGS_FWHM_mas >= 1.25*diffNGS_FWHM_mas and aNGS_FWHM_mas < 2*diffNGS_FWHM_mas:
+        elif aNGS_FWHM_mas >= 1.25*self.diffNGS_FWHM_mas and aNGS_FWHM_mas < 2*self.diffNGS_FWHM_mas and not self.LoopGain_LO=='test':
             if self.verbose:
-                print('mavisLO.computeBias, FWHM (',aNGS_FWHM_mas,') is less than 2 times the diffraction, but more than 1.25 times diffraction.')
+                print('mavisLO.computeBiasVariance, FWHM (',aNGS_FWHM_mas,') is less than 2 times the diffraction, but more than 1.25 times diffraction.')
             # if correction is "medium" we consider that there is a comination of diffration limited and seeing limited like PSF
             r0_SensingWavelength_LO = self.r0_Value * (self.SensingWavelength_LO/self.AtmosphereWavelength)**(6/5)
             seeing = 0.976*self.AtmosphereWavelength/r0_SensingWavelength_LO*206264.8 # * np.sqrt(1-2.183*(r0_SensingWavelength_LO/self.L0)*0.356)
-            seeing = np.sqrt( seeing**2 + subapNGS_FWHM_mas**2 )
+            seeing = np.sqrt( seeing**2 + self.subapNGS_FWHM_mas**2 )
             asigma_seeing = seeing/sigmaToFWHM/self.mediumPixelScale
             g2d_seeing = simple2Dgaussian( xGrid, yGrid, 0, 0, asigma)
             g2d_seeing = g2d_seeing * (1-aNGS_SR_LO) * aNGS_flux/self.SensorFrameRate_LO * 1 / np.sum(g2d_seeing)
-            peakValue = aNGS_flux/self.SensorFrameRate_LO*aNGS_SR_LO*4.0*np.log(2)/(np.pi*(diffNGS_FWHM_mas/self.mediumPixelScale)**2)
+            peakValue = aNGS_flux/self.SensorFrameRate_LO*aNGS_SR_LO*4.0*np.log(2)/(np.pi*(self.diffNGS_FWHM_mas/self.mediumPixelScale)**2)
             g2d = peakValue * simple2Dgaussian( xGrid, yGrid, 0, 0, asigma)
             g2d = g2d + g2d_seeing
             peakValue = np.max(g2d)
         else:
             if self.verbose:
-                print('mavisLO.computeBias, FWHM (',aNGS_FWHM_mas,') is less than 1.25 times the diffraction.')
+                print('mavisLO.computeBiasVariance, FWHM (',aNGS_FWHM_mas,') is less than 1.25 times the diffraction.')
             # if correction is high we consider that there is a diffraction limited core
             # in the center of the PSF and wings given by the fitting error
-            peakValue = aNGS_flux/self.SensorFrameRate_LO*aNGS_SR_LO*4.0*np.log(2)/(np.pi*(diffNGS_FWHM_mas/self.mediumPixelScale)**2)
+            peakValue = aNGS_flux/self.SensorFrameRate_LO*aNGS_SR_LO*4.0*np.log(2)/(np.pi*(self.diffNGS_FWHM_mas/self.mediumPixelScale)**2)
             g2d = peakValue * simple2Dgaussian( xGrid, yGrid, 0, 0, asigma)
             
         if self.verbose:
             print('mavisLO.computeBias, peakValue',peakValue)
 
         g2d = intRebin(g2d, self.mediumShape) * self.downsample_factor**2
         I_k_data = peakValue * simple2Dgaussian( xGrid, yGrid, 0, 0, asigma)
@@ -508,16 +550,14 @@
         W_Mask = np.where( np.logical_or(fx**2 +fy**2 > self.WindowRadiusWCoG_LO**2, fx**2 + fy**2 < 0**2), 0.0, 1.0)
         ii1, ii2 = int(self.mediumGridSize/2-self.smallGridSize/2), int(self.mediumGridSize/2+self.smallGridSize/2)
         f_k_data = f_k_data[ii1:ii2,ii1:ii2]
         f_k_prime_data = f_k_prime_data[ii1:ii2,ii1:ii2]
         W_Mask = W_Mask[ii1:ii2,ii1:ii2]
         fx = fx[ii1:ii2,ii1:ii2]
         fy = fy[ii1:ii2,ii1:ii2]
-        gridSpanArcsec= self.mediumPixelScale*self.smallGridSize/1000
-        gridSpanRad = gridSpanArcsec/radiansToArcsecs
         mu_ktr_array, var_ktr_array, sigma_ktr_array = self.meanVarSigma(f_k_data)
         mu_ktr_prime_array, var_ktr_prime_array, sigma_ktr_prime_array = self.meanVarSigma(f_k_prime_data)
         masked_mu0 = W_Mask*mu_ktr_array
         masked_mu = W_Mask*mu_ktr_prime_array
         masked_sigma = W_Mask*W_Mask*var_ktr_array
         mux = np.sum(masked_mu*fx)/np.sum(masked_mu)
         muy = np.sum(masked_mu*fy)/np.sum(masked_mu)
@@ -595,14 +635,16 @@
         else:
             xp = np
         if self.LoopGain_LO == 'optimize':
             # add small values of gain to have a good optimization
             # when the noise level is high.
             g0 = (0.00000001,0.0000001,0.000001,0.00001,0.0001,0.001)
             g0g = xp.concatenate((xp.asarray( g0),xp.linspace(0.01, 0.99, npoints)))
+        elif self.LoopGain_LO == 'test':
+            g0g = xp.asarray( xp.linspace(0.01, 0.99, npoints) )
         else:
             # if gain is set no optimization is done and bias is not compensated
             g0 = (bias*self.LoopGain_LO,bias*self.LoopGain_LO)
             g0g = xp.asarray(g0)
             
         e1 = psd_freq.reshape((1,psd_freq.shape[0]))
         e2 = psd_tip_wind.reshape((1,psd_tip_wind.shape[0]))
@@ -665,14 +707,16 @@
             xp = np
         
         if self.LoopGain_LO == 'optimize':
             # add small values of gain to have a good optimization
             # when the noise level is high.
             g0 = (0.00000001,0.0000001,0.000001,0.00001,0.0001,0.001)
             g0g = xp.concatenate((xp.asarray( g0),xp.linspace(0.01, 0.99, npoints)))
+        elif self.LoopGain_LO == 'test':
+            g0g = xp.asarray( xp.linspace(0.01, 0.99, npoints) )
         else:
             # if gain is set no optimization is done and bias is not compensated
             g0 = (bias*self.LoopGain_LO,bias*self.LoopGain_LO)
             g0g = xp.asarray(g0)
         g0g, g1g = xp.meshgrid( g0g,g0g )
         
         e1 = psd_freq.reshape((1,1,psd_freq.shape[0]))
@@ -814,19 +858,24 @@
 
         if self.verbose:
             print('mavisLO.computeTotalResidualMatrix')
             print('         aNGS_flux',aNGS_flux)
             print('         self.N_sa_tot_LO',self.N_sa_tot_LO)
             
         for starIndex in range(nNaturalGS):
-            bias, amu, avar = self.computeBias(aNGS_flux[starIndex], aNGS_SR_LO[starIndex], aNGS_FWHM_mas[starIndex]) # one scalar, two tuples of 2
+            if self.simpleVarianceComputation:
+                bias, amu, avar = self.simplifiedComputeBiasAndVariance(aNGS_flux[starIndex], aNGS_SR_LO[starIndex], aNGS_FWHM_mas[starIndex]) # one scalar, two
+            else:
+                bias, amu, avar = self.computeBiasAndVariance(aNGS_flux[starIndex], aNGS_SR_LO[starIndex], aNGS_FWHM_mas[starIndex]) # one scalar, two tuples of 2
+
             if self.verbose:
                 print('         bias',bias)
                 print('         amu',amu)
                 print('         avar',avar)
+                print('             ratio',avar/(bias**2))
 
             var1x = avar[0] * self.PixelScale_LO**2
             nr = self.computeNoiseResidual(0.25, 250.0, 1000, var1x, bias, self.platformlib )
             # TODO: this second computation must be embedded in the previous one.
             wr = self.computeWindResidual(self.psd_freq, self.psd_tip_wind, self.psd_tilt_wind, var1x, bias, self.platformlib )
             if self.verbose:
                 print('         noise residual:     ',nr)
```

### Comparing `mastsel-1.1/mastsel/mavisParams.py` & `mastsel-1.2/mastsel/mavisParams.py`

 * *Files identical despite different names*

### Comparing `mastsel-1.1/mastsel/mavisParamsOld.py` & `mastsel-1.2/mastsel/mavisParamsOld.py`

 * *Files identical despite different names*

### Comparing `mastsel-1.1/mastsel/mavisPsf.py` & `mastsel-1.2/mastsel/mavisPsf.py`

 * *Files 9% similar despite different names*

```diff
@@ -132,33 +132,38 @@
 
     def hostData(self, _data):
         if self.xp == cp and gpuEnabled:
             return cp.asnumpy(_data)
         else:
             return _data
 
+    def gModel1(self, x, y, sigma_X, sigma_Y, angle):
+        A = 1.0
+        x0 = self.N / 2
+        y0 = self.N / 2
+        x_stddev= sigma_X / self.pixel_size
+        y_stddev= sigma_Y / self.pixel_size
+        theta = angle
+        a = self.xp.cos(theta)*self.xp.cos(theta)/(2*x_stddev*x_stddev) + self.xp.sin(theta)*self.xp.sin(theta)/(2*y_stddev*y_stddev)
+        b = self.xp.sin(2*theta)/(2*x_stddev*x_stddev) - self.xp.sin(2*theta)/(2*y_stddev*y_stddev)
+        c = self.xp.sin(theta)*self.xp.sin(theta)/(2*x_stddev*x_stddev) + self.xp.cos(theta)*self.xp.cos(theta)/(2*y_stddev*y_stddev)
+        return A * self.xp.exp( -a*(x-x0)*(x-x0)-b*(x-x0)*(y-y0)-c*(y-y0)*(y-y0) )
+
     def loadSamplingFromFile(self, filename):
         hdul = fits.open(filename)
         self.sampling = self.xp.asarray(hdul[0].data, self.sampling.dtype)
 
     # put the peak at the center of the Field, could change if needed
     # angle in rad
     # sigma_X, sigma_Y in the same unit as the Field
     def setAsGaussianKernel(self, sigma_X, sigma_Y, angle):
-        gModel = models.Gaussian2D(
-            amplitude=1,
-            x_mean=self.N / 2,
-            y_mean=self.N / 2,
-            x_stddev=sigma_X / self.pixel_size,
-            y_stddev=sigma_Y / self.pixel_size,
-            theta=angle,
-            cov_matrix=None)
-        y, x = np.mgrid[:self.N, :self.N]
-        hostSampling = gModel(x, y)
-        self.sampling = self.xp.asarray(hostSampling)
+        yg, xg = self.xp.mgrid[:self.N, :self.N]
+        hostSampling1 = self.gModel1(xg, yg, sigma_X, sigma_Y, angle)
+        self.sampling = hostSampling1
+
 
     def setAsTelescopeMask(self, telescope_radius, occlusion_radius=0):
         fx = (self.xp.arange(-self.N / 2., self.N / 2., 1.0) + 0.5) * \
             self.pixel_size
         (fx, fy) = self.xp.meshgrid(fx, fx)
         self.sampling = self.xp.where(
             self.xp.logical_or(
@@ -391,18 +396,16 @@
     # step 2 : compute structure function
     # D_phi = 2.0 * (-B_phi + b0)
     D_phi = 2.0 * b0 - (B_phi + B_phi.conj())
         
     # step 3 : compute turbolence otf
     otf_turb = xp.exp(-0.5 * (D_phi))    
     # p_otft_turb = pitch
-    if gpuEnabled:
-        otf_turb = cp.asarray(congrid(cp.asnumpy(otf_turb), [otf_turb.shape[0]//2, otf_turb.shape[0]//2]))
-    else:
-        otf_turb = np.asarray(congrid(otf_turb, [otf_turb.shape[0]//2, otf_turb.shape[0]//2]))
+    otf_turb = congrid(otf_turb, [otf_turb.shape[0]//2, otf_turb.shape[0]//2])
+
     # step 4 : combine telescope and turbolence otfs
     otf_system = otf_turb * otf_tel
 
     # step 5 : system otf to system psf
     result.sampling = xp.real(ft_ft2(otf_system))
     if xp.__name__=='cupy':
         result.sampling =  xp.asnumpy(result.sampling)
```

### Comparing `mastsel-1.1/mastsel/mavisUtilities.py` & `mastsel-1.2/mastsel/mavisUtilities.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,147 @@
 from copy import deepcopy
+
 import numpy as np
 
 from astropy.io import fits
 import matplotlib.pyplot as plt
 from matplotlib import cm
 from astropy.modeling import models, fitting
 
 import scipy.signal
 import scipy.ndimage
-import scipy.interpolate
+
+from . import gpuEnabled
+
+if not gpuEnabled:
+    cp = np
+    import scipy.interpolate    
+    from scipy.interpolate import RegularGridInterpolator
+
+    def congrid(a, newdims, method='linear', centre=False, minusone=False):
+        '''Arbitrary resampling of source array to new dimension sizes.
+        Currently only supports maintaining the same number of dimensions.
+        To use 1-D arrays, first promote them to shape (x,1).
+
+        Uses the same parameters and creates the same co-ordinate lookup points
+        as IDL''s congrid routine, which apparently originally came from a VAX/VMS
+        routine of the same name.
+
+        method:
+        neighbour - closest value from original data
+        nearest and linear - uses n x 1-D interpolations using
+                             scipy.interpolate.interp1d
+        (see Numerical Recipes for validity of use of n 1-D interpolations)
+        spline - uses ndimage.map_coordinates
+
+        centre:
+        True - interpolation points are at the centres of the bins
+        False - points are at the front edge of the bin
+
+        minusone:
+        For example- inarray.shape = (i,j) & new dimensions = (x,y)
+        False - inarray is resampled by factors of (i/x) * (j/y)
+        True - inarray is resampled by(i-1)/(x-1) * (j-1)/(y-1)
+        This prevents extrapolation one element beyond bounds of input array.
+        '''
+        if a.dtype not in [np.float64, np.float32]:
+            a = np.cast[float](a)
+
+        m1 = np.cast[int](minusone)
+        ofs = np.cast[int](centre) * 0.5
+        old = np.array(a.shape)
+        ndims = len(a.shape)
+        if len(newdims) != ndims:
+            print("[congrid] dimensions error. "
+                  "This routine currently only support "
+                  "rebinning to the same number of dimensions.")
+            return None
+        newdims = np.asarray(newdims, dtype=float)
+        dimlist = []
+
+        if method == 'neighbour':
+            for i in range(ndims):
+                base = np.indices(newdims)[i]
+                dimlist.append((old[i] - m1) / (newdims[i] - m1)
+                               * (base + ofs) - ofs)
+            cd = np.array(dimlist).round().astype(int)
+            newa = a[list(cd)]
+            return newa
+
+        elif method in ['nearest', 'linear']:
+            # calculate new dims
+            for i in range(ndims):
+                base = np.arange(newdims[i])
+                dimlist.append((old[i] - m1) / (newdims[i] - m1)
+                               * (base + ofs) - ofs)
+            # specify old dims
+            olddims = [np.arange(i, dtype=float) for i in list(a.shape)]
+
+            # first interpolation - for ndims = any
+            mint = scipy.interpolate.interp1d(
+                olddims[-1], a, kind=method, fill_value="extrapolate")
+            newa = mint(dimlist[-1])
+
+            trorder = [ndims - 1] + list(range(ndims - 1))
+            for i in range(ndims - 2, -1, -1):
+                newa = newa.transpose(trorder)
+
+                mint = scipy.interpolate.interp1d(
+                    olddims[i], newa, kind=method, fill_value="extrapolate")
+                newa = mint(dimlist[i])
+
+            if ndims > 1:
+                # need one more transpose to return to original dimensions
+                newa = newa.transpose(trorder)
+
+            return newa
+        elif method in ['spline']:
+            oslices = [slice(0, j) for j in old]
+            oldcoords = np.ogrid[oslices]
+            nslices = [slice(0, j) for j in list(newdims)]
+            newcoords = np.mgrid[nslices]
+
+            newcoords_dims = range(np.rank(newcoords))
+            # make first index last
+            newcoords_dims.append(newcoords_dims.pop(0))
+            newcoords_tr = newcoords.transpose(newcoords_dims)
+            # makes a view that affects newcoords
+
+            newcoords_tr += ofs
+
+            deltas = (np.asarray(old) - m1) / (newdims - m1)
+            newcoords_tr *= deltas
+
+            newcoords_tr -= ofs
+
+            newa = scipy.ndimage.map_coordinates(a, newcoords)
+            return newa
+        else:
+            print("Congrid error: Unrecognized interpolation type.\n",
+                  "Currently only \'neighbour\', \'nearest\',\'linear\',",
+                  "and \'spline\' are supported.")
+        return None
+else:
+    import cupy as cp
+    from cupyx.scipy.interpolate import RegularGridInterpolator
+    # works for now, to be checked in different cases
+    def congrid(a, newdims):
+
+        newdims = np.asarray(newdims, dtype=int)
+        r1 = a.shape[0]/newdims[0]
+        r2 = a.shape[1]/newdims[1]
+
+        interp = RegularGridInterpolator((cp.linspace(0.5, a.shape[0]-0.5, a.shape[0]), cp.linspace(0.5, a.shape[1]-0.5, a.shape[1])), 
+                                         a, bounds_error=False, fill_value=None)
+
+        xx = cp.linspace(0.5, a.shape[0] - (r1 - 0.5), newdims[0])
+        yy = cp.linspace(0.5, a.shape[1] - (r2 - 0.5), newdims[1])
+
+        X, Y = cp.meshgrid(xx, yy, indexing='ij')
+        return interp((X, Y))
 
 degToRad = np.pi/180.0
 radToDeg = 1.0/degToRad
 radiansToArcsecs = 206265.0
 arcsecsToRadians = 1.0/radiansToArcsecs
 radiansToMas = radiansToArcsecs * 1000.0
 
@@ -54,120 +183,14 @@
         polar_data,
         coords,
         order=order,
         mode='constant',
         cval=np.nan)
     return(cart_data.reshape(len(y), len(x)).T)
 
-
-def congrid(a, newdims, method='linear', centre=False, minusone=False):
-    '''Arbitrary resampling of source array to new dimension sizes.
-    Currently only supports maintaining the same number of dimensions.
-    To use 1-D arrays, first promote them to shape (x,1).
-
-    Uses the same parameters and creates the same co-ordinate lookup points
-    as IDL''s congrid routine, which apparently originally came from a VAX/VMS
-    routine of the same name.
-
-    method:
-    neighbour - closest value from original data
-    nearest and linear - uses n x 1-D interpolations using
-                         scipy.interpolate.interp1d
-    (see Numerical Recipes for validity of use of n 1-D interpolations)
-    spline - uses ndimage.map_coordinates
-
-    centre:
-    True - interpolation points are at the centres of the bins
-    False - points are at the front edge of the bin
-
-    minusone:
-    For example- inarray.shape = (i,j) & new dimensions = (x,y)
-    False - inarray is resampled by factors of (i/x) * (j/y)
-    True - inarray is resampled by(i-1)/(x-1) * (j-1)/(y-1)
-    This prevents extrapolation one element beyond bounds of input array.
-    '''
-    if a.dtype not in [np.float64, np.float32]:
-        a = np.cast[float](a)
-
-    m1 = np.cast[int](minusone)
-    ofs = np.cast[int](centre) * 0.5
-    old = np.array(a.shape)
-    ndims = len(a.shape)
-    if len(newdims) != ndims:
-        print("[congrid] dimensions error. "
-              "This routine currently only support "
-              "rebinning to the same number of dimensions.")
-        return None
-    newdims = np.asarray(newdims, dtype=float)
-    dimlist = []
-
-    if method == 'neighbour':
-        for i in range(ndims):
-            base = np.indices(newdims)[i]
-            dimlist.append((old[i] - m1) / (newdims[i] - m1)
-                           * (base + ofs) - ofs)
-        cd = np.array(dimlist).round().astype(int)
-        newa = a[list(cd)]
-        return newa
-
-    elif method in ['nearest', 'linear']:
-        # calculate new dims
-        for i in range(ndims):
-            base = np.arange(newdims[i])
-            dimlist.append((old[i] - m1) / (newdims[i] - m1)
-                           * (base + ofs) - ofs)
-        # specify old dims
-        olddims = [np.arange(i, dtype=float) for i in list(a.shape)]
-
-        # first interpolation - for ndims = any
-        mint = scipy.interpolate.interp1d(
-            olddims[-1], a, kind=method, fill_value="extrapolate")
-        newa = mint(dimlist[-1])
-
-        trorder = [ndims - 1] + list(range(ndims - 1))
-        for i in range(ndims - 2, -1, -1):
-            newa = newa.transpose(trorder)
-
-            mint = scipy.interpolate.interp1d(
-                olddims[i], newa, kind=method, fill_value="extrapolate")
-            newa = mint(dimlist[i])
-
-        if ndims > 1:
-            # need one more transpose to return to original dimensions
-            newa = newa.transpose(trorder)
-
-        return newa
-    elif method in ['spline']:
-        oslices = [slice(0, j) for j in old]
-        oldcoords = np.ogrid[oslices]
-        nslices = [slice(0, j) for j in list(newdims)]
-        newcoords = np.mgrid[nslices]
-
-        newcoords_dims = range(np.rank(newcoords))
-        # make first index last
-        newcoords_dims.append(newcoords_dims.pop(0))
-        newcoords_tr = newcoords.transpose(newcoords_dims)
-        # makes a view that affects newcoords
-
-        newcoords_tr += ofs
-
-        deltas = (np.asarray(old) - m1) / (newdims - m1)
-        newcoords_tr *= deltas
-
-        newcoords_tr -= ofs
-
-        newa = scipy.ndimage.map_coordinates(a, newcoords)
-        return newa
-    else:
-        print("Congrid error: Unrecognized interpolation type.\n",
-              "Currently only \'neighbour\', \'nearest\',\'linear\',",
-              "and \'spline\' are supported.")
-        return None
-
-
 def fitGaussian(image):
     N = image.shape[0]
     p_init = models.Gaussian2D(
         amplitude=np.max(image),
         x_mean=N / 2,
         y_mean=N / 2)
     fit_p = fitting.LevMarLSQFitter()
@@ -194,16 +217,16 @@
     plt.xscale('linear')
     plt.yscale('log')
     plt.plot(result[:, result.shape[0] // 2])
     plt.plot(myResult[:, myResult.shape[0] // 2])
     plt.show()
 
 
-def simple2Dgaussian(x, y, x0=0.0, y0=0.0, sg=1.0):
-    return np.exp(-((x-x0)**2)/(2*sg**2)-((y-y0)**2)/(2*sg**2) )
+def simple2Dgaussian(x, y, x0=0.0, y0=0.0, sg=1.0, xp=np):
+    return xp.exp(-((x-x0)**2)/(2*sg**2)-((y-y0)**2)/(2*sg**2) )
 
 def intRebin(arr, new_shape):
     shape = (new_shape[0], arr.shape[0] // new_shape[0],
              new_shape[1], arr.shape[1] // new_shape[1])
     return arr.reshape(shape).mean(-1).mean(1)
```

### Comparing `mastsel-1.1/mastsel.egg-info/PKG-INFO` & `mastsel-1.2/mastsel.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: mastsel
-Version: 1.1
+Version: 1.2
 Summary: Asterism Selection for MAVIS instrument
 Author-email: Fabio Rossi <fabio.rossi@inaf.it>
 License: MIT License
 Project-URL: repository, https://github.com/astro-tiptop/MASTSEL
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: gpu
 License-File: LICENSE
 
 # MASTSEL
 
 This library was developed with 2 goals: support the Asterism Selection for
```

### Comparing `mastsel-1.1/mastsel.egg-info/SOURCES.txt` & `mastsel-1.2/mastsel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mastsel-1.1/notebooks/MAVIS-CONVOLUTION-TEST.ipynb` & `mastsel-1.2/notebooks/MAVIS-CONVOLUTION-TEST.ipynb`

 * *Files identical despite different names*

### Comparing `mastsel-1.1/notebooks/MAVIS-CONVOLUTION.ipynb` & `mastsel-1.2/notebooks/MAVIS-CONVOLUTION.ipynb`

 * *Files identical despite different names*

### Comparing `mastsel-1.1/notebooks/MAVIS.ipynb` & `mastsel-1.2/notebooks/MAVIS.ipynb`

 * *Files identical despite different names*

### Comparing `mastsel-1.1/notebooks/MAVIS2.ipynb` & `mastsel-1.2/notebooks/MAVIS2.ipynb`

 * *Files identical despite different names*

### Comparing `mastsel-1.1/notebooks/MAVIS3.ipynb` & `mastsel-1.2/notebooks/MAVIS3.ipynb`

 * *Files identical despite different names*

### Comparing `mastsel-1.1/notebooks/MAVIS_INT_REC.ipynb` & `mastsel-1.2/notebooks/MAVIS_INT_REC.ipynb`

 * *Files identical despite different names*

### Comparing `mastsel-1.1/notebooks/MAVIS_MAIN.ipynb` & `mastsel-1.2/notebooks/MAVIS_MAIN.ipynb`

 * *Files identical despite different names*

### Comparing `mastsel-1.1/pyproject.toml` & `mastsel-1.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -6,23 +6,24 @@
 name = "mastsel"
 authors = [
     {name = "Fabio Rossi", email = "fabio.rossi@inaf.it"},
 ]
 description = "Asterism Selection for MAVIS instrument"
 readme = "README.md"
 urls = {repository = "https://github.com/astro-tiptop/MASTSEL"}
-requires-python = ">=3.7"
+requires-python = ">=3.9"
 license = {text = "MIT License"}
 dependencies = [
     "astropy",
     "matplotlib",
     "numpy",
     "PyYAML",
     "scipy",
     "symao",
+    "seeing>=1.1",
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 gpu = ["cupy"]
 
 [tool.setuptools.packages]
```

### Comparing `mastsel-1.1/tests/allTests.py` & `mastsel-1.2/tests/allTests.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 class TestMavisLO(unittest.TestCase):
     @classmethod
     def setUpClass(cls):
         path = "../data/ini/"
         parametersFile = 'mavisParamsTests'
         fullPathFilename = path + parametersFile + '.ini'
         windPsdFile = '../data/windpsd_mavis.fits'
-        TestMavisLO.mLO = MavisLO(path, parametersFile)
+        TestMavisLO.mLO = MavisLO(path, parametersFile, verbose=True)
 
 class TestReconstructor(TestMavisLO):
                     
     def test_reconstructor(self):
         """
         Test 
         """                
@@ -74,32 +74,23 @@
 
 class TestWindResiduals(TestMavisLO):
     def test_wind_residuals(self):
         """
         Test 
         """ 
         print("Running Test: TestWindResiduals")
-        NGS_flux = [10000, 30000, 5000]
+        NGS_flux = [2500, 7500 , 1250]
         NGS_SR_1650 = [0.4, 0.2, 0.6]
         NGS_FWHM_mas = [51.677, 81.673, 42.373]
         
         mItGPU = Integrator(cp, cp.float64, '')
-        r1 = TestMavisLO.mLO.computeBias(NGS_flux[0], NGS_SR_1650[0], NGS_FWHM_mas[0])
-        r2 = TestMavisLO.mLO.computeBias(NGS_flux[1], NGS_SR_1650[1], NGS_FWHM_mas[1])
-        r3 = TestMavisLO.mLO.computeBias(NGS_flux[2], NGS_SR_1650[2], NGS_FWHM_mas[2])
-
-        '''
-        self.assertTrue( np.testing.assert_allclose( np.asarray(r1), np.asarray((0.4592354532951008, (0.1148088633237752, 3.348938898539153e-17), (0.08617446983322877, 0.08617446983322877))), rtol=1e-03, atol=1e-5)==None)
-        self.assertTrue( np.testing.assert_allclose( np.asarray(r2), np.asarray( (0.43007711055063774, (0.10751927763765944, 2.0234128532071065e-17), (0.059932427347737786, 0.059932427347737786))), rtol=1e-03, atol=1e-5)==None)
-        self.assertTrue( np.testing.assert_allclose( np.asarray(r3), np.asarray((0.42097905807645625, (0.10524476451911406, 0.0), (0.10381564644797976, 0.10381564644797978))), rtol=1e-03, atol=1e-5)==None)
-        
-        self.assertTrue( np.testing.assert_allclose( np.asarray(r1), np.asarray((0.4592354532951008, (0.1148088633237752, 3.348938898539153e-17), (0.08617446983322877, 0.08617446983322877))), rtol=1e-03, atol=1e-5)==None)
-        self.assertTrue( np.testing.assert_allclose( np.asarray(r2), np.asarray( (0.43007711055063774, (0.10751927763765944, 2.0234128532071065e-17), (0.059932427347737786, 0.059932427347737786))), rtol=1e-03, atol=1e-5)==None)
-        self.assertTrue( np.testing.assert_allclose( np.asarray(r3), np.asarray((0.42097905807645625, (0.10524476451911406, 0.0), (0.10381564644797976, 0.10381564644797978))), rtol=1e-03, atol=1e-5)==None)
-        '''
+        r1 = TestMavisLO.mLO.computeBiasAndVariance(NGS_flux[0], NGS_SR_1650[0], NGS_FWHM_mas[0])
+        r2 = TestMavisLO.mLO.computeBiasAndVariance(NGS_flux[1], NGS_SR_1650[1], NGS_FWHM_mas[1])
+        r3 = TestMavisLO.mLO.computeBiasAndVariance(NGS_flux[2], NGS_SR_1650[2], NGS_FWHM_mas[2])
+
         self.assertTrue( np.testing.assert_allclose(np.array(r1[0]), np.array((0.4592354532951008)), rtol=1e-03, atol=1e-5)==None)
         self.assertTrue( np.testing.assert_allclose(np.array(r1[1]), np.array((0.1148088633237752, 3.348938898539153e-17)), rtol=1e-03, atol=1e-5)==None)
         self.assertTrue( np.testing.assert_allclose(np.array(r1[2]), np.array((0.08617446983322877, 0.08617446983322877)), rtol=1e-03, atol=1e-5)==None)
         self.assertTrue( np.testing.assert_allclose(np.array(r2[0]), np.array((0.43007711055063774)), rtol=1e-03, atol=1e-5)==None)
         self.assertTrue( np.testing.assert_allclose(np.array(r2[1]), np.array((0.10751927763765944, 2.0234128532071065e-17)), rtol=1e-03, atol=1e-5)==None)
         self.assertTrue( np.testing.assert_allclose(np.array(r2[2]), np.array((0.059932427347737786, 0.059932427347737786)), rtol=1e-03, atol=1e-5)==None)
         self.assertTrue( np.testing.assert_allclose(np.array(r3[0]), np.array((0.42097905807645625)), rtol=1e-03, atol=1e-5)==None)
```

