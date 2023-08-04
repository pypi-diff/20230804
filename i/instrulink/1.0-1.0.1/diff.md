# Comparing `tmp/instrulink-1.0.tar.gz` & `tmp/instrulink-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "instrulink-1.0.tar", last modified: Wed May 17 19:15:15 2023, max compression
+gzip compressed data, was "instrulink-1.0.1.tar", last modified: Fri Aug  4 21:06:54 2023, max compression
```

## Comparing `instrulink-1.0.tar` & `instrulink-1.0.1.tar`

### file list

```diff
@@ -1,41 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:15:15.639804 instrulink-1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-17 19:14:59.000000 instrulink-1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-17 19:14:59.000000 instrulink-1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-05-17 19:15:15.639804 instrulink-1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-05-17 19:14:59.000000 instrulink-1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:15:15.639804 instrulink-1.0/instrulink/
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-17 19:14:59.000000 instrulink-1.0/instrulink/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31551 2023-05-17 19:14:59.000000 instrulink-1.0/instrulink/bk_2555.py
--rw-r--r--   0 runner    (1001) docker     (123)    21215 2023-05-17 19:14:59.000000 instrulink-1.0/instrulink/camera.py
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-17 19:14:59.000000 instrulink-1.0/instrulink/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-05-17 19:14:59.000000 instrulink-1.0/instrulink/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-05-17 19:14:59.000000 instrulink-1.0/instrulink/keysight_e5061b.py
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-05-17 19:14:59.000000 instrulink-1.0/instrulink/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     9190 2023-05-17 19:14:59.000000 instrulink-1.0/instrulink/nidaq.py
--rw-r--r--   0 runner    (1001) docker     (123)    14824 2023-05-17 19:14:59.000000 instrulink-1.0/instrulink/oscilloscope.py
--rw-r--r--   0 runner    (1001) docker     (123)    17859 2023-05-17 19:14:59.000000 instrulink-1.0/instrulink/rigol_dg1022z.py
--rw-r--r--   0 runner    (1001) docker     (123)    25707 2023-05-17 19:14:59.000000 instrulink-1.0/instrulink/rigol_ds1054z.py
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-05-17 19:14:59.000000 instrulink-1.0/instrulink/si_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    16427 2023-05-17 19:14:59.000000 instrulink-1.0/instrulink/sutter_mp285a.py
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-05-17 19:14:59.000000 instrulink-1.0/instrulink/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9976 2023-05-17 19:14:59.000000 instrulink-1.0/instrulink/visa_instrument.py
--rw-r--r--   0 runner    (1001) docker     (123)    14224 2023-05-17 19:14:59.000000 instrulink-1.0/instrulink/waveform_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-05-17 19:14:59.000000 instrulink-1.0/instrulink/wf_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:15:15.639804 instrulink-1.0/instrulink.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-05-17 19:15:15.000000 instrulink-1.0/instrulink.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-05-17 19:15:15.000000 instrulink-1.0/instrulink.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 19:15:15.000000 instrulink-1.0/instrulink.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 19:15:15.000000 instrulink-1.0/instrulink.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-17 19:15:15.000000 instrulink-1.0/instrulink.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-17 19:15:15.000000 instrulink-1.0/instrulink.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-17 19:14:59.000000 instrulink-1.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:15:15.639804 instrulink-1.0/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-17 19:14:59.000000 instrulink-1.0/scripts/list_visa_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-17 19:14:59.000000 instrulink-1.0/scripts/test_camera.py
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-05-17 19:14:59.000000 instrulink-1.0/scripts/test_e5061b.py
--rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-05-17 19:14:59.000000 instrulink-1.0/scripts/test_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-05-17 19:14:59.000000 instrulink-1.0/scripts/test_manipulator.py
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-17 19:14:59.000000 instrulink-1.0/scripts/test_nidaq.py
--rw-r--r--   0 runner    (1001) docker     (123)     5506 2023-05-17 19:14:59.000000 instrulink-1.0/scripts/test_scope.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 19:15:15.639804 instrulink-1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-05-17 19:14:59.000000 instrulink-1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:06:54.744891 instrulink-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 21:06:44.000000 instrulink-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-08-04 21:06:44.000000 instrulink-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-08-04 21:06:54.744891 instrulink-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-08-04 21:06:44.000000 instrulink-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:06:54.740891 instrulink-1.0.1/instrulink/
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-08-04 21:06:44.000000 instrulink-1.0.1/instrulink/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31551 2023-08-04 21:06:44.000000 instrulink-1.0.1/instrulink/bk_2555.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21215 2023-08-04 21:06:44.000000 instrulink-1.0.1/instrulink/camera.py
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-08-04 21:06:44.000000 instrulink-1.0.1/instrulink/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-08-04 21:06:44.000000 instrulink-1.0.1/instrulink/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9647 2023-08-04 21:06:44.000000 instrulink-1.0.1/instrulink/keysight_33500b.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-08-04 21:06:44.000000 instrulink-1.0.1/instrulink/keysight_e5061b.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-08-04 21:06:44.000000 instrulink-1.0.1/instrulink/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9190 2023-08-04 21:06:44.000000 instrulink-1.0.1/instrulink/nidaq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14824 2023-08-04 21:06:44.000000 instrulink-1.0.1/instrulink/oscilloscope.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43554 2023-08-04 21:06:44.000000 instrulink-1.0.1/instrulink/rigol_dg1022z.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25707 2023-08-04 21:06:44.000000 instrulink-1.0.1/instrulink/rigol_ds1054z.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-08-04 21:06:44.000000 instrulink-1.0.1/instrulink/si_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16427 2023-08-04 21:06:44.000000 instrulink-1.0.1/instrulink/sutter_mp285a.py
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-08-04 21:06:44.000000 instrulink-1.0.1/instrulink/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9976 2023-08-04 21:06:44.000000 instrulink-1.0.1/instrulink/visa_instrument.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15513 2023-08-04 21:06:44.000000 instrulink-1.0.1/instrulink/waveform_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13797 2023-08-04 21:06:44.000000 instrulink-1.0.1/instrulink/wf_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:06:54.740891 instrulink-1.0.1/instrulink.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-08-04 21:06:54.000000 instrulink-1.0.1/instrulink.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-08-04 21:06:54.000000 instrulink-1.0.1/instrulink.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 21:06:54.000000 instrulink-1.0.1/instrulink.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 21:06:54.000000 instrulink-1.0.1/instrulink.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-08-04 21:06:54.000000 instrulink-1.0.1/instrulink.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-04 21:06:54.000000 instrulink-1.0.1/instrulink.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-08-04 21:06:44.000000 instrulink-1.0.1/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:06:54.744891 instrulink-1.0.1/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-08-04 21:06:44.000000 instrulink-1.0.1/scripts/list_visa_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-08-04 21:06:44.000000 instrulink-1.0.1/scripts/test_33500b.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-08-04 21:06:44.000000 instrulink-1.0.1/scripts/test_camera.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-08-04 21:06:44.000000 instrulink-1.0.1/scripts/test_e5061b.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-08-04 21:06:44.000000 instrulink-1.0.1/scripts/test_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-08-04 21:06:44.000000 instrulink-1.0.1/scripts/test_manipulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-08-04 21:06:44.000000 instrulink-1.0.1/scripts/test_nidaq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5506 2023-08-04 21:06:44.000000 instrulink-1.0.1/scripts/test_scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-08-04 21:06:44.000000 instrulink-1.0.1/scripts/test_smoothed_waveform.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 21:06:54.744891 instrulink-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-08-04 21:06:44.000000 instrulink-1.0.1/setup.py
```

### Comparing `instrulink-1.0/LICENSE` & `instrulink-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `instrulink-1.0/PKG-INFO` & `instrulink-1.0.1/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,41 +1,45 @@
-Metadata-Version: 2.1
-Name: instrulink
-Version: 1.0
-Summary: Python package to interface diverse laboratory instruments
-Home-page: https://github.com/tjjlemaire/instrulink
-Author: Theo Lemaire
-Author-email: theo.lemaire1@gmail.com
-License: MIT
-Keywords: laboratory instrument interface python
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Science/Research
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Scientific/Engineering :: Physics
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # instrulink
 
 This python package provides built-in classes to interface diverse laboratory instruments, including:
 - **waveform generators**: [Rigol DG 1022Z](https://www.rigolna.com/products/waveform-generators/dg1000z/) (`RigolDG1022Z`)
 - **oscilloscopes**: [B&K Precision 2555](https://www.bkprecision.com/products/oscilloscopes/2555) (`BK2555`), [Rigol DS 1054Z](https://www.rigolna.com/products/digital-oscilloscopes/1000z/) (`RigolDS1054Z`)
 - **micro-manipulators**: [Sutter Instruments MP-285A](https://www.sutter.com/MICROMANIPULATION/mp285_frame.html) (`SutterMP285A`)
 - **infrared cameras**: FLIR cameras (`Camera`)
 - **acquisition systems**: [NI DAQmx](https://www.ni.com/docs/en-US/bundle/ni-daqmx/page/daqhelp/nidaqoverview.html) for pulse triggers
 
-## Requirements
+## Software dependencies
+
+To interface VISA instruments (i.e., waveforms generators and oscilloscopes), you will need to:
+- Download and install [IVI Compliance Package 21.0](https://www.ni.com/en-us/support/downloads/drivers/download.ivi-compliance-package.html#460618)
+  When installing, opt to include .NET Adapters and COM adapters as well (these are not selected by default)
+- Download and install the [NI Package Manager](https://www.ni.com/en-us/support/downloads/software-products/download.package-manager.html#322516). Through the NI package manager, also install the NI-VISA Driver.
+
+To interface Rigol instruments specifically, you will also need to download and install the associated [Rigol driver](https://www.rigolna.com/products/waveform-generators/dg1000z/)
 
-- [FlyCapture SDK](https://www.flir.com/products/flycapture-sdk/) (to use the FLIR camera interface class)
-- Anaconda
-- Python 3.6 (for compliance with FlyCapture SDK)
+To interface FLIR cameras, you will need to download and install the [FlyCapture SDK](https://www.flir.com/products/flycapture-sdk/)
+
+You will also need to install `Python 3.6` (for compliance with FlyCapture SDK), preferably as part of an environment manager such as [Anaconda](https://www.anaconda.com/products/individual).
 
 ## Installation
 
-- Clone this repository: `git clone https://github.com/tjjlemaire/instrulink.git`
-- Move to that directory (`cd instrulink`) and install it as a python package: `pip install -e .`
+This package can be directly installed from PyPI:
+
+```pip install instrulink```
+
+However, if you wish to amend the package code, you can also clone this repo and install it locally as an editable package: 
+
+```
+git clone https://github.com/tjjlemaire/instrulink.git
+cd instrulink
+pip install -e .
+```
 
 ## Usage
 
-Instruments can be easily accessed via generic `grab_camera`, `grab_generator`, `grab_oscilloscope` and `grab_manipulator` functions. By default, these functions will automatically detect the first available instrument connected to the PC. Optionally, you can also provide an instrument `key` to connect to a specific model type (e.g. `grab_osciloscope(key='bk')` to specifically connect to a B&K Precision oscilloscope).
+### Connecting to instruments
+
+Instruments can be easily connected to via generic `grab_camera`, `grab_generator`, `grab_oscilloscope` and `grab_manipulator` functions. By default, these functions will automatically detect the first available instrument connected to the PC. Optionally, you can also provide an instrument `key` to connect to a specific model type (e.g. `grab_osciloscope(key='bk')` to specifically connect to a B&K Precision oscilloscope).
+
+### Using instruments
 
 Example scripts are located in the `/scripts` subfolder.
```

### Comparing `instrulink-1.0/README.md` & `instrulink-1.0.1/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,25 +1,61 @@
+Metadata-Version: 2.1
+Name: instrulink
+Version: 1.0.1
+Summary: Python package to interface diverse laboratory instruments
+Home-page: https://github.com/tjjlemaire/instrulink
+Author: Theo Lemaire
+Author-email: theo.lemaire1@gmail.com
+License: MIT
+Keywords: laboratory instrument interface python
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Science/Research
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Scientific/Engineering :: Physics
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # instrulink
 
 This python package provides built-in classes to interface diverse laboratory instruments, including:
 - **waveform generators**: [Rigol DG 1022Z](https://www.rigolna.com/products/waveform-generators/dg1000z/) (`RigolDG1022Z`)
 - **oscilloscopes**: [B&K Precision 2555](https://www.bkprecision.com/products/oscilloscopes/2555) (`BK2555`), [Rigol DS 1054Z](https://www.rigolna.com/products/digital-oscilloscopes/1000z/) (`RigolDS1054Z`)
 - **micro-manipulators**: [Sutter Instruments MP-285A](https://www.sutter.com/MICROMANIPULATION/mp285_frame.html) (`SutterMP285A`)
 - **infrared cameras**: FLIR cameras (`Camera`)
 - **acquisition systems**: [NI DAQmx](https://www.ni.com/docs/en-US/bundle/ni-daqmx/page/daqhelp/nidaqoverview.html) for pulse triggers
 
-## Requirements
+## Software dependencies
+
+To interface VISA instruments (i.e., waveforms generators and oscilloscopes), you will need to:
+- Download and install [IVI Compliance Package 21.0](https://www.ni.com/en-us/support/downloads/drivers/download.ivi-compliance-package.html#460618)
+  When installing, opt to include .NET Adapters and COM adapters as well (these are not selected by default)
+- Download and install the [NI Package Manager](https://www.ni.com/en-us/support/downloads/software-products/download.package-manager.html#322516). Through the NI package manager, also install the NI-VISA Driver.
+
+To interface Rigol instruments specifically, you will also need to download and install the associated [Rigol driver](https://www.rigolna.com/products/waveform-generators/dg1000z/)
 
-- [FlyCapture SDK](https://www.flir.com/products/flycapture-sdk/) (to use the FLIR camera interface class)
-- Anaconda
-- Python 3.6 (for compliance with FlyCapture SDK)
+To interface FLIR cameras, you will need to download and install the [FlyCapture SDK](https://www.flir.com/products/flycapture-sdk/)
+
+You will also need to install `Python 3.6` (for compliance with FlyCapture SDK), preferably as part of an environment manager such as [Anaconda](https://www.anaconda.com/products/individual).
 
 ## Installation
 
-- Clone this repository: `git clone https://github.com/tjjlemaire/instrulink.git`
-- Move to that directory (`cd instrulink`) and install it as a python package: `pip install -e .`
+This package can be directly installed from PyPI:
+
+```pip install instrulink```
+
+However, if you wish to amend the package code, you can also clone this repo and install it locally as an editable package: 
+
+```
+git clone https://github.com/tjjlemaire/instrulink.git
+cd instrulink
+pip install -e .
+```
 
 ## Usage
 
-Instruments can be easily accessed via generic `grab_camera`, `grab_generator`, `grab_oscilloscope` and `grab_manipulator` functions. By default, these functions will automatically detect the first available instrument connected to the PC. Optionally, you can also provide an instrument `key` to connect to a specific model type (e.g. `grab_osciloscope(key='bk')` to specifically connect to a B&K Precision oscilloscope).
+### Connecting to instruments
+
+Instruments can be easily connected to via generic `grab_camera`, `grab_generator`, `grab_oscilloscope` and `grab_manipulator` functions. By default, these functions will automatically detect the first available instrument connected to the PC. Optionally, you can also provide an instrument `key` to connect to a specific model type (e.g. `grab_osciloscope(key='bk')` to specifically connect to a B&K Precision oscilloscope).
+
+### Using instruments
 
 Example scripts are located in the `/scripts` subfolder.
```

### Comparing `instrulink-1.0/instrulink/bk_2555.py` & `instrulink-1.0.1/instrulink/bk_2555.py`

 * *Files identical despite different names*

### Comparing `instrulink-1.0/instrulink/camera.py` & `instrulink-1.0.1/instrulink/camera.py`

 * *Files identical despite different names*

### Comparing `instrulink-1.0/instrulink/constants.py` & `instrulink-1.0.1/instrulink/constants.py`

 * *Files identical despite different names*

### Comparing `instrulink-1.0/instrulink/factory.py` & `instrulink-1.0.1/instrulink/factory.py`

 * *Files identical despite different names*

### Comparing `instrulink-1.0/instrulink/keysight_e5061b.py` & `instrulink-1.0.1/instrulink/keysight_e5061b.py`

 * *Files identical despite different names*

### Comparing `instrulink-1.0/instrulink/logger.py` & `instrulink-1.0.1/instrulink/logger.py`

 * *Files identical despite different names*

### Comparing `instrulink-1.0/instrulink/nidaq.py` & `instrulink-1.0.1/instrulink/nidaq.py`

 * *Files identical despite different names*

### Comparing `instrulink-1.0/instrulink/oscilloscope.py` & `instrulink-1.0.1/instrulink/oscilloscope.py`

 * *Files identical despite different names*

### Comparing `instrulink-1.0/instrulink/rigol_ds1054z.py` & `instrulink-1.0.1/instrulink/rigol_ds1054z.py`

 * *Files identical despite different names*

### Comparing `instrulink-1.0/instrulink/si_utils.py` & `instrulink-1.0.1/instrulink/si_utils.py`

 * *Files identical despite different names*

### Comparing `instrulink-1.0/instrulink/sutter_mp285a.py` & `instrulink-1.0.1/instrulink/sutter_mp285a.py`

 * *Files identical despite different names*

### Comparing `instrulink-1.0/instrulink/utils.py` & `instrulink-1.0.1/instrulink/utils.py`

 * *Files identical despite different names*

### Comparing `instrulink-1.0/instrulink/visa_instrument.py` & `instrulink-1.0.1/instrulink/visa_instrument.py`

 * *Files identical despite different names*

### Comparing `instrulink-1.0/instrulink/waveform_generator.py` & `instrulink-1.0.1/instrulink/waveform_generator.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 # @Author: Theo Lemaire
 # @Date:   2022-03-15 09:26:06
 # @Last Modified by:   Theo Lemaire
-# @Last Modified time: 2023-05-11 11:41:37
+# @Last Modified time: 2023-08-04 15:55:47
 
 import abc
 import numpy as np
 
 from .visa_instrument import *
 
 
@@ -20,15 +20,15 @@
     
     # --------------------- MISCELLANEOUS ---------------------
     
     def connect(self):
         super().connect()
         self.disable_output()
         self.beep()
-        self.display_for('instrument connected', duration=1.0)
+        # self.display_for('instrument connected', duration=1.0)
 
     def get_version(self):
         ''' Get system SCPI version. '''
         return float(self.query('SYST:VERS?'))
 
     def get_nchannels(self):
         ''' Get the number of channels available in the instrument '''
@@ -246,14 +246,29 @@
         raise NotImplementedError
 
     @abc.abstractmethod
     def get_waveform_offset(self, *args, **kwargs):
         ''' Get the waveform voltage offset (V). '''
         raise NotImplementedError
     
+    def check_phase(self, phi):
+        ''' Check the waveform phase '''
+        if phi < 0. or phi > 360:
+            raise VisaError(f'phase out of range : {phi} (must be within [0, 360]deg)')
+
+    @abc.abstractmethod
+    def set_waveform_phase(self, *args, **kwargs):
+        ''' Set the waveform phase of the specified channel (in degrees) '''
+        raise NotImplementedError
+    
+    @abc.abstractmethod
+    def get_waveform_phase(self, *args, **kwargs):
+        ''' Get the waveform phase of the specified channel (in degrees) '''
+        raise NotImplementedError
+    
     def check_duty_cycle(self, DC):
         ''' Check duty cycle '''
         if DC <= 0. or DC >= 100.:
             raise VisaError('Duty cycle out of range (must be within [0-100]%)')
     
     @abc.abstractmethod
     def set_square_duty_cycle(self, *args, **kwargs):
@@ -333,16 +348,17 @@
     @abc.abstractmethod
     def MAX_BURST_PERIOD(self):
         raise NotImplementedError
 
     def check_burst_duration(self, t, T):
         ''' Check the burst duration and return corresponding number of cycles '''
         if t < T:
-            raise VisaError(
-                f'burst duration ({t:.2e} s) shorter than stimulus period ({T:.2e} s)')
+            if not np.isclose(T - t, 0):
+                raise VisaError(
+                    f'burst duration ({si_format(t, 2)}s) shorter than stimulus periodicity ({si_format(T, 2)}s)')
         if t > self.MAX_BURST_PERIOD:
             raise VisaError(
                 f'burst duration ({t:.2e} s) above max value ({self.MAX_BURST_PERIOD:.2e} s)')
         return int(np.round(t / T))
 
     @abc.abstractmethod
     def set_burst_duration(self, *args, **kwargs):
@@ -375,14 +391,29 @@
         raise NotImplementedError
 
     @abc.abstractmethod
     def get_burst_gated_polarity(self, *args, **kwargs):
         ''' Get the gate polarity of the gated burst of the specified channel '''
         raise NotImplementedError
     
+
+    # --------------------- MODULATION ---------------------
+
+    def check_modulation_mode(self, mode):
+        ''' Check that modulation mode is available on the instrument '''
+        if mode not in self.MOD_MODES:
+            raise VisaError(
+                f'{mode} is not a valid modulation mode (options are {self.MOD_MODES})')
+    
+    def check_modulation_source(self, source):
+        ''' Check that modulation source is available on the instrument '''
+        if source not in self.MOD_SOURCES:
+            raise VisaError(
+                f'{source} is not a valid modulation source (options are {self.MOD_SOURCES})')
+    
     # --------------------- TRIGGER ---------------------
 
     @property
     @abc.abstractmethod
     def TRIGGER_SOURCES(self):
         raise NotImplementedError
```

### Comparing `instrulink-1.0/instrulink.egg-info/SOURCES.txt` & `instrulink-1.0.1/instrulink.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 requirements.txt
 setup.py
 instrulink/__init__.py
 instrulink/bk_2555.py
 instrulink/camera.py
 instrulink/constants.py
 instrulink/factory.py
+instrulink/keysight_33500b.py
 instrulink/keysight_e5061b.py
 instrulink/logger.py
 instrulink/nidaq.py
 instrulink/oscilloscope.py
 instrulink/rigol_dg1022z.py
 instrulink/rigol_ds1054z.py
 instrulink/si_utils.py
@@ -23,13 +24,15 @@
 instrulink.egg-info/PKG-INFO
 instrulink.egg-info/SOURCES.txt
 instrulink.egg-info/dependency_links.txt
 instrulink.egg-info/not-zip-safe
 instrulink.egg-info/requires.txt
 instrulink.egg-info/top_level.txt
 scripts/list_visa_resources.py
+scripts/test_33500b.py
 scripts/test_camera.py
 scripts/test_e5061b.py
 scripts/test_generator.py
 scripts/test_manipulator.py
 scripts/test_nidaq.py
-scripts/test_scope.py
+scripts/test_scope.py
+scripts/test_smoothed_waveform.py
```

### Comparing `instrulink-1.0/scripts/test_camera.py` & `instrulink-1.0.1/scripts/test_camera.py`

 * *Files identical despite different names*

### Comparing `instrulink-1.0/scripts/test_e5061b.py` & `instrulink-1.0.1/scripts/test_e5061b.py`

 * *Files identical despite different names*

### Comparing `instrulink-1.0/scripts/test_manipulator.py` & `instrulink-1.0.1/scripts/test_manipulator.py`

 * *Files identical despite different names*

### Comparing `instrulink-1.0/scripts/test_nidaq.py` & `instrulink-1.0.1/scripts/test_nidaq.py`

 * *Files identical despite different names*

### Comparing `instrulink-1.0/scripts/test_scope.py` & `instrulink-1.0.1/scripts/test_scope.py`

 * *Files identical despite different names*

### Comparing `instrulink-1.0/setup.py` & `instrulink-1.0.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 # @Author: Theo Lemaire
 # @Email: theo.lemaire@epfl.ch
 # @Date:   2017-06-13 09:40:02
 # @Last Modified by:   Theo Lemaire
-# @Last Modified time: 2023-05-17 11:48:50
+# @Last Modified time: 2023-08-04 16:54:26
 
 import os
 from setuptools import setup
 
 readme_file = 'README.md'
 req_file = 'requirements.txt'
 
@@ -21,15 +21,15 @@
         return f.readlines()
 
 def getFiles(path):
     return [f'{path}/{x}' for x in os.listdir(path)]
 
 setup(
     name='instrulink',
-    version='1.0',
+    version='1.0.1',
     description='Python package to interface diverse laboratory instruments',
     long_description_content_type='text/markdown',
     long_description=readme(),
     url='https://github.com/tjjlemaire/instrulink',
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Science/Research',
```

