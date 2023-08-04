# Comparing `tmp/scatfit-0.2.19.tar.gz` & `tmp/scatfit-0.2.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scatfit-0.2.19.tar", last modified: Wed Aug  2 15:11:43 2023, max compression
+gzip compressed data, was "scatfit-0.2.20.tar", last modified: Fri Aug  4 13:08:14 2023, max compression
```

## Comparing `scatfit-0.2.19.tar` & `scatfit-0.2.20.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 jankowsk   (501) staff       (20)        0 2023-08-02 15:11:43.777245 scatfit-0.2.19/
--rw-r--r--   0 jankowsk   (501) staff       (20)     1073 2022-11-11 18:11:38.000000 scatfit-0.2.19/LICENSE
--rw-r--r--   0 jankowsk   (501) staff       (20)     6440 2023-08-02 15:11:43.776430 scatfit-0.2.19/PKG-INFO
--rw-r--r--   0 jankowsk   (501) staff       (20)     5845 2023-08-02 14:51:44.000000 scatfit-0.2.19/README.md
--rw-r--r--   0 jankowsk   (501) staff       (20)      100 2023-08-02 14:51:44.000000 scatfit-0.2.19/pyproject.toml
-drwxr-xr-x   0 jankowsk   (501) staff       (20)        0 2023-08-02 15:11:43.765303 scatfit-0.2.19/scatfit/
--rw-r--r--   0 jankowsk   (501) staff       (20)       40 2022-11-17 17:45:33.000000 scatfit-0.2.19/scatfit/__init__.py
-drwxr-xr-x   0 jankowsk   (501) staff       (20)        0 2023-08-02 15:11:43.772973 scatfit-0.2.19/scatfit/apps/
--rw-r--r--   0 jankowsk   (501) staff       (20)        0 2022-11-11 18:11:39.000000 scatfit-0.2.19/scatfit/apps/__init__.py
--rw-r--r--   0 jankowsk   (501) staff       (20)    19079 2022-12-06 10:19:22.000000 scatfit-0.2.19/scatfit/apps/fit_frb.py
--rw-r--r--   0 jankowsk   (501) staff       (20)     7429 2022-11-11 18:11:39.000000 scatfit-0.2.19/scatfit/apps/simulate_pulse.py
--rw-r--r--   0 jankowsk   (501) staff       (20)      810 2022-11-17 17:45:33.000000 scatfit-0.2.19/scatfit/dm.py
--rw-r--r--   0 jankowsk   (501) staff       (20)    12644 2023-01-30 12:02:21.000000 scatfit-0.2.19/scatfit/plotting.py
--rw-r--r--   0 jankowsk   (501) staff       (20)     7183 2022-12-06 10:19:22.000000 scatfit-0.2.19/scatfit/pulsemodels.py
--rw-r--r--   0 jankowsk   (501) staff       (20)     6440 2022-12-06 10:19:22.000000 scatfit-0.2.19/scatfit/pulsemodels_cython.pyx
--rw-r--r--   0 jankowsk   (501) staff       (20)     4757 2022-12-06 10:19:22.000000 scatfit-0.2.19/scatfit/pulsemodels_python.py
--rw-r--r--   0 jankowsk   (501) staff       (20)     1387 2022-11-17 17:45:54.000000 scatfit-0.2.19/scatfit/sigproc.py
--rw-r--r--   0 jankowsk   (501) staff       (20)       23 2023-08-02 14:51:44.000000 scatfit-0.2.19/scatfit/version.py
-drwxr-xr-x   0 jankowsk   (501) staff       (20)        0 2023-08-02 15:11:43.770730 scatfit-0.2.19/scatfit.egg-info/
--rw-r--r--   0 jankowsk   (501) staff       (20)     6440 2023-08-02 15:11:43.000000 scatfit-0.2.19/scatfit.egg-info/PKG-INFO
--rw-r--r--   0 jankowsk   (501) staff       (20)      607 2023-08-02 15:11:43.000000 scatfit-0.2.19/scatfit.egg-info/SOURCES.txt
--rw-r--r--   0 jankowsk   (501) staff       (20)      105 2023-08-02 15:11:43.000000 scatfit-0.2.19/scatfit.egg-info/dependency_links.txt
--rw-r--r--   0 jankowsk   (501) staff       (20)      113 2023-08-02 15:11:43.000000 scatfit-0.2.19/scatfit.egg-info/entry_points.txt
--rw-r--r--   0 jankowsk   (501) staff       (20)        1 2023-08-02 15:11:43.000000 scatfit-0.2.19/scatfit.egg-info/not-zip-safe
--rw-r--r--   0 jankowsk   (501) staff       (20)      106 2023-08-02 15:11:43.000000 scatfit-0.2.19/scatfit.egg-info/requires.txt
--rw-r--r--   0 jankowsk   (501) staff       (20)        8 2023-08-02 15:11:43.000000 scatfit-0.2.19/scatfit.egg-info/top_level.txt
--rw-r--r--   0 jankowsk   (501) staff       (20)       38 2023-08-02 15:11:43.777451 scatfit-0.2.19/setup.cfg
--rw-r--r--   0 jankowsk   (501) staff       (20)     2087 2023-08-02 14:51:44.000000 scatfit-0.2.19/setup.py
-drwxr-xr-x   0 jankowsk   (501) staff       (20)        0 2023-08-02 15:11:43.775565 scatfit-0.2.19/tests/
--rw-r--r--   0 jankowsk   (501) staff       (20)     3032 2022-12-06 10:19:22.000000 scatfit-0.2.19/tests/test_pulsemodels.py
--rw-r--r--   0 jankowsk   (501) staff       (20)     3648 2022-12-06 10:19:22.000000 scatfit-0.2.19/tests/test_pulsemodels_cython.py
--rw-r--r--   0 jankowsk   (501) staff       (20)     1943 2022-12-06 10:19:22.000000 scatfit-0.2.19/tests/test_pulsemodels_visual.py
+drwxr-xr-x   0 jankowsk   (501) staff       (20)        0 2023-08-04 13:08:14.660834 scatfit-0.2.20/
+-rw-r--r--   0 jankowsk   (501) staff       (20)     1073 2022-11-11 18:11:38.000000 scatfit-0.2.20/LICENSE
+-rw-r--r--   0 jankowsk   (501) staff       (20)     7743 2023-08-04 13:08:14.659917 scatfit-0.2.20/PKG-INFO
+-rw-r--r--   0 jankowsk   (501) staff       (20)     7148 2023-08-04 12:59:15.000000 scatfit-0.2.20/README.md
+-rw-r--r--   0 jankowsk   (501) staff       (20)      100 2023-08-02 14:51:44.000000 scatfit-0.2.20/pyproject.toml
+drwxr-xr-x   0 jankowsk   (501) staff       (20)        0 2023-08-04 13:08:14.645373 scatfit-0.2.20/scatfit/
+-rw-r--r--   0 jankowsk   (501) staff       (20)       40 2023-08-02 22:06:53.000000 scatfit-0.2.20/scatfit/__init__.py
+drwxr-xr-x   0 jankowsk   (501) staff       (20)        0 2023-08-04 13:08:14.655270 scatfit-0.2.20/scatfit/apps/
+-rw-r--r--   0 jankowsk   (501) staff       (20)        0 2023-08-02 22:06:53.000000 scatfit-0.2.20/scatfit/apps/__init__.py
+-rw-r--r--   0 jankowsk   (501) staff       (20)    20193 2023-08-04 12:59:15.000000 scatfit-0.2.20/scatfit/apps/fit_frb.py
+-rw-r--r--   0 jankowsk   (501) staff       (20)    11251 2023-08-04 12:59:15.000000 scatfit-0.2.20/scatfit/apps/simulate_pulse.py
+-rw-r--r--   0 jankowsk   (501) staff       (20)      810 2023-08-02 22:06:53.000000 scatfit-0.2.20/scatfit/dm.py
+-rw-r--r--   0 jankowsk   (501) staff       (20)    12944 2023-08-04 12:59:15.000000 scatfit-0.2.20/scatfit/plotting.py
+-rw-r--r--   0 jankowsk   (501) staff       (20)     7183 2023-08-02 22:06:53.000000 scatfit-0.2.20/scatfit/pulsemodels.py
+-rw-r--r--   0 jankowsk   (501) staff       (20)     6440 2023-08-02 22:06:53.000000 scatfit-0.2.20/scatfit/pulsemodels_cython.pyx
+-rw-r--r--   0 jankowsk   (501) staff       (20)     4757 2023-08-02 22:06:53.000000 scatfit-0.2.20/scatfit/pulsemodels_python.py
+-rw-r--r--   0 jankowsk   (501) staff       (20)     1387 2023-08-02 22:06:53.000000 scatfit-0.2.20/scatfit/sigproc.py
+-rw-r--r--   0 jankowsk   (501) staff       (20)       23 2023-08-03 14:00:44.000000 scatfit-0.2.20/scatfit/version.py
+drwxr-xr-x   0 jankowsk   (501) staff       (20)        0 2023-08-04 13:08:14.652606 scatfit-0.2.20/scatfit.egg-info/
+-rw-r--r--   0 jankowsk   (501) staff       (20)     7743 2023-08-04 13:08:14.000000 scatfit-0.2.20/scatfit.egg-info/PKG-INFO
+-rw-r--r--   0 jankowsk   (501) staff       (20)      607 2023-08-04 13:08:14.000000 scatfit-0.2.20/scatfit.egg-info/SOURCES.txt
+-rw-r--r--   0 jankowsk   (501) staff       (20)      105 2023-08-04 13:08:14.000000 scatfit-0.2.20/scatfit.egg-info/dependency_links.txt
+-rw-r--r--   0 jankowsk   (501) staff       (20)      113 2023-08-04 13:08:14.000000 scatfit-0.2.20/scatfit.egg-info/entry_points.txt
+-rw-r--r--   0 jankowsk   (501) staff       (20)        1 2023-08-04 13:08:14.000000 scatfit-0.2.20/scatfit.egg-info/not-zip-safe
+-rw-r--r--   0 jankowsk   (501) staff       (20)      124 2023-08-04 13:08:14.000000 scatfit-0.2.20/scatfit.egg-info/requires.txt
+-rw-r--r--   0 jankowsk   (501) staff       (20)        8 2023-08-04 13:08:14.000000 scatfit-0.2.20/scatfit.egg-info/top_level.txt
+-rw-r--r--   0 jankowsk   (501) staff       (20)       38 2023-08-04 13:08:14.661096 scatfit-0.2.20/setup.cfg
+-rw-r--r--   0 jankowsk   (501) staff       (20)     1991 2023-08-03 18:11:51.000000 scatfit-0.2.20/setup.py
+drwxr-xr-x   0 jankowsk   (501) staff       (20)        0 2023-08-04 13:08:14.657853 scatfit-0.2.20/tests/
+-rw-r--r--   0 jankowsk   (501) staff       (20)     3044 2023-08-03 14:00:44.000000 scatfit-0.2.20/tests/test_pulsemodels.py
+-rw-r--r--   0 jankowsk   (501) staff       (20)     3660 2023-08-03 14:00:44.000000 scatfit-0.2.20/tests/test_pulsemodels_cython.py
+-rw-r--r--   0 jankowsk   (501) staff       (20)     1982 2023-08-03 14:00:44.000000 scatfit-0.2.20/tests/test_pulsemodels_visual.py
```

### Comparing `scatfit-0.2.19/LICENSE` & `scatfit-0.2.20/LICENSE`

 * *Files identical despite different names*

### Comparing `scatfit-0.2.19/PKG-INFO` & `scatfit-0.2.20/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,15 @@
-Metadata-Version: 2.1
-Name: scatfit
-Version: 0.2.19
-Summary: Scattering fits of time domain radio signals (Fast Radio Bursts or pulsars).
-Home-page: https://github.com/fjankowsk/scatfit
-Author: Fabian Jankowski
-Author-email: fjankowsk@gmail.com
-License: MIT
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-Provides-Extra: develop
-License-File: LICENSE
-
 # Scatfit: Scattering fits of time domain radio signals (Fast Radio Bursts or pulsars) #
 
+[![PyPI latest release](https://img.shields.io/pypi/v/scatfit.svg)](https://pypi.org/project/scatfit/)
+[![GitHub issues](https://img.shields.io/badge/issue_tracking-GitHub-blue.svg)](https://github.com/fjankowsk/scatfit/issues/)
+[![License - MIT](https://img.shields.io/pypi/l/scatfit.svg)](https://github.com/fjankowsk/scatfit/blob/master/LICENSE)
+[![Paper link](https://img.shields.io/badge/paper-10.1093/mnras/stad2041-blue.svg)](https://doi.org/10.1093/mnras/stad2041)
+[![arXiv link](https://img.shields.io/badge/arXiv-2302.10107-blue.svg)](https://arxiv.org/abs/2302.10107)
+
 This repository contains code to fit Fast Radio Burst or pulsar profiles to measure scattering and other parameters. The code is mainly developed for Python 3, but Python 2 from version 2.7 onwards should work fine.
 
 ## Author ##
 
 The software is primarily developed and maintained by Fabian Jankowski. For more information feel free to contact me via: fabian.jankowski at cnrs-orleans.fr.
 
 ## Paper ##
@@ -33,37 +22,38 @@
 
 The code is also listed in the Astrophysics Source Code Library (ASCL): https://ascl.net/code/v/3366
 
 ## Installation ##
 
 The easiest and recommended way to install the software is through `pip` from the central PyPI index by running:
 
-`pip3 install scatfit`
+`pip install scatfit`
 
 This will install the latest release and all its dependencies. If you need a more recent version of the software, install it directly from its GitHub software repository. For instance, to install the master branch of the code, use the following command:
 
-`pip3 install git+https://github.com/fjankowsk/scatfit.git@master`
+`pip install git+https://github.com/fjankowsk/scatfit.git@master`
 
 This will also automatically install all dependencies.
 
 Please verify that your installation works as expected by downloading a pre-generated `SIGPROC` filterbank file with synthetic data that comes bundled with the GitHub repository:
 
 `wget https://github.com/fjankowsk/scatfit/raw/master/extra/fake_burst_500_DM.fil`
 
 Then run the main analysis on the filterbank data file like this:
 
-`scatfit-fitfrb fake_burst_500_DM.fil 500.0 --fitscatindex --fast`
+`scatfit-fitfrb fake_burst_500_DM.fil 500.0 --fitscatindex --fscrunch 128 --fast`
 
 You should see several diagnostic windows open. The terminal output should show an updated DM close to 500 pc cm^-3, a scattering index near -4.0, and a scattering time at 1 GHz of about 20 ms.
 
 ## Usage ##
 
 ```
 $ scatfit-fitfrb -h
-usage: scatfit-fitfrb [-h] [--compare] [--binburst bin] [--fscrunch factor] [--tscrunch factor] [--fast] [--fitscatindex]
+usage: scatfit-fitfrb [-h] [--compare] [--binburst bin] [--fscrunch factor] [--tscrunch factor] [--fast] [--fitrange start end]
+                      [--fitscatindex]
                       [--smodel {unscattered,scattered_isotropic_analytic,scattered_isotropic_convolving,scattered_isotropic_bandintegrated,scattered_isotropic_afb_instrumental,scattered_isotropic_dfb_instrumental}]
                       [--showmodels] [--snr snr] [--publish] [-z start end]
                       filename dm
 
 Fit a scattering model to FRB data.
 
 positional arguments:
@@ -73,24 +63,36 @@
 options:
   -h, --help            show this help message and exit
   --compare             Fit an unscattered Gaussian model for comparison. (default: False)
   --binburst bin        Specify the burst location bin manually. (default: None)
   --fscrunch factor     Integrate this many frequency channels. (default: 256)
   --tscrunch factor     Integrate this many time samples. (default: 1)
   --fast                Enable fast processing. This reduces the number of MCMC steps drastically. (default: False)
+  --fitrange start end  Consider only this time range of data in the fit. Increase the region for wide or highly-scattered bursts.
+                        Ensure that most of the scattering tail is included in the fit. (default: [-200.0, 200.0])
   --fitscatindex        Fit the scattering times and determine the scattering index. (default: False)
   --smodel {unscattered,scattered_isotropic_analytic,scattered_isotropic_convolving,scattered_isotropic_bandintegrated,scattered_isotropic_afb_instrumental,scattered_isotropic_dfb_instrumental}
                         Use the specified scattering model. (default: scattered_isotropic_analytic)
   --showmodels          Show comparison plot of scattering models. (default: False)
   --snr snr             Only consider sub-bands above this S/N threshold. (default: 3.8)
   --publish             Output plots suitable for publication. (default: False)
   -z start end, --zoom start end
                         Zoom into this time region. (default: [-50.0, 50.0])
 ```
 
+```
+$ scatfit-simpulse -h
+usage: scatfit-simpulse [-h]
+
+Simulate scattered pulses.
+
+options:
+  -h, --help  show this help message and exit
+```
+
 ## Profile scattering models ##
 
 Several profile scattering models, i.e. pulse broadening functions and instrumental contributions, are implemented and others can easily be added. The image below shows a selection of them.
 
 ![Implemented profile scattering models](https://github.com/fjankowsk/scatfit/raw/master/docs/profile_models.png "Implemented profile scattering models")
 
 ## Example output ##
@@ -112,7 +114,11 @@
 ### Why do I get the following warning: `Could not import Cython pulse model implementations. Falling back to the Python versions.`? ###
 
 This could happen if you run `scatfit` from its software repository git checkout, where the current working directory takes import preference. Install the software as above and run it as `$ scatfit-fitfrb` in a different path.
 
 ### What data formats are supported? ###
 
 `scatfit` supports loading data from `SIGPROC` filterbank files. Alternative loaders can be implemented relatively easily.
+
+### Does it work on ARM-based Macs? ###
+
+Yes, `scatfit` works on ARM-based Macs with M1 or M2 processors. In fact, it runs blazing fast on them! The immense single-core performance results in a speedup of > 3x in comparison with similar x64-based systems, in my experience.
```

### Comparing `scatfit-0.2.19/README.md` & `scatfit-0.2.20/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,32 @@
+Metadata-Version: 2.1
+Name: scatfit
+Version: 0.2.20
+Summary: Scattering fits of time domain radio signals (Fast Radio Bursts or pulsars).
+Home-page: https://github.com/fjankowsk/scatfit
+Author: Fabian Jankowski
+Author-email: fjankowsk@gmail.com
+License: MIT
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 2
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+Provides-Extra: develop
+License-File: LICENSE
+
 # Scatfit: Scattering fits of time domain radio signals (Fast Radio Bursts or pulsars) #
 
+[![PyPI latest release](https://img.shields.io/pypi/v/scatfit.svg)](https://pypi.org/project/scatfit/)
+[![GitHub issues](https://img.shields.io/badge/issue_tracking-GitHub-blue.svg)](https://github.com/fjankowsk/scatfit/issues/)
+[![License - MIT](https://img.shields.io/pypi/l/scatfit.svg)](https://github.com/fjankowsk/scatfit/blob/master/LICENSE)
+[![Paper link](https://img.shields.io/badge/paper-10.1093/mnras/stad2041-blue.svg)](https://doi.org/10.1093/mnras/stad2041)
+[![arXiv link](https://img.shields.io/badge/arXiv-2302.10107-blue.svg)](https://arxiv.org/abs/2302.10107)
+
 This repository contains code to fit Fast Radio Burst or pulsar profiles to measure scattering and other parameters. The code is mainly developed for Python 3, but Python 2 from version 2.7 onwards should work fine.
 
 ## Author ##
 
 The software is primarily developed and maintained by Fabian Jankowski. For more information feel free to contact me via: fabian.jankowski at cnrs-orleans.fr.
 
 ## Paper ##
@@ -16,37 +39,38 @@
 
 The code is also listed in the Astrophysics Source Code Library (ASCL): https://ascl.net/code/v/3366
 
 ## Installation ##
 
 The easiest and recommended way to install the software is through `pip` from the central PyPI index by running:
 
-`pip3 install scatfit`
+`pip install scatfit`
 
 This will install the latest release and all its dependencies. If you need a more recent version of the software, install it directly from its GitHub software repository. For instance, to install the master branch of the code, use the following command:
 
-`pip3 install git+https://github.com/fjankowsk/scatfit.git@master`
+`pip install git+https://github.com/fjankowsk/scatfit.git@master`
 
 This will also automatically install all dependencies.
 
 Please verify that your installation works as expected by downloading a pre-generated `SIGPROC` filterbank file with synthetic data that comes bundled with the GitHub repository:
 
 `wget https://github.com/fjankowsk/scatfit/raw/master/extra/fake_burst_500_DM.fil`
 
 Then run the main analysis on the filterbank data file like this:
 
-`scatfit-fitfrb fake_burst_500_DM.fil 500.0 --fitscatindex --fast`
+`scatfit-fitfrb fake_burst_500_DM.fil 500.0 --fitscatindex --fscrunch 128 --fast`
 
 You should see several diagnostic windows open. The terminal output should show an updated DM close to 500 pc cm^-3, a scattering index near -4.0, and a scattering time at 1 GHz of about 20 ms.
 
 ## Usage ##
 
 ```
 $ scatfit-fitfrb -h
-usage: scatfit-fitfrb [-h] [--compare] [--binburst bin] [--fscrunch factor] [--tscrunch factor] [--fast] [--fitscatindex]
+usage: scatfit-fitfrb [-h] [--compare] [--binburst bin] [--fscrunch factor] [--tscrunch factor] [--fast] [--fitrange start end]
+                      [--fitscatindex]
                       [--smodel {unscattered,scattered_isotropic_analytic,scattered_isotropic_convolving,scattered_isotropic_bandintegrated,scattered_isotropic_afb_instrumental,scattered_isotropic_dfb_instrumental}]
                       [--showmodels] [--snr snr] [--publish] [-z start end]
                       filename dm
 
 Fit a scattering model to FRB data.
 
 positional arguments:
@@ -56,24 +80,36 @@
 options:
   -h, --help            show this help message and exit
   --compare             Fit an unscattered Gaussian model for comparison. (default: False)
   --binburst bin        Specify the burst location bin manually. (default: None)
   --fscrunch factor     Integrate this many frequency channels. (default: 256)
   --tscrunch factor     Integrate this many time samples. (default: 1)
   --fast                Enable fast processing. This reduces the number of MCMC steps drastically. (default: False)
+  --fitrange start end  Consider only this time range of data in the fit. Increase the region for wide or highly-scattered bursts.
+                        Ensure that most of the scattering tail is included in the fit. (default: [-200.0, 200.0])
   --fitscatindex        Fit the scattering times and determine the scattering index. (default: False)
   --smodel {unscattered,scattered_isotropic_analytic,scattered_isotropic_convolving,scattered_isotropic_bandintegrated,scattered_isotropic_afb_instrumental,scattered_isotropic_dfb_instrumental}
                         Use the specified scattering model. (default: scattered_isotropic_analytic)
   --showmodels          Show comparison plot of scattering models. (default: False)
   --snr snr             Only consider sub-bands above this S/N threshold. (default: 3.8)
   --publish             Output plots suitable for publication. (default: False)
   -z start end, --zoom start end
                         Zoom into this time region. (default: [-50.0, 50.0])
 ```
 
+```
+$ scatfit-simpulse -h
+usage: scatfit-simpulse [-h]
+
+Simulate scattered pulses.
+
+options:
+  -h, --help  show this help message and exit
+```
+
 ## Profile scattering models ##
 
 Several profile scattering models, i.e. pulse broadening functions and instrumental contributions, are implemented and others can easily be added. The image below shows a selection of them.
 
 ![Implemented profile scattering models](https://github.com/fjankowsk/scatfit/raw/master/docs/profile_models.png "Implemented profile scattering models")
 
 ## Example output ##
@@ -95,7 +131,11 @@
 ### Why do I get the following warning: `Could not import Cython pulse model implementations. Falling back to the Python versions.`? ###
 
 This could happen if you run `scatfit` from its software repository git checkout, where the current working directory takes import preference. Install the software as above and run it as `$ scatfit-fitfrb` in a different path.
 
 ### What data formats are supported? ###
 
 `scatfit` supports loading data from `SIGPROC` filterbank files. Alternative loaders can be implemented relatively easily.
+
+### Does it work on ARM-based Macs? ###
+
+Yes, `scatfit` works on ARM-based Macs with M1 or M2 processors. In fact, it runs blazing fast on them! The immense single-core performance results in a speedup of > 3x in comparison with similar x64-based systems, in my experience.
```

### Comparing `scatfit-0.2.19/scatfit/apps/fit_frb.py` & `scatfit-0.2.20/scatfit/apps/fit_frb.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #
 #   Fit scattering models to FRB data.
-#   2022 Fabian Jankowski
+#   2022 - 2023 Fabian Jankowski
 #
 
 import argparse
 import copy
 import inspect
 import os.path
 import sys
@@ -86,14 +86,24 @@
         dest="fast",
         action="store_true",
         default=False,
         help="Enable fast processing. This reduces the number of MCMC steps drastically.",
     )
 
     parser.add_argument(
+        "--fitrange",
+        dest="fitrange",
+        type=float,
+        nargs=2,
+        metavar=("start", "end"),
+        default=[-200.0, 200.0],
+        help="Consider only this time range of data in the fit. Increase the region for wide or highly-scattered bursts. Ensure that most of the scattering tail is included in the fit.",
+    )
+
+    parser.add_argument(
         "--fitscatindex",
         action="store_true",
         dest="fit_scatindex",
         default=False,
         help="Fit the scattering times and determine the scattering index.",
     )
 
@@ -149,14 +159,41 @@
     )
 
     args = parser.parse_args()
 
     return args
 
 
+def check_args(args):
+    """
+    Sanity check the commandline arguments.
+
+    Parameters
+    ----------
+    args: populated namespace
+        The commandline arguments.
+    """
+
+    # fitrange
+    if args.fitrange[0] < args.fitrange[1]:
+        pass
+    else:
+        print(
+            "Fit range is invalid: {0}, {1}".format(args.fitrange[0], args.fitrange[1])
+        )
+        sys.exit(1)
+
+    # zoom
+    if args.zoom[0] < args.zoom[1]:
+        pass
+    else:
+        print("Zoom range is invalid: {0}, {1}".format(args.zoom[0], args.zoom[1]))
+        sys.exit(1)
+
+
 def linear(x, x0, slope, intercept):
     """
     A linear function.
 
     Parameters
     ----------
     x: ~np.array
@@ -498,16 +535,18 @@
     )
 
     for iband in range(cand.dynspec.shape[0]):
         print("Running sub-band: {0}".format(iband))
 
         sub_profile = cand.dynspec[iband, :]
 
-        # select only the central +- 200 ms around the frb for the fit
-        mask = np.abs(plot_range) <= 200.0
+        # select only this time range of data for the fit
+        mask = (plot_range >= params["fitrange"][0]) & (
+            plot_range <= params["fitrange"][1]
+        )
         fit_range = np.copy(plot_range[mask])
         sub_profile = sub_profile[mask]
 
         # remove baseline and normalise
         sub_profile = sub_profile - np.mean(sub_profile)
         sub_profile = sub_profile / np.max(sub_profile)
 
@@ -606,14 +645,17 @@
 # MAIN
 #
 
 
 def main():
     args = parse_args()
 
+    # sanity check command line arguments
+    check_args(args)
+
     plotting.use_custom_matplotlib_formatting()
 
     if args.show_models:
         plotting.plot_profile_models()
         plt.show()
         sys.exit(0)
 
@@ -639,14 +681,15 @@
     else:
         bin_burst = np.argmax(profile)
     plot_range -= fact * bin_burst
 
     params = {
         "compare": args.compare,
         "fast": args.fast,
+        "fitrange": args.fitrange,
         "publish": args.publish,
         "snr": args.snr,
         "zoom": args.zoom,
     }
 
     # fit integrated profile
     fit_df = fit_profile(cand, plot_range, args.fscrunch_factor, args.smodel, params)
@@ -680,15 +723,15 @@
             params,
         )
     else:
         fitresult = None
 
     plotting.plot_width_scaling(fit_df, cand, fitresult)
 
-    plotting.plot_frb(cand, plot_range, profile)
+    plotting.plot_frb(cand, plot_range, profile, params)
 
     plt.show()
 
     print("All done.")
 
 
 if __name__ == "__main__":
```

### Comparing `scatfit-0.2.19/scatfit/dm.py` & `scatfit-0.2.20/scatfit/dm.py`

 * *Files identical despite different names*

### Comparing `scatfit-0.2.19/scatfit/plotting.py` & `scatfit-0.2.20/scatfit/plotting.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     matplotlib.rcParams["xtick.minor.width"] = 1.5
     matplotlib.rcParams["ytick.major.size"] = 6
     matplotlib.rcParams["ytick.major.width"] = 1.5
     matplotlib.rcParams["ytick.minor.size"] = 4
     matplotlib.rcParams["ytick.minor.width"] = 1.5
 
 
-def plot_frb(cand, plot_range, profile):
+def plot_frb(cand, plot_range, profile, params):
     """
     Plot the FRB data.
     """
 
     fig, (ax1, ax2) = plt.subplots(
         nrows=2,
         ncols=1,
@@ -51,14 +51,18 @@
         where="mid",
         color="black",
         ls="solid",
         lw=1.0,
         zorder=3,
     )
 
+    # highlight the data included in the fit
+    for item in params["fitrange"]:
+        ax1.axvline(x=item, color="tab:red", zorder=4)
+
     ax1.set_ylabel("Flux\n(a.u.)")
     ax1.tick_params(bottom=False)
 
     # plot dedispersed waterfall
     freqs = cand.freqs
     chan_bw = np.diff(freqs)[0]
 
@@ -76,16 +80,21 @@
             plot_range[-1],
             freqs[-1] - 0.5 * chan_bw,
             freqs[0] + 0.5 * chan_bw,
         ],
         cmap="Greys",
         vmin=quantiles[0],
         vmax=quantiles[-4],
+        zorder=3,
     )
 
+    # highlight the data included in the fit
+    for item in params["fitrange"]:
+        ax2.axvline(x=item, color="tab:red", zorder=4)
+
     ax2.set_ylabel("Frequency\n(MHz)")
     ax2.tick_params(bottom=False)
 
     # align ylabels horizontally
     fig.align_labels()
 
     fig.tight_layout()
```

### Comparing `scatfit-0.2.19/scatfit/pulsemodels.py` & `scatfit-0.2.20/scatfit/pulsemodels.py`

 * *Files identical despite different names*

### Comparing `scatfit-0.2.19/scatfit/pulsemodels_cython.pyx` & `scatfit-0.2.20/scatfit/pulsemodels_cython.pyx`

 * *Files identical despite different names*

### Comparing `scatfit-0.2.19/scatfit/pulsemodels_python.py` & `scatfit-0.2.20/scatfit/pulsemodels_python.py`

 * *Files identical despite different names*

### Comparing `scatfit-0.2.19/scatfit/sigproc.py` & `scatfit-0.2.20/scatfit/sigproc.py`

 * *Files identical despite different names*

### Comparing `scatfit-0.2.19/scatfit.egg-info/PKG-INFO` & `scatfit-0.2.20/scatfit.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scatfit
-Version: 0.2.19
+Version: 0.2.20
 Summary: Scattering fits of time domain radio signals (Fast Radio Bursts or pulsars).
 Home-page: https://github.com/fjankowsk/scatfit
 Author: Fabian Jankowski
 Author-email: fjankowsk@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
@@ -13,14 +13,20 @@
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Provides-Extra: develop
 License-File: LICENSE
 
 # Scatfit: Scattering fits of time domain radio signals (Fast Radio Bursts or pulsars) #
 
+[![PyPI latest release](https://img.shields.io/pypi/v/scatfit.svg)](https://pypi.org/project/scatfit/)
+[![GitHub issues](https://img.shields.io/badge/issue_tracking-GitHub-blue.svg)](https://github.com/fjankowsk/scatfit/issues/)
+[![License - MIT](https://img.shields.io/pypi/l/scatfit.svg)](https://github.com/fjankowsk/scatfit/blob/master/LICENSE)
+[![Paper link](https://img.shields.io/badge/paper-10.1093/mnras/stad2041-blue.svg)](https://doi.org/10.1093/mnras/stad2041)
+[![arXiv link](https://img.shields.io/badge/arXiv-2302.10107-blue.svg)](https://arxiv.org/abs/2302.10107)
+
 This repository contains code to fit Fast Radio Burst or pulsar profiles to measure scattering and other parameters. The code is mainly developed for Python 3, but Python 2 from version 2.7 onwards should work fine.
 
 ## Author ##
 
 The software is primarily developed and maintained by Fabian Jankowski. For more information feel free to contact me via: fabian.jankowski at cnrs-orleans.fr.
 
 ## Paper ##
@@ -33,37 +39,38 @@
 
 The code is also listed in the Astrophysics Source Code Library (ASCL): https://ascl.net/code/v/3366
 
 ## Installation ##
 
 The easiest and recommended way to install the software is through `pip` from the central PyPI index by running:
 
-`pip3 install scatfit`
+`pip install scatfit`
 
 This will install the latest release and all its dependencies. If you need a more recent version of the software, install it directly from its GitHub software repository. For instance, to install the master branch of the code, use the following command:
 
-`pip3 install git+https://github.com/fjankowsk/scatfit.git@master`
+`pip install git+https://github.com/fjankowsk/scatfit.git@master`
 
 This will also automatically install all dependencies.
 
 Please verify that your installation works as expected by downloading a pre-generated `SIGPROC` filterbank file with synthetic data that comes bundled with the GitHub repository:
 
 `wget https://github.com/fjankowsk/scatfit/raw/master/extra/fake_burst_500_DM.fil`
 
 Then run the main analysis on the filterbank data file like this:
 
-`scatfit-fitfrb fake_burst_500_DM.fil 500.0 --fitscatindex --fast`
+`scatfit-fitfrb fake_burst_500_DM.fil 500.0 --fitscatindex --fscrunch 128 --fast`
 
 You should see several diagnostic windows open. The terminal output should show an updated DM close to 500 pc cm^-3, a scattering index near -4.0, and a scattering time at 1 GHz of about 20 ms.
 
 ## Usage ##
 
 ```
 $ scatfit-fitfrb -h
-usage: scatfit-fitfrb [-h] [--compare] [--binburst bin] [--fscrunch factor] [--tscrunch factor] [--fast] [--fitscatindex]
+usage: scatfit-fitfrb [-h] [--compare] [--binburst bin] [--fscrunch factor] [--tscrunch factor] [--fast] [--fitrange start end]
+                      [--fitscatindex]
                       [--smodel {unscattered,scattered_isotropic_analytic,scattered_isotropic_convolving,scattered_isotropic_bandintegrated,scattered_isotropic_afb_instrumental,scattered_isotropic_dfb_instrumental}]
                       [--showmodels] [--snr snr] [--publish] [-z start end]
                       filename dm
 
 Fit a scattering model to FRB data.
 
 positional arguments:
@@ -73,24 +80,36 @@
 options:
   -h, --help            show this help message and exit
   --compare             Fit an unscattered Gaussian model for comparison. (default: False)
   --binburst bin        Specify the burst location bin manually. (default: None)
   --fscrunch factor     Integrate this many frequency channels. (default: 256)
   --tscrunch factor     Integrate this many time samples. (default: 1)
   --fast                Enable fast processing. This reduces the number of MCMC steps drastically. (default: False)
+  --fitrange start end  Consider only this time range of data in the fit. Increase the region for wide or highly-scattered bursts.
+                        Ensure that most of the scattering tail is included in the fit. (default: [-200.0, 200.0])
   --fitscatindex        Fit the scattering times and determine the scattering index. (default: False)
   --smodel {unscattered,scattered_isotropic_analytic,scattered_isotropic_convolving,scattered_isotropic_bandintegrated,scattered_isotropic_afb_instrumental,scattered_isotropic_dfb_instrumental}
                         Use the specified scattering model. (default: scattered_isotropic_analytic)
   --showmodels          Show comparison plot of scattering models. (default: False)
   --snr snr             Only consider sub-bands above this S/N threshold. (default: 3.8)
   --publish             Output plots suitable for publication. (default: False)
   -z start end, --zoom start end
                         Zoom into this time region. (default: [-50.0, 50.0])
 ```
 
+```
+$ scatfit-simpulse -h
+usage: scatfit-simpulse [-h]
+
+Simulate scattered pulses.
+
+options:
+  -h, --help  show this help message and exit
+```
+
 ## Profile scattering models ##
 
 Several profile scattering models, i.e. pulse broadening functions and instrumental contributions, are implemented and others can easily be added. The image below shows a selection of them.
 
 ![Implemented profile scattering models](https://github.com/fjankowsk/scatfit/raw/master/docs/profile_models.png "Implemented profile scattering models")
 
 ## Example output ##
@@ -112,7 +131,11 @@
 ### Why do I get the following warning: `Could not import Cython pulse model implementations. Falling back to the Python versions.`? ###
 
 This could happen if you run `scatfit` from its software repository git checkout, where the current working directory takes import preference. Install the software as above and run it as `$ scatfit-fitfrb` in a different path.
 
 ### What data formats are supported? ###
 
 `scatfit` supports loading data from `SIGPROC` filterbank files. Alternative loaders can be implemented relatively easily.
+
+### Does it work on ARM-based Macs? ###
+
+Yes, `scatfit` works on ARM-based Macs with M1 or M2 processors. In fact, it runs blazing fast on them! The immense single-core performance results in a speedup of > 3x in comparison with similar x64-based systems, in my experience.
```

### Comparing `scatfit-0.2.19/scatfit.egg-info/SOURCES.txt` & `scatfit-0.2.20/scatfit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scatfit-0.2.19/setup.py` & `scatfit-0.2.20/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -52,28 +52,22 @@
     entry_points={
         "console_scripts": [
             "scatfit-fitfrb = scatfit.apps.fit_frb:main",
             "scatfit-simpulse = scatfit.apps.simulate_pulse:main",
         ],
     },
     extras_require={
-        "develop": [
-            "black",
-            "Cython",
-            "nose2",
-        ],
+        "develop": ["black", "Cython", "pytest", "pytest-cov", "twine"],
     },
     ext_modules=[
         Extension(
             name="scatfit.pulsemodels_cython",
             sources=["scatfit/pulsemodels_cython.pyx"],
         ),
     ],
-    test_suite="nose2.collector.collector",
-    tests_require=["nose2"],
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 2",
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
     ],
```

### Comparing `scatfit-0.2.19/tests/test_pulsemodels.py` & `scatfit-0.2.20/tests/test_pulsemodels.py`

 * *Files 9% similar despite different names*

```diff
@@ -84,10 +84,10 @@
                     )
                     assert np.median(rel_residual) < 1e-8
                     assert np.mean(rel_residual) < 0.01
                     assert np.all(rel_residual < 0.07)
 
 
 if __name__ == "__main__":
-    import nose2
+    import pytest
 
-    nose2.main()
+    pytest.main([__file__])
```

### Comparing `scatfit-0.2.19/tests/test_pulsemodels_cython.py` & `scatfit-0.2.20/tests/test_pulsemodels_cython.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,10 +99,10 @@
                         )
 
                         # ensure that curves differ little
                         assert np.allclose(curve_python, curve_cython)
 
 
 if __name__ == "__main__":
-    import nose2
+    import pytest
 
-    nose2.main()
+    pytest.main([__file__])
```

### Comparing `scatfit-0.2.19/tests/test_pulsemodels_visual.py` & `scatfit-0.2.20/tests/test_pulsemodels_visual.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-import numpy as np
+import pytest
 
+import numpy as np
 import matplotlib.pyplot as plt
 
 import scatfit.pulsemodels as pulsemodels
 
 
 def plot_comparison(plot_range, curve1, curve2):
     """
@@ -42,14 +43,15 @@
     fig.align_ylabels()
 
     fig.tight_layout()
 
     return fig
 
 
+@pytest.mark.interactive
 def test_compare_models():
     """
     Compare the models visually.
     """
 
     plot_range = np.arange(40000) * 0.025
     plot_range -= plot_range[20000]
```

