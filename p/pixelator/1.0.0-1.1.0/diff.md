# Comparing `tmp/pixelator-1.0.0.tar.gz` & `tmp/pixelator-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pixelator-1.0.0.tar", last modified: Tue Nov 15 18:20:42 2022, max compression
+gzip compressed data, was "pixelator-1.1.0.tar", last modified: Fri Aug  4 13:42:12 2023, max compression
```

## Comparing `pixelator-1.0.0.tar` & `pixelator-1.1.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2022-11-15 18:20:42.041010 pixelator-1.0.0/
--rw-rw-r--   0 conmak    (1000) conmak    (1000)     1072 2022-11-15 16:32:58.000000 pixelator-1.0.0/LICENSE
--rw-rw-r--   0 conmak    (1000) conmak    (1000)     2963 2022-11-15 18:20:42.041010 pixelator-1.0.0/PKG-INFO
--rw-rw-r--   0 conmak    (1000) conmak    (1000)     2158 2022-11-15 18:16:35.000000 pixelator-1.0.0/README.md
-drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2022-11-15 18:20:42.041010 pixelator-1.0.0/pixelator/
--rw-rw-r--   0 conmak    (1000) conmak    (1000)       33 2022-11-15 16:34:17.000000 pixelator-1.0.0/pixelator/__init__.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)     8548 2022-11-15 18:09:15.000000 pixelator-1.0.0/pixelator/pixelator.py
-drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2022-11-15 18:20:42.041010 pixelator-1.0.0/pixelator.egg-info/
--rw-rw-r--   0 conmak    (1000) conmak    (1000)     2963 2022-11-15 18:20:42.000000 pixelator-1.0.0/pixelator.egg-info/PKG-INFO
--rw-rw-r--   0 conmak    (1000) conmak    (1000)      305 2022-11-15 18:20:42.000000 pixelator-1.0.0/pixelator.egg-info/SOURCES.txt
--rw-rw-r--   0 conmak    (1000) conmak    (1000)        1 2022-11-15 18:20:42.000000 pixelator-1.0.0/pixelator.egg-info/dependency_links.txt
--rw-rw-r--   0 conmak    (1000) conmak    (1000)       24 2022-11-15 18:20:42.000000 pixelator-1.0.0/pixelator.egg-info/requires.txt
--rw-rw-r--   0 conmak    (1000) conmak    (1000)       10 2022-11-15 18:20:42.000000 pixelator-1.0.0/pixelator.egg-info/top_level.txt
--rw-rw-r--   0 conmak    (1000) conmak    (1000)       89 2022-11-15 16:31:41.000000 pixelator-1.0.0/pyproject.toml
--rw-rw-r--   0 conmak    (1000) conmak    (1000)       79 2022-11-15 18:20:42.041010 pixelator-1.0.0/setup.cfg
--rw-rw-r--   0 conmak    (1000) conmak    (1000)     1133 2022-11-15 18:09:32.000000 pixelator-1.0.0/setup.py
-drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2022-11-15 18:20:42.041010 pixelator-1.0.0/test/
--rw-rw-r--   0 conmak    (1000) conmak    (1000)      429 2022-11-15 18:17:07.000000 pixelator-1.0.0/test/test_1.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)      589 2022-11-15 18:17:12.000000 pixelator-1.0.0/test/test_2.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)      468 2022-11-15 18:18:33.000000 pixelator-1.0.0/test/test_3.py
+drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2023-08-04 13:42:12.085740 pixelator-1.1.0/
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)     1072 2023-08-03 20:53:08.000000 pixelator-1.1.0/LICENSE
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)     3125 2023-08-04 13:42:12.085740 pixelator-1.1.0/PKG-INFO
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)     2320 2023-08-04 13:37:47.000000 pixelator-1.1.0/README.md
+drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2023-08-04 13:42:12.085740 pixelator-1.1.0/pixelator/
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)       33 2023-08-03 20:53:08.000000 pixelator-1.1.0/pixelator/__init__.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)     9152 2023-08-04 13:40:20.000000 pixelator-1.1.0/pixelator/pixelator.py
+drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2023-08-04 13:42:12.085740 pixelator-1.1.0/pixelator.egg-info/
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)     3125 2023-08-04 13:42:12.000000 pixelator-1.1.0/pixelator.egg-info/PKG-INFO
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)      305 2023-08-04 13:42:12.000000 pixelator-1.1.0/pixelator.egg-info/SOURCES.txt
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)        1 2023-08-04 13:42:12.000000 pixelator-1.1.0/pixelator.egg-info/dependency_links.txt
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)       24 2023-08-04 13:42:12.000000 pixelator-1.1.0/pixelator.egg-info/requires.txt
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)       10 2023-08-04 13:42:12.000000 pixelator-1.1.0/pixelator.egg-info/top_level.txt
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)       89 2023-08-03 20:53:08.000000 pixelator-1.1.0/pyproject.toml
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)       79 2023-08-04 13:42:12.085740 pixelator-1.1.0/setup.cfg
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)     1133 2023-08-04 13:41:17.000000 pixelator-1.1.0/setup.py
+drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2023-08-04 13:42:12.085740 pixelator-1.1.0/test/
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)      429 2023-08-03 20:53:08.000000 pixelator-1.1.0/test/test_1.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)      903 2023-08-03 21:10:02.000000 pixelator-1.1.0/test/test_2.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)      468 2023-08-03 20:53:08.000000 pixelator-1.1.0/test/test_3.py
```

### Comparing `pixelator-1.0.0/LICENSE` & `pixelator-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pixelator-1.0.0/PKG-INFO` & `pixelator-1.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pixelator
-Version: 1.0.0
+Version: 1.1.0
 Summary: Pixelate images to a specified size and color palette for AI/ML and various other purposes
 Home-page: https://github.com/connor-makowski/pixelator
-Download-URL: https://github.com/connor-makowski/pixelator/dist/pixelator-1.0.0.tar.gz
+Download-URL: https://github.com/connor-makowski/pixelator/dist/pixelator-1.1.0.tar.gz
 Author: Connor Makowski
 Author-email: connor.m.makowski@gmail.com
 License: MIT
 Keywords: pixelate,picture,pixel,pixels,ai,ml
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
@@ -26,14 +26,18 @@
 --------
 
 - Users can:
   1. Load in array data, image files or capture directly from a camera
   2. Pixelate images to a specific color palette and image resolution
   3. Access pixelated array data or write it back to an image file
 
+Technical Docs
+--------
+https://connor-makowski.github.io/pixelator/pixelator.html
+
 Setup
 ----------
 
 Make sure you have Python 3.6.x (or higher). You can download it [here](https://www.python.org/downloads/).
 
 ### Installation
 
@@ -60,30 +64,30 @@
 image = Pixelator(filename='./images/input.jpg')
 # Pixelate the image to a 28x28 black and white array
 pixelated_image = image.pixelate(
     width=28,
     height=28,
     palette=[[0,0,0],[255,255,255]]
 )
-# Write to `output.png` scaled up to a 500x500 image (to be easily viewed)
+# Write to `output.png` scaled up to a 300x300 image (to be easily viewed)
 pixelated_image.write(filename='./images/output_test_1.jpg', width=300, height=300)
 ```
 Input:
 ![](images/input.jpg)
 
 Output:
 ![](images/output_test_1.jpg)
 
 Capture from a webcam:
 ```
 from pixelator import Pixelator
 # Capture from a webcam since no data or filename is provided
 image = Pixelator()
 
-# Pixelate the image to a 28x28 black and white array
+# Pixelate the image to a 64x64 black, white and multiple gray array
 pixelated_image = image.pixelate(
     width=64,
     height=64,
     palette=[[0,0,0],[80,80,80],[160,160,160],[200,200,200],[255,255,255]]
 )
 # Write to `output.png` scaled up to a 500x500 image (to be easily viewed)
 pixelated_image.write(filename='./images/output_test_3.jpg', width=300, height=300)
@@ -99,8 +103,10 @@
 pixelated_image = image.pixelate(
     width=28,
     height=28,
     palette=[[0,0,0],[255,255,255]]
 )
 # Show pixelated image data
 print(pixelated_image.data)
+# Show Color Counts:
+print(pixelated_image.get_color_counts())
 ```
```

### Comparing `pixelator-1.0.0/README.md` & `pixelator-1.1.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -6,14 +6,18 @@
 --------
 
 - Users can:
   1. Load in array data, image files or capture directly from a camera
   2. Pixelate images to a specific color palette and image resolution
   3. Access pixelated array data or write it back to an image file
 
+Technical Docs
+--------
+https://connor-makowski.github.io/pixelator/pixelator.html
+
 Setup
 ----------
 
 Make sure you have Python 3.6.x (or higher). You can download it [here](https://www.python.org/downloads/).
 
 ### Installation
 
@@ -40,30 +44,30 @@
 image = Pixelator(filename='./images/input.jpg')
 # Pixelate the image to a 28x28 black and white array
 pixelated_image = image.pixelate(
     width=28,
     height=28,
     palette=[[0,0,0],[255,255,255]]
 )
-# Write to `output.png` scaled up to a 500x500 image (to be easily viewed)
+# Write to `output.png` scaled up to a 300x300 image (to be easily viewed)
 pixelated_image.write(filename='./images/output_test_1.jpg', width=300, height=300)
 ```
 Input:
 ![](images/input.jpg)
 
 Output:
 ![](images/output_test_1.jpg)
 
 Capture from a webcam:
 ```
 from pixelator import Pixelator
 # Capture from a webcam since no data or filename is provided
 image = Pixelator()
 
-# Pixelate the image to a 28x28 black and white array
+# Pixelate the image to a 64x64 black, white and multiple gray array
 pixelated_image = image.pixelate(
     width=64,
     height=64,
     palette=[[0,0,0],[80,80,80],[160,160,160],[200,200,200],[255,255,255]]
 )
 # Write to `output.png` scaled up to a 500x500 image (to be easily viewed)
 pixelated_image.write(filename='./images/output_test_3.jpg', width=300, height=300)
@@ -79,8 +83,10 @@
 pixelated_image = image.pixelate(
     width=28,
     height=28,
     palette=[[0,0,0],[255,255,255]]
 )
 # Show pixelated image data
 print(pixelated_image.data)
+# Show Color Counts:
+print(pixelated_image.get_color_counts())
 ```
```

### Comparing `pixelator-1.0.0/pixelator/pixelator.py` & `pixelator-1.1.0/pixelator/pixelator.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,21 +5,21 @@
     @staticmethod
     def crop_image(image, width, height):
         """
         Crops an image to a specified width and height (centered)
 
         Takes in three required arguments:
 
-            - `image`:
+            - 'image':
                 - Type: list of lists
                 - What: CV2 image data
-            - `width`:
+            - 'width':
                 - Type: int
                 - What: The width in pixels for the output image
-            - `height`:
+            - 'height':
                 - Type: int
                 - What: The height in pixels for the output image
         """
         (h, w) = image.shape[:2]
         if width > w or height > h:
             raise Exception("Cannot crop an image larger")
         h_start = (h - height) // 2
@@ -31,18 +31,18 @@
     @staticmethod
     def crop_to_aspect_ratio(image, aspect_ratio_w_by_h):
         """
         Crops an image to a specified aspect ratio
 
         Takes in two required arguments:
 
-            - `image`:
+            - 'image':
                 - Type: list of lists
                 - What: CV2 image data
-            - `aspect_ratio_w_by_h`:
+            - 'aspect_ratio_w_by_h':
                 - Type: int | float
                 - What: The aspect ratio for the cropped image
         """
         (h, w) = image.shape[:2]
         aspect_ratio_current = w / h
         if aspect_ratio_w_by_h == aspect_ratio_current:
             return image
@@ -57,38 +57,38 @@
     @staticmethod
     def resize(image, width, height, interpolation=cv2.INTER_AREA):
         """
         Resizes an image to a specified width and height
 
         Takes in three required arguments:
 
-            - `image`:
+            - 'image':
                 - Type: list of lists
                 - What: CV2 image data
-            - `width`:
+            - 'width':
                 - Type: int
                 - What: The width in pixels for the output image
-            - `height`:
+            - 'height':
                 - Type: int
                 - What: The height in pixels for the output image
         """
         image = Picture_Utils.crop_to_aspect_ratio(image, width / height)
         return cv2.resize(image, (width, height), interpolation=interpolation)
 
     @staticmethod
     def quantize_to_palette(image, palette):
         """
         Quantizes an image to a given palette
 
         Takes in two required arguments:
 
-            - `image`:
+            - 'image':
                 - Type: list of lists
                 - What: CV2 image data
-            - `palette`:
+            - 'palette':
                 - Type: list of lists
                 - What: A list of BGR lists for quantizing the image
         """
         palette = numpy.array(palette).astype(numpy.float32)
         hsv_palette = cv2.cvtColor(
             numpy.reshape(palette, (1,) + palette.shape), cv2.COLOR_BGR2HSV
         ).reshape(palette.shape)
@@ -105,15 +105,15 @@
     @staticmethod
     def capture(cam_port=0):
         """
         Uses an attached camera or webcam to capture its input at the time of calling
 
         Takes in one optional argument:
 
-            - `cam_port`:
+            - 'cam_port':
                 - Type: int
                 - What: The camera port to use for a capture
                 - Default: 0
                 - Note: For more info see the docs for cv2.VideoCapture.
         """
         cam = cv2.VideoCapture(cam_port)
         try:
@@ -127,21 +127,21 @@
     @staticmethod
     def to_colorscheme(image, colorscheme="bgr"):
         """
         Converts an image to an alternate colorscheme
 
         Takes in one required argument:
 
-            - `image`:
+            - 'image':
                 - Type: list of lists
                 - What: CV2 image data
 
         Takes in one optional argument:
 
-            - `colorscheme`:
+            - 'colorscheme':
                 - Type: str
                 - What: The color scheme to convert
                 - Options: ['bgr', 'rgb', 'gray', 'hsv']
                 - Default: 'bgr'
 
         """
         colorscheme = str(colorscheme).lower()
@@ -157,37 +157,37 @@
     @staticmethod
     def read(filename):
         """
         Reads a picture into CV2 image data
 
         Requires one argument:
 
-            - `filename`:
+            - 'filename':
                 - Type: str
                 - What: Filename from which to load a picture
         """
         return cv2.imread(filename)
 
 
 class Pixelator(Picture_Utils):
     def __init__(self, data=None, filename=None, cam_port=0):
         """
         Initialize a Pixelator object.
 
         Takes in three optional arguments:
 
-            - `data`:
+            - 'data':
                 - Type: list of lists
                 - What: BGR array of data to input
                 - Note: If not specified, proceeds to attempt to load from a filename
-            - `filename`:
+            - 'filename':
                 - Type: str
                 - What: Filename from which to load a picture
                 - Note: If not specified, proceeds to attempt a camera capture
-            - `cam_port`:
+            - 'cam_port':
                 - Type: int
                 - What: The camera port to use for a capture
                 - Note: For more info see the docs for cv2.VideoCapture.
         """
         if data is not None:
             self.data = data
         elif filename is not None:
@@ -199,23 +199,23 @@
         """
         Pixelates an image to a specific shape and color palette
 
         Returns a new Pixelator (class) image
 
         Takes in three optional arguments:
 
-            - `width`:
+            - 'width':
                 - Type: int
                 - What: The width in pixels for the output image
-                - Note: If either `width` or `height` are not specified, this function only applies the palette
-            - `height`:
+                - Note: If either 'width' or 'height' are not specified, this function only applies the palette
+            - 'height':
                 - Type: int
                 - What: The height in pixels for the output image
-                - Note: If either `width` or `height` are not specified, this function only applies the palette
-            - `palette`:
+                - Note: If either 'width' or 'height' are not specified, this function only applies the palette
+            - 'palette':
                 - Type: list of lists
                 - What: A list of BGR lists to apply as a pallete
                 - Note: If not specified, no palette is applied
         """
         out = self.resize(image=self.data, width=width, height=height)
         if palette is not None:
             out = self.quantize_to_palette(out, palette)
@@ -223,25 +223,42 @@
 
     def write(self, filename, width=None, height=None):
         """
         Writes the current image to a specific file and resizes to a given width and height if supplied
 
         Takes in one required argument:
 
-            - `filename`:
+            - 'filename':
                 - Type: str
                 - What: Filename at which to write the picture
 
         Takes in two optional arguments:
 
-            - `width`:
+            - 'width':
                 - Type: int
                 - What: The width in pixels for the output image
-                - Note: If either `width` or `height` are not specified, no resizing is done
-            - `height`:
+                - Note: If either 'width' or 'height' are not specified, no resizing is done
+            - 'height':
                 - Type: int
                 - What: The height in pixels for the output image
-                - Note: If either `width` or `height` are not specified, no resizing is done
+                - Note: If either 'width' or 'height' are not specified, no resizing is done
         """
         if width == None or height == None:
             (height, width) = self.data.shape[:2]
         cv2.imwrite(filename, self.resize(self.data, width, height))
+
+    def get_color_counts(self):
+        """
+        Gets the counts of each color in the image
+
+        Returns a dictionary of color counts where:
+            - The keys are the tuples of the colors
+            - The values are the counts of each color
+
+        EG: {(255, 255, 255): 100, (0, 0, 0): 50}
+        """
+        colors, count = numpy.unique(
+            self.data.reshape(-1, self.data.shape[-1]), axis=0, return_counts=True
+        )
+        # Force all items in colors to be integers
+        colors = colors.astype(int)
+        return dict(zip([tuple(color) for color in colors], count))
```

### Comparing `pixelator-1.0.0/pixelator.egg-info/PKG-INFO` & `pixelator-1.1.0/pixelator.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pixelator
-Version: 1.0.0
+Version: 1.1.0
 Summary: Pixelate images to a specified size and color palette for AI/ML and various other purposes
 Home-page: https://github.com/connor-makowski/pixelator
-Download-URL: https://github.com/connor-makowski/pixelator/dist/pixelator-1.0.0.tar.gz
+Download-URL: https://github.com/connor-makowski/pixelator/dist/pixelator-1.1.0.tar.gz
 Author: Connor Makowski
 Author-email: connor.m.makowski@gmail.com
 License: MIT
 Keywords: pixelate,picture,pixel,pixels,ai,ml
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
@@ -26,14 +26,18 @@
 --------
 
 - Users can:
   1. Load in array data, image files or capture directly from a camera
   2. Pixelate images to a specific color palette and image resolution
   3. Access pixelated array data or write it back to an image file
 
+Technical Docs
+--------
+https://connor-makowski.github.io/pixelator/pixelator.html
+
 Setup
 ----------
 
 Make sure you have Python 3.6.x (or higher). You can download it [here](https://www.python.org/downloads/).
 
 ### Installation
 
@@ -60,30 +64,30 @@
 image = Pixelator(filename='./images/input.jpg')
 # Pixelate the image to a 28x28 black and white array
 pixelated_image = image.pixelate(
     width=28,
     height=28,
     palette=[[0,0,0],[255,255,255]]
 )
-# Write to `output.png` scaled up to a 500x500 image (to be easily viewed)
+# Write to `output.png` scaled up to a 300x300 image (to be easily viewed)
 pixelated_image.write(filename='./images/output_test_1.jpg', width=300, height=300)
 ```
 Input:
 ![](images/input.jpg)
 
 Output:
 ![](images/output_test_1.jpg)
 
 Capture from a webcam:
 ```
 from pixelator import Pixelator
 # Capture from a webcam since no data or filename is provided
 image = Pixelator()
 
-# Pixelate the image to a 28x28 black and white array
+# Pixelate the image to a 64x64 black, white and multiple gray array
 pixelated_image = image.pixelate(
     width=64,
     height=64,
     palette=[[0,0,0],[80,80,80],[160,160,160],[200,200,200],[255,255,255]]
 )
 # Write to `output.png` scaled up to a 500x500 image (to be easily viewed)
 pixelated_image.write(filename='./images/output_test_3.jpg', width=300, height=300)
@@ -99,8 +103,10 @@
 pixelated_image = image.pixelate(
     width=28,
     height=28,
     palette=[[0,0,0],[255,255,255]]
 )
 # Show pixelated image data
 print(pixelated_image.data)
+# Show Color Counts:
+print(pixelated_image.get_color_counts())
 ```
```

### Comparing `pixelator-1.0.0/setup.py` & `pixelator-1.1.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
   name = 'pixelator',
   packages = ['pixelator'],
-  version = '1.0.0',
+  version = '1.1.0',
   license='MIT',
   description = 'Pixelate images to a specified size and color palette for AI/ML and various other purposes',
   long_description=long_description,
   long_description_content_type='text/markdown',
   author = 'Connor Makowski',
   author_email = 'connor.m.makowski@gmail.com',
   url = 'https://github.com/connor-makowski/pixelator',
-  download_url = 'https://github.com/connor-makowski/pixelator/dist/pixelator-1.0.0.tar.gz',
+  download_url = 'https://github.com/connor-makowski/pixelator/dist/pixelator-1.1.0.tar.gz',
   keywords = ['pixelate', 'picture', 'pixel', 'pixels', 'ai', 'ml'],
   install_requires=[
           'opencv-python>=4.6.0.66',
       ],
   classifiers=[
     'Development Status :: 3 - Alpha',
     'Intended Audience :: Developers',
```

