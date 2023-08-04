# Comparing `tmp/onnx-safetensors-0.1.0.tar.gz` & `tmp/onnx-safetensors-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onnx-safetensors-0.1.0.tar", last modified: Wed Aug  2 16:10:17 2023, max compression
+gzip compressed data, was "onnx-safetensors-0.1.1.tar", last modified: Fri Aug  4 04:02:51 2023, max compression
```

## Comparing `onnx-safetensors-0.1.0.tar` & `onnx-safetensors-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:10:17.699046 onnx-safetensors-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-08-02 16:10:06.000000 onnx-safetensors-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-08-02 16:10:17.699046 onnx-safetensors-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-08-02 16:10:06.000000 onnx-safetensors-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:10:17.699046 onnx-safetensors-0.1.0/onnx_safetensors/
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-08-02 16:10:06.000000 onnx-safetensors-0.1.0/onnx_safetensors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6406 2023-08-02 16:10:06.000000 onnx-safetensors-0.1.0/onnx_safetensors/_safetensors_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     5301 2023-08-02 16:10:06.000000 onnx-safetensors-0.1.0/onnx_safetensors/_safetensors_io_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-08-02 16:10:06.000000 onnx-safetensors-0.1.0/onnx_safetensors/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:10:17.699046 onnx-safetensors-0.1.0/onnx_safetensors.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-08-02 16:10:17.000000 onnx-safetensors-0.1.0/onnx_safetensors.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-08-02 16:10:17.000000 onnx-safetensors-0.1.0/onnx_safetensors.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 16:10:17.000000 onnx-safetensors-0.1.0/onnx_safetensors.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-02 16:10:17.000000 onnx-safetensors-0.1.0/onnx_safetensors.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-02 16:10:17.000000 onnx-safetensors-0.1.0/onnx_safetensors.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-08-02 16:10:06.000000 onnx-safetensors-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 16:10:17.699046 onnx-safetensors-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 04:02:51.301199 onnx-safetensors-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-08-04 04:02:39.000000 onnx-safetensors-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-08-04 04:02:51.301199 onnx-safetensors-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-08-04 04:02:39.000000 onnx-safetensors-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 04:02:51.301199 onnx-safetensors-0.1.1/onnx_safetensors/
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-08-04 04:02:39.000000 onnx-safetensors-0.1.1/onnx_safetensors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6406 2023-08-04 04:02:39.000000 onnx-safetensors-0.1.1/onnx_safetensors/_safetensors_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5301 2023-08-04 04:02:39.000000 onnx-safetensors-0.1.1/onnx_safetensors/_safetensors_io_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-08-04 04:02:39.000000 onnx-safetensors-0.1.1/onnx_safetensors/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 04:02:51.301199 onnx-safetensors-0.1.1/onnx_safetensors.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-08-04 04:02:51.000000 onnx-safetensors-0.1.1/onnx_safetensors.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-08-04 04:02:51.000000 onnx-safetensors-0.1.1/onnx_safetensors.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 04:02:51.000000 onnx-safetensors-0.1.1/onnx_safetensors.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-04 04:02:51.000000 onnx-safetensors-0.1.1/onnx_safetensors.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-04 04:02:51.000000 onnx-safetensors-0.1.1/onnx_safetensors.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-08-04 04:02:39.000000 onnx-safetensors-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 04:02:51.305199 onnx-safetensors-0.1.1/setup.cfg
```

### Comparing `onnx-safetensors-0.1.0/LICENSE` & `onnx-safetensors-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `onnx-safetensors-0.1.0/onnx_safetensors/_safetensors_io.py` & `onnx-safetensors-0.1.1/onnx_safetensors/_safetensors_io.py`

 * *Files identical despite different names*

### Comparing `onnx-safetensors-0.1.0/onnx_safetensors/_safetensors_io_test.py` & `onnx-safetensors-0.1.1/onnx_safetensors/_safetensors_io_test.py`

 * *Files identical despite different names*

### Comparing `onnx-safetensors-0.1.0/onnx_safetensors/utils.py` & `onnx-safetensors-0.1.1/onnx_safetensors/utils.py`

 * *Files identical despite different names*

### Comparing `onnx-safetensors-0.1.0/pyproject.toml` & `onnx-safetensors-0.1.1/pyproject.toml`

 * *Files identical despite different names*

