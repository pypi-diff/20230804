# Comparing `tmp/coversnap-0.0.2.tar.gz` & `tmp/coversnap-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coversnap-0.0.2.tar", last modified: Fri Aug  4 08:17:22 2023, max compression
+gzip compressed data, was "coversnap-0.0.3.tar", last modified: Fri Aug  4 08:50:31 2023, max compression
```

## Comparing `coversnap-0.0.2.tar` & `coversnap-0.0.3.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0     1064 2023-08-04 08:16:57.738610 coversnap-0.0.2/LICENSE
--rw-r--r--   0        0        0     1664 2023-08-04 08:16:57.738610 coversnap-0.0.2/README.md
--rw-r--r--   0        0        0     1464 2023-08-04 08:17:22.766428 coversnap-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      130 2023-08-04 08:16:57.742610 coversnap-0.0.2/src/coversnap/__init__.py
--rw-r--r--   0        0        0     1155 2023-08-04 08:16:57.742610 coversnap-0.0.2/src/coversnap/__main__.py
--rw-r--r--   0        0        0     1671 2023-08-04 08:16:57.742610 coversnap-0.0.2/src/coversnap/capture.py
--rw-r--r--   0        0        0        0 2023-08-04 08:16:57.742610 coversnap-0.0.2/tests/__init__.py
--rw-r--r--   0        0        0      638 2023-08-04 08:16:57.742610 coversnap-0.0.2/tests/test_captureimage.py
--rw-r--r--   0        0        0      236 2023-08-04 08:16:57.742610 coversnap-0.0.2/tests/test_checkimage.py
--rw-r--r--   0        0        0      973 2023-08-04 08:16:57.742610 coversnap-0.0.2/tests/util.py
--rw-r--r--   0        0        0     2308 1970-01-01 00:00:00.000000 coversnap-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-08-04 08:50:01.180547 coversnap-0.0.3/LICENSE
+-rw-r--r--   0        0        0     1919 2023-08-04 08:50:01.180547 coversnap-0.0.3/README.md
+-rw-r--r--   0        0        0     1464 2023-08-04 08:50:31.622271 coversnap-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      130 2023-08-04 08:50:01.184547 coversnap-0.0.3/src/coversnap/__init__.py
+-rw-r--r--   0        0        0     1198 2023-08-04 08:50:01.184547 coversnap-0.0.3/src/coversnap/__main__.py
+-rw-r--r--   0        0        0     1671 2023-08-04 08:50:01.184547 coversnap-0.0.3/src/coversnap/capture.py
+-rw-r--r--   0        0        0      395 2023-08-04 08:50:01.184547 coversnap-0.0.3/tests/CItestpip.py
+-rw-r--r--   0        0        0        0 2023-08-04 08:50:01.184547 coversnap-0.0.3/tests/__init__.py
+-rw-r--r--   0        0        0      638 2023-08-04 08:50:01.184547 coversnap-0.0.3/tests/test_captureimage.py
+-rw-r--r--   0        0        0      236 2023-08-04 08:50:01.184547 coversnap-0.0.3/tests/test_checkimage.py
+-rw-r--r--   0        0        0      973 2023-08-04 08:50:01.184547 coversnap-0.0.3/tests/util.py
+-rw-r--r--   0        0        0     2563 1970-01-01 00:00:00.000000 coversnap-0.0.3/PKG-INFO
```

### Comparing `coversnap-0.0.2/LICENSE` & `coversnap-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `coversnap-0.0.2/README.md` & `coversnap-0.0.3/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,40 +1,45 @@
 # CoverSnap
+
 A convenient Python library for capturing cover image from video.
 
 [![codecov](https://codecov.io/github/Biu-X/CoverSnap/branch/main/graph/badge.svg?token=FYCR8Y4NDI)](https://codecov.io/github/Biu-X/CoverSnap)
 [![CI-test](https://github.com/Biu-X/CoverSnap/actions/workflows/CI-test.yml/badge.svg)](https://github.com/Biu-X/CoverSnap/actions/workflows/CI-test.yml)
+[![pip-test](https://github.com/Biu-X/CoverSnap/actions/workflows/pip-test.yml/badge.svg)](https://github.com/Biu-X/CoverSnap/actions/workflows/pip-test.yml)
 [![Release](https://github.com/Biu-X/CoverSnap/actions/workflows/Release.yml/badge.svg)](https://github.com/Biu-X/CoverSnap/actions/workflows/Release.yml)
+[![PyPI version](https://badge.fury.io/py/CoverSnap.svg)](https://badge.fury.io/py/CoverSnap)
 ![GitHub](https://img.shields.io/github/license/Biu-X/CoverSnap)
 
-
 ## Installation
+
 You can install CoverSnap using pip (python >= 3.8):
 
 ```bash
 pip install coversnap
 ```
 
 ## CLI
+
 ```
 usage: coversnap [-h] -i INPUT -o OUTPUT
 
 Capture image from video and save it to file, return black image if failed
 
 optional arguments:
   -h, --help            show this help message and exit
   -i INPUT, --INPUT INPUT
                         absolute path to input video
   -o OUTPUT, --OUTPUT OUTPUT
                         absolute path to output image
 ```
 
-
 ## Python
-To capture a cover image from a video, use the `capture_image` function provided by the CoverSnap library. Here's an example of how to use it:
+
+To capture a cover image from a video, use the `capture_image` function provided by the CoverSnap library. Here's an
+example of how to use it:
 
 ```python
 import os
 import cv2
 from coversnap import capture_image
 
 input_video = "path/to/video.mp4"
@@ -45,8 +50,9 @@
 
 # Save the captured image to the specified file
 _, file_extension = os.path.splitext(output_image)
 cv2.imencode(file_extension, img)[1].tofile(output_image)
 ```
 
 ## License
+
 CoverSnap is licensed under the MIT License.
```

### Comparing `coversnap-0.0.2/pyproject.toml` & `coversnap-0.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "CoverSnap"
-version = "0.0.2"
+version = "0.0.3"
 description = "a convenient Python library for capturing cover image from video"
 authors = [
     { name = "Tohrusky", email = "65994850+Tohrusky@users.noreply.github.com" },
 ]
 dependencies = [
     "opencv-python",
     "Pathlib",
```

### Comparing `coversnap-0.0.2/src/coversnap/__main__.py` & `coversnap-0.0.3/src/coversnap/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -24,11 +24,12 @@
     img = capture_image(args.INPUT)
 
     if img is None:
         print('Failed to capture image, using black image instead')
         img = np.zeros((512, 512, 3), dtype=np.uint8)
 
     cv2.imencode(file_extension, img)[1].tofile(args.OUTPUT)
+    print(f'Cover saved to {args.OUTPUT}')
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `coversnap-0.0.2/src/coversnap/capture.py` & `coversnap-0.0.3/src/coversnap/capture.py`

 * *Files identical despite different names*

### Comparing `coversnap-0.0.2/tests/test_captureimage.py` & `coversnap-0.0.3/tests/test_captureimage.py`

 * *Files identical despite different names*

### Comparing `coversnap-0.0.2/tests/util.py` & `coversnap-0.0.3/tests/util.py`

 * *Files identical despite different names*

### Comparing `coversnap-0.0.2/PKG-INFO` & `coversnap-0.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CoverSnap
-Version: 0.0.2
+Version: 0.0.3
 Summary: a convenient Python library for capturing cover image from video
 Author-Email: Tohrusky <65994850+Tohrusky@users.noreply.github.com>
 License: MIT
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -12,46 +12,51 @@
 Project-URL: Repository, https://github.com/Biu-X/CoverSnap
 Requires-Python: >=3.8
 Requires-Dist: opencv-python
 Requires-Dist: Pathlib
 Description-Content-Type: text/markdown
 
 # CoverSnap
+
 A convenient Python library for capturing cover image from video.
 
 [![codecov](https://codecov.io/github/Biu-X/CoverSnap/branch/main/graph/badge.svg?token=FYCR8Y4NDI)](https://codecov.io/github/Biu-X/CoverSnap)
 [![CI-test](https://github.com/Biu-X/CoverSnap/actions/workflows/CI-test.yml/badge.svg)](https://github.com/Biu-X/CoverSnap/actions/workflows/CI-test.yml)
+[![pip-test](https://github.com/Biu-X/CoverSnap/actions/workflows/pip-test.yml/badge.svg)](https://github.com/Biu-X/CoverSnap/actions/workflows/pip-test.yml)
 [![Release](https://github.com/Biu-X/CoverSnap/actions/workflows/Release.yml/badge.svg)](https://github.com/Biu-X/CoverSnap/actions/workflows/Release.yml)
+[![PyPI version](https://badge.fury.io/py/CoverSnap.svg)](https://badge.fury.io/py/CoverSnap)
 ![GitHub](https://img.shields.io/github/license/Biu-X/CoverSnap)
 
-
 ## Installation
+
 You can install CoverSnap using pip (python >= 3.8):
 
 ```bash
 pip install coversnap
 ```
 
 ## CLI
+
 ```
 usage: coversnap [-h] -i INPUT -o OUTPUT
 
 Capture image from video and save it to file, return black image if failed
 
 optional arguments:
   -h, --help            show this help message and exit
   -i INPUT, --INPUT INPUT
                         absolute path to input video
   -o OUTPUT, --OUTPUT OUTPUT
                         absolute path to output image
 ```
 
-
 ## Python
-To capture a cover image from a video, use the `capture_image` function provided by the CoverSnap library. Here's an example of how to use it:
+
+To capture a cover image from a video, use the `capture_image` function provided by the CoverSnap library. Here's an
+example of how to use it:
 
 ```python
 import os
 import cv2
 from coversnap import capture_image
 
 input_video = "path/to/video.mp4"
@@ -62,8 +67,9 @@
 
 # Save the captured image to the specified file
 _, file_extension = os.path.splitext(output_image)
 cv2.imencode(file_extension, img)[1].tofile(output_image)
 ```
 
 ## License
+
 CoverSnap is licensed under the MIT License.
```

