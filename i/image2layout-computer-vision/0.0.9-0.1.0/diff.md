# Comparing `tmp/image2layout_computer_vision-0.0.9.tar.gz` & `tmp/image2layout_computer_vision-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "image2layout_computer_vision-0.0.9.tar", last modified: Mon Jul 31 07:07:25 2023, max compression
+gzip compressed data, was "image2layout_computer_vision-0.1.0.tar", last modified: Fri Aug  4 09:13:32 2023, max compression
```

## Comparing `image2layout_computer_vision-0.0.9.tar` & `image2layout_computer_vision-0.1.0.tar`

### file list

```diff
@@ -1,31 +1,34 @@
-drwxr-xr-x   0 felixdo    (501) staff       (20)        0 2023-07-31 07:07:25.610577 image2layout_computer_vision-0.0.9/
--rw-r--r--   0 felixdo    (501) staff       (20)     1073 2023-07-26 05:55:06.000000 image2layout_computer_vision-0.0.9/LICENSE
--rw-r--r--   0 felixdo    (501) staff       (20)     2963 2023-07-31 07:07:25.610320 image2layout_computer_vision-0.0.9/PKG-INFO
--rw-r--r--   0 felixdo    (501) staff       (20)     2393 2023-07-28 02:48:08.000000 image2layout_computer_vision-0.0.9/README.md
--rw-r--r--   0 felixdo    (501) staff       (20)      637 2023-07-31 07:05:05.000000 image2layout_computer_vision-0.0.9/pyproject.toml
--rw-r--r--   0 felixdo    (501) staff       (20)       38 2023-07-31 07:07:25.610644 image2layout_computer_vision-0.0.9/setup.cfg
-drwxr-xr-x   0 felixdo    (501) staff       (20)        0 2023-07-31 07:07:25.604968 image2layout_computer_vision-0.0.9/src/
-drwxr-xr-x   0 felixdo    (501) staff       (20)        0 2023-07-31 07:07:25.605313 image2layout_computer_vision-0.0.9/src/image2layout_computer_vision/
--rw-r--r--   0 felixdo    (501) staff       (20)      416 2023-07-27 04:43:37.000000 image2layout_computer_vision-0.0.9/src/image2layout_computer_vision/__init__.py
-drwxr-xr-x   0 felixdo    (501) staff       (20)        0 2023-07-31 07:07:25.606769 image2layout_computer_vision-0.0.9/src/image2layout_computer_vision/color_extract/
--rw-r--r--   0 felixdo    (501) staff       (20)       95 2023-07-26 08:56:49.000000 image2layout_computer_vision-0.0.9/src/image2layout_computer_vision/color_extract/__init__.py
--rw-r--r--   0 felixdo    (501) staff       (20)     8737 2023-07-28 02:57:52.000000 image2layout_computer_vision-0.0.9/src/image2layout_computer_vision/color_extract/main.py
-drwxr-xr-x   0 felixdo    (501) staff       (20)        0 2023-07-31 07:07:25.608260 image2layout_computer_vision-0.0.9/src/image2layout_computer_vision/ocr/
--rw-r--r--   0 felixdo    (501) staff       (20)      212 2023-07-27 04:43:44.000000 image2layout_computer_vision-0.0.9/src/image2layout_computer_vision/ocr/__init__.py
--rw-r--r--   0 felixdo    (501) staff       (20)    14270 2023-07-28 10:22:11.000000 image2layout_computer_vision-0.0.9/src/image2layout_computer_vision/ocr/imagebox.py
--rw-r--r--   0 felixdo    (501) staff       (20)     2652 2023-07-31 07:04:17.000000 image2layout_computer_vision-0.0.9/src/image2layout_computer_vision/ocr/main.py
--rw-r--r--   0 felixdo    (501) staff       (20)     6286 2023-07-26 05:55:06.000000 image2layout_computer_vision-0.0.9/src/image2layout_computer_vision/ocr/model_layoutmlv2.py
-drwxr-xr-x   0 felixdo    (501) staff       (20)        0 2023-07-31 07:07:25.609885 image2layout_computer_vision-0.0.9/src/image2layout_computer_vision/utils/
--rw-r--r--   0 felixdo    (501) staff       (20)      227 2023-07-27 11:28:42.000000 image2layout_computer_vision-0.0.9/src/image2layout_computer_vision/utils/__init__.py
--rw-r--r--   0 felixdo    (501) staff       (20)     2221 2023-07-27 11:32:07.000000 image2layout_computer_vision-0.0.9/src/image2layout_computer_vision/utils/annotation.py
--rw-r--r--   0 felixdo    (501) staff       (20)     4896 2023-07-26 08:33:29.000000 image2layout_computer_vision-0.0.9/src/image2layout_computer_vision/utils/color_system.py
--rw-r--r--   0 felixdo    (501) staff       (20)     1398 2023-07-26 05:55:06.000000 image2layout_computer_vision-0.0.9/src/image2layout_computer_vision/utils/imaging.py
--rw-r--r--   0 felixdo    (501) staff       (20)     1900 2023-07-26 05:55:06.000000 image2layout_computer_vision-0.0.9/src/image2layout_computer_vision/utils/pixel_mask.py
-drwxr-xr-x   0 felixdo    (501) staff       (20)        0 2023-07-31 07:07:25.606272 image2layout_computer_vision-0.0.9/src/image2layout_computer_vision.egg-info/
--rw-r--r--   0 felixdo    (501) staff       (20)     2963 2023-07-31 07:07:25.000000 image2layout_computer_vision-0.0.9/src/image2layout_computer_vision.egg-info/PKG-INFO
--rw-r--r--   0 felixdo    (501) staff       (20)      923 2023-07-31 07:07:25.000000 image2layout_computer_vision-0.0.9/src/image2layout_computer_vision.egg-info/SOURCES.txt
--rw-r--r--   0 felixdo    (501) staff       (20)        1 2023-07-31 07:07:25.000000 image2layout_computer_vision-0.0.9/src/image2layout_computer_vision.egg-info/dependency_links.txt
--rw-r--r--   0 felixdo    (501) staff       (20)       54 2023-07-31 07:07:25.000000 image2layout_computer_vision-0.0.9/src/image2layout_computer_vision.egg-info/top_level.txt
--rw-r--r--   0 felixdo    (501) staff       (20)    13593 2023-07-27 10:41:57.000000 image2layout_computer_vision-0.0.9/src/sandbox.py
--rw-r--r--   0 felixdo    (501) staff       (20)     8978 2023-07-31 07:03:32.000000 image2layout_computer_vision-0.0.9/src/sandbox_ocr.py
--rw-r--r--   0 felixdo    (501) staff       (20)      747 2023-07-26 09:01:24.000000 image2layout_computer_vision-0.0.9/src/test.py
+drwxrwxr-x   0 test      (1001) test      (1001)        0 2023-08-04 09:13:32.237408 image2layout_computer_vision-0.1.0/
+-rw-rw-r--   0 test      (1001) test      (1001)     1073 2023-07-20 04:03:09.000000 image2layout_computer_vision-0.1.0/LICENSE
+-rw-rw-r--   0 test      (1001) test      (1001)     2845 2023-08-04 09:13:32.237408 image2layout_computer_vision-0.1.0/PKG-INFO
+-rw-rw-r--   0 test      (1001) test      (1001)     2275 2023-08-04 09:12:59.000000 image2layout_computer_vision-0.1.0/README.md
+-rw-rw-r--   0 test      (1001) test      (1001)      637 2023-08-04 08:35:55.000000 image2layout_computer_vision-0.1.0/pyproject.toml
+-rw-rw-r--   0 test      (1001) test      (1001)       38 2023-08-04 09:13:32.237408 image2layout_computer_vision-0.1.0/setup.cfg
+drwxrwxr-x   0 test      (1001) test      (1001)        0 2023-08-04 09:13:32.233408 image2layout_computer_vision-0.1.0/src/
+drwxrwxr-x   0 test      (1001) test      (1001)        0 2023-08-04 09:13:32.233408 image2layout_computer_vision-0.1.0/src/image2layout_computer_vision/
+-rw-rw-r--   0 test      (1001) test      (1001)      613 2023-08-04 08:58:07.000000 image2layout_computer_vision-0.1.0/src/image2layout_computer_vision/__init__.py
+drwxrwxr-x   0 test      (1001) test      (1001)        0 2023-08-04 09:13:32.237408 image2layout_computer_vision-0.1.0/src/image2layout_computer_vision/color_extract/
+-rw-rw-r--   0 test      (1001) test      (1001)       95 2023-08-01 04:32:01.000000 image2layout_computer_vision-0.1.0/src/image2layout_computer_vision/color_extract/__init__.py
+-rw-rw-r--   0 test      (1001) test      (1001)    14464 2023-08-03 04:42:22.000000 image2layout_computer_vision-0.1.0/src/image2layout_computer_vision/color_extract/main.py
+drwxrwxr-x   0 test      (1001) test      (1001)        0 2023-08-04 09:13:32.237408 image2layout_computer_vision-0.1.0/src/image2layout_computer_vision/ocr/
+-rw-rw-r--   0 test      (1001) test      (1001)      251 2023-08-04 08:48:54.000000 image2layout_computer_vision-0.1.0/src/image2layout_computer_vision/ocr/__init__.py
+-rw-rw-r--   0 test      (1001) test      (1001)    16279 2023-08-04 08:55:20.000000 image2layout_computer_vision-0.1.0/src/image2layout_computer_vision/ocr/imagebox.py
+-rw-rw-r--   0 test      (1001) test      (1001)     3625 2023-08-04 09:10:20.000000 image2layout_computer_vision-0.1.0/src/image2layout_computer_vision/ocr/main.py
+-rw-rw-r--   0 test      (1001) test      (1001)     6286 2023-07-26 05:47:05.000000 image2layout_computer_vision-0.1.0/src/image2layout_computer_vision/ocr/model_layoutmlv2.py
+-rw-rw-r--   0 test      (1001) test      (1001)     2160 2023-08-04 08:16:49.000000 image2layout_computer_vision-0.1.0/src/image2layout_computer_vision/ocr/model_paddle.py
+drwxrwxr-x   0 test      (1001) test      (1001)        0 2023-08-04 09:13:32.237408 image2layout_computer_vision-0.1.0/src/image2layout_computer_vision/utils/
+-rw-rw-r--   0 test      (1001) test      (1001)      457 2023-08-04 08:57:51.000000 image2layout_computer_vision-0.1.0/src/image2layout_computer_vision/utils/__init__.py
+-rw-rw-r--   0 test      (1001) test      (1001)     7186 2023-08-04 09:09:14.000000 image2layout_computer_vision-0.1.0/src/image2layout_computer_vision/utils/annotation.py
+-rw-rw-r--   0 test      (1001) test      (1001)     4896 2023-08-01 04:32:01.000000 image2layout_computer_vision-0.1.0/src/image2layout_computer_vision/utils/color_system.py
+-rw-rw-r--   0 test      (1001) test      (1001)     3820 2023-08-03 10:44:05.000000 image2layout_computer_vision-0.1.0/src/image2layout_computer_vision/utils/imaging.py
+-rw-rw-r--   0 test      (1001) test      (1001)     2402 2023-08-02 09:28:26.000000 image2layout_computer_vision-0.1.0/src/image2layout_computer_vision/utils/pixel_mask.py
+-rw-rw-r--   0 test      (1001) test      (1001)     5469 2023-08-03 03:51:23.000000 image2layout_computer_vision-0.1.0/src/image2layout_computer_vision/utils/timing.py
+drwxrwxr-x   0 test      (1001) test      (1001)        0 2023-08-04 09:13:32.237408 image2layout_computer_vision-0.1.0/src/image2layout_computer_vision.egg-info/
+-rw-rw-r--   0 test      (1001) test      (1001)     2845 2023-08-04 09:13:32.000000 image2layout_computer_vision-0.1.0/src/image2layout_computer_vision.egg-info/PKG-INFO
+-rw-rw-r--   0 test      (1001) test      (1001)     1052 2023-08-04 09:13:32.000000 image2layout_computer_vision-0.1.0/src/image2layout_computer_vision.egg-info/SOURCES.txt
+-rw-rw-r--   0 test      (1001) test      (1001)        1 2023-08-04 09:13:32.000000 image2layout_computer_vision-0.1.0/src/image2layout_computer_vision.egg-info/dependency_links.txt
+-rw-rw-r--   0 test      (1001) test      (1001)       74 2023-08-04 09:13:32.000000 image2layout_computer_vision-0.1.0/src/image2layout_computer_vision.egg-info/top_level.txt
+-rw-rw-r--   0 test      (1001) test      (1001)    11005 2023-07-26 06:47:33.000000 image2layout_computer_vision-0.1.0/src/sandbox.py
+-rw-rw-r--   0 test      (1001) test      (1001)    11193 2023-08-03 04:03:51.000000 image2layout_computer_vision-0.1.0/src/sandbox_color.py
+-rw-rw-r--   0 test      (1001) test      (1001)     1246 2023-08-04 09:11:31.000000 image2layout_computer_vision-0.1.0/src/sandbox_ocr.py
+-rw-rw-r--   0 test      (1001) test      (1001)      812 2023-08-03 04:47:50.000000 image2layout_computer_vision-0.1.0/src/test_color.py
```

### Comparing `image2layout_computer_vision-0.0.9/LICENSE` & `image2layout_computer_vision-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `image2layout_computer_vision-0.0.9/PKG-INFO` & `image2layout_computer_vision-0.1.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: image2layout_computer_vision
-Version: 0.0.9
+Version: 0.1.0
 Summary: image processing and stuff
 Author-email: Felix Do <felix.do.1030@gmail.com>
 Project-URL: Homepage, https://github.com/felix-do-wizardry/image2layout-computer-vision
 Project-URL: Bug Tracker, https://github.com/felix-do-wizardry/image2layout-computer-vision
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -16,15 +16,15 @@
 
 An image processing module for some computer vision tasks (public module for image2layout)
 
 Package Page: [pypi](https://pypi.org/project/image2layout-computer-vision/)
 
 Features:
 
-1. Text Detection
+1. Text Detection and Recognition (OCR)
 2. Color extraction (background and main foreground)
 
 ## Installations
 
 ### Install with `python`/`conda` [Linux]
 
 1. (Optional) Conda
@@ -45,66 +45,58 @@
 sudo apt install tesseract-ocr libtesseract-dev -y
 ```
 
 
 3. Python libraries (python>=3.8)
 
 ```bash
-python -m pip install 'torch>=2.0' torchvision torchaudio
+# python -m pip install 'torch>=2.0' torchvision torchaudio
+conda install pytorch torchvision torchaudio cpuonly -c pytorch --name cv -y
 
 python -m pip install Pillow pandas numpy scikit-learn pyyaml==5.1 chardet pytesseract
 python -m pip install --upgrade datasets transformers
 
 python -m pip install 'git+https://github.com/facebookresearch/detectron2.git'
 
 python -m pip install --upgrade image2layout-computer-vision
 ```
 
 ### Install with `docker`
 
-Replace `Dockerfile_cpu` with `Dockerfile` if running with GPU
-API Implementation is in-progress
+<!-- Replace `Dockerfile_cpu` with `Dockerfile` if running with GPU (not yet supported) -->
 ```bash
 sudo docker build --tag cv -f Dockerfile_cpu .
 
-sudo docker run -it -v $(pwd):/app cv bash
+sudo docker run -it -p 0.0.0.0:8000:8000 -p 0.0.0.0:8001:8001 -v $(pwd):/app cv bash
+
+```
+
+From inside container
+```bash
+cd deployment
+conda activate cv
+python api_serve.py -n CV -p 8000
 ```
 
 ## Usage
 
 1. Run this python code to pre-download model weights
 
 ```python
 from image2layout_computer_vision import model_dispatch_layout
 model_dispatch_layout._load()
 ```
 
-2. Detect texts
+2. Recognize texts
 
 ```python
 import image2layout_computer_vision as icv
 
-# ImageBoxes object
-imageboxes = icv.detect_text('path/to/image.png')
-# draw annotations
-img_anno = imageboxes.draw_anno()
-
-# boxes_merged = merged boxes (sentences), boxes_raw = all boxes (words)
-boxes_merged, boxes_raw = icv.detect_text_boxes('path/to/image.png')
-
-# merge boxes
-boxes_merged = icv.ImageBoxes.group_boxes(
-    boxes_raw,
-    line_dist_max=1.0,
-    line_dist_min=-0.1,
-    line_iou_min=0.4,
-    row_hdist_max=0.4,
-    row_vdist_max=1.8,
-    row_height_ratio_min=0.8,
-)
+# 2 lists of dicts with keys [text, box, score]
+data_merged, data_raw = detect_text_full('path/to/image.png')
 ```
 
 3. Extract colors
 ```python
 import image2layout_computer_vision as icv
 
 color_bg, color_fg = icv.extract_colors('path/to/image.png')
@@ -112,13 +104,13 @@
 
 
 
 ## Build
 (for building and uploading this package)
 ```bash
 python -m pip install --upgrade pip
-python -m pip install --upgrade build twine
+python -m pip install --upgrade build twine "keyring<19.0"
 
 rm -rf dist
 python -m build
 python -m twine upload dist/* --verbose
 ```
```

### Comparing `image2layout_computer_vision-0.0.9/README.md` & `image2layout_computer_vision-0.1.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 An image processing module for some computer vision tasks (public module for image2layout)
 
 Package Page: [pypi](https://pypi.org/project/image2layout-computer-vision/)
 
 Features:
 
-1. Text Detection
+1. Text Detection and Recognition (OCR)
 2. Color extraction (background and main foreground)
 
 ## Installations
 
 ### Install with `python`/`conda` [Linux]
 
 1. (Optional) Conda
@@ -31,66 +31,58 @@
 sudo apt install tesseract-ocr libtesseract-dev -y
 ```
 
 
 3. Python libraries (python>=3.8)
 
 ```bash
-python -m pip install 'torch>=2.0' torchvision torchaudio
+# python -m pip install 'torch>=2.0' torchvision torchaudio
+conda install pytorch torchvision torchaudio cpuonly -c pytorch --name cv -y
 
 python -m pip install Pillow pandas numpy scikit-learn pyyaml==5.1 chardet pytesseract
 python -m pip install --upgrade datasets transformers
 
 python -m pip install 'git+https://github.com/facebookresearch/detectron2.git'
 
 python -m pip install --upgrade image2layout-computer-vision
 ```
 
 ### Install with `docker`
 
-Replace `Dockerfile_cpu` with `Dockerfile` if running with GPU
-API Implementation is in-progress
+<!-- Replace `Dockerfile_cpu` with `Dockerfile` if running with GPU (not yet supported) -->
 ```bash
 sudo docker build --tag cv -f Dockerfile_cpu .
 
-sudo docker run -it -v $(pwd):/app cv bash
+sudo docker run -it -p 0.0.0.0:8000:8000 -p 0.0.0.0:8001:8001 -v $(pwd):/app cv bash
+
+```
+
+From inside container
+```bash
+cd deployment
+conda activate cv
+python api_serve.py -n CV -p 8000
 ```
 
 ## Usage
 
 1. Run this python code to pre-download model weights
 
 ```python
 from image2layout_computer_vision import model_dispatch_layout
 model_dispatch_layout._load()
 ```
 
-2. Detect texts
+2. Recognize texts
 
 ```python
 import image2layout_computer_vision as icv
 
-# ImageBoxes object
-imageboxes = icv.detect_text('path/to/image.png')
-# draw annotations
-img_anno = imageboxes.draw_anno()
-
-# boxes_merged = merged boxes (sentences), boxes_raw = all boxes (words)
-boxes_merged, boxes_raw = icv.detect_text_boxes('path/to/image.png')
-
-# merge boxes
-boxes_merged = icv.ImageBoxes.group_boxes(
-    boxes_raw,
-    line_dist_max=1.0,
-    line_dist_min=-0.1,
-    line_iou_min=0.4,
-    row_hdist_max=0.4,
-    row_vdist_max=1.8,
-    row_height_ratio_min=0.8,
-)
+# 2 lists of dicts with keys [text, box, score]
+data_merged, data_raw = detect_text_full('path/to/image.png')
 ```
 
 3. Extract colors
 ```python
 import image2layout_computer_vision as icv
 
 color_bg, color_fg = icv.extract_colors('path/to/image.png')
@@ -98,13 +90,13 @@
 
 
 
 ## Build
 (for building and uploading this package)
 ```bash
 python -m pip install --upgrade pip
-python -m pip install --upgrade build twine
+python -m pip install --upgrade build twine "keyring<19.0"
 
 rm -rf dist
 python -m build
 python -m twine upload dist/* --verbose
 ```
```

### Comparing `image2layout_computer_vision-0.0.9/pyproject.toml` & `image2layout_computer_vision-0.1.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   "Pillow",
   "numpy",
   "pandas",
 ]
 
 [project]
 name = "image2layout_computer_vision"
-version = "0.0.9"
+version = "0.1.0"
 authors = [
   { name="Felix Do", email="felix.do.1030@gmail.com" },
 ]
 description = "image processing and stuff"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `image2layout_computer_vision-0.0.9/src/image2layout_computer_vision/color_extract/main.py` & `image2layout_computer_vision-0.1.0/src/image2layout_computer_vision/color_extract/main.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,75 +1,116 @@
 # %%
 import time
 import numpy as np
 import pandas as pd
 from typing import Any, Union, Dict, List, Tuple
 from PIL import Image, ImageDraw, ImageFont, ImageFilter
 
-from sklearn.cluster import KMeans
 
-from ..utils import get_image, COLOR, PixelMask
+from sklearn.cluster import KMeans, MiniBatchKMeans
+
+from ..utils import get_image, COLOR, PixelMask, Chrono, Timer
+
+# %%
+import logging
+debug_logger = logging.getLogger('color_extract')
+c_handler = logging.StreamHandler()
+debug_logger.addHandler(c_handler)
+debug_logger.setLevel(logging.WARNING)
 
 # %%
 class ColorKMeans:
     def __init__(self,
-                colors:Union[np.ndarray, Image.Image],
-                n_clusters:int=2,
-                edge_amounts:list=[0.05, 0.1, 0.15],
-                middle_amounts:list=[0.2, 0.4],
+                colors:Union[np.ndarray, Image.Image, None]=None,
+                colors_yiq:Union[np.ndarray, None]=None,
+                n_clusters:Union[int, None]=2,
+                cluster_centers:Union[np.ndarray, None]=None,
+                edge_amounts:list=[0.05, 0.1],
+                middle_amounts:list=[0.3],
                 ):
+        self.chrono = Chrono(f'ColorKMeans')
+        self.chrono.watch('load')
+        if colors_yiq is not None:
+            assert colors is None
+            self.colors_yiq = colors_yiq
+        else:
+            assert colors is not None
+            self.shape = colors.shape[:-1]
+            self.colors_yiq = COLOR.rgb2yiq(colors)
+        
+        self.shape = self.colors_yiq.shape[:-1]
+        self.colors_yiq_flat = self.colors_yiq.reshape(-1, 3)
+        
         assert n_clusters >= 2
         self.n_clusters = n_clusters
         
-        self.colors = COLOR.get_colors(np.array(colors), 3)
-        self.colors_yiq = COLOR.rgb2yiq(self.colors)
-        self.colors_yiq_flat = self.colors_yiq.reshape(-1, 3)
+        # assert n_clusters is None or n_clusters >= 2
+        # if cluster_centers is None:
+        #     assert isinstance(n_clusters, int)
+        #     assert n_clusters >= 2
+        #     self.n_clusters = n_clusters
+        #     uniques, counts = COLOR.count_unique_colors(self.colors_yiq_flat)
+        #     cluster_centers = uniques[:n_clusters]
+        #     if n_clusters > len(uniques):
+        #         cluster_centers = np.pad(
+        #             cluster_centers, [[0, n_clusters - len(uniques)], [0, 0]],
+        #             mode='edge',
+        #         )
         
-        self.shape = self.colors.shape[:-1]
-        uniques, counts = COLOR.count_unique_colors(self.colors_yiq_flat)
-        n_uniques = uniques.shape[0]
-        assert n_uniques > 0, f'`data` is either empty or invalid'
-        # if n_uniques == 1:
-        #     return np.zeros(shape, int), uniques[0]
-        assert n_clusters <= n_uniques
-    
+        # self.n_clusters = len(cluster_centers)
+        
+        self.chrono.watch('fit')
         self.model = KMeans(
-            n_clusters=n_clusters,
-            n_init='auto',
-            init=uniques[:n_clusters],
+            n_clusters=self.n_clusters,
+            n_init=1,
+            init=cluster_centers,
+            # n_init=2,
+            max_iter=60,
         )
+        # self.model = MiniBatchKMeans(
+        #     n_clusters=self.n_clusters,
+        #     n_init=1,
+        #     init=cluster_centers,
+        #     max_iter=20,
+        # )
         cluster_indices = self.model.fit_predict(self.colors_yiq_flat)
+        
+        self.chrono.watch('post')
         self.cluster_map = cluster_indices.reshape(self.shape)
         
         self.cluster_onehot = self.cluster_map[:, :, None] == np.arange(self.n_clusters)
         
         self.cluster_centers_yiq = self.model.cluster_centers_
         self.cluster_centers = COLOR.yiq2rgb(self.cluster_centers_yiq)
         
+        self.chrono.watch('score_prep')
         self.center_dists = np.linalg.norm(
             self.cluster_centers_yiq[None] - self.cluster_centers_yiq[:, None],
             axis=-1,
         )
         self.center_dist_max = self.center_dists.max()
         self.center_dists_nonzero = self.center_dists[
             np.logical_not(PixelMask.diagonal_mask(self.n_clusters))
         ].reshape(self.n_clusters, self.n_clusters-1)
         
+        self.chrono.watch('error')
         self.cluster_errors = np.array([
             np.linalg.norm(
                 self.colors_yiq[self.cluster_map == cluster_index] - self.cluster_centers_yiq[cluster_index][None],
                 axis=-1
             ).mean()
             for cluster_index in range(self.n_clusters)
         ])
         self.cluster_errors_ratio = self.cluster_errors / self.center_dist_max
         
+        self.chrono.watch('score')
         self.edge_scores = self.compute_scores_from_dist(amount=edge_amounts, from_edge=True)
         self.middle_scores = self.compute_scores_from_dist(amount=middle_amounts, from_edge=False)
         self.areas = self.cluster_onehot.mean(0).mean(0)
+        
     
     def __repr__(self) -> str:
         info = ' | '.join([
             f'{k}{v.round(3)}'
             for k, v in {
                 'areas': self.areas,
                 'errors_r': self.cluster_errors_ratio,
@@ -96,127 +137,234 @@
         _scores = np.zeros(self.n_clusters, float)
         _scores[_indices] = _counts / _counts.sum()
         return _scores
 
 # %%
 class ColorExtractor:
     def __init__(self,
-                image:Image.Image, 
-                n_clusters_max=5,
-                n_clusters_min=2,
+                image:Image.Image,
+                n_clusters_max=4,
+                n_clusters_min=4,
                 with_foreground=True,
                 **kwargs,
                 ):
         '''
         Parameters:
             n_clusters_min / n_clusters_max (int): range of values for KMeans n_clusters
             with_foreground (bool): whether to extract foreground color
             kwargs:
                 bg_error_ratio_max [0.05]
                 unique_ratio_min [0.5]
         '''
+        _id = np.random.choice(list('0123456789'), 10)
+        self.chrono = Chrono(f'ColorExtractor_{_id}')
+        
+        self.chrono.watch('load')
+        
         self.image = get_image(image).convert('RGB')
         self.size = self.image.size
         self.shape = np.array(self.image.size[::-1])
         
+        self.chrono.watch('score')
         self.extracted_data = self.extract_colors_from_scores_and_dist(
             image=self.image,
             n_clusters_max=n_clusters_max,
             n_clusters_min=n_clusters_min,
             with_foreground=with_foreground,
-            force_run_all=False,
             **kwargs,
         )
+        self.chrono.watch('map')
         self.extract_map = self.extracted_data['extract_map']
-        self.color_bg = tuple(self.extracted_data['color_bg'])
-        self.color_fg = tuple(self.extracted_data['color_fg'])
+        self.color_bg = tuple([int(v) for v in self.extracted_data['color_bg']])
+        self.color_fg = tuple([int(v) for v in self.extracted_data['color_fg']])
         self.colors = (self.color_bg, self.color_fg)
+        self.image_anno = None
+        
+        self.chrono.watch()
+        
+        debug_logger.debug(msg=f'ColorExtractor [{self.size[0]}x{self.size[1]}] > timers: ' + ' '.join([
+            f"{'.'.join(k)}[{v.time_total:.3f}]"
+            for k, v in self.chrono.timers.items()
+        ]))
     
     def __repr__(self) -> str:
         return f'ColorExtractor[{self.shape}]({self.color_bg} | {self.color_fg})'
     
     def draw_anno(self,):
-        img_anno_np = np.zeros([*self.shape, 4], np.uint8)
-        img_anno_np[self.extract_map == 0] = [*self.color_bg, 255]
-        img_anno_np[self.extract_map == 1] = [*self.color_fg, 255]
-        img_anno = Image.fromarray(img_anno_np, 'RGBA')
+        _transparent_contrast = 32
+        img_anno_np = np.zeros([*self.shape, 3], np.uint8) + (128 - _transparent_contrast)
+        mask_checker = PixelMask.checkerboard([*self.shape], int(max(min(self.shape) // 20, 4)))
+        img_anno_np[mask_checker] = [128 + _transparent_contrast] * 3
+        # img_anno_np[np.logical_not(mask_checker)] = [128 - _transparent_contrast] * 3
+        img_anno_np[self.extract_map == 0] = [*self.color_bg]
+        img_anno_np[self.extract_map == 1] = [*self.color_fg]
+        img_anno = Image.fromarray(img_anno_np, 'RGB')
+        self.image_anno = img_anno
         return img_anno
 
     @classmethod
     def get_primary_color(cls, colors:np.ndarray, unique_ratio_min=0.5):
         '''
         Parameters:
             colors: (np.ndarray) [..., 3] RGB colors
         '''
+        # time_perf_0 = time.perf_counter()
+        
         _colors = COLOR.get_colors(colors, 3).reshape(-1, 3)
-        uniques, counts = COLOR.count_unique_colors(_colors)
-        ratios = counts / counts.sum()
-        if ratios[0] >= unique_ratio_min:
-            return uniques[0]
-        colors_yiq = COLOR.rgb2yiq(_colors)
-        avg_color_yiq = colors_yiq.mean(0)
-        avg_color = COLOR.yiq2rgb(avg_color_yiq)
+        # uniques, counts = COLOR.count_unique_colors(_colors)
+        # ratios = counts / counts.sum()
+        # if ratios[0] >= unique_ratio_min:
+        #     time_perf_1 = time.perf_counter()
+        #     return uniques[0]
+        # colors_yiq = COLOR.rgb2yiq(_colors)
+        # avg_color_yiq = colors_yiq.mean(0)
+        # avg_color = COLOR.yiq2rgb(avg_color_yiq)
+        
+        # time_perf_1 = time.perf_counter()
+        
+        avg_color = _colors.mean(0).astype(np.uint8)
         return avg_color
     
     @classmethod
     def extract_colors_from_scores_and_dist(cls,
                 image,
                 n_clusters_max=5,
                 n_clusters_min=2,
                 bg_error_ratio_max=0.05,
                 with_foreground=True,
                 unique_ratio_min=0.5,
-                force_run_all=False,
                 **kwargs
                 ):
-        assert n_clusters_max >= n_clusters_min, f'n_clusters_max[{n_clusters_max}] >= n_clusters_min[{n_clusters_min}]'
-        data = []
-        _img = get_image(image).convert('RGB')
+        chrono = Chrono(f'ColorExtractor.extract_colors_from_scores_and_dist')
+        
+        chrono.watch('load')
+        assert n_clusters_max >= n_clusters_min >= 2, f'n_clusters_max[{n_clusters_max}] >= n_clusters_min[{n_clusters_min}] >= 2'
+        # data = []
+        assert isinstance(image, Image.Image)
+        assert image.mode == 'RGB'
+        if isinstance(image, Image.Image):
+            colors = COLOR.get_colors(np.array(image.convert('RGB')), 3)
+        # else:
+        #     assert isinstance(image, np.ndarray)
+        #     colors = COLOR.get_colors(image, 3)
+        
+        chrono.watch('convert')
+        # colors_yiq = COLOR.rgb2yiq(colors)
+        # colors_yiq_flat = colors_yiq.reshape(-1, 3)
+        shape = colors.shape[:-1]
+        
+        chrono.watch('count')
+        # _round_scale = 20
+        # colors_yiq_round = np.round(colors_yiq * _round_scale).astype(int)
+        # uniques_yiq_round, counts = COLOR.count_unique_colors(colors_yiq_round)
+        # uniques_yiq = uniques_yiq_round / _round_scale
+        
+        # TODO: experiment with ratios_cumsum for n_clusters selection ??
+        # ratios = counts / counts.sum()
+        # ratios_cumsum = np.cumsum(ratios)
+        
+        uniques_rgb = np.array([
+            v[1]
+            for v in sorted(image.getcolors(np.prod(image.size)))[-n_clusters_max:][::-1]
+        ], np.uint8)
+        chrono.watch('pre_cluster')
+        d_out = {
+            'n_clusters': 0,
+            'bg_passed': True,
+            'bg_error': 0.,
+            'color_bg': (255, 255, 255),
+            'color_fg': (0, 0, 0),
+            'extract_map': np.zeros(shape, bool), 
+        }
+        
+        n_uniques = len(uniques_rgb)
+        if n_uniques == 0:
+            return d_out
+        if n_uniques == 1:
+            d_out['color_bg'] = tuple([int(v) for v in n_uniques[0]])
+            return d_out
+        # n_clusters_max = min(n_clusters_max, n_uniques)
+        # n_clusters_min = min(n_clusters_min, n_clusters_max)
+        # if n_uniques < 2 or n_clusters_max < 2 or n_clusters_min < 2:
+        #     return d_out
+        
+        assert len(uniques_rgb) >= 2, f'must have 2 unique colors at this point'
+        n_clusters_max = min(n_clusters_max, n_uniques)
+        n_clusters_min = min(n_clusters_min, n_clusters_max)
+        
+        chrono.watch('cluster')
         for n_clusters in range(n_clusters_min, n_clusters_max+1):
-            ckm = ColorKMeans(_img, n_clusters=n_clusters, **kwargs)
-            extract_map = np.zeros(ckm.shape, int) - 1
+            chrono.watch('cluster', str(n_clusters))
+            # _cluster_centers = uniques_yiq[:n_clusters]
             
+            chrono.watch('cluster', str(n_clusters), 'CKM')
+            ckm = ColorKMeans(
+                # colors_yiq=colors_yiq,
+                colors_yiq=colors,
+                n_clusters=n_clusters,
+                # cluster_centers=_cluster_centers,
+                cluster_centers=uniques_rgb[:n_clusters],
+                **kwargs,
+            )
+            extract_map = np.zeros(shape, int) - 1
+            
+            chrono.watch('cluster', str(n_clusters), 'bg')
             bg_scores = ckm.edge_scores + ckm.areas / 4
             bg_order = np.argsort(bg_scores)[::-1]
             bg_index = bg_order[0]
             bg_mask = ckm.cluster_map == bg_index
-            bg_color = cls.get_primary_color(ckm.colors[bg_mask], unique_ratio_min=unique_ratio_min)
-            extract_map[bg_mask] = 0
             
-            bg_error = ckm.cluster_errors_ratio[bg_index]
-            bg_passed = bg_error <= bg_error_ratio_max
+            if bg_mask.sum() > 0:
+                chrono.watch('cluster', str(n_clusters), 'bg_primary')
+                bg_color = cls.get_primary_color(colors[bg_mask], unique_ratio_min=unique_ratio_min)
+                extract_map[bg_mask] = 0
+                bg_error = ckm.cluster_errors_ratio[bg_index]
+                bg_passed = bg_error <= bg_error_ratio_max
+            else:
+                bg_color = (255, 255, 255)
+                bg_error = 100.
+                bg_passed = False
             
-            fg_color = np.zeros(3, np.uint8)
+            fg_color = (0, 0, 0)
             if with_foreground:
+                chrono.watch('cluster', str(n_clusters), 'fg')
                 fg_scores = ckm.middle_scores + ckm.areas / 10
                 fg_order = np.argsort(fg_scores)[::-1]
                 fg_index = [v for v in fg_order if v != bg_index][0]
                 fg_mask = ckm.cluster_map == fg_index
-                extract_map[fg_mask] = 1
-                fg_color = cls.get_primary_color(ckm.colors[fg_mask], unique_ratio_min=unique_ratio_min)
+                
+                chrono.watch('cluster', str(n_clusters), 'fg_primary')
+                if fg_mask.sum() > 0:
+                    extract_map[fg_mask] = 1
+                    fg_color = cls.get_primary_color(colors[fg_mask], unique_ratio_min=unique_ratio_min)
             
-            d = {
+            d_out = {
                 'n_clusters': n_clusters,
                 'bg_passed': bg_passed,
                 'bg_error': bg_error,
-                'color_bg': bg_color,
-                'color_fg': fg_color,
-                # 'ckm': ckm,
+                'color_bg': tuple([int(v) for v in bg_color]),
+                'color_fg': tuple([int(v) for v in fg_color]),
                 'extract_map': extract_map, 
             }
-            data.append(d)
+            # data.append(d_out)
             del ckm
             
-            if not force_run_all and bg_passed:
-                return d
-            
-        else:
-            if not force_run_all:
-                return d
-        return data
+            chrono.watch('cluster', str(n_clusters))
+            if bg_passed:
+                break
+        
+        chrono.watch('cluster')
+        chrono.watch()
+        
+        debug_logger.debug(msg=f'extract_colors... [{shape[1]}x{shape[0]}] > timers(ms): ' + ' '.join([
+            f"{'.'.join(k)}[{v.time_total*1000:.0f}]"
+            for k, v in chrono.timers.items()
+        ]))
+        
+        return d_out
 
 
 # %%
 def extract_colors(image) -> Tuple[tuple]:
     img = get_image(image)
     color_extractor = ColorExtractor(img)
     return color_extractor.colors
```

### Comparing `image2layout_computer_vision-0.0.9/src/image2layout_computer_vision/ocr/imagebox.py` & `image2layout_computer_vision-0.1.0/src/image2layout_computer_vision/ocr/imagebox.py`

 * *Files 9% similar despite different names*

```diff
@@ -171,27 +171,35 @@
 class ImageBoxes(list):
     mask_color = tuple([0, 0, 0])
     mask_opacity = 0.5
     box_colors = [
         tuple([int(v * 255) for v in colorsys.hsv_to_rgb(i/3, 1.0, 1.0)])
         for i in range(3)
     ]
-    def __init__(self, boxes:list, image=None, size=None, offset=(0, 0), level=0):
+    def __init__(self,
+                boxes:list,
+                image=None,
+                size=None,
+                offset=(0, 0),
+                level=0,
+                parent=None,
+                ):
         '''
         image (PIL.Image.Image RGB): input image
         boxes (list): list of (lists of...) ints for xyxy coordinates
         '''
         
+        self.parent = parent
         self.offset = np.array(offset, int)
+        self.text = ''
+        self.texts = []
         
         if isinstance(boxes, np.ndarray):
             boxes = boxes.tolist()
-        if not isinstance(boxes, list):
-            print(f'found `boxes`<{type(boxes)}>: {boxes}')
-        assert isinstance(boxes, list), f'{boxes}'
+        assert isinstance(boxes, list), f'`boxes` must be of type [list, np.ndarray], found {type(boxes)}'
         
         self.is_single_instance = len(boxes) == 4 and all([isinstance(v, int) for v in boxes])
         self.image = get_image(image) if image is not None else None
         if self.image is not None:
             self.size = self.image.size
         else:
             assert size is not None
@@ -214,24 +222,24 @@
         else:
             imageboxes = []
             for i, box in enumerate(boxes):
                 child_imageboxes = ImageBoxes(
                     boxes=box,
                     size=self.size,
                     level=self.level + 1,
+                    parent=self,
                 )
                 imageboxes.append(child_imageboxes)
                 self.boxes.extend(child_imageboxes.boxes)
                 self.boxes_top.append(child_imageboxes.box_outer.tolist())
                 
                 if not self.box_outer_found:
                     self.box_outer_found = True
                     self.box_outer = np.array(child_imageboxes.box_outer, int)
                 else:
-                    # print(self.box_outer, child_imageboxes.box_outer)
                     self.box_outer[:2] = np.min([self.box_outer[:2], child_imageboxes.box_outer[:2]], axis=0)
                     self.box_outer[2:] = np.max([self.box_outer[2:], child_imageboxes.box_outer[2:]], axis=0)
                 
             self.box = np.array(self.box_outer, int)
             super().__init__(imageboxes)
     
     def _repr(self) -> list:
@@ -247,39 +255,92 @@
                 ],
                 ')',
             ]
         
     def __repr__(self) -> str:
         return '\n'.join(self._repr())
     
-    def set_text(self, text):
-        assert isinstance(text, list)
-        for child, _text in zip(self, text):
-            child.set_text(_text)
+    def set_texts(self, texts:list, update_from_children=True):
+        assert isinstance(texts, list), f''
+        assert len(texts) > 0
+        if self.is_single_instance:
+            _text = str(texts[0])
+            self.text = _text
+            self.texts = [_text]
+        else:
+            box_count = len(self.boxes)
+            assert len(texts) == box_count, 'len of texts does not match len of self.boxes'
+            _index_offset = 0
+            for child in self:
+                child_box_count = len(child.boxes)
+                _texts = texts[_index_offset: _index_offset+child_box_count]
+                child.set_texts(_texts, update_from_children=False)
+                _index_offset += child_box_count
+            
+            if update_from_children:
+                self.update_texts_from_children()
+    
+    def update_texts_from_children(self):
+        if not self.is_single_instance:
+            self.texts = []
+            for child in self:
+                _texts = child.update_texts_from_children()
+                self.texts.extend(_texts)
+            self.text = ' '.join(self.texts)
+        return self.texts
     
     @property
     def images(self):
         return [child.image for child in self]
     
     @property
-    def text(self):
+    def text_all(self):
+        if self.is_single_instance:
+            return self.text
         return ' '.join([
-            child.text if child.text is not None else '<>'
+            child.text_all if child.text_all else '<>'
             for child in self
         ])
     
     @property
     def df(self):
-        data = [
-            {
-                'text': child.text,
-                'box': child.box,
-            }
-            for child in self
-        ]
+        if self.is_single_instance:
+            data = [{
+                'index': 0,
+                'box': self.boxes[0],
+                'text': self.text,
+            }]
+        else:
+            data = [
+                {
+                    'index': i,
+                    'box': _box,
+                    'text': _text,
+                }
+                for i, (_box, _text) in enumerate(zip(self.boxes, self.texts))
+            ]
+        return pd.DataFrame(data)
+    
+    @property
+    def df_top(self):
+        if self.is_single_instance:
+            data = [{
+                'index': 0,
+                'box': self.boxes[0],
+                'text': self.text,
+            }]
+        else:
+            data = [
+                {
+                    'index': i,
+                    'box': child.box_outer,
+                    'text': child.text,
+                }
+                for i, child in enumerate(self)
+            ]
         return pd.DataFrame(data)
     
     def draw_anno(self,
                 width=2,
                 mode='box',
                 draw_image=True,
                 draw_level_0=False,
@@ -322,14 +383,15 @@
         else:
             boxes_nested_final = np.array(self.boxes)
         
         imageboxes_nested = ImageBoxes(
             boxes=boxes_nested_final,
             image=self.image.copy(),
         )
+        imageboxes_nested.set_texts(self.texts)
         return imageboxes_nested
     
     @classmethod
     def group_boxes(cls,
                 boxes:Union[np.ndarray, list],
                 line_dist_max:float=1.0,
                 line_dist_min:float=-0.1,
```

### Comparing `image2layout_computer_vision-0.0.9/src/image2layout_computer_vision/ocr/main.py` & `image2layout_computer_vision-0.1.0/src/image2layout_computer_vision/ocr/main.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,66 +2,99 @@
 import time
 import json
 import os
 import numpy as np
 import pandas as pd
 from PIL import Image
 from typing import Union, Any, List, Dict, Tuple
-from .model_layoutmlv2 import ModelDispatch_LayoutMLv2
 from ..utils import get_image, ImageConvert
 from .imagebox import ImageBoxes, BoxMerge
 
 # %%
-model_dispatch_layout = ModelDispatch_LayoutMLv2(
+import logging
+debug_logger = logging.getLogger('ocr')
+c_handler = logging.StreamHandler()
+debug_logger.addHandler(c_handler)
+debug_logger.setLevel(logging.WARNING)
+
+# %%
+# from .model_layoutmlv2 import ModelDispatch_LayoutMLv2
+# model_dispatch_layout = ModelDispatch_LayoutMLv2(
+#     device='cpu',
+# )
+
+# %%
+from .model_paddle import ModelDispatch_Paddle
+model_dispatch_paddle = ModelDispatch_Paddle(
     device='cpu',
 )
 
 # %%
-def detect_text(image: Union[Image.Image, np.ndarray], **kwargs) -> ImageBoxes:
+model_dispatch = model_dispatch_paddle
+
+# %%
+def detect_text(image: Union[Image.Image, np.ndarray], merge_boxes=True, **kwargs) -> ImageBoxes:
     '''predict boxes for text in the image
     Parameters:
         image: (PIL.Image.Image, np.ndarray) RGB image
         **kwargs:
             line_dist_max:          max distance between boxes to be in the same sentence (as a ratio of line height)
             line_dist_min:          min (negative) distance between boxes to be in the same sentence (as a ratio of line height)
             line_iou_min:           min vertical iou between boxes to be on the same line
             row_hdist_max:          max horizontal offset between rows to aligned as a column (as a ratio of line height)
             row_vdist_max:          max vertical distance between rows to be in the same column (as a ratio of line height)
             row_height_ratio_min:   min ratio between heights of rows to be in the same column
     Returns:
         imageboxes: (ImageBoxes) object containing prediction boxes
     '''
     _image = get_image(image).convert('RGB')
+    debug_logger.debug(msg=f'detect_text | input[{_image.size}]')
     
-    true_predictions, true_boxes = model_dispatch_layout(_image)
-    true_boxes_np = np.array(true_boxes, int)
-    true_boxes_check = np.all(true_boxes_np[:, 2:] > true_boxes_np[:, :2], axis=-1)
-    true_boxes_np = true_boxes_np[true_boxes_check]
+    result_df = model_dispatch_paddle(_image)
     
     imageboxes_raw = ImageBoxes(
         image=_image,
-        boxes=true_boxes_np.tolist(),
+        boxes=result_df['box'].tolist(),
     )
-    imageboxes = imageboxes_raw.to_grouped_imageboxes(**kwargs)
-    return imageboxes
+    if merge_boxes:
+        imageboxes = imageboxes_raw.to_grouped_imageboxes(**kwargs)
+        debug_logger.debug(msg=f'detect_text | merged[{len(imageboxes_raw.boxes_top)} -> {len(imageboxes.boxes_top)}]')
+        return imageboxes
+    
+    return imageboxes_raw
 
+# %%
 def detect_text_boxes(image: Union[Image.Image, np.ndarray], **kwargs) -> Tuple[np.ndarray, np.ndarray]:
     '''predict boxes for text in the image
     Parameters: (same as detect_text)
     Returns:
         boxes_merged: (np.ndarray) [M, 4] text boxes detected, merged boxes
         boxes_raw:    (np.ndarray) [N, 4] text boxes detected, all individual boxes (N >= M)
     '''
     imageboxes = detect_text(image, **kwargs)
     
     boxes_merged = np.array(imageboxes.boxes_top, int)
     boxes_raw = np.array(imageboxes.boxes, int)
     return boxes_merged, boxes_raw
 
 # %%
+def detect_text_full(image: Union[Image.Image, np.ndarray], **kwargs) -> List[Dict]:
+    _image = get_image(image).convert('RGB')
+    result_df = model_dispatch_paddle(image)
+    result_data = result_df.to_dict('records')
+    imageboxes_raw = ImageBoxes(
+        image=_image,
+        boxes=result_df['box'].tolist(),
+    )
+    imageboxes_raw.set_texts(result_df['text'].tolist())
+    imageboxes_merged = imageboxes_raw.to_grouped_imageboxes(**kwargs)
+    
+    return imageboxes_merged.df_top.to_dict('records'), imageboxes_raw.df_top.to_dict('records')
+
+# %%
 if __name__ == '__main__':
     imageboxes = detect_text('data/inputs/SCR-20230710-ixfw.jpeg')
     
     imageboxes.draw_anno(width=3)
     
     boxes_merged = np.array(imageboxes.boxes_top, int)
     boxes_raw = np.array(imageboxes.boxes, int)
```

### Comparing `image2layout_computer_vision-0.0.9/src/image2layout_computer_vision/ocr/model_layoutmlv2.py` & `image2layout_computer_vision-0.1.0/src/image2layout_computer_vision/ocr/model_layoutmlv2.py`

 * *Files identical despite different names*

### Comparing `image2layout_computer_vision-0.0.9/src/image2layout_computer_vision/utils/color_system.py` & `image2layout_computer_vision-0.1.0/src/image2layout_computer_vision/utils/color_system.py`

 * *Files identical despite different names*

### Comparing `image2layout_computer_vision-0.0.9/src/image2layout_computer_vision/utils/pixel_mask.py` & `image2layout_computer_vision-0.1.0/src/image2layout_computer_vision/utils/pixel_mask.py`

 * *Files 22% similar despite different names*

```diff
@@ -51,7 +51,20 @@
         '''
         coords = cls.coordinates(shape=shape)
         mid_pos = (np.array(shape) - 1) / 2
         dist_map_yx = (coords - mid_pos) / mid_pos
         dist_map = np.linalg.norm(dist_map_yx, axis=-1)
         dist_map /= np.clip(dist_map.max(), 0.000001, None)
         return dist_map
+    
+    @classmethod
+    def checkerboard(cls, shape=(10, 10), cell_size:int=10) -> np.ndarray:
+        '''
+        Parameters:
+            cell_size: (int) the size of the checkerboard cells
+        Return:
+            checker_mask: [H, W] (bool) checkerboard mask
+        '''
+        coords = PixelMask.coordinates(shape=shape).astype(float)
+        coord_mod = np.floor(coords / cell_size).astype(int) % 2
+        checker_mask = coord_mod[:, :, 0] == coord_mod[:, :, 1]
+        return checker_mask
```

### Comparing `image2layout_computer_vision-0.0.9/src/image2layout_computer_vision.egg-info/PKG-INFO` & `image2layout_computer_vision-0.1.0/src/image2layout_computer_vision.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: image2layout-computer-vision
-Version: 0.0.9
+Version: 0.1.0
 Summary: image processing and stuff
 Author-email: Felix Do <felix.do.1030@gmail.com>
 Project-URL: Homepage, https://github.com/felix-do-wizardry/image2layout-computer-vision
 Project-URL: Bug Tracker, https://github.com/felix-do-wizardry/image2layout-computer-vision
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -16,15 +16,15 @@
 
 An image processing module for some computer vision tasks (public module for image2layout)
 
 Package Page: [pypi](https://pypi.org/project/image2layout-computer-vision/)
 
 Features:
 
-1. Text Detection
+1. Text Detection and Recognition (OCR)
 2. Color extraction (background and main foreground)
 
 ## Installations
 
 ### Install with `python`/`conda` [Linux]
 
 1. (Optional) Conda
@@ -45,66 +45,58 @@
 sudo apt install tesseract-ocr libtesseract-dev -y
 ```
 
 
 3. Python libraries (python>=3.8)
 
 ```bash
-python -m pip install 'torch>=2.0' torchvision torchaudio
+# python -m pip install 'torch>=2.0' torchvision torchaudio
+conda install pytorch torchvision torchaudio cpuonly -c pytorch --name cv -y
 
 python -m pip install Pillow pandas numpy scikit-learn pyyaml==5.1 chardet pytesseract
 python -m pip install --upgrade datasets transformers
 
 python -m pip install 'git+https://github.com/facebookresearch/detectron2.git'
 
 python -m pip install --upgrade image2layout-computer-vision
 ```
 
 ### Install with `docker`
 
-Replace `Dockerfile_cpu` with `Dockerfile` if running with GPU
-API Implementation is in-progress
+<!-- Replace `Dockerfile_cpu` with `Dockerfile` if running with GPU (not yet supported) -->
 ```bash
 sudo docker build --tag cv -f Dockerfile_cpu .
 
-sudo docker run -it -v $(pwd):/app cv bash
+sudo docker run -it -p 0.0.0.0:8000:8000 -p 0.0.0.0:8001:8001 -v $(pwd):/app cv bash
+
+```
+
+From inside container
+```bash
+cd deployment
+conda activate cv
+python api_serve.py -n CV -p 8000
 ```
 
 ## Usage
 
 1. Run this python code to pre-download model weights
 
 ```python
 from image2layout_computer_vision import model_dispatch_layout
 model_dispatch_layout._load()
 ```
 
-2. Detect texts
+2. Recognize texts
 
 ```python
 import image2layout_computer_vision as icv
 
-# ImageBoxes object
-imageboxes = icv.detect_text('path/to/image.png')
-# draw annotations
-img_anno = imageboxes.draw_anno()
-
-# boxes_merged = merged boxes (sentences), boxes_raw = all boxes (words)
-boxes_merged, boxes_raw = icv.detect_text_boxes('path/to/image.png')
-
-# merge boxes
-boxes_merged = icv.ImageBoxes.group_boxes(
-    boxes_raw,
-    line_dist_max=1.0,
-    line_dist_min=-0.1,
-    line_iou_min=0.4,
-    row_hdist_max=0.4,
-    row_vdist_max=1.8,
-    row_height_ratio_min=0.8,
-)
+# 2 lists of dicts with keys [text, box, score]
+data_merged, data_raw = detect_text_full('path/to/image.png')
 ```
 
 3. Extract colors
 ```python
 import image2layout_computer_vision as icv
 
 color_bg, color_fg = icv.extract_colors('path/to/image.png')
@@ -112,13 +104,13 @@
 
 
 
 ## Build
 (for building and uploading this package)
 ```bash
 python -m pip install --upgrade pip
-python -m pip install --upgrade build twine
+python -m pip install --upgrade build twine "keyring<19.0"
 
 rm -rf dist
 python -m build
 python -m twine upload dist/* --verbose
 ```
```

### Comparing `image2layout_computer_vision-0.0.9/src/image2layout_computer_vision.egg-info/SOURCES.txt` & `image2layout_computer_vision-0.1.0/src/image2layout_computer_vision.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 LICENSE
 README.md
 pyproject.toml
 src/sandbox.py
+src/sandbox_color.py
 src/sandbox_ocr.py
-src/test.py
+src/test_color.py
 src/image2layout_computer_vision/__init__.py
 src/image2layout_computer_vision.egg-info/PKG-INFO
 src/image2layout_computer_vision.egg-info/SOURCES.txt
 src/image2layout_computer_vision.egg-info/dependency_links.txt
 src/image2layout_computer_vision.egg-info/top_level.txt
 src/image2layout_computer_vision/color_extract/__init__.py
 src/image2layout_computer_vision/color_extract/main.py
 src/image2layout_computer_vision/ocr/__init__.py
 src/image2layout_computer_vision/ocr/imagebox.py
 src/image2layout_computer_vision/ocr/main.py
 src/image2layout_computer_vision/ocr/model_layoutmlv2.py
+src/image2layout_computer_vision/ocr/model_paddle.py
 src/image2layout_computer_vision/utils/__init__.py
 src/image2layout_computer_vision/utils/annotation.py
 src/image2layout_computer_vision/utils/color_system.py
 src/image2layout_computer_vision/utils/imaging.py
-src/image2layout_computer_vision/utils/pixel_mask.py
+src/image2layout_computer_vision/utils/pixel_mask.py
+src/image2layout_computer_vision/utils/timing.py
```

### Comparing `image2layout_computer_vision-0.0.9/src/sandbox.py` & `image2layout_computer_vision-0.1.0/src/sandbox.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,38 @@
 # %%
 import os, time, string, json
 import numpy as np
 import pandas as pd
 from PIL import Image
+import image2layout_computer_vision as icv
+
+# %%
+fp = '/home/test/code/image2layout_computer_vision/data/inputs/image 559.png'
+img = icv.get_image(fp)
+img
+
+# %%
+CE = icv.ColorExtractor(img)
+CE
+
+# %%
+CE.color_clusters_df
+
+# %%
+
+
+
+
+
+
+# %%
+import os, time, string, json
+import numpy as np
+import pandas as pd
+from PIL import Image
 import plotly.express as px
 import plotly.io as pio
 pio.templates.default = 'plotly_dark'
 
 from image2layout_computer_vision import get_image, COLOR, PixelMask
 from image2layout_computer_vision.color_extract import (
     kmeans_cluster_colors,
@@ -104,15 +130,15 @@
             })
         
         color_clusters_df = pd.DataFrame(cluster_hist_data).sort_values('bg_score', ascending=False)
         
         return color_clusters_df
 
 # %%
-fp = '../data/inputs/image 559.png'
+fp = '/home/test/code/image2layout_computer_vision/data/inputs/image 559.png'
 img = get_image(fp).convert('RGB')
 shape = img.size[::-1]
 img
 
 # %%
 cluster_df = ColorExtractor.analyze_colors_kmeans(img, 2)
 cluster_df
@@ -230,138 +256,59 @@
         _mask = PixelMask.edge_mask(shape=self.shape, amount=float(amount))
         if not from_edge:
             _mask = np.logical_not(_mask)
         _indices, _counts = COLOR.count_uniques(self.cluster_map[_mask])
         _scores = np.zeros(self.n_clusters, float)
         _scores[_indices] = _counts / _counts.sum()
         return _scores
+    
+ckm = ColorKMeans(img, 3)
+ckm
 
 # %%
-def get_primary_color(colors:np.ndarray, unique_ratio_min=0.5):
-    '''
-    Parameters:
-        colors: (np.ndarray) [..., 3] RGB colors
-    '''
-    _colors = COLOR.get_colors(colors, 3).reshape(-1, 3)
-    uniques, counts = COLOR.count_unique_colors(_colors)
-    ratios = counts / counts.sum()
-    if ratios[0] >= unique_ratio_min:
-        return uniques[0]
-    colors_yiq = COLOR.rgb2yiq(_colors)
-    avg_color_yiq = colors_yiq.mean(0)
-    avg_color = COLOR.yiq2rgb(avg_color_yiq)
-    return avg_color
-
-# %%
-def extract_colors_from_scores_and_dist(
-            img,
-            n_clusters_max=5,
-            n_clusters_min=2,
-            bg_error_ratio_max=0.05,
-            with_foreground=True,
-            unique_ratio_min=0.5,
-            force_run_all=False,
-            **kwargs
-            ):
-    assert n_clusters_max >= n_clusters_min, f'n_clusters_max[{n_clusters_max}] >= n_clusters_min[{n_clusters_min}]'
-    data = []
-    _img = get_image(img).convert('RGB')
-    for n_clusters in range(n_clusters_min, n_clusters_max+1):
-        ckm = ColorKMeans(_img, n_clusters=n_clusters, **kwargs)
-        extract_map = np.zeros(ckm.shape, int) - 1
-        
-        bg_scores = ckm.edge_scores + ckm.areas / 4
-        bg_order = np.argsort(bg_scores)[::-1]
-        bg_index = bg_order[0]
-        bg_mask = ckm.cluster_map == bg_index
-        bg_color = get_primary_color(ckm.colors[bg_mask], unique_ratio_min=unique_ratio_min)
-        extract_map[bg_mask] = 0
-        # px.imshow(bg_mask)
-        
-        bg_error = ckm.cluster_errors_ratio[bg_index]
-        bg_passed = bg_error <= bg_error_ratio_max
-        
-        fg_color = None
-        if with_foreground:
-            fg_scores = ckm.middle_scores + ckm.areas / 10
-            fg_order = np.argsort(fg_scores)[::-1]
-            fg_index = [v for v in fg_order if v != bg_index][0]
-            fg_mask = ckm.cluster_map == fg_index
-            extract_map[fg_mask] = 1
-            # px.imshow(fg_mask)
-            fg_color = get_primary_color(ckm.colors[fg_mask], unique_ratio_min=unique_ratio_min)
-        
-        d = {
-            'n_clusters': n_clusters,
-            'bg_passed': bg_passed,
-            'bg_error': bg_error,
-            'bg_color': bg_color,
-            'fg_color': fg_color,
-            # 'ckm': ckm,
-            'extract_map': extract_map, 
-        }
-        data.append(d)
-        del ckm
-        
-        if not force_run_all and bg_passed:
-            return d
-        
-    else:
-        if not force_run_all:
-            return d
-    return data
-
-
-data = extract_colors_from_scores_and_dist(
-    # '/Users/felixdo/Documents/Code/AI/image2layout-computer-vision/data/inputs/Screenshot 2023-07-26 at 14.18.22.png',
-    # '/Users/felixdo/Documents/Code/AI/image2layout-computer-vision/data/inputs/Screenshot 2023-07-26 at 14.22.06.png',
-    img_r2,
-    n_clusters_min=2,
-    n_clusters_max=3,
-)
-data
+bg_scores = ckm.edge_scores + ckm.areas / 4
+bg_order = np.argsort(bg_scores)[::-1]
+bg_index = bg_order[0]
+bg_mask = ckm.cluster_map == bg_index
+px.imshow(bg_mask)
 
 # %%
-for d in data:
-    # d['n_clusters']
-    fig = px.imshow(
-        img=d['extract_map'],
-        zmin=-1, zmax=1,
-        color_continuous_scale=[
-            '#808080',
-            COLOR.rgb2hex(d['bg_color']),
-            COLOR.rgb2hex(d['fg_color']),
-        ],
-    )
-    fig.update_layout(
-        title=f"n={d['n_clusters']} passed={d['bg_passed']}",
-    )
-    fig.show()
-
-# %%
-img_anno_np = np.zeros([*img_r2.size[::-1], 4], np.uint8)
-img_anno_np[data[0]['extract_map'] == 0] = [*d['bg_color'], 255]
-img_anno_np[data[0]['extract_map'] == 1] = [*d['fg_color'], 255]
-img_anno = Image.fromarray(img_anno_np, 'RGBA')
-img_anno.convert('RGB')
-
-# %%
-img_r = get_image('/Users/felixdo/Documents/Code/AI/image2layout-computer-vision/data/inputs/Screenshot 2023-07-26 at 14.18.22.png').convert('RGB')
-crop_amount = 0.1
-img2 = img.crop((np.array(img_r.size)[:, None] * [crop_amount, 1-crop_amount]).T.reshape(-1))
-img_r2
+# px.imshow(ckm.cluster_map)
+ckm.cluster_map.shape
+
+ckm.compute_edge_scores()
 
 # %%
+cluster_onehot = ckm.cluster_map[:, :, None] == np.arange(ckm.n_clusters)
+cluster_onehot.shape
+
+# %%
+edge_ratios = np.zeros(ckm.n_clusters, float)
+edge_mask = PixelMask.edge_mask(shape=ckm.shape, amount=.1)
+_indices, _counts = COLOR.count_uniques(ckm.cluster_map[edge_mask])
+edge_ratios[_indices] = _counts / _counts.sum()
+edge_ratios
 
 
+# %%
+ckm.cluster_errors / ckm.center_dists_nonzero.min(-1)
 
+# %%
+center_dists_nearest = ckm.center_dists[ckm.center_dists > 0]
+center_dists_nearest
 
 
 
 # %%
+ckm_3 = ColorKMeans(img, 3)
+ckm_3.cluster_mask
+
+px.imshow(ckm_3.cluster_mask)
+
+# %%
 ckm_4 = ColorKMeans(img, 4)
 ckm_4.cluster_mask
 
 px.imshow(ckm_4.cluster_mask)
 
 # %%
 import numpy as np
```

