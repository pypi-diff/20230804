# Comparing `tmp/ripplegw-0.0.2.tar.gz` & `tmp/ripplegw-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ripplegw-0.0.2.tar", last modified: Thu Apr 20 15:10:44 2023, max compression
+gzip compressed data, was "ripplegw-0.0.3.tar", last modified: Fri Aug  4 17:00:41 2023, max compression
```

## Comparing `ripplegw-0.0.2.tar` & `ripplegw-0.0.3.tar`

### file list

```diff
@@ -1,37 +1,34 @@
-drwxr-xr-x   0 thomasedwards   (501) staff       (20)        0 2023-04-20 15:10:44.892833 ripplegw-0.0.2/
--rw-r--r--   0 thomasedwards   (501) staff       (20)     1088 2022-10-12 22:06:55.000000 ripplegw-0.0.2/LICENSE
--rw-r--r--   0 thomasedwards   (501) staff       (20)     2735 2023-04-20 15:10:44.892911 ripplegw-0.0.2/PKG-INFO
--rw-r--r--   0 thomasedwards   (501) staff       (20)     2208 2023-04-20 15:08:56.000000 ripplegw-0.0.2/README.md
--rw-r--r--   0 thomasedwards   (501) staff       (20)      104 2022-10-12 22:06:55.000000 ripplegw-0.0.2/pyproject.toml
--rw-r--r--   0 thomasedwards   (501) staff       (20)      726 2023-04-20 15:10:44.893286 ripplegw-0.0.2/setup.cfg
--rw-r--r--   0 thomasedwards   (501) staff       (20)       38 2022-10-12 22:06:55.000000 ripplegw-0.0.2/setup.py
-drwxr-xr-x   0 thomasedwards   (501) staff       (20)        0 2023-04-20 15:10:44.885270 ripplegw-0.0.2/src/
-drwxr-xr-x   0 thomasedwards   (501) staff       (20)        0 2023-04-20 15:10:44.886652 ripplegw-0.0.2/src/ripple/
--rw-r--r--   0 thomasedwards   (501) staff       (20)     9886 2023-01-26 20:48:01.000000 ripplegw-0.0.2/src/ripple/__init__.py
--rw-r--r--   0 thomasedwards   (501) staff       (20)      483 2023-01-06 18:06:40.000000 ripplegw-0.0.2/src/ripple/constants.py
--rw-r--r--   0 thomasedwards   (501) staff       (20)     4002 2022-10-12 22:06:55.000000 ripplegw-0.0.2/src/ripple/noise.py
-drwxr-xr-x   0 thomasedwards   (501) staff       (20)        0 2023-04-20 15:10:44.890385 ripplegw-0.0.2/src/ripple/noise_resources/
--rw-r--r--   0 thomasedwards   (501) staff       (20)    48230 2022-10-12 22:06:55.000000 ripplegw-0.0.2/src/ripple/noise_resources/O2_ASD.dat
--rw-r--r--   0 thomasedwards   (501) staff       (20)  1117811 2022-10-12 22:06:55.000000 ripplegw-0.0.2/src/ripple/noise_resources/O3a_Livingston_ASD.dat
--rw-r--r--   0 thomasedwards   (501) staff       (20)        0 2022-10-12 22:06:55.000000 ripplegw-0.0.2/src/ripple/noise_resources/__init__.py
--rw-r--r--   0 thomasedwards   (501) staff       (20)    56415 2022-10-12 22:06:55.000000 ripplegw-0.0.2/src/ripple/noise_resources/aLIGO.dat
--rw-r--r--   0 thomasedwards   (501) staff       (20)    10070 2022-10-12 22:06:55.000000 ripplegw-0.0.2/src/ripple/noise_resources/aLIGOZeroDetHighPower.dat
--rw-r--r--   0 thomasedwards   (501) staff       (20)    87114 2022-10-12 22:06:55.000000 ripplegw-0.0.2/src/ripple/noise_resources/ce.dat
--rw-r--r--   0 thomasedwards   (501) staff       (20)    87132 2022-10-12 22:06:55.000000 ripplegw-0.0.2/src/ripple/noise_resources/et.dat
--rw-r--r--   0 thomasedwards   (501) staff       (20)      201 2022-10-12 22:06:55.000000 ripplegw-0.0.2/src/ripple/typing.py
-drwxr-xr-x   0 thomasedwards   (501) staff       (20)        0 2023-04-20 15:10:44.891828 ripplegw-0.0.2/src/ripple/waveforms/
--rw-r--r--   0 thomasedwards   (501) staff       (20)    19476 2023-04-20 15:01:50.000000 ripplegw-0.0.2/src/ripple/waveforms/IMRPhenomD.py
--rw-r--r--   0 thomasedwards   (501) staff       (20)    53661 2023-01-31 13:59:58.000000 ripplegw-0.0.2/src/ripple/waveforms/IMRPhenomD_QNMdata.py
--rw-r--r--   0 thomasedwards   (501) staff       (20)    15783 2023-01-06 19:15:14.000000 ripplegw-0.0.2/src/ripple/waveforms/IMRPhenomD_utils.py
--rw-r--r--   0 thomasedwards   (501) staff       (20)    44771 2023-04-20 15:01:50.000000 ripplegw-0.0.2/src/ripple/waveforms/IMRPhenomXAS.py
--rw-r--r--   0 thomasedwards   (501) staff       (20)    39958 2023-04-20 15:01:50.000000 ripplegw-0.0.2/src/ripple/waveforms/IMRPhenomX_utils.py
--rw-r--r--   0 thomasedwards   (501) staff       (20)        0 2022-10-12 22:06:55.000000 ripplegw-0.0.2/src/ripple/waveforms/__init__.py
-drwxr-xr-x   0 thomasedwards   (501) staff       (20)        0 2023-04-20 15:10:44.892448 ripplegw-0.0.2/src/ripplegw.egg-info/
--rw-r--r--   0 thomasedwards   (501) staff       (20)     2735 2023-04-20 15:10:44.000000 ripplegw-0.0.2/src/ripplegw.egg-info/PKG-INFO
--rw-r--r--   0 thomasedwards   (501) staff       (20)      881 2023-04-20 15:10:44.000000 ripplegw-0.0.2/src/ripplegw.egg-info/SOURCES.txt
--rw-r--r--   0 thomasedwards   (501) staff       (20)        1 2023-04-20 15:10:44.000000 ripplegw-0.0.2/src/ripplegw.egg-info/dependency_links.txt
--rw-r--r--   0 thomasedwards   (501) staff       (20)       17 2023-04-20 15:10:44.000000 ripplegw-0.0.2/src/ripplegw.egg-info/requires.txt
--rw-r--r--   0 thomasedwards   (501) staff       (20)        7 2023-04-20 15:10:44.000000 ripplegw-0.0.2/src/ripplegw.egg-info/top_level.txt
-drwxr-xr-x   0 thomasedwards   (501) staff       (20)        0 2023-04-20 15:10:44.892714 ripplegw-0.0.2/test/
--rw-r--r--   0 thomasedwards   (501) staff       (20)    26166 2023-04-20 15:01:50.000000 ripplegw-0.0.2/test/test_IMRPhenomX.py
--rw-r--r--   0 thomasedwards   (501) staff       (20)    21003 2023-01-30 21:58:17.000000 ripplegw-0.0.2/test/test_imrphenomd.py
+drwxr-xr-x   0 thomasedwards   (501) staff       (20)        0 2023-08-04 17:00:41.425680 ripplegw-0.0.3/
+-rw-r--r--   0 thomasedwards   (501) staff       (20)     1088 2022-10-12 22:06:55.000000 ripplegw-0.0.3/LICENSE
+-rw-r--r--   0 thomasedwards   (501) staff       (20)     3126 2023-08-04 17:00:41.425955 ripplegw-0.0.3/PKG-INFO
+-rw-r--r--   0 thomasedwards   (501) staff       (20)     2600 2023-08-04 16:58:21.000000 ripplegw-0.0.3/README.md
+-rw-r--r--   0 thomasedwards   (501) staff       (20)      104 2022-10-12 22:06:55.000000 ripplegw-0.0.3/pyproject.toml
+-rw-r--r--   0 thomasedwards   (501) staff       (20)      725 2023-08-04 17:00:41.431237 ripplegw-0.0.3/setup.cfg
+-rw-r--r--   0 thomasedwards   (501) staff       (20)       38 2022-10-12 22:06:55.000000 ripplegw-0.0.3/setup.py
+drwxr-xr-x   0 thomasedwards   (501) staff       (20)        0 2023-08-04 17:00:41.296975 ripplegw-0.0.3/src/
+drwxr-xr-x   0 thomasedwards   (501) staff       (20)        0 2023-08-04 17:00:41.334527 ripplegw-0.0.3/src/ripple/
+-rw-r--r--   0 thomasedwards   (501) staff       (20)     9943 2023-08-04 16:58:21.000000 ripplegw-0.0.3/src/ripple/__init__.py
+-rw-r--r--   0 thomasedwards   (501) staff       (20)      483 2023-01-06 18:06:40.000000 ripplegw-0.0.3/src/ripple/constants.py
+-rw-r--r--   0 thomasedwards   (501) staff       (20)     3156 2023-08-04 16:58:21.000000 ripplegw-0.0.3/src/ripple/noise.py
+drwxr-xr-x   0 thomasedwards   (501) staff       (20)        0 2023-08-04 17:00:41.375122 ripplegw-0.0.3/src/ripple/noise_resources/
+-rw-r--r--   0 thomasedwards   (501) staff       (20)    48230 2022-10-12 22:06:55.000000 ripplegw-0.0.3/src/ripple/noise_resources/O2_ASD.dat
+-rw-r--r--   0 thomasedwards   (501) staff       (20)  1117811 2022-10-12 22:06:55.000000 ripplegw-0.0.3/src/ripple/noise_resources/O3a_Livingston_ASD.dat
+-rw-r--r--   0 thomasedwards   (501) staff       (20)        0 2022-10-12 22:06:55.000000 ripplegw-0.0.3/src/ripple/noise_resources/__init__.py
+-rw-r--r--   0 thomasedwards   (501) staff       (20)    56415 2022-10-12 22:06:55.000000 ripplegw-0.0.3/src/ripple/noise_resources/aLIGO.dat
+-rw-r--r--   0 thomasedwards   (501) staff       (20)    10070 2022-10-12 22:06:55.000000 ripplegw-0.0.3/src/ripple/noise_resources/aLIGOZeroDetHighPower.dat
+-rw-r--r--   0 thomasedwards   (501) staff       (20)    87114 2022-10-12 22:06:55.000000 ripplegw-0.0.3/src/ripple/noise_resources/ce.dat
+-rw-r--r--   0 thomasedwards   (501) staff       (20)    87132 2022-10-12 22:06:55.000000 ripplegw-0.0.3/src/ripple/noise_resources/et.dat
+-rw-r--r--   0 thomasedwards   (501) staff       (20)      201 2022-10-12 22:06:55.000000 ripplegw-0.0.3/src/ripple/typing.py
+drwxr-xr-x   0 thomasedwards   (501) staff       (20)        0 2023-08-04 17:00:41.389047 ripplegw-0.0.3/src/ripple/waveforms/
+-rw-r--r--   0 thomasedwards   (501) staff       (20)    19453 2023-08-04 16:58:21.000000 ripplegw-0.0.3/src/ripple/waveforms/IMRPhenomD.py
+-rw-r--r--   0 thomasedwards   (501) staff       (20)    53661 2023-01-31 13:59:58.000000 ripplegw-0.0.3/src/ripple/waveforms/IMRPhenomD_QNMdata.py
+-rw-r--r--   0 thomasedwards   (501) staff       (20)    15783 2023-01-06 19:15:14.000000 ripplegw-0.0.3/src/ripple/waveforms/IMRPhenomD_utils.py
+-rw-r--r--   0 thomasedwards   (501) staff       (20)    45388 2023-08-04 16:58:21.000000 ripplegw-0.0.3/src/ripple/waveforms/IMRPhenomXAS.py
+-rw-r--r--   0 thomasedwards   (501) staff       (20)    39958 2023-04-20 15:01:50.000000 ripplegw-0.0.3/src/ripple/waveforms/IMRPhenomX_utils.py
+-rw-r--r--   0 thomasedwards   (501) staff       (20)        0 2022-10-12 22:06:55.000000 ripplegw-0.0.3/src/ripple/waveforms/__init__.py
+drwxr-xr-x   0 thomasedwards   (501) staff       (20)        0 2023-08-04 17:00:41.425217 ripplegw-0.0.3/src/ripplegw.egg-info/
+-rw-r--r--   0 thomasedwards   (501) staff       (20)     3126 2023-08-04 17:00:41.000000 ripplegw-0.0.3/src/ripplegw.egg-info/PKG-INFO
+-rw-r--r--   0 thomasedwards   (501) staff       (20)      833 2023-08-04 17:00:41.000000 ripplegw-0.0.3/src/ripplegw.egg-info/SOURCES.txt
+-rw-r--r--   0 thomasedwards   (501) staff       (20)        1 2023-08-04 17:00:41.000000 ripplegw-0.0.3/src/ripplegw.egg-info/dependency_links.txt
+-rw-r--r--   0 thomasedwards   (501) staff       (20)       17 2023-08-04 17:00:41.000000 ripplegw-0.0.3/src/ripplegw.egg-info/requires.txt
+-rw-r--r--   0 thomasedwards   (501) staff       (20)        7 2023-08-04 17:00:41.000000 ripplegw-0.0.3/src/ripplegw.egg-info/top_level.txt
```

### Comparing `ripplegw-0.0.2/LICENSE` & `ripplegw-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ripplegw-0.0.2/PKG-INFO` & `ripplegw-0.0.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: ripplegw
-Version: 0.0.2
+Version: 0.0.3
 Summary: A small jax package for differentiable and fast gravitational wave data analysis.
 Home-page: https://ripple.readthedocs.io/en/latest/
 Project-URL: Bug Tracker, https://github.com/tedwards2412/ripple
 Keywords: gravitational waves,jax
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Ripple :ocean:
 
 A small `jax` package for differentiable and fast gravitational wave data analysis.
 
@@ -24,14 +24,24 @@
 
 Ripple can be installed using 
 
 ```
 pip3 install ripplegw
 ```
 
+Note that by default we do not include enable float64 in jax since we want allow users to use float32 to improve performance.
+If you require float64, please include the following code at the start of the script:
+
+```
+from jax import config
+config.update("jax_enable_x64", True)
+```
+
+See https://jax.readthedocs.io/en/latest/notebooks/Common_Gotchas_in_JAX.html for other common `jax` gotchas.
+
 ### Supported waveforms
 
 - IMRPhenomXAS (aligned spin)
 - IMRPhenomD (aligned spin)
 
 ### Generating a waveform and its derivative
 
@@ -74,22 +84,22 @@
 f_l = 24
 f_u = 512
 del_f = 0.01
 fs = jnp.arange(f_l, f_u, del_f)
 f_ref = f_l
 
 # And finally lets generate the waveform!
-hp_ripple, hc_ripple = IMRPhenomXAS.gen_IMRPhenomXAS_polar(fs, theta_ripple, f_ref)
+hp_ripple, hc_ripple = IMRPhenomXAS.gen_IMRPhenomXAS_hphc(fs, theta_ripple, f_ref)
 
 # Note that we have not internally jitted the functions since this would
 # introduce an annoying overhead each time the user evaluated the function with a different length frequency array
 # We therefore recommend that the user jit the function themselves to accelerate evaluations. For example:
 
 import jax
 
 @jax.jit
 def waveform(theta):
-    return IMRPhenomXAS.gen_IMRPhenomXAS_polar(fs, theta)
+    return IMRPhenomXAS.gen_IMRPhenomXAS_hphc(fs, theta)
 ```
```

### Comparing `ripplegw-0.0.2/README.md` & `ripplegw-0.0.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -10,14 +10,24 @@
 
 Ripple can be installed using 
 
 ```
 pip3 install ripplegw
 ```
 
+Note that by default we do not include enable float64 in jax since we want allow users to use float32 to improve performance.
+If you require float64, please include the following code at the start of the script:
+
+```
+from jax import config
+config.update("jax_enable_x64", True)
+```
+
+See https://jax.readthedocs.io/en/latest/notebooks/Common_Gotchas_in_JAX.html for other common `jax` gotchas.
+
 ### Supported waveforms
 
 - IMRPhenomXAS (aligned spin)
 - IMRPhenomD (aligned spin)
 
 ### Generating a waveform and its derivative
 
@@ -60,22 +70,22 @@
 f_l = 24
 f_u = 512
 del_f = 0.01
 fs = jnp.arange(f_l, f_u, del_f)
 f_ref = f_l
 
 # And finally lets generate the waveform!
-hp_ripple, hc_ripple = IMRPhenomXAS.gen_IMRPhenomXAS_polar(fs, theta_ripple, f_ref)
+hp_ripple, hc_ripple = IMRPhenomXAS.gen_IMRPhenomXAS_hphc(fs, theta_ripple, f_ref)
 
 # Note that we have not internally jitted the functions since this would
 # introduce an annoying overhead each time the user evaluated the function with a different length frequency array
 # We therefore recommend that the user jit the function themselves to accelerate evaluations. For example:
 
 import jax
 
 @jax.jit
 def waveform(theta):
-    return IMRPhenomXAS.gen_IMRPhenomXAS_polar(fs, theta)
+    return IMRPhenomXAS.gen_IMRPhenomXAS_hphc(fs, theta)
 ```
```

### Comparing `ripplegw-0.0.2/setup.cfg` & `ripplegw-0.0.3/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ripplegw
-version = 0.0.2
+version = 0.0.3
 description = A small jax package for differentiable and fast gravitational wave data analysis.
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = gravitational waves, jax
 url = https://ripple.readthedocs.io/en/latest/
 project_urls = 
 	Bug Tracker = https://github.com/tedwards2412/ripple
@@ -13,15 +13,15 @@
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 
 [options]
 package_dir = 
 	= src
 packages = find:
-python_requires = >=3.10
+python_requires = >=3.9
 install_requires = 
 	jax
 	jaxlib
 	numpy
 
 [options.package_data]
 * = *.dat
```

### Comparing `ripplegw-0.0.2/src/ripple/__init__.py` & `ripplegw-0.0.3/src/ripple/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Core utilities for calculating properties of binaries, sampling their parameters
 and comparing waveforms.
 """
 
-from jax.config import config
-
-config.update("jax_enable_x64", True)
+# Note that we turned this off to test float32 capabilities
+# from jax.config import config
+# config.update("jax_enable_x64", True)
 
 from math import pi
 from typing import Callable, Optional, Tuple
 import warnings
 
 from jax import random
 import jax.numpy as jnp
@@ -27,15 +27,15 @@
 
     Returns:
         :math:`(m1, m2)`, with the chirp mass in the same units as
         the component masses
     """
     Mchirp, eta = m
     M = Mchirp / (eta ** (3 / 5))
-    m2 = (M - jnp.sqrt(M ** 2 - 4 * M ** 2 * eta)) / 2
+    m2 = (M - jnp.sqrt(M**2 - 4 * M**2 * eta)) / 2
     m1 = M - m2
     return m1, m2
 
 
 def ms_to_Mc_eta(m):
     r"""
     Converts binary component masses to chirp mass and symmetric mass ratio.
@@ -57,15 +57,15 @@
 
     Args:
         m: the black hole's mass in kg
 
     Returns:
         The ISCO frequency in Hz
     """
-    return 1 / (6 ** (3 / 2) * pi * m / (C ** 3 / G))
+    return 1 / (6 ** (3 / 2) * pi * m / (C**3 / G))
 
 
 def get_M_eta_sampler(
     M_range: Tuple[float, float], eta_range: Tuple[float, float]
 ) -> Callable[[PRNGKeyArray, int], Array]:
     """
     Uniformly values of the chirp mass and samples over the specified ranges.
```

### Comparing `ripplegw-0.0.2/src/ripple/noise.py` & `ripplegw-0.0.3/src/ripple/noise.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,13 @@
 """
 Detector noise power spectral densities.
 """
 
-try:
-    import importlib.resources as pkg_resources
-except ImportError:
-    # Try backported to PY<37 `importlib_resources`.
-    import importlib_resources as pkg_resources  # type: ignore
 
+import importlib.resources as pkg_resources
 from typing import Callable, Tuple
 
 import jax
 import jax.numpy as jnp
 import numpy as np
 
 from . import noise_resources
@@ -49,43 +45,17 @@
         normalization
         * 9
         * ((4.49 * x) ** (-56) + 0.16 * x ** (-4.52) + 0.52 + 0.32 * x**2),
         jnp.inf,
     )
 
 
-f_range_LISA = (2e-5, 1.0)  # Hz, from LISA Science Requirements fig. 1
-r"""
-LISA frequency band [Hz].
-
-References:
-    LISA Science Requirements, fig. 1 (`<https://www.cosmos.esa.int/documents/678316/1700384/SciRD.pdf>`_)
-"""
-
-
-def Sn_LISA(f):
-    r"""
-    LISA noise PSD, averaged over sky position and polarization angle.
-
-    Reference:
-        Travis Robson et al 2019 Class. Quantum Grav. 36 105011
-        `<https://arxiv.org/abs/1803.01944>`_`
-    """
-    return jnp.where(
-        jnp.logical_and(f >= f_range_LISA[0], f <= f_range_LISA[1]),
-        1
-        / f**14
-        * 1.80654e-17
-        * (0.000606151 + f**2)
-        * (3.6864e-76 + 3.6e-37 * f**8 + 2.25e-30 * f**10 + 8.66941e-21 * f**14),
-        jnp.inf,
-    )
-
-
-def _load_noise(name: str, asd: bool = False) -> Tuple[Callable[[Array], Array], Tuple[float, float]]:
+def _load_noise(
+    name: str, asd: bool = False
+) -> Tuple[Callable[[Array], Array], Tuple[float, float]]:
     r"""
     Loads noise PSD from text data file into an interpolator. The file's
     columns must contain the frequencies and corresponding noise power spectral
     density or amplitude spectral density values.
 
     Args:
         name: name of data file in ``noise_resources`` without the `.dat`
@@ -105,15 +75,18 @@
 
     Sns[Sns == 0.0] = np.inf
 
     fs = jnp.array(fs)
     Sns = jnp.array(Sns)
     f_range = (fs[0], fs[-1])
 
-    return jax.jit(lambda f: jnp.interp(f, fs, Sns, left=jnp.inf, right=jnp.inf)), f_range
+    return (
+        jax.jit(lambda f: jnp.interp(f, fs, Sns, left=jnp.inf, right=jnp.inf)),
+        f_range,
+    )
 
 
 Sn_aLIGO, f_range_aLIGO = _load_noise("aLIGO", asd=True)
 r"""The advanced LIGO noise PSD and frequency range.
 
 References:
     `<https://dcc.ligo.org/LIGO-T1800044/public>`_
@@ -130,15 +103,17 @@
 r"""The Einstein Telescope noise PSD and frequency range.
 
 References:
     `<http://www.et-gw.eu/index.php/etsensitivities>`_
 """
 
 
-Sn_aLIGOZeroDetHighPower, f_range_aLIGOZeroDetHighPower = _load_noise("aLIGOZeroDetHighPower")
+Sn_aLIGOZeroDetHighPower, f_range_aLIGOZeroDetHighPower = _load_noise(
+    "aLIGOZeroDetHighPower"
+)
 r"""The aLIGOZeroDetHighPower noise PSD from pycbc and frequency range.
 
 References:
     ???
 
 Args:
     f: frequency
```

### Comparing `ripplegw-0.0.2/src/ripple/noise_resources/O2_ASD.dat` & `ripplegw-0.0.3/src/ripple/noise_resources/O2_ASD.dat`

 * *Files identical despite different names*

### Comparing `ripplegw-0.0.2/src/ripple/noise_resources/O3a_Livingston_ASD.dat` & `ripplegw-0.0.3/src/ripple/noise_resources/O3a_Livingston_ASD.dat`

 * *Files identical despite different names*

### Comparing `ripplegw-0.0.2/src/ripple/noise_resources/aLIGO.dat` & `ripplegw-0.0.3/src/ripple/noise_resources/aLIGO.dat`

 * *Files identical despite different names*

### Comparing `ripplegw-0.0.2/src/ripple/noise_resources/aLIGOZeroDetHighPower.dat` & `ripplegw-0.0.3/src/ripple/noise_resources/aLIGOZeroDetHighPower.dat`

 * *Files identical despite different names*

### Comparing `ripplegw-0.0.2/src/ripple/noise_resources/ce.dat` & `ripplegw-0.0.3/src/ripple/noise_resources/ce.dat`

 * *Files identical despite different names*

### Comparing `ripplegw-0.0.2/src/ripple/noise_resources/et.dat` & `ripplegw-0.0.3/src/ripple/noise_resources/et.dat`

 * *Files identical despite different names*

### Comparing `ripplegw-0.0.2/src/ripple/waveforms/IMRPhenomD.py` & `ripplegw-0.0.3/src/ripple/waveforms/IMRPhenomD.py`

 * *Files 0% similar despite different names*

```diff
@@ -549,15 +549,14 @@
 
     A = Amp(f, theta_intrinsic, coeffs, transition_freqs, D=theta_extrinsic[0])
 
     h0 = A * jnp.exp(1j * -Psi)
     return h0
 
 
-# @jax.jit
 def gen_IMRPhenomD(f: Array, params: Array, f_ref: float):
     """
     Generate PhenomD frequency domain waveform following 1508.07253.
     vars array contains both intrinsic and extrinsic variables
     theta = [Mchirp, eta, chi1, chi2, D, tc, phic]
     Mchirp: Chirp mass of the system [solar masses]
     eta: Symmetric mass ratio [between 0.0 and 0.25]
@@ -579,16 +578,15 @@
     theta_extrinsic = jnp.array([params[4], params[5], params[6]])
 
     coeffs = get_coeffs(theta_intrinsic)
     h0 = _gen_IMRPhenomD(f, theta_intrinsic, theta_extrinsic, coeffs, f_ref)
     return h0
 
 
-# @jax.jit
-def gen_IMRPhenomD_polar(f: Array, params: Array, f_ref: float):
+def gen_IMRPhenomD_hphc(f: Array, params: Array, f_ref: float):
     """
     Generate PhenomD frequency domain waveform following 1508.07253.
     vars array contains both intrinsic and extrinsic variables
     theta = [Mchirp, eta, chi1, chi2, D, tc, phic]
     Mchirp: Chirp mass of the system [solar masses]
     eta: Symmetric mass ratio [between 0.0 and 0.25]
     chi1: Dimensionless aligned spin of the primary object [between -1 and 1]
```

### Comparing `ripplegw-0.0.2/src/ripple/waveforms/IMRPhenomD_QNMdata.py` & `ripplegw-0.0.3/src/ripple/waveforms/IMRPhenomD_QNMdata.py`

 * *Files identical despite different names*

### Comparing `ripplegw-0.0.2/src/ripple/waveforms/IMRPhenomD_utils.py` & `ripplegw-0.0.3/src/ripple/waveforms/IMRPhenomD_utils.py`

 * *Files identical despite different names*

### Comparing `ripplegw-0.0.2/src/ripple/waveforms/IMRPhenomXAS.py` & `ripplegw-0.0.3/src/ripple/waveforms/IMRPhenomXAS.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,129 +68,137 @@
             )
         )
         / 16.0
     ) * PI ** (
         4.0 / 3.0
     )
     phi5 = 0.0
-    phi5L = ((5 * (46374 - 6552 * eta) * PI) / 4536.0) * PI ** (5.0 / 3.0) + (
+    phi5L = ((5.0 * (46374.0 - 6552.0 * eta) * PI) / 4536.0) * PI ** (5.0 / 3.0) + (
         (
-            -732985 * (chi1 + chi2 + chi1 * delta - chi2 * delta)
-            - 560 * (-1213 * (chi1 + chi2) + 63 * (chi1 - chi2) * delta) * eta
-            + 85680 * (chi1 + chi2) * eta2
+            -732985.0 * (chi1 + chi2 + chi1 * delta - chi2 * delta)
+            - 560.0 * (-1213.0 * (chi1 + chi2) + 63.0 * (chi1 - chi2) * delta) * eta
+            + 85680.0 * (chi1 + chi2) * eta2
         )
         / 4536.0
     ) * PI ** (5.0 / 3.0)
-    phi6L = (-6848 / 63.0) * PI**2.0
+    phi6L = (-6848.0 / 63.0) * PI**2.0
     phi6 = (
         (
-            11583231236531 / 4.69421568e9
-            - (5 * eta * (3147553127 + 588 * eta * (-45633 + 102260 * eta)))
+            11583231236531.0 / 4.69421568e9
+            - (5.0 * eta * (3147553127.0 + 588.0 * eta * (-45633.0 + 102260.0 * eta)))
             / 3.048192e6
-            - (6848 * EulerGamma) / 21.0
-            - (640 * PI**2.0) / 3.0
-            + (2255 * eta * PI**2.0) / 12.0
-            - (13696 * jnp.log(2)) / 21.0
-            - (6848 * jnp.log(PI)) / 63.0
+            - (6848.0 * EulerGamma) / 21.0
+            - (640.0 * PI**2.0) / 3.0
+            + (2255.0 * eta * PI**2.0) / 12.0
+            - (13696.0 * jnp.log(2.0)) / 21.0
+            - (6848.0 * jnp.log(PI)) / 63.0
         )
         * PI**2.0
         + (
             (
                 5
                 * (
-                    227 * (chi1 + chi2 + chi1 * delta - chi2 * delta)
-                    - 156 * (chi1 + chi2) * eta
+                    227.0 * (chi1 + chi2 + chi1 * delta - chi2 * delta)
+                    - 156.0 * (chi1 + chi2) * eta
                 )
                 * PI
             )
             / 3.0
         )
         * PI**2.0
         + (
             (
-                5
+                5.0
                 * (
-                    20 * chi1L2L * eta * (11763 + 12488 * eta)
-                    + 7
+                    20.0 * chi1L2L * eta * (11763.0 + 12488.0 * eta)
+                    + 7.0
                     * chi2L2
                     * (
-                        -15103 * (-1 + delta)
-                        + 2 * (-21683 + 6580 * delta) * eta
-                        - 9808 * eta2
+                        -15103.0 * (-1 + delta)
+                        + 2.0 * (-21683.0 + 6580.0 * delta) * eta
+                        - 9808.0 * eta2
                     )
-                    - 7
+                    - 7.0
                     * chi1L2
                     * (
-                        -15103 * (1 + delta)
-                        + 2 * (21683 + 6580 * delta) * eta
-                        + 9808 * eta2
+                        -15103.0 * (1 + delta)
+                        + 2.0 * (21683.0 + 6580.0 * delta) * eta
+                        + 9808.0 * eta2
                     )
                 )
             )
             / 4032.0
         )
         * PI**2.0
     )
     phi7 = (
-        ((5 * (15419335 + 168 * (75703 - 29618 * eta) * eta) * PI) / 254016.0)
+        ((5.0 * (15419335.0 + 168.0 * (75703.0 - 29618.0 * eta) * eta) * PI) / 254016.0)
         * PI ** (7.0 / 3.0)
         + (
             (
-                5
+                5.0
                 * (
-                    -5030016755 * (chi1 + chi2 + chi1 * delta - chi2 * delta)
-                    + 4
-                    * (2113331119 * (chi1 + chi2) + 675484362 * (chi1 - chi2) * delta)
+                    -5030016755.0 * (chi1 + chi2 + chi1 * delta - chi2 * delta)
+                    + 4.0
+                    * (
+                        2113331119.0 * (chi1 + chi2)
+                        + 675484362.0 * (chi1 - chi2) * delta
+                    )
                     * eta
-                    - 1008
-                    * (208433 * (chi1 + chi2) + 25011 * (chi1 - chi2) * delta)
+                    - 1008.0
+                    * (208433.0 * (chi1 + chi2) + 25011.0 * (chi1 - chi2) * delta)
                     * eta2
-                    + 90514368 * (chi1 + chi2) * eta3
+                    + 90514368.0 * (chi1 + chi2) * eta3
                 )
             )
             / 6.096384e6
         )
         * PI ** (7.0 / 3.0)
         + (
-            -5
+            -5.0
             * (
-                57 * chi1L2 * (1 + delta - 2 * eta)
-                + 220 * chi1L2L * eta
-                - 57 * chi2L2 * (-1 + delta + 2 * eta)
+                57.0 * chi1L2 * (1 + delta - 2 * eta)
+                + 220.0 * chi1L2L * eta
+                - 57.0 * chi2L2 * (-1 + delta + 2 * eta)
             )
             * PI
         )
         * PI ** (7.0 / 3.0)
         + (
             (
-                14585 * (-(chi2L3 * (-1 + delta)) + chi1L3 * (1 + delta))
-                - 5
+                14585.0 * (-(chi2L3 * (-1 + delta)) + chi1L3 * (1 + delta))
+                - 5.0
                 * (
-                    chi2L3 * (8819 - 2985 * delta)
-                    + 8439 * chi1 * chi2L2 * (-1 + delta)
-                    - 8439 * chi1L2 * chi2 * (1 + delta)
-                    + chi1L3 * (8819 + 2985 * delta)
+                    chi2L3 * (8819.0 - 2985.0 * delta)
+                    + 8439.0 * chi1 * chi2L2 * (-1.0 + delta)
+                    - 8439.0 * chi1L2 * chi2 * (1.0 + delta)
+                    + chi1L3 * (8819.0 + 2985.0 * delta)
                 )
                 * eta
-                + 40 * (chi1 + chi2) * (17 * chi1L2 - 14 * chi1L2L + 17 * chi2L2) * eta2
+                + 40.0
+                * (chi1 + chi2)
+                * (17.0 * chi1L2 - 14.0 * chi1L2L + 17.0 * chi2L2)
+                * eta2
             )
             / 48.0
         )
         * PI ** (7.0 / 3.0)
     )
     phi8 = (
         (
-            -5
+            -5.0
             * (
-                1263141 * (chi1 + chi2 + chi1 * delta - chi2 * delta)
-                - 2 * (794075 * (chi1 + chi2) + 178533 * (chi1 - chi2) * delta) * eta
-                + 94344 * (chi1 + chi2) * eta2
+                1263141.0 * (chi1 + chi2 + chi1 * delta - chi2 * delta)
+                - 2.0
+                * (794075.0 * (chi1 + chi2) + 178533.0 * (chi1 - chi2) * delta)
+                * eta
+                + 94344.0 * (chi1 + chi2) * eta2
             )
             * PI
-            * (-1 + jnp.log(PI))
+            * (-1.0 + jnp.log(PI))
         )
         / 9072.0
     ) * PI ** (8.0 / 3.0)
     phi8L = (
         (
             -5.0
             * (
@@ -813,84 +821,95 @@
 
     _, _, fMs_MECO, fMs_ISCO = IMRPhenomX_utils.get_cutoff_fMs(m1, m2, chi1, chi2)
     fMs_AmpInsMax = fMs_MECO + 0.25 * (fMs_ISCO - fMs_MECO)
     fMs_AmpMatchIN = fMs_AmpInsMax
 
     A0 = 1.0
     # A1 = 0.0
-    A2 = ((-969 + 1804 * eta) / 672.0) * (PI ** (2.0 / 3.0))
+    A2 = ((-969.0 + 1804.0 * eta) / 672.0) * (PI ** (2.0 / 3.0))
     A3 = (
         (
-            81 * (chi1 + chi2)
-            + 81 * chi1 * delta
-            - 81 * chi2 * delta
-            - 44 * (chi1 + chi2) * eta
+            81.0 * (chi1 + chi2)
+            + 81.0 * chi1 * delta
+            - 81.0 * chi2 * delta
+            - 44.0 * (chi1 + chi2) * eta
         )
         / 48.0
     ) * PI
     A4 = (
         (
-            -27312085
-            - 10287648 * chi1**2 * (1 + delta)
-            + 24
+            -27312085.0
+            - 10287648.0 * chi1**2.0 * (1.0 + delta)
+            + 24.0
             * (
-                428652 * chi2**2 * (-1 + delta)
+                428652.0 * chi2**2 * (-1 + delta)
                 + (
-                    -1975055
-                    + 10584 * (81 * chi1**2 - 94 * chi1 * chi2 + 81 * chi2**2)
+                    -1975055.0
+                    + 10584.0
+                    * (81.0 * chi1**2.0 - 94.0 * chi1 * chi2 + 81.0 * chi2**2)
                 )
                 * eta
-                + 1473794 * eta2
+                + 1473794.0 * eta2
             )
         )
         / 8.128512e6
     ) * (PI ** (4.0 / 3.0))
     A5 = (
         (
-            -6048 * chi1**2 * chi1 * (-1 - delta + (3 + delta) * eta)
+            -6048.0 * chi1**2.0 * chi1 * (-1.0 - delta + (3.0 + delta) * eta)
             + chi2
             * (
-                -((287213 + 6048 * chi2**2) * (-1 + delta))
-                + 4 * (-93414 + 1512 * chi2**2 * (-3 + delta) + 2083 * delta) * eta
-                - 35632 * eta2
+                -((287213.0 + 6048.0 * chi2**2) * (-1.0 + delta))
+                + 4
+                * (-93414.0 + 1512.0 * chi2**2.0 * (-3.0 + delta) + 2083.0 * delta)
+                * eta
+                - 35632.0 * eta2
             )
             + chi1
-            * (287213 * (1 + delta) - 4 * eta * (93414 + 2083 * delta + 8908 * eta))
-            + 42840 * (-1 + 4 * eta) * PI
+            * (
+                287213.0 * (1.0 + delta)
+                - 4.0 * eta * (93414.0 + 2083.0 * delta + 8908.0 * eta)
+            )
+            + 42840.0 * (-1.0 + 4.0 * eta) * PI
         )
         / 32256.0
     ) * (PI ** (5.0 / 3.0))
     A6 = (
         (
-            -1242641879927
+            -1242641879927.0
             + 12.0
             * (
                 28.0
                 * (
                     -3248849057.0
-                    + 11088
-                    * (163199 * chi1**2 - 266498 * chi1 * chi2 + 163199 * chi2**2)
+                    + 11088.0
+                    * (
+                        163199.0 * chi1**2.0
+                        - 266498.0 * chi1 * chi2
+                        + 163199.0 * chi2**2.0
+                    )
                 )
                 * eta2
-                + 27026893936 * eta2 * eta
-                - 116424
+                + 27026893936.0 * eta2 * eta
+                - 116424.0
                 * (
-                    147117 * (-(chi2**2 * (-1.0 + delta)) + chi1**2 * (1.0 + delta))
-                    + 60928 * (chi1 + chi2 + chi1 * delta - chi2 * delta) * PI
+                    147117.0
+                    * (-(chi2**2.0 * (-1.0 + delta)) + chi1**2.0 * (1.0 + delta))
+                    + 60928.0 * (chi1 + chi2 + chi1 * delta - chi2 * delta) * PI
                 )
                 + eta
                 * (
                     545384828789.0
-                    - 77616
+                    - 77616.0
                     * (
-                        638642 * chi1 * chi2
-                        + chi1**2 * (-158633 + 282718 * delta)
-                        - chi2**2 * (158633.0 + 282718.0 * delta)
+                        638642.0 * chi1 * chi2
+                        + chi1**2.0 * (-158633.0 + 282718.0 * delta)
+                        - chi2**2.0 * (158633.0 + 282718.0 * delta)
                         - 107520.0 * (chi1 + chi2) * PI
-                        + 275520 * PI**2
+                        + 275520.0 * PI**2
                     )
                 )
             )
         )
         / 6.0085960704e10
     ) * PI**2
 
@@ -1342,15 +1361,14 @@
     Psi = Psi + (linb * fM_s) + lina + phifRef - 2 * PI + ext_phase_contrib
 
     A = Amp(f, theta_intrinsic, amp_coeffs, D=theta_extrinsic[0])
     h0 = A * jnp.exp(1j * Psi)
     return h0
 
 
-# @jax.jit
 def gen_IMRPhenomXAS(f: Array, params: Array, f_ref: float):
     """
     Generate PhenomXAS frequency domain waveform following 2001.11412.
     Note that this waveform also assumes that object one is the more massive.
     vars array contains both intrinsic and extrinsic variables
     theta = [Mchirp, eta, chi1, chi2, D, tc, phic]
     Mchirp: Chirp mass of the system [solar masses]
@@ -1374,16 +1392,15 @@
 
     h0 = _gen_IMRPhenomXAS(
         f, theta_intrinsic, theta_extrinsic, phase_coeffs, amp_coeffs, f_ref
     )
     return h0
 
 
-# @jax.jit
-def gen_IMRPhenomXAS_polar(f: Array, params: Array, f_ref: float):
+def gen_IMRPhenomXAS_hphc(f: Array, params: Array, f_ref: float):
     """
     Generate PhenomXAS frequency domain waveform following 2001.11412.
     vars array contains both intrinsic and extrinsic variables
     theta = [Mchirp, eta, chi1, chi2, D, tc, phic]
     Mchirp: Chirp mass of the system [solar masses]
     eta: Symmetric mass ratio [between 0.0 and 0.25]
     chi1: Dimensionless aligned spin of the primary object [between -1 and 1]
```

### Comparing `ripplegw-0.0.2/src/ripple/waveforms/IMRPhenomX_utils.py` & `ripplegw-0.0.3/src/ripple/waveforms/IMRPhenomX_utils.py`

 * *Files identical despite different names*

### Comparing `ripplegw-0.0.2/src/ripplegw.egg-info/PKG-INFO` & `ripplegw-0.0.3/src/ripplegw.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: ripplegw
-Version: 0.0.2
+Version: 0.0.3
 Summary: A small jax package for differentiable and fast gravitational wave data analysis.
 Home-page: https://ripple.readthedocs.io/en/latest/
 Project-URL: Bug Tracker, https://github.com/tedwards2412/ripple
 Keywords: gravitational waves,jax
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Ripple :ocean:
 
 A small `jax` package for differentiable and fast gravitational wave data analysis.
 
@@ -24,14 +24,24 @@
 
 Ripple can be installed using 
 
 ```
 pip3 install ripplegw
 ```
 
+Note that by default we do not include enable float64 in jax since we want allow users to use float32 to improve performance.
+If you require float64, please include the following code at the start of the script:
+
+```
+from jax import config
+config.update("jax_enable_x64", True)
+```
+
+See https://jax.readthedocs.io/en/latest/notebooks/Common_Gotchas_in_JAX.html for other common `jax` gotchas.
+
 ### Supported waveforms
 
 - IMRPhenomXAS (aligned spin)
 - IMRPhenomD (aligned spin)
 
 ### Generating a waveform and its derivative
 
@@ -74,22 +84,22 @@
 f_l = 24
 f_u = 512
 del_f = 0.01
 fs = jnp.arange(f_l, f_u, del_f)
 f_ref = f_l
 
 # And finally lets generate the waveform!
-hp_ripple, hc_ripple = IMRPhenomXAS.gen_IMRPhenomXAS_polar(fs, theta_ripple, f_ref)
+hp_ripple, hc_ripple = IMRPhenomXAS.gen_IMRPhenomXAS_hphc(fs, theta_ripple, f_ref)
 
 # Note that we have not internally jitted the functions since this would
 # introduce an annoying overhead each time the user evaluated the function with a different length frequency array
 # We therefore recommend that the user jit the function themselves to accelerate evaluations. For example:
 
 import jax
 
 @jax.jit
 def waveform(theta):
-    return IMRPhenomXAS.gen_IMRPhenomXAS_polar(fs, theta)
+    return IMRPhenomXAS.gen_IMRPhenomXAS_hphc(fs, theta)
 ```
```

### Comparing `ripplegw-0.0.2/src/ripplegw.egg-info/SOURCES.txt` & `ripplegw-0.0.3/src/ripplegw.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -20,10 +20,8 @@
 src/ripple/waveforms/IMRPhenomXAS.py
 src/ripple/waveforms/IMRPhenomX_utils.py
 src/ripple/waveforms/__init__.py
 src/ripplegw.egg-info/PKG-INFO
 src/ripplegw.egg-info/SOURCES.txt
 src/ripplegw.egg-info/dependency_links.txt
 src/ripplegw.egg-info/requires.txt
-src/ripplegw.egg-info/top_level.txt
-test/test_IMRPhenomX.py
-test/test_imrphenomd.py
+src/ripplegw.egg-info/top_level.txt
```

