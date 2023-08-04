# Comparing `tmp/cybotrade_indicators-0.0.3.tar.gz` & `tmp/cybotrade-indicators-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cybotrade-indicators-0.0.3.tar", last modified: Wed Jul 26 03:01:12 2023, max compression
+gzip compressed data, was "cybotrade-indicators-0.0.4.tar", last modified: Fri Aug  4 09:44:40 2023, max compression
```

## Comparing `cybotrade_indicators-0.0.3.tar` & `cybotrade-indicators-0.0.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 marcus     (501) staff       (20)        0 2023-07-26 03:01:12.230521 cybotrade-indicators-0.0.3/
--rw-r--r--   0 marcus     (501) staff       (20)      433 2023-07-25 20:08:51.000000 cybotrade-indicators-0.0.3/AUTHORS
--rw-r--r--   0 marcus     (501) staff       (20)     7650 2023-07-25 20:08:38.000000 cybotrade-indicators-0.0.3/LICENSE
--rw-r--r--   0 marcus     (501) staff       (20)      238 2023-07-26 03:00:01.000000 cybotrade-indicators-0.0.3/MANIFEST.in
--rw-r--r--   0 marcus     (501) staff       (20)     3493 2023-07-26 03:01:12.230386 cybotrade-indicators-0.0.3/PKG-INFO
--rw-r--r--   0 marcus     (501) staff       (20)     2818 2023-07-25 20:06:26.000000 cybotrade-indicators-0.0.3/README.md
-drwxr-xr-x   0 marcus     (501) staff       (20)        0 2023-07-26 03:01:12.221196 cybotrade-indicators-0.0.3/external/
--rw-r--r--   0 marcus     (501) staff       (20)    53547 2023-07-25 10:32:29.000000 cybotrade-indicators-0.0.3/external/indicators.h
--rw-r--r--   0 marcus     (501) staff       (20)   419800 2023-07-25 10:32:24.000000 cybotrade-indicators-0.0.3/external/tiamalgamation.c
--rw-r--r--   0 marcus     (501) staff       (20)      920 2023-07-26 03:01:07.000000 cybotrade-indicators-0.0.3/pyproject.toml
--rw-r--r--   0 marcus     (501) staff       (20)       38 2023-07-26 03:01:12.230574 cybotrade-indicators-0.0.3/setup.cfg
--rw-r--r--   0 marcus     (501) staff       (20)      370 2023-07-25 19:18:28.000000 cybotrade-indicators-0.0.3/setup.py
-drwxr-xr-x   0 marcus     (501) staff       (20)        0 2023-07-26 03:01:12.219386 cybotrade-indicators-0.0.3/src/
-drwxr-xr-x   0 marcus     (501) staff       (20)        0 2023-07-26 03:01:12.228563 cybotrade-indicators-0.0.3/src/cybotrade_indicators/
--rw-r--r--   0 marcus     (501) staff       (20)  4146314 2023-07-26 02:34:36.000000 cybotrade-indicators-0.0.3/src/cybotrade_indicators/__init__.c
--rw-r--r--   0 marcus     (501) staff       (20)    24376 2023-07-25 19:55:33.000000 cybotrade-indicators-0.0.3/src/cybotrade_indicators/__init__.pyi
--rw-r--r--   0 marcus     (501) staff       (20)    56715 2023-07-25 19:55:33.000000 cybotrade-indicators-0.0.3/src/cybotrade_indicators/__init__.pyx
--rw-r--r--   0 marcus     (501) staff       (20)     1817 2023-07-25 19:17:58.000000 cybotrade-indicators-0.0.3/src/cybotrade_indicators/indicators.pxd
--rw-r--r--   0 marcus     (501) staff       (20)        0 2023-07-25 20:15:15.000000 cybotrade-indicators-0.0.3/src/cybotrade_indicators/py.typed
-drwxr-xr-x   0 marcus     (501) staff       (20)        0 2023-07-26 03:01:12.229211 cybotrade-indicators-0.0.3/src/cybotrade_indicators.egg-info/
--rw-r--r--   0 marcus     (501) staff       (20)     3493 2023-07-26 03:01:12.000000 cybotrade-indicators-0.0.3/src/cybotrade_indicators.egg-info/PKG-INFO
--rw-r--r--   0 marcus     (501) staff       (20)      548 2023-07-26 03:01:12.000000 cybotrade-indicators-0.0.3/src/cybotrade_indicators.egg-info/SOURCES.txt
--rw-r--r--   0 marcus     (501) staff       (20)        1 2023-07-26 03:01:12.000000 cybotrade-indicators-0.0.3/src/cybotrade_indicators.egg-info/dependency_links.txt
--rw-r--r--   0 marcus     (501) staff       (20)       30 2023-07-26 03:01:12.000000 cybotrade-indicators-0.0.3/src/cybotrade_indicators.egg-info/requires.txt
--rw-r--r--   0 marcus     (501) staff       (20)       21 2023-07-26 03:01:12.000000 cybotrade-indicators-0.0.3/src/cybotrade_indicators.egg-info/top_level.txt
-drwxr-xr-x   0 marcus     (501) staff       (20)        0 2023-07-26 03:01:12.229343 cybotrade-indicators-0.0.3/tests/
--rw-r--r--   0 marcus     (501) staff       (20)     2219 2023-07-25 19:35:10.000000 cybotrade-indicators-0.0.3/tests/test.py
+drwxr-xr-x   0 marcus     (501) staff       (20)        0 2023-08-04 09:44:40.215543 cybotrade-indicators-0.0.4/
+-rw-r--r--   0 marcus     (501) staff       (20)      433 2023-07-25 20:08:51.000000 cybotrade-indicators-0.0.4/AUTHORS
+-rw-r--r--   0 marcus     (501) staff       (20)     7650 2023-07-25 20:08:38.000000 cybotrade-indicators-0.0.4/LICENSE
+-rw-r--r--   0 marcus     (501) staff       (20)      238 2023-07-26 03:00:01.000000 cybotrade-indicators-0.0.4/MANIFEST.in
+-rw-r--r--   0 marcus     (501) staff       (20)     3493 2023-08-04 09:44:40.215349 cybotrade-indicators-0.0.4/PKG-INFO
+-rw-r--r--   0 marcus     (501) staff       (20)     2818 2023-07-25 20:06:26.000000 cybotrade-indicators-0.0.4/README.md
+drwxr-xr-x   0 marcus     (501) staff       (20)        0 2023-08-04 09:44:40.195197 cybotrade-indicators-0.0.4/external/
+-rw-r--r--   0 marcus     (501) staff       (20)    53547 2023-07-25 10:32:29.000000 cybotrade-indicators-0.0.4/external/indicators.h
+-rw-r--r--   0 marcus     (501) staff       (20)   419813 2023-08-04 09:22:41.000000 cybotrade-indicators-0.0.4/external/tiamalgamation.c
+-rw-r--r--   0 marcus     (501) staff       (20)      920 2023-08-04 09:43:44.000000 cybotrade-indicators-0.0.4/pyproject.toml
+-rw-r--r--   0 marcus     (501) staff       (20)       38 2023-08-04 09:44:40.215608 cybotrade-indicators-0.0.4/setup.cfg
+-rw-r--r--   0 marcus     (501) staff       (20)      370 2023-07-25 19:18:28.000000 cybotrade-indicators-0.0.4/setup.py
+drwxr-xr-x   0 marcus     (501) staff       (20)        0 2023-08-04 09:44:40.190969 cybotrade-indicators-0.0.4/src/
+drwxr-xr-x   0 marcus     (501) staff       (20)        0 2023-08-04 09:44:40.213216 cybotrade-indicators-0.0.4/src/cybotrade_indicators/
+-rw-r--r--   0 marcus     (501) staff       (20)  4146665 2023-08-04 09:35:32.000000 cybotrade-indicators-0.0.4/src/cybotrade_indicators/__init__.c
+-rw-r--r--   0 marcus     (501) staff       (20)    24376 2023-07-25 19:55:33.000000 cybotrade-indicators-0.0.4/src/cybotrade_indicators/__init__.pyi
+-rw-r--r--   0 marcus     (501) staff       (20)    56715 2023-07-25 19:55:33.000000 cybotrade-indicators-0.0.4/src/cybotrade_indicators/__init__.pyx
+-rw-r--r--   0 marcus     (501) staff       (20)     1817 2023-07-25 19:17:58.000000 cybotrade-indicators-0.0.4/src/cybotrade_indicators/indicators.pxd
+-rw-r--r--   0 marcus     (501) staff       (20)        0 2023-07-25 20:15:15.000000 cybotrade-indicators-0.0.4/src/cybotrade_indicators/py.typed
+drwxr-xr-x   0 marcus     (501) staff       (20)        0 2023-08-04 09:44:40.214475 cybotrade-indicators-0.0.4/src/cybotrade_indicators.egg-info/
+-rw-r--r--   0 marcus     (501) staff       (20)     3493 2023-08-04 09:44:40.000000 cybotrade-indicators-0.0.4/src/cybotrade_indicators.egg-info/PKG-INFO
+-rw-r--r--   0 marcus     (501) staff       (20)      548 2023-08-04 09:44:40.000000 cybotrade-indicators-0.0.4/src/cybotrade_indicators.egg-info/SOURCES.txt
+-rw-r--r--   0 marcus     (501) staff       (20)        1 2023-08-04 09:44:40.000000 cybotrade-indicators-0.0.4/src/cybotrade_indicators.egg-info/dependency_links.txt
+-rw-r--r--   0 marcus     (501) staff       (20)       30 2023-08-04 09:44:40.000000 cybotrade-indicators-0.0.4/src/cybotrade_indicators.egg-info/requires.txt
+-rw-r--r--   0 marcus     (501) staff       (20)       21 2023-08-04 09:44:40.000000 cybotrade-indicators-0.0.4/src/cybotrade_indicators.egg-info/top_level.txt
+drwxr-xr-x   0 marcus     (501) staff       (20)        0 2023-08-04 09:44:40.214673 cybotrade-indicators-0.0.4/tests/
+-rw-r--r--   0 marcus     (501) staff       (20)     2219 2023-07-25 19:35:10.000000 cybotrade-indicators-0.0.4/tests/test.py
```

### Comparing `cybotrade-indicators-0.0.3/LICENSE` & `cybotrade-indicators-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cybotrade-indicators-0.0.3/PKG-INFO` & `cybotrade-indicators-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cybotrade-indicators
-Version: 0.0.3
+Version: 0.0.4
 Summary: This library provides a set of technical analysis indicators that can be used to craft trading strategies.
 Author-email: Marcus Lee <marcuslee@balaenaquant.com>, Lee Ze Lim <zelim@balaenaquant.com>
 Project-URL: Homepage, https://app.cybotrade.rs
 Project-URL: Documentation, https://docs.cybotrade.rs
 Project-URL: Repository, https://github.com/cybotrade/cybotrade-indicators
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `cybotrade-indicators-0.0.3/README.md` & `cybotrade-indicators-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `cybotrade-indicators-0.0.3/external/indicators.h` & `cybotrade-indicators-0.0.4/external/indicators.h`

 * *Files identical despite different names*

### Comparing `cybotrade-indicators-0.0.3/external/tiamalgamation.c` & `cybotrade-indicators-0.0.4/external/tiamalgamation.c`

 * *Files 0% similar despite different names*

```diff
@@ -128,17 +128,17 @@
 typedef struct ti_indicator_info {
   const char *name;
   const char *full_name;
   ti_indicator_start_function start;
   ti_indicator_function indicator;
   ti_indicator_function indicator_ref;
   int type, inputs, options, outputs;
-  const char *input_names[TI_MAXINDPARAMS];
-  const char *option_names[TI_MAXINDPARAMS];
-  const char *output_names[TI_MAXINDPARAMS];
+  const char *input_names[TI_MAXINDPARAMS + 1];
+  const char *option_names[TI_MAXINDPARAMS + 1];
+  const char *output_names[TI_MAXINDPARAMS + 1];
   ti_indicator_stream_new stream_new;
   ti_indicator_stream_run stream_run;
   ti_indicator_stream_free stream_free;
 } ti_indicator_info;
 
 /*Complete array of all indicators. Last element is 0,0,0,0...*/
 extern ti_indicator_info ti_indicators[];
@@ -6058,15 +6058,15 @@
     int buffer_idx;
     TI_REAL buffer[];
 } ti_stream_sma;
 int ti_sma_stream_new(TI_REAL const *options, ti_stream **stream_in) {
     ti_stream_sma **stream = (ti_stream_sma**)stream_in;
     int period = (int)options[0];
     if (period < 1) return TI_INVALID_OPTION;
-    *stream = malloc(sizeof(ti_stream_sma) + sizeof(TI_REAL[period]));
+    *stream = malloc(sizeof(ti_stream_sma) + sizeof(TI_REAL) * period);
     if (!stream) {
         return TI_OUT_OF_MEMORY;
     }
     (*stream)->index = TI_INDICATOR_SMA_INDEX;
     (*stream)->progress = -ti_sma_start(options);
     (*stream)->period = period;
     (*stream)->per = 1. / period;
```

### Comparing `cybotrade-indicators-0.0.3/pyproject.toml` & `cybotrade-indicators-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
 [project]
 name = "cybotrade-indicators"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
     { name = "Marcus Lee", email = "marcuslee@balaenaquant.com" },
     { name = "Lee Ze Lim", email = "zelim@balaenaquant.com" },
 ]
 description = "This library provides a set of technical analysis indicators that can be used to craft trading strategies."
 readme = "README.md"
 requires-python = ">=3.11"
```

### Comparing `cybotrade-indicators-0.0.3/src/cybotrade_indicators/__init__.c` & `cybotrade-indicators-0.0.4/src/cybotrade_indicators/__init__.c`

 * *Files 0% similar despite different names*

```diff
@@ -1438,177 +1438,177 @@
   char new_packmode;
   char enc_packmode;
   char is_valid_array;
 } __Pyx_BufFmt_Context;
 
 /* #### Code section: numeric_typedefs ### */
 
-/* "../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":730
+/* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":730
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":731
+/* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":731
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":732
+/* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":732
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":733
+/* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":733
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":737
+/* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":737
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":738
+/* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":738
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":739
+/* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":739
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":740
+/* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":740
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":744
+/* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":744
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":745
+/* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":745
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":754
+/* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":754
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":755
+/* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":755
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":757
+/* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":757
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":758
+/* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":758
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":760
+/* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":760
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":761
+/* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":761
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":763
+/* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":763
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":764
+/* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":764
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":765
+/* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":765
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1638,42 +1638,42 @@
 static CYTHON_INLINE __pyx_t_double_complex __pyx_t_double_complex_from_parts(double, double);
 
 /* #### Code section: type_declarations ### */
 
 /*--- Type declarations ---*/
 struct __pyx_obj_20cybotrade_indicators__Indicator;
 
-/* "../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":767
+/* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":767
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":768
+/* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":768
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":769
+/* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":769
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":771
+/* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":771
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -6541,261 +6541,261 @@
 #define __pyx_codeobj__304 __pyx_mstate_global->__pyx_codeobj__304
 #define __pyx_codeobj__305 __pyx_mstate_global->__pyx_codeobj__305
 #define __pyx_codeobj__307 __pyx_mstate_global->__pyx_codeobj__307
 #define __pyx_codeobj__309 __pyx_mstate_global->__pyx_codeobj__309
 #define __pyx_codeobj__310 __pyx_mstate_global->__pyx_codeobj__310
 /* #### Code section: module_code ### */
 
-/* "../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":245
+/* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_7ndarray_4base_base(PyArrayObject *__pyx_v_self) {
   PyObject *__pyx_r;
 
-  /* "../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":248
+  /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":248
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  *             return PyArray_BASE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_BASE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":245
+  /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":251
+/* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
 static CYTHON_INLINE PyArray_Descr *__pyx_f_5numpy_7ndarray_5descr_descr(PyArrayObject *__pyx_v_self) {
   PyArray_Descr *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyArray_Descr *__pyx_t_1;
   __Pyx_RefNannySetupContext("descr", 0);
 
-  /* "../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":254
+  /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":254
  *             """Returns an owned reference to the dtype of the array.
  *             """
  *             return <dtype>PyArray_DESCR(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __Pyx_XDECREF((PyObject *)__pyx_r);
   __pyx_t_1 = PyArray_DESCR(__pyx_v_self);
   __Pyx_INCREF((PyObject *)((PyArray_Descr *)__pyx_t_1));
   __pyx_r = ((PyArray_Descr *)__pyx_t_1);
   goto __pyx_L0;
 
-  /* "../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":251
+  /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":257
+/* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_7ndarray_4ndim_ndim(PyArrayObject *__pyx_v_self) {
   int __pyx_r;
 
-  /* "../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":260
+  /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":260
  *             """Returns the number of dimensions in the array.
  *             """
  *             return PyArray_NDIM(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_NDIM(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":257
+  /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":263
+/* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_5shape_shape(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":268
+  /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":268
  *             Can return NULL for 0-dimensional arrays.
  *             """
  *             return PyArray_DIMS(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_DIMS(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":263
+  /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":271
+/* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_7strides_strides(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":275
+  /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":275
  *             The number of elements matches the number of dimensions of the array (ndim).
  *             """
  *             return PyArray_STRIDES(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_STRIDES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":271
+  /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":278
+/* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
 static CYTHON_INLINE npy_intp __pyx_f_5numpy_7ndarray_4size_size(PyArrayObject *__pyx_v_self) {
   npy_intp __pyx_r;
 
-  /* "../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":281
+  /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":281
  *             """Returns the total size (in number of elements) of the array.
  *             """
  *             return PyArray_SIZE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_SIZE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":278
+  /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":284
+/* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
 static CYTHON_INLINE char *__pyx_f_5numpy_7ndarray_4data_data(PyArrayObject *__pyx_v_self) {
   char *__pyx_r;
 
-  /* "../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":290
+  /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":290
  *             of `PyArray_DATA()` instead, which returns a 'void*'.
  *             """
  *             return PyArray_BYTES(self)             # <<<<<<<<<<<<<<
  * 
  *     ctypedef unsigned char      npy_bool
  */
   __pyx_r = PyArray_BYTES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":284
+  /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":773
+/* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":773
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -6804,29 +6804,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":774
+  /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":774
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 774, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":773
+  /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":773
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -6837,15 +6837,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":776
+/* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":776
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -6854,29 +6854,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":777
+  /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":777
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 777, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":776
+  /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":776
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -6887,15 +6887,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":779
+/* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -6904,29 +6904,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":780
+  /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":780
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 780, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":779
+  /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -6937,15 +6937,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":782
+/* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -6954,29 +6954,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":783
+  /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":783
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 783, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":782
+  /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -6987,15 +6987,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":785
+/* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -7004,29 +7004,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":786
+  /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":786
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 786, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":785
+  /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -7037,89 +7037,89 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":788
+/* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":789
+  /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":789
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = PyDataType_HASSUBARRAY(__pyx_v_d);
   if (__pyx_t_1) {
 
-    /* "../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":790
+    /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":790
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":789
+    /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":789
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":792
+  /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":792
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":788
+  /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":967
+/* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":967
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
@@ -7127,33 +7127,33 @@
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":968
+  /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":968
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":969
+  /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":969
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   __pyx_t_1 = PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(2, 969, __pyx_L1_error)
 
-  /* "../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":967
+  /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":967
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
@@ -7161,96 +7161,96 @@
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_AddTraceback("numpy.set_array_base", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":971
+/* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":971
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":972
+  /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":972
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":973
+  /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":973
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = (__pyx_v_base == NULL);
   if (__pyx_t_1) {
 
-    /* "../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":974
+    /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":974
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":973
+    /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":973
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":975
+  /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":975
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":971
+  /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":971
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":979
+/* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":979
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -7266,15 +7266,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":980
+  /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":980
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -7282,68 +7282,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":981
+      /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":981
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 981, __pyx_L3_error)
 
-      /* "../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":980
+      /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":980
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":982
+    /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":982
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 982, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":983
+      /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":983
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 983, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 983, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":980
+    /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":980
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -7351,15 +7351,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":979
+  /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":979
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -7374,15 +7374,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":985
+/* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":985
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -7398,15 +7398,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":986
+  /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":986
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -7414,68 +7414,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":987
+      /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":987
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 987, __pyx_L3_error)
 
-      /* "../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":986
+      /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":986
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":988
+    /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":988
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 988, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":989
+      /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":989
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 989, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 989, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":986
+    /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":986
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -7483,15 +7483,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":985
+  /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":985
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -7506,15 +7506,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":991
+/* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":991
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -7530,15 +7530,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":992
+  /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":992
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -7546,68 +7546,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":993
+      /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":993
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 993, __pyx_L3_error)
 
-      /* "../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":992
+      /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":992
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":994
+    /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":994
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 994, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":995
+      /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":995
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * 
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 995, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 995, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":992
+    /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":992
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -7615,15 +7615,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":991
+  /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":991
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -7638,176 +7638,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":998
+/* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":998
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1010
+  /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1010
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":998
+  /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":998
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1013
+/* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1013
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1025
+  /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1025
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1013
+  /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1013
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1028
+/* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1028
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1035
+  /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1035
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1028
+  /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1028
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1038
+/* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1038
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1042
+  /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1042
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1038
+  /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1038
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1045
+/* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1045
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1049
+  /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1049
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1045
+  /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1045
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -33910,26 +33910,26 @@
 }
 /* #### Code section: cached_constants ### */
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":983
+  /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":983
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_s_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple_)) __PYX_ERR(2, 983, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple_);
   __Pyx_GIVEREF(__pyx_tuple_);
 
-  /* "../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":989
+  /* "../../../../../../opt/homebrew/Caskroom/miniconda/base/envs/cybotrade-indicators/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":989
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(2, 989, __pyx_L1_error)
```

### Comparing `cybotrade-indicators-0.0.3/src/cybotrade_indicators/__init__.pyi` & `cybotrade-indicators-0.0.4/src/cybotrade_indicators/__init__.pyi`

 * *Files identical despite different names*

### Comparing `cybotrade-indicators-0.0.3/src/cybotrade_indicators/__init__.pyx` & `cybotrade-indicators-0.0.4/src/cybotrade_indicators/__init__.pyx`

 * *Files identical despite different names*

### Comparing `cybotrade-indicators-0.0.3/src/cybotrade_indicators/indicators.pxd` & `cybotrade-indicators-0.0.4/src/cybotrade_indicators/indicators.pxd`

 * *Files identical despite different names*

### Comparing `cybotrade-indicators-0.0.3/src/cybotrade_indicators.egg-info/PKG-INFO` & `cybotrade-indicators-0.0.4/src/cybotrade_indicators.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cybotrade-indicators
-Version: 0.0.3
+Version: 0.0.4
 Summary: This library provides a set of technical analysis indicators that can be used to craft trading strategies.
 Author-email: Marcus Lee <marcuslee@balaenaquant.com>, Lee Ze Lim <zelim@balaenaquant.com>
 Project-URL: Homepage, https://app.cybotrade.rs
 Project-URL: Documentation, https://docs.cybotrade.rs
 Project-URL: Repository, https://github.com/cybotrade/cybotrade-indicators
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `cybotrade-indicators-0.0.3/src/cybotrade_indicators.egg-info/SOURCES.txt` & `cybotrade-indicators-0.0.4/src/cybotrade_indicators.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cybotrade-indicators-0.0.3/tests/test.py` & `cybotrade-indicators-0.0.4/tests/test.py`

 * *Files identical despite different names*

