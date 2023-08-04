# Comparing `tmp/pyem_st_artifacts-1.0.1.post4.tar.gz` & `tmp/pyem_st_artifacts-1.0.1.post5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pyem_st_artifacts-1.0.1.post4.tar", last modified: Fri Jul 21 12:45:41 2023, max compression
+gzip compressed data, was "dist\pyem_st_artifacts-1.0.1.post5.tar", last modified: Fri Aug  4 12:50:25 2023, max compression
```

## Comparing `pyem_st_artifacts-1.0.1.post4.tar` & `pyem_st_artifacts-1.0.1.post5.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-07-21 12:45:41.000000 pyem_st_artifacts-1.0.1.post4/
--rw-rw-rw-   0        0        0     1090 2023-04-19 10:44:40.000000 pyem_st_artifacts-1.0.1.post4/LICENSE
--rw-rw-rw-   0        0        0     9699 2023-07-21 12:45:41.000000 pyem_st_artifacts-1.0.1.post4/PKG-INFO
--rw-rw-rw-   0        0        0     9145 2023-07-12 15:47:03.000000 pyem_st_artifacts-1.0.1.post4/README.md
-drwxrwxrwx   0        0        0        0 2023-07-21 12:45:41.000000 pyem_st_artifacts-1.0.1.post4/em_st_artifacts/
--rw-rw-rw-   0        0        0        0 2023-05-24 13:24:57.000000 pyem_st_artifacts-1.0.1.post4/em_st_artifacts/__init__.py
--rw-rw-rw-   0        0        0    24174 2023-07-21 12:39:50.000000 pyem_st_artifacts-1.0.1.post4/em_st_artifacts/emotional_math.py
-drwxrwxrwx   0        0        0        0 2023-07-21 12:45:41.000000 pyem_st_artifacts-1.0.1.post4/em_st_artifacts/libs/
-drwxrwxrwx   0        0        0        0 2023-07-21 12:45:41.000000 pyem_st_artifacts-1.0.1.post4/em_st_artifacts/libs/x64/
--rw-rw-rw-   0        0        0    73216 2023-05-24 13:24:57.000000 pyem_st_artifacts-1.0.1.post4/em_st_artifacts/libs/x64/artifacts-x64.dll
--rw-rw-rw-   0        0        0   174080 2023-06-07 09:52:32.000000 pyem_st_artifacts-1.0.1.post4/em_st_artifacts/libs/x64/em_st_artifacts-x64.dll
--rw-rw-rw-   0        0        0   320512 2023-02-09 11:55:16.000000 pyem_st_artifacts-1.0.1.post4/em_st_artifacts/libs/x64/filters.dll
-drwxrwxrwx   0        0        0        0 2023-07-21 12:45:41.000000 pyem_st_artifacts-1.0.1.post4/em_st_artifacts/libs/x86/
--rw-rw-rw-   0        0        0    56320 2023-05-24 13:24:57.000000 pyem_st_artifacts-1.0.1.post4/em_st_artifacts/libs/x86/artifacts-x86.dll
--rw-rw-rw-   0        0        0   133632 2023-06-07 09:53:04.000000 pyem_st_artifacts-1.0.1.post4/em_st_artifacts/libs/x86/em_st_artifacts-x86.dll
--rw-rw-rw-   0        0        0   268288 2023-02-09 11:55:16.000000 pyem_st_artifacts-1.0.1.post4/em_st_artifacts/libs/x86/filters.dll
--rw-rw-rw-   0        0        0     3448 2023-06-07 13:09:40.000000 pyem_st_artifacts-1.0.1.post4/em_st_artifacts/sample.py
-drwxrwxrwx   0        0        0        0 2023-07-21 12:45:41.000000 pyem_st_artifacts-1.0.1.post4/em_st_artifacts/utils/
--rw-rw-rw-   0        0        0      193 2023-05-24 13:24:57.000000 pyem_st_artifacts-1.0.1.post4/em_st_artifacts/utils/EmotionalMathException.py
--rw-rw-rw-   0        0        0        0 2023-05-24 13:24:57.000000 pyem_st_artifacts-1.0.1.post4/em_st_artifacts/utils/__init__.py
--rw-rw-rw-   0        0        0      945 2023-07-21 12:40:14.000000 pyem_st_artifacts-1.0.1.post4/em_st_artifacts/utils/lib_settings.py
--rw-rw-rw-   0        0        0      655 2023-06-06 13:59:02.000000 pyem_st_artifacts-1.0.1.post4/em_st_artifacts/utils/support_classes.py
-drwxrwxrwx   0        0        0        0 2023-07-21 12:45:41.000000 pyem_st_artifacts-1.0.1.post4/pyem_st_artifacts.egg-info/
--rw-rw-rw-   0        0        0     9699 2023-07-21 12:45:41.000000 pyem_st_artifacts-1.0.1.post4/pyem_st_artifacts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      697 2023-07-21 12:45:41.000000 pyem_st_artifacts-1.0.1.post4/pyem_st_artifacts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-21 12:45:41.000000 pyem_st_artifacts-1.0.1.post4/pyem_st_artifacts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-07-21 12:45:41.000000 pyem_st_artifacts-1.0.1.post4/pyem_st_artifacts.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-21 12:45:41.000000 pyem_st_artifacts-1.0.1.post4/setup.cfg
--rw-rw-rw-   0        0        0     1414 2023-07-21 12:41:12.000000 pyem_st_artifacts-1.0.1.post4/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-04 12:50:25.000000 pyem_st_artifacts-1.0.1.post5/
+-rw-rw-rw-   0        0        0     1090 2023-04-19 10:44:40.000000 pyem_st_artifacts-1.0.1.post5/LICENSE
+-rw-rw-rw-   0        0        0     9699 2023-08-04 12:50:25.000000 pyem_st_artifacts-1.0.1.post5/PKG-INFO
+-rw-rw-rw-   0        0        0     9145 2023-07-12 15:47:03.000000 pyem_st_artifacts-1.0.1.post5/README.md
+drwxrwxrwx   0        0        0        0 2023-08-04 12:50:25.000000 pyem_st_artifacts-1.0.1.post5/em_st_artifacts/
+-rw-rw-rw-   0        0        0        0 2023-05-24 13:24:57.000000 pyem_st_artifacts-1.0.1.post5/em_st_artifacts/__init__.py
+-rw-rw-rw-   0        0        0    24458 2023-08-04 12:41:48.000000 pyem_st_artifacts-1.0.1.post5/em_st_artifacts/emotional_math.py
+drwxrwxrwx   0        0        0        0 2023-08-04 12:50:25.000000 pyem_st_artifacts-1.0.1.post5/em_st_artifacts/libs/
+drwxrwxrwx   0        0        0        0 2023-08-04 12:50:25.000000 pyem_st_artifacts-1.0.1.post5/em_st_artifacts/libs/x64/
+-rw-rw-rw-   0        0        0    73216 2023-05-24 13:24:57.000000 pyem_st_artifacts-1.0.1.post5/em_st_artifacts/libs/x64/artifacts-x64.dll
+-rw-rw-rw-   0        0        0   174080 2023-06-07 09:52:32.000000 pyem_st_artifacts-1.0.1.post5/em_st_artifacts/libs/x64/em_st_artifacts-x64.dll
+-rw-rw-rw-   0        0        0   320512 2023-02-09 11:55:16.000000 pyem_st_artifacts-1.0.1.post5/em_st_artifacts/libs/x64/filters.dll
+drwxrwxrwx   0        0        0        0 2023-08-04 12:50:25.000000 pyem_st_artifacts-1.0.1.post5/em_st_artifacts/libs/x86/
+-rw-rw-rw-   0        0        0    56320 2023-05-24 13:24:57.000000 pyem_st_artifacts-1.0.1.post5/em_st_artifacts/libs/x86/artifacts-x86.dll
+-rw-rw-rw-   0        0        0   133632 2023-06-07 09:53:04.000000 pyem_st_artifacts-1.0.1.post5/em_st_artifacts/libs/x86/em_st_artifacts-x86.dll
+-rw-rw-rw-   0        0        0   268288 2023-02-09 11:55:16.000000 pyem_st_artifacts-1.0.1.post5/em_st_artifacts/libs/x86/filters.dll
+-rw-rw-rw-   0        0        0     3528 2023-08-04 12:36:52.000000 pyem_st_artifacts-1.0.1.post5/em_st_artifacts/sample.py
+drwxrwxrwx   0        0        0        0 2023-08-04 12:50:25.000000 pyem_st_artifacts-1.0.1.post5/em_st_artifacts/utils/
+-rw-rw-rw-   0        0        0      193 2023-05-24 13:24:57.000000 pyem_st_artifacts-1.0.1.post5/em_st_artifacts/utils/EmotionalMathException.py
+-rw-rw-rw-   0        0        0        0 2023-05-24 13:24:57.000000 pyem_st_artifacts-1.0.1.post5/em_st_artifacts/utils/__init__.py
+-rw-rw-rw-   0        0        0      945 2023-07-21 12:40:14.000000 pyem_st_artifacts-1.0.1.post5/em_st_artifacts/utils/lib_settings.py
+-rw-rw-rw-   0        0        0      655 2023-06-06 13:59:02.000000 pyem_st_artifacts-1.0.1.post5/em_st_artifacts/utils/support_classes.py
+drwxrwxrwx   0        0        0        0 2023-08-04 12:50:25.000000 pyem_st_artifacts-1.0.1.post5/pyem_st_artifacts.egg-info/
+-rw-rw-rw-   0        0        0     9699 2023-08-04 12:50:24.000000 pyem_st_artifacts-1.0.1.post5/pyem_st_artifacts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      697 2023-08-04 12:50:24.000000 pyem_st_artifacts-1.0.1.post5/pyem_st_artifacts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-04 12:50:24.000000 pyem_st_artifacts-1.0.1.post5/pyem_st_artifacts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-08-04 12:50:24.000000 pyem_st_artifacts-1.0.1.post5/pyem_st_artifacts.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-04 12:50:25.000000 pyem_st_artifacts-1.0.1.post5/setup.cfg
+-rw-rw-rw-   0        0        0     1414 2023-08-04 12:50:11.000000 pyem_st_artifacts-1.0.1.post5/setup.py
```

### Comparing `pyem_st_artifacts-1.0.1.post4/LICENSE` & `pyem_st_artifacts-1.0.1.post5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyem_st_artifacts-1.0.1.post4/PKG-INFO` & `pyem_st_artifacts-1.0.1.post5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyem_st_artifacts
-Version: 1.0.1.post4
+Version: 1.0.1.post5
 Summary: Python wrapper for Emotions library
 Home-page: https://gitlab.com/neurosdk2/neurosamples/-/tree/main/python
 Author: Brainbit Inc.
 Author-email: support@brainbit.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyem_st_artifacts-1.0.1.post4/README.md` & `pyem_st_artifacts-1.0.1.post5/README.md`

 * *Files identical despite different names*

### Comparing `pyem_st_artifacts-1.0.1.post4/em_st_artifacts/emotional_math.py` & `pyem_st_artifacts-1.0.1.post5/em_st_artifacts/emotional_math.py`

 * *Files 1% similar despite different names*

```diff
@@ -273,17 +273,18 @@
     def set_skip_wins_after_artifact(self, nwins: int):
         op_status = self._NativeOpStatus()
         self._set_skip_wins_after_artifact(self._native_ptr, nwins, ctypes.byref(op_status))
         self._check_error(op_status)
 
     def push_data(self, samples: List[RawChannels]):
         op_status = self._NativeOpStatus()
+        raw_ch_len = len(samples)
         self._push_data(self._native_ptr,
-                        (self._NativeRawChannels * len(samples))(*samples),
-                        len(samples),
+                        (self._NativeRawChannels * raw_ch_len)(*[self._NativeRawChannels(samples[i].left_bipolar, samples[i].right_bipolar) for i in range(raw_ch_len)]),
+                        raw_ch_len,
                         ctypes.byref(op_status))
         self._check_error(op_status)
 
     def push_data_arr(self, samples: List[RawChannelsArray]):
         native_list = []
 
         for x in samples:
@@ -370,17 +371,17 @@
     def read_mental_data_arr(self) -> List[MindData]:
         arr_size = self.read_mental_data_arr_size()
 
         if arr_size == 0:
             return []
 
         native_result = (self._NativeMindData * arr_size)()
-
+        native_arr_size = ctypes.c_int(arr_size)
         op_status = self._NativeOpStatus()
-        self._read_mental_data_arr(self._native_ptr, native_result, arr_size, ctypes.byref(op_status))
+        self._read_mental_data_arr(self._native_ptr, native_result, ctypes.byref(native_arr_size), ctypes.byref(op_status))
         self._check_error(op_status)
 
         return [MindData(x.Rel_Attention, x.Rel_Relaxation, x.Inst_Attention, x.Inst_Relaxation) for x in native_result]
 
     def read_average_mental_data(self, n_last_wins_to_average: int) -> MindData:
         native_result = self._NativeMindData()
 
@@ -408,17 +409,17 @@
     def read_spectral_data_percents_arr(self) -> List[SpectralDataPercents]:
         arr_size = self.read_spectral_data_percents_arr_size()
 
         if arr_size == 0:
             return []
 
         native_result = (self._NativeSpectralDataPercents * arr_size)()
-
+        native_arr_size = ctypes.c_int(arr_size)
         op_status = self._NativeOpStatus()
-        self._read_spectral_data_percents_arr(self._native_ptr, native_result, arr_size, ctypes.byref(op_status))
+        self._read_spectral_data_percents_arr(self._native_ptr, native_result, ctypes.byref(native_arr_size), ctypes.byref(op_status))
         self._check_error(op_status)
 
         return [SpectralDataPercents(x.Delta, x.Theta, x.Alpha, x.Beta, x.Gamma) for x in native_result]
 
     def read_raw_spectral_vals(self) -> RawSpectVals:
         native_result = self._NativeRawSpectVals()
 
@@ -462,15 +463,15 @@
         self._check_error(op_status)
 
         return result.value
 
     @staticmethod
     def _check_error(op_status: _NativeOpStatus):
         if not op_status.Success:
-            error_msg = "".join([op_status.ErrorMsg[x] for x in range(512)])
+            error_msg = op_status.ErrorMsg#"".join([op_status.ErrorMsg[x] for x in range(512)])
             raise EmotionalMathException(error_msg)
 
     def __del__(self):
         if self._native_ptr is None:
             op_status = self._NativeOpStatus()
 
             self._free_math_lib(self._native_ptr, ctypes.byref(op_status))
```

### Comparing `pyem_st_artifacts-1.0.1.post4/em_st_artifacts/libs/x64/artifacts-x64.dll` & `pyem_st_artifacts-1.0.1.post5/em_st_artifacts/libs/x64/artifacts-x64.dll`

 * *Files identical despite different names*

### Comparing `pyem_st_artifacts-1.0.1.post4/em_st_artifacts/libs/x64/em_st_artifacts-x64.dll` & `pyem_st_artifacts-1.0.1.post5/em_st_artifacts/libs/x64/em_st_artifacts-x64.dll`

 * *Files identical despite different names*

### Comparing `pyem_st_artifacts-1.0.1.post4/em_st_artifacts/libs/x64/filters.dll` & `pyem_st_artifacts-1.0.1.post5/em_st_artifacts/libs/x64/filters.dll`

 * *Files identical despite different names*

### Comparing `pyem_st_artifacts-1.0.1.post4/em_st_artifacts/libs/x86/artifacts-x86.dll` & `pyem_st_artifacts-1.0.1.post5/em_st_artifacts/libs/x86/artifacts-x86.dll`

 * *Files identical despite different names*

### Comparing `pyem_st_artifacts-1.0.1.post4/em_st_artifacts/libs/x86/em_st_artifacts-x86.dll` & `pyem_st_artifacts-1.0.1.post5/em_st_artifacts/libs/x86/em_st_artifacts-x86.dll`

 * *Files identical despite different names*

### Comparing `pyem_st_artifacts-1.0.1.post4/em_st_artifacts/libs/x86/filters.dll` & `pyem_st_artifacts-1.0.1.post5/em_st_artifacts/libs/x86/filters.dll`

 * *Files identical despite different names*

### Comparing `pyem_st_artifacts-1.0.1.post4/em_st_artifacts/sample.py` & `pyem_st_artifacts-1.0.1.post5/em_st_artifacts/sample.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 import math
 
-from em_st_artifactslib import (ArtifactDetectSetting, EmotionalMath, MathLibSetting, MentalAndSpectralSetting,
-                                RawChannelsArray, ShortArtifactDetectSetting, )
+from em_st_artifacts.utils.support_classes import RawChannelsArray, RawChannels
+
+from em_st_artifacts.emotional_math import EmotionalMath
+
+from em_st_artifacts.utils.lib_settings import MathLibSetting, ArtifactDetectSetting, ShortArtifactDetectSetting, \
+    MentalAndSpectralSetting
 
 current_sin_step = 0
 
 
 def get_sin_wave_sample(sample_rate: int, hz: int, step: int):
     return 50 * math.sin(hz * step * (2 * math.pi / sample_rate))
 
@@ -26,15 +30,15 @@
     calibration_length = 8
     nwins_skip_after_artifact = 10
 
     mls = MathLibSetting(sampling_rate=250,
                          process_win_freq=25,
                          fft_window=1000,
                          n_first_sec_skipped=4,
-                         bipolar_mode=False,
+                         bipolar_mode=True,
                          channels_number=4,
                          channel_for_analysis=3)
 
     ads = ArtifactDetectSetting(hanning_win_spectrum=True, num_wins_for_quality_avg=125)
 
     sads = ShortArtifactDetectSetting(ampl_art_extremum_border=25)
 
@@ -48,17 +52,17 @@
     emotions.set_spect_normalization_by_bands_width(True)
 
     size = 1500
     while True:
         raw_channels_list = []
 
         for _ in range(size):
-            raw_channels_list.append(RawChannelsArray(get_sin(4)))
+            raw_channels_list.append(RawChannels(3, 1))
 
-        emotions.push_data_arr(raw_channels_list)
+        emotions.push_data(raw_channels_list)
         emotions.process_data_arr()
 
         mind_data_list = emotions.read_mental_data_arr()
         mind_data = emotions.read_average_mental_data(1)
         raw_spect_vals = emotions.read_raw_spectral_vals()
         percents = emotions.read_spectral_data_percents_arr()
         if emotions.is_both_sides_artifacted():
```

### Comparing `pyem_st_artifacts-1.0.1.post4/em_st_artifacts/utils/lib_settings.py` & `pyem_st_artifacts-1.0.1.post5/em_st_artifacts/utils/lib_settings.py`

 * *Files identical despite different names*

### Comparing `pyem_st_artifacts-1.0.1.post4/em_st_artifacts/utils/support_classes.py` & `pyem_st_artifacts-1.0.1.post5/em_st_artifacts/utils/support_classes.py`

 * *Files identical despite different names*

### Comparing `pyem_st_artifacts-1.0.1.post4/pyem_st_artifacts.egg-info/PKG-INFO` & `pyem_st_artifacts-1.0.1.post5/pyem_st_artifacts.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyem-st-artifacts
-Version: 1.0.1.post4
+Version: 1.0.1.post5
 Summary: Python wrapper for Emotions library
 Home-page: https://gitlab.com/neurosdk2/neurosamples/-/tree/main/python
 Author: Brainbit Inc.
 Author-email: support@brainbit.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyem_st_artifacts-1.0.1.post4/pyem_st_artifacts.egg-info/SOURCES.txt` & `pyem_st_artifacts-1.0.1.post5/pyem_st_artifacts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyem_st_artifacts-1.0.1.post4/setup.py` & `pyem_st_artifacts-1.0.1.post5/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='pyem_st_artifacts',
-    version='1.0.1.post4',
+    version='1.0.1.post5',
     py_modules=[
         'em_st_artifacts.emotional_math',
         'em_st_artifacts.utils.lib_settings',
         'em_st_artifacts.utils.support_classes',
         'em_st_artifacts.utils.EmotionalMathException'],
     packages=['em_st_artifacts'],
     url='https://gitlab.com/neurosdk2/neurosamples/-/tree/main/python',
```

