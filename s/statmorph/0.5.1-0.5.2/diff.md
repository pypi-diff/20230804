# Comparing `tmp/statmorph-0.5.1.tar.gz` & `tmp/statmorph-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "statmorph-0.5.1.tar", last modified: Tue Jul  4 07:14:14 2023, max compression
+gzip compressed data, was "statmorph-0.5.2.tar", last modified: Fri Aug  4 03:24:09 2023, max compression
```

## Comparing `statmorph-0.5.1.tar` & `statmorph-0.5.2.tar`

### file list

```diff
@@ -1,42 +1,44 @@
-drwxr-xr-x   0 vrg       (1000) users      (985)        0 2023-07-04 07:14:14.543779 statmorph-0.5.1/
--rw-r--r--   0 vrg       (1000) users      (985)     1528 2023-01-02 20:02:18.000000 statmorph-0.5.1/LICENSE
--rw-r--r--   0 vrg       (1000) users      (985)      176 2022-10-15 05:52:48.000000 statmorph-0.5.1/MANIFEST.in
--rw-r--r--   0 vrg       (1000) users      (985)     2263 2023-07-04 07:14:14.543779 statmorph-0.5.1/PKG-INFO
--rw-r--r--   0 vrg       (1000) users      (985)     1585 2022-10-15 05:52:47.000000 statmorph-0.5.1/README.rst
-drwxr-xr-x   0 vrg       (1000) users      (985)        0 2023-07-04 07:14:14.540446 statmorph-0.5.1/docs/
--rw-r--r--   0 vrg       (1000) users      (985)      609 2022-10-15 05:52:47.000000 statmorph-0.5.1/docs/Makefile
-drwxr-xr-x   0 vrg       (1000) users      (985)        0 2023-07-04 07:14:14.540446 statmorph-0.5.1/docs/_static/
--rw-r--r--   0 vrg       (1000) users      (985)    15518 2022-10-15 05:52:47.000000 statmorph-0.5.1/docs/_static/banner.svg
--rw-r--r--   0 vrg       (1000) users      (985)     2238 2022-10-15 05:52:47.000000 statmorph-0.5.1/docs/_static/favicon.ico
--rw-r--r--   0 vrg       (1000) users      (985)    31694 2022-10-15 05:52:47.000000 statmorph-0.5.1/docs/_static/logo.png
--rw-r--r--   0 vrg       (1000) users      (985)      132 2022-10-15 05:52:47.000000 statmorph-0.5.1/docs/api.rst
--rw-r--r--   0 vrg       (1000) users      (985)     2613 2023-07-04 06:46:23.000000 statmorph-0.5.1/docs/conf.py
--rw-r--r--   0 vrg       (1000) users      (985)     4210 2023-01-06 20:26:43.000000 statmorph-0.5.1/docs/description.rst
--rw-r--r--   0 vrg       (1000) users      (985)     1412 2023-01-06 19:48:09.000000 statmorph-0.5.1/docs/index.rst
--rw-r--r--   0 vrg       (1000) users      (985)      780 2022-10-15 05:52:47.000000 statmorph-0.5.1/docs/installation.rst
-drwxr-xr-x   0 vrg       (1000) users      (985)        0 2023-07-04 07:14:14.540446 statmorph-0.5.1/docs/notebooks/
--rw-r--r--   0 vrg       (1000) users      (985)    13954 2023-01-06 19:31:51.000000 statmorph-0.5.1/docs/notebooks/tutorial.ipynb
--rw-r--r--   0 vrg       (1000) users      (985)     1884 2022-10-15 05:52:47.000000 statmorph-0.5.1/docs/overview.rst
--rw-r--r--   0 vrg       (1000) users      (985)       30 2022-10-15 05:52:47.000000 statmorph-0.5.1/docs/requirements.txt
--rw-r--r--   0 vrg       (1000) users      (985)       73 2022-10-15 05:52:48.000000 statmorph-0.5.1/requirements.txt
--rw-r--r--   0 vrg       (1000) users      (985)       38 2023-07-04 07:14:14.543779 statmorph-0.5.1/setup.cfg
--rw-r--r--   0 vrg       (1000) users      (985)     1363 2023-07-04 06:44:51.000000 statmorph-0.5.1/setup.py
-drwxr-xr-x   0 vrg       (1000) users      (985)        0 2023-07-04 07:14:14.540446 statmorph-0.5.1/statmorph/
--rw-r--r--   0 vrg       (1000) users      (985)       25 2022-10-15 05:52:47.000000 statmorph-0.5.1/statmorph/__init__.py
--rw-r--r--   0 vrg       (1000) users      (985)    97512 2023-07-04 06:45:09.000000 statmorph-0.5.1/statmorph/statmorph.py
-drwxr-xr-x   0 vrg       (1000) users      (985)        0 2023-07-04 07:14:14.543779 statmorph-0.5.1/statmorph/tests/
--rw-r--r--   0 vrg       (1000) users      (985)       30 2022-10-15 05:52:47.000000 statmorph-0.5.1/statmorph/tests/__init__.py
-drwxr-xr-x   0 vrg       (1000) users      (985)        0 2023-07-04 07:14:14.543779 statmorph-0.5.1/statmorph/tests/data/
--rw-r--r--   0 vrg       (1000) users      (985)   276480 2022-10-15 05:52:47.000000 statmorph-0.5.1/statmorph/tests/data/slice.fits
--rw-r--r--   0 vrg       (1000) users      (985)    13959 2023-07-04 02:09:35.000000 statmorph-0.5.1/statmorph/tests/test_statmorph.py
-drwxr-xr-x   0 vrg       (1000) users      (985)        0 2023-07-04 07:14:14.543779 statmorph-0.5.1/statmorph/utils/
--rw-r--r--   0 vrg       (1000) users      (985)       33 2022-10-15 05:52:47.000000 statmorph-0.5.1/statmorph/utils/__init__.py
--rwxr-xr-x   0 vrg       (1000) users      (985)    14333 2023-01-06 20:37:18.000000 statmorph-0.5.1/statmorph/utils/image_diagnostics.py
-drwxr-xr-x   0 vrg       (1000) users      (985)        0 2023-07-04 07:14:14.543779 statmorph-0.5.1/statmorph/utils/tests/
--rw-r--r--   0 vrg       (1000) users      (985)     1170 2022-10-15 05:52:47.000000 statmorph-0.5.1/statmorph/utils/tests/test_image_diagnostics.py
-drwxr-xr-x   0 vrg       (1000) users      (985)        0 2023-07-04 07:14:14.543779 statmorph-0.5.1/statmorph.egg-info/
--rw-r--r--   0 vrg       (1000) users      (985)     2263 2023-07-04 07:14:14.000000 statmorph-0.5.1/statmorph.egg-info/PKG-INFO
--rw-r--r--   0 vrg       (1000) users      (985)      711 2023-07-04 07:14:14.000000 statmorph-0.5.1/statmorph.egg-info/SOURCES.txt
--rw-r--r--   0 vrg       (1000) users      (985)        1 2023-07-04 07:14:14.000000 statmorph-0.5.1/statmorph.egg-info/dependency_links.txt
--rw-r--r--   0 vrg       (1000) users      (985)      103 2023-07-04 07:14:14.000000 statmorph-0.5.1/statmorph.egg-info/requires.txt
--rw-r--r--   0 vrg       (1000) users      (985)       10 2023-07-04 07:14:14.000000 statmorph-0.5.1/statmorph.egg-info/top_level.txt
+drwxr-xr-x   0 vrg       (1000) users      (985)        0 2023-08-04 03:24:09.159616 statmorph-0.5.2/
+-rw-r--r--   0 vrg       (1000) users      (985)     1528 2023-01-02 20:02:18.000000 statmorph-0.5.2/LICENSE
+-rw-r--r--   0 vrg       (1000) users      (985)      176 2022-10-15 05:52:48.000000 statmorph-0.5.2/MANIFEST.in
+-rw-r--r--   0 vrg       (1000) users      (985)     2263 2023-08-04 03:24:09.159616 statmorph-0.5.2/PKG-INFO
+-rw-r--r--   0 vrg       (1000) users      (985)     1585 2022-10-15 05:52:47.000000 statmorph-0.5.2/README.rst
+drwxr-xr-x   0 vrg       (1000) users      (985)        0 2023-08-04 03:24:09.156282 statmorph-0.5.2/docs/
+-rw-r--r--   0 vrg       (1000) users      (985)      609 2022-10-15 05:52:47.000000 statmorph-0.5.2/docs/Makefile
+drwxr-xr-x   0 vrg       (1000) users      (985)        0 2023-08-04 03:24:09.156282 statmorph-0.5.2/docs/_static/
+-rw-r--r--   0 vrg       (1000) users      (985)    15518 2022-10-15 05:52:47.000000 statmorph-0.5.2/docs/_static/banner.svg
+-rw-r--r--   0 vrg       (1000) users      (985)     2238 2022-10-15 05:52:47.000000 statmorph-0.5.2/docs/_static/favicon.ico
+-rw-r--r--   0 vrg       (1000) users      (985)    31694 2022-10-15 05:52:47.000000 statmorph-0.5.2/docs/_static/logo.png
+-rw-r--r--   0 vrg       (1000) users      (985)      132 2022-10-15 05:52:47.000000 statmorph-0.5.2/docs/api.rst
+-rw-r--r--   0 vrg       (1000) users      (985)     2613 2023-08-04 02:55:14.000000 statmorph-0.5.2/docs/conf.py
+-rw-r--r--   0 vrg       (1000) users      (985)     5009 2023-08-03 22:44:15.000000 statmorph-0.5.2/docs/description.rst
+-rw-r--r--   0 vrg       (1000) users      (985)       88 2023-08-01 00:03:20.000000 statmorph-0.5.2/docs/examples.rst
+-rw-r--r--   0 vrg       (1000) users      (985)     1424 2023-08-01 00:01:24.000000 statmorph-0.5.2/docs/index.rst
+-rw-r--r--   0 vrg       (1000) users      (985)      780 2022-10-15 05:52:47.000000 statmorph-0.5.2/docs/installation.rst
+drwxr-xr-x   0 vrg       (1000) users      (985)        0 2023-08-04 03:24:09.156282 statmorph-0.5.2/docs/notebooks/
+-rw-r--r--   0 vrg       (1000) users      (985)    16239 2023-08-04 02:51:15.000000 statmorph-0.5.2/docs/notebooks/doublesersic.ipynb
+-rw-r--r--   0 vrg       (1000) users      (985)    13558 2023-08-03 22:47:05.000000 statmorph-0.5.2/docs/notebooks/tutorial.ipynb
+-rw-r--r--   0 vrg       (1000) users      (985)     1904 2023-07-31 22:59:58.000000 statmorph-0.5.2/docs/overview.rst
+-rw-r--r--   0 vrg       (1000) users      (985)       30 2022-10-15 05:52:47.000000 statmorph-0.5.2/docs/requirements.txt
+-rw-r--r--   0 vrg       (1000) users      (985)       73 2022-10-15 05:52:48.000000 statmorph-0.5.2/requirements.txt
+-rw-r--r--   0 vrg       (1000) users      (985)       38 2023-08-04 03:24:09.159616 statmorph-0.5.2/setup.cfg
+-rw-r--r--   0 vrg       (1000) users      (985)     1363 2023-08-04 02:53:42.000000 statmorph-0.5.2/setup.py
+drwxr-xr-x   0 vrg       (1000) users      (985)        0 2023-08-04 03:24:09.156282 statmorph-0.5.2/statmorph/
+-rw-r--r--   0 vrg       (1000) users      (985)       25 2022-10-15 05:52:47.000000 statmorph-0.5.2/statmorph/__init__.py
+-rw-r--r--   0 vrg       (1000) users      (985)   113849 2023-08-04 02:53:56.000000 statmorph-0.5.2/statmorph/statmorph.py
+drwxr-xr-x   0 vrg       (1000) users      (985)        0 2023-08-04 03:24:09.159616 statmorph-0.5.2/statmorph/tests/
+-rw-r--r--   0 vrg       (1000) users      (985)       30 2022-10-15 05:52:47.000000 statmorph-0.5.2/statmorph/tests/__init__.py
+drwxr-xr-x   0 vrg       (1000) users      (985)        0 2023-08-04 03:24:09.159616 statmorph-0.5.2/statmorph/tests/data/
+-rw-r--r--   0 vrg       (1000) users      (985)   276480 2022-10-15 05:52:47.000000 statmorph-0.5.2/statmorph/tests/data/slice.fits
+-rw-r--r--   0 vrg       (1000) users      (985)    14790 2023-08-03 22:53:49.000000 statmorph-0.5.2/statmorph/tests/test_statmorph.py
+drwxr-xr-x   0 vrg       (1000) users      (985)        0 2023-08-04 03:24:09.159616 statmorph-0.5.2/statmorph/utils/
+-rw-r--r--   0 vrg       (1000) users      (985)       33 2022-10-15 05:52:47.000000 statmorph-0.5.2/statmorph/utils/__init__.py
+-rwxr-xr-x   0 vrg       (1000) users      (985)    14333 2023-01-06 20:37:18.000000 statmorph-0.5.2/statmorph/utils/image_diagnostics.py
+drwxr-xr-x   0 vrg       (1000) users      (985)        0 2023-08-04 03:24:09.159616 statmorph-0.5.2/statmorph/utils/tests/
+-rw-r--r--   0 vrg       (1000) users      (985)     1170 2022-10-15 05:52:47.000000 statmorph-0.5.2/statmorph/utils/tests/test_image_diagnostics.py
+drwxr-xr-x   0 vrg       (1000) users      (985)        0 2023-08-04 03:24:09.156282 statmorph-0.5.2/statmorph.egg-info/
+-rw-r--r--   0 vrg       (1000) users      (985)     2263 2023-08-04 03:24:09.000000 statmorph-0.5.2/statmorph.egg-info/PKG-INFO
+-rw-r--r--   0 vrg       (1000) users      (985)      763 2023-08-04 03:24:09.000000 statmorph-0.5.2/statmorph.egg-info/SOURCES.txt
+-rw-r--r--   0 vrg       (1000) users      (985)        1 2023-08-04 03:24:09.000000 statmorph-0.5.2/statmorph.egg-info/dependency_links.txt
+-rw-r--r--   0 vrg       (1000) users      (985)      103 2023-08-04 03:24:09.000000 statmorph-0.5.2/statmorph.egg-info/requires.txt
+-rw-r--r--   0 vrg       (1000) users      (985)       10 2023-08-04 03:24:09.000000 statmorph-0.5.2/statmorph.egg-info/top_level.txt
```

### Comparing `statmorph-0.5.1/LICENSE` & `statmorph-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `statmorph-0.5.1/PKG-INFO` & `statmorph-0.5.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: statmorph
-Version: 0.5.1
+Version: 0.5.2
 Summary: Non-parametric morphological diagnostics of galaxy images
 Home-page: https://github.com/vrodgom/statmorph
 Author: Vicente Rodriguez-Gomez
 Author-email: vrodgom.astro@gmail.com
 License: BSD
 Keywords: astronomy galaxies galaxy-morphology non-parametric
 Classifier: Development Status :: 4 - Beta
```

### Comparing `statmorph-0.5.1/README.rst` & `statmorph-0.5.2/README.rst`

 * *Files identical despite different names*

### Comparing `statmorph-0.5.1/docs/Makefile` & `statmorph-0.5.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `statmorph-0.5.1/docs/_static/banner.svg` & `statmorph-0.5.2/docs/_static/banner.svg`

 * *Files identical despite different names*

### Comparing `statmorph-0.5.1/docs/_static/favicon.ico` & `statmorph-0.5.2/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `statmorph-0.5.1/docs/_static/logo.png` & `statmorph-0.5.2/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `statmorph-0.5.1/docs/conf.py` & `statmorph-0.5.2/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # -- Project information -----------------------------------------------------
 
 project = 'statmorph'
 copyright = '2017-2023, Vicente Rodriguez-Gomez'
 author = 'Vicente Rodriguez-Gomez'
 
 # The full version, including alpha/beta/rc tags
-release = '0.5.1'
+release = '0.5.2'
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
```

### Comparing `statmorph-0.5.1/docs/description.rst` & `statmorph-0.5.2/docs/description.rst`

 * *Files 10% similar despite different names*

```diff
@@ -41,26 +41,33 @@
   that should be masked (e.g., to remove contamination from foreground stars).
 - ``psf`` : A 2D array (usually smaller than the image) representing the point
   spread function (PSF). This is used when fitting Sersic profiles.
 
 In addition, almost all of the parameters used in the calculation of the
 morphological diagnostics can be specified by the user as keyword
 arguments, although it is recommended to leave the default values alone.
+An exception might be the ``cutout_extent`` parameter, which specifies the
+extent of the region (as a multiple of the size of the appropriate segment
+in the segmentation map) used by statmorph to perform the morphological
+measurements. Since the segmentation map is user-defined, in some cases it
+makes sense to increase the value of ``cutout_extent`` from 2.5 (the default)
+to 5 or 10, depending on the sensitivity of the original segmentation map.
+
 For a complete list of keyword arguments, please see the
 `API Reference <api.html>`_.
 
 Output
 ------
 
 The output of the `source_morphology` function is a list of
 `SourceMorphology` objects, one for each labeled source, in which the
 different morphological measurements can be accessed as keys or attributes.
 
-Apart from the morphological parameters, statmorph also returns two
-different quality flags:
+Apart from the morphological parameters, statmorph also returns three
+quality flags:
 
 - ``flag`` : indicates the quality of the basic morphological measurements.
   It can take one of the following values:
 
   - 0 (good): there were no problems with the measurements.
   - 1 (suspect): the Gini segmap is discontinuous (e.g., due to a secondary
     source that was not properly labeled/masked) or the Gini and MID segmaps
@@ -71,20 +78,27 @@
     are attempted anyway and a non-null value (i.e., not -99) might be
     returned for most measurements.
   - 3 (n/a): not currently used.
   - 4 (catastrophic): this value is returned when even the most basic
     measurements would be futile (e.g., a source with a negative total flux).
     This replaces the ``flag_catastrophic`` from earlier versions of statmorph.
 
-- ``flag_sersic`` : indicates if there was a problem during the
-  Sersic profile fitting: values of 0 and 1 indicate good
-  and bad fits, respectively.
-
-In general, users should enforce ``flag <= 1``, while ``flag_sersic == 0``
-should be used only when users are actually interested in Sersic fits
-(which can fail for merging galaxies and other "irregular" objects).
+- ``flag_sersic`` : indicates the quality of the Sersic fit. Just like
+  ``flag``, it can take the following values: 0 (good), 1 (suspect), 2 (bad),
+  and 4 (catastrophic).
+
+- ``flag_doublesersic`` : indicates the quality of the double Sersic fit.
+  It can take values of 0 (good), 1 (suspect), 2 (bad), and 4 (catastrophic).
+  This flag is only generated when statmorph is called with the option
+  ``include_doublesersic = True``.
+
+
+In general, users should enforce ``flag <= 1``, while ``flag_sersic <= 1``
+and ``flag_doublesersic <= 1`` should only be imposed when the user is
+actually interested in the corresponding model fits (which, naturally, can
+fail when the model is not a good description of the data).
 
-In addition to the flags described above, the output should
+In addition to the flags described above, the output should usually
 not be trusted when the smallest of the measured distance scales (``r20``)
 is smaller than the radius at half-maximum of the PSF,
 or when the signal-to-noise per pixel (``sn_per_pixel``) is lower than 2.5
 (`Lotz et al. 2006 <https://ui.adsabs.harvard.edu/abs/2006ApJ...636..592L>`_).
```

### Comparing `statmorph-0.5.1/docs/index.rst` & `statmorph-0.5.2/docs/index.rst`

 * *Files 2% similar despite different names*

```diff
@@ -23,16 +23,17 @@
 
 .. toctree::
    :maxdepth: 2
    :caption: Contents:
    
    overview
    installation
-   notebooks/tutorial
    description
+   notebooks/tutorial
+   examples
    api
 
 Citing
 ------
 
 If you use this code for a scientific publication, please cite the following
 article:
```

### Comparing `statmorph-0.5.1/docs/installation.rst` & `statmorph-0.5.2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `statmorph-0.5.1/docs/notebooks/tutorial.ipynb` & `statmorph-0.5.2/docs/notebooks/tutorial.ipynb`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9720975505975507%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(3, '\\n'), (4, 'If you already have a real astronomical "*

 * *            'image and segmentation map to work with, jump to [Running '*

 * *            "statmorph](#Running-statmorph).\\n'), (5, '\\n'), (9, 'We import some Python packages "*

 * *            'first. If you are missing any of these, please see the the installation '*

 * *            "instructions.')], delete: [6]}}, 1: {'source': {insert: [(3, 'from "*

 * *            "astropy.modeling.models import Sersic2D\\n'), (4, 'from ast […]*

```diff
@@ -4,82 +4,82 @@
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Tutorial / How to use\n",
                 "\n",
                 "In this tutorial we create a (simplified) synthetic galaxy image from scratch, along with its associated segmentation map, and then run the statmorph code on it.\n",
                 "\n",
+                "If you already have a real astronomical image and segmentation map to work with, jump to [Running statmorph](#Running-statmorph).\n",
+                "\n",
+                "\n",
                 "### Setting up\n",
                 "\n",
-                "We import some Python packages first. If you are missing any of these, please see the the Installation section of the README."
+                "We import some Python packages first. If you are missing any of these, please see the the installation instructions."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import numpy as np\n",
                 "import matplotlib.pyplot as plt\n",
-                "import scipy.ndimage as ndi\n",
                 "from astropy.visualization import simple_norm\n",
-                "from astropy.modeling import models\n",
-                "from astropy.convolution import convolve\n",
-                "import photutils\n",
+                "from astropy.modeling.models import Sersic2D\n",
+                "from astropy.convolution import convolve, Gaussian2DKernel\n",
+                "from photutils.segmentation import detect_threshold, detect_sources\n",
                 "import time\n",
                 "import statmorph\n",
                 "%matplotlib inline"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "**Creating a model galaxy image**\n",
                 "\n",
-                "We assume that the image size is 240x240 pixels, and that the \"true\" light distribution is described by a 2D Sersic profile with the following parameters:"
+                "We assume that the image size is 240x240 pixels and that the \"true\" light distribution is described by a 2D Sersic model with the following parameters:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "ny, nx = 240, 240\n",
                 "y, x = np.mgrid[0:ny, 0:nx]\n",
-                "sersic_model = models.Sersic2D(\n",
+                "sersic_model = Sersic2D(\n",
                 "    amplitude=1, r_eff=20, n=2.5, x_0=120.5, y_0=96.5,\n",
-                "    ellip=0.5, theta=-0.5)\n",
+                "    ellip=0.5, theta=0.5)\n",
                 "image = sersic_model(x, y)\n",
                 "plt.imshow(image, cmap='gray', origin='lower',\n",
                 "           norm=simple_norm(image, stretch='log', log_a=10000))"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "**Convolving with a PSF**\n",
                 "\n",
-                "In practice, every astronomical image is the convolution of a \"true\" image with a point spread function (PSF), which depends on the optics of the telescope, atmospheric conditions, etc. Here we assume that the PSF is a simple 2D Gaussian distribution:"
+                "In practice, every astronomical image is the convolution of a \"true\" image with a point spread function (PSF), which depends on the optics of the telescope, atmospheric conditions, etc. Here we assume that the PSF is a simple 2D Gaussian kernel with a standard deviation of 2 pixels:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "size = 20  # on each side from the center\n",
-                "sigma_psf = 2.0\n",
-                "y, x = np.mgrid[-size:size+1, -size:size+1]\n",
-                "psf = np.exp(-(x**2 + y**2)/(2.0*sigma_psf**2))\n",
-                "psf /= np.sum(psf)\n",
+                "kernel = Gaussian2DKernel(2)\n",
+                "kernel.normalize()  # make sure kernel adds up to 1\n",
+                "psf = kernel.array  # we only need the numpy array\n",
                 "plt.imshow(psf, origin='lower', cmap='gray')"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -97,120 +97,107 @@
                 "           norm=simple_norm(image, stretch='log', log_a=10000))"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "**Adding noise**\n",
+                "**Applying shot noise**\n",
                 "\n",
-                "Here we add homogeneous Gaussian background noise, optimistically assuming that the signal-to-noise ratio (S/N) is 100 at the effective radius (where we had defined the S\u00e9rsic profile amplitude as 1.0). For simplicity, we do not consider Poisson noise associated with the source itself."
+                "One source of noise in astronomical images originates from the Poisson statistics of the number of electrons recorded by each pixel. We can model this effect by introducing a *gain* parameter, a scalar that can be multiplied by the science image to obtain the number of electrons per pixel.\n",
+                "\n",
+                "For the sake of this example, we choose a very large gain value, so that shot noise becomes almost negligible (10^5 electrons/pixel at the effective radius, where we had defined an amplitude of 1.0 in arbitrary units). The resulting image after applying shot noise looks very similar to the one from the previous step and is not shown."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "metadata": {
-                "scrolled": false
-            },
+            "metadata": {},
             "outputs": [],
             "source": [
-                "np.random.seed(1)\n",
-                "snp = 100.0\n",
-                "image += (1.0 / snp) * np.random.standard_normal(size=(ny, nx))\n",
-                "plt.imshow(image, cmap='gray', origin='lower',\n",
-                "           norm=simple_norm(image, stretch='log', log_a=10000))"
+                "np.random.seed(3)\n",
+                "gain = 1e5\n",
+                "image = np.random.poisson(image * gain) / gain"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "**Gain and weight maps**\n",
+                "**Applying background noise**\n",
                 "\n",
-                "The code will ask for one of two input arguments: (1) a weight map, which is a 2D array (of the same size as the input image) representing one standard deviation at each pixel value, or (2) the gain, a scalar that can be multiplied by the science image to obtain the number of electron counts per pixel. The gain parameter is used internally by statmorph to calculate the weight map.\n",
+                "Apart from shot noise, astronomical images have a sky background noise component, which we here model with a uniform Gaussian distribution centered at zero (since the image is background-subtracted).\n",
                 "\n",
-                "Here we assume, also somewhat optimistically, that there is an average of 10,000 electron counts/pixel at the effective radius (where we had defined the amplitude as 1.0), so that the gain is 10,000."
+                "We assume, somewhat optimistically, that the signal-to-noise ratio (S/N) per pixel is 100 at the effective radius (where we had defined the Sersic model amplitude as 1.0)."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "metadata": {},
+            "metadata": {
+                "scrolled": false
+            },
             "outputs": [],
             "source": [
-                "gain = 10000.0"
+                "snp = 100.0\n",
+                "sky_sigma = 1.0 / snp\n",
+                "image += sky_sigma * np.random.standard_normal(size=(ny, nx))\n",
+                "plt.imshow(image, cmap='gray', origin='lower',\n",
+                "           norm=simple_norm(image, stretch='log', log_a=10000))"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "**Creating a segmentation map**\n",
+                "**Gain and weight maps**\n",
                 "\n",
-                "Besides the image itself and the weight map/gain, the only other *required* argument is the segmentation map, which labels the pixels belonging to different sources. It is usually generated by specialized tools such as SExtractor, but here we create it using photutils:"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "threshold = photutils.detect_threshold(image, 1.5)\n",
-                "npixels = 5  # minimum number of connected pixels\n",
-                "segm = photutils.detect_sources(image, threshold, npixels)"
+                "Note that statmorph will ask for one of two input arguments: (1) a weight map, which is a 2D array (of the same size as the input image) representing one standard deviation at each pixel value, or (2) the gain, which was described above. In the latter case, the gain parameter is used internally by statmorph (along with an automatic estimation of the sky background noise) to calculate the weight map."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "Although statmorph is designed to process all the sources labeled by the segmentation map, in this example we only focus on the main (largest) source found in the image."
+                "**Creating a segmentation map**\n",
+                "\n",
+                "Besides the image itself and the weight map/gain, the only other *required* argument is the segmentation map, which labels the pixels belonging to different sources. It is usually generated with specialized tools such as SExtractor or photutils. Here we use the latter to create a simplified segmentation map, where we detect sources that lie above a 1.5-sigma detection threshold.\n",
+                "\n",
+                "Note that the detection stage (but, importantly, not the threshold calculation) is carried out on a \"convolved\" version of the image. This is done in order to smooth out small-scale noise and thus ensure that the shapes of the detected segments are reasonably smooth."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "# Keep only the largest segment\n",
-                "label = np.argmax(segm.areas) + 1\n",
-                "segmap = segm.data == label\n",
+                "threshold = detect_threshold(image, 1.5)\n",
+                "npixels = 5  # minimum number of connected pixels\n",
+                "convolved_image = convolve(image, psf)\n",
+                "segmap = detect_sources(convolved_image, threshold, npixels)\n",
                 "plt.imshow(segmap, origin='lower', cmap='gray')"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "We regularize a bit the shape of the segmentation map:"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "segmap_float = ndi.uniform_filter(np.float64(segmap), size=10)\n",
-                "segmap = np.int64(segmap_float > 0.5)\n",
-                "plt.imshow(segmap, origin='lower', cmap='gray')"
+                "In this particular case, the obtained segmap has only two values: 0 for the background (as should always be the case) and 1 for the only labeled source. However, statmorph is designed to process all the sources labeled by a segmentation map, which makes it applicable to large mosaic images."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Running statmorph\n",
                 "\n",
-                "**Measuring morphological parameters**\n",
+                "Now that we have all the required data, we are ready to measure the morphology of the source just created. Note that we include the PSF as a keyword argument, which results in more correct Sersic profile fits.\n",
                 "\n",
-                "Now that we have all the required data, we are ready to measure the morphology of the source just created. Note that we include the PSF as a keyword argument. In principle, this results in more correct Sersic profile fits, although it can also make the code run slower, depending on the size of the PSF."
+                "Also note that we do not attempt to fit a *double* Sersic model, which would be degenerate in this particular case (the two components would be identical and their relative amplitudes would be unconstrained). For a demonstration of statmorph's double Sersic fitting functionality, see the [Double 2D Sersic example](./doublesersic.html)."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -221,15 +208,17 @@
                 "print('Time: %g s.' % (time.time() - start))"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "In general, `source_morphs` is a list of objects, each corresponding to a labeled source in the image. Here we focus on the first (and only) labeled source."
+                "### Examining the output\n",
+                "\n",
+                "In general, `source_morphs` is a list of objects corresponding to each labeled source in the image. Here we focus on the first (and only) labeled source:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -246,14 +235,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
+                "print('BASIC MEASUREMENTS (NON-PARAMETRIC)')\n",
                 "print('xc_centroid =', morph.xc_centroid)\n",
                 "print('yc_centroid =', morph.yc_centroid)\n",
                 "print('ellipticity_centroid =', morph.ellipticity_centroid)\n",
                 "print('elongation_centroid =', morph.elongation_centroid)\n",
                 "print('orientation_centroid =', morph.orientation_centroid)\n",
                 "print('xc_asymmetry =', morph.xc_asymmetry)\n",
                 "print('yc_asymmetry =', morph.yc_asymmetry)\n",
@@ -270,96 +260,57 @@
                 "print('M20 =', morph.m20)\n",
                 "print('F(G, M20) =', morph.gini_m20_bulge)\n",
                 "print('S(G, M20) =', morph.gini_m20_merger)\n",
                 "print('sn_per_pixel =', morph.sn_per_pixel)\n",
                 "print('C =', morph.concentration)\n",
                 "print('A =', morph.asymmetry)\n",
                 "print('S =', morph.smoothness)\n",
+                "print()\n",
+                "print('SERSIC MODEL')\n",
                 "print('sersic_amplitude =', morph.sersic_amplitude)\n",
                 "print('sersic_rhalf =', morph.sersic_rhalf)\n",
                 "print('sersic_n =', morph.sersic_n)\n",
                 "print('sersic_xc =', morph.sersic_xc)\n",
                 "print('sersic_yc =', morph.sersic_yc)\n",
                 "print('sersic_ellip =', morph.sersic_ellip)\n",
                 "print('sersic_theta =', morph.sersic_theta)\n",
+                "print('sersic_chi2_dof =', morph.sersic_chi2_dof)\n",
+                "print()\n",
+                "print('OTHER')\n",
                 "print('sky_mean =', morph.sky_mean)\n",
                 "print('sky_median =', morph.sky_median)\n",
                 "print('sky_sigma =', morph.sky_sigma)\n",
                 "print('flag =', morph.flag)\n",
                 "print('flag_sersic =', morph.flag_sersic)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "Note that the fitted Sersic profile is in pretty good agreement with the \"true\" Sersic profile that we originally defined (n=2.5, r_eff=20, etc.). However, such agreement tends to deteriorate somewhat at higher noise levels and larger Sersic indices (not to mention that real galaxies are not always well described by Sersic profiles).\n",
+                "Note that the fitted Sersic model is in very good agreement with the \"true\" Sersic model that we originally defined (n = 2.5, rhalf = 20, etc.) and that the reduced chi-squared statistic (sersic_chi2_dof) is close to 1, indicating a good fit without overfitting. However, such good agreement tends to deteriorate somewhat at higher noise levels, and one has to keep in mind that not all galaxies are well described by Sersic profiles.\n",
                 "\n",
-                "Other morphological measurements that are more general and more robust to noise, which are also calculated by statmorph, include the Gini-M20 (Lotz et al. 2004), CAS (Conselice 2003) and MID (Freeman et al. 2013) statistics, as well as the outer asymmetry (Wen et al. 2014) and shape asymmetry (Pawlik et al. 2016).\n",
+                "Other morphological measurements that are more general and robust to noise, which are also calculated by statmorph, include the Gini-M20 (Lotz et al. 2004), CAS (Conselice 2003) and MID (Freeman et al. 2013) statistics, as well as the outer asymmetry (Wen et al. 2014) and shape asymmetry (Pawlik et al. 2016).\n",
                 "\n",
                 "Also note that statmorph returns two quality flags:\n",
                 "\n",
-                "1. ``flag`` : indicates the quality the basic morphological measurements, taking one of the following values: 0 (good), 1 (suspect), 2 (bad), or 4 (catastrophic). More details can be found [here](https://statmorph.readthedocs.io/en/latest/description.html#output).\n",
+                "1. ``flag`` : indicates the quality of the basic morphological measurements, taking one of the following values: 0 (good), 1 (suspect), 2 (bad), or 4 (catastrophic). More details can be found [here](../description.html#output).\n",
                 "\n",
-                "2. ``flag_sersic`` : indicates if there was a problem/warning during the Sersic profile fitting: values of 0 and 1 indicate good and bad fits, respectively.\n",
+                "2. ``flag_sersic`` : indicates the quality of the Sersic fit, also taking values of 0 (good), 1 (suspect), 2 (bad), or 4 (catastrophic).\n",
                 "\n",
-                "In general, ``flag <= 1`` should always be enforced, while ``flag_sersic == 0`` should only be used when one is interested in Sersic fits (which might fail for merging galaxies and other \"irregular\" objects)."
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "**Examining the fitted Sersic profile**\n",
-                "\n",
-                "Finally, we can reconstruct the fitted Sersic profile and examine its residual. Here we used the ``ConvolvedSersic2D`` class defined in ``statmorph``."
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "ny, nx = image.shape\n",
-                "y, x = np.mgrid[0:ny, 0:nx]\n",
-                "fitted_model = statmorph.ConvolvedSersic2D(\n",
-                "    amplitude=morph.sersic_amplitude,\n",
-                "    r_eff=morph.sersic_rhalf,\n",
-                "    n=morph.sersic_n,\n",
-                "    x_0=morph.sersic_xc,\n",
-                "    y_0=morph.sersic_yc,\n",
-                "    ellip=morph.sersic_ellip,\n",
-                "    theta=morph.sersic_theta)\n",
-                "fitted_model.set_psf(psf)  # required when using ConvolvedSersic2D\n",
-                "image_model = fitted_model(x, y)\n",
-                "bg_noise = (1.0 / snp) * np.random.standard_normal(size=(ny, nx))\n",
-                "fig = plt.figure(figsize=(15,5))\n",
-                "ax = fig.add_subplot(131)\n",
-                "ax.imshow(image, cmap='gray', origin='lower',\n",
-                "           norm=simple_norm(image, stretch='log', log_a=10000))\n",
-                "ax.set_title('Original image')\n",
-                "ax = fig.add_subplot(132)\n",
-                "ax.imshow(image_model + bg_noise, cmap='gray', origin='lower',\n",
-                "           norm=simple_norm(image, stretch='log', log_a=10000))\n",
-                "ax.set_title('Fitted model')\n",
-                "ax = fig.add_subplot(133)\n",
-                "residual = image - image_model\n",
-                "ax.imshow(residual, cmap='gray', origin='lower',\n",
-                "           norm=simple_norm(residual, stretch='linear'))\n",
-                "ax.set_title('Residual')"
+                "In general, ``flag <= 1`` should always be enforced, while ``flag_sersic <= 1`` should only be used when one is interested in the Sersic fits (which might fail for merging galaxies and other \"irregular\" objects)."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "**Examining other morphological diagnostics**\n",
+                "**Visualizing the morphological measurements**\n",
                 "\n",
-                "For convenience, we also provide a ``make_figure`` function that can be used to visualize some of the basic morphological measurements carried out by ``statmorph``. This creates a multi-panel figure analogous to Fig. 4 from Rodriguez-Gomez et al. (2019)."
+                "For convenience, statmorph includes a ``make_figure`` function that can be used to visualize some of the morphological measurements. This creates a multi-panel figure analogous to Fig. 4 from Rodriguez-Gomez et al. (2019)."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -391,13 +342,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.8"
+            "version": "3.10.11"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 2
 }
```

### Comparing `statmorph-0.5.1/docs/overview.rst` & `statmorph-0.5.2/docs/overview.rst`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 - Gini-M20 statistics (Lotz et al. 2004; Snyder et al. 2015a,b)
 - Concentration, Asymmetry and Smoothness (CAS) statistics
   (Bershady et al. 2000; Conselice 2003; Lotz et al. 2004)
 - Multimode, Intensity and Deviation (MID) statistics (Freeman et al. 2013;
   Peth et al. 2016)
 - Outer asymmetry and shape asymmetry (Wen et al. 2014; Pawlik et al. 2016)
-- Sérsic index (Sérsic 1968)
+- Single and double Sérsic indices (Sérsic 1968)
 - Several shape and size measurements associated to the above statistics
   (ellipticity, Petrosian radius, half-light radius, etc.)
 
 .. ~ For more information, please see:
 
 .. ~ - `Rodriguez-Gomez et al. (2019) <https://ui.adsabs.harvard.edu/abs/2019MNRAS.483.4140R>`_
```

### Comparing `statmorph-0.5.1/setup.py` & `statmorph-0.5.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 # Get the long description from the README file
 with open(path.join(here, 'README.rst'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='statmorph',
-    version='0.5.1',
+    version='0.5.2',
     description='Non-parametric morphological diagnostics of galaxy images',
     long_description=long_description,
     url='https://github.com/vrodgom/statmorph',
     author='Vicente Rodriguez-Gomez',
     author_email='vrodgom.astro@gmail.com',
     license='BSD',
     classifiers=[
```

### Comparing `statmorph-0.5.1/statmorph/statmorph.py` & `statmorph-0.5.2/statmorph/statmorph.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,38 +1,44 @@
 """
 Python code for calculating non-parametric morphological diagnostics
 of galaxy images.
 """
 # Author: Vicente Rodriguez-Gomez <vrodgom.astro@gmail.com>
 # Licensed under a 3-Clause BSD License.
-from pkg_resources import parse_version
 import warnings
 import time
 import numpy as np
 import scipy.optimize as opt
 import scipy.ndimage as ndi
 import scipy.signal
 import skimage.measure
 import skimage.transform
 import skimage.feature
 import skimage.segmentation
 from astropy.utils import lazyproperty
 from astropy.stats import sigma_clipped_stats
-from astropy.modeling import models, fitting
+from astropy.modeling import models, fitting, Fittable2DModel, Parameter
 from astropy.utils.exceptions import (
     AstropyUserWarning, AstropyDeprecationWarning)
 from astropy.convolution import convolve
 import photutils
 
-__all__ = ['ConvolvedSersic2D', 'SourceMorphology', 'source_morphology',
-           '__version__']
+__all__ = [
+    'ConvolvedSersic2D',
+    'DoubleSersic2D',
+    'ConvolvedDoubleSersic2D',
+    'SourceMorphology',
+    'source_morphology',
+    '__version__',
+]
 
-__version__ = '0.5.1'
+__version__ = '0.5.2'
 
-# A list of all the quantities that are calculated by SourceMorphology:
+# A list of the quantities calculated by SourceMorphology,
+# excluding the double Sersic parameters:
 _quantity_names = [
     'xc_centroid',
     'yc_centroid',
     'ellipticity_centroid',
     'elongation_centroid',
     'orientation_centroid',
     'xc_asymmetry',
@@ -67,57 +73,79 @@
     'sersic_amplitude',
     'sersic_rhalf',
     'sersic_n',
     'sersic_xc',
     'sersic_yc',
     'sersic_ellip',
     'sersic_theta',
+    'sersic_chi2_dof',
     'sky_mean',
     'sky_median',
     'sky_sigma',
     'xmin_stamp',
     'ymin_stamp',
     'xmax_stamp',
     'ymax_stamp',
     'nx_stamp',
     'ny_stamp',
 ]
 
+# A list of the quantities generated by the double Sersic fit:
+_doublesersic_quantity_names = [
+    'doublesersic_xc',
+    'doublesersic_yc',
+    'doublesersic_amplitude1',
+    'doublesersic_rhalf1',
+    'doublesersic_n1',
+    'doublesersic_ellip1',
+    'doublesersic_theta1',
+    'doublesersic_amplitude2',
+    'doublesersic_rhalf2',
+    'doublesersic_n2',
+    'doublesersic_ellip2',
+    'doublesersic_theta2',
+    'doublesersic_chi2_dof',
+]
+
+
 def _quantile(sorted_values, q):
     """
     For a sorted (in increasing order) 1-d array, return the value
     corresponding to the quantile ``q``.
 
     Notes
     -----
     The result is identical to np.percentile(..., interpolation='lower'),
     but the currently defined function is infinitely faster for sorted arrays.
     """
     if q < 0 or q > 1:
         raise ValueError('Quantiles must be in the range [0, 1].')
     return sorted_values[int(q*(len(sorted_values)-1))]
 
+
 def _aperture_area(ap, mask, **kwargs):
     """
     Calculate the area of a photutils aperture object,
     excluding masked pixels.
     """
     return ap.do_photometry(np.float64(~mask), **kwargs)[0][0]
 
+
 def _aperture_mean_nomask(ap, image, **kwargs):
     """
     Calculate the mean flux of an image for a given photutils
     aperture object. Note that we do not use ``_aperture_area``
     here. Instead, we divide by the full area of the
     aperture, regardless of masked and out-of-range pixels.
     This avoids problems when the aperture is larger than the
     region of interest.
     """
     return ap.do_photometry(image, **kwargs)[0][0] / ap.area
 
+
 def _fraction_of_total_function_circ(r, image, center, fraction, total_sum):
     """
     Helper function to calculate ``_radius_at_fraction_of_total_circ``.
     """
     assert (r >= 0) & (fraction >= 0) & (fraction <= 1) & (total_sum > 0)
     if r == 0:
         cur_fraction = 0.0
@@ -125,14 +153,15 @@
         ap = photutils.aperture.CircularAperture(center, r)
         # Force flux sum to be positive:
         ap_sum = np.abs(ap.do_photometry(image, method='exact')[0][0])
         cur_fraction = ap_sum / total_sum
 
     return cur_fraction - fraction
 
+
 def _radius_at_fraction_of_total_circ(image, center, r_total, fraction):
     """
     Return the radius (in pixels) of a concentric circle that
     contains a given fraction of the light within ``r_total``.
     """
     flag = 0
 
@@ -165,14 +194,15 @@
         i += 1
 
     r = opt.brentq(_fraction_of_total_function_circ, r_min, r_max,
                    args=(image, center, fraction, total_sum), xtol=1e-6)
 
     return r, flag
 
+
 def _fraction_of_total_function_ellip(a, image, center, elongation, theta,
                                       fraction, total_sum):
     """
     Helper function to calculate ``_radius_at_fraction_of_total_ellip``.
     """
     assert (a >= 0) & (fraction >= 0) & (fraction <= 1) & (total_sum > 0)
     if a == 0:
@@ -182,14 +212,15 @@
         ap = photutils.aperture.EllipticalAperture(center, a, b, theta=theta)
         # Force flux sum to be positive:
         ap_sum = np.abs(ap.do_photometry(image, method='exact')[0][0])
         cur_fraction = ap_sum / total_sum
 
     return cur_fraction - fraction
 
+
 def _radius_at_fraction_of_total_ellip(image, center, elongation, theta,
                                        a_total, fraction):
     """
     Return the semimajor axis (in pixels) of a concentric ellipse that
     contains a given fraction of the light within a larger ellipse of
     semimajor axis ``a_total``.
     """
@@ -227,46 +258,148 @@
 
     a = opt.brentq(_fraction_of_total_function_ellip, a_min, a_max,
                    args=(image, center, elongation, theta, fraction, total_sum),
                    xtol=1e-6)
 
     return a, flag
 
+
+def _postfitting_fix(a, ellip, theta):
+    """
+    In some rare cases, the ellipticity of the fitted Sersic models is
+    outside the range [0, 1]. While we could constrain this parameter
+    during the fit using the ``bounds`` keyword argument in `Sersic2D`,
+    a less aggressive solution is to create an equivalent model after
+    fitting by exploiting degeneracies between the ellipticity,
+    semimajor and semiminor axes, and position angle, as we do here.
+    """
+    if a < 0:  # (1)
+        # First of all, we make sure that the semimajor axis is positive
+        # (note that only a^2 appears in the equations in Sersic2D).
+        a *= -1
+    if ellip > 1:  # (2)
+        # Note that the semiminor axis is given by
+        # b = (1 - ellip) * a.
+        # This would yield a negative value for b, but since only b^2
+        # is required, we can define an equivalent ellipticity as
+        # 1 - ellip' = -(1 - ellip)  =>  ellip' = 2 - ellip.
+        ellip = 2.0 - ellip
+    if ellip < 0:  # (3)
+        # This can be interpreted as a, b being flipped (a < b), so we
+        # switch them and define an equivalent ellipticity as
+        # 1 - ellip' = 1 / (1 - ellip)  =>  ellip' = ellip / (ellip - 1).
+        a = (1 - ellip) * a
+        ellip = ellip / (ellip - 1)
+        # We also need to rotate the position angle by 90 degrees:
+        theta += np.pi / 2
+    # Finally, note that the "corrections" above are not mutually exclusive.
+    # If a Sersic model has ellipticity > 2, then steps (2) and (3) are
+    # applied successively.
+
+    return a, ellip, theta
+
+
 class ConvolvedSersic2D(models.Sersic2D):
     """
-    Two-dimensional Sersic surface brightness profile, convolved with
-    a PSF provided by the user as a numpy array.
+    Sersic2D model convolved with a PSF (provided by the user as a
+    numpy array).
 
     See Also
     --------
     astropy.modeling.models.Sersic2D
 
     """
     psf = None
 
-    @classmethod
-    def set_psf(cls, psf):
+    def set_psf(self, psf):
         """
         Specify the PSF to be convolved with the Sersic2D model.
         """
-        cls.psf = psf / np.sum(psf)  # make sure it's normalized
+        self.psf = np.float64(psf) / np.sum(psf)  # make sure it's normalized
 
-    @classmethod
-    def evaluate(cls, x, y, amplitude, r_eff, n, x_0, y_0, ellip, theta):
+    def evaluate(self, x, y, amplitude, r_eff, n, x_0, y_0, ellip, theta):
         """
         Evaluate the ConvolvedSersic2D model.
         """
-        z_sersic = models.Sersic2D.evaluate(x, y, amplitude, r_eff, n, x_0, y_0,
-                                            ellip, theta)
-        if cls.psf is None:
+        z = models.Sersic2D.evaluate(
+            x, y, amplitude, r_eff, n, x_0, y_0, ellip, theta)
+        if self.psf is None:
+            raise AssertionError('Must specify PSF using set_psf method.')
+
+        assert z.dtype == np.float64 and self.psf.dtype == np.float64
+
+        return scipy.signal.fftconvolve(z, self.psf, mode='same')
+
+
+class DoubleSersic2D(Fittable2DModel):
+    """
+    Custom class for a double 2D Sersic model. Note that the two
+    components share the same center.
+    """
+    # Shared center
+    x_0 = Parameter(default=0)
+    y_0 = Parameter(default=0)
+    # First component
+    amplitude_1 = Parameter(default=1)
+    r_eff_1 = Parameter(default=1)
+    n_1 = Parameter(default=4)  # de Vaucouleurs
+    ellip_1 = Parameter(default=0)
+    theta_1 = Parameter(default=0)
+    # Second component
+    amplitude_2 = Parameter(default=1)
+    r_eff_2 = Parameter(default=1)
+    n_2 = Parameter(default=1)  # exponential
+    ellip_2 = Parameter(default=0)
+    theta_2 = Parameter(default=0)
+
+    @classmethod
+    def evaluate(cls, x, y, x_0, y_0,
+                 amplitude_1, r_eff_1, n_1, ellip_1, theta_1,
+                 amplitude_2, r_eff_2, n_2, ellip_2, theta_2):
+        """
+        Evaluate the DoubleSersic2D model.
+        """
+        return (
+            models.Sersic2D.evaluate(
+                x, y, amplitude_1, r_eff_1, n_1, x_0, y_0, ellip_1, theta_1)
+            + models.Sersic2D.evaluate(
+                x, y, amplitude_2, r_eff_2, n_2, x_0, y_0, ellip_2, theta_2)
+        )
+
+
+class ConvolvedDoubleSersic2D(DoubleSersic2D):
+    """
+    DoubleSersic2D model convolved with a PSF (provided by the user
+    as a numpy array).
+    """
+    psf = None
+
+    def set_psf(self, psf):
+        """
+        Specify the PSF to be convolved with the DoubleSersic2D model.
+        """
+        self.psf = np.float64(psf) / np.sum(psf)  # make sure it's normalized
+
+    def evaluate(self, x, y, x_0, y_0,
+                 amplitude_1, r_eff_1, n_1, ellip_1, theta_1,
+                 amplitude_2, r_eff_2, n_2, ellip_2, theta_2):
+        """
+        Evaluate the ConvolvedDoubleSersic2D model.
+        """
+        z = DoubleSersic2D.evaluate(
+            x, y, x_0, y_0,
+            amplitude_1, r_eff_1, n_1, ellip_1, theta_1,
+            amplitude_2, r_eff_2, n_2, ellip_2, theta_2)
+        if self.psf is None:
             raise AssertionError('Must specify PSF using set_psf method.')
 
-        # Apparently, scipy.signal also wants double:
-        return scipy.signal.fftconvolve(
-            np.float64(z_sersic), np.float64(cls.psf), mode='same')
+        assert z.dtype == np.float64 and self.psf.dtype == np.float64
+
+        return scipy.signal.fftconvolve(z, self.psf, mode='same')
+
 
 class SourceMorphology(object):
     """
     Class to measure the morphological parameters of a single labeled
     source. The parameters can be accessed as attributes or keys.
 
     Parameters
@@ -298,15 +431,15 @@
         weight map (i.e., the sigma-image) using Poisson statistics.
         This parameter is only used when ``weightmap`` is not provided.
     psf : array-like, optional
         A 2D array representing the PSF, where the central pixel
         corresponds to the center of the PSF. Typically, including
         this keyword argument will make the code run slower by a
         factor of a few, depending on the size of the PSF, but the
-        resulting Sersic fits will in principle be more correct.
+        resulting Sersic fits will be more correct.
     cutout_extent : float, optional
         The target fractional size of the data cutout relative to
         the minimal bounding box containing the source. The value
         must be >= 1.
     min_cutout_size : int, optional
         The minimum size of the cutout, in case ``cutout_extent`` times
         the size of the minimal bounding box is smaller than this.
@@ -372,14 +505,29 @@
         which sets a lower bound for the fitted Sersic index.
         Note that, by default, statmorph will make reasonable
         initial guesses for all the model parameters (recommended),
         although this functionality can be overridden for more
         customized fits.
     sersic_maxiter : int, optional
         Deprecated. Please use ``sersic_fitting_args`` instead.
+    include_doublesersic : bool, optional
+        If ``True``, also fit a double 2D Sersic model. The default is
+        ``False``.
+    doublesersic_tied_ellip : bool, optional
+        If True, both components of the double Sersic model share the
+        same ellipticity and position angle. The same effect could be
+        achieved using doublesersic_model_args in combination with the
+        'tied' argument, although the syntax would be slightly more
+        involved. The default value is ``False``.
+    doublesersic_fitting_args : dict, optional
+        Same as sersic_fitting_args, but for the double 2D Sersic fit.
+        The default is {'maxiter': 500, 'acc': 1e-5}.
+    doublesersic_model_args : dict, optional
+        Same as sersic_model_args, but for the double 2D Sersic fit.
+        The default is {'bounds': {'n_1': (0.01, None), 'n_2': (0.01, None)}}.
     segmap_overlap_ratio : float, optional
         The minimum ratio (in order to have a "good" measurement)
         between the area of the intersection of the Gini and MID segmaps
         and the area of the largest of these two segmaps.
     verbose : bool, optional
         If ``True``, this prints various minor warnings (which do not
         result in "bad" measurements) during the calculations.
@@ -395,15 +543,20 @@
                  n_sigma_outlier=10, annulus_width=1.0,
                  eta=0.2, petro_fraction_gini=0.2, skybox_size=32,
                  petro_extent_cas=1.5, petro_fraction_cas=0.25,
                  boxcar_size_mid=3.0, niter_bh_mid=5, sigma_mid=1.0,
                  petro_extent_flux=2.0, boxcar_size_shape_asym=3.0,
                  sersic_fitting_args={'maxiter': 500, 'acc': 1e-5},
                  sersic_model_args={'bounds': {'n': (0.01, None)}},
-                 sersic_maxiter=None, segmap_overlap_ratio=0.25, verbose=False):
+                 sersic_maxiter=None, include_doublesersic=False,
+                 doublesersic_tied_ellip=False,
+                 doublesersic_fitting_args={'maxiter': 500, 'acc': 1e-5},
+                 doublesersic_model_args={
+                     'bounds': {'n_1': (0.01, None), 'n_2': (0.01, None)}},
+                 segmap_overlap_ratio=0.25, verbose=False):
         self._image = image
         self._segmap = segmap
         self.label = label
         self._mask = mask
         self._weightmap = weightmap
         self._gain = gain
         self._psf = psf
@@ -419,14 +572,18 @@
         self._boxcar_size_mid = boxcar_size_mid
         self._niter_bh_mid = niter_bh_mid
         self._sigma_mid = sigma_mid
         self._petro_extent_flux = petro_extent_flux
         self._boxcar_size_shape_asym = boxcar_size_shape_asym
         self._sersic_fitting_args = sersic_fitting_args.copy()
         self._sersic_model_args = sersic_model_args.copy()
+        self._include_doublesersic = include_doublesersic
+        self._doublesersic_tied_ellip = doublesersic_tied_ellip
+        self._doublesersic_fitting_args = doublesersic_fitting_args.copy()
+        self._doublesersic_model_args = doublesersic_model_args.copy()
         self._segmap_overlap_ratio = segmap_overlap_ratio
         self._verbose = verbose
 
         # Measure runtime
         start = time.time()
 
         if not isinstance(self._segmap, photutils.segmentation.SegmentationImage):
@@ -447,21 +604,19 @@
             assert self._mask.dtype == np.bool_
         if self._weightmap is not None:
             assert self._weightmap.shape == self._image.shape
 
         if self._weightmap is None and self._gain is None:
             raise AssertionError('Must provide either weightmap or gain.')
 
-        # Normalize PSF
-        if self._psf is not None:
-            self._psf = self._psf / np.sum(self._psf)
-
         # These flags will be modified during the calculations:
         self.flag = 0  # attempts to flag bad measurements (0-4)
         self.flag_sersic = 0  # attempts to flag bad Sersic fits (0 or 1)
+        if self._include_doublesersic:
+            self.flag_doublesersic = 0  # flag bad double Sersic fits (0 or 1)
 
         # If something goes wrong, use centroid instead of asymmetry center
         # (better performance in some pathological cases, e.g. GOODS-S 32143):
         self._use_centroid = False
 
         # Check that the labeled galaxy segment has a positive flux sum.
         # If not, this is bad enough to abort all calculations and return
@@ -547,24 +702,31 @@
         interrupting the constructor.
         """
         for q in _quantity_names:
             setattr(self, q, -99.0)
         self.nx_stamp = -99
         self.ny_stamp = -99
         self.flag = 4  # catastrophic
-        self.flag_sersic = 1
+        self.flag_sersic = 4
         self.runtime = -99.0
+        self.sersic_runtime = -99.0
+        if self._include_doublesersic:
+            self.flag_doublesersic = 4
+            self.doublesersic_runtime = -99.0
 
     def _calculate_morphology(self):
         """
-        Calculate all morphological parameters, which are stored
+        Calculate morphological parameters and store them
         as "lazy" properties.
         """
         for q in _quantity_names:
-            tmp = self[q]
+            _ = self[q]
+        if self._include_doublesersic:
+            for q in _doublesersic_quantity_names:
+                _ = self[q]
 
     def _check_segmaps(self):
         """
         Compare Gini segmap and MID segmap; set flag = 1 (suspect) if they are
         very different from each other.
         """
         area_max = max(np.sum(self._segmap_gini),
@@ -1834,15 +1996,15 @@
         """
         Create a new segmentation map as described in Section 4.3 from
         Freeman et al. (2013).
 
         Notes
         -----
         This implementation improves upon previous ones by making
-        the MID segmap independent from the number of quantiles
+        the MID segmap independent of the number of quantiles
         used in the calculation, as well as other parameters.
         """
         num_pixelvals = len(self._sorted_pixelvals_stamp_no_bg_nonnegative)
 
         # In some rare cases (as a consequence of an erroneous
         # initial segmap, as in J095553.0+694048_g.fits.gz),
         # the MID segmap is technically undefined because the
@@ -2288,17 +2450,17 @@
 
         return rmax_circ
 
     @lazyproperty
     def rmax_ellip(self):
         """
         Return the semimajor axis of the minimal ellipse (with fixed
-        center, elongation and orientation) that contains all of
-        the main segment of the shape asymmetry segmap. In most
-        cases this is almost identical to rmax_circ.
+        center, elongation and orientation) that contains the entire
+        main segment of the shape asymmetry segmap. In most cases
+        this is almost identical to rmax_circ.
         """
         image = self._cutout_stamp_maskzeroed
         ny, nx = image.shape
 
         # Center at pixel that minimizes asymmetry
         xc, yc = self._asymmetry_center
 
@@ -2344,24 +2506,27 @@
     # SERSIC MODEL FIT #
     ####################
 
     @lazyproperty
     def _sersic_model(self):
         """
         Fit a 2D Sersic profile using Astropy's model fitting library.
-        An initial guess for the Sersic model will be generated based on
+        An initial guess for the model is automatically generated based on
         other statmorph measurements, although users can provide their
         own initial values (and optionally keep them fixed) via the
         ``sersic_model_args`` keyword argument.
 
         Return the fitted model object.
         """
         image = self._cutout_stamp_maskzeroed
         ny, nx = image.shape
 
+        # Measure runtime
+        start = time.time()
+
         # Start from approximate relation between n and concentration
         empirical_n = 10.0**(-1.5) * self.concentration**3.5
         empirical_n = min(max(empirical_n, 1.0), 3.5)  # limit to range [1, 3.5]
 
         # Create initial guesses for some model parameters (amplitude later)
         if 'r_eff' not in self._sersic_model_args:
             self._sersic_model_args['r_eff'] = self.rhalf_ellip
@@ -2372,15 +2537,15 @@
         if 'y_0' not in self._sersic_model_args:
             self._sersic_model_args['y_0'] = self.yc_asymmetry
         if 'ellip' not in self._sersic_model_args:
             self._sersic_model_args['ellip'] = self.ellipticity_asymmetry
         if 'theta' not in self._sersic_model_args:
             self._sersic_model_args['theta'] = self.orientation_asymmetry
 
-        # Get position of center with respect to image cutout
+        # Origin must coincide with that of image cutout
         self._sersic_model_args['x_0'] -= self.xmin_stamp
         self._sersic_model_args['y_0'] -= self.ymin_stamp
 
         # For readability
         guess_r_eff = self._sersic_model_args['r_eff']
         guess_center = np.array([self._sersic_model_args['x_0'],
                                  self._sersic_model_args['y_0']])
@@ -2389,102 +2554,110 @@
 
         # Get mean flux at the effective "radius"
         a_in = guess_r_eff - 0.5 * self._annulus_width
         a_out = guess_r_eff + 0.5 * self._annulus_width
         if a_in < 0:
             warnings.warn('[sersic] guess_r_eff < annulus_width.',
                           AstropyUserWarning)
-            self.flag_sersic = 1
+            self.flag_sersic = 2
             a_in = guess_r_eff
         b_out = (1 - guess_ellip) * a_out
         ellip_annulus = photutils.aperture.EllipticalAnnulus(
             guess_center, a_in, a_out, b_out, theta=guess_theta)
         ellip_annulus_mean_flux = _aperture_mean_nomask(
             ellip_annulus, image, method='exact')
         if ellip_annulus_mean_flux <= 0.0:
             warnings.warn('[sersic] Nonpositive flux at r_e.', AstropyUserWarning)
-            self.flag_sersic = 1
+            self.flag_sersic = 2
             ellip_annulus_mean_flux = np.abs(ellip_annulus_mean_flux)
 
         # Final parameter
         if 'amplitude' not in self._sersic_model_args:
             self._sersic_model_args['amplitude'] = ellip_annulus_mean_flux
 
         # Create initial model
         if self._psf is None:
             sersic_init = models.Sersic2D(**self._sersic_model_args)
         else:
             sersic_init = ConvolvedSersic2D(**self._sersic_model_args)
             sersic_init.set_psf(self._psf)
 
+        # Dummy value (in case calculations are aborted)
+        self._sersic_chi2 = -99.0
+
         # Prepare data for fitting
         z = image.copy()
-        y, x = np.mgrid[0:ny, 0:nx]
+        y, x = np.float64(np.mgrid[0:ny, 0:nx])
         weightmap = self._weightmap_stamp
         # Exclude pixels with image == 0 or weightmap == 0 from the fit.
         fit_weights = np.zeros_like(z)
         locs = (image != 0) & (weightmap != 0)
         # The sky background noise is already included in the weightmap:
         fit_weights[locs] = 1.0 / weightmap[locs]
+        # Number of "valid" pixels
+        num_validpixels = np.sum(locs)
 
-        # The number of data points cannot be smaller than the number of
-        # free parameters (7 in the case of Sersic2D)
-        if z.size < sersic_init.parameters.size:
+        # Calculate number of free parameters and degrees of freedom
+        num_freeparam = sersic_init.parameters.size  # 7 for Sersic2D
+        for kwarg in ['fixed', 'tied']:
+            if kwarg in self._sersic_model_args:
+                for param, value in self._sersic_model_args[kwarg].items():
+                    if value:
+                        num_freeparam -= 1
+        assert num_freeparam >= 0
+        self._sersic_num_dof = num_validpixels - num_freeparam
+        if self._sersic_num_dof <= 0:
             warnings.warn('[sersic] Not enough data for fit.',
                           AstropyUserWarning)
-            self.flag_sersic = 1
+            self.flag_sersic = 2
             return sersic_init
 
         # Since model fitting can be computationally expensive (especially
         # with a large PSF), only do it when the other measurements are OK.
         if self.flag >= 2:
             warnings.warn('[sersic] Skipping Sersic fit...',
                           AstropyUserWarning)
-            self.flag_sersic = 1
+            self.flag_sersic = 2
             return sersic_init
 
         # Try to fit model
         fit_sersic = fitting.LevMarLSQFitter()
         sersic_model = fit_sersic(sersic_init, x, y, z=z, weights=fit_weights,
                                   **self._sersic_fitting_args)
         if fit_sersic.fit_info['ierr'] not in [1, 2, 3, 4]:
-            warnings.warn("fit_info['message']: " + fit_sersic.fit_info['message'],
+            warnings.warn("[sersic] fit_info['message']: "
+                          + fit_sersic.fit_info['message'],
                           AstropyUserWarning)
-            self.flag_sersic = 1
+            self.flag_sersic = 2
 
-        # Make sure the effective radius is positive:
-        if sersic_model.r_eff.value <= 0:
-            warnings.warn('[sersic] Nonpositive effective radius?',
-                          AstropyUserWarning)
-            self.flag_sersic = 1
-            return sersic_init
+        # If any of the parameters gets "stuck" to a boundary, label the
+        # fit as "suspect" (flag_sersic = 1).
+        if 'bounds' in self._sersic_model_args:
+            for param, bounds in self._sersic_model_args['bounds'].items():
+                value = getattr(sersic_model, param).value
+                if value in bounds:
+                    if self._verbose:
+                        warnings.warn(
+                            f"[sersic] {param} got stuck at {value}.",
+                            AstropyUserWarning)
+                    self.flag_sersic = max(self.flag_sersic, 1)
+
+        # Apply post-fitting corrections (if applicable)
+        (sersic_model.r_eff.value,
+         sersic_model.ellip.value,
+         sersic_model.theta.value) = _postfitting_fix(
+            sersic_model.r_eff.value,
+            sersic_model.ellip.value,
+            sersic_model.theta.value)
 
-        # In some rare cases, the fitted ellipticity is outside the
-        # range [0, 1]. While we could constrain this parameter during
-        # the fit using the ``bounds`` keyword argument in `Sersic2D`, a less
-        # aggressive solution is to create an equivalent model as follows:
-        if sersic_model.ellip.value > 1:
-            # Note that the semiminor axis is given by
-            # b = (1 - ellip) * a.
-            # This would yield a negative value for b, but since only b^2
-            # appears in the code, we can define an equivalent ellipticity as
-            # 1 - ellip' = -(1 - ellip)  =>  ellip' = 2 - ellip.
-            sersic_model.ellip.value = 2.0 - sersic_model.ellip.value
-        if sersic_model.ellip.value < 0:
-            # This can be interpreted as a, b being flipped (a < b), so we
-            # switch them and define an equivalent ellipticity as
-            # 1 - ellip' = 1 / (1 - ellip)  =>  ellip' = ellip / (ellip - 1).
-            e = sersic_model.ellip.value
-            sersic_model.r_eff.value = (1 - e) * sersic_model.r_eff.value
-            sersic_model.ellip.value = e / (e - 1)
-            # We also need to rotate the model by 90 degrees:
-            sersic_model.theta.value += np.pi/2
-        # Finally, note that the two cases above are not mutually exclusive.
-        # If a Sersic model has ellipticity > 2, then both "corrections" are
-        # applied successively.
+        # Calculate chi^2 statistic of the fitted model.
+        self._sersic_chi2 = np.sum((fit_weights * (z - sersic_model(x, y)))**2)
+
+        # Save runtime
+        self.sersic_runtime = time.time() - start
 
         return sersic_model
 
     @lazyproperty
     def sersic_amplitude(self):
         """
         The amplitude of the 2D Sersic fit at the effective (half-light)
@@ -2538,14 +2711,280 @@
         """
         The orientation (counterclockwise, in radians) of the
         2D Sersic fit (`astropy.modeling.models.Sersic2D`).
         """
         theta = self._sersic_model.theta.value
         return theta - np.floor(theta/np.pi) * np.pi
 
+    @lazyproperty
+    def sersic_chi2_dof(self):
+        """
+        Reduced chi^2 statistic of the fitted model.
+        """
+        _ = self._sersic_model
+        if self._sersic_chi2 == -99.0:
+            return -99.0
+
+        return self._sersic_chi2 / self._sersic_num_dof
+
+    ###########################
+    # DOUBLE SERSIC MODEL FIT #
+    ###########################
+
+    @lazyproperty
+    def _doublesersic_model(self):
+        """
+        Fit a double 2D Sersic profile using Astropy's model fitting library.
+        An initial guess for the model is automatically generated based on
+        other statmorph measurements, although users can provide their own
+        initial values (and optionally keep them fixed) via the
+        ``doublesersic_model_args`` keyword argument.
+
+        Return the fitted model object.
+        """
+        image = self._cutout_stamp_maskzeroed
+        ny, nx = image.shape
+
+        # Measure runtime
+        start = time.time()
+
+        # Create initial guesses for the model parameters
+        if 'x_0' not in self._doublesersic_model_args:
+            self._doublesersic_model_args['x_0'] = self.sersic_xc
+        if 'y_0' not in self._doublesersic_model_args:
+            self._doublesersic_model_args['y_0'] = self.sersic_yc
+        if 'amplitude_1' not in self._doublesersic_model_args:
+            self._doublesersic_model_args['amplitude_1'] = (
+                self.sersic_amplitude / 2)
+        if 'r_eff_1' not in self._doublesersic_model_args:
+            self._doublesersic_model_args['r_eff_1'] = self.sersic_rhalf
+        if 'n_1' not in self._doublesersic_model_args:
+            self._doublesersic_model_args['n_1'] = 4.0  # de Vaucouleurs
+        if 'ellip_1' not in self._doublesersic_model_args:
+            self._doublesersic_model_args['ellip_1'] = self.sersic_ellip
+        if 'theta_1' not in self._doublesersic_model_args:
+            self._doublesersic_model_args['theta_1'] = self.sersic_theta
+        if 'amplitude_2' not in self._doublesersic_model_args:
+            self._doublesersic_model_args['amplitude_2'] = (
+                self.sersic_amplitude / 2)
+        if 'r_eff_2' not in self._doublesersic_model_args:
+            self._doublesersic_model_args['r_eff_2'] = self.sersic_rhalf
+        if 'n_2' not in self._doublesersic_model_args:
+            self._doublesersic_model_args['n_2'] = 1.0  # exponential
+        if 'ellip_2' not in self._doublesersic_model_args:
+            self._doublesersic_model_args['ellip_2'] = self.sersic_ellip
+        if 'theta_2' not in self._doublesersic_model_args:
+            self._doublesersic_model_args['theta_2'] = self.sersic_theta
+
+        # Origin must coincide with that of image cutout
+        self._doublesersic_model_args['x_0'] -= self.xmin_stamp
+        self._doublesersic_model_args['y_0'] -= self.ymin_stamp
+
+        # Create initial model
+        if self._psf is None:
+            doublesersic_init = DoubleSersic2D(**self._doublesersic_model_args)
+        else:
+            doublesersic_init = ConvolvedDoubleSersic2D(**self._doublesersic_model_args)
+            doublesersic_init.set_psf(self._psf)
+
+        # Tie ellipticity and position angle of the two components
+        if self._doublesersic_tied_ellip:
+            doublesersic_init.ellip_2.tied = lambda model: model.ellip_1
+            doublesersic_init.theta_2.tied = lambda model: model.theta_1
+
+        # Dummy value (in case calculations are aborted)
+        self._doublesersic_chi2 = -99.0
+
+        # Prepare data for fitting
+        z = image.copy()
+        y, x = np.float64(np.mgrid[0:ny, 0:nx])
+        weightmap = self._weightmap_stamp
+        # Exclude pixels with image == 0 or weightmap == 0 from the fit.
+        fit_weights = np.zeros_like(z)
+        locs = (image != 0) & (weightmap != 0)
+        # The sky background noise is already included in the weightmap:
+        fit_weights[locs] = 1.0 / weightmap[locs]
+        # Number of "valid" pixels
+        num_validpixels = np.sum(locs)
+
+        # Calculate number of free parameters and degrees of freedom
+        num_freeparam = doublesersic_init.parameters.size  # 12 for DoubleSersic2D
+        for kwarg in ['fixed', 'tied']:
+            if kwarg in self._doublesersic_model_args:
+                for param, value in self._doublesersic_model_args[kwarg].items():
+                    if value:
+                        num_freeparam -= 1
+        assert num_freeparam >= 0
+        self._doublesersic_num_dof = num_validpixels - num_freeparam
+        if self._doublesersic_num_dof <= 0:
+            warnings.warn('[doublesersic] Not enough data for fit.',
+                          AstropyUserWarning)
+            self.flag_doublesersic = 2
+            return doublesersic_init
+
+        # Since model fitting can be computationally expensive (especially
+        # with a large PSF), only do it when the other measurements are OK.
+        if self.flag >= 2:
+            warnings.warn('[doublesersic] Skipping double Sersic fit...',
+                          AstropyUserWarning)
+            self.flag_doublesersic = 2
+            return doublesersic_init
+
+        # Try to fit model
+        fit_doublesersic = fitting.LevMarLSQFitter()
+        doublesersic_model = fit_doublesersic(
+            doublesersic_init, x, y, z=z, weights=fit_weights,
+            **self._doublesersic_fitting_args)
+        if fit_doublesersic.fit_info['ierr'] not in [1, 2, 3, 4]:
+            warnings.warn("[doublesersic] fit_info['message']: "
+                          + fit_doublesersic.fit_info['message'],
+                          AstropyUserWarning)
+            self.flag_doublesersic = 2
+
+        # If any of the parameters gets "stuck" to a boundary, label the
+        # fit as "suspect" (flag_doublesersic = 1).
+        if 'bounds' in self._doublesersic_model_args:
+            for param, bounds in self._doublesersic_model_args['bounds'].items():
+                value = getattr(doublesersic_model, param).value
+                if value in bounds:
+                    if self._verbose:
+                        warnings.warn(
+                            f"[doublesersic] {param} got stuck at {value}.",
+                            AstropyUserWarning)
+                    self.flag_doublesersic = max(self.flag_doublesersic, 1)
+
+        # Apply post-fitting corrections (if applicable)
+        (doublesersic_model.r_eff_1.value,
+         doublesersic_model.ellip_1.value,
+         doublesersic_model.theta_1.value) = _postfitting_fix(
+            doublesersic_model.r_eff_1.value,
+            doublesersic_model.ellip_1.value,
+            doublesersic_model.theta_1.value)
+        (doublesersic_model.r_eff_2.value,
+         doublesersic_model.ellip_2.value,
+         doublesersic_model.theta_2.value) = _postfitting_fix(
+            doublesersic_model.r_eff_2.value,
+            doublesersic_model.ellip_2.value,
+            doublesersic_model.theta_2.value)
+
+        # Calculate chi^2 statistic of the fitted model.
+        self._doublesersic_chi2 = np.sum((fit_weights * (z - doublesersic_model(x, y)))**2)
+
+        # Save runtime
+        self.doublesersic_runtime = time.time() - start
+
+        return doublesersic_model
+
+    @lazyproperty
+    def doublesersic_xc(self):
+        """
+        The x-coordinate of the center of the double 2D Sersic fit,
+        relative to the original image.
+        """
+        return self.xmin_stamp + self._doublesersic_model.x_0.value
+
+    @lazyproperty
+    def doublesersic_yc(self):
+        """
+        The y-coordinate of the center of the double 2D Sersic fit,
+        relative to the original image.
+        """
+        return self.ymin_stamp + self._doublesersic_model.y_0.value
+
+    @lazyproperty
+    def doublesersic_amplitude1(self):
+        """
+        The amplitude of the first component of the double 2D Sersic fit
+        at its effective radius (rhalf1).
+        """
+        return self._doublesersic_model.amplitude_1.value
+
+    @lazyproperty
+    def doublesersic_rhalf1(self):
+        """
+        The effective (half-light) radius of the first component of the
+        double 2D Sersic fit.
+        """
+        return self._doublesersic_model.r_eff_1.value
+
+    @lazyproperty
+    def doublesersic_n1(self):
+        """
+        The Sersic index ``n`` of the first component of the double 2D
+        Sersic fit.
+        """
+        return self._doublesersic_model.n_1.value
+
+    @lazyproperty
+    def doublesersic_ellip1(self):
+        """
+        The ellipticity of the first component of the double 2D Sersic fit.
+        """
+        return self._doublesersic_model.ellip_1.value
+
+    @lazyproperty
+    def doublesersic_theta1(self):
+        """
+        The orientation (counterclockwise, in radians) of the
+        first component of the double 2D Sersic fit.
+        """
+        theta = self._doublesersic_model.theta_1.value
+        return theta - np.floor(theta/np.pi) * np.pi
+
+    @lazyproperty
+    def doublesersic_amplitude2(self):
+        """
+        The amplitude of the second component of the double 2D Sersic fit
+        at its effective radius (rhalf2).
+        """
+        return self._doublesersic_model.amplitude_2.value
+
+    @lazyproperty
+    def doublesersic_rhalf2(self):
+        """
+        The effective (half-light) radius of the second component of the
+        double 2D Sersic fit.
+        """
+        return self._doublesersic_model.r_eff_2.value
+
+    @lazyproperty
+    def doublesersic_n2(self):
+        """
+        The Sersic index ``n`` of the second component of the double 2D
+        Sersic fit.
+        """
+        return self._doublesersic_model.n_2.value
+
+    @lazyproperty
+    def doublesersic_ellip2(self):
+        """
+        The ellipticity of the second component of the double 2D Sersic fit.
+        """
+        return self._doublesersic_model.ellip_2.value
+
+    @lazyproperty
+    def doublesersic_theta2(self):
+        """
+        The orientation (counterclockwise, in radians) of the
+        second component of the double 2D Sersic fit.
+        """
+        theta = self._doublesersic_model.theta_2.value
+        return theta - np.floor(theta/np.pi) * np.pi
+
+    @lazyproperty
+    def doublesersic_chi2_dof(self):
+        """
+        Reduced chi^2 statistic of the fitted double 2D Sersic model.
+        """
+        _ = self._doublesersic_model
+        if self._doublesersic_chi2 == -99.0:
+            return -99.0
+
+        return self._doublesersic_chi2 / self._doublesersic_num_dof
+
 
 def source_morphology(image, segmap, **kwargs):
     """
     Calculate the morphological parameters of all sources in ``image``
     as labeled by ``segmap``.
 
     Parameters
```

### Comparing `statmorph-0.5.1/statmorph/tests/data/slice.fits` & `statmorph-0.5.2/statmorph/tests/data/slice.fits`

 * *Files identical despite different names*

### Comparing `statmorph-0.5.1/statmorph/tests/test_statmorph.py` & `statmorph-0.5.2/statmorph/tests/test_statmorph.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 # Author: Vicente Rodriguez-Gomez <vrodgom.astro@gmail.com>
 # Licensed under a 3-Clause BSD License.
 import numpy as np
 import os
 import pytest
 import statmorph
-from astropy.modeling import models
+from astropy.modeling.models import Sersic2D
 from astropy.io import fits
 from astropy.utils.exceptions import AstropyUserWarning
 from numpy.testing import assert_allclose
 
 __all__ = ['runall']
 
 
@@ -30,25 +30,24 @@
     with pytest.raises(ValueError):
         _ = _quantile(data, -0.5)
         _ = _quantile(data, 1.5)
 
 
 def test_convolved_sersic():
     from scipy.signal import fftconvolve
+    from astropy.convolution import Gaussian2DKernel
     # Create Gaussian PSF.
-    size = 10  # on each side from the center
-    sigma_psf = 2.0
-    y, x = np.mgrid[-size:size + 1, -size:size + 1]
-    psf = np.exp(-(x ** 2 + y ** 2) / (2.0 * sigma_psf ** 2))
-    psf /= np.sum(psf)
+    kernel = Gaussian2DKernel(2.0)
+    kernel.normalize()  # make sure kernel adds up to 1
+    psf = kernel.array  # we only need the numpy array
     # Create 2D Sersic profile.
     ny, nx = 25, 25
     y, x = np.mgrid[0:ny, 0:nx]
-    sersic = models.Sersic2D(amplitude=1, r_eff=5, n=1.5, x_0=12, y_0=12,
-                             ellip=0.5, theta=0)
+    sersic = Sersic2D(
+        amplitude=1, r_eff=5, n=1.5, x_0=12, y_0=12, ellip=0.5, theta=0)
     z = sersic(x, y)
     # Create "convolved" Sersic profile with same properties as normal one.
     convolved_sersic = statmorph.ConvolvedSersic2D(
         amplitude=1, r_eff=5, n=1.5, x_0=12, y_0=12, ellip=0.5, theta=0)
     with pytest.raises(AssertionError):
         _ = convolved_sersic(x, y)  # PSF not set yet
     convolved_sersic.set_psf(psf)
@@ -155,15 +154,15 @@
     image = np.zeros((2, 3), dtype=np.float64)
     image[:, 1] = 1.0
     segmap = np.int64(image)
     with pytest.warns() as w:
         morph = statmorph.SourceMorphology(image, segmap, label, gain=1.0,
                                            n_sigma_outlier=-1)
     assert w[-2].category == AstropyUserWarning
-    assert '[sersic] Not enough data for fit.' in str(w[-2].message)
+    assert 'Not enough data for fit.' in str(w[-2].message)
     assert morph.flag == 2
 
 
 def test_asymmetric():
     """
     Test a case in which the asymmetry center is pushed outside of
     the image boundaries.
@@ -252,16 +251,16 @@
     label = 1
     ny, nx = 11, 11
     y, x = np.mgrid[0:ny, 0:nx]
     image = np.exp(-((x - nx // 2) ** 2 + (y - ny // 2) ** 2) / 50)
     segmap = np.int64(image > 0.5)
     with pytest.warns() as w:
         morph = statmorph.SourceMorphology(image, segmap, label, gain=1.0)
-    assert w[-3].category == AstropyUserWarning
-    assert 'Full Gini segmap!' in str(w[-3].message)
+    assert w[2].category == AstropyUserWarning
+    assert 'Full Gini segmap!' in str(w[2].message)
     assert morph.flag == 2
 
 
 def test_merger():
     """
     Test a "merger" scenario. This manages to produce different Gini
     and MID segmaps, as well as a failed Sersic fit.
@@ -323,64 +322,82 @@
             'sersic_amplitude': 1296.95288208155739,
             'sersic_rhalf': 22.45788866502031,
             'sersic_n': 0.61206828194077,
             'sersic_xc': 81.56197595338546,
             'sersic_yc': 80.40465135599014,
             'sersic_ellip': 0.05083866217150,
             'sersic_theta': 2.47831542907976,
+            'sersic_chi2_dof': 1.3376238276749,
+            'doublesersic_xc': 81.532553358593,
+            'doublesersic_yc': 80.536548408219,
+            'doublesersic_amplitude1': 977.16534068311,
+            'doublesersic_rhalf1': 22.484298765876,
+            'doublesersic_n1': 0.79327851914927,
+            'doublesersic_ellip1': 0.080276873646978,
+            'doublesersic_theta1': 2.2974159066311,
+            'doublesersic_amplitude2': 317.68798626787,
+            'doublesersic_rhalf2': 25.935143308214,
+            'doublesersic_n2': 0.01,
+            'doublesersic_ellip2': 0.1426514566223,
+            'doublesersic_theta2': 0.41940953820527,
+            'doublesersic_chi2_dof': 1.2682460649336,
             'sky_mean': 3.48760604858398,
             'sky_median': -2.68543863296509,
             'sky_sigma': 150.91754150390625,
             'xmin_stamp': 0,
             'ymin_stamp': 0,
             'xmax_stamp': 161,
             'ymax_stamp': 161,
             'nx_stamp': 162,
             'ny_stamp': 162,
             'flag': 0,
             'flag_sersic': 0,
+            'flag_doublesersic': 2,
         }
 
         # Run statmorph on the same galaxy from which the above values
         # were obtained.
         curdir = os.path.dirname(__file__)
         with fits.open('%s/data/slice.fits' % (curdir,)) as hdulist:
             self.image = hdulist[0].data
             self.segmap = hdulist[1].data
             self.mask = np.bool_(hdulist[2].data)
         self.gain = 1.0
 
     def test_no_psf(self, print_values=False):
         source_morphs = statmorph.source_morphology(
-            self.image, self.segmap, mask=self.mask, gain=self.gain)
+            self.image, self.segmap, mask=self.mask, gain=self.gain,
+            include_doublesersic=True)
         morph = source_morphs[0]
         for key in self.correct_values:
             assert_allclose(morph[key], self.correct_values[key],
                             err_msg="%s value did not match." % (key,))
             if print_values:
                 print("'%s': %.14g," % (key, morph[key]))
 
     def test_psf(self):
         # Try delta-like PSF, which should give the same results as no PSF.
         psf = np.array([[0, 0, 0],
                         [0, 1, 0],
                         [0, 0, 0]], dtype=np.float64)
         source_morphs = statmorph.source_morphology(
-            self.image, self.segmap, mask=self.mask, gain=self.gain, psf=psf)
+            self.image, self.segmap, mask=self.mask, gain=self.gain, psf=psf,
+            include_doublesersic=True)
         morph = source_morphs[0]
         for key in self.correct_values:
             assert_allclose(morph[key], self.correct_values[key],
                             err_msg="%s value did not match." % (key,))
 
     def test_weightmap(self):
         # Manually create weight map instead of using the gain argument.
         weightmap = np.sqrt(
             np.abs(self.image) / self.gain + self.correct_values['sky_sigma']**2)
         source_morphs = statmorph.source_morphology(
-            self.image, self.segmap, mask=self.mask, weightmap=weightmap)
+            self.image, self.segmap, mask=self.mask, weightmap=weightmap,
+            include_doublesersic=True)
         morph = source_morphs[0]
         for key in self.correct_values:
             assert_allclose(morph[key], self.correct_values[key],
                             err_msg="%s value did not match." % (key,))
 
 
 def runall(print_values=False):
```

### Comparing `statmorph-0.5.1/statmorph/utils/image_diagnostics.py` & `statmorph-0.5.2/statmorph/utils/image_diagnostics.py`

 * *Files identical despite different names*

### Comparing `statmorph-0.5.1/statmorph/utils/tests/test_image_diagnostics.py` & `statmorph-0.5.2/statmorph/utils/tests/test_image_diagnostics.py`

 * *Files identical despite different names*

### Comparing `statmorph-0.5.1/statmorph.egg-info/PKG-INFO` & `statmorph-0.5.2/statmorph.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: statmorph
-Version: 0.5.1
+Version: 0.5.2
 Summary: Non-parametric morphological diagnostics of galaxy images
 Home-page: https://github.com/vrodgom/statmorph
 Author: Vicente Rodriguez-Gomez
 Author-email: vrodgom.astro@gmail.com
 License: BSD
 Keywords: astronomy galaxies galaxy-morphology non-parametric
 Classifier: Development Status :: 4 - Beta
```

