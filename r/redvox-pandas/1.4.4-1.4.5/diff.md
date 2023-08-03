# Comparing `tmp/redvox-pandas-1.4.4.tar.gz` & `tmp/redvox-pandas-1.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redvox-pandas-1.4.4.tar", last modified: Tue Aug  1 19:56:54 2023, max compression
+gzip compressed data, was "redvox-pandas-1.4.5.tar", last modified: Thu Aug  3 22:48:48 2023, max compression
```

## Comparing `redvox-pandas-1.4.4.tar` & `redvox-pandas-1.4.5.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-08-01 19:56:54.350568 redvox-pandas-1.4.4/
--rw-rw-r--   0 opq       (1000) opq       (1000)    11359 2021-07-02 00:27:05.000000 redvox-pandas-1.4.4/LICENSE
--rw-r--r--   0 opq       (1000) opq       (1000)    15648 2023-08-01 19:56:54.350568 redvox-pandas-1.4.4/PKG-INFO
--rw-r--r--   0 opq       (1000) opq       (1000)     2266 2023-04-27 21:26:24.000000 redvox-pandas-1.4.4/README.md
--rw-r--r--   0 opq       (1000) opq       (1000)      910 2023-08-01 19:55:46.000000 redvox-pandas-1.4.4/pyproject.toml
-drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-08-01 19:56:54.349568 redvox-pandas-1.4.4/redpandas/
--rw-rw-r--   0 opq       (1000) opq       (1000)      305 2022-07-07 20:44:53.000000 redvox-pandas-1.4.4/redpandas/__init__.py
--rw-r--r--   0 opq       (1000) opq       (1000)    19300 2023-04-27 21:26:25.000000 redvox-pandas-1.4.4/redpandas/redpd_build_station.py
--rw-rw-r--   0 opq       (1000) opq       (1000)    15456 2022-07-07 20:44:53.000000 redvox-pandas-1.4.4/redpandas/redpd_cohere.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     6751 2021-08-03 22:13:07.000000 redvox-pandas-1.4.4/redpandas/redpd_config.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     4051 2022-07-07 20:44:53.000000 redvox-pandas-1.4.4/redpandas/redpd_datawin.py
--rw-r--r--   0 opq       (1000) opq       (1000)     4981 2023-04-27 21:26:25.000000 redvox-pandas-1.4.4/redpandas/redpd_df.py
--rw-rw-r--   0 opq       (1000) opq       (1000)    14773 2022-07-07 20:44:53.000000 redvox-pandas-1.4.4/redpandas/redpd_dq.py
--rw-rw-r--   0 opq       (1000) opq       (1000)    16853 2021-08-03 22:13:07.000000 redvox-pandas-1.4.4/redpandas/redpd_ensonify.py
--rw-rw-r--   0 opq       (1000) opq       (1000)      403 2021-10-18 19:57:34.000000 redvox-pandas-1.4.4/redpandas/redpd_errors.py
--rw-rw-r--   0 opq       (1000) opq       (1000)    26898 2021-10-18 19:57:34.000000 redvox-pandas-1.4.4/redpandas/redpd_filter.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     8524 2022-07-07 20:44:53.000000 redvox-pandas-1.4.4/redpandas/redpd_geospatial.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     4200 2022-07-07 20:44:53.000000 redvox-pandas-1.4.4/redpandas/redpd_gravity.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     3790 2022-07-07 20:44:53.000000 redvox-pandas-1.4.4/redpandas/redpd_iterator.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     7874 2022-07-07 20:44:53.000000 redvox-pandas-1.4.4/redpandas/redpd_orientation.py
-drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-08-01 19:56:54.350568 redvox-pandas-1.4.4/redpandas/redpd_plot/
--rw-rw-r--   0 opq       (1000) opq       (1000)        0 2021-08-03 22:13:07.000000 redvox-pandas-1.4.4/redpandas/redpd_plot/__init__.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     4423 2021-08-03 22:13:07.000000 redvox-pandas-1.4.4/redpandas/redpd_plot/coherence.py
--rw-r--r--   0 opq       (1000) opq       (1000)    33263 2023-04-27 21:26:25.000000 redvox-pandas-1.4.4/redpandas/redpd_plot/mesh.py
--rw-rw-r--   0 opq       (1000) opq       (1000)      467 2021-10-18 19:57:34.000000 redvox-pandas-1.4.4/redpandas/redpd_plot/parameters.py
--rw-r--r--   0 opq       (1000) opq       (1000)    35442 2023-04-27 21:26:25.000000 redvox-pandas-1.4.4/redpandas/redpd_plot/wiggles.py
--rw-r--r--   0 opq       (1000) opq       (1000)    15627 2023-04-27 21:26:25.000000 redvox-pandas-1.4.4/redpandas/redpd_preprocess.py
--rw-r--r--   0 opq       (1000) opq       (1000)     8703 2023-04-27 21:26:25.000000 redvox-pandas-1.4.4/redpandas/redpd_report.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     1482 2022-07-07 20:44:53.000000 redvox-pandas-1.4.4/redpandas/redpd_scales.py
--rw-rw-r--   0 opq       (1000) opq       (1000)       80 2022-07-07 20:44:53.000000 redvox-pandas-1.4.4/redpandas/redpd_state.py
--rw-r--r--   0 opq       (1000) opq       (1000)    15899 2023-04-27 21:26:25.000000 redvox-pandas-1.4.4/redpandas/redpd_tfr.py
--rw-rw-r--   0 opq       (1000) opq       (1000)    21018 2022-07-07 20:44:53.000000 redvox-pandas-1.4.4/redpandas/redpd_xcorr.py
-drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-08-01 19:56:54.350568 redvox-pandas-1.4.4/redvox_pandas.egg-info/
--rw-rw-r--   0 opq       (1000) opq       (1000)    15648 2023-08-01 19:56:54.000000 redvox-pandas-1.4.4/redvox_pandas.egg-info/PKG-INFO
--rw-rw-r--   0 opq       (1000) opq       (1000)      908 2023-08-01 19:56:54.000000 redvox-pandas-1.4.4/redvox_pandas.egg-info/SOURCES.txt
--rw-rw-r--   0 opq       (1000) opq       (1000)        1 2023-08-01 19:56:54.000000 redvox-pandas-1.4.4/redvox_pandas.egg-info/dependency_links.txt
--rw-rw-r--   0 opq       (1000) opq       (1000)      102 2023-08-01 19:56:54.000000 redvox-pandas-1.4.4/redvox_pandas.egg-info/requires.txt
--rw-rw-r--   0 opq       (1000) opq       (1000)       10 2023-08-01 19:56:54.000000 redvox-pandas-1.4.4/redvox_pandas.egg-info/top_level.txt
--rw-r--r--   0 opq       (1000) opq       (1000)       38 2023-08-01 19:56:54.351568 redvox-pandas-1.4.4/setup.cfg
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-08-03 22:48:48.177967 redvox-pandas-1.4.5/
+-rw-r--r--   0 tyler      (501) staff       (20)    11359 2021-07-07 01:00:28.000000 redvox-pandas-1.4.5/LICENSE
+-rw-r--r--   0 tyler      (501) staff       (20)    15648 2023-08-03 22:48:48.177332 redvox-pandas-1.4.5/PKG-INFO
+-rw-r--r--   0 tyler      (501) staff       (20)     2266 2023-06-21 00:46:50.000000 redvox-pandas-1.4.5/README.md
+-rw-r--r--   0 tyler      (501) staff       (20)      910 2023-08-03 22:42:03.000000 redvox-pandas-1.4.5/pyproject.toml
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-08-03 22:48:48.168479 redvox-pandas-1.4.5/redpandas/
+-rw-r--r--   0 tyler      (501) staff       (20)      305 2022-03-22 17:51:29.000000 redvox-pandas-1.4.5/redpandas/__init__.py
+-rw-r--r--   0 tyler      (501) staff       (20)    19300 2023-06-21 00:46:50.000000 redvox-pandas-1.4.5/redpandas/redpd_build_station.py
+-rw-r--r--   0 tyler      (501) staff       (20)    15456 2022-03-22 17:51:29.000000 redvox-pandas-1.4.5/redpandas/redpd_cohere.py
+-rw-r--r--   0 tyler      (501) staff       (20)     6751 2021-09-07 22:36:58.000000 redvox-pandas-1.4.5/redpandas/redpd_config.py
+-rw-r--r--   0 tyler      (501) staff       (20)     4051 2023-08-03 22:42:35.000000 redvox-pandas-1.4.5/redpandas/redpd_datawin.py
+-rw-r--r--   0 tyler      (501) staff       (20)     4980 2023-08-03 21:54:26.000000 redvox-pandas-1.4.5/redpandas/redpd_df.py
+-rw-r--r--   0 tyler      (501) staff       (20)    14773 2021-12-09 21:13:47.000000 redvox-pandas-1.4.5/redpandas/redpd_dq.py
+-rw-r--r--   0 tyler      (501) staff       (20)    16853 2021-08-03 22:10:02.000000 redvox-pandas-1.4.5/redpandas/redpd_ensonify.py
+-rw-r--r--   0 tyler      (501) staff       (20)      403 2021-09-03 01:25:44.000000 redvox-pandas-1.4.5/redpandas/redpd_errors.py
+-rw-r--r--   0 tyler      (501) staff       (20)    26898 2021-12-08 01:10:31.000000 redvox-pandas-1.4.5/redpandas/redpd_filter.py
+-rw-r--r--   0 tyler      (501) staff       (20)     8524 2022-03-22 17:51:29.000000 redvox-pandas-1.4.5/redpandas/redpd_geospatial.py
+-rw-r--r--   0 tyler      (501) staff       (20)     4200 2022-03-22 17:51:29.000000 redvox-pandas-1.4.5/redpandas/redpd_gravity.py
+-rw-r--r--   0 tyler      (501) staff       (20)     3790 2022-03-22 17:51:29.000000 redvox-pandas-1.4.5/redpandas/redpd_iterator.py
+-rw-r--r--   0 tyler      (501) staff       (20)     7874 2022-03-22 17:51:29.000000 redvox-pandas-1.4.5/redpandas/redpd_orientation.py
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-08-03 22:48:48.173285 redvox-pandas-1.4.5/redpandas/redpd_plot/
+-rw-r--r--   0 tyler      (501) staff       (20)        0 2021-08-03 22:10:02.000000 redvox-pandas-1.4.5/redpandas/redpd_plot/__init__.py
+-rw-r--r--   0 tyler      (501) staff       (20)     4423 2021-08-03 22:10:02.000000 redvox-pandas-1.4.5/redpandas/redpd_plot/coherence.py
+-rw-r--r--   0 tyler      (501) staff       (20)    33263 2023-06-21 00:46:50.000000 redvox-pandas-1.4.5/redpandas/redpd_plot/mesh.py
+-rw-r--r--   0 tyler      (501) staff       (20)      467 2021-12-08 01:10:31.000000 redvox-pandas-1.4.5/redpandas/redpd_plot/parameters.py
+-rw-r--r--   0 tyler      (501) staff       (20)    35442 2023-06-21 00:46:50.000000 redvox-pandas-1.4.5/redpandas/redpd_plot/wiggles.py
+-rw-r--r--   0 tyler      (501) staff       (20)    15627 2023-06-21 00:46:50.000000 redvox-pandas-1.4.5/redpandas/redpd_preprocess.py
+-rw-r--r--   0 tyler      (501) staff       (20)     8703 2023-06-21 00:46:50.000000 redvox-pandas-1.4.5/redpandas/redpd_report.py
+-rw-r--r--   0 tyler      (501) staff       (20)     1482 2022-03-22 17:51:29.000000 redvox-pandas-1.4.5/redpandas/redpd_scales.py
+-rw-r--r--   0 tyler      (501) staff       (20)       80 2022-03-22 17:51:29.000000 redvox-pandas-1.4.5/redpandas/redpd_state.py
+-rw-r--r--   0 tyler      (501) staff       (20)    15899 2023-06-21 00:46:50.000000 redvox-pandas-1.4.5/redpandas/redpd_tfr.py
+-rw-r--r--   0 tyler      (501) staff       (20)    21018 2022-03-22 17:51:29.000000 redvox-pandas-1.4.5/redpandas/redpd_xcorr.py
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-08-03 22:48:48.176595 redvox-pandas-1.4.5/redvox_pandas.egg-info/
+-rw-r--r--   0 tyler      (501) staff       (20)    15648 2023-08-03 22:48:48.000000 redvox-pandas-1.4.5/redvox_pandas.egg-info/PKG-INFO
+-rw-r--r--   0 tyler      (501) staff       (20)      908 2023-08-03 22:48:48.000000 redvox-pandas-1.4.5/redvox_pandas.egg-info/SOURCES.txt
+-rw-r--r--   0 tyler      (501) staff       (20)        1 2023-08-03 22:48:48.000000 redvox-pandas-1.4.5/redvox_pandas.egg-info/dependency_links.txt
+-rw-r--r--   0 tyler      (501) staff       (20)      102 2023-08-03 22:48:48.000000 redvox-pandas-1.4.5/redvox_pandas.egg-info/requires.txt
+-rw-r--r--   0 tyler      (501) staff       (20)       10 2023-08-03 22:48:48.000000 redvox-pandas-1.4.5/redvox_pandas.egg-info/top_level.txt
+-rw-r--r--   0 tyler      (501) staff       (20)       38 2023-08-03 22:48:48.178146 redvox-pandas-1.4.5/setup.cfg
```

### Comparing `redvox-pandas-1.4.4/LICENSE` & `redvox-pandas-1.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `redvox-pandas-1.4.4/PKG-INFO` & `redvox-pandas-1.4.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redvox-pandas
-Version: 1.4.4
+Version: 1.4.5
 Summary: Library to streamline preprocessing of RedVox API 900 and API 1000 data
 Author-email: "RedVox, Inc" <support@redvox.io>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `redvox-pandas-1.4.4/README.md` & `redvox-pandas-1.4.5/README.md`

 * *Files identical despite different names*

### Comparing `redvox-pandas-1.4.4/pyproject.toml` & `redvox-pandas-1.4.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 # See:
 # - https://setuptools.pypa.io/en/latest/userguide/pyproject_config.html
 # - https://packaging.python.org/en/latest/specifications/declaring-project-metadata/
 
 [project]
 name = "redvox-pandas"
-version = "1.4.4"
+version = "1.4.5"
 authors = [
     { name = "RedVox, Inc", email = "support@redvox.io" }
 ]
 description = "Library to streamline preprocessing of RedVox API 900 and API 1000 data"
 readme = "README.md"
 requires-python = ">=3.8"
 license = { file = "LICENSE" }
 
 dependencies = [
     "matplotlib==3.7.1",
     "numpy==1.23.5",
     "obspy==1.4.0",
     "pandas==2.0.1",
     "pymap3d==3.0.1",
-    "redvox==3.5.2",
+    "redvox==3.6.0",
     "scipy==1.10.1",
 ]
 
 [project.urls]
 homepage = "https://github.com/RedVoxInc/redpandas"
 PyPI = "https://pypi.org/project/redpandas/"
```

### Comparing `redvox-pandas-1.4.4/redpandas/redpd_build_station.py` & `redvox-pandas-1.4.5/redpandas/redpd_build_station.py`

 * *Files identical despite different names*

### Comparing `redvox-pandas-1.4.4/redpandas/redpd_cohere.py` & `redvox-pandas-1.4.5/redpandas/redpd_cohere.py`

 * *Files identical despite different names*

### Comparing `redvox-pandas-1.4.4/redpandas/redpd_config.py` & `redvox-pandas-1.4.5/redpandas/redpd_config.py`

 * *Files identical despite different names*

### Comparing `redvox-pandas-1.4.4/redpandas/redpd_datawin.py` & `redvox-pandas-1.4.5/redpandas/redpd_datawin.py`

 * *Files identical despite different names*

### Comparing `redvox-pandas-1.4.4/redpandas/redpd_df.py` & `redvox-pandas-1.4.5/redpandas/redpd_df.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,28 +10,28 @@
 import pandas as pd
 from redvox.common.data_window import DataWindow
 import redpandas.redpd_build_station as rpd_build_sta
 import redpandas.redpd_scales as rpd_scales
 
 
 def redpd_dataframe(input_dw: DataWindow,
-                    sensor_labels: Optional[List[str]] = ["audio"],
+                    sensor_labels: Optional[List[str]] = None,
                     highpass_type: Optional[str] = 'obspy',
                     frequency_filter_low: Optional[float] = 1./rpd_scales.Slice.T100S,
                     filter_order: Optional[int] = 4) -> pd.DataFrame:
     """
     Construct pandas dataframe from RedVox DataWindow. Default sensor extracted is audio, for more options see
     sensor_labels parameter.
 
     :param input_dw: REQUIRED. Redvox DataWindow
     :param sensor_labels: optional list of strings, list of sensors available ['audio', 'barometer', 'accelerometer',
         'gyroscope', 'magnetometer', 'health', 'location', 'synchronization', 'clock', 'best_location']. For example:
         sensor_labels = ['audio', 'accelerometer']. Default is ["audio"]
     :param highpass_type: optional string, type of highpass applied. One of: 'obspy', 'butter', or 'rc'.
-    Default is 'obspy'
+        Default is 'obspy'
     :param frequency_filter_low: optional float, lowest frequency for highpass filter. Default is 100 second periods
     :param filter_order: optional integer, the order of the filter. Default is 4
 
     :return: pd.DataFrame
     """
     # TODO: make debug/verbose option
     print("Initiating conversion from RedVox DataWindow to RedPandas:")
```

### Comparing `redvox-pandas-1.4.4/redpandas/redpd_dq.py` & `redvox-pandas-1.4.5/redpandas/redpd_dq.py`

 * *Files identical despite different names*

### Comparing `redvox-pandas-1.4.4/redpandas/redpd_ensonify.py` & `redvox-pandas-1.4.5/redpandas/redpd_ensonify.py`

 * *Files identical despite different names*

### Comparing `redvox-pandas-1.4.4/redpandas/redpd_filter.py` & `redvox-pandas-1.4.5/redpandas/redpd_filter.py`

 * *Files identical despite different names*

### Comparing `redvox-pandas-1.4.4/redpandas/redpd_geospatial.py` & `redvox-pandas-1.4.5/redpandas/redpd_geospatial.py`

 * *Files identical despite different names*

### Comparing `redvox-pandas-1.4.4/redpandas/redpd_gravity.py` & `redvox-pandas-1.4.5/redpandas/redpd_gravity.py`

 * *Files identical despite different names*

### Comparing `redvox-pandas-1.4.4/redpandas/redpd_iterator.py` & `redvox-pandas-1.4.5/redpandas/redpd_iterator.py`

 * *Files identical despite different names*

### Comparing `redvox-pandas-1.4.4/redpandas/redpd_orientation.py` & `redvox-pandas-1.4.5/redpandas/redpd_orientation.py`

 * *Files identical despite different names*

### Comparing `redvox-pandas-1.4.4/redpandas/redpd_plot/coherence.py` & `redvox-pandas-1.4.5/redpandas/redpd_plot/coherence.py`

 * *Files identical despite different names*

### Comparing `redvox-pandas-1.4.4/redpandas/redpd_plot/mesh.py` & `redvox-pandas-1.4.5/redpandas/redpd_plot/mesh.py`

 * *Files identical despite different names*

### Comparing `redvox-pandas-1.4.4/redpandas/redpd_plot/wiggles.py` & `redvox-pandas-1.4.5/redpandas/redpd_plot/wiggles.py`

 * *Files identical despite different names*

### Comparing `redvox-pandas-1.4.4/redpandas/redpd_preprocess.py` & `redvox-pandas-1.4.5/redpandas/redpd_preprocess.py`

 * *Files identical despite different names*

### Comparing `redvox-pandas-1.4.4/redpandas/redpd_report.py` & `redvox-pandas-1.4.5/redpandas/redpd_report.py`

 * *Files identical despite different names*

### Comparing `redvox-pandas-1.4.4/redpandas/redpd_scales.py` & `redvox-pandas-1.4.5/redpandas/redpd_scales.py`

 * *Files identical despite different names*

### Comparing `redvox-pandas-1.4.4/redpandas/redpd_tfr.py` & `redvox-pandas-1.4.5/redpandas/redpd_tfr.py`

 * *Files identical despite different names*

### Comparing `redvox-pandas-1.4.4/redpandas/redpd_xcorr.py` & `redvox-pandas-1.4.5/redpandas/redpd_xcorr.py`

 * *Files identical despite different names*

### Comparing `redvox-pandas-1.4.4/redvox_pandas.egg-info/PKG-INFO` & `redvox-pandas-1.4.5/redvox_pandas.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redvox-pandas
-Version: 1.4.4
+Version: 1.4.5
 Summary: Library to streamline preprocessing of RedVox API 900 and API 1000 data
 Author-email: "RedVox, Inc" <support@redvox.io>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `redvox-pandas-1.4.4/redvox_pandas.egg-info/SOURCES.txt` & `redvox-pandas-1.4.5/redvox_pandas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

