# Comparing `tmp/alpaka-job-coverage-1.5.0.tar.gz` & `tmp/alpaka-job-coverage-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alpaka-job-coverage-1.5.0.tar", last modified: Thu Aug  3 12:16:01 2023, max compression
+gzip compressed data, was "alpaka-job-coverage-1.5.1.tar", last modified: Fri Aug  4 14:08:02 2023, max compression
```

## Comparing `alpaka-job-coverage-1.5.0.tar` & `alpaka-job-coverage-1.5.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:16:01.181329 alpaka-job-coverage-1.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-08-03 12:15:42.000000 alpaka-job-coverage-1.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-03 12:15:42.000000 alpaka-job-coverage-1.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7189 2023-08-03 12:16:01.181329 alpaka-job-coverage-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6489 2023-08-03 12:15:42.000000 alpaka-job-coverage-1.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-08-03 12:15:42.000000 alpaka-job-coverage-1.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 12:16:01.181329 alpaka-job-coverage-1.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-08-03 12:15:42.000000 alpaka-job-coverage-1.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:16:01.177329 alpaka-job-coverage-1.5.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:16:01.181329 alpaka-job-coverage-1.5.0/src/alpaka_job_coverage/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-08-03 12:15:42.000000 alpaka-job-coverage-1.5.0/src/alpaka_job_coverage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8120 2023-08-03 12:15:42.000000 alpaka-job-coverage-1.5.0/src/alpaka_job_coverage/filter_backend_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-08-03 12:15:42.000000 alpaka-job-coverage-1.5.0/src/alpaka_job_coverage/filter_compiler_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     7951 2023-08-03 12:15:42.000000 alpaka-job-coverage-1.5.0/src/alpaka_job_coverage/filter_compiler_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     7966 2023-08-03 12:15:42.000000 alpaka-job-coverage-1.5.0/src/alpaka_job_coverage/filter_software_dependency.py
--rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-08-03 12:15:42.000000 alpaka-job-coverage-1.5.0/src/alpaka_job_coverage/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)     6564 2023-08-03 12:15:42.000000 alpaka-job-coverage-1.5.0/src/alpaka_job_coverage/main_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11246 2023-08-03 12:15:42.000000 alpaka-job-coverage-1.5.0/src/alpaka_job_coverage/util.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12117 2023-08-03 12:15:42.000000 alpaka-job-coverage-1.5.0/src/alpaka_job_coverage/validate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-08-03 12:15:42.000000 alpaka-job-coverage-1.5.0/src/alpaka_job_coverage/versions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:16:01.181329 alpaka-job-coverage-1.5.0/src/alpaka_job_coverage.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7189 2023-08-03 12:16:01.000000 alpaka-job-coverage-1.5.0/src/alpaka_job_coverage.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-08-03 12:16:01.000000 alpaka-job-coverage-1.5.0/src/alpaka_job_coverage.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 12:16:01.000000 alpaka-job-coverage-1.5.0/src/alpaka_job_coverage.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-08-03 12:16:01.000000 alpaka-job-coverage-1.5.0/src/alpaka_job_coverage.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-08-03 12:16:01.000000 alpaka-job-coverage-1.5.0/src/alpaka_job_coverage.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-03 12:16:01.000000 alpaka-job-coverage-1.5.0/src/alpaka_job_coverage.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:16:01.181329 alpaka-job-coverage-1.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-08-03 12:15:42.000000 alpaka-job-coverage-1.5.0/tests/test_compiler_names.py
--rw-r--r--   0 runner    (1001) docker     (123)    42016 2023-08-03 12:15:42.000000 alpaka-job-coverage-1.5.0/tests/test_cuda_sdk.py
--rw-r--r--   0 runner    (1001) docker     (123)    12280 2023-08-03 12:15:42.000000 alpaka-job-coverage-1.5.0/tests/test_hipcc.py
--rw-r--r--   0 runner    (1001) docker     (123)    12040 2023-08-03 12:15:42.000000 alpaka-job-coverage-1.5.0/tests/test_icpx.py
--rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-08-03 12:15:42.000000 alpaka-job-coverage-1.5.0/tests/test_single_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     5548 2023-08-03 12:15:42.000000 alpaka-job-coverage-1.5.0/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-08-03 12:15:42.000000 alpaka-job-coverage-1.5.0/tests/test_versions.py
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-03 12:15:42.000000 alpaka-job-coverage-1.5.0/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 14:08:02.460948 alpaka-job-coverage-1.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-08-04 14:07:45.000000 alpaka-job-coverage-1.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-04 14:07:45.000000 alpaka-job-coverage-1.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7189 2023-08-04 14:08:02.460948 alpaka-job-coverage-1.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6489 2023-08-04 14:07:45.000000 alpaka-job-coverage-1.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-08-04 14:07:45.000000 alpaka-job-coverage-1.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 14:08:02.460948 alpaka-job-coverage-1.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-08-04 14:07:45.000000 alpaka-job-coverage-1.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 14:08:02.456948 alpaka-job-coverage-1.5.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 14:08:02.456948 alpaka-job-coverage-1.5.1/src/alpaka_job_coverage/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-08-04 14:07:45.000000 alpaka-job-coverage-1.5.1/src/alpaka_job_coverage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8120 2023-08-04 14:07:45.000000 alpaka-job-coverage-1.5.1/src/alpaka_job_coverage/filter_backend_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-08-04 14:07:45.000000 alpaka-job-coverage-1.5.1/src/alpaka_job_coverage/filter_compiler_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7951 2023-08-04 14:07:45.000000 alpaka-job-coverage-1.5.1/src/alpaka_job_coverage/filter_compiler_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7966 2023-08-04 14:07:45.000000 alpaka-job-coverage-1.5.1/src/alpaka_job_coverage/filter_software_dependency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-08-04 14:07:45.000000 alpaka-job-coverage-1.5.1/src/alpaka_job_coverage/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6564 2023-08-04 14:07:45.000000 alpaka-job-coverage-1.5.1/src/alpaka_job_coverage/main_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11246 2023-08-04 14:07:45.000000 alpaka-job-coverage-1.5.1/src/alpaka_job_coverage/util.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12117 2023-08-04 14:07:45.000000 alpaka-job-coverage-1.5.1/src/alpaka_job_coverage/validate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-08-04 14:07:45.000000 alpaka-job-coverage-1.5.1/src/alpaka_job_coverage/versions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 14:08:02.460948 alpaka-job-coverage-1.5.1/src/alpaka_job_coverage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7189 2023-08-04 14:08:02.000000 alpaka-job-coverage-1.5.1/src/alpaka_job_coverage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-08-04 14:08:02.000000 alpaka-job-coverage-1.5.1/src/alpaka_job_coverage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 14:08:02.000000 alpaka-job-coverage-1.5.1/src/alpaka_job_coverage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-08-04 14:08:02.000000 alpaka-job-coverage-1.5.1/src/alpaka_job_coverage.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-08-04 14:08:02.000000 alpaka-job-coverage-1.5.1/src/alpaka_job_coverage.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-04 14:08:02.000000 alpaka-job-coverage-1.5.1/src/alpaka_job_coverage.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 14:08:02.460948 alpaka-job-coverage-1.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-08-04 14:07:45.000000 alpaka-job-coverage-1.5.1/tests/test_compiler_names.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42016 2023-08-04 14:07:45.000000 alpaka-job-coverage-1.5.1/tests/test_cuda_sdk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12280 2023-08-04 14:07:45.000000 alpaka-job-coverage-1.5.1/tests/test_hipcc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12096 2023-08-04 14:07:45.000000 alpaka-job-coverage-1.5.1/tests/test_icpx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-08-04 14:07:45.000000 alpaka-job-coverage-1.5.1/tests/test_single_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5548 2023-08-04 14:07:45.000000 alpaka-job-coverage-1.5.1/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-08-04 14:07:45.000000 alpaka-job-coverage-1.5.1/tests/test_versions.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-04 14:07:45.000000 alpaka-job-coverage-1.5.1/version.txt
```

### Comparing `alpaka-job-coverage-1.5.0/LICENSE` & `alpaka-job-coverage-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `alpaka-job-coverage-1.5.0/PKG-INFO` & `alpaka-job-coverage-1.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alpaka-job-coverage
-Version: 1.5.0
+Version: 1.5.1
 Summary: The library provides everything needed to generate a sparse combination matrix for alpaca-based projects, including a set of general-purpose combination rules.
 Home-page: https://github.com/alpaka-group/alpaka-job-matrix-library
 Author: Simeon Ehrig
 Author-email: s.ehrig@hzdr.de
 Project-URL: Bug Tracker, https://github.com/alpaka-group/alpaka-job-matrix-library/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
```

### Comparing `alpaka-job-coverage-1.5.0/README.md` & `alpaka-job-coverage-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `alpaka-job-coverage-1.5.0/setup.py` & `alpaka-job-coverage-1.5.1/setup.py`

 * *Files identical despite different names*

### Comparing `alpaka-job-coverage-1.5.0/src/alpaka_job_coverage/filter_backend_version.py` & `alpaka-job-coverage-1.5.1/src/alpaka_job_coverage/filter_backend_version.py`

 * *Files identical despite different names*

### Comparing `alpaka-job-coverage-1.5.0/src/alpaka_job_coverage/filter_compiler_name.py` & `alpaka-job-coverage-1.5.1/src/alpaka_job_coverage/filter_compiler_name.py`

 * *Files identical despite different names*

### Comparing `alpaka-job-coverage-1.5.0/src/alpaka_job_coverage/filter_compiler_version.py` & `alpaka-job-coverage-1.5.1/src/alpaka_job_coverage/filter_compiler_version.py`

 * *Files identical despite different names*

### Comparing `alpaka-job-coverage-1.5.0/src/alpaka_job_coverage/filter_software_dependency.py` & `alpaka-job-coverage-1.5.1/src/alpaka_job_coverage/filter_software_dependency.py`

 * *Files identical despite different names*

### Comparing `alpaka-job-coverage-1.5.0/src/alpaka_job_coverage/globals.py` & `alpaka-job-coverage-1.5.1/src/alpaka_job_coverage/globals.py`

 * *Files identical despite different names*

### Comparing `alpaka-job-coverage-1.5.0/src/alpaka_job_coverage/main_functions.py` & `alpaka-job-coverage-1.5.1/src/alpaka_job_coverage/main_functions.py`

 * *Files identical despite different names*

### Comparing `alpaka-job-coverage-1.5.0/src/alpaka_job_coverage/util.py` & `alpaka-job-coverage-1.5.1/src/alpaka_job_coverage/util.py`

 * *Files identical despite different names*

### Comparing `alpaka-job-coverage-1.5.0/src/alpaka_job_coverage/validate.py` & `alpaka-job-coverage-1.5.1/src/alpaka_job_coverage/validate.py`

 * *Files identical despite different names*

### Comparing `alpaka-job-coverage-1.5.0/src/alpaka_job_coverage/versions.py` & `alpaka-job-coverage-1.5.1/src/alpaka_job_coverage/versions.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         "11.7",
         "11.8",
         "12.0",
         "12.1",
         "12.2",
     ],
     HIPCC: ["5.0", "5.1", "5.2", "5.3", "5.4", "5.5"],
-    ICPX: ["2023.1", "2023.2"],
+    ICPX: ["2023.1.0", "2023.2.0"],
     UBUNTU: ["18.04", "20.04"],
     CMAKE: ["3.18", "3.19", "3.20", "3.21", "3.22", "3.23", "3.24", "3.25", "3.26"],
     BOOST: [
         "1.74.0",
         "1.75.0",
         "1.76.0",
         "1.77.0",
```

### Comparing `alpaka-job-coverage-1.5.0/src/alpaka_job_coverage.egg-info/PKG-INFO` & `alpaka-job-coverage-1.5.1/src/alpaka_job_coverage.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alpaka-job-coverage
-Version: 1.5.0
+Version: 1.5.1
 Summary: The library provides everything needed to generate a sparse combination matrix for alpaca-based projects, including a set of general-purpose combination rules.
 Home-page: https://github.com/alpaka-group/alpaka-job-matrix-library
 Author: Simeon Ehrig
 Author-email: s.ehrig@hzdr.de
 Project-URL: Bug Tracker, https://github.com/alpaka-group/alpaka-job-matrix-library/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
```

### Comparing `alpaka-job-coverage-1.5.0/src/alpaka_job_coverage.egg-info/SOURCES.txt` & `alpaka-job-coverage-1.5.1/src/alpaka_job_coverage.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alpaka-job-coverage-1.5.0/tests/test_compiler_names.py` & `alpaka-job-coverage-1.5.1/tests/test_compiler_names.py`

 * *Files identical despite different names*

### Comparing `alpaka-job-coverage-1.5.0/tests/test_cuda_sdk.py` & `alpaka-job-coverage-1.5.1/tests/test_cuda_sdk.py`

 * *Files identical despite different names*

### Comparing `alpaka-job-coverage-1.5.0/tests/test_hipcc.py` & `alpaka-job-coverage-1.5.1/tests/test_hipcc.py`

 * *Files identical despite different names*

### Comparing `alpaka-job-coverage-1.5.0/tests/test_icpx.py` & `alpaka-job-coverage-1.5.1/tests/test_icpx.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,16 +33,16 @@
         param_map = {}
 
     # test that no combination is forbidden when only icpx is the host compiler
     # and no other parameter is set
     def test_only_host_compiler(self):
         valid_combs = [
             [(ICPX, "0")],
-            [(ICPX, "2023.1")],
-            [(ICPX, "2023.2")],
+            [(ICPX, "2023.1.0")],
+            [(ICPX, "2023.2.0")],
         ]
 
         for comb in valid_combs:
             self.assertTrue(
                 general_compiler_filter_typed(comb),
                 f"HOST_COMPILER: {comb[0][0]}",
             )
@@ -126,16 +126,16 @@
                 f"HOST_COMPILER: {comb[0][0]}, DEVICE_COMPILER: {comb[1][0]}",
             )
 
     # verify that only icpx can be used, if it set as host and device compiler
     # and has the same compiler version
     def test_host_device_compiler_version(self):
         valid_combs = [
-            [(ICPX, "2023.1"), (ICPX, "2023.1")],
-            [(ICPX, "2023.2"), (ICPX, "2023.2")],
+            [(ICPX, "2023.1.0"), (ICPX, "2023.1.0")],
+            [(ICPX, "2023.2.0"), (ICPX, "2023.2.0")],
         ]
 
         for comb in valid_combs:
             self.assertTrue(
                 general_compiler_filter_typed(comb),
                 f"HOST_COMPILER: {comb[0][0]} {comb[0][1]}, "
                 f"DEVICE_COMPILER: {comb[1][0]} {comb[1][1]}",
@@ -158,16 +158,16 @@
             self.assertTrue(
                 full_filter_chain(comb),
                 f"HOST_COMPILER: {comb[0][0]} {comb[0][1]}, "
                 f"DEVICE_COMPILER: {comb[1][0]} {comb[1][1]}",
             )
 
         invalid_combs = [
-            [(ICPX, "2023.1"), (ICPX, "2023.2")],
-            [(ICPX, "2023.2"), (ICPX, "2023.1")],
+            [(ICPX, "2023.1.0"), (ICPX, "2023.2.0")],
+            [(ICPX, "2023.2.0"), (ICPX, "2023.1.0")],
         ]
 
         for comb in invalid_combs:
             self.assertTrue(
                 general_compiler_filter_typed(comb),
                 f"HOST_COMPILER: {comb[0][0]} {comb[0][1]}, "
                 f"DEVICE_COMPILER: {comb[1][0]} {comb[1][1]}",
@@ -192,28 +192,28 @@
                 f"HOST_COMPILER: {comb[0][0]} {comb[0][1]}, "
                 f"DEVICE_COMPILER: {comb[1][0]} {comb[1][1]}",
             )
 
     # Allowed back-ends are SYCL and the CPU back-ends
     def test_host_device_compiler_backend(self):
         valid_combs = [
-            [(ICPX, "2023.1"), (ICPX, "2023.1"), [(ALPAKA_ACC_SYCL_ENABLE, ON_VER)]],
-            [(ICPX, "2023.2"), (ICPX, "2023.2"), [(ALPAKA_ACC_SYCL_ENABLE, ON_VER)]],
+            [(ICPX, "2023.1.0"), (ICPX, "2023.1.0"), [(ALPAKA_ACC_SYCL_ENABLE, ON_VER)]],
+            [(ICPX, "2023.2.0"), (ICPX, "2023.2.0"), [(ALPAKA_ACC_SYCL_ENABLE, ON_VER)]],
             [
-                (ICPX, "2023.1"),
-                (ICPX, "2023.1"),
+                (ICPX, "2023.1.0"),
+                (ICPX, "2023.1.0"),
                 [
                     (ALPAKA_ACC_CPU_B_TBB_T_SEQ_ENABLE, ON_VER),
                     (ALPAKA_ACC_CPU_B_SEQ_T_OMP2_ENABLE, ON_VER),
                     (ALPAKA_ACC_SYCL_ENABLE, ON_VER),
                 ],
             ],
             [
-                (ICPX, "2023.2"),
-                (ICPX, "2023.2"),
+                (ICPX, "2023.2.0"),
+                (ICPX, "2023.2.0"),
                 [
                     (ALPAKA_ACC_CPU_B_TBB_T_SEQ_ENABLE, ON_VER),
                     (ALPAKA_ACC_CPU_B_SEQ_T_OMP2_ENABLE, ON_VER),
                     (ALPAKA_ACC_CPU_B_OMP2_T_SEQ_ENABLE, ON_VER),
                     (ALPAKA_ACC_GPU_HIP_ENABLE, OFF_VER),
                     (ALPAKA_ACC_GPU_CUDA_ENABLE, OFF_VER),
                 ],
@@ -249,30 +249,30 @@
                 full_filter_chain(comb),
                 f"HOST_COMPILER: {comb[0][0]} {comb[0][1]}, "
                 f"DEVICE_COMPILER: {comb[1][0]} {comb[1][1]}, "
                 f"BACKENDS: {comb[2]}",
             )
 
         invalid_combs = [
-            [(ICPX, "2023.1"), (ICPX, "2023.1"), [(ALPAKA_ACC_GPU_HIP_ENABLE, "4.4")]],
-            [(ICPX, "2023.2"), (ICPX, "2023.2"), [(ALPAKA_ACC_GPU_HIP_ENABLE, "5.2")]],
-            [(ICPX, "2023.1"), (ICPX, "2023.1"), [(ALPAKA_ACC_GPU_CUDA_ENABLE, "12.1")]],
+            [(ICPX, "2023.1.0"), (ICPX, "2023.1.0"), [(ALPAKA_ACC_GPU_HIP_ENABLE, "4.4")]],
+            [(ICPX, "2023.2.0"), (ICPX, "2023.2.0"), [(ALPAKA_ACC_GPU_HIP_ENABLE, "5.2")]],
+            [(ICPX, "2023.1.0"), (ICPX, "2023.1.0"), [(ALPAKA_ACC_GPU_CUDA_ENABLE, "12.1")]],
             [
-                (ICPX, "2023.2"),
-                (ICPX, "2023.2"),
+                (ICPX, "2023.2.0"),
+                (ICPX, "2023.2.0"),
                 [
                     (ALPAKA_ACC_CPU_B_TBB_T_SEQ_ENABLE, ON_VER),
                     (ALPAKA_ACC_CPU_B_SEQ_T_OMP2_ENABLE, ON_VER),
                     (ALPAKA_ACC_GPU_HIP_ENABLE, "5.5"),
                 ],
             ],
             # it is forbidden to enable the CUDA and SYCL back-end at the same time
             [
-                (ICPX, "2023.1"),
-                (ICPX, "2023.1"),
+                (ICPX, "2023.1.0"),
+                (ICPX, "2023.1.0"),
                 [
                     (ALPAKA_ACC_GPU_CUDA_ENABLE, "11.2"),
                     (ALPAKA_ACC_SYCL_ENABLE, ON_VER),
                 ],
             ],
         ]
```

### Comparing `alpaka-job-coverage-1.5.0/tests/test_single_rules.py` & `alpaka-job-coverage-1.5.1/tests/test_single_rules.py`

 * *Files identical despite different names*

### Comparing `alpaka-job-coverage-1.5.0/tests/test_util.py` & `alpaka-job-coverage-1.5.1/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `alpaka-job-coverage-1.5.0/tests/test_versions.py` & `alpaka-job-coverage-1.5.1/tests/test_versions.py`

 * *Files identical despite different names*

