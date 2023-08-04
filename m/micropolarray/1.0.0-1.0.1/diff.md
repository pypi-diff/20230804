# Comparing `tmp/micropolarray-1.0.0.tar.gz` & `tmp/micropolarray-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "micropolarray-1.0.0.tar", last modified: Wed Jun 21 09:37:31 2023, max compression
+gzip compressed data, was "micropolarray-1.0.1.tar", last modified: Fri Aug  4 15:54:19 2023, max compression
```

## Comparing `micropolarray-1.0.0.tar` & `micropolarray-1.0.1.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxrwxr-x   0 herve     (1000) herve     (1000)        0 2023-06-21 09:37:31.199768 micropolarray-1.0.0/
--rw-rw-r--   0 herve     (1000) herve     (1000)     1494 2023-02-09 16:24:14.000000 micropolarray-1.0.0/LICENSE
--rw-rw-r--   0 herve     (1000) herve     (1000)     3571 2023-06-21 09:37:31.199768 micropolarray-1.0.0/PKG-INFO
--rw-rw-r--   0 herve     (1000) herve     (1000)     1235 2023-06-20 15:13:24.000000 micropolarray-1.0.0/README.md
-drwxrwxr-x   0 herve     (1000) herve     (1000)        0 2023-06-21 09:37:31.199768 micropolarray-1.0.0/build/
-drwxrwxr-x   0 herve     (1000) herve     (1000)        0 2023-06-21 09:37:31.199768 micropolarray-1.0.0/build/lib/
-drwxrwxr-x   0 herve     (1000) herve     (1000)        0 2023-06-21 09:37:31.199768 micropolarray-1.0.0/build/lib/micropolarray/
--rw-rw-r--   0 herve     (1000) herve     (1000)     1260 2023-06-07 07:29:37.000000 micropolarray-1.0.0/build/lib/micropolarray/__init__.py
--rw-rw-r--   0 herve     (1000) herve     (1000)     3906 2023-06-08 16:48:19.000000 micropolarray-1.0.0/build/lib/micropolarray/cameras.py
--rw-rw-r--   0 herve     (1000) herve     (1000)     8236 2023-06-08 16:07:08.000000 micropolarray-1.0.0/build/lib/micropolarray/image.py
--rw-rw-r--   0 herve     (1000) herve     (1000)    32981 2023-06-15 16:16:38.000000 micropolarray-1.0.0/build/lib/micropolarray/micropol_image.py
--rw-rw-r--   0 herve     (1000) herve     (1000)     1096 2023-02-09 16:24:14.000000 micropolarray-1.0.0/build/lib/micropolarray/parallelize.py
--rw-rw-r--   0 herve     (1000) herve     (1000)     1405 2023-02-23 09:57:19.000000 micropolarray-1.0.0/build/lib/micropolarray/polarization_functions.py
-drwxrwxr-x   0 herve     (1000) herve     (1000)        0 2023-06-21 09:37:31.199768 micropolarray-1.0.0/build/lib/micropolarray/processing/
--rw-rw-r--   0 herve     (1000) herve     (1000)       13 2023-02-09 16:24:14.000000 micropolarray-1.0.0/build/lib/micropolarray/processing/__init__.py
--rw-rw-r--   0 herve     (1000) herve     (1000)    11209 2023-02-23 09:22:33.000000 micropolarray-1.0.0/build/lib/micropolarray/processing/chen_wan_liang_calibration.py
--rw-rw-r--   0 herve     (1000) herve     (1000)     2099 2023-02-09 16:24:14.000000 micropolarray-1.0.0/build/lib/micropolarray/processing/congrid.py
--rw-rw-r--   0 herve     (1000) herve     (1000)     3990 2023-06-08 15:41:06.000000 micropolarray-1.0.0/build/lib/micropolarray/processing/convert.py
--rw-rw-r--   0 herve     (1000) herve     (1000)    28155 2023-02-09 16:24:14.000000 micropolarray-1.0.0/build/lib/micropolarray/processing/demodulation.py
--rw-rw-r--   0 herve     (1000) herve     (1000)     5248 2023-06-13 08:37:05.000000 micropolarray-1.0.0/build/lib/micropolarray/processing/demosaic.py
--rw-rw-r--   0 herve     (1000) herve     (1000)    27860 2023-06-20 13:09:02.000000 micropolarray-1.0.0/build/lib/micropolarray/processing/new_demodulation.py
--rw-rw-r--   0 herve     (1000) herve     (1000)    10922 2023-06-08 16:52:50.000000 micropolarray-1.0.0/build/lib/micropolarray/processing/nrgf.py
--rw-rw-r--   0 herve     (1000) herve     (1000)     4019 2023-06-20 13:38:20.000000 micropolarray-1.0.0/build/lib/micropolarray/processing/rebin.py
--rw-rw-r--   0 herve     (1000) herve     (1000)     7903 2023-06-13 13:43:50.000000 micropolarray-1.0.0/build/lib/micropolarray/utils.py
-drwxrwxr-x   0 herve     (1000) herve     (1000)        0 2023-06-21 09:37:31.199768 micropolarray-1.0.0/micropolarray.egg-info/
--rw-rw-r--   0 herve     (1000) herve     (1000)     3571 2023-06-21 09:37:31.000000 micropolarray-1.0.0/micropolarray.egg-info/PKG-INFO
--rw-rw-r--   0 herve     (1000) herve     (1000)      969 2023-06-21 09:37:31.000000 micropolarray-1.0.0/micropolarray.egg-info/SOURCES.txt
--rw-rw-r--   0 herve     (1000) herve     (1000)        1 2023-06-21 09:37:31.000000 micropolarray-1.0.0/micropolarray.egg-info/dependency_links.txt
--rw-rw-r--   0 herve     (1000) herve     (1000)      118 2023-06-21 09:37:31.000000 micropolarray-1.0.0/micropolarray.egg-info/requires.txt
--rw-rw-r--   0 herve     (1000) herve     (1000)       14 2023-06-21 09:37:31.000000 micropolarray-1.0.0/micropolarray.egg-info/top_level.txt
--rw-rw-r--   0 herve     (1000) herve     (1000)      888 2023-06-21 09:35:02.000000 micropolarray-1.0.0/pyproject.toml
--rw-rw-r--   0 herve     (1000) herve     (1000)       38 2023-06-21 09:37:31.199768 micropolarray-1.0.0/setup.cfg
--rw-rw-r--   0 herve     (1000) herve     (1000)     1057 2023-06-21 09:35:06.000000 micropolarray-1.0.0/setup.py
+drwxrwxr-x   0 herve     (1000) herve     (1000)        0 2023-08-04 15:54:19.792335 micropolarray-1.0.1/
+-rw-rw-r--   0 herve     (1000) herve     (1000)     1494 2023-02-09 16:24:14.000000 micropolarray-1.0.1/LICENSE
+-rw-rw-r--   0 herve     (1000) herve     (1000)     3786 2023-08-04 15:54:19.792335 micropolarray-1.0.1/PKG-INFO
+-rw-rw-r--   0 herve     (1000) herve     (1000)     1449 2023-07-13 09:31:03.000000 micropolarray-1.0.1/README.md
+drwxrwxr-x   0 herve     (1000) herve     (1000)        0 2023-08-04 15:54:19.788335 micropolarray-1.0.1/build/
+drwxrwxr-x   0 herve     (1000) herve     (1000)        0 2023-08-04 15:54:19.788335 micropolarray-1.0.1/build/lib/
+drwxrwxr-x   0 herve     (1000) herve     (1000)        0 2023-08-04 15:54:19.788335 micropolarray-1.0.1/build/lib/micropolarray/
+-rw-rw-r--   0 herve     (1000) herve     (1000)     1366 2023-07-27 08:14:18.000000 micropolarray-1.0.1/build/lib/micropolarray/__init__.py
+-rw-rw-r--   0 herve     (1000) herve     (1000)     4034 2023-07-31 15:10:17.000000 micropolarray-1.0.1/build/lib/micropolarray/cameras.py
+-rw-rw-r--   0 herve     (1000) herve     (1000)     9979 2023-08-04 15:17:18.000000 micropolarray-1.0.1/build/lib/micropolarray/image.py
+-rw-rw-r--   0 herve     (1000) herve     (1000)    38213 2023-08-04 15:52:07.000000 micropolarray-1.0.1/build/lib/micropolarray/micropol_image.py
+-rw-rw-r--   0 herve     (1000) herve     (1000)     1096 2023-02-09 16:24:14.000000 micropolarray-1.0.1/build/lib/micropolarray/parallelize.py
+-rw-rw-r--   0 herve     (1000) herve     (1000)     1960 2023-08-04 15:43:35.000000 micropolarray-1.0.1/build/lib/micropolarray/polarization_functions.py
+drwxrwxr-x   0 herve     (1000) herve     (1000)        0 2023-08-04 15:54:19.792335 micropolarray-1.0.1/build/lib/micropolarray/processing/
+-rw-rw-r--   0 herve     (1000) herve     (1000)       13 2023-02-09 16:24:14.000000 micropolarray-1.0.1/build/lib/micropolarray/processing/__init__.py
+-rw-rw-r--   0 herve     (1000) herve     (1000)    11209 2023-02-23 09:22:33.000000 micropolarray-1.0.1/build/lib/micropolarray/processing/chen_wan_liang_calibration.py
+-rw-rw-r--   0 herve     (1000) herve     (1000)     2132 2023-08-04 13:32:36.000000 micropolarray-1.0.1/build/lib/micropolarray/processing/congrid.py
+-rw-rw-r--   0 herve     (1000) herve     (1000)     5540 2023-08-01 08:46:30.000000 micropolarray-1.0.1/build/lib/micropolarray/processing/convert.py
+-rw-rw-r--   0 herve     (1000) herve     (1000)    28032 2023-08-04 13:35:35.000000 micropolarray-1.0.1/build/lib/micropolarray/processing/demodulation.py
+-rw-rw-r--   0 herve     (1000) herve     (1000)     5248 2023-08-03 14:05:05.000000 micropolarray-1.0.1/build/lib/micropolarray/processing/demosaic.py
+-rw-rw-r--   0 herve     (1000) herve     (1000)    30697 2023-08-04 15:50:34.000000 micropolarray-1.0.1/build/lib/micropolarray/processing/new_demodulation.py
+-rw-rw-r--   0 herve     (1000) herve     (1000)    12486 2023-08-03 09:22:12.000000 micropolarray-1.0.1/build/lib/micropolarray/processing/nrgf.py
+-rw-rw-r--   0 herve     (1000) herve     (1000)     5732 2023-08-04 10:19:02.000000 micropolarray-1.0.1/build/lib/micropolarray/processing/rebin.py
+-rw-rw-r--   0 herve     (1000) herve     (1000)     1133 2023-07-26 07:55:50.000000 micropolarray-1.0.1/build/lib/micropolarray/processing/shift.py
+-rw-rw-r--   0 herve     (1000) herve     (1000)     9460 2023-08-04 13:46:47.000000 micropolarray-1.0.1/build/lib/micropolarray/utils.py
+drwxrwxr-x   0 herve     (1000) herve     (1000)        0 2023-08-04 15:54:19.792335 micropolarray-1.0.1/micropolarray.egg-info/
+-rw-rw-r--   0 herve     (1000) herve     (1000)     3786 2023-08-04 15:54:19.000000 micropolarray-1.0.1/micropolarray.egg-info/PKG-INFO
+-rw-rw-r--   0 herve     (1000) herve     (1000)     1015 2023-08-04 15:54:19.000000 micropolarray-1.0.1/micropolarray.egg-info/SOURCES.txt
+-rw-rw-r--   0 herve     (1000) herve     (1000)        1 2023-08-04 15:54:19.000000 micropolarray-1.0.1/micropolarray.egg-info/dependency_links.txt
+-rw-rw-r--   0 herve     (1000) herve     (1000)      118 2023-08-04 15:54:19.000000 micropolarray-1.0.1/micropolarray.egg-info/requires.txt
+-rw-rw-r--   0 herve     (1000) herve     (1000)       14 2023-08-04 15:54:19.000000 micropolarray-1.0.1/micropolarray.egg-info/top_level.txt
+-rw-rw-r--   0 herve     (1000) herve     (1000)      889 2023-08-04 14:06:43.000000 micropolarray-1.0.1/pyproject.toml
+-rw-rw-r--   0 herve     (1000) herve     (1000)       38 2023-08-04 15:54:19.792335 micropolarray-1.0.1/setup.cfg
+-rw-rw-r--   0 herve     (1000) herve     (1000)     1057 2023-08-04 14:06:36.000000 micropolarray-1.0.1/setup.py
```

### Comparing `micropolarray-1.0.0/LICENSE` & `micropolarray-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `micropolarray-1.0.0/PKG-INFO` & `micropolarray-1.0.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micropolarray
-Version: 1.0.0
+Version: 1.0.1
 Summary: micropolarizer array data utilities
 Home-page: https://github.com/Hevil33/micropolarray_master
 Author: Hervé Haudemand
 Author-email: Herve Haudemand <herve.haudemand@inaf.it>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, Hevil33
@@ -35,15 +35,15 @@
         OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
         
 Project-URL: Homepage, https://github.com/Hevil33/micropolarray_master
 Keywords: micropolarizer,polarcam,polarization
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.9
+Requires-Python: >=3.0
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # micropolarray
 
 Python module for loading and using micropolarizer array and polarcam images.
@@ -90,7 +90,15 @@
 pol_0_image = image.single_pol_subimages[image.angle_dic[0]]
 
 demosaiced_image = image.demosaic() 
 
 binned_image = image.rebin(binning=4)  # binned 4x4 image
 
 ```
+
+If demodulation matrices are available, it is easy to get demodulated images
+
+```
+
+demodulator = ml.Demodulator(demodulation_tensor_path)
+
+demo_image = image.demodulate(demodulator) # This image is now demodulated
```

### Comparing `micropolarray-1.0.0/README.md` & `micropolarray-1.0.1/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -44,7 +44,15 @@
 pol_0_image = image.single_pol_subimages[image.angle_dic[0]]
 
 demosaiced_image = image.demosaic() 
 
 binned_image = image.rebin(binning=4)  # binned 4x4 image
 
 ```
+
+If demodulation matrices are available, it is easy to get demodulated images
+
+```
+
+demodulator = ml.Demodulator(demodulation_tensor_path)
+
+demo_image = image.demodulate(demodulator) # This image is now demodulated
```

### Comparing `micropolarray-1.0.0/build/lib/micropolarray/__init__.py` & `micropolarray-1.0.1/build/lib/micropolarray/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,35 @@
 from micropolarray.image import Image
-from micropolarray.micropol_image import MicroPolarizerArrayImage
+from micropolarray.micropol_image import (
+    MicroPolarizerArrayImage,
+    set_default_angles,
+)
 from micropolarray.cameras import PolarCam, Kasi, Antarticor
 
 from micropolarray.processing.new_demodulation import Demodulator
 from micropolarray.processing.new_demodulation import (
     calculate_demodulation_tensor,
 )
 from micropolarray.processing.nrgf import (
     find_occulter_position,
     roi_from_polar,
     nrgf,
 )
 from micropolarray.processing.convert import (
     convert_set,
     convert_rawfile_to_fits,
+    average_rawfiles_to_fits,
 )
 from micropolarray.processing.demosaic import demosaic
 from micropolarray.utils import (
     sigma_DN,
     mean_minus_std,
     mean_plus_std,
+    median_minus_std,
+    median_plus_std,
     get_Bsun_units,
     get_malus_normalization,
 )
 from micropolarray.processing.chen_wan_liang_calibration import (
     chen_wan_liang_calibration,
     ifov_jitcorrect,
 )
```

### Comparing `micropolarray-1.0.0/build/lib/micropolarray/cameras.py` & `micropolarray-1.0.1/build/lib/micropolarray/cameras.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import numpy as np
 from micropolarray.processing.nrgf import roi_from_polar
 
+# TODO: aggiungere tutti i bei dati qua, rendere le camere personalizzabili (caricare dark da cartelle e cose cosi)
+
 
 class Camera:
     def __init__(self):
         pass
 
     def occulter_roi(
         self, data: np.array, fill: float = 0.0, overoccult: int = 0
@@ -49,20 +51,16 @@
             False,
         )
         return occulter_mask
 
 
 class Kasi(Camera):
     def __init__(self):
-        self.angle_dic = {
-            -45: 0,
-            0: 1,
-            90: 2,
-            45: 3,
-        }
+        # self.angle_dic = {-45: 0, 0: 1, 90: 2, 45: 3}  # old
+        self.angle_dic = {0: 0, 45: 1, -45: 2, 90: 3}  # new
         self.linearity_range = [0.0, 2500.0]
         self.PTC = 2.64  # [e-/ADU]
         self.readout_noise = 10  # [e-]
         self.full_well = 10500  # [e-]
         self.h_image = 3000
         self.w_image = 4096
```

### Comparing `micropolarray-1.0.0/build/lib/micropolarray/image.py` & `micropolarray-1.0.1/build/lib/micropolarray/image.py`

 * *Files 20% similar despite different names*

```diff
@@ -31,24 +31,31 @@
         self._set_data(np.array(data))
         self.filename = "image.fits"
 
     def _init_image_from_file(self, filenames, averageimages) -> None:
         filenames_list = (
             [filenames] if type(filenames) is not list else filenames
         )
+
         filenames_len = len(filenames_list)
         if filenames_len == 0:
             raise NameError("Can't load files, empty filenames list.")
         datetimes = [0] * filenames_len
 
         print_info_message = True
         for idx, filename in enumerate(filenames_list):
+            if ".raw" in filenames_list:
+                raise NameError(
+                    "Can't load a raw file, convert it to fits first."
+                )  # to fix
             with fits.open(filename) as hul:
                 if idx == 0:
-                    combined_data = hul[0].data
+                    combined_data = hul[0].data / (
+                        1 + int(averageimages) * (filenames_len - 1)
+                    )
                     self.header = hul[0].header
                 else:
                     if print_info_message:
                         if averageimages:
                             info(f"Averaging {filenames_len} images...")
                         else:
                             info(f"Summing {filenames_len} images...")
@@ -126,17 +133,26 @@
         self.header["NAXIS2"] = data.shape[0]
 
     # ----------------------------------------------------------------
     # -------------------------- SAVING ------------------------------
     # ----------------------------------------------------------------
 
     def save_as_fits(self, filename: str, fixto: str[float, float] = None):
-        """Save image as fits file with current instance header."""
+        """Saves image as fits with current header
+
+        Args:
+            filename (str): output filename
+            fixto (str[float, float], optional): Set a maximum and minimum range for the data. Defaults to None.
+
+        Raises:
+            ValueError: filename does not end with ".fits"
+        """
         filepath = Path(filename)
-        if not filepath.suffix:
+        if filepath.suffix != ".fits":
+            print(filepath.suffix)
             raise ValueError("filename must be a valid file name, not folder.")
         filepath = Path(make_abs_and_create_dir(filename))
         if fixto:
             data = fix_data(self.data, *fixto)
         else:
             data = self.data
         hdu = fits.PrimaryHDU(
@@ -147,23 +163,47 @@
         )
         filename = str(
             filepath.joinpath(filepath.parent, filepath.stem + ".fits")
         )
         hdu.writeto(filename, overwrite=True)
         info(f'Image successfully saved to "{filename}".')
 
+    def save_as_raw(self, filename: str):
+        """Saves the image as a raw binary file
+
+        Args:
+            filename (str): output filename
+
+        Raises:
+            ValueError: filename does not end with ".raw"
+        """
+        print(self.data.shape)
+        if Path(filename).suffix is not ".raw":
+            raise ValueError("Filename must have .raw extension")
+        self.data.astype("int16").tofile(filename)
+
     # ----------------------------------------------------------------
     # ------------------------------ SHOW ----------------------------
     # ----------------------------------------------------------------
 
-    def show(self, cmap="Greys_r", vmin=None, vmax=None):
-        """Shows image data with colorbar."""
+    def show(self, cmap="Greys_r", vmin=None, vmax=None) -> tuple:
+        """Shows the image data
+
+        Args:
+            cmap (str, optional): figure colorbar. Defaults to "Greys_r".
+            vmin (_type_, optional): Minimum value to plot. Defaults to None.
+            vmax (_type_, optional): Maximum value to plot. Defaults to None.
+
+        Returns:
+            tuple: fig, ax tuple as returned by matplotlib.pyplot.subplots
+        """
         data_to_plot = self.data
         data_ratio = data_to_plot.shape[0] / data_to_plot.shape[1]
-        image_fig, imageax = plt.subplots(figsize=(9, 9))
+        # image_fig, imageax = plt.subplots(figsize=(9, 9))
+        image_fig, imageax = plt.subplots(dpi=200)
         if vmin is None:
             vmin = np.min(data_to_plot)
         if vmax is None:
             vmax = np.max(data_to_plot)
         pos = imageax.imshow(data_to_plot, cmap=cmap, vmin=vmin, vmax=vmax)
         imageax.set_title(
             f"Image data (avrg {np.mean(data_to_plot, where=np.where(data_to_plot>0, True, False)):3.2f}+-{np.std(data_to_plot, where=np.where(data_to_plot>0, True, False)):3.2f})",
@@ -173,45 +213,52 @@
         imageax.set_ylabel("y")
         image_fig.colorbar(
             pos, ax=imageax, label="DN", fraction=data_ratio * 0.05
         )
 
         return image_fig, imageax
 
-    def show_histogram(self, bins: int = 1000):
-        """Shows a histogram of the image"""
-        fig, ax = plt.subplots(figsize=(9, 9))
+    def show_histogram(self, bins: int = 1000) -> tuple:
+        """Print the histogram of the flattened image data
+
+        Args:
+            bins (int, optional): Numbers of bin to compute the histogram from. Defaults to 1000.
+
+        Returns:
+            tuple: fig, ax tuple as returned by matplotlib.pyplot.subplots
+        """
+        fig, ax = plt.subplots(dpi=200, constrained_layout=True)
         histo = np.histogram(self.data, bins=bins)
         ax.stairs(*histo)
         ax.set_title("Image histogram", color="black")
         ax.set_xlabel("Signal [DN]")
         ax.set_ylabel("Number of pixels")
 
         return fig, ax
 
-    def __add__(self, second):
+    def __add__(self, second) -> Image:
         if type(self) is type(second):
             newdata = self.data + second.data
         else:
             newdata = self.data + second
         return Image(newdata)
 
-    def __sub__(self, second):
+    def __sub__(self, second) -> Image:
         if type(self) is type(second):
             newdata = self.data - second.data
         else:
             newdata = self.data - second
         return Image(newdata)
 
-    def __mul__(self, second):
+    def __mul__(self, second) -> Image:
         if type(self) is type(second):
             newdata = self.data * second.data
         else:
             newdata = self.data * second
         return Image(newdata)
 
-    def __truediv__(self, second):
+    def __truediv__(self, second) -> Image:
         if type(self) is type(second):
-            newdata = self.data / second.data
+            newdata = np.where(second.data != 0, self.data / second.data, 4096)
         else:
-            newdata = self.data / second
+            newdata = np.where(second != 0, self.data / second, 4096)
         return Image(newdata)
```

### Comparing `micropolarray-1.0.0/build/lib/micropolarray/micropol_image.py` & `micropolarray-1.0.1/build/lib/micropolarray/micropol_image.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,77 +7,92 @@
 from micropolarray.image import Image
 from micropolarray.processing.demosaic import (
     demosaic,
     split_polarizations,
     merge_polarizations,
 )
 from micropolarray.processing.rebin import (
-    micropolarray_jitrebin,
-    trim_to_match_2xbinning,
-    standard_jitrebin,
+    micropolarray_rebin,
 )
-from micropolarray.cameras import PolarCam
+from micropolarray.cameras import PolarCam, Camera
 from micropolarray.processing.new_demodulation import Demodulator
 from micropolarray.utils import make_abs_and_create_dir, fix_data
 from micropolarray.processing.congrid import congrid
 from PIL import Image as PILImage
 from pathlib import Path
 from logging import warning, debug, info, error
 from micropolarray.processing.chen_wan_liang_calibration import (
     ifov_jitcorrect,
 )
 from micropolarray.processing.nrgf import roi_from_polar
 from micropolarray.utils import mean_minus_std, mean_plus_std, timer
+from micropolarray.processing.shift import shift, shift_micropol
 
 
 @dataclass
 class PolParam:
     """Auxiliary class for polarization parameters.
+
     Members:
-      ID (str): parameter identifier
-      data (np.array): parameter image as numpy 2D array
-      title (str): brief title of the parameter, useful for plotting
-      measure_unit (str): initial measure units of the parameter
-      fix_data (bool): controls whether data has to be constrained to [0, 4096] interval (not implemented yet)
+        ID (str): parameter identifier
+        data (np.array): parameter image as numpy 2D array
+        title (str): brief title of the parameter, useful for plotting
+        measure_unit (str): initial measure units of the parameter
+        fix_data (bool): controls whether data has to be constrained to [0, 4096] interval (not implemented yet)
     """
 
     ID: str
     data: np.ndarray
     title: str
     measure_unit: str
     fix_data: bool
 
 
+DEFAULT_ANGLES_DIC = None  # sets the micropolarizer orientations with a dictionary {angle : position in superpix 1->3}
+
+
+def set_default_angles(angles_dic: dict):
+    """Sets the default micropolarizer orientations for images.
+
+    Args:
+        angles_dic (dict): dictionary {value : pos} where value is the angle in degrees from -90 to 90 and pos is the pixel position in superpixel, from 0 to 3 (position [y, x], fast index x)
+    """
+    global DEFAULT_ANGLES_DIC
+    DEFAULT_ANGLES_DIC = angles_dic
+
+
 class MicroPolarizerArrayImage(Image):
     """Micro-polarizer array image class. Can be initialized from a 2d array, a list of 1 or more file names (use the boolean keyword averageimages to select if sum or average is taken) or another MicroPolarizerArrayImage. Dark and flat micropolarray images can also be provided to automatically correct the result."""
 
     first_call = True  # Avoid repeating messages
-    default_angle_dic = PolarCam().angle_dic
 
     def __init__(
         self,
         initializer: str | np.ndarray | list | MicroPolarizerArrayImage,
         angle_dic: dict = None,
-        demosaic_mode: str = "mean",
+        demosaic_mode: str = "adjacent",
         dark: MicroPolarizerArrayImage = None,
         flat: MicroPolarizerArrayImage = None,
         averageimages: bool = True,
     ):
         self._is_demodulated = False
         self._is_demosaiced = False
         self._binning = 1
         self._flat_subtracted = False
         self._dark_subtracted = False
         if angle_dic is None:
-            if MicroPolarizerArrayImage.first_call:
-                warning(
-                    f"No dictionary provided for micropolarizer orientations, defaulting to {MicroPolarizerArrayImage.default_angle_dic}\n"
-                )
+            global DEFAULT_ANGLES_DIC
+            if DEFAULT_ANGLES_DIC is None:
+                if MicroPolarizerArrayImage.first_call:
+                    warning(
+                        f"Micropolarizer orientation dictionary defaults to {PolarCam().angle_dic}, set it via set_default_angles(camera)\n"
+                    )
                 MicroPolarizerArrayImage.first_call = False
-            angle_dic = MicroPolarizerArrayImage.default_angle_dic
+                DEFAULT_ANGLES_DIC = PolarCam().angle_dic
+            angle_dic = DEFAULT_ANGLES_DIC
         self.angle_dic = angle_dic
         self.demosaic_mode = demosaic_mode
         self.demosaiced_images = None
 
         if type(initializer) is str and len(initializer) > 1:
             self._num_of_images = len(initializer)
         else:
@@ -183,14 +198,25 @@
             self.U,
             self.pB,
             self.AoLP,
             self.DoLP,
         ]
 
     def demodulate(self, demodulator: Demodulator) -> MicroPolarizerArrayImage:
+        """Returns a MicroPolarizerArrayImage with polarization parameters calculated from the demodulation tensor provided.
+
+        Args:
+            demodulator (Demodulator): Demodulator object containing the demodulation tensor components (see processing.new_demodulation)
+
+        Raises:
+            ValueError: raised if image and demodulator do not have the same dimension, for example in case of different binning
+
+        Returns:
+            MicroPolarizerArrayImage: copy of the input image with I, Q, U, pB, DoLP, AoLP calculated from the demodulation tensor.
+        """
         if (self.height, self.width) != (
             demodulator.mij.shape[2],
             demodulator.mij.shape[3],
         ):
             print(demodulator.mij.shape[2], demodulator.mij.shape[3])
             print(self.height, self.width)
             raise ValueError(
@@ -201,20 +227,23 @@
         demodulated_image.Stokes_vec = (
             demodulated_image._get_Stokes_from_demodulator(demodulator)
         )
         demodulated_image._update_single_pol_subimages()
         demodulated_image._update_stokes_derived_internal_dataclasses()
         demodulated_image._is_demodulated = True
 
+        info("Image correctly demodulated")
         return demodulated_image
 
     def set_data_only(self, data: np.array = None) -> None:
         if data is None:
             data = self.data
         self.data = data
+        self.height = data.shape[0]
+        self.width = data.shape[1]
         if (data.shape[0] % 2) or (data.shape[1] % 2):
             warning(
                 "Odd number of pixels is incompatible"
                 " with micropolarizer arrays operations."
             )
         self._update_single_pol_subimages()
         if self._is_demosaiced:
@@ -240,32 +269,23 @@
         self.height, self.width = data.shape
         self._update_single_pol_subimages()
 
         if not self._is_demosaiced:
             self.Stokes_vec = self._get_theo_Stokes_vec_components(
                 self.single_pol_subimages
             )
+            self._update_stokes_derived_internal_dataclasses()
         else:
             self.demosaic()
             self.Stokes_vec = self._get_theo_Stokes_vec_components(
                 self.demosaiced_images
             )
-        self._update_stokes_derived_internal_dataclasses()
 
     def _update_single_pol_subimages(self) -> None:
-        single_pol_subimages = np.array(
-            [self.data[j::2, i::2] for j in range(2) for i in range(2)],
-            # [
-            #    self.data[0::2, 0::2], # x= 0, y = 0
-            #    self.data[0::2, 1::2], # x= 1, y = 0
-            #    self.data[1::2, 0::2], # x= 0, y = 1
-            #    self.data[1::2, 1::2], # x= 1, y = 1
-            # ],
-            dtype=np.float,
-        )
+        single_pol_subimages = split_polarizations(self.data)
 
         self.single_pol_subimages = single_pol_subimages
         self.pol0 = PolParam(
             "0",
             single_pol_subimages[self.angle_dic[0]],
             "0 deg orientation pixels",
             "DN",
@@ -377,58 +397,81 @@
 
         S = np.array([I, Q, U], dtype=float)
         return S
 
     def subtract_dark(
         self, dark: MicroPolarizerArrayImage
     ) -> MicroPolarizerArrayImage:
-        """Subtracts dark data from image data."""
+        """Correctly subtracts the input dark image from the image
+
+        Args:
+            dark (MicroPolarizerArrayImage): dark to subtract
+
+        Returns:
+            MicroPolarizerArrayImage: copy of input image with dark subtracted
+        """
         self.data = self.data - dark.data
         self.data = np.where(self.data >= 0, self.data, 0)  # Fix data
         self._set_data_and_Stokes()
         self._dark_subtracted = True
         return self
 
     def correct_flat(
         self, flat: MicroPolarizerArrayImage
     ) -> MicroPolarizerArrayImage:
-        """Divides image data by flat data."""
+        """Normalizes the flat and uses it to correct the image.
+
+        Args:
+            flat (MicroPolarizerArrayImage): flat image, does not need to be normalized.
+
+        Returns:
+            MicroPolarizerArrayImage: copy of input image corrected by flat
+        """
         normalized_flat = flat.data / np.max(flat.data)
         self.data = np.where(
             normalized_flat != 0, self.data / normalized_flat, self.data
         )
         # self.data = np.where(self.data >= 0, self.data, 0)
         # self.data = np.where(self.data < 4096, self.data, 4096)
         self._set_data_and_Stokes()
         self._flat_subtracted = True
         return self
 
     def correct_ifov(self) -> MicroPolarizerArrayImage:
+        """Corrects differences in single pixels fields of view inside each superpixel
+
+        Returns:
+            MicroPolarizerArrayImage: image with data corrected for field of view differences
+        """
         corrected_data = self.data.copy()
         corrected_data = ifov_jitcorrect(self.data, self.height, self.width)
         self._set_data_and_Stokes(corrected_data)
         return self
 
     # ----------------------------------------------------------------
     # ------------------------------ SHOW ----------------------------
     # ----------------------------------------------------------------
 
-    def show_with_pol_params(self, cmap="Greys_r"):
+    def show_with_pol_params(self, cmap="Greys_r") -> tuple:
         """Returns a fig for each set of image parameters. User must call
         plt.show after this is called.
         Returned parameters:
         - Original image
         - Stokes vector I, Q, U
-        - Angle, degree of linear polarizaimagetion
-        - Polarized brightness
+        - Angle, degree of linear polarizaimagetion Polarized brightness
+
+
+        Args:
+            cmap (str, optional): colormap string. Defaults to "Greys_r".
+
+        Returns:
+            tuple: a (figure, axis) couple same as matplotlib.pyplot.subplots for the image data and another for the six polarization parameters
         """
         data_ratio = self.data.shape[0] / self.data.shape[1]
-        image_fig, imageax = plt.subplots(
-            figsize=(10, 9), constrained_layout=True
-        )
+        image_fig, imageax = plt.subplots(dpi=200, constrained_layout=True)
         mappable = imageax.imshow(
             self.data,
             cmap=cmap,
             vmin=mean_minus_std(self.data),
             vmax=mean_plus_std(self.data),
         )
         avg = np.mean(self.data)
@@ -441,15 +484,14 @@
         imageax.set_ylabel("y [px]")
         image_fig.colorbar(
             mappable, ax=imageax, label="[DN]", fraction=data_ratio * 0.05
         )
         stokes_fig, stokesax = plt.subplots(
             2, 3, figsize=(14, 9), constrained_layout=True
         )
-        # stokes_fig.tight_layout()
 
         stokesax = stokesax.ravel()
         for i, stokes in enumerate(stokesax):
             vmin = mean_minus_std(self.polparam_list[i].data)
             vmax = mean_plus_std(self.polparam_list[i].data)
             avg = np.mean(self.polparam_list[i].data)
             stdev = np.std(self.polparam_list[i].data)
@@ -468,14 +510,22 @@
                 ax=stokes,
                 label=self.polparam_list[i].measure_unit,
                 fraction=data_ratio * 0.05,
             )
         return image_fig, imageax, stokes_fig, stokesax
 
     def show_single_pol_images(self, cmap="Greys_r"):
+        """Plots the four polarizations images.
+
+        Args:
+            cmap (str, optional): colormap for the plot. Defaults to "Greys_r".
+
+        Returns:
+            tuple: a (figure, axis) couple same as matplotlib.pyplot.subplots
+        """
         data_ratio = self.data.shape[0] / self.data.shape[1]
         fig, ax = plt.subplots(2, 2, figsize=(9, 9), constrained_layout=True)
         ax = ax.ravel()
         polslist = [self.pol0, self.pol45, self.pol90, self.pol_45]
         for i, singlepolax in enumerate(ax):
             mappable = singlepolax.imshow(polslist[i].data, cmap=cmap)
             singlepolax.set_title(polslist[i].title)
@@ -487,14 +537,22 @@
                 label=polslist[i].measure_unit,
                 fraction=data_ratio * 0.05,
                 pad=0.01,
             )
         return fig, ax
 
     def show_demo_images(self, cmap="Greys_r"):
+        """Plots the four demosaiced images.
+
+        Args:
+            cmap (str, optional): colormap for the plot. Defaults to "Greys_r".
+
+        Returns:
+            tuple: a (figure, axis) couple same as matplotlib.pyplot.subplots
+        """
         if not self._is_demosaiced:
             error("Image is not yet demosaiced.")
         data_ratio = self.data.shape[0] / self.data.shape[1]
         fig, ax = plt.subplots(2, 2, figsize=(9, 9), constrained_layout=True)
         ax = ax.ravel()
         demo_images_list = self.demosaiced_images
         for i, single_demo_ax in enumerate(ax):
@@ -515,16 +573,25 @@
                 label="DN",
                 fraction=data_ratio * 0.05,
                 pad=0.01,
             )
         return fig, ax
 
     def show_pol_param(self, polparam: PolParam, cmap="Greys_r"):
+        """Plots a single polarization parameter given as input
+
+        Args:
+            polparam (PolParam): image PolParam containing the parameter to plot. Can be one among [self.I, self.Q, self.U, self.pB, self.AoLP, self.DoLP]
+            cmap (str, optional): colormap for the plot. Defaults to "Greys_r".
+
+        Returns:
+            tuple: a (figure, axis) couple same as matplotlib.pyplot.subplots
+        """
         data_ratio = self.data.shape[0] / self.data.shape[1]
-        fig, ax = plt.subplots(figsize=(9, 9))
+        fig, ax = plt.subplots(dpi=200)
         mappable = ax.imshow(
             polparam.data,
             cmap=cmap,
             vmin=mean_minus_std(polparam.data),
             vmax=mean_plus_std(polparam.data),
         )
         ax.set_title(polparam.title)
@@ -541,17 +608,26 @@
     # ----------------------------------------------------------------
     # -------------------------- SAVING ------------------------------
     # ----------------------------------------------------------------
 
     def save_single_pol_images(
         self, filename: str, fixto: list[float, float] = None
     ) -> None:
+        """Saves the four polarized images as fits files
+
+        Args:
+            filename (str): filename of the output image. The four images will be saved as filename_POLXX.fits
+            fixto (list[float, float], optional): set the minimum and maximum value for the output images. Defaults to None.
+
+        Raises:
+            ValueError: an invalid file name is provided
+        """
         polslist = [self.pol0, self.pol45, self.pol90, self.pol_45]
         filepath = Path(make_abs_and_create_dir(filename))
-        if not filepath.suffix:
+        if filepath.suffix != ".fits":
             raise ValueError("filename must be a valid file name, not folder.")
         group_filepath = filepath.joinpath(filepath.parent, filepath.stem)
         for single_pol in polslist:
             hdr = self.header.copy()
             hdr["POL"] = (single_pol.ID, "Micropolarizer orientation")
             if fixto:
                 data = fix_data(single_pol.data, *fixto)
@@ -573,16 +649,26 @@
 
     def save_param_as_fits(
         self,
         filename: str,
         polparam: PolParam,
         fixto: list[float, float] = None,
     ) -> None:
+        """Saves chosen polarization parameter as a fits file
+
+        Args:
+            filename (str): filename of the output image.
+            polparam (PolParam): polarization parameter to save. Can be one among [self.I, self.Q, self.U, self.pB, self.AoLP, self.DoLP]
+            fixto (list[float, float], optional): set the minimum and maximum value for the output images. Defaults to None.
+
+        Raises:
+            ValueError: filename is not a valid .fits file
+        """
         filepath = Path(make_abs_and_create_dir(filename))
-        if not filepath.suffix:
+        if filepath.suffix != ".fits":
             raise ValueError("filename must be a valid file name, not folder.")
         hdr = self.header.copy()
         hdr["PARAM"] = (str(polparam.title), "Polarization parameter")
         hdr["UNITS"] = (str(polparam.measure_unit), "Measure units")
         if fixto:
             data = fix_data(polparam.data, *fixto)
         else:
@@ -603,16 +689,24 @@
         # filename_with_ID = (
         #    filename.split(".")[-2] + "_" + polparam.ID + ".fits"
         # )
         hdu.writeto(filename_with_ID, overwrite=True)
         info(f'"{filename_with_ID}" {polparam.ID} successfully saved')
 
     def save_all_pol_params_as_fits(self, filename: str) -> None:
+        """Saves the image and all polarization parameters as fits file with the same name
+
+        Args:
+            filename (str): filename of the output image. Will be saved as filename_[I, Q, U, pB, AoLP, DoLP].fits
+
+        Raises:
+            ValueError: filename is not a valid .fits file
+        """
         filepath = Path(filename)
-        if not filepath.suffix:
+        if filepath.suffix != ".fits":
             raise ValueError("filename must be a valid file name, not folder.")
         filepath = Path(make_abs_and_create_dir(filename))
         group_filename = str(filepath.joinpath(filepath.parent, filepath.stem))
         for param in self.polparam_list:
             hdr = self.header.copy()
             hdr["PARAM"] = (str(param.title), "Polarization parameter")
             hdr["UNITS"] = (str(param.measure_unit), "Measure units")
@@ -629,14 +723,23 @@
             filename_with_ID = group_filename + "_" + param.ID + ".fits"
             hdu.writeto(filename_with_ID, overwrite=True)
         info(f'All params successfully saved to "{group_filename}"')
 
     def save_demosaiced_images_as_fits(
         self, filename: str, fixto: list[float, float] = None
     ) -> None:
+        """Saves the four demosaiced images as fits files
+
+        Args:
+            filename (str): filename of the output image. The four images will be saved as filename_POLXX.fits
+            fixto (list[float, float], optional): set the minimum and maximum value for the output images. Defaults to None.
+
+        Raises:
+            ValueError: an invalid file name is provided
+        """
         if not self._is_demosaiced:
             raise ValueError("Demosaiced images not yet calculated.")
         imageHdr = self.header.copy()
         filepath = Path(filename)
         if not filepath.suffix:
             raise ValueError("filename must be a valid file name, not folder.")
         filepath = Path(make_abs_and_create_dir(filename))
@@ -662,56 +765,51 @@
             f'Demosaiced images successfully saved to "{group_filename}_POLX.fits"'
         )
 
     # ----------------------------------------------------------------
     # -------------------- DATA MANIPULATION -------------------------
     # ----------------------------------------------------------------
     def demosaic(self) -> MicroPolarizerArrayImage:
+        """Returns a demosaiced copy of the image with updated polarization parameters.
+
+        Returns:
+            MicroPolarizerArrayImage: demosaiced image
+        """
         self.demosaiced_images = demosaic(self.data, option=self.demosaic_mode)
         self.Stokes_vec = self._get_theo_Stokes_vec_components(
             self.demosaiced_images
         )
         self._update_stokes_derived_internal_dataclasses()
         self._is_demosaiced = True
 
         return self
 
     def rebin(self, binning: int) -> MicroPolarizerArrayImage:
         """Rebins the micropolarizer array image, binned each
-        binningxbinning. Sum bins by default."""
+        binningxbinning. Sum bins by default.
+
+        Args:
+            binning (int): binning to perform. A value of n will be translated in a nxn binning.
+
+        Raises:
+            ValueError: negative binning provided
+
+        Returns:
+            MicroPolarizerArrayImage: copy of the input image, rebinned.
+        """
         if binning <= 0:
             raise ValueError(f"Negative binning {binning}x{binning}")
         rebinned_image = MicroPolarizerArrayImage(self)
-        rebinned_data = micropolarray_jitrebin(
+        rebinned_data = micropolarray_rebin(
             np.array(rebinned_image.data, dtype=np.double),
-            rebinned_image.width,
-            rebinned_image.height,
+            *rebinned_image.data.shape,
             binning,
         )
-        rebinned_image.set_data_only(rebinned_data)
 
-        # find a better way to do this
-        rebinned_image.I.data = standard_jitrebin(
-            self.I.data, *self.I.data.shape, binning=binning
-        )
-        rebinned_image.Q.data = standard_jitrebin(
-            self.Q.data, *self.Q.data.shape, binning=binning
-        )
-        rebinned_image.U.data = standard_jitrebin(
-            self.U.data, *self.U.data.shape, binning=binning
-        )
-        rebinned_image.pB.data = standard_jitrebin(
-            self.pB.data, *self.pB.data.shape, binning=binning
-        )
-        rebinned_image.AoLP.data = standard_jitrebin(
-            self.AoLP.data, *self.AoLP.data.shape, binning=binning
-        )
-        rebinned_image.DoLP.data = standard_jitrebin(
-            self.DoLP.data, *self.DoLP.data.shape, binning=binning
-        )
+        rebinned_image._set_data_and_Stokes(rebinned_data)
 
         return rebinned_image
 
     def congrid(
         self, newdim_y: int, newdim_x: int
     ) -> MicroPolarizerArrayImage:
         # Trim to nearest superpixel
@@ -765,26 +863,26 @@
     def mask_occulter(
         self,
         y: int = PolarCam().occulter_pos_last[0],
         x: int = PolarCam().occulter_pos_last[1],
         r: int = PolarCam().occulter_pos_last[2],
         overoccult: int = 0,
         camera=PolarCam(),
-    ):
+    ) -> None:
         """Masks occulter for all image parameters
 
         Args:
             y (int, optional): Occulter y position. Defaults to PolarCam().occulter_pos_last[0].
             x (int, optional): Occulter x position. Defaults to PolarCam().occulter_pos_last[1].
             r (int, optional): Occulter radius. Defaults to PolarCam().occulter_pos_last[2].
             overoccult (int, optional): Pixels to overoccult. Defaults to 0.
             camera (_type_, optional): Camera image type. Defaults to PolarCam().
 
         Returns:
-            _type_: _description_
+            None
         """
         # y, x, r = camera.occulter_pos_last
 
         relative_y = y / camera.h_image
         relative_x = x / camera.w_image
         relative_r = (r + overoccult) / camera.h_image
 
@@ -831,37 +929,66 @@
                         * (param.data.shape[0] + param.data.shape[1])
                         / 2
                     ),
                     2 * np.max((param.data.shape[0], param.data.shape[0])),
                 ],
             )
 
+    def shift(self, y: int, x: int) -> MicroPolarizerArrayImage:
+        """Shifts image by y, x pixels and fills with 0 the remaining space. Positive numbers for up/right shift and negative for down/left shift. Image is split into polarizations, each one is shifted, then they are merged again.
+
+        Args:
+            y (int): vertical shift in pix
+            x (int): horizontal shift in pix
+
+        Returns:
+            MicroPolarizerArrayImage: shifted image copied from the original
+        """
+        # newdata = shift(self.data, y, x)
+        newdata = shift_micropol(self.data, y, x)
+        newimage = MicroPolarizerArrayImage(self)
+        newimage._set_data_and_Stokes(newdata)
+
+        return newimage
+
     # ----------------------------------------------------------------
     # ------------------------ OVERLOADING ---------------------------
     # ----------------------------------------------------------------
     def __add__(self, second) -> MicroPolarizerArrayImage:
         if type(self) is type(second):
             newdata = self.data + second.data
+            newimage = MicroPolarizerArrayImage(self)
+            newimage._set_data_and_Stokes(newdata)
+            return newimage
         else:
             newdata = self.data + second
-        return MicroPolarizerArrayImage(newdata, angle_dic=self.angle_dic)
+            return MicroPolarizerArrayImage(newdata, angle_dic=self.angle_dic)
 
     def __sub__(self, second) -> MicroPolarizerArrayImage:
         if type(self) is type(second):
             newdata = self.data - second.data
+            newimage = MicroPolarizerArrayImage(self)
+            newimage._set_data_and_Stokes(newdata)
+            return newimage
         else:
             newdata = self.data - second
-        return MicroPolarizerArrayImage(newdata, angle_dic=self.angle_dic)
+            return MicroPolarizerArrayImage(newdata, angle_dic=self.angle_dic)
 
     def __mul__(self, second) -> MicroPolarizerArrayImage:
         if type(self) is type(second):
             newdata = self.data * second.data
+            newimage = MicroPolarizerArrayImage(self)
+            newimage._set_data_and_Stokes(newdata)
+            return newimage
         else:
             newdata = self.data * second
-        return MicroPolarizerArrayImage(newdata, angle_dic=self.angle_dic)
+            return MicroPolarizerArrayImage(newdata, angle_dic=self.angle_dic)
 
     def __truediv__(self, second) -> MicroPolarizerArrayImage:
         if type(self) is type(second):
             newdata = np.where(second.data != 0, self.data / second.data, 4096)
+            newimage = MicroPolarizerArrayImage(self)
+            newimage._set_data_and_Stokes(newdata)
+            return newimage
         else:
-            newdata = np.where(second > 0, self.data / second, 4096)
-        return MicroPolarizerArrayImage(newdata, angle_dic=self.angle_dic)
+            newdata = np.where(second != 0, self.data / second, 4096)
+            return MicroPolarizerArrayImage(newdata, angle_dic=self.angle_dic)
```

### Comparing `micropolarray-1.0.0/build/lib/micropolarray/parallelize.py` & `micropolarray-1.0.1/build/lib/micropolarray/parallelize.py`

 * *Files identical despite different names*

### Comparing `micropolarray-1.0.0/build/lib/micropolarray/polarization_functions.py` & `micropolarray-1.0.1/build/lib/micropolarray/polarization_functions.py`

 * *Files 21% similar despite different names*

```diff
@@ -11,35 +11,53 @@
         Stokes_vec_components (numpy.array[3, number of y pixels, number of x pixels]): array containing elements of the Stokes vector of an np.array[y, x] image, in the form [S0, S1, S2].
 """
 
 
 def AoLP(Stokes_vec_components):
     """Angle of linear polarization in [rad]"""
     I, Q, U = Stokes_vec_components
-    return 0.5 * np.arctan2(U, Q)
+    angle = 0.5 * np.arctan(
+        np.divide(1.0 * U, 1.0 * Q, out=np.zeros_like(U), where=Q != 0),
+        dtype=float,
+    )  # avoids warning when dividing by 0
+    return angle
+    angle = np.where(
+        Q != 0,
+        0.5 * np.arctan(1.0 * U / (1.0 * Q), dtype=float),
+        np.deg2rad(90.0),
+    )  # set it to 90 deg when denominator explodes
+    return angle
 
 
 def DoLP(Stokes_vec_components):
     """Degree of linear polarization in [%]"""
     I, Q, U = Stokes_vec_components
     return np.divide(
-        np.sqrt((Q * Q) + (U * U)), I, where=(I != 0)
+        np.sqrt((Q * Q) + (U * U), dtype=float), I, where=(I != 0)
     )  # avoids 0/0 error
 
 
 def pB(Stokes_vec_components):
     """Polarized brighness in [%]"""
     I, Q, U = Stokes_vec_components
-    return np.sqrt((Q * Q) + (U * U))
+    return np.sqrt((Q * Q) + (U * U), dtype=float)
 
 
 """----------------------------------------------------------------------"""
 
 
 def normalize2pi(angles_list):
+    """Normalizes the input angle list in the -90,90 range
+
+    Args:
+        angles_list (_type_): list of input angles in degrees
+
+    Returns:
+        _type_: normalized angles
+    """
     if type(angles_list) is not list:
         angles_list = [
             angles_list,
         ]
     for i, angle in enumerate(angles_list):
         while angle > 90:
             angle -= 180
```

### Comparing `micropolarray-1.0.0/build/lib/micropolarray/processing/chen_wan_liang_calibration.py` & `micropolarray-1.0.1/build/lib/micropolarray/processing/chen_wan_liang_calibration.py`

 * *Files identical despite different names*

### Comparing `micropolarray-1.0.0/build/lib/micropolarray/processing/congrid.py` & `micropolarray-1.0.1/build/lib/micropolarray/processing/congrid.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,24 +25,24 @@
 
 
 def interpolate(x, x_0, y_0, x_1, y_1):
     return (x - x_0) * ((y_1 - y_0) / (x_1 - x_0)) + y_0
 
 
 # Copied from IDL congrid, arbitrary reshape
-def congrid(a, newdims, kind="linear"):
+def congrid(a, newdims, kind="linear") -> np.ndarray:
     """Reshapes the data into any new lenght and width
 
     Args:
         a (np.array): data to be reshaped
         newdims (tuple | list): new lenght and width
         kind (str, optional): interpolation type. Defaults to "linear".
 
     Returns:
-        _type_: _description_
+        ndarray: numpy array of congridded image
     """
     if not a.dtype in [np.float64, np.float32]:
         a = np.cast[float](a)
 
     m1 = np.cast[int](True)
     old = np.array(a.shape)
     ndims = len(a.shape)
```

### Comparing `micropolarray-1.0.0/build/lib/micropolarray/processing/convert.py` & `micropolarray-1.0.1/build/lib/micropolarray/processing/convert.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import multiprocessing as mp
 from astropy.io import fits
 import sys
 import tqdm
 import datetime
 import pytz
 from logging import critical, info
+from pathlib import Path
 
 
 def three_bytes_to_two_ints(filecontent):
     """Needed for parallelization, this will be run by each thread for a slice of the original array.
 
     Returns:
         np.array: array of saved data
@@ -60,42 +61,82 @@
     )
     with mp.Pool(processes=chunks_n) as p:
         result = p.map(three_bytes_to_two_ints, splitted)
     newarr = np.array(result).reshape((1952, 1952))
     return newarr
 
 
-def convert_set(filenames, new_filename):
-    """Sums a set of filenames and converts them to one fits file.
+def convert_set(filenames, new_filename, height, width):
+    """ANTARTICOR ONLY: Sums a set of filenames and converts them to one fits file.
+
 
     Args:
         filenames (list): list of file names to be summed before being converted
         new_filename (str): new .fits file name
     """
-    if new_filename.split(".")[-1] != "fits":
+    abs_new_filename = os.path.abspath(new_filename)
+    if abs_new_filename.split(".")[-1] != "fits":
         raise ValueError(
             "Trying to save a .fits file to .bin, check new filename"
         )
     if type(filenames) is not list:
         filenames = [
             filenames,
         ]
     images_n = len(filenames)
-    arr = np.zeros(shape=(1952, 1952))
+    arr = np.zeros(shape=(height, width))
     for filename in tqdm.tqdm(filenames):
         arr += nparr_from_binary(filename) / images_n
     hdu = fits.PrimaryHDU(data=arr)
     date_and_time = datetime.datetime.now(
         tz=pytz.timezone("Australia/Perth")
     ).strftime("%Y-%m-%dT%H:%M:%S%z")
     hdu.header["CREATED"] = (
         str(date_and_time),
         "Datetime conversion from bin to fits file (Dome C timezone).",
     )
-    hdu.writeto(new_filename, overwrite=True)
+    hdu.writeto(abs_new_filename, overwrite=True)
+
+
+def average_rawfiles_to_fits(
+    filenames: list, new_filename: str, height: int, width: int
+):
+    """Saves the mean of a list of rawfiles to a new fits file.
+
+    Args:
+        filenames (list): list of raw filenames
+        new_filename (str): new fits filename
+        height (int): image height in pix
+        width (int): image width in pix
+
+    Raises:
+        ValueError: trying to save in a file that does not end with .fits
+    """
+    abs_new_filename = str(Path(new_filename).absolute())
+    if abs_new_filename.split(".")[-1] != "fits":
+        raise ValueError("Output filename must have a .fits extension.")
+    if type(filenames) is not list:
+        filenames = [
+            filenames,
+        ]
+    images_n = len(filenames)
+    arr = np.zeros(shape=(height, width))
+    for filename in tqdm.tqdm(filenames):
+        with open(filename, mode="rb") as file:
+            buffer = file.read()
+        data = np.ndarray(shape=(height, width), dtype="<u2", buffer=buffer)
+
+        arr += data / images_n
+    hdu = fits.PrimaryHDU(data=arr)
+    date_and_time = datetime.datetime.now().strftime("%Y-%m-%dT%H:%M:%S%z")
+    hdu.header["CREATED"] = (
+        str(date_and_time),
+        "Datetime conversion from bin to fits file (Dome C timezone).",
+    )
+    hdu.writeto(abs_new_filename, overwrite=True)
 
 
 def convert_rawfile_to_fits(
     filename: str, height: int, width: int, remove_old: bool = False
 ):
     """Converts a raw file to a fits one, using default header
 
@@ -110,13 +151,16 @@
     """
     if not ".raw" in filename:
         raise ValueError("Can't convert: not a row file")
     with open(filename, mode="rb") as file:
         buffer = file.read()
     data = np.ndarray(shape=(height, width), dtype="<u2", buffer=buffer)
     HDU = fits.PrimaryHDU(data=data)
-    new_filename = "/".join(filename.split(".")[:-1]) + ".fits"
+    filename = os.path.abspath(
+        filename
+    )  # prevents bug when "../" is in filename
+    new_filename = os.path.pathsep.join(filename.split(".")[:-1]) + ".fits"
     HDU.writeto(new_filename, overwrite=True)
     info(f'Image successfully saved to "{new_filename}".')
 
     if remove_old:
         os.remove(filename)
```

### Comparing `micropolarray-1.0.0/build/lib/micropolarray/processing/demodulation.py` & `micropolarray-1.0.1/build/lib/micropolarray/processing/demodulation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from micropolarray_lib.process.rebin import (
+from micropolarray.processing.rebin import (
     standard_jitrebin,
     micropolarray_jitrebin,
     trim_to_match_binning,
 )
-from micropolarray_lib.process.nrgf import (
+from micropolarray.processing.nrgf import (
     find_occulter_position,
     roi_from_polar,
 )
 
 from scipy.optimize import curve_fit
 import glob
 import os
@@ -26,15 +26,15 @@
 class Demodulator:
     """Demodulation class needed for MicroPolarizerArrayImage
     demodulation."""
 
     def __init__(self, demo_matrices_path: str, binning: bool = False):
         self.demo_matrices_path = demo_matrices_path
         self.binning = binning  # needed for a correct image binning
-        self.mij = self.get_demodulation_tensor(demo_matrices_path)
+        self.mij = self._get_demodulation_tensor(demo_matrices_path)
 
     def rebin(self, binning: int):
         warning("USE OF BINNED DEMODULATION MATRIX IS INCORRECT")
         binned_demodulator = Demodulator(self.demo_matrices_path)
         end_y, end_x = self.mij[0, 0].shape
         end_y, end_x = trim_to_match_binning(end_y, end_x, binning)
         new_mij = np.zeros(
@@ -59,18 +59,15 @@
                 #    single_mij.shape[0],
                 #    single_mij.shape[1],
                 #    binning=binning,
                 # )
         binned_demodulator.mij = new_mij
         return binned_demodulator
 
-    def get_demodulation_tensor(self, binning: bool = False):
-        """Reads files "MIJ.fits" from path folder and returns a (3,4,y,x)
-        numpy array representing the demodulation tensor."""
-
+    def _get_demodulation_tensor(self, binning: bool = False) -> np.ndarray:
         if not os.path.exists(self.demo_matrices_path):
             raise FileNotFoundError("self.demo_matrices_path not found.")
         mij_filenames_list = glob.glob(
             self.demo_matrices_path + os.path.sep + "*.fits"
         )
 
         with fits.open(mij_filenames_list[0]) as firsthul:
```

### Comparing `micropolarray-1.0.0/build/lib/micropolarray/processing/demosaic.py` & `micropolarray-1.0.1/build/lib/micropolarray/processing/demosaic.py`

 * *Files identical despite different names*

### Comparing `micropolarray-1.0.0/build/lib/micropolarray/processing/new_demodulation.py` & `micropolarray-1.0.1/build/lib/micropolarray/processing/new_demodulation.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from micropolarray.processing.rebin import (
     standard_rebin,
-    micropolarray_jitrebin,
+    micropolarray_rebin,
     trim_to_match_binning,
 )
 from micropolarray.processing.nrgf import (
     find_occulter_position,
     roi_from_polar,
 )
 from micropolarray.cameras import PolarCam
@@ -20,14 +20,15 @@
 from tqdm import tqdm
 import multiprocessing as mp
 import time
 from logging import warning, info, error
 from micropolarray.processing.chen_wan_liang_calibration import (
     ifov_jitcorrect,
 )
+from micropolarray.utils import mean_plus_std
 
 # Shape of the demodulation matrix
 N_PIXELS_IN_SUPERPIX = 4
 N_MALUS_PARAMS = 3
 
 
 class Demodulator:
@@ -35,19 +36,29 @@
     demodulation."""
 
     def __init__(self, demo_matrices_path: str):
         self.n_pixels_in_superpix = N_PIXELS_IN_SUPERPIX
         self.n_malus_params = N_MALUS_PARAMS
         self.demo_matrices_path = demo_matrices_path
 
-        self.mij = self.get_demodulation_tensor()
+        self.mij = self._get_demodulation_tensor()
 
-    def get_demodulation_tensor(self):
+    def _get_demodulation_tensor(self):
         """Reads files "MIJ.fits" from path folder and returns a (3,4,y,x)
-        numpy array representing the demodulation tensor."""
+        numpy array representing the demodulation tensor.
+
+        Args:
+            binning (bool, optional): _description_. Defaults to False.
+
+        Raises:
+            FileNotFoundError: couldn't find the matrices in the specified path
+
+        Returns:
+            ndarray: (3, 4, *data.shape) array containing the demodulation tensor
+        """
 
         if not os.path.exists(self.demo_matrices_path):
             raise FileNotFoundError("self.demo_matrices_path not found.")
         filenames_list = glob.glob(
             self.demo_matrices_path + os.path.sep + "*.fits"
         )
 
@@ -59,32 +70,74 @@
                 self.n_pixels_in_superpix,
                 sample_data.shape[0],
                 sample_data.shape[1],
             ),
             dtype=float,
         )
 
+        matches = 0
         for filename in filenames_list:
             if (
                 re.search("[Mm][0-9]{2}", filename.split(os.path.sep)[-1])
                 is not None
             ):  # Exclude files not matching m/Mij
+                matches += 1
                 i, j = re.search(
                     "[Mm][0-9]{2}", filename.split(os.path.sep)[-1]
                 ).group()[
                     -2:
                 ]  # Searches for pattern M/m + ij as last string before .fits
                 i = int(i)
                 j = int(j)
                 with fits.open(filename) as hul:
                     Mij[i, j] = hul[0].data
+        if matches != 12:
+            raise ValueError(
+                "Some matrices were not found in the selected folder. Check correct folder name and files pattern M_ij.fits or mij.fits"
+            )
 
         return Mij
 
+    def show(self, vmin=-1, vmax=1, cmap="Greys") -> tuple:
+        """Shows the demodulation tensor
+
+        Args:
+            vmin (int, optional): Minimum shown value. Defaults to -1.
+            vmax (int, optional): Maximum shown value. Defaults to 1.
+            cmap (str, optional): Colormap of the plot. Defaults to "Greys".
+
+        Returns:
+            tuple: fig, ax tuple as returned by matplotlib.pyplot.subplots
+        """
+        fig, ax = plt.subplots(
+            3,
+            4,
+            dpi=300,
+            figsize=(4, 3),
+            constrained_layout=True,
+            sharex="col",
+            sharey="row",
+        )
+        for i in range(3):
+            for j in range(4):
+                mappable = ax[i, j].imshow(
+                    self.mij[i, j], cmap=cmap, vmin=vmin, vmax=vmax
+                )
+                ax[i, j].set_title(rf"M$_{i}$$_{j}$")
+        for ax in fig.get_axes():
+            ax.label_outer()
+
+        fig.subplots_adjust(right=0.8)
+        cbar_ax = fig.add_axes([0.85, 0.15, 0.05, 0.7])
+        fig.colorbar(mappable, cax=cbar_ax)
+
+        return fig, ax
+
     def rebin(self, binning):  # TODO
+        """DO NOT USE THIS, calculate the tensor from the binned images"""
         if (int(self.mij.shape[2] / binning) % 2) or (
             int(self.mij.shape[3] / binning) % 2
         ):
             raise ValueError(
                 f"incorrect binning, resulting matrix would be {int(self.mij.shape[2] / binning)}x{int(self.mij.shape[3] / binning)} (not even values)."
             )
         new_demodulator = Demodulator(self.demo_matrices_path)
@@ -120,46 +173,51 @@
 def calculate_demodulation_tensor(
     polarizer_orientations,
     filenames_list,
     micropol_phases_previsions,
     gain,  #  needed for errors
     output_dir,
     binning=1,
-    occulter=False,
+    occulter=None,
     procs_grid=[4, 4],
     dark_filename=None,
     flat_filename=None,
+    normalizing_S=None,
+    DEBUG=False,
 ):
     """Calculates the demodulation tensor images and saves them. Requires a set of images with different polarizations to fit a Malus curve model.
 
     Args:
         polarizer_orientations (list[float]): List containing the orientations of the incoming light for each image.
         filenames_list (list[str]): List of input images filenames to read. Must include [0, 45, 90, -45].
         micropol_phases_previsions (list[float]): Previsions for the micropolarizer orientations required to initialize fit.
         gain (float): Detector [e-/DN], required to compute errors.
+        output_dir (str): output folder to save matrix to.
         binning (int, optional): Output matrices binning. Defaults to 1 (no binning). Be warned that binning matrices AFTER calculation is an incorrect operation.
-        occulter (bool, optional): Whether to account for a central circle to exclude from calculation. Defaults to False.
+        occulter (list, optional): occulter y, x center and radius to exclude from calculations. Defaults to None.
         procs_grid ([int, int], optional): number of processors per side [Y, X], parallelization will be done in a Y x X grid. Defaults to [4,4] (16 procs in a 4x4 grid).
         dark_filename (str, optional): Dark image filename to correct input images. Defaults to None.
         flat_filename (str, optional): Flat image filename to correct input images. Defaults to None.
+        normalizing_S (float, optional): maximum signal used to normalize single pixel signal. Defaults to None.
 
     Raises:
         ValueError: Raised if any among [0, 45, 90, -45] is not included in the input polarizations.
 
     Notes:
         In the binning process the sum of values is considered, which is ok because data is normalized over the maximum S before being fitted.
     """
 
-    DEBUG = False
     correct_ifov = True
 
     # polarizations = array of polarizer orientations
     # filenames_list = list of filenames
     firstcall = True
-    if not np.all(np.isin([0, 45, 90, -45], polarizer_orientations)):
+    if (normalizing_S is None) and (
+        not np.all(np.isin([0, 45, 90, -45], polarizer_orientations))
+    ):
         raise ValueError(
             "Each one among (0, 45, 90, -45) polarizations must be included in the polarizer orientation array"
         )  # for calculating normalizing_S
     # Have to be sorted
     polarizer_orientations, filenames_list = (
         list(t)
         for t in zip(*sorted(zip(polarizer_orientations, filenames_list)))
@@ -167,33 +225,33 @@
     micropol_phases_previsions = np.array(micropol_phases_previsions)
     rad_micropol_phases_previsions = np.deg2rad(micropol_phases_previsions)
 
     # Flag occulter position to not be fitted, expand to superpixel.
     with fits.open(filenames_list[0]) as file:
         data = file[0].data  # get data dimension
 
+    print("qui")
     # Count binning before dimensions
     data = np.array(data, dtype=float)
-    data = micropolarray_jitrebin(data, *data.shape, binning=binning)
+    data = micropolarray_rebin(data, *data.shape, binning=binning)
     height, width = data.shape
 
     occulter_flag = np.ones_like(data)  # 0 if not a occulted px, 1 otherwise
     if occulter:
-        info("Cleaning occulter...")
-        # Mean values from coronal observations 2022_12_03
-        # (campagna_2022/mean_occulter_pos.py)
-        occulter_y, occulter_x, occulter_r = PolarCam().occulter_pos_last
-        overoccult = 16
-        overoccult = 0
-        occulter_r = occulter_r + overoccult
+        # info("Cleaning occulter...")
+        ## Mean values from coronal observations 2022_12_03
+        ## (campagna_2022/mean_occulter_pos.py)
+        # occulter_y, occulter_x, occulter_r = PolarCam().occulter_pos_last
+        # overoccult = 16
+        # overoccult = 0
+        # occulter_r = occulter_r + overoccult
 
         # Match binning if needed
-        occulter_y = int(occulter_y / binning)
-        occulter_x = int(occulter_x / binning)
-        occulter_r = int(occulter_r / binning)
+        binned_occulter = [int(val / binning) for val in occulter]
+        occulter_y, occulter_x, occulter_r = binned_occulter
 
         occulter_flag = roi_from_polar(
             occulter_flag, [occulter_y, occulter_x], [0, occulter_r]
         )
         for super_y in range(0, occulter_flag.shape[0], 2):
             for super_x in range(0, occulter_flag.shape[1], 2):
                 if np.any(
@@ -206,42 +264,45 @@
     else:
         occulter_flag *= 0
 
     # Collect dark
     if dark_filename:
         with fits.open(dark_filename) as file:
             dark = np.array(file[0].data, dtype=np.float)
-            dark = micropolarray_jitrebin(dark, *dark.shape, binning)
+            dark = micropolarray_rebin(dark, *dark.shape, binning)
     # Collect flat field, normalize it
     if flat_filename:
         with fits.open(flat_filename) as file:
             flat = np.array(file[0].data, dtype=np.float)
-            if correct_ifov:
-                flat = ifov_jitcorrect(flat, *flat.shape)
-            flat = micropolarray_jitrebin(flat, *flat.shape, binning)
+        if correct_ifov:
+            flat = ifov_jitcorrect(flat, *flat.shape)
+        flat = micropolarray_rebin(flat, *flat.shape, binning)
+        # flat_max = np.max(flat, axis=(0, 1))
+        flat_max = mean_plus_std(flat, stds_n=1)
     if flat_filename and dark_filename:
         flat -= dark  # correct flat too
         flat = np.where(flat > 0, flat, 1.0)
         if occulter:
             flat = np.where(occulter_flag, 1.0, flat)
-        flat_max = np.max(flat, axis=(0, 1))
+        # flat_max = np.max(flat, axis=(0, 1))
+        flat_max = mean_plus_std(flat, stds_n=1)
     if flat_filename:
         normalized_flat = np.where(occulter_flag, 1.0, flat / flat_max)
 
     # collect data
     all_data_arr = [0.0] * len(filenames_list)
     info("Collecting data from files...")
     for idx, filename in enumerate(filenames_list):
         with fits.open(filename) as file:
             all_data_arr[idx] = np.array(file[0].data, dtype=float)
             if correct_ifov:
                 all_data_arr[idx] = ifov_jitcorrect(
                     all_data_arr[idx], *all_data_arr[idx].shape
                 )
-            all_data_arr[idx] = micropolarray_jitrebin(
+            all_data_arr[idx] = micropolarray_rebin(
                 all_data_arr[idx], *all_data_arr[idx].shape, binning
             )
             if dark_filename is not None:
                 all_data_arr[idx] -= dark
                 all_data_arr[idx] = np.where(
                     all_data_arr[idx] >= 0, all_data_arr[idx], 0.0
                 )
@@ -288,74 +349,79 @@
             splitted_occulter[i + chunks_n_y * j] = np.array(
                 occulter_flag[
                     i * (chunk_size_y) : (i + 1) * chunk_size_y,
                     j * (chunk_size_x) : (j + 1) * chunk_size_x,
                 ]
             )  # shape = (chunks_n*chunks_n, chunk_size_y, chunk_size_x)
 
-    info("Calculating normalization...")
-    S_max = np.zeros(
-        shape=(height, width)
-    )  # tk_sum = tk_0 + tk_45 + tk_90 + tk_45
-    for pol, image in zip(polarizer_orientations, all_data_arr):
-        if pol in [0, 90, 45, -45]:
-            S_max += 0.5 * image
-    # Normalizing S, has a spike of which maximum is taken
-    bins = 1000
-    histo = np.histogram(S_max, bins=bins)
-    maxvalue = np.max(histo[0])
-    index = np.where(histo[0] == maxvalue)[0][0]
-    normalizing_S = (
-        histo[1][index] + histo[1][index + 1] + histo[1][index - 1]
-    ) / 3
-    # normalizing_S = np.max(S_max) # old
-
-    # ----------------------------------------------
-    # fit gaussian to S for normalization signal
-    def gauss(x, norm, x_0, sigma):
-        return norm * np.exp(-((x - x_0) ** 2) / (4 * sigma**2))
-
-    hist_roi = 10  # bins around max value
-    xvalues = np.array(histo[1])[index - hist_roi : index + hist_roi]
-    yvalues = np.array(histo[0])[index - hist_roi : index + hist_roi]
-    yvalues_sum = np.sum(yvalues)
-    yvalues = yvalues / yvalues_sum
-    xvalues = np.array(
-        [value + (xvalues[1] - xvalues[0]) / 2 for value in xvalues]
-    )  # shift each bin to center
-    prediction = [
-        yvalues[int(len(yvalues) / 2)],  # normalization
-        xvalues[int(len(xvalues) / 2)],  # center
-        xvalues[int(len(xvalues) / 2) + int(hist_roi / 2)]
-        - xvalues[int(len(xvalues) / 2)],  # sigma
-    ]
-    params, cov = curve_fit(
-        gauss,
-        xvalues,
-        yvalues,
-        prediction,
-    )
-    normalizing_S = params[1] + 4 * params[2]  # center of gaussian + 2sigma
-    # 3sigma -> P = 2.7e-3 outliers
-    # 4sigma -> P = 6.3e-5 outliers
-    # ----------------------------------------------
+    if normalizing_S is None:
+        info("Calculating normalization...")
+        S_max = np.zeros(
+            shape=(height, width)
+        )  # tk_sum = tk_0 + tk_45 + tk_90 + tk_45
+        for pol, image in zip(polarizer_orientations, all_data_arr):
+            if pol in [0, 90, 45, -45]:
+                S_max += 0.5 * image
+        # Normalizing S, has a spike of which maximum is taken
+        bins = 1000
+        histo = np.histogram(S_max, bins=bins)
+        maxvalue = np.max(histo[0])
+        index = np.where(histo[0] == maxvalue)[0][0]
+        normalizing_S = (
+            histo[1][index] + histo[1][index + 1] + histo[1][index - 1]
+        ) / 3
+        # normalizing_S = np.max(S_max) # old
+
+        # ----------------------------------------------
+        # fit gaussian to S for normalization signal
+        def gauss(x, norm, x_0, sigma):
+            return norm * np.exp(-((x - x_0) ** 2) / (4 * sigma**2))
+
+        hist_roi = 10  # bins around max value
+        xvalues = np.array(histo[1])[index - hist_roi : index + hist_roi]
+        yvalues = np.array(histo[0])[index - hist_roi : index + hist_roi]
+        yvalues_sum = np.sum(yvalues)
+        yvalues = yvalues / yvalues_sum
+        xvalues = np.array(
+            [value + (xvalues[1] - xvalues[0]) / 2 for value in xvalues]
+        )  # shift each bin to center
+        prediction = [
+            yvalues[int(len(yvalues) / 2)],  # normalization
+            xvalues[int(len(xvalues) / 2)],  # center
+            xvalues[int(len(xvalues) / 2) + int(hist_roi / 2)]
+            - xvalues[int(len(xvalues) / 2)],  # sigma
+        ]
+        params, cov = curve_fit(
+            gauss,
+            xvalues,
+            yvalues,
+            prediction,
+        )
+        normalizing_S = (
+            params[1] + 4 * params[2]
+        )  # center of gaussian + 2sigma
+        # 3sigma -> P = 2.7e-3 outliers
+        # 4sigma -> P = 6.3e-5 outliers
+        # ----------------------------------------------
+    else:
+        normalizing_S *= binning * binning  # account binning
 
     # Debug
     if False:
-        index = 5
+        index = 0
         histo_0 = np.histogram(all_data_arr[index], bins=1000)
         fig, ax = plt.subplots(figsize=(9, 9))
         ax.stairs(histo_0[0], histo_0[1], label="sample image")
         ax.stairs(histo[0], histo[1], label=f"S, max = {np.max(S_max)}")
         ax.axvline(normalizing_S, color="red", label="normalizing_S")
-        ax.plot(
-            xvalues,
-            gauss(xvalues, params[0] * yvalues_sum, params[1], params[2]),
-            label="Fitted curve for normalizing S",
-        )
+        # ax.plot(
+        #    xvalues,
+        #    gauss(xvalues, params[0] * yvalues_sum, params[1], params[2]),
+        #    label="Fitted curve for normalizing S",
+        # )
         ax.set_title(f"Prepol at {polarizer_orientations[index]} deg")
         ax.set_xlabel("S [DN]")
         ax.set_ylabel("Counts")
         ax.legend()
         plt.show()
         sys.exit()
 
@@ -503,20 +569,23 @@
     polarizations_rad = np.deg2rad(polarizer_orientations)
     tk_prediction = 0.5
     efficiency_prediction = 0.4
 
     # Checked errors
     sigma_S2 = np.sqrt(0.5 * normalizing_S / gain)
     normalizing_S2 = normalizing_S * normalizing_S
-    pix_DN_sigma = np.sqrt(
-        splitted_dara_arr / (gain * normalizing_S2)
-        + sigma_S2
-        * (splitted_dara_arr * splitted_dara_arr)
-        / (normalizing_S2 * normalizing_S2)
-    )
+    # pix_DN_sigma = np.sqrt(
+    #    splitted_dara_arr / (gain * normalizing_S2)
+    #    + sigma_S2
+    #    * (splitted_dara_arr * splitted_dara_arr)
+    #    / (normalizing_S2 * normalizing_S2)
+    # )
+    pix_DN_sigma = (
+        np.sqrt(splitted_dara_arr / gain) / normalizing_S
+    )  # poisson error on the photoelectrons
 
     normalized_splitted_data = splitted_dara_arr / normalizing_S
     all_zeros = np.zeros(shape=(num_of_points))
 
     m_ij = np.zeros(
         shape=(N_MALUS_PARAMS, N_PIXELS_IN_SUPERPIX, height, width)
     )  # demodulation matrix
@@ -528,23 +597,28 @@
     predictions = np.zeros(shape=(N_PIXELS_IN_SUPERPIX, N_MALUS_PARAMS))
     predictions[:, 0] = tk_prediction  # Throughput prediction
     predictions[:, 1] = efficiency_prediction  # Efficiency prediction
     predictions[:, 2] = rad_micropol_phases_previsions  # Angle prediction
 
     bounds = np.zeros(shape=(N_PIXELS_IN_SUPERPIX, 2, N_MALUS_PARAMS))
     bounds[:, 0, 0], bounds[:, 1, 0] = 0.1, 0.9999999  # Throughput bounds
+
+    # bounds[:, 0, 0], bounds[:, 1, 0] = (
+    #    0.1,
+    #    2.0,
+    # )  # tk is multiplied by 0.5 so it can actually be > 1 and still physical
     bounds[:, 0, 1], bounds[:, 1, 1] = 0.1, 0.9999999  # Efficiency bounds
     bounds[:, 0, 2] = rad_micropol_phases_previsions - 15  # Lower angle bounds
     bounds[:, 1, 2] = rad_micropol_phases_previsions + 15  # Upper angle bounds
 
     # Fit for each superpixel. Use theoretical demodulation matrix for
     # occulter if present.
     if DEBUG:
-        x_start, x_end = 8, 10
-        y_start, y_end = 8, 10
+        x_start, x_end = 100, 110
+        y_start, y_end = 100, 110
     else:
         y_start, y_end = 0, height
         x_start, x_end = 0, width
     milestones = [
         int(height / 4),
         int(height / 4) + 1,
         int(height / 2),
@@ -605,25 +679,27 @@
                     for i in range(4):
                         ax.errorbar(
                             np.rad2deg(polarizations_rad),
                             normalized_superpix_arr[:, i],
                             yerr=sigma_pix[:, i],
                             xerr=[1.0] * len(polarizations_rad),
                             label=f"points {i}",
-                            fmt="None",
+                            fmt="k-",
                             color=colors[i],
                         )
                         min = np.min(polarizations_rad)
+                        # min = 225
                         max = np.max(polarizations_rad)
+                        # max = 405
                         x = np.arange(min, max, (max - min) / 100)
-                        x = np.arange(-np.pi / 2, np.pi, np.pi / 100)
                         ax.plot(
                             np.rad2deg(x),
                             Malus(x, *superpix_params[i]),
                             label=f"t = {superpix_params[i,0]:2.2f}, e = {superpix_params[i, 1]:2.2f}, phi = {np.rad2deg(superpix_params[i, 2]):2.2f}",
+                            color=colors[i],
                         )
                         ax.set_title(
                             f"super_y = {super_y}, super_x = {super_x},"
                         )
                         ax.set_xlabel("Prepolarizer orientations [deg]")
                         ax.set_ylabel("signal / S")
 
@@ -639,28 +715,42 @@
                     continue
 
                 # Compute modulation matrix and its inverse
                 t = superpix_params[:, 0]
                 eff = superpix_params[:, 1]
                 phi = superpix_params[:, 2]
 
-                # modified 2023_02_13, worse
-                # t = t * (1 + FPN)
-                # eff = eff * (1 + FPN)
-
                 modulation_matrix = np.array(
                     [
                         0.5 * t,
                         0.5 * t * eff * np.cos(2.0 * phi),
                         0.5 * t * eff * np.sin(2.0 * phi),
                     ]
                 )
                 modulation_matrix = modulation_matrix.T
                 demodulation_matrix = np.linalg.pinv(modulation_matrix)
 
+                if DEBUG:
+                    print()
+                    print("MOD")
+                    print(modulation_matrix)
+                    print(theo_modulation_matrix)
+
+                    print()
+                    print("DEMOD")
+                    print(demodulation_matrix)
+                    print(theo_demodulation_matrix)
+
+                    print()
+                    print("params")
+                    print(t)
+                    print(eff)
+                    print(phi)
+                    print("---")
+
                 # Remove matrices with big numbers
                 if np.any(demodulation_matrix > 100) or np.any(
                     demodulation_matrix < -100
                 ):
                     demodulation_matrix = theo_demodulation_matrix
 
                 for i in range(2):
@@ -713,25 +803,7 @@
 def Malus(angle, throughput, efficiency, phase):
     # original
     modulated_efficiency = efficiency * (
         np.cos(2.0 * phase) * np.cos(2.0 * angle)
         + np.sin(2.0 * phase) * np.sin(2.0 * angle)
     )
     return 0.5 * throughput * (1.0 + modulated_efficiency)
-
-
-"""
-
-
-def Malus(angle, throughput, efficiency, phase, FPN):
-    # modified version 2022_02_13
-    modulated_efficiency = efficiency * (
-        np.cos(2.0 * phase) * np.cos(2.0 * angle)
-        + np.sin(2.0 * phase) * np.sin(2.0 * angle)
-    )
-    return (
-        0.5
-        * throughput
-        * (1.0 + FPN)
-        * (1.0 + modulated_efficiency * (1.0 + FPN))
-    )
-"""
```

### Comparing `micropolarray-1.0.0/build/lib/micropolarray/processing/nrgf.py` & `micropolarray-1.0.1/build/lib/micropolarray/processing/nrgf.py`

 * *Files 14% similar despite different names*

```diff
@@ -166,19 +166,18 @@
 
     Args:
         data (np.array): input data
         method (str, optional): Method to find occulter edges. If "sigmoid" it will try to fit four sigmoids at the image edges centers, inferring the occulter edges from the parameters. If "algo" it will start from the image edge center and infer the occulter position when DN[i] > threshold*mean(DN[:i]) Defaults to "sigmoid".
         threshold (float, optional): Threshold for the algo method. Defaults to 4.0.
 
     Raises:
-        ValueError: _description_
-        ValueError: _description_
+        UnboundLocalError: couldn't converge
 
     Returns:
-        _type_: _description_
+        list: occulter y, occulter x, occulter radius
     """
     # works if occulter is not entirely inside a single quadrant, fits
     # a sigmoid to find occulter bounds
     half_y = int(data.shape[0] / 2)
     half_x = int(data.shape[1] / 2)
     values_x_0 = np.flip(data[half_y, :half_x])
     values_x_1 = data[half_y, half_x:]
@@ -196,54 +195,56 @@
             "Upper vertical",
             "Right horizontal",
             "Left horizontal",
         ]
 
     if method == "sigmoid":
         for idx, half_array in enumerate(
-            [values_x_0, values_x_1, values_y_0, values_y_1]
+            [values_y_0, values_y_1, values_x_0, values_x_1]
         ):
             # Artificial plateau after maximum
             # max_half_array = np.max(half_array)
             # for i, element in enumerate(half_array):
             #    if element == max_half_array:
             #        max_i = i
             #        break
             # half_array[max_i:] = max_half_array
 
             # x = np.arange(0, half_y, 1)
             x = np.arange(0, int(len(half_array / 2)), 1)
 
             params = [
+                # np.mean(half_array[int(len(half_array) / 2) :]),
                 np.max(half_array),
+                # np.mean(half_array[: int(len(half_array) / 2)]),
                 np.min(half_array),
-                1.0,
-                -data.shape[0] / 4,
+                0.5,
+                len(half_array) / 2,
             ]
             params, pcov = curve_fit(sigmoid, x, half_array, params)
             occulter_bounds[idx] = params[3]
 
             if show:
                 axis = ax[idx]
                 axis.scatter(x, half_array, c="grey")
                 axis.plot(x, sigmoid(x, *params), c="black")
                 axis.set_title(titles[idx])
                 axis.set_xlabel("Pixels from center")
                 axis.set_ylabel("DN")
 
         try:
-            occulter_bounds[0] = half_x + occulter_bounds[0]
-            occulter_bounds[1] = half_x - occulter_bounds[1]
-            occulter_bounds[2] = half_y + occulter_bounds[2]
-            occulter_bounds[3] = half_y - occulter_bounds[3]
+            occulter_bounds[0] = half_y - occulter_bounds[0]
+            occulter_bounds[1] = half_y + occulter_bounds[1]
+            occulter_bounds[2] = half_x - occulter_bounds[2]
+            occulter_bounds[3] = half_x + occulter_bounds[3]
         except UnboundLocalError:
             raise ValueError("Edges not found, try to change the threshold")
 
     elif method == "algo":
-        # OLD, ALGORITM INSTEAD OF FITTING
+        # OLD, ALGORITM INSTEAD OF FITTING - less stable
         min_points = 5
         threshold = threshold
 
         for i, val in enumerate(values_x_0):
             if i > min_points:
                 mean = np.mean(values_x_0[:i])
                 if val > (threshold * mean):
@@ -264,35 +265,75 @@
         for i, val in enumerate(values_y_1):
             if i > min_points:
                 mean = np.mean(values_y_1[:i])
                 if val > (threshold * mean):
                     occulter_end_y = half_y + i
                     break
         try:
-            occulter_bounds[0] = occulter_start_x
-            occulter_bounds[1] = occulter_end_x
-            occulter_bounds[2] = occulter_start_y
-            occulter_bounds[3] = occulter_end_y
+            occulter_bounds[0] = occulter_start_y
+            occulter_bounds[1] = occulter_end_y
+            occulter_bounds[2] = occulter_start_x
+            occulter_bounds[3] = occulter_end_x
         except UnboundLocalError:
             raise ValueError(
                 "ERROR: occulter edges not found, try to change the threshold"
             )
     if show:
         plt.show()
 
     x_center = int(np.mean([occulter_bounds[:2]]))
     y_center = int(np.mean([occulter_bounds[2:]]))
     radius = int(
         np.mean(
             [
-                (occulter_bounds[1] - occulter_bounds[0]) / 2,
-                (occulter_bounds[3] - occulter_bounds[2]) / 2,
+                np.abs(occulter_bounds[1] - occulter_bounds[0]) / 2,
+                np.abs(occulter_bounds[3] - occulter_bounds[2]) / 2,
             ]
         )
     )
 
     return [y_center, x_center, radius]
 
 
+def remove_outliers_simple(original, neighbours=2):
+    """EXPERIMENTAL DO NOT USE, for improving fitting on occulter position"""
+    data = original.copy()
+    for i, element in enumerate(data[neighbours:-neighbours]):
+        median = np.median(data[i - neighbours : i + neighbours])
+        std = np.median(np.abs(data[i - neighbours : i + neighbours] - median))
+        if (element < median - 3 * std) or (element > median + 3 * std):
+            print()
+            print(element)
+            print(data[neighbours:-neighbours])
+            data[i] = median
+            print(data[neighbours:-neighbours])
+    return data
+
+    median = np.median(data)
+
+    median_deviation = np.abs(data - np.median(data))
+    condition = (data < (median + 3 * median_deviation)) | (
+        data > (median - 3 * median_deviation)
+    )
+    data = np.where(condition, data, median)
+    return data
+    extreme = 2
+    outliers = []
+    for i, element in enumerate(data[extreme:-extreme]):
+        mean = np.mean([data[i], data[i + 1]])
+        std = np.std([data[i], data[i + 1]])
+        if (element > (mean + 3 * std)) or (element < (mean - 3 * std)):
+            outliers.append(i + 1)
+    data = np.delete(data, outliers)
+    return data
+
+
+def reject_outliers(data, m=2.0):
+    d = np.abs(data - np.median(data))
+    mdev = np.median(d)
+    s = d / mdev if mdev else np.zeros(len(d))
+    return data[s < m]
+
+
 def sigmoid(x, max, min, slope, intercept):
-    sigma = slope * (x + intercept)
+    sigma = slope * (x - intercept)
     return max * np.exp(sigma) / (1 + np.exp(sigma)) + min
```

### Comparing `micropolarray-1.0.0/build/lib/micropolarray/processing/rebin.py` & `micropolarray-1.0.1/build/lib/micropolarray/processing/rebin.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,52 @@
-from numba import njit
+from numba import njit, jit
 import numpy as np
 from logging import info
 
 
-@njit
 def print_trimming_info(height, width, new_height, new_width):
+    # print(
+    #    f"Data trimmed to fit rebinning: ({height}, {width}) -> ({new_height}, {new_width})"
+    # )
     print(
-        f"Data trimmed to fit rebinning: ({height}, {width}) -> ({new_height}, {new_width})"
+        "Data trimmed to fit rebinning: (",
+        height,
+        ",",
+        width,
+        ") -> (",
+        new_height,
+        ",",
+        new_width,
+        ")",
     )
 
 
+def micropolarray_rebin(data: np.ndarray, height: int, width: int, binning=2):
+    """Wrapper for the faster rebinning donw with numba. First deletes last row/column until binning is possible, then calls binning on the result shape.
+
+    Args:
+        data (np.ndarray): data to rebin
+        height (int): lenght of first axis
+        width (int): lenght of second axis
+        binning (int, optional): Binning to be performed. Defaults to 2.
+
+    Returns:
+        ndarray: binned data, trimmed if necessary
+    """
+    trimmed = False
+    new_height, new_width = trim_to_match_2xbinning(height, width, binning)
+    new_height = int(new_height / binning)
+    new_width = int(new_width / binning)
+    new_data = micropolarray_jitrebin(data, new_height, new_width, binning)
+
+    return new_data
+
+
 @njit
-def micropolarray_jitrebin(data, height, width, binning=2):
+def micropolarray_jitrebin_old(data, height, width, binning=2):
     """Fast rebinning function for the micropolarray image."""
     # Skip last row/columns until they are divisible by binning,
     # allows any binning
     trimmed = False
     new_height, new_width = trim_to_match_2xbinning(height, width, binning)
     new_height = int(new_height / binning)
     new_width = int(new_width / binning)
@@ -29,14 +60,31 @@
                     i = (new_y - new_y % 2) * binning + y_scaler
                     j = (new_x - new_x % 2) * binning + x_scaler
                     new_data[new_y, new_x] += data[i, j]
 
     return new_data
 
 
+@njit
+def micropolarray_jitrebin(data, new_height, new_width, binning=2):
+    """Fast rebinning function for the micropolarray image. Needs to be wrapped to print info."""
+    new_data = np.zeros(shape=(new_height, new_width), dtype=np.double)
+    for new_y in range(new_height):
+        for new_x in range(new_width):
+            for y_scaler in range((new_y % 2), (new_y % 2) + 2 * binning, 2):
+                for x_scaler in range(
+                    (new_x % 2), (new_x % 2) + 2 * binning, 2
+                ):
+                    i = (new_y - new_y % 2) * binning + y_scaler
+                    j = (new_x - new_x % 2) * binning + x_scaler
+                    new_data[new_y, new_x] += data[i, j]
+
+    return new_data
+
+
 def standard_rebin(data, binning: int) -> np.array:
     """Rebins the data, binned each binningxbinning.
 
     Args:
         image (np.array): data to be binned
         binning (int): binning to be applied. A value of 2 will result in a 2x2 binning (1 pixel is a sum of 4 neighbour pixels)
 
@@ -68,15 +116,14 @@
                         binning * new_y + y_scaler,
                         binning * new_x + x_scaler,
                     ]
 
     return new_data
 
 
-@njit
 def trim_to_match_2xbinning(height: int, width: int, binning: int):
     """Deletes the last image pixels until superpixel binning is compatible with new dimensions
 
     Args:
         height (int): image height_
         width (int): image width
         binning (int): image binning
```

### Comparing `micropolarray-1.0.0/build/lib/micropolarray/utils.py` & `micropolarray-1.0.1/build/lib/micropolarray/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -62,21 +62,69 @@
     fixed_data = data.copy()
     fixed_data = np.where(fixed_data > min, fixed_data, min)
     fixed_data = np.where(fixed_data < max, fixed_data, max)
     return fixed_data
 
 
 def mean_minus_std(data: np.array, stds_n: int = 1) -> float:
+    """Returns the value at the mean - standard deviation for the input data
+
+    Args:
+        data (np.array): input data
+        stds_n (int, optional): number of standard deviations. Defaults to 1.
+
+    Returns:
+        float: mean value - n*stdevs
+    """
     return np.mean(data) - stds_n * np.std(data)
 
 
 def mean_plus_std(data: np.array, stds_n: int = 1) -> float:
+    """Returns the value at the mean + standard deviation for the input data
+
+    Args:
+        data (np.array): input data
+        stds_n (int, optional): number of standard deviations. Defaults to 1.
+
+    Returns:
+        float: mean value + n*stdevs
+    """
     return np.mean(data) + stds_n * np.std(data)
 
 
+def median_minus_std(data: np.array, stds_n: int = 1) -> float:
+    """Returns the value at the median - median deviation for the input data
+
+    Args:
+        data (np.array): input data
+        stds_n (int, optional): number of standard deviations. Defaults to 1.
+
+    Returns:
+        float: median value - n*mediandevs
+    """
+    median = np.median(data)
+    median_std = np.median(np.abs(data - median))
+    return median - stds_n * median_std
+
+
+def median_plus_std(data: np.array, stds_n: int = 1) -> float:
+    """Returns the value at the median + median deviation for the input data
+
+    Args:
+        data (np.array): input data
+        stds_n (int, optional): number of standard deviations. Defaults to 1.
+
+    Returns:
+        float: median value + n*mediandevs
+    """
+    median = np.median(data)
+    median_std = np.median(np.abs(data - median))
+    return median + stds_n * median_std
+
+
 def normalize2pi(angles_list):
     if type(angles_list) is not list:
         angles_list = [
             angles_list,
         ]
     for i, angle in enumerate(angles_list):
         while angle > 90:
@@ -86,14 +134,20 @@
         angles_list[i] = angle
 
     return angles_list
 
 
 # timer decorator
 def timer(func):
+    """Use this to time function execution
+
+    Args:
+        func (function): function of which to measure execution time
+    """
+
     def wrapper(*args, **kwargs):
         start = time.time()
         result = func(*args, **kwargs)
         end = time.time()
         print(
             f"Function {func.__name__} took {round(end - start, 4)} ns to run"
         )
```

### Comparing `micropolarray-1.0.0/micropolarray.egg-info/PKG-INFO` & `micropolarray-1.0.1/micropolarray.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micropolarray
-Version: 1.0.0
+Version: 1.0.1
 Summary: micropolarizer array data utilities
 Home-page: https://github.com/Hevil33/micropolarray_master
 Author: Hervé Haudemand
 Author-email: Herve Haudemand <herve.haudemand@inaf.it>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, Hevil33
@@ -35,15 +35,15 @@
         OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
         
 Project-URL: Homepage, https://github.com/Hevil33/micropolarray_master
 Keywords: micropolarizer,polarcam,polarization
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.9
+Requires-Python: >=3.0
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # micropolarray
 
 Python module for loading and using micropolarizer array and polarcam images.
@@ -90,7 +90,15 @@
 pol_0_image = image.single_pol_subimages[image.angle_dic[0]]
 
 demosaiced_image = image.demosaic() 
 
 binned_image = image.rebin(binning=4)  # binned 4x4 image
 
 ```
+
+If demodulation matrices are available, it is easy to get demodulated images
+
+```
+
+demodulator = ml.Demodulator(demodulation_tensor_path)
+
+demo_image = image.demodulate(demodulator) # This image is now demodulated
```

### Comparing `micropolarray-1.0.0/micropolarray.egg-info/SOURCES.txt` & `micropolarray-1.0.1/micropolarray.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -14,12 +14,13 @@
 ./build/lib/micropolarray/processing/congrid.py
 ./build/lib/micropolarray/processing/convert.py
 ./build/lib/micropolarray/processing/demodulation.py
 ./build/lib/micropolarray/processing/demosaic.py
 ./build/lib/micropolarray/processing/new_demodulation.py
 ./build/lib/micropolarray/processing/nrgf.py
 ./build/lib/micropolarray/processing/rebin.py
+./build/lib/micropolarray/processing/shift.py
 micropolarray.egg-info/PKG-INFO
 micropolarray.egg-info/SOURCES.txt
 micropolarray.egg-info/dependency_links.txt
 micropolarray.egg-info/requires.txt
 micropolarray.egg-info/top_level.txt
```

### Comparing `micropolarray-1.0.0/pyproject.toml` & `micropolarray-1.0.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "micropolarray"
-version = "1.0.0"
+version = "1.0.1"
 description = "micropolarizer array data utilities"
 readme = "README.md"
 authors = [{ name ="Herve Haudemand", email = "herve.haudemand@inaf.it" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: BSD License",
     "Programming Language :: Python",
@@ -22,14 +22,14 @@
     "dataclasses",
     "astropy",
     "matplotlib",
     "scipy",
     "wheel",
     "tqdm",
 ]
-requires-python = ">=3.9"
+requires-python = ">=3.0"
 
 [project.optional-dependencies]
 dev = ["black", "bumpver", "isort", "pip-tools", "pytest"]
 
 [project.urls]
-Homepage = "https://github.com/Hevil33/micropolarray_master"
+Homepage = "https://github.com/Hevil33/micropolarray_master"
```

### Comparing `micropolarray-1.0.0/setup.py` & `micropolarray-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 
 setup(
     name="micropolarray",
-    version="1.0.0",
+    version="1.0.1",
     description="Micro-Polarizer array and PolarCam images processing libraries",
     url="https://github.com/Hevil33/micropolarray_master",
     author="Hervé Haudemand",
     author_email="herve.haudemand@inaf.it",
     install_requires=[
         "numpy<1.24.0",  # compatibility with pip installation
         "pandas",
```

