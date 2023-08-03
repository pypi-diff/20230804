# Comparing `tmp/fmetools-0.7.1.tar.gz` & `tmp/fmetools-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fmetools-0.7.1.tar", last modified: Wed Jul 19 23:54:24 2023, max compression
+gzip compressed data, was "fmetools-0.7.3.tar", last modified: Thu Aug  3 23:32:33 2023, max compression
```

## Comparing `fmetools-0.7.1.tar` & `fmetools-0.7.3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 23:54:24.110852 fmetools-0.7.1/
--rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-07-19 23:54:11.000000 fmetools-0.7.1/CHANGES.md
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-07-19 23:54:11.000000 fmetools-0.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-19 23:54:11.000000 fmetools-0.7.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4682 2023-07-19 23:54:24.110852 fmetools-0.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-07-19 23:54:11.000000 fmetools-0.7.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-19 23:54:11.000000 fmetools-0.7.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-19 23:54:24.110852 fmetools-0.7.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 23:54:24.106852 fmetools-0.7.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 23:54:24.110852 fmetools-0.7.1/src/fmetools/
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-19 23:54:11.000000 fmetools-0.7.1/src/fmetools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8175 2023-07-19 23:54:11.000000 fmetools-0.7.1/src/fmetools/features.py
--rw-r--r--   0 runner    (1001) docker     (123)     6477 2023-07-19 23:54:11.000000 fmetools-0.7.1/src/fmetools/guiparams.py
--rw-r--r--   0 runner    (1001) docker     (123)    25690 2023-07-19 23:54:11.000000 fmetools-0.7.1/src/fmetools/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-07-19 23:54:11.000000 fmetools-0.7.1/src/fmetools/localize.py
--rw-r--r--   0 runner    (1001) docker     (123)     3361 2023-07-19 23:54:11.000000 fmetools-0.7.1/src/fmetools/logfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     8524 2023-07-19 23:54:11.000000 fmetools-0.7.1/src/fmetools/paramparsing.py
--rw-r--r--   0 runner    (1001) docker     (123)    11982 2023-07-19 23:54:11.000000 fmetools-0.7.1/src/fmetools/parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)    24775 2023-07-19 23:54:11.000000 fmetools-0.7.1/src/fmetools/plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-07-19 23:54:11.000000 fmetools-0.7.1/src/fmetools/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9386 2023-07-19 23:54:11.000000 fmetools-0.7.1/src/fmetools/webservices.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 23:54:24.110852 fmetools-0.7.1/src/fmetools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4682 2023-07-19 23:54:24.000000 fmetools-0.7.1/src/fmetools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-07-19 23:54:24.000000 fmetools-0.7.1/src/fmetools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 23:54:24.000000 fmetools-0.7.1/src/fmetools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-19 23:54:24.000000 fmetools-0.7.1/src/fmetools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-19 23:54:24.000000 fmetools-0.7.1/src/fmetools.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 23:54:24.110852 fmetools-0.7.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4106 2023-07-19 23:54:11.000000 fmetools-0.7.1/tests/test_features.py
--rw-r--r--   0 runner    (1001) docker     (123)    11161 2023-07-19 23:54:11.000000 fmetools-0.7.1/tests/test_fmehttp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-07-19 23:54:11.000000 fmetools-0.7.1/tests/test_guiparams.py
--rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-07-19 23:54:11.000000 fmetools-0.7.1/tests/test_logfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     4606 2023-07-19 23:54:11.000000 fmetools-0.7.1/tests/test_paramparsing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-07-19 23:54:11.000000 fmetools-0.7.1/tests/test_parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-07-19 23:54:11.000000 fmetools-0.7.1/tests/test_plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 23:32:33.945150 fmetools-0.7.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-08-03 23:32:18.000000 fmetools-0.7.3/CHANGES.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-08-03 23:32:18.000000 fmetools-0.7.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-08-03 23:32:18.000000 fmetools-0.7.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4938 2023-08-03 23:32:33.945150 fmetools-0.7.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-08-03 23:32:18.000000 fmetools-0.7.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 23:32:18.000000 fmetools-0.7.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-08-03 23:32:33.949149 fmetools-0.7.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 23:32:33.941150 fmetools-0.7.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 23:32:33.945150 fmetools-0.7.3/src/fmetools/
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-08-03 23:32:18.000000 fmetools-0.7.3/src/fmetools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8175 2023-08-03 23:32:18.000000 fmetools-0.7.3/src/fmetools/features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6477 2023-08-03 23:32:18.000000 fmetools-0.7.3/src/fmetools/guiparams.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25690 2023-08-03 23:32:18.000000 fmetools-0.7.3/src/fmetools/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-08-03 23:32:18.000000 fmetools-0.7.3/src/fmetools/localize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3361 2023-08-03 23:32:18.000000 fmetools-0.7.3/src/fmetools/logfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8524 2023-08-03 23:32:18.000000 fmetools-0.7.3/src/fmetools/paramparsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11982 2023-08-03 23:32:18.000000 fmetools-0.7.3/src/fmetools/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24904 2023-08-03 23:32:18.000000 fmetools-0.7.3/src/fmetools/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-08-03 23:32:18.000000 fmetools-0.7.3/src/fmetools/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9386 2023-08-03 23:32:18.000000 fmetools-0.7.3/src/fmetools/webservices.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 23:32:33.945150 fmetools-0.7.3/src/fmetools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4938 2023-08-03 23:32:33.000000 fmetools-0.7.3/src/fmetools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-08-03 23:32:33.000000 fmetools-0.7.3/src/fmetools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 23:32:33.000000 fmetools-0.7.3/src/fmetools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-08-03 23:32:33.000000 fmetools-0.7.3/src/fmetools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-03 23:32:33.000000 fmetools-0.7.3/src/fmetools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 23:32:33.945150 fmetools-0.7.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4106 2023-08-03 23:32:18.000000 fmetools-0.7.3/tests/test_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11161 2023-08-03 23:32:18.000000 fmetools-0.7.3/tests/test_fmehttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-08-03 23:32:18.000000 fmetools-0.7.3/tests/test_guiparams.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-08-03 23:32:18.000000 fmetools-0.7.3/tests/test_logfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4606 2023-08-03 23:32:18.000000 fmetools-0.7.3/tests/test_paramparsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-08-03 23:32:18.000000 fmetools-0.7.3/tests/test_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-08-03 23:32:18.000000 fmetools-0.7.3/tests/test_plugins.py
```

### Comparing `fmetools-0.7.1/CHANGES.md` & `fmetools-0.7.3/CHANGES.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,17 @@
 # fmetools changes
 
+## 0.7.3
+
+* Add links to HTML docs.
+
+## 0.7.2
+
+* Relax FME version requirements from 0.7.0 release.
+
 ## 0.7.1
 
 * Fix type annotations when using Python 3.8 and earlier.
 
 ## 0.7.0
 
 * Add HTML docs and expanded existing docstrings.
```

### Comparing `fmetools-0.7.1/LICENSE` & `fmetools-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fmetools-0.7.1/PKG-INFO` & `fmetools-0.7.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: fmetools
-Version: 0.7.1
+Version: 0.7.3
 Summary: Tools for extending Safe Software's FME using Python.
 Home-page: https://github.com/safesoftware/fmetools
 Author: Safe Software Inc.
 License: BSD
+Project-URL: Documentation, https://docs.safe.com/fme/html/fmetools/
 Keywords: FME fmeobjects
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -29,14 +30,16 @@
 and requires an FME installation with Python 3.7 or newer.
 
 ## Getting started
 
 The best way to get started with fmetools is through the tutorials in the [FME Packages SDK Guide][fpkg-sdk].
 The [Hello World package tutorial][hello world] guides you through creating a simple FME Package that uses fmetools.
 
+The fmetools API reference is available at https://docs.safe.com/fme/html/fmetools/.
+
 [fme]: https://safe.com
 [hub]: https://hub.safe.com
 [fpkg-sdk]: https://docs.safe.com/fme/html/fpkg-sdk/
 [hello world]: https://docs.safe.com/fme/html/fpkg-sdk/hello-world-package/
 [vendorize]: https://pypi.org/project/vendorize/
 [fmeobjects]: https://docs.safe.com/fme/html/fmepython/index.html
 
@@ -57,14 +60,22 @@
 2. Install dev requirements using `pip install -r requirements.txt`
 3. Do a dev install using `pip install --editable .`
 4. Run tests using `pytest`
 5. Build wheel using `python -m build --wheel`
 
 # fmetools changes
 
+## 0.7.3
+
+* Add links to HTML docs.
+
+## 0.7.2
+
+* Relax FME version requirements from 0.7.0 release.
+
 ## 0.7.1
 
 * Fix type annotations when using Python 3.8 and earlier.
 
 ## 0.7.0
 
 * Add HTML docs and expanded existing docstrings.
```

### Comparing `fmetools-0.7.1/README.md` & `fmetools-0.7.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 and requires an FME installation with Python 3.7 or newer.
 
 ## Getting started
 
 The best way to get started with fmetools is through the tutorials in the [FME Packages SDK Guide][fpkg-sdk].
 The [Hello World package tutorial][hello world] guides you through creating a simple FME Package that uses fmetools.
 
+The fmetools API reference is available at https://docs.safe.com/fme/html/fmetools/.
+
 [fme]: https://safe.com
 [hub]: https://hub.safe.com
 [fpkg-sdk]: https://docs.safe.com/fme/html/fpkg-sdk/
 [hello world]: https://docs.safe.com/fme/html/fpkg-sdk/hello-world-package/
 [vendorize]: https://pypi.org/project/vendorize/
 [fmeobjects]: https://docs.safe.com/fme/html/fmepython/index.html
```

### Comparing `fmetools-0.7.1/setup.cfg` & `fmetools-0.7.3/setup.cfg`

 * *Files 17% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 version = attr: fmetools.__version__
 author = Safe Software Inc.
 description = Tools for extending Safe Software's FME using Python.
 long_description = file: README.md, CHANGES.md
 long_description_content_type = text/markdown
 keywords = FME fmeobjects
 url = https://github.com/safesoftware/fmetools
+project_urls = 
+	Documentation = https://docs.safe.com/fme/html/fmetools/
 license = BSD
 license_file = LICENSE
 classifiers = 
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
```

### Comparing `fmetools-0.7.1/src/fmetools/features.py` & `fmetools-0.7.3/src/fmetools/features.py`

 * *Files identical despite different names*

### Comparing `fmetools-0.7.1/src/fmetools/guiparams.py` & `fmetools-0.7.3/src/fmetools/guiparams.py`

 * *Files identical despite different names*

### Comparing `fmetools-0.7.1/src/fmetools/http.py` & `fmetools-0.7.3/src/fmetools/http.py`

 * *Files identical despite different names*

### Comparing `fmetools-0.7.1/src/fmetools/localize.py` & `fmetools-0.7.3/src/fmetools/localize.py`

 * *Files identical despite different names*

### Comparing `fmetools-0.7.1/src/fmetools/logfile.py` & `fmetools-0.7.3/src/fmetools/logfile.py`

 * *Files identical despite different names*

### Comparing `fmetools-0.7.1/src/fmetools/paramparsing.py` & `fmetools-0.7.3/src/fmetools/paramparsing.py`

 * *Files identical despite different names*

### Comparing `fmetools-0.7.1/src/fmetools/parsers.py` & `fmetools-0.7.3/src/fmetools/parsers.py`

 * *Files identical despite different names*

### Comparing `fmetools-0.7.1/src/fmetools/plugins.py` & `fmetools-0.7.3/src/fmetools/plugins.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,21 @@
 
 :class:`FMEEnhancedTransformer` is the recommended base class for transformers.
 Transformer developers should subclass it to implement their own transformers.
 """
 import logging
 import warnings
 
-from fmeobjects import FME_SUPPORT_FEATURE_TABLE_SHIM, FMEFeature
+from fmeobjects import FMEFeature
+
+try:
+    from fmeobjects import FME_SUPPORT_FEATURE_TABLE_SHIM
+except ImportError:  # Support < FME 2022.0 b22235
+    FME_SUPPORT_FEATURE_TABLE_SHIM = 0
+
 from pluginbuilder import FMEReader, FMEWriter
 
 from .logfile import get_configured_logger
 from .parsers import MappingFile, OpenParameters
 
 # These are relevant externally.
 # Reader and writer base classes are omitted because they're not intended for general use.
```

### Comparing `fmetools-0.7.1/src/fmetools/utils.py` & `fmetools-0.7.3/src/fmetools/utils.py`

 * *Files identical despite different names*

### Comparing `fmetools-0.7.1/src/fmetools/webservices.py` & `fmetools-0.7.3/src/fmetools/webservices.py`

 * *Files identical despite different names*

### Comparing `fmetools-0.7.1/src/fmetools.egg-info/PKG-INFO` & `fmetools-0.7.3/src/fmetools.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: fmetools
-Version: 0.7.1
+Version: 0.7.3
 Summary: Tools for extending Safe Software's FME using Python.
 Home-page: https://github.com/safesoftware/fmetools
 Author: Safe Software Inc.
 License: BSD
+Project-URL: Documentation, https://docs.safe.com/fme/html/fmetools/
 Keywords: FME fmeobjects
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -29,14 +30,16 @@
 and requires an FME installation with Python 3.7 or newer.
 
 ## Getting started
 
 The best way to get started with fmetools is through the tutorials in the [FME Packages SDK Guide][fpkg-sdk].
 The [Hello World package tutorial][hello world] guides you through creating a simple FME Package that uses fmetools.
 
+The fmetools API reference is available at https://docs.safe.com/fme/html/fmetools/.
+
 [fme]: https://safe.com
 [hub]: https://hub.safe.com
 [fpkg-sdk]: https://docs.safe.com/fme/html/fpkg-sdk/
 [hello world]: https://docs.safe.com/fme/html/fpkg-sdk/hello-world-package/
 [vendorize]: https://pypi.org/project/vendorize/
 [fmeobjects]: https://docs.safe.com/fme/html/fmepython/index.html
 
@@ -57,14 +60,22 @@
 2. Install dev requirements using `pip install -r requirements.txt`
 3. Do a dev install using `pip install --editable .`
 4. Run tests using `pytest`
 5. Build wheel using `python -m build --wheel`
 
 # fmetools changes
 
+## 0.7.3
+
+* Add links to HTML docs.
+
+## 0.7.2
+
+* Relax FME version requirements from 0.7.0 release.
+
 ## 0.7.1
 
 * Fix type annotations when using Python 3.8 and earlier.
 
 ## 0.7.0
 
 * Add HTML docs and expanded existing docstrings.
```

### Comparing `fmetools-0.7.1/src/fmetools.egg-info/SOURCES.txt` & `fmetools-0.7.3/src/fmetools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fmetools-0.7.1/tests/test_features.py` & `fmetools-0.7.3/tests/test_features.py`

 * *Files identical despite different names*

### Comparing `fmetools-0.7.1/tests/test_fmehttp.py` & `fmetools-0.7.3/tests/test_fmehttp.py`

 * *Files identical despite different names*

### Comparing `fmetools-0.7.1/tests/test_guiparams.py` & `fmetools-0.7.3/tests/test_guiparams.py`

 * *Files identical despite different names*

### Comparing `fmetools-0.7.1/tests/test_logfile.py` & `fmetools-0.7.3/tests/test_logfile.py`

 * *Files identical despite different names*

### Comparing `fmetools-0.7.1/tests/test_paramparsing.py` & `fmetools-0.7.3/tests/test_paramparsing.py`

 * *Files identical despite different names*

### Comparing `fmetools-0.7.1/tests/test_parsers.py` & `fmetools-0.7.3/tests/test_parsers.py`

 * *Files identical despite different names*

### Comparing `fmetools-0.7.1/tests/test_plugins.py` & `fmetools-0.7.3/tests/test_plugins.py`

 * *Files identical despite different names*

