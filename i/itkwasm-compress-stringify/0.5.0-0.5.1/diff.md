# Comparing `tmp/itkwasm_compress_stringify-0.5.0.tar.gz` & `tmp/itkwasm_compress_stringify-0.5.1.tar.gz`

## Comparing `itkwasm_compress_stringify-0.5.0.tar` & `itkwasm_compress_stringify-0.5.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-0.5.0/docs/Makefile
--rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-0.5.0/docs/conf.py
--rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-0.5.0/docs/index.md
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-0.5.0/docs/make.bat
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-0.5.0/docs/requirements.txt
--rw-r--r--   0        0        0    13605 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-0.5.0/docs/_static/favicon.png
--rw-r--r--   0        0        0     2949 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-0.5.0/docs/_static/logo.svg
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-0.5.0/itkwasm_compress_stringify/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-0.5.0/itkwasm_compress_stringify/_version.py
--rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-0.5.0/itkwasm_compress_stringify/compress_stringify.py
--rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-0.5.0/itkwasm_compress_stringify/compress_stringify_async.py
--rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-0.5.0/itkwasm_compress_stringify/parse_string_decompress.py
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-0.5.0/itkwasm_compress_stringify/parse_string_decompress_async.py
--rw-r--r--   0        0        0     2562 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-0.5.0/test/test_compress_stringify_emscripten.py
--rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-0.5.0/test/test_compress_stringify_wasi.py
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-0.5.0/.gitignore
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-0.5.0/README.md
--rw-r--r--   0        0        0     2045 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-0.5.1/docs/Makefile
+-rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-0.5.1/docs/conf.py
+-rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-0.5.1/docs/index.md
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-0.5.1/docs/make.bat
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-0.5.1/docs/requirements.txt
+-rw-r--r--   0        0        0    13605 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-0.5.1/docs/_static/favicon.png
+-rw-r--r--   0        0        0     2949 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-0.5.1/docs/_static/logo.svg
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-0.5.1/itkwasm_compress_stringify/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-0.5.1/itkwasm_compress_stringify/_version.py
+-rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-0.5.1/itkwasm_compress_stringify/compress_stringify.py
+-rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-0.5.1/itkwasm_compress_stringify/compress_stringify_async.py
+-rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-0.5.1/itkwasm_compress_stringify/parse_string_decompress.py
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-0.5.1/itkwasm_compress_stringify/parse_string_decompress_async.py
+-rw-r--r--   0        0        0     2562 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-0.5.1/test/test_compress_stringify_emscripten.py
+-rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-0.5.1/test/test_compress_stringify_wasi.py
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-0.5.1/.gitignore
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-0.5.1/README.md
+-rw-r--r--   0        0        0     2045 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-0.5.1/PKG-INFO
```

### Comparing `itkwasm_compress_stringify-0.5.0/docs/Makefile` & `itkwasm_compress_stringify-0.5.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `itkwasm_compress_stringify-0.5.0/docs/conf.py` & `itkwasm_compress_stringify-0.5.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `itkwasm_compress_stringify-0.5.0/docs/index.md` & `itkwasm_compress_stringify-0.5.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `itkwasm_compress_stringify-0.5.0/docs/make.bat` & `itkwasm_compress_stringify-0.5.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `itkwasm_compress_stringify-0.5.0/docs/_static/favicon.png` & `itkwasm_compress_stringify-0.5.1/docs/_static/favicon.png`

 * *Files identical despite different names*

### Comparing `itkwasm_compress_stringify-0.5.0/docs/_static/logo.svg` & `itkwasm_compress_stringify-0.5.1/docs/_static/logo.svg`

 * *Files identical despite different names*

### Comparing `itkwasm_compress_stringify-0.5.0/itkwasm_compress_stringify/compress_stringify.py` & `itkwasm_compress_stringify-0.5.1/itkwasm_compress_stringify/compress_stringify.py`

 * *Files identical despite different names*

### Comparing `itkwasm_compress_stringify-0.5.0/itkwasm_compress_stringify/compress_stringify_async.py` & `itkwasm_compress_stringify-0.5.1/itkwasm_compress_stringify/compress_stringify_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_compress_stringify-0.5.0/itkwasm_compress_stringify/parse_string_decompress.py` & `itkwasm_compress_stringify-0.5.1/itkwasm_compress_stringify/parse_string_decompress.py`

 * *Files identical despite different names*

### Comparing `itkwasm_compress_stringify-0.5.0/itkwasm_compress_stringify/parse_string_decompress_async.py` & `itkwasm_compress_stringify-0.5.1/itkwasm_compress_stringify/parse_string_decompress_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_compress_stringify-0.5.0/test/test_compress_stringify_emscripten.py` & `itkwasm_compress_stringify-0.5.1/test/test_compress_stringify_emscripten.py`

 * *Files identical despite different names*

### Comparing `itkwasm_compress_stringify-0.5.0/test/test_compress_stringify_wasi.py` & `itkwasm_compress_stringify-0.5.1/test/test_compress_stringify_wasi.py`

 * *Files identical despite different names*

### Comparing `itkwasm_compress_stringify-0.5.0/pyproject.toml` & `itkwasm_compress_stringify-0.5.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `itkwasm_compress_stringify-0.5.0/PKG-INFO` & `itkwasm_compress_stringify-0.5.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: itkwasm-compress-stringify
-Version: 0.5.0
+Version: 0.5.1
 Project-URL: Home, https://itk-wasm-compress-stringify-python-docs.on.fleek.co
 Project-URL: Source, https://github.com/InsightSoftwareConsortium/itk-wasm
 Project-URL: Issues, https://github.com/InsightSoftwareConsortium/itk-wasm/issues
 License-Expression: Apache-2.0
 Keywords: emscripten,itkwasm,wasi,webassembly
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: WebAssembly
```

