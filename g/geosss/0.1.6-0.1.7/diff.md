# Comparing `tmp/geosss-0.1.6.tar.gz` & `tmp/geosss-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geosss-0.1.6.tar", max compression
+gzip compressed data, was "geosss-0.1.7.tar", max compression
```

## Comparing `geosss-0.1.6.tar` & `geosss-0.1.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1474 2023-07-24 16:27:27.579099 geosss-0.1.6/LICENSE
--rw-r--r--   0        0        0     4772 2023-07-26 13:19:07.794133 geosss-0.1.6/README.md
--rw-r--r--   0        0        0      793 2023-07-25 18:35:32.784913 geosss-0.1.6/geosss/__init__.py
--rw-r--r--   0        0        0     1981 2023-07-25 18:35:32.784913 geosss-0.1.6/geosss/demo_vis.py
--rw-r--r--   0        0        0     5522 2023-07-25 18:35:32.784913 geosss-0.1.6/geosss/distributions.py
--rw-r--r--   0        0        0    10284 2023-07-25 18:35:32.784913 geosss-0.1.6/geosss/mcmc.py
--rw-r--r--   0        0        0     5091 2023-07-25 18:35:32.784913 geosss-0.1.6/geosss/rand.py
--rw-r--r--   0        0        0     3000 2023-07-25 18:35:32.784913 geosss-0.1.6/geosss/sphere.py
--rw-r--r--   0        0        0     7334 2023-07-25 18:35:32.784913 geosss-0.1.6/geosss/testing.py
--rw-r--r--   0        0        0     5156 2023-07-25 18:35:32.784913 geosss-0.1.6/geosss/utils.py
--rw-r--r--   0        0        0     9249 2023-07-25 18:35:32.784913 geosss-0.1.6/geosss/vMF_diagnostics.py
--rw-r--r--   0        0        0      967 2023-07-26 12:59:39.769724 geosss-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     5751 1970-01-01 00:00:00.000000 geosss-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1474 2023-07-24 16:27:27.579099 geosss-0.1.7/LICENSE
+-rw-r--r--   0        0        0     4834 2023-08-04 10:22:11.067558 geosss-0.1.7/README.md
+-rw-r--r--   0        0        0      793 2023-07-25 18:35:32.784913 geosss-0.1.7/geosss/__init__.py
+-rw-r--r--   0        0        0     1981 2023-07-25 18:35:32.784913 geosss-0.1.7/geosss/demo_vis.py
+-rw-r--r--   0        0        0     5522 2023-07-25 18:35:32.784913 geosss-0.1.7/geosss/distributions.py
+-rw-r--r--   0        0        0    10284 2023-07-25 18:35:32.784913 geosss-0.1.7/geosss/mcmc.py
+-rw-r--r--   0        0        0     5091 2023-07-25 18:35:32.784913 geosss-0.1.7/geosss/rand.py
+-rw-r--r--   0        0        0     3000 2023-07-25 18:35:32.784913 geosss-0.1.7/geosss/sphere.py
+-rw-r--r--   0        0        0     7334 2023-07-25 18:35:32.784913 geosss-0.1.7/geosss/testing.py
+-rw-r--r--   0        0        0     5156 2023-07-25 18:35:32.784913 geosss-0.1.7/geosss/utils.py
+-rw-r--r--   0        0        0     9249 2023-07-25 18:35:32.784913 geosss-0.1.7/geosss/vMF_diagnostics.py
+-rw-r--r--   0        0        0     1068 2023-08-04 10:40:23.159238 geosss-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     5935 1970-01-01 00:00:00.000000 geosss-0.1.7/PKG-INFO
```

### Comparing `geosss-0.1.6/LICENSE` & `geosss-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `geosss-0.1.6/README.md` & `geosss-0.1.7/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,38 +1,49 @@
 <p align="center">
 <img src="https://raw.githubusercontent.com/microscopic-image-analysis/geosss/927ff8c8187b88a1a72725c4e450ae0f0523431b/assets/logo.svg" width="300">
 </p>
 
-[![PyPI](https://img.shields.io/pypi/v/geosss)](https://pypi.org/project/geosss/)
-![Python 3.9+](https://img.shields.io/badge/python-3.9+-green.svg)
-[![arXiv](https://img.shields.io/badge/DOI-10.1038%2Fs41586--020--2649--2-blue)](
-https://doi.org/10.48550/arXiv.2301.08056)
-[![License](https://img.shields.io/badge/License-BSD_3--Clause-purple.svg)](https://opensource.org/licenses/BSD-3-Clause)
+<div align="center">
+
+  [![PyPI](https://img.shields.io/pypi/v/geosss)](https://pypi.org/project/geosss/)
+  ![Python 3.9+](https://img.shields.io/badge/python-3.9+-green.svg)
+  [![arXiv](https://img.shields.io/badge/DOI-10.1038%2Fs41586--020--2649--2-blue)](
+  https://doi.org/10.48550/arXiv.2301.08056)
+  [![License](https://img.shields.io/badge/License-BSD_3--Clause-purple.svg)](https://opensource.org/licenses/BSD-3-Clause)
+
+</div>
 
 # GeoSSS: Geodesic Slice Sampling on the Sphere
 
-This Python package implements two novel tuning-free MCMC algorithms, an **ideal geodesic slice sampler** based on accept/reject strategy and a **shrinkage-based geodesic slice sampler** to sample from spherical distributions on arbitrary dimensions. The package also includes the implementation of random-walk Metropolis-Hastings (RWMH) and Hamiltonian Monte Carlo (HMC) whose step-size parameter is automatically tuned.
+This python package implements two novel tuning-free MCMC algorithms, an **ideal geodesic slice sampler** based on accept/reject strategy and a **shrinkage-based geodesic slice sampler** to sample from spherical distributions on arbitrary dimensions. The package also includes the implementation of random-walk Metropolis-Hastings (RWMH) and Hamiltonian Monte Carlo (HMC) whose step-size parameter is automatically tuned.
 As shown in our [paper](https://doi.org/10.48550/arXiv.2301.08056), our algorithms have outperformed RWMH and HMC for spherical distributions. 
 
 This demo quickly illustrates that. We consider a target that is a mixture of von Mises-Fisher distribution on a 2-sphere with concentration parameter $\kappa=80$. By using $10^3$ samples, our samplers GeoSSS (reject) and GeoSSS (shrink) (top row) explore all modes, whereas RWMH and HMC (bottom row) get stuck in a single mode. 
 
 ![animation_vMF](https://github.com/microscopic-image-analysis/geosss/blob/927ff8c8187b88a1a72725c4e450ae0f0523431b/assets/animation_vMF.gif?raw=true)
 
 ## Installation
 
 GeoSSS is available for installation from [PyPI](https://pypi.org/project/geosss/). Therefore, simply type:
 
 ```bash
 pip install geosss
 ```
 
+To install dependencies required to run scripts under [`scripts/`](scripts/),
+
+```bash
+pip install geosss[extras]
+```
+
 ## Getting Started
 
 A minimal example to get started as well as reproduce the above demo:
 
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/microscopic-image-analysis/geosss/blob/main/scripts/demo.ipynb)
 ```python
 import geosss as gs
 import numpy as np
 
 # parameters for mixture of von Mises-Fisher (vMF)
 # distributions
 d = 3                          # required dimension
@@ -87,22 +98,14 @@
 
 ```bash
 git clone https://github.com/microscopic-image-analysis/geosss.git
 cd geosss
 pip install .[dev]
 ```
 
-Alternatively, you can install this package with [poetry](https://github.com/python-poetry/poetry) in a dedicated virtual environment with the following commands:
-
-```bash
-git clone https://github.com/microscopic-image-analysis/geosss.git
-cd geosss
-poetry install --all-extras
-```
-
 ## Citation
 
 If you use this package, or ideas from the paper, please consider citing us.
 ```bash
 @misc{habeck2023,
       title={Geodesic slice sampling on the sphere}, 
       author={Michael Habeck and Mareike Hasenpflug and Shantanu Kodgirwar and Daniel Rudolf},
```

### Comparing `geosss-0.1.6/geosss/__init__.py` & `geosss-0.1.7/geosss/__init__.py`

 * *Files identical despite different names*

### Comparing `geosss-0.1.6/geosss/demo_vis.py` & `geosss-0.1.7/geosss/demo_vis.py`

 * *Files identical despite different names*

### Comparing `geosss-0.1.6/geosss/distributions.py` & `geosss-0.1.7/geosss/distributions.py`

 * *Files identical despite different names*

### Comparing `geosss-0.1.6/geosss/mcmc.py` & `geosss-0.1.7/geosss/mcmc.py`

 * *Files identical despite different names*

### Comparing `geosss-0.1.6/geosss/rand.py` & `geosss-0.1.7/geosss/rand.py`

 * *Files identical despite different names*

### Comparing `geosss-0.1.6/geosss/sphere.py` & `geosss-0.1.7/geosss/sphere.py`

 * *Files identical despite different names*

### Comparing `geosss-0.1.6/geosss/testing.py` & `geosss-0.1.7/geosss/testing.py`

 * *Files identical despite different names*

### Comparing `geosss-0.1.6/geosss/utils.py` & `geosss-0.1.7/geosss/utils.py`

 * *Files identical despite different names*

### Comparing `geosss-0.1.6/geosss/vMF_diagnostics.py` & `geosss-0.1.7/geosss/vMF_diagnostics.py`

 * *Files identical despite different names*

### Comparing `geosss-0.1.6/pyproject.toml` & `geosss-0.1.7/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "geosss"
-version = "0.1.6"
+version = "0.1.7"
 description = "Python package implementing an ideal and shrinkage-based geodesic slice sampling on the sphere."
 authors = ["Michael Habeck <michael.habeck@uni-jena.de>",
            "Shantanu Kodgirwar <shantanu.kodgirwar@uni-jena.de>", 
            "Mareike Hasenpflug <mareike.hasenpflug@uni-passau.de>",
            "Daniel Rudolf <daniel.rudolf@uni-passau.de>"]
 license = "BSD-3-Clause"
 readme = "README.md"
@@ -16,14 +16,16 @@
 numpy = "^1.25.1"
 matplotlib = "^3.7.2"
 csb = "^1.2.5"
 arviz = "^0.15.1"
 seaborn = { version = "^0.12.2", optional = true }
 tsp-solver = { version = "^0.1", optional = true }
 black = { version = "^23.7.0", optional = true }
+ipykernel = { version = "^6.25.0", optional = true }
 
 [tool.poetry.extras]
-dev = ["seaborn", "tsp-solver", "black"]
+extras = ["seaborn", "tsp-solver"]
+dev = ["seaborn", "tsp-solver", "black", "ipykernel"]
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `geosss-0.1.6/PKG-INFO` & `geosss-0.1.7/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,64 +1,77 @@
 Metadata-Version: 2.1
 Name: geosss
-Version: 0.1.6
+Version: 0.1.7
 Summary: Python package implementing an ideal and shrinkage-based geodesic slice sampling on the sphere.
 Home-page: https://github.com/microscopic-image-analysis/geosss
 License: BSD-3-Clause
 Author: Michael Habeck
 Author-email: michael.habeck@uni-jena.de
 Requires-Python: >=3.9,<3.13
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: dev
+Provides-Extra: extras
 Requires-Dist: arviz (>=0.15.1,<0.16.0)
 Requires-Dist: black (>=23.7.0,<24.0.0) ; extra == "dev"
 Requires-Dist: csb (>=1.2.5,<2.0.0)
+Requires-Dist: ipykernel (>=6.25.0,<7.0.0) ; extra == "dev"
 Requires-Dist: matplotlib (>=3.7.2,<4.0.0)
 Requires-Dist: numpy (>=1.25.1,<2.0.0)
 Requires-Dist: scipy (>=1.11.1,<2.0.0)
-Requires-Dist: seaborn (>=0.12.2,<0.13.0) ; extra == "dev"
-Requires-Dist: tsp-solver (>=0.1,<0.2) ; extra == "dev"
+Requires-Dist: seaborn (>=0.12.2,<0.13.0) ; extra == "extras" or extra == "dev"
+Requires-Dist: tsp-solver (>=0.1,<0.2) ; extra == "extras" or extra == "dev"
 Project-URL: Repository, https://github.com/microscopic-image-analysis/geosss
 Description-Content-Type: text/markdown
 
 <p align="center">
 <img src="https://raw.githubusercontent.com/microscopic-image-analysis/geosss/927ff8c8187b88a1a72725c4e450ae0f0523431b/assets/logo.svg" width="300">
 </p>
 
-[![PyPI](https://img.shields.io/pypi/v/geosss)](https://pypi.org/project/geosss/)
-![Python 3.9+](https://img.shields.io/badge/python-3.9+-green.svg)
-[![arXiv](https://img.shields.io/badge/DOI-10.1038%2Fs41586--020--2649--2-blue)](
-https://doi.org/10.48550/arXiv.2301.08056)
-[![License](https://img.shields.io/badge/License-BSD_3--Clause-purple.svg)](https://opensource.org/licenses/BSD-3-Clause)
+<div align="center">
+
+  [![PyPI](https://img.shields.io/pypi/v/geosss)](https://pypi.org/project/geosss/)
+  ![Python 3.9+](https://img.shields.io/badge/python-3.9+-green.svg)
+  [![arXiv](https://img.shields.io/badge/DOI-10.1038%2Fs41586--020--2649--2-blue)](
+  https://doi.org/10.48550/arXiv.2301.08056)
+  [![License](https://img.shields.io/badge/License-BSD_3--Clause-purple.svg)](https://opensource.org/licenses/BSD-3-Clause)
+
+</div>
 
 # GeoSSS: Geodesic Slice Sampling on the Sphere
 
-This Python package implements two novel tuning-free MCMC algorithms, an **ideal geodesic slice sampler** based on accept/reject strategy and a **shrinkage-based geodesic slice sampler** to sample from spherical distributions on arbitrary dimensions. The package also includes the implementation of random-walk Metropolis-Hastings (RWMH) and Hamiltonian Monte Carlo (HMC) whose step-size parameter is automatically tuned.
+This python package implements two novel tuning-free MCMC algorithms, an **ideal geodesic slice sampler** based on accept/reject strategy and a **shrinkage-based geodesic slice sampler** to sample from spherical distributions on arbitrary dimensions. The package also includes the implementation of random-walk Metropolis-Hastings (RWMH) and Hamiltonian Monte Carlo (HMC) whose step-size parameter is automatically tuned.
 As shown in our [paper](https://doi.org/10.48550/arXiv.2301.08056), our algorithms have outperformed RWMH and HMC for spherical distributions. 
 
 This demo quickly illustrates that. We consider a target that is a mixture of von Mises-Fisher distribution on a 2-sphere with concentration parameter $\kappa=80$. By using $10^3$ samples, our samplers GeoSSS (reject) and GeoSSS (shrink) (top row) explore all modes, whereas RWMH and HMC (bottom row) get stuck in a single mode. 
 
 ![animation_vMF](https://github.com/microscopic-image-analysis/geosss/blob/927ff8c8187b88a1a72725c4e450ae0f0523431b/assets/animation_vMF.gif?raw=true)
 
 ## Installation
 
 GeoSSS is available for installation from [PyPI](https://pypi.org/project/geosss/). Therefore, simply type:
 
 ```bash
 pip install geosss
 ```
 
+To install dependencies required to run scripts under [`scripts/`](scripts/),
+
+```bash
+pip install geosss[extras]
+```
+
 ## Getting Started
 
 A minimal example to get started as well as reproduce the above demo:
 
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/microscopic-image-analysis/geosss/blob/main/scripts/demo.ipynb)
 ```python
 import geosss as gs
 import numpy as np
 
 # parameters for mixture of von Mises-Fisher (vMF)
 # distributions
 d = 3                          # required dimension
@@ -113,22 +126,14 @@
 
 ```bash
 git clone https://github.com/microscopic-image-analysis/geosss.git
 cd geosss
 pip install .[dev]
 ```
 
-Alternatively, you can install this package with [poetry](https://github.com/python-poetry/poetry) in a dedicated virtual environment with the following commands:
-
-```bash
-git clone https://github.com/microscopic-image-analysis/geosss.git
-cd geosss
-poetry install --all-extras
-```
-
 ## Citation
 
 If you use this package, or ideas from the paper, please consider citing us.
 ```bash
 @misc{habeck2023,
       title={Geodesic slice sampling on the sphere}, 
       author={Michael Habeck and Mareike Hasenpflug and Shantanu Kodgirwar and Daniel Rudolf},
```

