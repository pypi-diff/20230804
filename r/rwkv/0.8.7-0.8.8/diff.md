# Comparing `tmp/rwkv-0.8.7.tar.gz` & `tmp/rwkv-0.8.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rwkv-0.8.7.tar", last modified: Sat Jul 29 09:30:59 2023, max compression
+gzip compressed data, was "rwkv-0.8.8.tar", last modified: Fri Aug  4 03:30:22 2023, max compression
```

## Comparing `rwkv-0.8.7.tar` & `rwkv-0.8.8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 blinkdl  (424401630) Domain Users (424400513)        0 2023-07-29 09:30:59.000000 rwkv-0.8.7/
--rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)    11357 2023-03-01 07:25:16.000000 rwkv-0.8.7/LICENSE
--rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)       47 2023-05-19 16:15:03.000000 rwkv-0.8.7/MANIFEST.in
--rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)     4842 2023-07-29 09:30:59.000000 rwkv-0.8.7/PKG-INFO
--rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)     4372 2023-06-26 03:17:49.000000 rwkv-0.8.7/README.md
--rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)      499 2023-07-29 09:26:39.000000 rwkv-0.8.7/pyproject.toml
--rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)       38 2023-07-29 09:30:59.000000 rwkv-0.8.7/setup.cfg
-drwxr-xr-x   0 blinkdl  (424401630) Domain Users (424400513)        0 2023-07-29 09:30:58.000000 rwkv-0.8.7/src/
-drwxr-xr-x   0 blinkdl  (424401630) Domain Users (424400513)        0 2023-07-29 09:30:58.000000 rwkv-0.8.7/src/rwkv/
--rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)        0 2023-02-28 12:56:58.000000 rwkv-0.8.7/src/rwkv/__init__.py
-drwxr-xr-x   0 blinkdl  (424401630) Domain Users (424400513)        0 2023-07-29 09:30:59.000000 rwkv-0.8.7/src/rwkv/cuda/
--rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)     3621 2023-07-29 09:25:30.000000 rwkv-0.8.7/src/rwkv/cuda/gemm_fp16_cublas.cpp
--rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)     8677 2023-04-27 19:18:02.000000 rwkv-0.8.7/src/rwkv/cuda/operators.cu
--rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)     5002 2023-07-29 09:25:30.000000 rwkv-0.8.7/src/rwkv/cuda/wrapper.cpp
--rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)    40726 2023-07-29 09:29:04.000000 rwkv-0.8.7/src/rwkv/model.py
--rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)     3201 2023-06-10 18:48:52.000000 rwkv-0.8.7/src/rwkv/rwkv_tokenizer.py
--rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)  1093733 2023-05-18 04:00:58.000000 rwkv-0.8.7/src/rwkv/rwkv_vocab_v20230424.txt
--rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)     5356 2023-06-26 03:07:02.000000 rwkv-0.8.7/src/rwkv/utils.py
-drwxr-xr-x   0 blinkdl  (424401630) Domain Users (424400513)        0 2023-07-29 09:30:59.000000 rwkv-0.8.7/src/rwkv.egg-info/
--rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)     4842 2023-07-29 09:30:58.000000 rwkv-0.8.7/src/rwkv.egg-info/PKG-INFO
--rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)      409 2023-07-29 09:30:58.000000 rwkv-0.8.7/src/rwkv.egg-info/SOURCES.txt
--rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)        1 2023-07-29 09:30:58.000000 rwkv-0.8.7/src/rwkv.egg-info/dependency_links.txt
--rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)       19 2023-07-29 09:30:58.000000 rwkv-0.8.7/src/rwkv.egg-info/requires.txt
--rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)        5 2023-07-29 09:30:58.000000 rwkv-0.8.7/src/rwkv.egg-info/top_level.txt
+drwxr-xr-x   0 blinkdl  (424401630) Domain Users (424400513)        0 2023-08-04 03:30:22.000000 rwkv-0.8.8/
+-rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)    11357 2023-03-01 07:25:16.000000 rwkv-0.8.8/LICENSE
+-rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)       47 2023-05-19 16:15:03.000000 rwkv-0.8.8/MANIFEST.in
+-rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)     4842 2023-08-04 03:30:22.000000 rwkv-0.8.8/PKG-INFO
+-rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)     4372 2023-06-26 03:17:49.000000 rwkv-0.8.8/README.md
+-rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)      499 2023-08-04 03:29:43.000000 rwkv-0.8.8/pyproject.toml
+-rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)       38 2023-08-04 03:30:22.000000 rwkv-0.8.8/setup.cfg
+drwxr-xr-x   0 blinkdl  (424401630) Domain Users (424400513)        0 2023-08-04 03:30:22.000000 rwkv-0.8.8/src/
+drwxr-xr-x   0 blinkdl  (424401630) Domain Users (424400513)        0 2023-08-04 03:30:22.000000 rwkv-0.8.8/src/rwkv/
+-rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)        0 2023-02-28 12:56:58.000000 rwkv-0.8.8/src/rwkv/__init__.py
+drwxr-xr-x   0 blinkdl  (424401630) Domain Users (424400513)        0 2023-08-04 03:30:22.000000 rwkv-0.8.8/src/rwkv/cuda/
+-rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)     3633 2023-08-04 03:28:50.000000 rwkv-0.8.8/src/rwkv/cuda/gemm_fp16_cublas.cpp
+-rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)     8677 2023-04-27 19:18:02.000000 rwkv-0.8.8/src/rwkv/cuda/operators.cu
+-rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)     5002 2023-07-29 09:25:30.000000 rwkv-0.8.8/src/rwkv/cuda/wrapper.cpp
+-rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)    40726 2023-07-29 09:29:04.000000 rwkv-0.8.8/src/rwkv/model.py
+-rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)     3201 2023-06-10 18:48:52.000000 rwkv-0.8.8/src/rwkv/rwkv_tokenizer.py
+-rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)  1093733 2023-05-18 04:00:58.000000 rwkv-0.8.8/src/rwkv/rwkv_vocab_v20230424.txt
+-rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)     5356 2023-06-26 03:07:02.000000 rwkv-0.8.8/src/rwkv/utils.py
+drwxr-xr-x   0 blinkdl  (424401630) Domain Users (424400513)        0 2023-08-04 03:30:22.000000 rwkv-0.8.8/src/rwkv.egg-info/
+-rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)     4842 2023-08-04 03:30:22.000000 rwkv-0.8.8/src/rwkv.egg-info/PKG-INFO
+-rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)      409 2023-08-04 03:30:22.000000 rwkv-0.8.8/src/rwkv.egg-info/SOURCES.txt
+-rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)        1 2023-08-04 03:30:22.000000 rwkv-0.8.8/src/rwkv.egg-info/dependency_links.txt
+-rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)       19 2023-08-04 03:30:22.000000 rwkv-0.8.8/src/rwkv.egg-info/requires.txt
+-rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)        5 2023-08-04 03:30:22.000000 rwkv-0.8.8/src/rwkv.egg-info/top_level.txt
```

### Comparing `rwkv-0.8.7/LICENSE` & `rwkv-0.8.8/LICENSE`

 * *Files identical despite different names*

### Comparing `rwkv-0.8.7/PKG-INFO` & `rwkv-0.8.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rwkv
-Version: 0.8.7
+Version: 0.8.8
 Summary: The RWKV Language Model
 Author: Bo PENG
 Project-URL: Homepage, https://github.com/BlinkDL/ChatRWKV
 Project-URL: Bug Tracker, https://github.com/BlinkDL/ChatRWKV/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `rwkv-0.8.7/README.md` & `rwkv-0.8.8/README.md`

 * *Files identical despite different names*

### Comparing `rwkv-0.8.7/src/rwkv/cuda/gemm_fp16_cublas.cpp` & `rwkv-0.8.8/src/rwkv/cuda/gemm_fp16_cublas.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -59,23 +59,23 @@
 
 #if CUDA_VERSION >= 11000
   cublasGemmAlgo_t algo = CUBLAS_GEMM_DEFAULT;
 #else
   cublasGemmAlgo_t algo = CUBLAS_GEMM_DFALT_TENSOR_OP;
 #endif
   const float sp_beta = 0.f;
-  if (a.dense_dim() == 2 && b.dense_dim() == 2) {
+  if (a.sizes().size() == 2 && b.sizes().size() == 2) {
     CUBLAS_CHECK(cublasGemmEx(
         cublas_handle, cublas_trans_a, cublas_trans_b, m, n, k, &sp_alpha,
         a.data_ptr(), cuda_data_type, cublas_lda, b.data_ptr(), cuda_data_type,
         cublas_ldb, &sp_beta, c.data_ptr(), cuda_c_data_type, cublas_ldc,
         compute_type, algo));
   } else {
     // batch matmul
-    assert(a.dense_dim() == 3 && b.dense_dim() == 3);
+    assert(a.sizes().size() == 3 && b.sizes().size() == 3);
 
     const long long int cublas_stride_a = m * k;
     const long long int cublas_stride_b = k * n;
     const long long int cublas_stride_c = m * n;
     CUBLAS_CHECK(cublasGemmStridedBatchedEx(
         cublas_handle, cublas_trans_a, cublas_trans_b, m,
         n, k, &sp_alpha, a.data_ptr(), cuda_data_type, cublas_lda,
```

### Comparing `rwkv-0.8.7/src/rwkv/cuda/operators.cu` & `rwkv-0.8.8/src/rwkv/cuda/operators.cu`

 * *Files identical despite different names*

### Comparing `rwkv-0.8.7/src/rwkv/cuda/wrapper.cpp` & `rwkv-0.8.8/src/rwkv/cuda/wrapper.cpp`

 * *Files identical despite different names*

### Comparing `rwkv-0.8.7/src/rwkv/model.py` & `rwkv-0.8.8/src/rwkv/model.py`

 * *Files identical despite different names*

### Comparing `rwkv-0.8.7/src/rwkv/rwkv_tokenizer.py` & `rwkv-0.8.8/src/rwkv/rwkv_tokenizer.py`

 * *Files identical despite different names*

### Comparing `rwkv-0.8.7/src/rwkv/rwkv_vocab_v20230424.txt` & `rwkv-0.8.8/src/rwkv/rwkv_vocab_v20230424.txt`

 * *Files identical despite different names*

### Comparing `rwkv-0.8.7/src/rwkv/utils.py` & `rwkv-0.8.8/src/rwkv/utils.py`

 * *Files identical despite different names*

### Comparing `rwkv-0.8.7/src/rwkv.egg-info/PKG-INFO` & `rwkv-0.8.8/src/rwkv.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rwkv
-Version: 0.8.7
+Version: 0.8.8
 Summary: The RWKV Language Model
 Author: Bo PENG
 Project-URL: Homepage, https://github.com/BlinkDL/ChatRWKV
 Project-URL: Bug Tracker, https://github.com/BlinkDL/ChatRWKV/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

