# Comparing `tmp/citlalicue-0.7.0.tar.gz` & `tmp/citlalicue-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/barraganl/Dropbox/Projects/citlalicue/dist/tmp_5mmpq4j/citlalicue-0.7.0.tar", last modified: Tue Feb  1 09:41:42 2022, max compression
+gzip compressed data, was "citlalicue-0.7.1.tar", last modified: Fri Aug  4 10:56:55 2023, max compression
```

## Comparing `citlalicue-0.7.0.tar` & `citlalicue-0.7.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 barraganl  (1001) barraganl  (1002)        0 2022-02-01 09:41:41.000000 citlalicue-0.7.0/
--rw-r--r--   0 barraganl  (1001) barraganl  (1002)    35147 2020-07-03 15:20:18.000000 citlalicue-0.7.0/LICENSE
--rw-r--r--   0 barraganl  (1001) barraganl  (1002)     2015 2020-09-09 09:25:12.000000 citlalicue-0.7.0/README.md
--rw-r--r--   0 barraganl  (1001) barraganl  (1002)      783 2022-02-01 09:39:59.000000 citlalicue-0.7.0/setup.py
-drwxrwxr-x   0 barraganl  (1001) barraganl  (1002)        0 2022-02-01 09:41:41.000000 citlalicue-0.7.0/citlalicue.egg-info/
--rw-r--r--   0 barraganl  (1001) barraganl  (1002)      268 2022-02-01 09:41:41.000000 citlalicue-0.7.0/citlalicue.egg-info/SOURCES.txt
--rw-r--r--   0 barraganl  (1001) barraganl  (1002)        1 2022-02-01 09:41:41.000000 citlalicue-0.7.0/citlalicue.egg-info/dependency_links.txt
--rw-r--r--   0 barraganl  (1001) barraganl  (1002)       46 2022-02-01 09:41:41.000000 citlalicue-0.7.0/citlalicue.egg-info/requires.txt
--rw-r--r--   0 barraganl  (1001) barraganl  (1002)       11 2022-02-01 09:41:41.000000 citlalicue-0.7.0/citlalicue.egg-info/top_level.txt
--rw-r--r--   0 barraganl  (1001) barraganl  (1002)     2507 2022-02-01 09:41:41.000000 citlalicue-0.7.0/citlalicue.egg-info/PKG-INFO
--rw-rw-r--   0 barraganl  (1001) barraganl  (1002)     2507 2022-02-01 09:41:41.000000 citlalicue-0.7.0/PKG-INFO
-drwxrwxr-x   0 barraganl  (1001) barraganl  (1002)        0 2022-02-01 09:41:41.000000 citlalicue-0.7.0/citlalicue/
--rw-r--r--   0 barraganl  (1001) barraganl  (1002)    23041 2022-02-01 09:28:50.000000 citlalicue-0.7.0/citlalicue/detrending.py
--rw-r--r--   0 barraganl  (1001) barraganl  (1002)     5672 2021-05-17 12:56:02.000000 citlalicue-0.7.0/citlalicue/citlalicue.py
--rw-r--r--   0 barraganl  (1001) barraganl  (1002)        0 2020-07-03 15:21:10.000000 citlalicue-0.7.0/citlalicue/__init__.py
--rw-rw-r--   0 barraganl  (1001) barraganl  (1002)       38 2022-02-01 09:41:41.000000 citlalicue-0.7.0/setup.cfg
+drwxrwxr-x   0 barraganl  (1001) barraganl  (1002)        0 2023-08-04 10:56:55.008329 citlalicue-0.7.1/
+-rw-r--r--   0 barraganl  (1001) barraganl  (1002)    35147 2020-07-03 15:20:18.000000 citlalicue-0.7.1/LICENSE
+-rw-rw-r--   0 barraganl  (1001) barraganl  (1002)     2470 2023-08-04 10:56:55.008329 citlalicue-0.7.1/PKG-INFO
+-rw-r--r--   0 barraganl  (1001) barraganl  (1002)     2015 2020-09-09 09:25:12.000000 citlalicue-0.7.1/README.md
+drwxrwxr-x   0 barraganl  (1001) barraganl  (1002)        0 2023-08-04 10:56:55.008329 citlalicue-0.7.1/citlalicue/
+-rw-r--r--   0 barraganl  (1001) barraganl  (1002)        0 2020-07-03 15:21:10.000000 citlalicue-0.7.1/citlalicue/__init__.py
+-rw-r--r--   0 barraganl  (1001) barraganl  (1002)     5672 2021-05-17 12:56:02.000000 citlalicue-0.7.1/citlalicue/citlalicue.py
+-rw-r--r--   0 barraganl  (1001) barraganl  (1002)    23041 2022-02-01 09:28:50.000000 citlalicue-0.7.1/citlalicue/detrending.py
+drwxrwxr-x   0 barraganl  (1001) barraganl  (1002)        0 2023-08-04 10:56:55.008329 citlalicue-0.7.1/citlalicue.egg-info/
+-rw-r--r--   0 barraganl  (1001) barraganl  (1002)     2470 2023-08-04 10:56:55.000000 citlalicue-0.7.1/citlalicue.egg-info/PKG-INFO
+-rw-r--r--   0 barraganl  (1001) barraganl  (1002)      268 2023-08-04 10:56:55.000000 citlalicue-0.7.1/citlalicue.egg-info/SOURCES.txt
+-rw-r--r--   0 barraganl  (1001) barraganl  (1002)        1 2023-08-04 10:56:55.000000 citlalicue-0.7.1/citlalicue.egg-info/dependency_links.txt
+-rw-r--r--   0 barraganl  (1001) barraganl  (1002)       73 2023-08-04 10:56:55.000000 citlalicue-0.7.1/citlalicue.egg-info/requires.txt
+-rw-r--r--   0 barraganl  (1001) barraganl  (1002)       11 2023-08-04 10:56:55.000000 citlalicue-0.7.1/citlalicue.egg-info/top_level.txt
+-rw-rw-r--   0 barraganl  (1001) barraganl  (1002)       38 2023-08-04 10:56:55.008329 citlalicue-0.7.1/setup.cfg
+-rw-r--r--   0 barraganl  (1001) barraganl  (1002)      831 2023-08-04 10:55:05.000000 citlalicue-0.7.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `citlalicue-0.7.0/LICENSE` & `citlalicue-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `citlalicue-0.7.0/README.md` & `citlalicue-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `citlalicue-0.7.0/setup.py` & `citlalicue-0.7.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="citlalicue",
-    version="0.7.0",
+    version="0.7.1",
     author="Oscar Barragán",
     author_email="oscaribv@gmail.com",
     description="Create stellar light curves!",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/oscaribv/citlalicue",
     packages=setuptools.find_packages(),
      install_requires = ["numpy",
     "matplotlib",
     "scipy",
     "pytransit",
     "george",
-    "emcee"],
+    "emcee",
+    "celerite",
+    "corner",
+    "lightkurve"],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3',
 )
```

### Comparing `citlalicue-0.7.0/citlalicue.egg-info/PKG-INFO` & `citlalicue-0.7.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: citlalicue
-Version: 0.7.0
+Version: 0.7.1
 Summary: Create stellar light curves!
 Home-page: https://github.com/oscaribv/citlalicue
 Author: Oscar Barragán
 Author-email: oscaribv@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -51,9 +49,7 @@
 Check the example of how to use Citlalicue to create light curves in the link
 [example_light_curves.ipynb](https://github.com/oscaribv/citlalicue/blob/master/example_light_curves.ipynb).
 
 ### Detrend light curves
 
 Check the example of how to use Citlalicue to detrend light curves in the link
 [example_detrending.ipynb](https://github.com/oscaribv/citlalicue/blob/master/example_detrending.ipynb).
-
-
```

#### html2text {}

```diff
@@ -1,27 +1,27 @@
-Metadata-Version: 2.1 Name: citlalicue Version: 0.7.0 Summary: Create stellar
+Metadata-Version: 2.1 Name: citlalicue Version: 0.7.1 Summary: Create stellar
 light curves! Home-page: https://github.com/oscaribv/citlalicue Author: Oscar
-BarragÃ¡n Author-email: oscaribv@gmail.com License: UNKNOWN Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
-Approved :: GNU General Public License v3 (GPLv3) Classifier: Operating System
-:: OS Independent Requires-Python: >=3 Description-Content-Type: text/markdown
-License-File: LICENSE # Citlalicue ### Oscar BarragÃ¡n (Sept 2020)
-*_Citlalicue_* is the name of the Aztec Goddess who created the stars. This
-code allows you to mimic Citlalicue powers to create and manipulate stellar
-light curves. The actual version of the code allows you to create synthetic
-stellar light curves (transits, stellar variability and white noise) and
-detrend light curves using Gaussian Processes (GPs). ##### Dependencies: *
-Numpy * Matplotlib * Scipy * [PyTransit](https://github.com/hpparvi/PyTransit)
-* [george](https://github.com/dfm/george) ##### Try it now! Install it by
-typing ``` pip install citlalicue ``` ### Simulate light curves Transits are
-implemented using [PyTransit](https://github.com/hpparvi/PyTransit), while the
-stellar variability is added from samples of a Quasi-Periodic Kernel with
-covariance given by [https://latex.codecogs.com/gif.latex?\gamma
-(t_i,t_j)&space;=&space;A&space;\exp&space;\left[&space;-&space;\frac{\sin^2
-[\pi(t_i&space;-&space;t_j)/P_{\rm&space;GP}]}{2&space;\lambda_
-{\rm&space;P}^2}&space;-&space;\frac{(t_i&space;-&space;t_j)^2}{2\lambda_
-{\rm&space;e}^2}&space;\right]] Check the example of how to use Citlalicue to
-create light curves in the link [example_light_curves.ipynb](https://
-github.com/oscaribv/citlalicue/blob/master/example_light_curves.ipynb). ###
-Detrend light curves Check the example of how to use Citlalicue to detrend
-light curves in the link [example_detrending.ipynb](https://github.com/
-oscaribv/citlalicue/blob/master/example_detrending.ipynb).
+BarragÃ¡n Author-email: oscaribv@gmail.com Classifier: Programming Language ::
+Python :: 3 Classifier: License :: OSI Approved :: GNU General Public License
+v3 (GPLv3) Classifier: Operating System :: OS Independent Requires-Python: >=3
+Description-Content-Type: text/markdown License-File: LICENSE # Citlalicue ###
+Oscar BarragÃ¡n (Sept 2020) *_Citlalicue_* is the name of the Aztec Goddess who
+created the stars. This code allows you to mimic Citlalicue powers to create
+and manipulate stellar light curves. The actual version of the code allows you
+to create synthetic stellar light curves (transits, stellar variability and
+white noise) and detrend light curves using Gaussian Processes (GPs). #####
+Dependencies: * Numpy * Matplotlib * Scipy * [PyTransit](https://github.com/
+hpparvi/PyTransit) * [george](https://github.com/dfm/george) ##### Try it now!
+Install it by typing ``` pip install citlalicue ``` ### Simulate light curves
+Transits are implemented using [PyTransit](https://github.com/hpparvi/
+PyTransit), while the stellar variability is added from samples of a Quasi-
+Periodic Kernel with covariance given by [https://latex.codecogs.com/
+gif.latex?\gamma(t_i,t_j)&space;=&space;A&space;\exp&space;\left[&space;-
+&space;\frac{\sin^2[\pi(t_i&space;-&space;t_j)/P_{\rm&space;GP}]}
+{2&space;\lambda_{\rm&space;P}^2}&space;-&space;\frac{(t_i&space;-
+&space;t_j)^2}{2\lambda_{\rm&space;e}^2}&space;\right]] Check the example of
+how to use Citlalicue to create light curves in the link
+[example_light_curves.ipynb](https://github.com/oscaribv/citlalicue/blob/
+master/example_light_curves.ipynb). ### Detrend light curves Check the example
+of how to use Citlalicue to detrend light curves in the link
+[example_detrending.ipynb](https://github.com/oscaribv/citlalicue/blob/master/
+example_detrending.ipynb).
```

### Comparing `citlalicue-0.7.0/PKG-INFO` & `citlalicue-0.7.1/citlalicue.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: citlalicue
-Version: 0.7.0
+Version: 0.7.1
 Summary: Create stellar light curves!
 Home-page: https://github.com/oscaribv/citlalicue
 Author: Oscar Barragán
 Author-email: oscaribv@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -51,9 +49,7 @@
 Check the example of how to use Citlalicue to create light curves in the link
 [example_light_curves.ipynb](https://github.com/oscaribv/citlalicue/blob/master/example_light_curves.ipynb).
 
 ### Detrend light curves
 
 Check the example of how to use Citlalicue to detrend light curves in the link
 [example_detrending.ipynb](https://github.com/oscaribv/citlalicue/blob/master/example_detrending.ipynb).
-
-
```

#### html2text {}

```diff
@@ -1,27 +1,27 @@
-Metadata-Version: 2.1 Name: citlalicue Version: 0.7.0 Summary: Create stellar
+Metadata-Version: 2.1 Name: citlalicue Version: 0.7.1 Summary: Create stellar
 light curves! Home-page: https://github.com/oscaribv/citlalicue Author: Oscar
-BarragÃ¡n Author-email: oscaribv@gmail.com License: UNKNOWN Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
-Approved :: GNU General Public License v3 (GPLv3) Classifier: Operating System
-:: OS Independent Requires-Python: >=3 Description-Content-Type: text/markdown
-License-File: LICENSE # Citlalicue ### Oscar BarragÃ¡n (Sept 2020)
-*_Citlalicue_* is the name of the Aztec Goddess who created the stars. This
-code allows you to mimic Citlalicue powers to create and manipulate stellar
-light curves. The actual version of the code allows you to create synthetic
-stellar light curves (transits, stellar variability and white noise) and
-detrend light curves using Gaussian Processes (GPs). ##### Dependencies: *
-Numpy * Matplotlib * Scipy * [PyTransit](https://github.com/hpparvi/PyTransit)
-* [george](https://github.com/dfm/george) ##### Try it now! Install it by
-typing ``` pip install citlalicue ``` ### Simulate light curves Transits are
-implemented using [PyTransit](https://github.com/hpparvi/PyTransit), while the
-stellar variability is added from samples of a Quasi-Periodic Kernel with
-covariance given by [https://latex.codecogs.com/gif.latex?\gamma
-(t_i,t_j)&space;=&space;A&space;\exp&space;\left[&space;-&space;\frac{\sin^2
-[\pi(t_i&space;-&space;t_j)/P_{\rm&space;GP}]}{2&space;\lambda_
-{\rm&space;P}^2}&space;-&space;\frac{(t_i&space;-&space;t_j)^2}{2\lambda_
-{\rm&space;e}^2}&space;\right]] Check the example of how to use Citlalicue to
-create light curves in the link [example_light_curves.ipynb](https://
-github.com/oscaribv/citlalicue/blob/master/example_light_curves.ipynb). ###
-Detrend light curves Check the example of how to use Citlalicue to detrend
-light curves in the link [example_detrending.ipynb](https://github.com/
-oscaribv/citlalicue/blob/master/example_detrending.ipynb).
+BarragÃ¡n Author-email: oscaribv@gmail.com Classifier: Programming Language ::
+Python :: 3 Classifier: License :: OSI Approved :: GNU General Public License
+v3 (GPLv3) Classifier: Operating System :: OS Independent Requires-Python: >=3
+Description-Content-Type: text/markdown License-File: LICENSE # Citlalicue ###
+Oscar BarragÃ¡n (Sept 2020) *_Citlalicue_* is the name of the Aztec Goddess who
+created the stars. This code allows you to mimic Citlalicue powers to create
+and manipulate stellar light curves. The actual version of the code allows you
+to create synthetic stellar light curves (transits, stellar variability and
+white noise) and detrend light curves using Gaussian Processes (GPs). #####
+Dependencies: * Numpy * Matplotlib * Scipy * [PyTransit](https://github.com/
+hpparvi/PyTransit) * [george](https://github.com/dfm/george) ##### Try it now!
+Install it by typing ``` pip install citlalicue ``` ### Simulate light curves
+Transits are implemented using [PyTransit](https://github.com/hpparvi/
+PyTransit), while the stellar variability is added from samples of a Quasi-
+Periodic Kernel with covariance given by [https://latex.codecogs.com/
+gif.latex?\gamma(t_i,t_j)&space;=&space;A&space;\exp&space;\left[&space;-
+&space;\frac{\sin^2[\pi(t_i&space;-&space;t_j)/P_{\rm&space;GP}]}
+{2&space;\lambda_{\rm&space;P}^2}&space;-&space;\frac{(t_i&space;-
+&space;t_j)^2}{2\lambda_{\rm&space;e}^2}&space;\right]] Check the example of
+how to use Citlalicue to create light curves in the link
+[example_light_curves.ipynb](https://github.com/oscaribv/citlalicue/blob/
+master/example_light_curves.ipynb). ### Detrend light curves Check the example
+of how to use Citlalicue to detrend light curves in the link
+[example_detrending.ipynb](https://github.com/oscaribv/citlalicue/blob/master/
+example_detrending.ipynb).
```

### Comparing `citlalicue-0.7.0/citlalicue/detrending.py` & `citlalicue-0.7.1/citlalicue/detrending.py`

 * *Files identical despite different names*

### Comparing `citlalicue-0.7.0/citlalicue/citlalicue.py` & `citlalicue-0.7.1/citlalicue/citlalicue.py`

 * *Files identical despite different names*

