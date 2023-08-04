# Comparing `tmp/meerk40t-barcodes-0.2.0.tar.gz` & `tmp/meerk40t-barcodes-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meerk40t-barcodes-0.2.0.tar", last modified: Tue Apr 18 20:34:29 2023, max compression
+gzip compressed data, was "meerk40t-barcodes-0.2.1.tar", last modified: Fri Aug  4 15:48:40 2023, max compression
```

## Comparing `meerk40t-barcodes-0.2.0.tar` & `meerk40t-barcodes-0.2.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 20:34:29.951460 meerk40t-barcodes-0.2.0/
--rw-rw-rw-   0        0        0     1086 2022-10-05 19:57:23.000000 meerk40t-barcodes-0.2.0/LICENSE
--rw-rw-rw-   0        0        0     4038 2023-04-18 20:34:29.952460 meerk40t-barcodes-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     2614 2023-04-18 20:27:08.000000 meerk40t-barcodes-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-18 20:34:29.931459 meerk40t-barcodes-0.2.0/barcodes/
--rw-rw-rw-   0        0        0       28 2023-04-18 20:27:08.000000 meerk40t-barcodes-0.2.0/barcodes/__init__.py
--rw-rw-rw-   0        0        0    24622 2023-04-18 20:27:08.000000 meerk40t-barcodes-0.2.0/barcodes/bcode_logic.py
--rw-rw-rw-   0        0        0    27455 2023-04-18 20:27:08.000000 meerk40t-barcodes-0.2.0/barcodes/gui.py
--rw-rw-rw-   0        0        0    16153 2023-04-18 20:27:08.000000 meerk40t-barcodes-0.2.0/barcodes/main.py
-drwxrwxrwx   0        0        0        0 2023-04-18 20:34:29.936459 meerk40t-barcodes-0.2.0/barcodes/tools/
--rw-rw-rw-   0        0        0        0 2022-10-05 19:57:23.000000 meerk40t-barcodes-0.2.0/barcodes/tools/__init__.py
--rw-rw-rw-   0        0        0    11818 2022-10-05 19:57:23.000000 meerk40t-barcodes-0.2.0/barcodes/tools/icons.py
-drwxrwxrwx   0        0        0        0 2023-04-18 20:34:29.951460 meerk40t-barcodes-0.2.0/meerk40t_barcodes.egg-info/
--rw-rw-rw-   0        0        0     4038 2023-04-18 20:34:29.000000 meerk40t-barcodes-0.2.0/meerk40t_barcodes.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      550 2023-04-18 20:34:29.000000 meerk40t-barcodes-0.2.0/meerk40t_barcodes.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 20:34:29.000000 meerk40t-barcodes-0.2.0/meerk40t_barcodes.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2023-04-18 20:34:29.000000 meerk40t-barcodes-0.2.0/meerk40t_barcodes.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       52 2023-04-18 20:34:29.000000 meerk40t-barcodes-0.2.0/meerk40t_barcodes.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-18 20:34:29.000000 meerk40t-barcodes-0.2.0/meerk40t_barcodes.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2022-10-05 19:58:04.000000 meerk40t-barcodes-0.2.0/meerk40t_barcodes.egg-info/zip-safe
--rw-rw-rw-   0        0        0     1103 2023-04-18 20:34:29.954460 meerk40t-barcodes-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0      159 2022-10-05 19:57:23.000000 meerk40t-barcodes-0.2.0/setup.py
+drwxrwxr-x   0 jens      (1000) jens      (1000)        0 2023-08-04 15:48:40.515639 meerk40t-barcodes-0.2.1/
+-rw-rw-r--   0 jens      (1000) jens      (1000)     1065 2023-08-04 15:16:40.000000 meerk40t-barcodes-0.2.1/LICENSE
+-rw-rw-r--   0 jens      (1000) jens      (1000)     3412 2023-08-04 15:48:40.515639 meerk40t-barcodes-0.2.1/PKG-INFO
+-rw-rw-r--   0 jens      (1000) jens      (1000)     2548 2023-08-04 15:16:40.000000 meerk40t-barcodes-0.2.1/README.md
+drwxrwxr-x   0 jens      (1000) jens      (1000)        0 2023-08-04 15:48:40.503640 meerk40t-barcodes-0.2.1/barcodes/
+-rw-rw-r--   0 jens      (1000) jens      (1000)       27 2023-08-04 15:16:40.000000 meerk40t-barcodes-0.2.1/barcodes/__init__.py
+-rw-rw-r--   0 jens      (1000) jens      (1000)    24044 2023-08-04 15:33:22.000000 meerk40t-barcodes-0.2.1/barcodes/bcode_logic.py
+-rw-rw-r--   0 jens      (1000) jens      (1000)    26809 2023-08-04 15:16:40.000000 meerk40t-barcodes-0.2.1/barcodes/gui.py
+-rw-rw-r--   0 jens      (1000) jens      (1000)    15679 2023-08-04 15:16:40.000000 meerk40t-barcodes-0.2.1/barcodes/main.py
+drwxrwxr-x   0 jens      (1000) jens      (1000)        0 2023-08-04 15:48:40.503640 meerk40t-barcodes-0.2.1/barcodes/tools/
+-rw-rw-r--   0 jens      (1000) jens      (1000)        0 2023-08-04 15:16:40.000000 meerk40t-barcodes-0.2.1/barcodes/tools/__init__.py
+-rw-rw-r--   0 jens      (1000) jens      (1000)    11519 2023-08-04 15:16:40.000000 meerk40t-barcodes-0.2.1/barcodes/tools/icons.py
+drwxrwxr-x   0 jens      (1000) jens      (1000)        0 2023-08-04 15:48:40.507640 meerk40t-barcodes-0.2.1/meerk40t_barcodes.egg-info/
+-rw-rw-r--   0 jens      (1000) jens      (1000)     3412 2023-08-04 15:48:40.000000 meerk40t-barcodes-0.2.1/meerk40t_barcodes.egg-info/PKG-INFO
+-rw-rw-r--   0 jens      (1000) jens      (1000)      461 2023-08-04 15:48:40.000000 meerk40t-barcodes-0.2.1/meerk40t_barcodes.egg-info/SOURCES.txt
+-rw-rw-r--   0 jens      (1000) jens      (1000)        1 2023-08-04 15:48:40.000000 meerk40t-barcodes-0.2.1/meerk40t_barcodes.egg-info/dependency_links.txt
+-rw-rw-r--   0 jens      (1000) jens      (1000)       52 2023-08-04 15:48:40.000000 meerk40t-barcodes-0.2.1/meerk40t_barcodes.egg-info/entry_points.txt
+-rw-rw-r--   0 jens      (1000) jens      (1000)       52 2023-08-04 15:48:40.000000 meerk40t-barcodes-0.2.1/meerk40t_barcodes.egg-info/requires.txt
+-rw-rw-r--   0 jens      (1000) jens      (1000)        9 2023-08-04 15:48:40.000000 meerk40t-barcodes-0.2.1/meerk40t_barcodes.egg-info/top_level.txt
+-rw-rw-r--   0 jens      (1000) jens      (1000)        1 2023-08-04 15:17:28.000000 meerk40t-barcodes-0.2.1/meerk40t_barcodes.egg-info/zip-safe
+-rw-rw-r--   0 jens      (1000) jens      (1000)     1058 2023-08-04 15:48:40.519639 meerk40t-barcodes-0.2.1/setup.cfg
+-rw-rw-r--   0 jens      (1000) jens      (1000)      152 2023-08-04 15:16:40.000000 meerk40t-barcodes-0.2.1/setup.py
```

### Comparing `meerk40t-barcodes-0.2.0/LICENSE` & `meerk40t-barcodes-0.2.1/LICENSE`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2022 MeerK40t
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2022 MeerK40t
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `meerk40t-barcodes-0.2.0/PKG-INFO` & `meerk40t-barcodes-0.2.1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,89 +1,89 @@
-Metadata-Version: 2.1
-Name: meerk40t-barcodes
-Version: 0.2.0
-Summary: MeerK40t Barcode Extension
-Home-page: https://github.com/meerk40t/meerk40t-barcodes
-Author: jpirnay
-Author-email: tatarize@gmail.com
-License: MIT
-Description: # meerk40t-barcodes
-        MeerK40t 0.8+ Barcode extension.
-        
-        
-        # Barcode-Extension
-        
-        * Registers the console command: `qrcode` which will generate a qrcode
-        
-        Usage:    `qrcode x_pos y_pos dim code`
-        
-        Arguments:
-        >     x_pos          X-position of qr-code
-        >     y_pos          Y-position of qr-code
-        >     dim            Width/length of qr-code
-        >     code           Text to create qr-code from
-        
-        Options:
-        >     --boxsize  (-x)      Boxsize (default 10)
-        >     --border   (-b)      Border around qr-code (default 4)
-        >     --version  (-v)      size (1..40)
-        >     --errcorr  (-e)      error correction, one of L (7%), M (15%), Q (25%), H (30%)
-        
-        * Registers the console command: `barcode` which will generate a barcode
-        
-        Usage:    `barcode x_pos y_pos dimx dimy btype code`
-        
-        Arguments:
-        >     x_pos     X-Position of barcode
-        >     y_pos     Y-Position of barcode
-        >     dim       Width of barcode, may be 'auto' to keep native width
-        >     dimy      Height of barcode, may be 'auto' to keep native height
-        >     btype     Barcode type
-        >     code      The code to process
-        
-         Options:
-        >    --notext  (-n)      suppress text display
-        
-        * GUI-Support
-        The installation of this tool will register a new button in the Design section of MeerK40t:
-        <img width="639" alt="image" src="https://user-images.githubusercontent.com/2670784/232893108-c2f4293c-f084-4d5b-8900-b4cbd74f0e38.png">
-        
-        If you click on it then a dialog will pop up allowing you to design a qr-code / a barcode:
-        
-        <img width="258" alt="image" src="https://user-images.githubusercontent.com/2670784/232893402-88694837-370a-4b34-a0b7-e9e2ac83c0bc.png">
-        
-        This will create an element in Meerk40t that can be treated like any other regular path, but which will allow post-creation change of the underlying code (ie the barcode will be regenerated based on the new input).
-        
-        <img width="432" alt="image" src="https://user-images.githubusercontent.com/2670784/232892296-c3cbae13-53d8-4143-9667-94cdc31cb4a5.png">
-        
-        # Installing
-        * `pip install meerk40t-barcodes`
-        Or
-        * Download into a directory:
-        * `$ pip install .`
-        
-        # Development
-        
-        * If you are developing your own extension for meerk40t you will want to use:
-        * `$ pip install -e .` this installs the python module in edit mode which allows you to easily see and experience your changes. Without reinstalling your module.
-        
-        # Acknowledgements
-        
-        * This MeerK40t extension uses the work of two great libraries to create barcodes & QR codes:
-        
-        - The python-barcode library (https://github.com/WhyNotHugo/python-barcode)
-        - The qrcode library (https://github.com/lincolnloop/python-qrcode)
-        
-Keywords: lasercutter,laser,vector,parser
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Topic :: Multimedia :: Graphics
-Classifier: Topic :: Multimedia :: Graphics :: Editors :: Vector-Based
-Classifier: Topic :: Utilities
-Description-Content-Type: text/markdown
+Metadata-Version: 2.1
+Name: meerk40t-barcodes
+Version: 0.2.1
+Summary: MeerK40t Barcode Extension
+Home-page: https://github.com/meerk40t/meerk40t-barcodes
+Author: jpirnay
+Author-email: tatarize@gmail.com
+License: MIT
+Keywords: lasercutter,laser,vector,parser
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Topic :: Multimedia :: Graphics
+Classifier: Topic :: Multimedia :: Graphics :: Editors :: Vector-Based
+Classifier: Topic :: Utilities
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# meerk40t-barcodes
+MeerK40t 0.8+ Barcode extension.
+
+
+# Barcode-Extension
+
+* Registers the console command: `qrcode` which will generate a qrcode
+
+Usage:    `qrcode x_pos y_pos dim code`
+
+Arguments:
+>     x_pos          X-position of qr-code
+>     y_pos          Y-position of qr-code
+>     dim            Width/length of qr-code
+>     code           Text to create qr-code from
+
+Options:
+>     --boxsize  (-x)      Boxsize (default 10)
+>     --border   (-b)      Border around qr-code (default 4)
+>     --version  (-v)      size (1..40)
+>     --errcorr  (-e)      error correction, one of L (7%), M (15%), Q (25%), H (30%)
+
+* Registers the console command: `barcode` which will generate a barcode
+
+Usage:    `barcode x_pos y_pos dimx dimy btype code`
+
+Arguments:
+>     x_pos     X-Position of barcode
+>     y_pos     Y-Position of barcode
+>     dim       Width of barcode, may be 'auto' to keep native width
+>     dimy      Height of barcode, may be 'auto' to keep native height
+>     btype     Barcode type
+>     code      The code to process
+
+ Options:
+>    --notext  (-n)      suppress text display
+
+* GUI-Support
+The installation of this tool will register a new button in the Design section of MeerK40t:
+<img width="639" alt="image" src="https://user-images.githubusercontent.com/2670784/232893108-c2f4293c-f084-4d5b-8900-b4cbd74f0e38.png">
+
+If you click on it then a dialog will pop up allowing you to design a qr-code / a barcode:
+
+<img width="258" alt="image" src="https://user-images.githubusercontent.com/2670784/232893402-88694837-370a-4b34-a0b7-e9e2ac83c0bc.png">
+
+This will create an element in Meerk40t that can be treated like any other regular path, but which will allow post-creation change of the underlying code (ie the barcode will be regenerated based on the new input).
+
+<img width="432" alt="image" src="https://user-images.githubusercontent.com/2670784/232892296-c3cbae13-53d8-4143-9667-94cdc31cb4a5.png">
+
+# Installing
+* `pip install meerk40t-barcodes`
+Or
+* Download into a directory:
+* `$ pip install .`
+
+# Development
+
+* If you are developing your own extension for meerk40t you will want to use:
+* `$ pip install -e .` this installs the python module in edit mode which allows you to easily see and experience your changes. Without reinstalling your module.
+
+# Acknowledgements
+
+* This MeerK40t extension uses the work of two great libraries to create barcodes & QR codes:
+
+- The python-barcode library (https://github.com/WhyNotHugo/python-barcode)
+- The qrcode library (https://github.com/lincolnloop/python-qrcode)
```

### Comparing `meerk40t-barcodes-0.2.0/README.md` & `meerk40t-barcodes-0.2.1/meerk40t_barcodes.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,66 +1,89 @@
-# meerk40t-barcodes
-MeerK40t 0.8+ Barcode extension.
-
-
-# Barcode-Extension
-
-* Registers the console command: `qrcode` which will generate a qrcode
-
-Usage:    `qrcode x_pos y_pos dim code`
-
-Arguments:
->     x_pos          X-position of qr-code
->     y_pos          Y-position of qr-code
->     dim            Width/length of qr-code
->     code           Text to create qr-code from
-
-Options:
->     --boxsize  (-x)      Boxsize (default 10)
->     --border   (-b)      Border around qr-code (default 4)
->     --version  (-v)      size (1..40)
->     --errcorr  (-e)      error correction, one of L (7%), M (15%), Q (25%), H (30%)
-
-* Registers the console command: `barcode` which will generate a barcode
-
-Usage:    `barcode x_pos y_pos dimx dimy btype code`
-
-Arguments:
->     x_pos     X-Position of barcode
->     y_pos     Y-Position of barcode
->     dim       Width of barcode, may be 'auto' to keep native width
->     dimy      Height of barcode, may be 'auto' to keep native height
->     btype     Barcode type
->     code      The code to process
-
- Options:
->    --notext  (-n)      suppress text display
-
-* GUI-Support
-The installation of this tool will register a new button in the Design section of MeerK40t:
-<img width="639" alt="image" src="https://user-images.githubusercontent.com/2670784/232893108-c2f4293c-f084-4d5b-8900-b4cbd74f0e38.png">
-
-If you click on it then a dialog will pop up allowing you to design a qr-code / a barcode:
-
-<img width="258" alt="image" src="https://user-images.githubusercontent.com/2670784/232893402-88694837-370a-4b34-a0b7-e9e2ac83c0bc.png">
-
-This will create an element in Meerk40t that can be treated like any other regular path, but which will allow post-creation change of the underlying code (ie the barcode will be regenerated based on the new input).
-
-<img width="432" alt="image" src="https://user-images.githubusercontent.com/2670784/232892296-c3cbae13-53d8-4143-9667-94cdc31cb4a5.png">
-
-# Installing
-* `pip install meerk40t-barcodes`
-Or
-* Download into a directory:
-* `$ pip install .`
-
-# Development
-
-* If you are developing your own extension for meerk40t you will want to use:
-* `$ pip install -e .` this installs the python module in edit mode which allows you to easily see and experience your changes. Without reinstalling your module.
-
-# Acknowledgements
-
-* This MeerK40t extension uses the work of two great libraries to create barcodes & QR codes:
-
-- The python-barcode library (https://github.com/WhyNotHugo/python-barcode)
-- The qrcode library (https://github.com/lincolnloop/python-qrcode)
+Metadata-Version: 2.1
+Name: meerk40t-barcodes
+Version: 0.2.1
+Summary: MeerK40t Barcode Extension
+Home-page: https://github.com/meerk40t/meerk40t-barcodes
+Author: jpirnay
+Author-email: tatarize@gmail.com
+License: MIT
+Keywords: lasercutter,laser,vector,parser
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Topic :: Multimedia :: Graphics
+Classifier: Topic :: Multimedia :: Graphics :: Editors :: Vector-Based
+Classifier: Topic :: Utilities
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# meerk40t-barcodes
+MeerK40t 0.8+ Barcode extension.
+
+
+# Barcode-Extension
+
+* Registers the console command: `qrcode` which will generate a qrcode
+
+Usage:    `qrcode x_pos y_pos dim code`
+
+Arguments:
+>     x_pos          X-position of qr-code
+>     y_pos          Y-position of qr-code
+>     dim            Width/length of qr-code
+>     code           Text to create qr-code from
+
+Options:
+>     --boxsize  (-x)      Boxsize (default 10)
+>     --border   (-b)      Border around qr-code (default 4)
+>     --version  (-v)      size (1..40)
+>     --errcorr  (-e)      error correction, one of L (7%), M (15%), Q (25%), H (30%)
+
+* Registers the console command: `barcode` which will generate a barcode
+
+Usage:    `barcode x_pos y_pos dimx dimy btype code`
+
+Arguments:
+>     x_pos     X-Position of barcode
+>     y_pos     Y-Position of barcode
+>     dim       Width of barcode, may be 'auto' to keep native width
+>     dimy      Height of barcode, may be 'auto' to keep native height
+>     btype     Barcode type
+>     code      The code to process
+
+ Options:
+>    --notext  (-n)      suppress text display
+
+* GUI-Support
+The installation of this tool will register a new button in the Design section of MeerK40t:
+<img width="639" alt="image" src="https://user-images.githubusercontent.com/2670784/232893108-c2f4293c-f084-4d5b-8900-b4cbd74f0e38.png">
+
+If you click on it then a dialog will pop up allowing you to design a qr-code / a barcode:
+
+<img width="258" alt="image" src="https://user-images.githubusercontent.com/2670784/232893402-88694837-370a-4b34-a0b7-e9e2ac83c0bc.png">
+
+This will create an element in Meerk40t that can be treated like any other regular path, but which will allow post-creation change of the underlying code (ie the barcode will be regenerated based on the new input).
+
+<img width="432" alt="image" src="https://user-images.githubusercontent.com/2670784/232892296-c3cbae13-53d8-4143-9667-94cdc31cb4a5.png">
+
+# Installing
+* `pip install meerk40t-barcodes`
+Or
+* Download into a directory:
+* `$ pip install .`
+
+# Development
+
+* If you are developing your own extension for meerk40t you will want to use:
+* `$ pip install -e .` this installs the python module in edit mode which allows you to easily see and experience your changes. Without reinstalling your module.
+
+# Acknowledgements
+
+* This MeerK40t extension uses the work of two great libraries to create barcodes & QR codes:
+
+- The python-barcode library (https://github.com/WhyNotHugo/python-barcode)
+- The qrcode library (https://github.com/lincolnloop/python-qrcode)
```

### Comparing `meerk40t-barcodes-0.2.0/barcodes/bcode_logic.py` & `meerk40t-barcodes-0.2.1/barcodes/bcode_logic.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,665 +1,668 @@
-"""
-This module contains the logic to create the different barcode elements
-"""
-
-
-def render_barcode(
-    context,
-    x_pos=None,
-    y_pos=None,
-    dimx=None,
-    dimy=None,
-    btype=None,
-    code=None,
-    notext=None,
-):
-    import barcode
-    from meerk40t.svgelements import Color, Matrix, Path
-
-    def poor_mans_svg_parser(svg_str, actionable):
-        origin_x = float("inf")
-        origin_y = float("inf")
-        maximum_height = 0
-        maximum_width = 0
-        data = []
-        if actionable:
-            # We run through it just to establish
-            # the maximum_width and maximum_height
-            (
-                maximum_width,
-                maximum_height,
-                origin_x,
-                origin_y,
-                dummy_data,
-            ) = poor_mans_svg_parser(svg_str, False)
-            scale_x = 1
-            scale_y = 1
-            if dimx != "auto":
-                if maximum_width - origin_x != 0:
-                    scale_x = elements.length_x(dimx) / (maximum_width - origin_x)
-            if dimy != "auto":
-                if maximum_height - origin_y != 0:
-                    scale_y = elements.length_y(dimy) / (maximum_height - origin_y)
-            offset_x = elements.length_x(x_pos)
-            offset_y = elements.length_y(y_pos)
-        barcodepath = None
-        pathcode = ""
-        pattern_rect = "<rect"
-        pattern_text = "<text"
-        pattern_group_start = "<g "
-        pattern_group_end = "</g>"
-        # A barcode just contains a couple of rects and
-        # a text inside a group, so no need to get overly fancy...
-        # print(svg_str)
-        svg_lines = svg_str.split("\r\n")
-        for line in svg_lines:
-            # print (f"{line}")
-            if pattern_rect in line:
-                subpattern = (
-                    ('height="', "height"),
-                    ('width="', "width"),
-                    ('x="', "x"),
-                    ('y="', "y"),
-                    ('style="', ""),
-                )
-                line_items = line.strip().split(" ")
-                elem = {
-                    "type": "elem rect",
-                    "x": None,
-                    "y": None,
-                    "width": None,
-                    "height": None,
-                    "fill": None,
-                    "stroke": None,
-                }
-                for idx, item in enumerate(line_items):
-                    for pattern in subpattern:
-                        if item.startswith(pattern[0]):
-                            content = item[len(pattern[0]) : -1]
-                            # print (f"Found '{content}' for '{pattern[0]}' in '{item}' --> {pattern[1]}")
-                            key = pattern[1]
-                            if key == "":
-                                # Special case fill/stroke
-                                if "fill:black" in content:
-                                    elem["fill"] = "black"
-                                if "stroke:black" in content:
-                                    elem["stroke"] = "black"
-                            else:
-                                elem[pattern[1]] = content
-                # print (f"Line {line}")
-                # print (f"Decoded {elem['type']}: x={elem['x']}, y={elem['y']}, w={elem['width']}, h={elem['height']}, stroke={elem['stroke']}, fill={elem['fill']}")
-                if elem["x"] is None or elem["y"] is None:
-                    continue
-                if actionable:
-                    this_x = offset_x + scale_x * (
-                        elements.length_x(elem["x"]) - origin_x
-                    )
-                    this_y = offset_y + scale_y * (
-                        elements.length_y(elem["y"]) - origin_y
-                    )
-                    this_wd = scale_x * elements.length_x(elem["width"])
-                    this_ht = scale_y * elements.length_y(elem["height"])
-                    # A direct creation of the path with it's native methods failed for me
-                    # so I circumvent this by preparing a valid SVG path definition and let
-                    # the path parse it - this works, so I assume a flaw in my coding or
-                    # in the underlying application of the matrix (which should be very simple
-                    # as I provide all coordinates in base units) - whatever this method
-                    # works, the other doesn't....
-
-                    # barcodepath.move(this_x, this_y)
-                    # barcodepath.line(this_x + this_wd, this_y)
-                    # barcodepath.line(this_x + this_wd, this_y + this_ht)
-                    # barcodepath.line(this_x, this_y + this_ht)
-                    # barcodepath.line(this_x, this_y)
-                    # barcodepath.closed(relative=True)
-                    pathcode += f"M {this_x:.1f} {this_y:.1f} "
-                    pathcode += f"L {this_x + this_wd:.1f} {this_y:.1f} "
-                    pathcode += f"L {this_x + this_wd:.1f} {this_y + this_ht:.1f} "
-                    pathcode += f"L {this_x:.1f} {this_y + this_ht:.1f} "
-                    pathcode += f"L {this_x:.1f} {this_y:.1f} "
-                    pathcode += f"z "
-                else:
-                    # just establish dimensions
-                    # print (f"check rect extent for x={elem['x']}, y={elem['y']}, wd={elem['width']}, ht={elem['height']}")
-                    this_extent_x = elements.length_x(elem["x"])
-                    this_extent_y = elements.length_y(elem["y"])
-                    this_extent_maxx = this_extent_x + elements.length_x(elem["width"])
-                    this_extent_maxy = this_extent_y + elements.length_y(elem["height"])
-                    origin_x = min(origin_x, this_extent_x)
-                    origin_y = min(origin_y, this_extent_y)
-                    maximum_width = max(maximum_width, this_extent_maxx)
-                    maximum_height = max(maximum_height, this_extent_maxy)
-            elif pattern_text in line:
-                NATIVE_UNIT_PER_INCH = 65535
-                DEFAULT_PPI = 96.0
-                UNITS_PER_PIXEL = NATIVE_UNIT_PER_INCH / DEFAULT_PPI
-                subpattern = (
-                    ('height="', "height"),
-                    ('width="', "width"),
-                    ('x="', "x"),
-                    ('y="', "y"),
-                    ('style="', ""),
-                )
-                stylepattern = (
-                    ("fill:", "fill"),
-                    ("font-size:", "size"),
-                    ("text-anchor:", "anchor"),
-                )
-                elem = {
-                    "type": "elem text",
-                    "text": None,
-                    "x": None,
-                    "y": None,
-                    "size": None,
-                    "anchor": None,
-                    "fill": None,
-                    "stroke": None,
-                }
-                line_items = line.strip().split(" ")
-                for idx, item in enumerate(line_items):
-                    for pattern in subpattern:
-                        if item.startswith(pattern[0]):
-                            content = item[len(pattern[0]) : -1]
-                            # print (f"Found '{content}' for '{pattern[0]}' in '{item}' --> {pattern[1]}")
-                            key = pattern[1]
-                            if key == "":
-                                style_items = content.strip().split(";")
-                                for sidx, sitem in enumerate(style_items):
-                                    # print(f"Styleitem: {sitem}")
-                                    if sitem.startswith('">'):
-                                        content = sitem[2:]
-                                        eidx = content.find("</text")
-                                        if eidx > 0:
-                                            content = content[:eidx]
-                                        elem["text"] = content
-                                        continue
-                                    for spattern in stylepattern:
-                                        if sitem.startswith(spattern[0]):
-                                            content = sitem[len(spattern[0]) :]
-                                            # print (f"Found '{content}' for '{pattern[0]}' in '{item}' --> {pattern[1]}")
-                                            key = spattern[1]
-                                            if key != "":
-                                                elem[spattern[1]] = content
-                            else:
-                                elem[pattern[1]] = content
-
-                # print (f"Line {line}")
-                # print (f"Decoded {elem['type']}: txt='{elem['text']}', x={elem['x']}, y={elem['y']}, anchor={elem['anchor']}, size={elem['size']}, stroke={elem['stroke']}, fill={elem['fill']}")
-                if elem["x"] is None or elem["y"] is None:
-                    continue
-                if actionable and not notext:
-                    this_x = offset_x + scale_x * (
-                        elements.length_x(elem["x"]) - origin_x
-                    )
-                    # Y is always too high - we compensate that by bringing it up
-                    #
-                    compensation = 0
-                    if elem["size"] is not None:
-                        if elem["size"].endswith("pt"):
-                            this_size = float(elem["size"][:-2])
-                        else:
-                            this_size = float(elem["size"])
-                        compensation = 1.25 * this_size * NATIVE_UNIT_PER_INCH / 72
-                    # print (f"Size: {this_size:.1f}, Compensation: {compensation:.1f}")
-                    this_y = (
-                        offset_y
-                        - scale_y * compensation
-                        + scale_y * (elements.length_y(elem["y"]) - origin_y)
-                    )
-                    node = elements.elem_branch.create(
-                        text=elem["text"],
-                        matrix=Matrix(
-                            f"translate({this_x}, {this_y}) scale({UNITS_PER_PIXEL})"
-                        ),
-                        anchor="start" if elem["anchor"] is None else elem["anchor"],
-                        type="elem text",
-                    )
-                    if elem["size"] is not None:
-                        font_size = int(this_size * min(scale_x, scale_y))
-                        if font_size <= 1:
-                            font_size = this_size
-                        node.font_size = font_size
-                    node.stroke = (
-                        None if elem["stroke"] is None else Color(elem["stroke"])
-                    )
-                    node.fill = None if elem["fill"] is None else Color(elem["fill"])
-                    data.append(node)
-                else:
-                    # We establish dimensions, but we don't apply it
-                    # print (f"check text extent for x={elem['x']}, y={elem['y']}")
-                    this_extent_x = elements.length_x(elem["x"])
-                    this_extent_y = elements.length_y(elem["y"])
-                    # maximum_width = max(maximum_width, this_extent_x)
-                    # maximum_height = max(maximum_height, this_extent_y)
-            elif pattern_group_end in line:
-                #  print (f"Group end: '{line}'")
-                if actionable:
-                    # We need to close and add the path
-                    barcodepath = Path(
-                        fill=Color("black"),
-                        stroke=None,
-                        fillrule=0,  # FILLRULE_NONZERO,
-                        matrix=Matrix(),
-                    )
-                    barcodepath.parse(pathcode)
-                    node = elements.elem_branch.create(
-                        path=abs(barcodepath),
-                        stroke_width=0,
-                        stroke_scaled=False,
-                        type="elem path",
-                        fillrule=0,  # nonzero
-                        label=f"{btype}={code}",
-                    )
-                    node.matrix.post_translate(
-                        -node.bounds[0] + offset_x, -node.bounds[1] + offset_y
-                    )
-                    node.modified()
-                    node.stroke = (
-                        None if elem["stroke"] is None else Color(elem["stroke"])
-                    )
-                    node.fill = None if elem["fill"] is None else Color(elem["fill"])
-                    data.append(node)
-
-            elif pattern_group_start in line:
-                # print(f"Group start: '{line}'")
-                if actionable:
-                    pathcode = ""
-        return maximum_width, maximum_height, origin_x, origin_y, data
-
-    elements = context.elements
-    bcode_class = barcode.get_barcode_class(btype)
-    if hasattr(bcode_class, "digits"):
-        digits = getattr(bcode_class, "digits", 0)
-        if digits > 0:
-            while len(code) < digits:
-                code = "0" + code
-    writer = barcode.writer.SVGWriter()
-    try:
-        my_barcode = bcode_class(code, writer=writer)
-    except:
-        return None
-    if hasattr(my_barcode, "build"):
-        my_barcode.build()
-    # print(f"Generated barcode for {code} ({btype})")
-    bytes_result = my_barcode.render()
-    result = bytes_result.decode("utf-8")
-    max_wd, max_ht, ox, oy, data = poor_mans_svg_parser(result, True)
-    return data
-
-
-def create_barcode(
-    kernel,
-    channel,
-    x_pos=None,
-    y_pos=None,
-    dimx=None,
-    dimy=None,
-    btype=None,
-    code=None,
-    notext=None,
-):
-    # ---------------------------------
-    _ = kernel.translation
-    elements = kernel.elements
-    orgcode = code
-    if code is not None:
-        code = elements.mywordlist.translate(code)
-    if btype is None:
-        btype = "ean14"
-    btype = btype.lower()
-    # Check lengths for validity
-    try:
-        if dimx != "auto":
-            __ = elements.length_x(dimx)
-        if dimy != "auto":
-            __ = elements.length_x(dimy)
-        __ = elements.length_x(x_pos)
-        __ = elements.length_y(y_pos)
-    except ValueError:
-        channel(_("Invalid dimensions provided"))
-        return None
-    if notext is None:
-        notext = False
-
-    data = render_barcode(
-        kernel,
-        x_pos=x_pos,
-        y_pos=y_pos,
-        dimx=dimx,
-        dimy=dimy,
-        btype=btype,
-        code=code,
-        notext=notext,
-    )
-    if data is None:
-        return None
-
-    groupnode = None
-    if len(data) > 0:
-        groupnode = elements.elem_branch.add(type="group", label=f"{btype} - {orgcode}")
-
-    for node in data:
-        if node.type == "elem path":
-            # We store the data for later customisation
-            node.mktext = orgcode
-            node.mkbarcode = "ean"
-            node.mkparam = btype
-            node._translated_text = code
-        elements.elem_branch.add_node(node)
-        if groupnode is not None:
-            groupnode.append_child(node)
-    return data
-
-
-def update_barcode(context, node, code):
-    if node is None:
-        return
-    if (
-        not hasattr(node, "mktext")
-        or not hasattr(node, "mkbarcode")
-        or getattr(node, "mkbarcode") != "ean"
-    ):
-        return
-
-    elements = context.elements
-    oldcode = node.mktext
-    if oldcode is not None:
-        oldcode = elements.mywordlist.translate(code)
-    orgcode = code
-    if code is not None:
-        code = elements.mywordlist.translate(code)
-    # print(f"ean update called with {code} ({orgcode}) for {node.label}")
-
-    btype = getattr(node, "mkparam", "")
-    if btype == "":
-        btype = "ean14"
-    bb = node.path.bbox(False)
-    x_pos = bb[0]
-    y_pos = bb[1]
-    dimx = bb[2] - bb[0]
-    dimy = bb[3] - bb[1]
-    notext = False
-    data = render_barcode(
-        context=context,
-        x_pos=x_pos,
-        y_pos=y_pos,
-        dimx=dimx,
-        dimy=dimy,
-        btype=btype,
-        code=code,
-        notext=notext,
-    )
-    if data is None:
-        return None
-    newcode = None
-    for e in data:
-        if e.type == "elem path":
-            olda = node.path.transform.a
-            oldb = node.path.transform.b
-            oldc = node.path.transform.c
-            oldd = node.path.transform.d
-            olde = node.path.transform.e
-            oldf = node.path.transform.f
-            node.path = abs(e.path)
-            node.path.transform.reset()
-            node.path.transform.a = olda
-            node.path.transform.b = oldb
-            node.path.transform.c = oldc
-            node.path.transform.d = oldd
-            node.path.transform.e = olde
-            node.path.transform.f = oldf
-
-            node.mktext = orgcode
-            node._translated_text = code
-            node.altered()
-        elif e.type == "elem text":
-            newcode = e.text
-    # Let's see if we can find a text node in the same group as this...
-    if newcode is None or oldcode is None:
-        return
-    parent = node.parent
-    if parent.type == "group" and len(parent.children) == 2:
-        for e in parent.children:
-            if e.type == "elem text":
-                e.text = newcode
-                e.modified()
-
-
-def render_qr(context, version, errc, boxsize, border, wd, code):
-    import qrcode
-    import qrcode.image.svg
-    from meerk40t.core.units import Length
-    from meerk40t.svgelements import Matrix, Path
-
-    path = None
-    elements = context.elements
-    qr = qrcode.QRCode(
-        version=version,
-        error_correction=errc,
-        box_size=boxsize,
-        border=border,
-    )
-
-    qr.add_data(code)
-    factory = qrcode.image.svg.SvgPathImage
-    qr.image_factory = factory
-    if version is None:
-        img = qr.make_image(fit=True)
-    else:
-        img = qr.make_image()
-    # We do get a ready to go svg string, but let's try to
-    # extract some basic information
-    # 1) Dimension
-
-    dim_x = "3cm"
-    dim_y = "3cm"
-    test = Length(wd)
-    txt = str(img.to_string())
-    pattern = 'viewBox="'
-    idx = txt.find(pattern)
-    if idx >= 0:
-        txt = txt[idx + len(pattern) :]
-        idx = txt.find('"')
-        if idx >= 0:
-            txt = txt[:idx]
-            vp = txt.split(" ")
-            dim_x = str(float(vp[2]) - 2 * border) + "mm"
-            dim_y = str(float(vp[3]) - 2 * border) + "mm"
-    svg_x = elements.length_x(dim_x)
-    svg_y = elements.length_y(dim_y)
-    # 2) Path definition
-    txt = str(img.to_string())
-    pathstr = ""
-    pattern = '<path d="'
-    idx = txt.find(pattern)
-    if idx >= 0:
-        txt = txt[idx + len(pattern) :]
-        idx = txt.find(" id=")
-        if idx >= 0:
-            txt = txt[: idx - 1]
-            pathstr = txt
-    if len(pathstr):
-        mm = elements.length("1mm")
-        sx = mm
-        sy = mm
-
-        sx *= wd / svg_x
-        sy *= wd / svg_y
-        # px = -border * mm + xp
-        # py = -border * mm + yp
-        matrix = Matrix(f"scale({sx},{sy})")
-        # channel(f"scale({sx},{sy})")
-        path = Path(
-            fill="black",
-            stroke=None,
-            width=dim_x,
-            height=dim_y,
-            matrix=Matrix(),
-        )
-        path.parse(pathstr)
-        matrix = Matrix(f"scale({sx},{sy})")
-        path.transform *= matrix
-        # channel(f"pathstr={pathstr[:10]}...{pathstr[-10:]}")
-        # channel(f"x={dim_x}, y={dim_y},")
-    return path
-
-
-def create_qr(
-    kernel,
-    channel,
-    x_pos=None,
-    y_pos=None,
-    dim=None,
-    code=None,
-    errcode=None,
-    boxsize=None,
-    border=None,
-    version=None,
-    data=None,
-    **kwargs,
-):
-    import qrcode
-
-    _ = kernel.translation
-    elements = kernel.elements
-    data = []
-    orgcode = code
-    # Make sure we translate any patterns if needed
-    if code is not None:
-        code = elements.mywordlist.translate(orgcode)
-    # - version=None    We don't preestablish the size but let the routine decide
-    # - box_size        controls how many pixels each “box” of the QR code is.
-    # - border          how many boxes thick the border should be (the default
-    #                   is 4, which is the minimum according to the specs).
-    if errcode is None:
-        errcode = "M"
-    errcode = errcode.upper()
-    if errcode == "L":
-        errc = qrcode.constants.ERROR_CORRECT_L
-    elif errcode == "Q":
-        errc = qrcode.constants.ERROR_CORRECT_Q
-    elif errcode == "H":
-        errc = qrcode.constants.ERROR_CORRECT_H
-    else:
-        errc = qrcode.constants.ERROR_CORRECT_M
-    if border is None or border < 4:
-        border = 4
-    if boxsize is None:
-        boxsize = 10
-    try:
-        xp = elements.length_x(x_pos)
-        yp = elements.length_y(y_pos)
-        wd = elements.length(dim)
-    except ValueError:
-        channel(_("Invalid dimensions provided"))
-        return None
-    path = render_qr(kernel, version, errc, boxsize, border, wd, code)
-    if path is None:
-        return None
-    node = elements.elem_branch.add(
-        path=abs(path),
-        stroke_width=0,
-        stroke_scaled=False,
-        type="elem path",
-        fillrule=0,  # nonzero
-        label=f"qr={code}",
-    )
-    node.matrix.post_translate(-node.bounds[0] + xp, -node.bounds[1] + yp)
-    node.modified()
-    node.mktext = orgcode
-    node._translated_text = code
-    node.mkbarcode = "qr"
-    node.mkparam = (version, errc, boxsize, border)
-
-    data = [node]
-    return data
-
-
-def update_qr(context, node, code):
-    import qrcode
-
-    if node is None:
-        return
-    if (
-        not hasattr(node, "mktext")
-        or not hasattr(node, "mkbarcode")
-        or getattr(node, "mkbarcode") != "qr"
-    ):
-        return
-    elements = context.elements
-    orgcode = code
-    if code is not None:
-        code = elements.mywordlist.translate(orgcode)
-    print(f"qr update called with {code} ({orgcode}) for {node.label}")
-
-    version = None
-    errcode = "M"
-    if errcode == "L":
-        errc = qrcode.constants.ERROR_CORRECT_L
-    elif errcode == "Q":
-        errc = qrcode.constants.ERROR_CORRECT_Q
-    elif errcode == "H":
-        errc = qrcode.constants.ERROR_CORRECT_H
-    else:
-        errc = qrcode.constants.ERROR_CORRECT_M
-
-    boxsize = 10
-    border = 4
-    if hasattr(node, "mkparam"):
-        valu = node.mkparam
-        if isinstance(valu, (list, tuple)) and len(valu) > 3:
-            version = valu[0]
-            errc = valu[1]
-            boxsize = valu[2]
-            border = valu[3]
-
-    bb = node.path.bbox(False)
-    wd = bb[2] - bb[0]
-    path = render_qr(context, version, errc, boxsize, border, wd, code)
-
-    # DEBUG CODE
-    # bb = node.bounds
-    # oldwd1 = bb[2] - bb[0]
-    # bb = node.path.bbox(False)
-    # oldwd2 = bb[2] - bb[0]
-    # bb = path.bbox(False)
-    # midwd2 = bb[2] - bb[0]
-    # olds = str(node.path)[0:50]
-    # news = str(path)[0:50]
-
-    olda = node.path.transform.a
-    oldb = node.path.transform.b
-    oldc = node.path.transform.c
-    oldd = node.path.transform.d
-    olde = node.path.transform.e
-    oldf = node.path.transform.f
-    np = abs(path)
-    from copy import copy
-
-    node.path = copy(np)
-    node.path.transform.reset()
-    node.path.transform.a = olda
-    node.path.transform.b = oldb
-    node.path.transform.c = oldc
-    node.path.transform.d = oldd
-    node.path.transform.e = olde
-    node.path.transform.f = oldf
-    # print (f"x={node.mkcoordx}, y={node.mkcoordy}")
-
-    # oldtext = node.mktext
-    # old_trans = getattr(node, "_translated_text", "")
-
-    node.mktext = orgcode
-    node._translated_text = code
-    node.altered()
-
-    # DEBUG CODE
-    # bb = node.bounds
-    # newwd1 = bb[2] - bb[0]
-    # bb = node.path.bbox(False)
-    # newwd2 = bb[2] - bb[0]
-
-    # print(f"Updated: from {oldtext} ({old_trans}) -> {orgcode} ({code})")
-    # print(f"Old width: {oldwd1:.2f} ({oldwd2:.2f}), mid: ({midwd2:.2f}), new:{newwd1:.2f} ({newwd2:.2f})")
-    # print(f"Old: {olds}")
-    # print(f"New: {news}")
+"""
+This module contains the logic to create the different barcode elements
+"""
+
+
+def render_barcode(
+    context,
+    x_pos=None,
+    y_pos=None,
+    dimx=None,
+    dimy=None,
+    btype=None,
+    code=None,
+    notext=None,
+):
+    import barcode
+    from meerk40t.svgelements import Color, Matrix, Path
+
+    def poor_mans_svg_parser(svg_str, actionable):
+        origin_x = float("inf")
+        origin_y = float("inf")
+        maximum_height = 0
+        maximum_width = 0
+        data = []
+        if actionable:
+            # We run through it just to establish
+            # the maximum_width and maximum_height
+            (
+                maximum_width,
+                maximum_height,
+                origin_x,
+                origin_y,
+                dummy_data,
+            ) = poor_mans_svg_parser(svg_str, False)
+            scale_x = 1
+            scale_y = 1
+            if dimx != "auto":
+                if maximum_width - origin_x != 0:
+                    scale_x = elements.length_x(dimx) / (maximum_width - origin_x)
+            if dimy != "auto":
+                if maximum_height - origin_y != 0:
+                    scale_y = elements.length_y(dimy) / (maximum_height - origin_y)
+            offset_x = elements.length_x(x_pos)
+            offset_y = elements.length_y(y_pos)
+        barcodepath = None
+        pathcode = ""
+        pattern_rect = "<rect"
+        pattern_text = "<text"
+        pattern_group_start = "<g "
+        pattern_group_end = "</g>"
+        # A barcode just contains a couple of rects and
+        # a text inside a group, so no need to get overly fancy...
+        # print(svg_str)
+        svg_lines = svg_str.split("\r\n")
+        if len(svg_lines) <= 1:
+            svg_lines = svg_str.split("\n")
+        
+        for line in svg_lines:
+            # print (f"{line}")
+            if pattern_rect in line:
+                subpattern = (
+                    ('height="', "height"),
+                    ('width="', "width"),
+                    ('x="', "x"),
+                    ('y="', "y"),
+                    ('style="', ""),
+                )
+                line_items = line.strip().split(" ")
+                elem = {
+                    "type": "elem rect",
+                    "x": None,
+                    "y": None,
+                    "width": None,
+                    "height": None,
+                    "fill": None,
+                    "stroke": None,
+                }
+                for idx, item in enumerate(line_items):
+                    for pattern in subpattern:
+                        if item.startswith(pattern[0]):
+                            content = item[len(pattern[0]) : -1]
+                            # print (f"Found '{content}' for '{pattern[0]}' in '{item}' --> {pattern[1]}")
+                            key = pattern[1]
+                            if key == "":
+                                # Special case fill/stroke
+                                if "fill:black" in content:
+                                    elem["fill"] = "black"
+                                if "stroke:black" in content:
+                                    elem["stroke"] = "black"
+                            else:
+                                elem[pattern[1]] = content
+                # print (f"Line {line}")
+                # print (f"Decoded {elem['type']}: x={elem['x']}, y={elem['y']}, w={elem['width']}, h={elem['height']}, stroke={elem['stroke']}, fill={elem['fill']}")
+                if elem["x"] is None or elem["y"] is None:
+                    continue
+                if actionable:
+                    this_x = offset_x + scale_x * (
+                        elements.length_x(elem["x"]) - origin_x
+                    )
+                    this_y = offset_y + scale_y * (
+                        elements.length_y(elem["y"]) - origin_y
+                    )
+                    this_wd = scale_x * elements.length_x(elem["width"])
+                    this_ht = scale_y * elements.length_y(elem["height"])
+                    # A direct creation of the path with it's native methods failed for me
+                    # so I circumvent this by preparing a valid SVG path definition and let
+                    # the path parse it - this works, so I assume a flaw in my coding or
+                    # in the underlying application of the matrix (which should be very simple
+                    # as I provide all coordinates in base units) - whatever this method
+                    # works, the other doesn't....
+
+                    # barcodepath.move(this_x, this_y)
+                    # barcodepath.line(this_x + this_wd, this_y)
+                    # barcodepath.line(this_x + this_wd, this_y + this_ht)
+                    # barcodepath.line(this_x, this_y + this_ht)
+                    # barcodepath.line(this_x, this_y)
+                    # barcodepath.closed(relative=True)
+                    pathcode += f"M {this_x:.1f} {this_y:.1f} "
+                    pathcode += f"L {this_x + this_wd:.1f} {this_y:.1f} "
+                    pathcode += f"L {this_x + this_wd:.1f} {this_y + this_ht:.1f} "
+                    pathcode += f"L {this_x:.1f} {this_y + this_ht:.1f} "
+                    pathcode += f"L {this_x:.1f} {this_y:.1f} "
+                    pathcode += f"z "
+                else:
+                    # just establish dimensions
+                    # print (f"check rect extent for x={elem['x']}, y={elem['y']}, wd={elem['width']}, ht={elem['height']}")
+                    this_extent_x = elements.length_x(elem["x"])
+                    this_extent_y = elements.length_y(elem["y"])
+                    this_extent_maxx = this_extent_x + elements.length_x(elem["width"])
+                    this_extent_maxy = this_extent_y + elements.length_y(elem["height"])
+                    origin_x = min(origin_x, this_extent_x)
+                    origin_y = min(origin_y, this_extent_y)
+                    maximum_width = max(maximum_width, this_extent_maxx)
+                    maximum_height = max(maximum_height, this_extent_maxy)
+            elif pattern_text in line:
+                NATIVE_UNIT_PER_INCH = 65535
+                DEFAULT_PPI = 96.0
+                UNITS_PER_PIXEL = NATIVE_UNIT_PER_INCH / DEFAULT_PPI
+                subpattern = (
+                    ('height="', "height"),
+                    ('width="', "width"),
+                    ('x="', "x"),
+                    ('y="', "y"),
+                    ('style="', ""),
+                )
+                stylepattern = (
+                    ("fill:", "fill"),
+                    ("font-size:", "size"),
+                    ("text-anchor:", "anchor"),
+                )
+                elem = {
+                    "type": "elem text",
+                    "text": None,
+                    "x": None,
+                    "y": None,
+                    "size": None,
+                    "anchor": None,
+                    "fill": None,
+                    "stroke": None,
+                }
+                line_items = line.strip().split(" ")
+                for idx, item in enumerate(line_items):
+                    for pattern in subpattern:
+                        if item.startswith(pattern[0]):
+                            content = item[len(pattern[0]) : -1]
+                            # print (f"Found '{content}' for '{pattern[0]}' in '{item}' --> {pattern[1]}")
+                            key = pattern[1]
+                            if key == "":
+                                style_items = content.strip().split(";")
+                                for sidx, sitem in enumerate(style_items):
+                                    # print(f"Styleitem: {sitem}")
+                                    if sitem.startswith('">'):
+                                        content = sitem[2:]
+                                        eidx = content.find("</text")
+                                        if eidx > 0:
+                                            content = content[:eidx]
+                                        elem["text"] = content
+                                        continue
+                                    for spattern in stylepattern:
+                                        if sitem.startswith(spattern[0]):
+                                            content = sitem[len(spattern[0]) :]
+                                            # print (f"Found '{content}' for '{pattern[0]}' in '{item}' --> {pattern[1]}")
+                                            key = spattern[1]
+                                            if key != "":
+                                                elem[spattern[1]] = content
+                            else:
+                                elem[pattern[1]] = content
+
+                # print (f"Line {line}")
+                # print (f"Decoded {elem['type']}: txt='{elem['text']}', x={elem['x']}, y={elem['y']}, anchor={elem['anchor']}, size={elem['size']}, stroke={elem['stroke']}, fill={elem['fill']}")
+                if elem["x"] is None or elem["y"] is None:
+                    continue
+                if actionable and not notext:
+                    this_x = offset_x + scale_x * (
+                        elements.length_x(elem["x"]) - origin_x
+                    )
+                    # Y is always too high - we compensate that by bringing it up
+                    #
+                    compensation = 0
+                    if elem["size"] is not None:
+                        if elem["size"].endswith("pt"):
+                            this_size = float(elem["size"][:-2])
+                        else:
+                            this_size = float(elem["size"])
+                        compensation = 1.25 * this_size * NATIVE_UNIT_PER_INCH / 72
+                    # print (f"Size: {this_size:.1f}, Compensation: {compensation:.1f}")
+                    this_y = (
+                        offset_y
+                        - scale_y * compensation
+                        + scale_y * (elements.length_y(elem["y"]) - origin_y)
+                    )
+                    node = elements.elem_branch.create(
+                        text=elem["text"],
+                        matrix=Matrix(
+                            f"translate({this_x}, {this_y}) scale({UNITS_PER_PIXEL})"
+                        ),
+                        anchor="start" if elem["anchor"] is None else elem["anchor"],
+                        type="elem text",
+                    )
+                    if elem["size"] is not None:
+                        font_size = int(this_size * min(scale_x, scale_y))
+                        if font_size <= 1:
+                            font_size = this_size
+                        node.font_size = font_size
+                    node.stroke = (
+                        None if elem["stroke"] is None else Color(elem["stroke"])
+                    )
+                    node.fill = None if elem["fill"] is None else Color(elem["fill"])
+                    data.append(node)
+                else:
+                    # We establish dimensions, but we don't apply it
+                    # print (f"check text extent for x={elem['x']}, y={elem['y']}")
+                    this_extent_x = elements.length_x(elem["x"])
+                    this_extent_y = elements.length_y(elem["y"])
+                    # maximum_width = max(maximum_width, this_extent_x)
+                    # maximum_height = max(maximum_height, this_extent_y)
+            elif pattern_group_end in line:
+                #  print (f"Group end: '{line}'")
+                if actionable:
+                    # We need to close and add the path
+                    barcodepath = Path(
+                        fill=Color("black"),
+                        stroke=None,
+                        fillrule=0,  # FILLRULE_NONZERO,
+                        matrix=Matrix(),
+                    )
+                    barcodepath.parse(pathcode)
+                    node = elements.elem_branch.create(
+                        path=abs(barcodepath),
+                        stroke_width=0,
+                        stroke_scaled=False,
+                        type="elem path",
+                        fillrule=0,  # nonzero
+                        label=f"{btype}={code}",
+                    )
+                    node.matrix.post_translate(
+                        -node.bounds[0] + offset_x, -node.bounds[1] + offset_y
+                    )
+                    node.modified()
+                    node.stroke = (
+                        None if elem["stroke"] is None else Color(elem["stroke"])
+                    )
+                    node.fill = None if elem["fill"] is None else Color(elem["fill"])
+                    data.append(node)
+
+            elif pattern_group_start in line:
+                # print(f"Group start: '{line}'")
+                if actionable:
+                    pathcode = ""
+        return maximum_width, maximum_height, origin_x, origin_y, data
+
+    elements = context.elements
+    bcode_class = barcode.get_barcode_class(btype)
+    if hasattr(bcode_class, "digits"):
+        digits = getattr(bcode_class, "digits", 0)
+        if digits > 0:
+            while len(code) < digits:
+                code = "0" + code
+    writer = barcode.writer.SVGWriter()
+    try:
+        my_barcode = bcode_class(code, writer=writer)
+    except:
+        return None
+    if hasattr(my_barcode, "build"):
+        my_barcode.build()
+    # print(f"Generated barcode for {code} ({btype})")
+    bytes_result = my_barcode.render()
+    result = bytes_result.decode("utf-8")
+    max_wd, max_ht, ox, oy, data = poor_mans_svg_parser(result, True)
+    return data
+
+
+def create_barcode(
+    kernel,
+    channel,
+    x_pos=None,
+    y_pos=None,
+    dimx=None,
+    dimy=None,
+    btype=None,
+    code=None,
+    notext=None,
+):
+    # ---------------------------------
+    _ = kernel.translation
+    elements = kernel.elements
+    orgcode = code
+    if code is not None:
+        code = elements.mywordlist.translate(code)
+    if btype is None:
+        btype = "ean14"
+    btype = btype.lower()
+    # Check lengths for validity
+    try:
+        if dimx != "auto":
+            __ = elements.length_x(dimx)
+        if dimy != "auto":
+            __ = elements.length_x(dimy)
+        __ = elements.length_x(x_pos)
+        __ = elements.length_y(y_pos)
+    except ValueError:
+        channel(_("Invalid dimensions provided"))
+        return None
+    if notext is None:
+        notext = False
+
+    data = render_barcode(
+        kernel,
+        x_pos=x_pos,
+        y_pos=y_pos,
+        dimx=dimx,
+        dimy=dimy,
+        btype=btype,
+        code=code,
+        notext=notext,
+    )
+    if data is None:
+        return None
+
+    groupnode = None
+    if len(data) > 0:
+        groupnode = elements.elem_branch.add(type="group", label=f"{btype} - {orgcode}")
+
+    for node in data:
+        if node.type == "elem path":
+            # We store the data for later customisation
+            node.mktext = orgcode
+            node.mkbarcode = "ean"
+            node.mkparam = btype
+            node._translated_text = code
+        elements.elem_branch.add_node(node)
+        if groupnode is not None:
+            groupnode.append_child(node)
+    return data
+
+
+def update_barcode(context, node, code):
+    if node is None:
+        return
+    if (
+        not hasattr(node, "mktext")
+        or not hasattr(node, "mkbarcode")
+        or getattr(node, "mkbarcode") != "ean"
+    ):
+        return
+
+    elements = context.elements
+    oldcode = node.mktext
+    if oldcode is not None:
+        oldcode = elements.mywordlist.translate(code)
+    orgcode = code
+    if code is not None:
+        code = elements.mywordlist.translate(code)
+    # print(f"ean update called with {code} ({orgcode}) for {node.label}")
+
+    btype = getattr(node, "mkparam", "")
+    if btype == "":
+        btype = "ean14"
+    bb = node.path.bbox(False)
+    x_pos = bb[0]
+    y_pos = bb[1]
+    dimx = bb[2] - bb[0]
+    dimy = bb[3] - bb[1]
+    notext = False
+    data = render_barcode(
+        context=context,
+        x_pos=x_pos,
+        y_pos=y_pos,
+        dimx=dimx,
+        dimy=dimy,
+        btype=btype,
+        code=code,
+        notext=notext,
+    )
+    if data is None:
+        return None
+    newcode = None
+    for e in data:
+        if e.type == "elem path":
+            olda = node.path.transform.a
+            oldb = node.path.transform.b
+            oldc = node.path.transform.c
+            oldd = node.path.transform.d
+            olde = node.path.transform.e
+            oldf = node.path.transform.f
+            node.path = abs(e.path)
+            node.path.transform.reset()
+            node.path.transform.a = olda
+            node.path.transform.b = oldb
+            node.path.transform.c = oldc
+            node.path.transform.d = oldd
+            node.path.transform.e = olde
+            node.path.transform.f = oldf
+
+            node.mktext = orgcode
+            node._translated_text = code
+            node.altered()
+        elif e.type == "elem text":
+            newcode = e.text
+    # Let's see if we can find a text node in the same group as this...
+    if newcode is None or oldcode is None:
+        return
+    parent = node.parent
+    if parent.type == "group" and len(parent.children) == 2:
+        for e in parent.children:
+            if e.type == "elem text":
+                e.text = newcode
+                e.modified()
+
+
+def render_qr(context, version, errc, boxsize, border, wd, code):
+    import qrcode
+    import qrcode.image.svg
+    from meerk40t.core.units import Length
+    from meerk40t.svgelements import Matrix, Path
+
+    path = None
+    elements = context.elements
+    qr = qrcode.QRCode(
+        version=version,
+        error_correction=errc,
+        box_size=boxsize,
+        border=border,
+    )
+
+    qr.add_data(code)
+    factory = qrcode.image.svg.SvgPathImage
+    qr.image_factory = factory
+    if version is None:
+        img = qr.make_image(fit=True)
+    else:
+        img = qr.make_image()
+    # We do get a ready to go svg string, but let's try to
+    # extract some basic information
+    # 1) Dimension
+
+    dim_x = "3cm"
+    dim_y = "3cm"
+    test = Length(wd)
+    txt = str(img.to_string())
+    pattern = 'viewBox="'
+    idx = txt.find(pattern)
+    if idx >= 0:
+        txt = txt[idx + len(pattern) :]
+        idx = txt.find('"')
+        if idx >= 0:
+            txt = txt[:idx]
+            vp = txt.split(" ")
+            dim_x = str(float(vp[2]) - 2 * border) + "mm"
+            dim_y = str(float(vp[3]) - 2 * border) + "mm"
+    svg_x = elements.length_x(dim_x)
+    svg_y = elements.length_y(dim_y)
+    # 2) Path definition
+    txt = str(img.to_string())
+    pathstr = ""
+    pattern = '<path d="'
+    idx = txt.find(pattern)
+    if idx >= 0:
+        txt = txt[idx + len(pattern) :]
+        idx = txt.find(" id=")
+        if idx >= 0:
+            txt = txt[: idx - 1]
+            pathstr = txt
+    if len(pathstr):
+        mm = elements.length("1mm")
+        sx = mm
+        sy = mm
+
+        sx *= wd / svg_x
+        sy *= wd / svg_y
+        # px = -border * mm + xp
+        # py = -border * mm + yp
+        matrix = Matrix(f"scale({sx},{sy})")
+        # channel(f"scale({sx},{sy})")
+        path = Path(
+            fill="black",
+            stroke=None,
+            width=dim_x,
+            height=dim_y,
+            matrix=Matrix(),
+        )
+        path.parse(pathstr)
+        matrix = Matrix(f"scale({sx},{sy})")
+        path.transform *= matrix
+        # channel(f"pathstr={pathstr[:10]}...{pathstr[-10:]}")
+        # channel(f"x={dim_x}, y={dim_y},")
+    return path
+
+
+def create_qr(
+    kernel,
+    channel,
+    x_pos=None,
+    y_pos=None,
+    dim=None,
+    code=None,
+    errcode=None,
+    boxsize=None,
+    border=None,
+    version=None,
+    data=None,
+    **kwargs,
+):
+    import qrcode
+
+    _ = kernel.translation
+    elements = kernel.elements
+    data = []
+    orgcode = code
+    # Make sure we translate any patterns if needed
+    if code is not None:
+        code = elements.mywordlist.translate(orgcode)
+    # - version=None    We don't preestablish the size but let the routine decide
+    # - box_size        controls how many pixels each “box” of the QR code is.
+    # - border          how many boxes thick the border should be (the default
+    #                   is 4, which is the minimum according to the specs).
+    if errcode is None:
+        errcode = "M"
+    errcode = errcode.upper()
+    if errcode == "L":
+        errc = qrcode.constants.ERROR_CORRECT_L
+    elif errcode == "Q":
+        errc = qrcode.constants.ERROR_CORRECT_Q
+    elif errcode == "H":
+        errc = qrcode.constants.ERROR_CORRECT_H
+    else:
+        errc = qrcode.constants.ERROR_CORRECT_M
+    if border is None or border < 4:
+        border = 4
+    if boxsize is None:
+        boxsize = 10
+    try:
+        xp = elements.length_x(x_pos)
+        yp = elements.length_y(y_pos)
+        wd = elements.length(dim)
+    except ValueError:
+        channel(_("Invalid dimensions provided"))
+        return None
+    path = render_qr(kernel, version, errc, boxsize, border, wd, code)
+    if path is None:
+        return None
+    node = elements.elem_branch.add(
+        path=abs(path),
+        stroke_width=0,
+        stroke_scaled=False,
+        type="elem path",
+        fillrule=0,  # nonzero
+        label=f"qr={code}",
+    )
+    node.matrix.post_translate(-node.bounds[0] + xp, -node.bounds[1] + yp)
+    node.modified()
+    node.mktext = orgcode
+    node._translated_text = code
+    node.mkbarcode = "qr"
+    node.mkparam = (version, errc, boxsize, border)
+
+    data = [node]
+    return data
+
+
+def update_qr(context, node, code):
+    import qrcode
+
+    if node is None:
+        return
+    if (
+        not hasattr(node, "mktext")
+        or not hasattr(node, "mkbarcode")
+        or getattr(node, "mkbarcode") != "qr"
+    ):
+        return
+    elements = context.elements
+    orgcode = code
+    if code is not None:
+        code = elements.mywordlist.translate(orgcode)
+    # print(f"qr update called with {code} ({orgcode}) for {node.label}")
+
+    version = None
+    errcode = "M"
+    if errcode == "L":
+        errc = qrcode.constants.ERROR_CORRECT_L
+    elif errcode == "Q":
+        errc = qrcode.constants.ERROR_CORRECT_Q
+    elif errcode == "H":
+        errc = qrcode.constants.ERROR_CORRECT_H
+    else:
+        errc = qrcode.constants.ERROR_CORRECT_M
+
+    boxsize = 10
+    border = 4
+    if hasattr(node, "mkparam"):
+        valu = node.mkparam
+        if isinstance(valu, (list, tuple)) and len(valu) > 3:
+            version = valu[0]
+            errc = valu[1]
+            boxsize = valu[2]
+            border = valu[3]
+
+    bb = node.path.bbox(False)
+    wd = bb[2] - bb[0]
+    path = render_qr(context, version, errc, boxsize, border, wd, code)
+
+    # DEBUG CODE
+    # bb = node.bounds
+    # oldwd1 = bb[2] - bb[0]
+    # bb = node.path.bbox(False)
+    # oldwd2 = bb[2] - bb[0]
+    # bb = path.bbox(False)
+    # midwd2 = bb[2] - bb[0]
+    # olds = str(node.path)[0:50]
+    # news = str(path)[0:50]
+
+    olda = node.path.transform.a
+    oldb = node.path.transform.b
+    oldc = node.path.transform.c
+    oldd = node.path.transform.d
+    olde = node.path.transform.e
+    oldf = node.path.transform.f
+    np = abs(path)
+    from copy import copy
+
+    node.path = copy(np)
+    node.path.transform.reset()
+    node.path.transform.a = olda
+    node.path.transform.b = oldb
+    node.path.transform.c = oldc
+    node.path.transform.d = oldd
+    node.path.transform.e = olde
+    node.path.transform.f = oldf
+    # print (f"x={node.mkcoordx}, y={node.mkcoordy}")
+
+    # oldtext = node.mktext
+    # old_trans = getattr(node, "_translated_text", "")
+
+    node.mktext = orgcode
+    node._translated_text = code
+    node.altered()
+
+    # DEBUG CODE
+    # bb = node.bounds
+    # newwd1 = bb[2] - bb[0]
+    # bb = node.path.bbox(False)
+    # newwd2 = bb[2] - bb[0]
+
+    # print(f"Updated: from {oldtext} ({old_trans}) -> {orgcode} ({code})")
+    # print(f"Old width: {oldwd1:.2f} ({oldwd2:.2f}), mid: ({midwd2:.2f}), new:{newwd1:.2f} ({newwd2:.2f})")
+    # print(f"Old: {olds}")
+    # print(f"New: {news}")
```

### Comparing `meerk40t-barcodes-0.2.0/barcodes/gui.py` & `meerk40t-barcodes-0.2.1/barcodes/gui.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,646 +1,646 @@
-import wx
-from barcode import PROVIDED_BARCODES
-
-from .bcode_logic import update_barcode, update_qr
-
-_ = wx.GetTranslation
-
-
-class BarcodeDialog(wx.Dialog):
-
-    # from meerk40t.gui.wxutils import TextCtrl
-
-    def __init__(self, context, *args, **kwds):
-        self.context = context
-        _ = context._
-        self.command = ""
-        # begin wxGlade: RefAlign.__init__
-        kwds["style"] = kwds.get("style", 0) | wx.DEFAULT_DIALOG_STYLE
-        wx.Dialog.__init__(self, *args, **kwds)
-        self.SetTitle(_("Create a barcode"))
-        mainsizer = wx.BoxSizer(wx.VERTICAL)
-
-        input_sizer = wx.StaticBoxSizer(
-            wx.StaticBox(self, wx.ID_ANY, _("Text to use:")), wx.HORIZONTAL
-        )
-        self.text_code = wx.TextCtrl(self, wx.ID_ANY)
-        self.text_code.SetToolTip(
-            _("The barcode/qrcode will be based on this content.")
-        )
-        label = wx.StaticText(self, wx.ID_ANY, label=_("Code:"))
-        input_sizer.Add(label, 0, wx.ALIGN_CENTER_VERTICAL, 0)
-        input_sizer.Add(self.text_code, 1, wx.EXPAND, 0)
-
-        xy_sizer = wx.StaticBoxSizer(
-            wx.StaticBox(self, wx.ID_ANY, _("Coordinates:")), wx.HORIZONTAL
-        )
-        x_sizer = wx.StaticBoxSizer(
-            wx.StaticBox(self, wx.ID_ANY, _("X:")), wx.HORIZONTAL
-        )
-        y_sizer = wx.StaticBoxSizer(
-            wx.StaticBox(self, wx.ID_ANY, _("Y:")), wx.HORIZONTAL
-        )
-        self.text_xpos = wx.TextCtrl(self, wx.ID_ANY, "0cm")
-        self.text_xpos.SetToolTip(
-            _("Where will the barcode will be located (top left corner).")
-        )
-        self.text_xpos.SetMaxSize(wx.Size(100, -1))
-
-        x_sizer.Add(self.text_xpos, 1, wx.EXPAND, 0)
-
-        self.text_ypos = wx.TextCtrl(self, wx.ID_ANY, "0cm")
-        self.text_ypos.SetToolTip(
-            _("Where will the barcode will be located (top left corner).")
-        )
-        self.text_ypos.SetMaxSize(wx.Size(100, -1))
-
-        y_sizer.Add(self.text_ypos, 1, wx.EXPAND, 0)
-        xy_sizer.Add(x_sizer, 1, wx.EXPAND, 0)
-        xy_sizer.Add(y_sizer, 1, wx.EXPAND, 0)
-
-        self.option_qr = wx.RadioButton(self, wx.ID_ANY, _("QR-Code"))
-        self.option_bar = wx.RadioButton(self, wx.ID_ANY, _("Barcode"))
-
-        codes_sizer = wx.BoxSizer(wx.HORIZONTAL)
-        qr_sizer = wx.StaticBoxSizer(
-            wx.StaticBox(self, wx.ID_ANY, _("QR-Code:")), wx.VERTICAL
-        )
-        qrnotebook = wx.Notebook(self, wx.ID_ANY)
-
-        # --------------- Option Panel
-
-        qrmain_panel = wx.Panel(qrnotebook, wx.ID_ANY)
-        qrnotebook.AddPage(qrmain_panel, _("Options"))
-        qroptions_sizer = wx.BoxSizer(wx.VERTICAL)
-        qrmain_panel.SetSizer(qroptions_sizer)
-        qrdim_sizer = wx.BoxSizer(wx.HORIZONTAL)
-        #      --boxsize  (-x)      Boxsize (default 10)
-        #  --border   (-b)      Border around qr-code (default 4)
-        #  --version  (-v)      size (1..40)
-        #  --errcorr  (-e)      error correction, one of L (7%), M (15%), Q (25%), H (30%)
-        label = wx.StaticText(qrmain_panel, wx.ID_ANY, label=_("Width/Height:"))
-        label.SetMinSize(wx.Size(80, -1))
-        self.text_qrdim = wx.TextCtrl(qrmain_panel, wx.ID_ANY, "4cm")
-        self.text_qrdim.SetToolTip(_("How wide/high will the resulting qr-code be?"))
-        self.text_qrdim.SetMaxSize(wx.Size(100, -1))
-        qrdim_sizer.Add(label, 0, wx.ALIGN_CENTER_VERTICAL, 0)
-        qrdim_sizer.Add(self.text_qrdim, 1, wx.EXPAND, 0)
-
-        qrres_sizer = wx.BoxSizer(wx.HORIZONTAL)
-        label = wx.StaticText(qrmain_panel, wx.ID_ANY, label=_("Resolution:"))
-        label.SetMinSize(wx.Size(80, -1))
-        self.text_qrres = wx.TextCtrl(qrmain_panel, wx.ID_ANY, value="1")
-        self.text_qrres.SetToolTip(
-            _("How big will the qr-code become (1..40, default 1)?")
-        )
-        self.text_qrres.SetMaxSize(wx.Size(50, -1))
-        qrres_sizer.Add(label, 0, wx.ALIGN_CENTER_VERTICAL, 0)
-        qrres_sizer.Add(self.text_qrres, 1, wx.EXPAND, 0)
-
-        # qrborder_sizer = wx.BoxSizer(wx.HORIZONTAL)
-        # label = wx.StaticText(self, wx.ID_ANY, label=_("Border:"))
-        # label.SetMinSize(wx.Size(80, -1))
-        # self.text_qrborder = wx.TextCtrl(self, wx.ID_ANY, value="4")
-        # self.text_qrborder.SetToolTip(_("How wide is the border around the qr-code (default 4)?"))
-        # self.text_qrborder.SetMaxSize(wx.Size(50, -1))
-        # qrborder_sizer.Add(label, 0, wx.ALIGN_CENTER_VERTICAL, 0)
-        # qrborder_sizer.Add(self.text_qrborder, 1, wx.EXPAND, 0)
-
-        qrbox_sizer = wx.BoxSizer(wx.HORIZONTAL)
-        label = wx.StaticText(qrmain_panel, wx.ID_ANY, label=_("Boxsize:"))
-        label.SetMinSize(wx.Size(80, -1))
-        self.text_qrbox = wx.TextCtrl(qrmain_panel, wx.ID_ANY, value="10")
-        self.text_qrbox.SetToolTip(
-            _("How big is the boxsize of the pixels (default 10)?")
-        )
-        self.text_qrbox.SetMaxSize(wx.Size(50, -1))
-        qrbox_sizer.Add(label, 0, wx.ALIGN_CENTER_VERTICAL, 0)
-        qrbox_sizer.Add(self.text_qrbox, 1, wx.EXPAND, 0)
-
-        qrerrcorr_sizer = wx.BoxSizer(wx.HORIZONTAL)
-        label = wx.StaticText(qrmain_panel, wx.ID_ANY, label=_("Error:"))
-        label.SetMinSize(wx.Size(80, -1))
-        errchoices = ["L (7%)", "M (15%)", "Q (25%)", "H (30%)"]
-        self.combo_errcorr = wx.ComboBox(
-            qrmain_panel,
-            wx.ID_ANY,
-            choices=errchoices,
-            style=wx.CB_DROPDOWN | wx.CB_READONLY,
-        )
-        self.combo_errcorr.SetToolTip(
-            _("Establish the error correction used for the QR Code")
-        )
-        self.combo_errcorr.SetSelection(1)  # (M)
-        qrerrcorr_sizer.Add(label, 0, wx.ALIGN_CENTER_VERTICAL, 0)
-        qrerrcorr_sizer.Add(self.combo_errcorr, 1, wx.EXPAND, 0)
-
-        qroptions_sizer.Add(qrdim_sizer, 0, wx.EXPAND, 0)
-        qroptions_sizer.Add(qrres_sizer, 0, wx.EXPAND, 0)
-        # qroptions_sizer.Add(qrborder_sizer, 0, wx.EXPAND, 0)
-        qroptions_sizer.Add(qrbox_sizer, 0, wx.EXPAND, 0)
-        qroptions_sizer.Add(qrerrcorr_sizer, 0, wx.EXPAND, 0)
-
-        # --------------- WIFI PANEL
-
-        qrwifi_panel = wx.Panel(qrnotebook, wx.ID_ANY)
-        qrnotebook.AddPage(qrwifi_panel, _("WiFi"))
-        qrwifi_sizer = wx.BoxSizer(wx.VERTICAL)
-        qrwifi_panel.SetSizer(qrwifi_sizer)
-        qrwifi_ssid_sizer = wx.BoxSizer(wx.HORIZONTAL)
-        self.text_wifi_ssid = wx.TextCtrl(qrwifi_panel, wx.ID_ANY)
-        ssid_label = wx.StaticText(qrwifi_panel, wx.ID_ANY, _("SSID:"))
-        ssid_label.SetMinSize(wx.Size(45, -1))
-        qrwifi_ssid_sizer.Add(ssid_label, 0, wx.ALIGN_CENTER_VERTICAL, 0)
-        qrwifi_ssid_sizer.Add(self.text_wifi_ssid, 1, wx.EXPAND, 0)
-
-        qrwifi_passwd_sizer = wx.BoxSizer(wx.HORIZONTAL)
-
-        self.text_wifi_password = wx.TextCtrl(qrwifi_panel, wx.ID_ANY)
-        pass_label = wx.StaticText(qrwifi_panel, wx.ID_ANY, _("Key:"))
-        pass_label.SetMinSize(wx.Size(45, -1))
-        qrwifi_passwd_sizer.Add(pass_label, 0, wx.ALIGN_CENTER_VERTICAL, 0)
-        qrwifi_passwd_sizer.Add(self.text_wifi_password, 1, wx.EXPAND, 0)
-
-        qrwifi_wpa_sizer = wx.BoxSizer(wx.HORIZONTAL)
-        self.combo_wifi_wpa = wx.ComboBox(
-            qrwifi_panel,
-            wx.ID_ANY,
-            choices=(_("WPA/WPA2/WPA3"), _("WEP"), _("None")),
-            style=wx.CB_DROPDOWN | wx.CB_READONLY,
-        )
-        self.combo_wifi_wpa.SetToolTip(
-            _("What kind of encryption does the network use?")
-        )
-        self.combo_wifi_wpa.SetSelection(0)  # WPA
-        wpa_label = wx.StaticText(qrwifi_panel, wx.ID_ANY, _("Encryption:"))
-        qrwifi_wpa_sizer.Add(wpa_label, 0, wx.ALIGN_CENTER_VERTICAL, 0)
-        qrwifi_wpa_sizer.Add(self.combo_wifi_wpa, 0, wx.EXPAND, 0)
-
-        qrwifi_hidden_sizer = wx.BoxSizer(wx.HORIZONTAL)
-
-        self.check_hidden = wx.CheckBox(qrwifi_panel, wx.ID_ANY, _("Hidden"))
-        self.check_hidden.SetToolTip(_("Is the network hidden?"))
-        self.check_hidden.SetValue(False)
-        qrwifi_hidden_sizer.Add(self.check_hidden, 0, wx.ALIGN_CENTER_VERTICAL, 0)
-
-        qrwifi_sizer.Add(qrwifi_ssid_sizer, 0, wx.EXPAND, 0)
-        qrwifi_sizer.Add(qrwifi_passwd_sizer, 0, wx.EXPAND, 0)
-        qrwifi_sizer.Add(qrwifi_wpa_sizer, 0, wx.EXPAND, 0)
-        qrwifi_sizer.Add(qrwifi_hidden_sizer, 0, wx.EXPAND, 0)
-        self.button_wifi = wx.Button(qrwifi_panel, wx.ID_ANY, _("Generate Pattern"))
-        qrwifi_sizer.Add(self.button_wifi, 0, 0, 0)
-        self.button_wifi.Bind(wx.EVT_BUTTON, self.on_wifi)
-
-        # --------------- WIFI PANEL
-
-        qrvcard_panel = wx.Panel(qrnotebook, wx.ID_ANY)
-        qrnotebook.AddPage(qrvcard_panel, _("VCard"))
-        qrvcard_sizer = wx.BoxSizer(wx.VERTICAL)
-        qrvcard_panel.SetSizer(qrvcard_sizer)
-        qrvcard_name = wx.BoxSizer(wx.HORIZONTAL)
-        self.text_vcard_name = wx.TextCtrl(qrvcard_panel, wx.ID_ANY)
-        self.text_vcard_name.SetToolTip(_("Provide your name as lastname,firstname"))
-        vcard_name_label = wx.StaticText(qrvcard_panel, wx.ID_ANY, _("Name:"))
-        vcard_name_label.SetMinSize(wx.Size(45, -1))
-        qrvcard_name.Add(vcard_name_label, 0, wx.ALIGN_CENTER_VERTICAL, 0)
-        qrvcard_name.Add(self.text_vcard_name, 1, wx.EXPAND, 0)
-
-        qrvcard_address = wx.BoxSizer(wx.HORIZONTAL)
-        self.text_vcard_address = wx.TextCtrl(qrvcard_panel, wx.ID_ANY)
-        self.text_vcard_address.SetToolTip(
-            _(
-                "Provide your address as:\n"
-                + "PO box, room number, house number, city, prefecture, zip code and country"
-            )
-        )
-        vcard_address_label = wx.StaticText(qrvcard_panel, wx.ID_ANY, _("Address:"))
-        vcard_address_label.SetMinSize(wx.Size(45, -1))
-        qrvcard_address.Add(vcard_address_label, 0, wx.ALIGN_CENTER_VERTICAL, 0)
-        qrvcard_address.Add(self.text_vcard_address, 1, wx.EXPAND, 0)
-
-        qrvcard_tel = wx.BoxSizer(wx.HORIZONTAL)
-        self.text_vcard_tel = wx.TextCtrl(qrvcard_panel, wx.ID_ANY)
-        self.text_vcard_tel.SetToolTip(_("Provide your phone-number"))
-        vcard_tel_label = wx.StaticText(qrvcard_panel, wx.ID_ANY, _("Phone:"))
-        vcard_tel_label.SetMinSize(wx.Size(45, -1))
-        qrvcard_tel.Add(vcard_tel_label, 0, wx.ALIGN_CENTER_VERTICAL, 0)
-        qrvcard_tel.Add(self.text_vcard_tel, 1, wx.EXPAND, 0)
-
-        qrvcard_email = wx.BoxSizer(wx.HORIZONTAL)
-        self.text_vcard_email = wx.TextCtrl(qrvcard_panel, wx.ID_ANY)
-        self.text_vcard_email.SetToolTip(_("Provide your email-Address"))
-        vcard_email_label = wx.StaticText(qrvcard_panel, wx.ID_ANY, _("email:"))
-        vcard_email_label.SetMinSize(wx.Size(45, -1))
-        qrvcard_email.Add(vcard_email_label, 0, wx.ALIGN_CENTER_VERTICAL, 0)
-        qrvcard_email.Add(self.text_vcard_email, 1, wx.EXPAND, 0)
-
-        qrvcard_url = wx.BoxSizer(wx.HORIZONTAL)
-        self.text_vcard_url = wx.TextCtrl(qrvcard_panel, wx.ID_ANY)
-        self.text_vcard_url.SetToolTip(_("Provide a valid URL"))
-        vcard_url_label = wx.StaticText(qrvcard_panel, wx.ID_ANY, _("URL:"))
-        vcard_url_label.SetMinSize(wx.Size(45, -1))
-        qrvcard_url.Add(vcard_url_label, 0, wx.ALIGN_CENTER_VERTICAL, 0)
-        qrvcard_url.Add(self.text_vcard_url, 1, wx.EXPAND, 0)
-
-        qrvcard_sizer.Add(qrvcard_name, 0, wx.EXPAND, 0)
-        qrvcard_sizer.Add(qrvcard_address, 0, wx.EXPAND, 0)
-        qrvcard_sizer.Add(qrvcard_tel, 0, wx.EXPAND, 0)
-        qrvcard_sizer.Add(qrvcard_email, 0, wx.EXPAND, 0)
-        qrvcard_sizer.Add(qrvcard_url, 0, wx.EXPAND, 0)
-        self.button_vcard = wx.Button(qrvcard_panel, wx.ID_ANY, _("Generate Pattern"))
-        qrvcard_sizer.Add(self.button_vcard, 0, 0, 0)
-        self.button_vcard.Bind(wx.EVT_BUTTON, self.on_vcard)
-
-        # --------------- Barcode Section
-
-        bar_sizer = wx.StaticBoxSizer(
-            wx.StaticBox(self, wx.ID_ANY, _("Barcode:")), wx.VERTICAL
-        )
-        baroptions_sizer = wx.StaticBoxSizer(
-            wx.StaticBox(self, wx.ID_ANY, _("Options:")), wx.VERTICAL
-        )
-
-        bartype_sizer = wx.BoxSizer(wx.HORIZONTAL)
-        label = wx.StaticText(self, wx.ID_ANY, label=_("Type:"))
-        label.SetMinSize(wx.Size(80, -1))
-        self.combo_barcode = wx.ComboBox(
-            self,
-            wx.ID_ANY,
-            choices=PROVIDED_BARCODES,
-            style=wx.CB_DROPDOWN | wx.CB_READONLY,
-        )
-        self.combo_barcode.SetToolTip(_("What kind of barcode do you want to create?"))
-        self.combo_barcode.SetSelection(4)  # ean13
-        bartype_sizer.Add(label, 0, wx.ALIGN_CENTER_VERTICAL, 0)
-        bartype_sizer.Add(self.combo_barcode, 1, wx.EXPAND, 0)
-
-        bardimx_sizer = wx.BoxSizer(wx.HORIZONTAL)
-        label = wx.StaticText(self, wx.ID_ANY, label=_("Width:"))
-        label.SetMinSize(wx.Size(80, -1))
-        self.text_bardimx = wx.TextCtrl(self, wx.ID_ANY, "auto")
-        self.text_bardimx.SetToolTip(_("How wide will the resulting barcode be?"))
-        self.text_bardimx.SetMaxSize(wx.Size(100, -1))
-        bardimx_sizer.Add(label, 0, wx.ALIGN_CENTER_VERTICAL, 0)
-        bardimx_sizer.Add(self.text_bardimx, 1, wx.EXPAND, 0)
-
-        bardimy_sizer = wx.BoxSizer(wx.HORIZONTAL)
-        label = wx.StaticText(self, wx.ID_ANY, label=_("Height:"))
-        label.SetMinSize(wx.Size(80, -1))
-        self.text_bardimy = wx.TextCtrl(self, wx.ID_ANY, "auto")
-        self.text_bardimy.SetToolTip(_("How high will the resulting barcode be?"))
-        self.text_bardimy.SetMaxSize(wx.Size(100, -1))
-        bardimy_sizer.Add(label, 0, wx.ALIGN_CENTER_VERTICAL, 0)
-        bardimy_sizer.Add(self.text_bardimy, 1, wx.EXPAND, 0)
-
-        barcheck1_sizer = wx.BoxSizer(wx.HORIZONTAL)
-        label = wx.StaticText(self, wx.ID_ANY, label=_("No text:"))
-        label.SetMinSize(wx.Size(80, -1))
-        self.check_suppress = wx.CheckBox(self, wx.ID_ANY, "")
-        self.check_suppress.SetToolTip(_("Suppress the text under the barcode?"))
-        self.check_suppress.SetMinSize(self.text_bardimx.GetSize())
-        barcheck1_sizer.Add(label, 0, wx.ALIGN_CENTER_VERTICAL, 0)
-        barcheck1_sizer.Add(self.check_suppress, 1, wx.ALIGN_CENTER_VERTICAL, 0)
-
-        baroptions_sizer.Add(bartype_sizer, 0, wx.EXPAND, 0)
-        baroptions_sizer.Add(bardimx_sizer, 0, wx.EXPAND, 0)
-        baroptions_sizer.Add(bardimy_sizer, 0, wx.EXPAND, 0)
-        baroptions_sizer.Add(barcheck1_sizer, 0, wx.EXPAND, 0)
-
-        qr_sizer.Add(self.option_qr, 0, wx.EXPAND, 1)
-        qr_sizer.Add(qrnotebook, 1, wx.EXPAND, 0)
-        bar_sizer.Add(self.option_bar, 0, wx.EXPAND, 1)
-        bar_sizer.Add(baroptions_sizer, 1, wx.EXPAND, 0)
-
-        codes_sizer.Add(qr_sizer, 1, wx.EXPAND, 0)
-        codes_sizer.Add(bar_sizer, 1, wx.EXPAND, 0)
-        sizer_buttons = wx.StdDialogButtonSizer()
-
-        self.button_OK = wx.Button(self, wx.ID_OK, "")
-        self.button_OK.SetToolTip(_("Create a barcode/qrcode"))
-        self.button_OK.SetDefault()
-        sizer_buttons.AddButton(self.button_OK)
-
-        self.button_CANCEL = wx.Button(self, wx.ID_CANCEL, "")
-        self.button_CANCEL.SetToolTip(_("Close without creating anything"))
-        sizer_buttons.AddButton(self.button_CANCEL)
-
-        sizer_buttons.Realize()
-        mainsizer.Add(input_sizer, 0, wx.EXPAND, 0)
-        mainsizer.Add(xy_sizer, 0, wx.EXPAND, 0)
-        mainsizer.Add(codes_sizer, 0, wx.EXPAND, 0)
-        mainsizer.Add(sizer_buttons, 0, wx.ALIGN_RIGHT | wx.ALL, 4)
-
-        self.SetSizer(mainsizer)
-        mainsizer.Fit(self)
-        self.Bind(wx.EVT_TEXT, self.enable_buttons, self.text_xpos)
-        self.Bind(wx.EVT_TEXT, self.enable_buttons, self.text_ypos)
-        self.Bind(wx.EVT_TEXT, self.enable_buttons, self.text_code)
-
-        self.Bind(wx.EVT_TEXT, self.enable_buttons, self.text_qrdim)
-        # self.Bind(wx.EVT_TEXT, self.enable_buttons, self.text_qrborder)
-        self.Bind(wx.EVT_TEXT, self.enable_buttons, self.text_qrbox)
-        self.Bind(wx.EVT_TEXT, self.enable_buttons, self.text_qrres)
-
-        self.Bind(wx.EVT_TEXT, self.enable_buttons, self.text_bardimx)
-        self.Bind(wx.EVT_TEXT, self.enable_buttons, self.text_bardimy)
-
-        self.Bind(wx.EVT_RADIOBUTTON, self.enable_controls, self.option_bar)
-        self.Bind(wx.EVT_RADIOBUTTON, self.enable_controls, self.option_qr)
-
-        self.Bind(wx.EVT_BUTTON, self.on_okay, self.button_OK)
-        # Force disable/enable of elements
-        self.option_qr.SetValue(True)
-        self.enable_buttons(None)
-        self.enable_controls(None)
-
-    def enable_controls(self, event):
-        qr = self.option_qr.GetValue()
-        bar = not qr
-
-        self.text_qrdim.Enable(qr)
-        # self.text_qrborder.Enable(qr)
-        self.text_qrbox.Enable(qr)
-        self.text_qrres.Enable(qr)
-        self.combo_errcorr.Enable(qr)
-
-        self.combo_barcode.Enable(bar)
-        self.text_bardimx.Enable(bar)
-        self.text_bardimy.Enable(bar)
-        self.check_suppress.Enable(bar)
-
-    def enable_buttons(self, event):
-        active = True
-        if len(self.text_code.GetValue()) == 0:
-            active = False
-        try:
-            if len(self.text_xpos.GetValue()) == 0:
-                active = False
-            else:
-                __ = self.context.elements.length_x(self.text_xpos.GetValue())
-        except ValueError:
-            active = False
-        try:
-            if len(self.text_ypos.GetValue()) == 0:
-                active = False
-            else:
-                __ = self.context.elements.length_y(self.text_ypos.GetValue())
-        except ValueError:
-            active = False
-        if self.option_qr.GetValue():
-            try:
-                __ = self.context.elements.length(self.text_qrdim.GetValue())
-                __ = int(self.text_qrbox.GetValue())
-                # __ = int(self.text_qrborder.GetValue())
-                __ = int(self.text_qrres.GetValue())
-            except ValueError:
-                active = False
-        else:
-            # Barcode
-            try:
-                if self.text_bardimx.GetValue() != "auto":
-                    __ = self.context.elements.length_x(self.text_bardimx.GetValue())
-                if self.text_bardimy.GetValue() != "auto":
-                    __ = self.context.elements.length_y(self.text_bardimy.GetValue())
-            except ValueError:
-                active = False
-
-        self.button_OK.Enable(active)
-
-    def on_okay(self, event):
-        result = ""
-        code = self.text_code.GetValue()
-        xpos = self.text_xpos.GetValue()
-        ypos = self.text_ypos.GetValue()
-        if self.option_qr.GetValue():
-            dim = self.text_qrdim.GetValue()
-            # border = self.text_qrborder.GetValue()
-            box = self.text_qrbox.GetValue()
-            res = self.text_qrres.GetValue()
-            ecval = self.combo_errcorr.GetSelection()
-            corrcode = ("M", "L", "Q", "H")
-            errc = corrcode[ecval]
-            result = f'qrcode {xpos} {ypos} {dim} "{code}" '
-            result += f"--boxsize {box} --version {res} --errcorr {errc}"
-            # result += f" --border {border}"
-        else:
-            # Barcode
-            dimx = self.text_bardimx.GetValue()
-            dimy = self.text_bardimy.GetValue()
-            btype = PROVIDED_BARCODES[self.combo_barcode.GetSelection()]
-            if self.check_suppress.GetValue():
-                suppress = " --notext"
-            else:
-                suppress = ""
-            result = f'barcode {xpos} {ypos} {dimx} {dimy} {btype} "{code}"'
-            result += f"{suppress}"
-        self.command = result
-        event.Skip()
-
-    def on_wifi(self, event):
-        hidden = bool(self.check_hidden.GetValue())  # False, True, None
-        ssid = self.text_wifi_ssid.GetValue()
-        password = self.text_wifi_password.GetValue()
-        security = max(0, self.combo_wifi_wpa.GetSelection())
-        # 0=WPA, 1=WEP, 2 = None
-        result = "WIFI:"
-        if ssid:
-            result += f"S:{ssid};"
-        if password:
-            result += f"P:{password};"
-        if security == 0:
-            result += "T:WPA;"
-        if security == 1:
-            result += "T:WEP;"
-        if hidden is None:
-            result += ";"
-        elif hidden:
-            result += "H:TRUE;"
-        else:
-            result += "H:FALSE;"
-        while not result.endswith(";;"):
-            result += ";"
-        self.option_qr.SetValue(True)
-        self.text_code.SetValue(result)
-
-    def on_vcard(self, event):
-        """
-        Tag	i-mode compatible bar code recognition function	Description	Example
-        ADR	        The physical delivery address. The fields divided by commas (,) denote
-                    PO box, room number, house number, city, prefecture, zip code and country, in order.
-                    ADR:,,123 Main St.,Springfield,IL,12345,USA;
-        BDAY	    8 digits for date of birth: year (4 digits), month (2 digits) and day (2 digits), in order.
-                    BDAY:19700310;
-        EMAIL	    The address for electronic mail communication.
-                    EMAIL:johndoe@hotmail.com;
-        N	        A structured representation of the name of the person. When a field is divided
-                    by a comma (,), the first half is treated as the last name and the second half
-                    is treated as the first name.
-                    N:Doe,John;
-        NICKNAME    Familiar name for the object represented by this MeCard.
-                    NICKNAME:Johnny;
-        NOTE	    Specifies supplemental information to be set as memo in the phonebook.
-                    NOTE:I am proficient in Tiger-Crane Style,\nand I am more than proficient in the exquisite art of the Samurai sword.;
-        SOUND	    Designates a text string to be set as the kana name in the phonebook.
-                    When a field is divided by a comma (,), the first half is treated as the last name
-                    and the second half is treated as the first name.
-        TEL	        The canonical number string for a telephone number for telephony communication.
-                    TEL:(123) 555-5832;
-        TEL-AV	    The canonical string for a videophone number communication.
-                    TEL-AV:(123) 555-5832;
-        URL	        A URL pointing to a website that represents the person in some way.
-                    URL:https://www.johndoe.com/;
-        """
-        result = "MECARD:"
-        vcardname = self.text_vcard_name.GetValue().strip()
-        vcardtel = self.text_vcard_tel.GetValue().strip()
-        vcardadr = self.text_vcard_address.GetValue().strip()
-        vcardemail = self.text_vcard_email.GetValue().strip()
-        vcardurl = self.text_vcard_url.GetValue().strip()
-        if vcardname != "":
-            result += f"N:{vcardname};"
-        if vcardadr != "":
-            result += f"ADR:{vcardadr};"
-        if vcardemail != "":
-            result += f"EMAIL:{vcardemail};"
-        if vcardtel != "":
-            result += f"TEL:{vcardtel};"
-        if vcardurl != "":
-            result += f"URL:{vcardurl};"
-
-        while not result.endswith(";;"):
-            result += ";"
-        self.text_code.SetValue(result)
-        self.option_qr.SetValue(True)
-
-
-class QRCodePropertyPanel(wx.Panel):
-    """
-    Panel for post-creation qrcode text editing
-    """
-
-    def __init__(
-        self,
-        *args,
-        context=None,
-        node=None,
-        **kwds,
-    ):
-        # begin wxGlade: LayerSettingPanel.__init__
-        kwds["style"] = kwds.get("style", 0)
-        wx.Panel.__init__(self, *args, **kwds)
-        self.context = context
-        self.node = node
-
-        main_sizer = wx.StaticBoxSizer(
-            wx.StaticBox(self, wx.ID_ANY, _("Text to use for QR-Code:")), wx.HORIZONTAL
-        )
-        self.text_text = wx.TextCtrl(self, wx.ID_ANY, "")
-        main_sizer.Add(self.text_text, 1, wx.EXPAND, 0)
-
-        self.SetSizer(main_sizer)
-        self.Layout()
-        self.text_text.Bind(wx.EVT_TEXT, self.on_text_change)
-        self.set_widgets(self.node)
-
-    def pane_hide(self):
-        pass
-
-    def pane_show(self):
-        pass
-
-    def accepts(self, node):
-        if (
-            hasattr(node, "mktext")
-            and hasattr(node, "mkbarcode")
-            and getattr(node, "mkbarcode") == "qr"
-        ):
-            return True
-        else:
-            return False
-
-    def set_widgets(self, node):
-        self.node = node
-        # print(f"set_widget for {self.attribute} to {str(node)}")
-        if self.node is None or not self.accepts(node):
-            self.Hide()
-            return
-        self.text_text.SetValue(str(node.mktext))
-        self.Show()
-
-    def update_node(self):
-        vtext = self.text_text.GetValue()
-        if self.node.mktext == vtext:
-            return
-        update_qr(self.context, self.node, vtext)
-        self.context.signal("element_property_reload", self.node)
-        self.context.signal("refresh_scene", "Scene")
-
-    def on_text_change(self, event):
-        self.update_node()
-
-
-class EANCodePropertyPanel(wx.Panel):
-    """
-    Panel for post-creation eancode text editing
-    """
-
-    def __init__(
-        self,
-        *args,
-        context=None,
-        node=None,
-        **kwds,
-    ):
-        # begin wxGlade: LayerSettingPanel.__init__
-        kwds["style"] = kwds.get("style", 0)
-        wx.Panel.__init__(self, *args, **kwds)
-        self.context = context
-        self.node = node
-
-        main_sizer = wx.StaticBoxSizer(
-            wx.StaticBox(self, wx.ID_ANY, _("Text to use for Barcode:")), wx.HORIZONTAL
-        )
-        self.text_text = wx.TextCtrl(self, wx.ID_ANY, "")
-        main_sizer.Add(self.text_text, 1, wx.EXPAND, 0)
-
-        self.SetSizer(main_sizer)
-        self.Layout()
-        self.text_text.Bind(wx.EVT_TEXT, self.on_text_change)
-        self.set_widgets(self.node)
-
-    def pane_hide(self):
-        pass
-
-    def pane_show(self):
-        pass
-
-    def accepts(self, node):
-        if (
-            hasattr(node, "mktext")
-            and hasattr(node, "mkbarcode")
-            and getattr(node, "mkbarcode") == "ean"
-        ):
-            return True
-        else:
-            return False
-
-    def set_widgets(self, node):
-        self.node = node
-        # print(f"set_widget for {self.attribute} to {str(node)}")
-        if self.node is None or not self.accepts(node):
-            self.Hide()
-            return
-        self.text_text.SetValue(str(node.mktext))
-        self.Show()
-
-    def update_node(self):
-        vtext = self.text_text.GetValue()
-        if self.node.mktext == vtext:
-            return
-        self.node.mktext = vtext
-        update_barcode(self.context, self.node, vtext)
-        self.context.signal("element_property_reload", self.node)
-        self.context.signal("refresh_scene", "Scene")
-
-    def on_text_change(self, event):
-        self.update_node()
+import wx
+from barcode import PROVIDED_BARCODES
+
+from .bcode_logic import update_barcode, update_qr
+
+_ = wx.GetTranslation
+
+
+class BarcodeDialog(wx.Dialog):
+
+    # from meerk40t.gui.wxutils import TextCtrl
+
+    def __init__(self, context, *args, **kwds):
+        self.context = context
+        _ = context._
+        self.command = ""
+        # begin wxGlade: RefAlign.__init__
+        kwds["style"] = kwds.get("style", 0) | wx.DEFAULT_DIALOG_STYLE
+        wx.Dialog.__init__(self, *args, **kwds)
+        self.SetTitle(_("Create a barcode"))
+        mainsizer = wx.BoxSizer(wx.VERTICAL)
+
+        input_sizer = wx.StaticBoxSizer(
+            wx.StaticBox(self, wx.ID_ANY, _("Text to use:")), wx.HORIZONTAL
+        )
+        self.text_code = wx.TextCtrl(self, wx.ID_ANY)
+        self.text_code.SetToolTip(
+            _("The barcode/qrcode will be based on this content.")
+        )
+        label = wx.StaticText(self, wx.ID_ANY, label=_("Code:"))
+        input_sizer.Add(label, 0, wx.ALIGN_CENTER_VERTICAL, 0)
+        input_sizer.Add(self.text_code, 1, wx.EXPAND, 0)
+
+        xy_sizer = wx.StaticBoxSizer(
+            wx.StaticBox(self, wx.ID_ANY, _("Coordinates:")), wx.HORIZONTAL
+        )
+        x_sizer = wx.StaticBoxSizer(
+            wx.StaticBox(self, wx.ID_ANY, _("X:")), wx.HORIZONTAL
+        )
+        y_sizer = wx.StaticBoxSizer(
+            wx.StaticBox(self, wx.ID_ANY, _("Y:")), wx.HORIZONTAL
+        )
+        self.text_xpos = wx.TextCtrl(self, wx.ID_ANY, "0cm")
+        self.text_xpos.SetToolTip(
+            _("Where will the barcode will be located (top left corner).")
+        )
+        self.text_xpos.SetMaxSize(wx.Size(100, -1))
+
+        x_sizer.Add(self.text_xpos, 1, wx.EXPAND, 0)
+
+        self.text_ypos = wx.TextCtrl(self, wx.ID_ANY, "0cm")
+        self.text_ypos.SetToolTip(
+            _("Where will the barcode will be located (top left corner).")
+        )
+        self.text_ypos.SetMaxSize(wx.Size(100, -1))
+
+        y_sizer.Add(self.text_ypos, 1, wx.EXPAND, 0)
+        xy_sizer.Add(x_sizer, 1, wx.EXPAND, 0)
+        xy_sizer.Add(y_sizer, 1, wx.EXPAND, 0)
+
+        self.option_qr = wx.RadioButton(self, wx.ID_ANY, _("QR-Code"))
+        self.option_bar = wx.RadioButton(self, wx.ID_ANY, _("Barcode"))
+
+        codes_sizer = wx.BoxSizer(wx.HORIZONTAL)
+        qr_sizer = wx.StaticBoxSizer(
+            wx.StaticBox(self, wx.ID_ANY, _("QR-Code:")), wx.VERTICAL
+        )
+        qrnotebook = wx.Notebook(self, wx.ID_ANY)
+
+        # --------------- Option Panel
+
+        qrmain_panel = wx.Panel(qrnotebook, wx.ID_ANY)
+        qrnotebook.AddPage(qrmain_panel, _("Options"))
+        qroptions_sizer = wx.BoxSizer(wx.VERTICAL)
+        qrmain_panel.SetSizer(qroptions_sizer)
+        qrdim_sizer = wx.BoxSizer(wx.HORIZONTAL)
+        #      --boxsize  (-x)      Boxsize (default 10)
+        #  --border   (-b)      Border around qr-code (default 4)
+        #  --version  (-v)      size (1..40)
+        #  --errcorr  (-e)      error correction, one of L (7%), M (15%), Q (25%), H (30%)
+        label = wx.StaticText(qrmain_panel, wx.ID_ANY, label=_("Width/Height:"))
+        label.SetMinSize(wx.Size(80, -1))
+        self.text_qrdim = wx.TextCtrl(qrmain_panel, wx.ID_ANY, "4cm")
+        self.text_qrdim.SetToolTip(_("How wide/high will the resulting qr-code be?"))
+        self.text_qrdim.SetMaxSize(wx.Size(100, -1))
+        qrdim_sizer.Add(label, 0, wx.ALIGN_CENTER_VERTICAL, 0)
+        qrdim_sizer.Add(self.text_qrdim, 1, wx.EXPAND, 0)
+
+        qrres_sizer = wx.BoxSizer(wx.HORIZONTAL)
+        label = wx.StaticText(qrmain_panel, wx.ID_ANY, label=_("Resolution:"))
+        label.SetMinSize(wx.Size(80, -1))
+        self.text_qrres = wx.TextCtrl(qrmain_panel, wx.ID_ANY, value="1")
+        self.text_qrres.SetToolTip(
+            _("How big will the qr-code become (1..40, default 1)?")
+        )
+        self.text_qrres.SetMaxSize(wx.Size(50, -1))
+        qrres_sizer.Add(label, 0, wx.ALIGN_CENTER_VERTICAL, 0)
+        qrres_sizer.Add(self.text_qrres, 1, wx.EXPAND, 0)
+
+        # qrborder_sizer = wx.BoxSizer(wx.HORIZONTAL)
+        # label = wx.StaticText(self, wx.ID_ANY, label=_("Border:"))
+        # label.SetMinSize(wx.Size(80, -1))
+        # self.text_qrborder = wx.TextCtrl(self, wx.ID_ANY, value="4")
+        # self.text_qrborder.SetToolTip(_("How wide is the border around the qr-code (default 4)?"))
+        # self.text_qrborder.SetMaxSize(wx.Size(50, -1))
+        # qrborder_sizer.Add(label, 0, wx.ALIGN_CENTER_VERTICAL, 0)
+        # qrborder_sizer.Add(self.text_qrborder, 1, wx.EXPAND, 0)
+
+        qrbox_sizer = wx.BoxSizer(wx.HORIZONTAL)
+        label = wx.StaticText(qrmain_panel, wx.ID_ANY, label=_("Boxsize:"))
+        label.SetMinSize(wx.Size(80, -1))
+        self.text_qrbox = wx.TextCtrl(qrmain_panel, wx.ID_ANY, value="10")
+        self.text_qrbox.SetToolTip(
+            _("How big is the boxsize of the pixels (default 10)?")
+        )
+        self.text_qrbox.SetMaxSize(wx.Size(50, -1))
+        qrbox_sizer.Add(label, 0, wx.ALIGN_CENTER_VERTICAL, 0)
+        qrbox_sizer.Add(self.text_qrbox, 1, wx.EXPAND, 0)
+
+        qrerrcorr_sizer = wx.BoxSizer(wx.HORIZONTAL)
+        label = wx.StaticText(qrmain_panel, wx.ID_ANY, label=_("Error:"))
+        label.SetMinSize(wx.Size(80, -1))
+        errchoices = ["L (7%)", "M (15%)", "Q (25%)", "H (30%)"]
+        self.combo_errcorr = wx.ComboBox(
+            qrmain_panel,
+            wx.ID_ANY,
+            choices=errchoices,
+            style=wx.CB_DROPDOWN | wx.CB_READONLY,
+        )
+        self.combo_errcorr.SetToolTip(
+            _("Establish the error correction used for the QR Code")
+        )
+        self.combo_errcorr.SetSelection(1)  # (M)
+        qrerrcorr_sizer.Add(label, 0, wx.ALIGN_CENTER_VERTICAL, 0)
+        qrerrcorr_sizer.Add(self.combo_errcorr, 1, wx.EXPAND, 0)
+
+        qroptions_sizer.Add(qrdim_sizer, 0, wx.EXPAND, 0)
+        qroptions_sizer.Add(qrres_sizer, 0, wx.EXPAND, 0)
+        # qroptions_sizer.Add(qrborder_sizer, 0, wx.EXPAND, 0)
+        qroptions_sizer.Add(qrbox_sizer, 0, wx.EXPAND, 0)
+        qroptions_sizer.Add(qrerrcorr_sizer, 0, wx.EXPAND, 0)
+
+        # --------------- WIFI PANEL
+
+        qrwifi_panel = wx.Panel(qrnotebook, wx.ID_ANY)
+        qrnotebook.AddPage(qrwifi_panel, _("WiFi"))
+        qrwifi_sizer = wx.BoxSizer(wx.VERTICAL)
+        qrwifi_panel.SetSizer(qrwifi_sizer)
+        qrwifi_ssid_sizer = wx.BoxSizer(wx.HORIZONTAL)
+        self.text_wifi_ssid = wx.TextCtrl(qrwifi_panel, wx.ID_ANY)
+        ssid_label = wx.StaticText(qrwifi_panel, wx.ID_ANY, _("SSID:"))
+        ssid_label.SetMinSize(wx.Size(45, -1))
+        qrwifi_ssid_sizer.Add(ssid_label, 0, wx.ALIGN_CENTER_VERTICAL, 0)
+        qrwifi_ssid_sizer.Add(self.text_wifi_ssid, 1, wx.EXPAND, 0)
+
+        qrwifi_passwd_sizer = wx.BoxSizer(wx.HORIZONTAL)
+
+        self.text_wifi_password = wx.TextCtrl(qrwifi_panel, wx.ID_ANY)
+        pass_label = wx.StaticText(qrwifi_panel, wx.ID_ANY, _("Key:"))
+        pass_label.SetMinSize(wx.Size(45, -1))
+        qrwifi_passwd_sizer.Add(pass_label, 0, wx.ALIGN_CENTER_VERTICAL, 0)
+        qrwifi_passwd_sizer.Add(self.text_wifi_password, 1, wx.EXPAND, 0)
+
+        qrwifi_wpa_sizer = wx.BoxSizer(wx.HORIZONTAL)
+        self.combo_wifi_wpa = wx.ComboBox(
+            qrwifi_panel,
+            wx.ID_ANY,
+            choices=(_("WPA/WPA2/WPA3"), _("WEP"), _("None")),
+            style=wx.CB_DROPDOWN | wx.CB_READONLY,
+        )
+        self.combo_wifi_wpa.SetToolTip(
+            _("What kind of encryption does the network use?")
+        )
+        self.combo_wifi_wpa.SetSelection(0)  # WPA
+        wpa_label = wx.StaticText(qrwifi_panel, wx.ID_ANY, _("Encryption:"))
+        qrwifi_wpa_sizer.Add(wpa_label, 0, wx.ALIGN_CENTER_VERTICAL, 0)
+        qrwifi_wpa_sizer.Add(self.combo_wifi_wpa, 0, wx.EXPAND, 0)
+
+        qrwifi_hidden_sizer = wx.BoxSizer(wx.HORIZONTAL)
+
+        self.check_hidden = wx.CheckBox(qrwifi_panel, wx.ID_ANY, _("Hidden"))
+        self.check_hidden.SetToolTip(_("Is the network hidden?"))
+        self.check_hidden.SetValue(False)
+        qrwifi_hidden_sizer.Add(self.check_hidden, 0, wx.ALIGN_CENTER_VERTICAL, 0)
+
+        qrwifi_sizer.Add(qrwifi_ssid_sizer, 0, wx.EXPAND, 0)
+        qrwifi_sizer.Add(qrwifi_passwd_sizer, 0, wx.EXPAND, 0)
+        qrwifi_sizer.Add(qrwifi_wpa_sizer, 0, wx.EXPAND, 0)
+        qrwifi_sizer.Add(qrwifi_hidden_sizer, 0, wx.EXPAND, 0)
+        self.button_wifi = wx.Button(qrwifi_panel, wx.ID_ANY, _("Generate Pattern"))
+        qrwifi_sizer.Add(self.button_wifi, 0, 0, 0)
+        self.button_wifi.Bind(wx.EVT_BUTTON, self.on_wifi)
+
+        # --------------- WIFI PANEL
+
+        qrvcard_panel = wx.Panel(qrnotebook, wx.ID_ANY)
+        qrnotebook.AddPage(qrvcard_panel, _("VCard"))
+        qrvcard_sizer = wx.BoxSizer(wx.VERTICAL)
+        qrvcard_panel.SetSizer(qrvcard_sizer)
+        qrvcard_name = wx.BoxSizer(wx.HORIZONTAL)
+        self.text_vcard_name = wx.TextCtrl(qrvcard_panel, wx.ID_ANY)
+        self.text_vcard_name.SetToolTip(_("Provide your name as lastname,firstname"))
+        vcard_name_label = wx.StaticText(qrvcard_panel, wx.ID_ANY, _("Name:"))
+        vcard_name_label.SetMinSize(wx.Size(45, -1))
+        qrvcard_name.Add(vcard_name_label, 0, wx.ALIGN_CENTER_VERTICAL, 0)
+        qrvcard_name.Add(self.text_vcard_name, 1, wx.EXPAND, 0)
+
+        qrvcard_address = wx.BoxSizer(wx.HORIZONTAL)
+        self.text_vcard_address = wx.TextCtrl(qrvcard_panel, wx.ID_ANY)
+        self.text_vcard_address.SetToolTip(
+            _(
+                "Provide your address as:\n"
+                + "PO box, room number, house number, city, prefecture, zip code and country"
+            )
+        )
+        vcard_address_label = wx.StaticText(qrvcard_panel, wx.ID_ANY, _("Address:"))
+        vcard_address_label.SetMinSize(wx.Size(45, -1))
+        qrvcard_address.Add(vcard_address_label, 0, wx.ALIGN_CENTER_VERTICAL, 0)
+        qrvcard_address.Add(self.text_vcard_address, 1, wx.EXPAND, 0)
+
+        qrvcard_tel = wx.BoxSizer(wx.HORIZONTAL)
+        self.text_vcard_tel = wx.TextCtrl(qrvcard_panel, wx.ID_ANY)
+        self.text_vcard_tel.SetToolTip(_("Provide your phone-number"))
+        vcard_tel_label = wx.StaticText(qrvcard_panel, wx.ID_ANY, _("Phone:"))
+        vcard_tel_label.SetMinSize(wx.Size(45, -1))
+        qrvcard_tel.Add(vcard_tel_label, 0, wx.ALIGN_CENTER_VERTICAL, 0)
+        qrvcard_tel.Add(self.text_vcard_tel, 1, wx.EXPAND, 0)
+
+        qrvcard_email = wx.BoxSizer(wx.HORIZONTAL)
+        self.text_vcard_email = wx.TextCtrl(qrvcard_panel, wx.ID_ANY)
+        self.text_vcard_email.SetToolTip(_("Provide your email-Address"))
+        vcard_email_label = wx.StaticText(qrvcard_panel, wx.ID_ANY, _("email:"))
+        vcard_email_label.SetMinSize(wx.Size(45, -1))
+        qrvcard_email.Add(vcard_email_label, 0, wx.ALIGN_CENTER_VERTICAL, 0)
+        qrvcard_email.Add(self.text_vcard_email, 1, wx.EXPAND, 0)
+
+        qrvcard_url = wx.BoxSizer(wx.HORIZONTAL)
+        self.text_vcard_url = wx.TextCtrl(qrvcard_panel, wx.ID_ANY)
+        self.text_vcard_url.SetToolTip(_("Provide a valid URL"))
+        vcard_url_label = wx.StaticText(qrvcard_panel, wx.ID_ANY, _("URL:"))
+        vcard_url_label.SetMinSize(wx.Size(45, -1))
+        qrvcard_url.Add(vcard_url_label, 0, wx.ALIGN_CENTER_VERTICAL, 0)
+        qrvcard_url.Add(self.text_vcard_url, 1, wx.EXPAND, 0)
+
+        qrvcard_sizer.Add(qrvcard_name, 0, wx.EXPAND, 0)
+        qrvcard_sizer.Add(qrvcard_address, 0, wx.EXPAND, 0)
+        qrvcard_sizer.Add(qrvcard_tel, 0, wx.EXPAND, 0)
+        qrvcard_sizer.Add(qrvcard_email, 0, wx.EXPAND, 0)
+        qrvcard_sizer.Add(qrvcard_url, 0, wx.EXPAND, 0)
+        self.button_vcard = wx.Button(qrvcard_panel, wx.ID_ANY, _("Generate Pattern"))
+        qrvcard_sizer.Add(self.button_vcard, 0, 0, 0)
+        self.button_vcard.Bind(wx.EVT_BUTTON, self.on_vcard)
+
+        # --------------- Barcode Section
+
+        bar_sizer = wx.StaticBoxSizer(
+            wx.StaticBox(self, wx.ID_ANY, _("Barcode:")), wx.VERTICAL
+        )
+        baroptions_sizer = wx.StaticBoxSizer(
+            wx.StaticBox(self, wx.ID_ANY, _("Options:")), wx.VERTICAL
+        )
+
+        bartype_sizer = wx.BoxSizer(wx.HORIZONTAL)
+        label = wx.StaticText(self, wx.ID_ANY, label=_("Type:"))
+        label.SetMinSize(wx.Size(80, -1))
+        self.combo_barcode = wx.ComboBox(
+            self,
+            wx.ID_ANY,
+            choices=PROVIDED_BARCODES,
+            style=wx.CB_DROPDOWN | wx.CB_READONLY,
+        )
+        self.combo_barcode.SetToolTip(_("What kind of barcode do you want to create?"))
+        self.combo_barcode.SetSelection(4)  # ean13
+        bartype_sizer.Add(label, 0, wx.ALIGN_CENTER_VERTICAL, 0)
+        bartype_sizer.Add(self.combo_barcode, 1, wx.EXPAND, 0)
+
+        bardimx_sizer = wx.BoxSizer(wx.HORIZONTAL)
+        label = wx.StaticText(self, wx.ID_ANY, label=_("Width:"))
+        label.SetMinSize(wx.Size(80, -1))
+        self.text_bardimx = wx.TextCtrl(self, wx.ID_ANY, "auto")
+        self.text_bardimx.SetToolTip(_("How wide will the resulting barcode be?"))
+        self.text_bardimx.SetMaxSize(wx.Size(100, -1))
+        bardimx_sizer.Add(label, 0, wx.ALIGN_CENTER_VERTICAL, 0)
+        bardimx_sizer.Add(self.text_bardimx, 1, wx.EXPAND, 0)
+
+        bardimy_sizer = wx.BoxSizer(wx.HORIZONTAL)
+        label = wx.StaticText(self, wx.ID_ANY, label=_("Height:"))
+        label.SetMinSize(wx.Size(80, -1))
+        self.text_bardimy = wx.TextCtrl(self, wx.ID_ANY, "auto")
+        self.text_bardimy.SetToolTip(_("How high will the resulting barcode be?"))
+        self.text_bardimy.SetMaxSize(wx.Size(100, -1))
+        bardimy_sizer.Add(label, 0, wx.ALIGN_CENTER_VERTICAL, 0)
+        bardimy_sizer.Add(self.text_bardimy, 1, wx.EXPAND, 0)
+
+        barcheck1_sizer = wx.BoxSizer(wx.HORIZONTAL)
+        label = wx.StaticText(self, wx.ID_ANY, label=_("No text:"))
+        label.SetMinSize(wx.Size(80, -1))
+        self.check_suppress = wx.CheckBox(self, wx.ID_ANY, "")
+        self.check_suppress.SetToolTip(_("Suppress the text under the barcode?"))
+        self.check_suppress.SetMinSize(self.text_bardimx.GetSize())
+        barcheck1_sizer.Add(label, 0, wx.ALIGN_CENTER_VERTICAL, 0)
+        barcheck1_sizer.Add(self.check_suppress, 1, wx.ALIGN_CENTER_VERTICAL, 0)
+
+        baroptions_sizer.Add(bartype_sizer, 0, wx.EXPAND, 0)
+        baroptions_sizer.Add(bardimx_sizer, 0, wx.EXPAND, 0)
+        baroptions_sizer.Add(bardimy_sizer, 0, wx.EXPAND, 0)
+        baroptions_sizer.Add(barcheck1_sizer, 0, wx.EXPAND, 0)
+
+        qr_sizer.Add(self.option_qr, 0, wx.EXPAND, 1)
+        qr_sizer.Add(qrnotebook, 1, wx.EXPAND, 0)
+        bar_sizer.Add(self.option_bar, 0, wx.EXPAND, 1)
+        bar_sizer.Add(baroptions_sizer, 1, wx.EXPAND, 0)
+
+        codes_sizer.Add(qr_sizer, 1, wx.EXPAND, 0)
+        codes_sizer.Add(bar_sizer, 1, wx.EXPAND, 0)
+        sizer_buttons = wx.StdDialogButtonSizer()
+
+        self.button_OK = wx.Button(self, wx.ID_OK, "")
+        self.button_OK.SetToolTip(_("Create a barcode/qrcode"))
+        self.button_OK.SetDefault()
+        sizer_buttons.AddButton(self.button_OK)
+
+        self.button_CANCEL = wx.Button(self, wx.ID_CANCEL, "")
+        self.button_CANCEL.SetToolTip(_("Close without creating anything"))
+        sizer_buttons.AddButton(self.button_CANCEL)
+
+        sizer_buttons.Realize()
+        mainsizer.Add(input_sizer, 0, wx.EXPAND, 0)
+        mainsizer.Add(xy_sizer, 0, wx.EXPAND, 0)
+        mainsizer.Add(codes_sizer, 0, wx.EXPAND, 0)
+        mainsizer.Add(sizer_buttons, 0, wx.ALIGN_RIGHT | wx.ALL, 4)
+
+        self.SetSizer(mainsizer)
+        mainsizer.Fit(self)
+        self.Bind(wx.EVT_TEXT, self.enable_buttons, self.text_xpos)
+        self.Bind(wx.EVT_TEXT, self.enable_buttons, self.text_ypos)
+        self.Bind(wx.EVT_TEXT, self.enable_buttons, self.text_code)
+
+        self.Bind(wx.EVT_TEXT, self.enable_buttons, self.text_qrdim)
+        # self.Bind(wx.EVT_TEXT, self.enable_buttons, self.text_qrborder)
+        self.Bind(wx.EVT_TEXT, self.enable_buttons, self.text_qrbox)
+        self.Bind(wx.EVT_TEXT, self.enable_buttons, self.text_qrres)
+
+        self.Bind(wx.EVT_TEXT, self.enable_buttons, self.text_bardimx)
+        self.Bind(wx.EVT_TEXT, self.enable_buttons, self.text_bardimy)
+
+        self.Bind(wx.EVT_RADIOBUTTON, self.enable_controls, self.option_bar)
+        self.Bind(wx.EVT_RADIOBUTTON, self.enable_controls, self.option_qr)
+
+        self.Bind(wx.EVT_BUTTON, self.on_okay, self.button_OK)
+        # Force disable/enable of elements
+        self.option_qr.SetValue(True)
+        self.enable_buttons(None)
+        self.enable_controls(None)
+
+    def enable_controls(self, event):
+        qr = self.option_qr.GetValue()
+        bar = not qr
+
+        self.text_qrdim.Enable(qr)
+        # self.text_qrborder.Enable(qr)
+        self.text_qrbox.Enable(qr)
+        self.text_qrres.Enable(qr)
+        self.combo_errcorr.Enable(qr)
+
+        self.combo_barcode.Enable(bar)
+        self.text_bardimx.Enable(bar)
+        self.text_bardimy.Enable(bar)
+        self.check_suppress.Enable(bar)
+
+    def enable_buttons(self, event):
+        active = True
+        if len(self.text_code.GetValue()) == 0:
+            active = False
+        try:
+            if len(self.text_xpos.GetValue()) == 0:
+                active = False
+            else:
+                __ = self.context.elements.length_x(self.text_xpos.GetValue())
+        except ValueError:
+            active = False
+        try:
+            if len(self.text_ypos.GetValue()) == 0:
+                active = False
+            else:
+                __ = self.context.elements.length_y(self.text_ypos.GetValue())
+        except ValueError:
+            active = False
+        if self.option_qr.GetValue():
+            try:
+                __ = self.context.elements.length(self.text_qrdim.GetValue())
+                __ = int(self.text_qrbox.GetValue())
+                # __ = int(self.text_qrborder.GetValue())
+                __ = int(self.text_qrres.GetValue())
+            except ValueError:
+                active = False
+        else:
+            # Barcode
+            try:
+                if self.text_bardimx.GetValue() != "auto":
+                    __ = self.context.elements.length_x(self.text_bardimx.GetValue())
+                if self.text_bardimy.GetValue() != "auto":
+                    __ = self.context.elements.length_y(self.text_bardimy.GetValue())
+            except ValueError:
+                active = False
+
+        self.button_OK.Enable(active)
+
+    def on_okay(self, event):
+        result = ""
+        code = self.text_code.GetValue()
+        xpos = self.text_xpos.GetValue()
+        ypos = self.text_ypos.GetValue()
+        if self.option_qr.GetValue():
+            dim = self.text_qrdim.GetValue()
+            # border = self.text_qrborder.GetValue()
+            box = self.text_qrbox.GetValue()
+            res = self.text_qrres.GetValue()
+            ecval = self.combo_errcorr.GetSelection()
+            corrcode = ("M", "L", "Q", "H")
+            errc = corrcode[ecval]
+            result = f'qrcode {xpos} {ypos} {dim} "{code}" '
+            result += f"--boxsize {box} --version {res} --errcorr {errc}"
+            # result += f" --border {border}"
+        else:
+            # Barcode
+            dimx = self.text_bardimx.GetValue()
+            dimy = self.text_bardimy.GetValue()
+            btype = PROVIDED_BARCODES[self.combo_barcode.GetSelection()]
+            if self.check_suppress.GetValue():
+                suppress = " --notext"
+            else:
+                suppress = ""
+            result = f'barcode {xpos} {ypos} {dimx} {dimy} {btype} "{code}"'
+            result += f"{suppress}"
+        self.command = result
+        event.Skip()
+
+    def on_wifi(self, event):
+        hidden = bool(self.check_hidden.GetValue())  # False, True, None
+        ssid = self.text_wifi_ssid.GetValue()
+        password = self.text_wifi_password.GetValue()
+        security = max(0, self.combo_wifi_wpa.GetSelection())
+        # 0=WPA, 1=WEP, 2 = None
+        result = "WIFI:"
+        if ssid:
+            result += f"S:{ssid};"
+        if password:
+            result += f"P:{password};"
+        if security == 0:
+            result += "T:WPA;"
+        if security == 1:
+            result += "T:WEP;"
+        if hidden is None:
+            result += ";"
+        elif hidden:
+            result += "H:TRUE;"
+        else:
+            result += "H:FALSE;"
+        while not result.endswith(";;"):
+            result += ";"
+        self.option_qr.SetValue(True)
+        self.text_code.SetValue(result)
+
+    def on_vcard(self, event):
+        """
+        Tag	i-mode compatible bar code recognition function	Description	Example
+        ADR	        The physical delivery address. The fields divided by commas (,) denote
+                    PO box, room number, house number, city, prefecture, zip code and country, in order.
+                    ADR:,,123 Main St.,Springfield,IL,12345,USA;
+        BDAY	    8 digits for date of birth: year (4 digits), month (2 digits) and day (2 digits), in order.
+                    BDAY:19700310;
+        EMAIL	    The address for electronic mail communication.
+                    EMAIL:johndoe@hotmail.com;
+        N	        A structured representation of the name of the person. When a field is divided
+                    by a comma (,), the first half is treated as the last name and the second half
+                    is treated as the first name.
+                    N:Doe,John;
+        NICKNAME    Familiar name for the object represented by this MeCard.
+                    NICKNAME:Johnny;
+        NOTE	    Specifies supplemental information to be set as memo in the phonebook.
+                    NOTE:I am proficient in Tiger-Crane Style,\nand I am more than proficient in the exquisite art of the Samurai sword.;
+        SOUND	    Designates a text string to be set as the kana name in the phonebook.
+                    When a field is divided by a comma (,), the first half is treated as the last name
+                    and the second half is treated as the first name.
+        TEL	        The canonical number string for a telephone number for telephony communication.
+                    TEL:(123) 555-5832;
+        TEL-AV	    The canonical string for a videophone number communication.
+                    TEL-AV:(123) 555-5832;
+        URL	        A URL pointing to a website that represents the person in some way.
+                    URL:https://www.johndoe.com/;
+        """
+        result = "MECARD:"
+        vcardname = self.text_vcard_name.GetValue().strip()
+        vcardtel = self.text_vcard_tel.GetValue().strip()
+        vcardadr = self.text_vcard_address.GetValue().strip()
+        vcardemail = self.text_vcard_email.GetValue().strip()
+        vcardurl = self.text_vcard_url.GetValue().strip()
+        if vcardname != "":
+            result += f"N:{vcardname};"
+        if vcardadr != "":
+            result += f"ADR:{vcardadr};"
+        if vcardemail != "":
+            result += f"EMAIL:{vcardemail};"
+        if vcardtel != "":
+            result += f"TEL:{vcardtel};"
+        if vcardurl != "":
+            result += f"URL:{vcardurl};"
+
+        while not result.endswith(";;"):
+            result += ";"
+        self.text_code.SetValue(result)
+        self.option_qr.SetValue(True)
+
+
+class QRCodePropertyPanel(wx.Panel):
+    """
+    Panel for post-creation qrcode text editing
+    """
+
+    def __init__(
+        self,
+        *args,
+        context=None,
+        node=None,
+        **kwds,
+    ):
+        # begin wxGlade: LayerSettingPanel.__init__
+        kwds["style"] = kwds.get("style", 0)
+        wx.Panel.__init__(self, *args, **kwds)
+        self.context = context
+        self.node = node
+
+        main_sizer = wx.StaticBoxSizer(
+            wx.StaticBox(self, wx.ID_ANY, _("Text to use for QR-Code:")), wx.HORIZONTAL
+        )
+        self.text_text = wx.TextCtrl(self, wx.ID_ANY, "")
+        main_sizer.Add(self.text_text, 1, wx.EXPAND, 0)
+
+        self.SetSizer(main_sizer)
+        self.Layout()
+        self.text_text.Bind(wx.EVT_TEXT, self.on_text_change)
+        self.set_widgets(self.node)
+
+    def pane_hide(self):
+        pass
+
+    def pane_show(self):
+        pass
+
+    def accepts(self, node):
+        if (
+            hasattr(node, "mktext")
+            and hasattr(node, "mkbarcode")
+            and getattr(node, "mkbarcode") == "qr"
+        ):
+            return True
+        else:
+            return False
+
+    def set_widgets(self, node):
+        self.node = node
+        # print(f"set_widget for {self.attribute} to {str(node)}")
+        if self.node is None or not self.accepts(node):
+            self.Hide()
+            return
+        self.text_text.SetValue(str(node.mktext))
+        self.Show()
+
+    def update_node(self):
+        vtext = self.text_text.GetValue()
+        if self.node.mktext == vtext:
+            return
+        update_qr(self.context, self.node, vtext)
+        self.context.signal("element_property_reload", self.node)
+        self.context.signal("refresh_scene", "Scene")
+
+    def on_text_change(self, event):
+        self.update_node()
+
+
+class EANCodePropertyPanel(wx.Panel):
+    """
+    Panel for post-creation eancode text editing
+    """
+
+    def __init__(
+        self,
+        *args,
+        context=None,
+        node=None,
+        **kwds,
+    ):
+        # begin wxGlade: LayerSettingPanel.__init__
+        kwds["style"] = kwds.get("style", 0)
+        wx.Panel.__init__(self, *args, **kwds)
+        self.context = context
+        self.node = node
+
+        main_sizer = wx.StaticBoxSizer(
+            wx.StaticBox(self, wx.ID_ANY, _("Text to use for Barcode:")), wx.HORIZONTAL
+        )
+        self.text_text = wx.TextCtrl(self, wx.ID_ANY, "")
+        main_sizer.Add(self.text_text, 1, wx.EXPAND, 0)
+
+        self.SetSizer(main_sizer)
+        self.Layout()
+        self.text_text.Bind(wx.EVT_TEXT, self.on_text_change)
+        self.set_widgets(self.node)
+
+    def pane_hide(self):
+        pass
+
+    def pane_show(self):
+        pass
+
+    def accepts(self, node):
+        if (
+            hasattr(node, "mktext")
+            and hasattr(node, "mkbarcode")
+            and getattr(node, "mkbarcode") == "ean"
+        ):
+            return True
+        else:
+            return False
+
+    def set_widgets(self, node):
+        self.node = node
+        # print(f"set_widget for {self.attribute} to {str(node)}")
+        if self.node is None or not self.accepts(node):
+            self.Hide()
+            return
+        self.text_text.SetValue(str(node.mktext))
+        self.Show()
+
+    def update_node(self):
+        vtext = self.text_text.GetValue()
+        if self.node.mktext == vtext:
+            return
+        self.node.mktext = vtext
+        update_barcode(self.context, self.node, vtext)
+        self.context.signal("element_property_reload", self.node)
+        self.context.signal("refresh_scene", "Scene")
+
+    def on_text_change(self, event):
+        self.update_node()
```

### Comparing `meerk40t-barcodes-0.2.0/barcodes/tools/icons.py` & `meerk40t-barcodes-0.2.1/barcodes/tools/icons.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,299 +1,299 @@
-import wx
-
-from wx.lib.embeddedimage import PyEmbeddedImage as py_embedded_image
-
-"""
-icons serves as a central repository for icons and other assets. These are all processed as PyEmbeddedImages which is
-extended from the wx.lib utility of the same name. We allow several additional modifications to these assets. For
-example we allow resizing and inverting this allows us to easily reuse the icons and to use the icons for dark themed
-guis. We permit rotation of the icons, so as to permit reusing these icons and coloring the icons to match a particular
-colored object, for example the icons in the tree for operations using color specific matching.
-"""
-
-DARKMODE = False
-
-STD_ICON_SIZE = 50
-
-_MIN_ICON_SIZE = 0
-_GLOBAL_FACTOR = 1.0
-
-
-def set_icon_appearance(factor, min_size):
-    global _MIN_ICON_SIZE
-    global _GLOBAL_FACTOR
-    _MIN_ICON_SIZE = min_size
-    _GLOBAL_FACTOR = factor
-
-
-def get_default_icon_size():
-    return int(_GLOBAL_FACTOR * STD_ICON_SIZE)
-
-
-def get_default_scale_factor():
-    return _GLOBAL_FACTOR
-
-
-class PyEmbeddedImage(py_embedded_image):
-    def __init__(self, data):
-        super().__init__(data)
-
-    def GetBitmap(
-        self,
-        use_theme=True,
-        resize=None,
-        color=None,
-        rotate=None,
-        noadjustment=False,
-        keepalpha=False,
-    ):
-        """
-        Assumes greyscale icon black on transparent background using alpha for shading
-        Ready for Dark Theme
-        If color is provided, the black is changed to this
-        If color is close to background, alpha is removed and negative background added
-        so, we don't get black icon on black background or white on white background.
-
-        @param use_theme:
-        @param resize:
-        @param color:
-        @param rotate:
-        @param noadjustment: Disables size adjustment based on global factor
-        @param keepalpha: maintain the alpha from the original asset
-        @return:
-        """
-
-        image = py_embedded_image.GetImage(self)
-        if not noadjustment and _GLOBAL_FACTOR != 1.0:
-            oldresize = resize
-            wd, ht = image.GetSize()
-            if resize is not None:
-                if isinstance(resize, int) or isinstance(resize, float):
-                    resize *= _GLOBAL_FACTOR
-                    if 0 < _MIN_ICON_SIZE < oldresize:
-                        if resize < _MIN_ICON_SIZE:
-                            resize = _MIN_ICON_SIZE
-                elif isinstance(resize, tuple):  # (tuple wd ht)
-                    resize = [oldresize[0], oldresize[1]]
-                    for i in range(2):
-                        resize[i] *= _GLOBAL_FACTOR
-                        if 0 < _MIN_ICON_SIZE < oldresize[i]:
-                            if resize[i] < _MIN_ICON_SIZE:
-                                resize[i] = _MIN_ICON_SIZE
-            else:
-                resize = [wd, ht]
-                oldresize = (wd, ht)
-                for i in range(2):
-                    resize[i] *= _GLOBAL_FACTOR
-                    if 0 < _MIN_ICON_SIZE < oldresize[i]:
-                        if resize[i] < _MIN_ICON_SIZE:
-                            resize[i] = _MIN_ICON_SIZE
-            # print ("Will adjust from %s to %s (was: %s)" % ((wd, ht), resize, oldresize))
-
-        if resize is not None:
-            if isinstance(resize, int) or isinstance(resize, float):
-                image = image.Scale(int(resize), int(resize))
-            else:
-                image = image.Scale(int(resize[0]), int(resize[1]))
-        if rotate is not None:
-            if rotate == 1:
-                image = image.Rotate90()
-            elif rotate == 2:
-                image = image.Rotate180()
-            elif rotate == 3:
-                image = image.Rotate90(False)
-        if (
-            color is not None
-            and color.red is not None
-            and color.green is not None
-            and color.blue is not None
-        ):
-            image.Replace(0, 0, 0, color.red, color.green, color.blue)
-            if DARKMODE and use_theme:
-                reverse = color.distance_to("black") <= 200
-                black_bg = False
-            else:
-                reverse = color.distance_to("white") <= 200
-                black_bg = True
-            if reverse and not keepalpha:
-                self.RemoveAlpha(image, black_bg=black_bg)
-        elif DARKMODE and use_theme:
-            image.Replace(0, 0, 0, 255, 255, 255)
-        return wx.Bitmap(image)
-
-    def RemoveAlpha(self, image, black_bg=False):
-        if not image.HasAlpha():
-            return
-        bg_rgb = 0 if black_bg else 255
-        for x in range(image.GetWidth()):
-            for y in range(image.GetHeight()):
-                a = image.GetAlpha(x, y)
-                bg = int((255 - a) * bg_rgb / 255)
-                r = int(image.GetRed(x, y) * a / 255) + bg
-                g = int(image.GetGreen(x, y) * a / 255) + bg
-                b = int(image.GetBlue(x, y) * a / 255) + bg
-                image.SetRGB(x, y, r, g, b)
-                image.SetAlpha(x, y, wx.IMAGE_ALPHA_OPAQUE)
-        image.ClearAlpha()
-
-class EmptyIcon():
-    def __init__(self, size, color, msg=None, ptsize=None, **args):
-        if size <= 0:
-            size = 50
-        size = int(size)
-        self._size = size
-        self._color = color
-        bmp = self.populate_image(msg, ptsize)
-        self._image = bmp.ConvertToImage()
-        # self._image = wx.Image(width=size, height=size, clear=True)
-        # for x in range(size):
-        #     for y in range(size):
-        #         self._image.SetRGB(x, y, color.red, color.green, color.blue)
-
-    def populate_image(self, msg=None, ptsize=None):
-        imgBit = wx.Bitmap(self._size, self._size)
-        dc = wx.MemoryDC(imgBit)
-        dc.SelectObject(imgBit)
-        brush = wx.Brush(self._color, wx.BRUSHSTYLE_SOLID)
-        dc.SetBackground(brush)
-        dc.Clear()
-        if msg is not None and msg != "":
-            # We only take the very first letter for
-            pattern={
-                "[red]": wx.RED,
-                "[green]": wx.GREEN,
-                "[blue]": wx.BLUE,
-                "[white]": wx.WHITE,
-                "[black]": wx.BLACK,
-            }
-            txt_color = wx.BLACK
-            for pat in pattern:
-                if msg.startswith(pat):
-                    txt_color = pattern[pat]
-                    msg = msg[len(pat):]
-            if ptsize is None:
-                ptsize = 12
-            font = wx.Font(
-                ptsize,
-                wx.FONTFAMILY_SWISS,
-                wx.FONTSTYLE_NORMAL,
-                wx.FONTWEIGHT_NORMAL,
-            )
-            dc.SetTextForeground(txt_color)
-            dc.SetFont(font)
-            (t_w, t_h) = dc.GetTextExtent(msg)
-            x = (self._size - t_w) / 2
-            y = (self._size - t_h) / 2
-            pt = wx.Point(x, y)
-            dc.DrawText(msg, pt)
-        # Now release dc
-        dc.SelectObject(wx.NullBitmap)
-        return imgBit
-
-    def GetBitmap(
-        self,
-        use_theme=True,
-        resize=None,
-        color=None,
-        rotate=None,
-        noadjustment=False,
-        keepalpha=False,
-    ):
-        """
-        Assumes greyscale icon black on transparent background using alpha for shading
-        Ready for Dark Theme
-        If color is provided, the black is changed to this
-        If color is close to background, alpha is removed and negative background added
-        so, we don't get black icon on black background or white on white background.
-
-        @param use_theme:
-        @param resize:
-        @param color:
-        @param rotate:
-        @param noadjustment: Disables size adjustment based on global factor
-        @param keepalpha: maintain the alpha from the original asset
-        @return:
-        """
-
-        image = self._image
-        if not noadjustment and _GLOBAL_FACTOR != 1.0:
-            oldresize = resize
-            wd, ht = image.GetSize()
-            if resize is not None:
-                if isinstance(resize, int) or isinstance(resize, float):
-                    resize *= _GLOBAL_FACTOR
-                    if 0 < _MIN_ICON_SIZE < oldresize:
-                        if resize < _MIN_ICON_SIZE:
-                            resize = _MIN_ICON_SIZE
-                elif isinstance(resize, tuple):  # (tuple wd ht)
-                    resize = [oldresize[0], oldresize[1]]
-                    for i in range(2):
-                        resize[i] *= _GLOBAL_FACTOR
-                        if 0 < _MIN_ICON_SIZE < oldresize[i]:
-                            if resize[i] < _MIN_ICON_SIZE:
-                                resize[i] = _MIN_ICON_SIZE
-            else:
-                resize = [wd, ht]
-                oldresize = (wd, ht)
-                for i in range(2):
-                    resize[i] *= _GLOBAL_FACTOR
-                    if 0 < _MIN_ICON_SIZE < oldresize[i]:
-                        if resize[i] < _MIN_ICON_SIZE:
-                            resize[i] = _MIN_ICON_SIZE
-            # print ("Will adjust from %s to %s (was: %s)" % ((wd, ht), resize, oldresize))
-
-        if resize is not None:
-            if isinstance(resize, int) or isinstance(resize, float):
-                image = image.Scale(int(resize), int(resize))
-            else:
-                image = image.Scale(int(resize[0]), int(resize[1]))
-        if rotate is not None:
-            if rotate == 1:
-                image = image.Rotate90()
-            elif rotate == 2:
-                image = image.Rotate180()
-            elif rotate == 3:
-                image = image.Rotate90(False)
-        if (
-            color is not None
-            and color.red is not None
-            and color.green is not None
-            and color.blue is not None
-        ):
-#            image.Replace(0, 0, 0, color.red, color.green, color.blue)
-            image.Replace(self._color.red, self._color.green, self._color.blue, color.red, color.green, color.blue)
-            if DARKMODE and use_theme:
-                reverse = color.distance_to("black") <= 200
-                black_bg = False
-            else:
-                reverse = color.distance_to("white") <= 200
-                black_bg = True
-            if reverse and not keepalpha:
-                self.RemoveAlpha(image, black_bg=black_bg)
-        elif DARKMODE and use_theme:
-            image.Replace(0, 0, 0, 255, 255, 255)
-        return wx.Bitmap(image)
-
-    def RemoveAlpha(self, image, black_bg=False):
-        if not image.HasAlpha():
-            return
-        bg_rgb = 0 if black_bg else 255
-        for x in range(image.GetWidth()):
-            for y in range(image.GetHeight()):
-                a = image.GetAlpha(x, y)
-                bg = int((255 - a) * bg_rgb / 255)
-                r = int(image.GetRed(x, y) * a / 255) + bg
-                g = int(image.GetGreen(x, y) * a / 255) + bg
-                b = int(image.GetBlue(x, y) * a / 255) + bg
-                image.SetRGB(x, y, r, g, b)
-                image.SetAlpha(x, y, wx.IMAGE_ALPHA_OPAQUE)
-        image.ClearAlpha()
-
-
-icons8_barcode_50 = PyEmbeddedImage(
-    b'iVBORw0KGgoAAAANSUhEUgAAADIAAAAyCAYAAAAeP4ixAAAABmJLR0QA/wD/AP+gvaeTAAAA'
-    b'4ElEQVRoge3Zuw3CMBSF4R9EzwIwAQswAgtkAjaABVgAqNLBBmnooKOkShcWSJmKCaBxkGXZ'
-    b'RkIUF+l8kmX5+nlqg4iIyPcGkdoOmHrjLXADlsAic1YDbIAJsA/mCtcfgHFkb+qOM3AE5sDa'
-    b'q7fAKvOW94OeXusfUQb1sF3dullkrtcl9qbuKF29COpN+Ojhp1T/QkGsURBrFMQaBbFGQaxR'
-    b'EGsUxBoFsUZBrFEQaxTEGgWxRkGsURBrFMSaUaR2Ae7euHV9DVSZs/o/i0dm3Yn4R0/qjtqb'
-    b'ryLrRUREfuIFnSA3JAyP8hcAAAAASUVORK5CYII=')
-
+import wx
+
+from wx.lib.embeddedimage import PyEmbeddedImage as py_embedded_image
+
+"""
+icons serves as a central repository for icons and other assets. These are all processed as PyEmbeddedImages which is
+extended from the wx.lib utility of the same name. We allow several additional modifications to these assets. For
+example we allow resizing and inverting this allows us to easily reuse the icons and to use the icons for dark themed
+guis. We permit rotation of the icons, so as to permit reusing these icons and coloring the icons to match a particular
+colored object, for example the icons in the tree for operations using color specific matching.
+"""
+
+DARKMODE = False
+
+STD_ICON_SIZE = 50
+
+_MIN_ICON_SIZE = 0
+_GLOBAL_FACTOR = 1.0
+
+
+def set_icon_appearance(factor, min_size):
+    global _MIN_ICON_SIZE
+    global _GLOBAL_FACTOR
+    _MIN_ICON_SIZE = min_size
+    _GLOBAL_FACTOR = factor
+
+
+def get_default_icon_size():
+    return int(_GLOBAL_FACTOR * STD_ICON_SIZE)
+
+
+def get_default_scale_factor():
+    return _GLOBAL_FACTOR
+
+
+class PyEmbeddedImage(py_embedded_image):
+    def __init__(self, data):
+        super().__init__(data)
+
+    def GetBitmap(
+        self,
+        use_theme=True,
+        resize=None,
+        color=None,
+        rotate=None,
+        noadjustment=False,
+        keepalpha=False,
+    ):
+        """
+        Assumes greyscale icon black on transparent background using alpha for shading
+        Ready for Dark Theme
+        If color is provided, the black is changed to this
+        If color is close to background, alpha is removed and negative background added
+        so, we don't get black icon on black background or white on white background.
+
+        @param use_theme:
+        @param resize:
+        @param color:
+        @param rotate:
+        @param noadjustment: Disables size adjustment based on global factor
+        @param keepalpha: maintain the alpha from the original asset
+        @return:
+        """
+
+        image = py_embedded_image.GetImage(self)
+        if not noadjustment and _GLOBAL_FACTOR != 1.0:
+            oldresize = resize
+            wd, ht = image.GetSize()
+            if resize is not None:
+                if isinstance(resize, int) or isinstance(resize, float):
+                    resize *= _GLOBAL_FACTOR
+                    if 0 < _MIN_ICON_SIZE < oldresize:
+                        if resize < _MIN_ICON_SIZE:
+                            resize = _MIN_ICON_SIZE
+                elif isinstance(resize, tuple):  # (tuple wd ht)
+                    resize = [oldresize[0], oldresize[1]]
+                    for i in range(2):
+                        resize[i] *= _GLOBAL_FACTOR
+                        if 0 < _MIN_ICON_SIZE < oldresize[i]:
+                            if resize[i] < _MIN_ICON_SIZE:
+                                resize[i] = _MIN_ICON_SIZE
+            else:
+                resize = [wd, ht]
+                oldresize = (wd, ht)
+                for i in range(2):
+                    resize[i] *= _GLOBAL_FACTOR
+                    if 0 < _MIN_ICON_SIZE < oldresize[i]:
+                        if resize[i] < _MIN_ICON_SIZE:
+                            resize[i] = _MIN_ICON_SIZE
+            # print ("Will adjust from %s to %s (was: %s)" % ((wd, ht), resize, oldresize))
+
+        if resize is not None:
+            if isinstance(resize, int) or isinstance(resize, float):
+                image = image.Scale(int(resize), int(resize))
+            else:
+                image = image.Scale(int(resize[0]), int(resize[1]))
+        if rotate is not None:
+            if rotate == 1:
+                image = image.Rotate90()
+            elif rotate == 2:
+                image = image.Rotate180()
+            elif rotate == 3:
+                image = image.Rotate90(False)
+        if (
+            color is not None
+            and color.red is not None
+            and color.green is not None
+            and color.blue is not None
+        ):
+            image.Replace(0, 0, 0, color.red, color.green, color.blue)
+            if DARKMODE and use_theme:
+                reverse = color.distance_to("black") <= 200
+                black_bg = False
+            else:
+                reverse = color.distance_to("white") <= 200
+                black_bg = True
+            if reverse and not keepalpha:
+                self.RemoveAlpha(image, black_bg=black_bg)
+        elif DARKMODE and use_theme:
+            image.Replace(0, 0, 0, 255, 255, 255)
+        return wx.Bitmap(image)
+
+    def RemoveAlpha(self, image, black_bg=False):
+        if not image.HasAlpha():
+            return
+        bg_rgb = 0 if black_bg else 255
+        for x in range(image.GetWidth()):
+            for y in range(image.GetHeight()):
+                a = image.GetAlpha(x, y)
+                bg = int((255 - a) * bg_rgb / 255)
+                r = int(image.GetRed(x, y) * a / 255) + bg
+                g = int(image.GetGreen(x, y) * a / 255) + bg
+                b = int(image.GetBlue(x, y) * a / 255) + bg
+                image.SetRGB(x, y, r, g, b)
+                image.SetAlpha(x, y, wx.IMAGE_ALPHA_OPAQUE)
+        image.ClearAlpha()
+
+class EmptyIcon():
+    def __init__(self, size, color, msg=None, ptsize=None, **args):
+        if size <= 0:
+            size = 50
+        size = int(size)
+        self._size = size
+        self._color = color
+        bmp = self.populate_image(msg, ptsize)
+        self._image = bmp.ConvertToImage()
+        # self._image = wx.Image(width=size, height=size, clear=True)
+        # for x in range(size):
+        #     for y in range(size):
+        #         self._image.SetRGB(x, y, color.red, color.green, color.blue)
+
+    def populate_image(self, msg=None, ptsize=None):
+        imgBit = wx.Bitmap(self._size, self._size)
+        dc = wx.MemoryDC(imgBit)
+        dc.SelectObject(imgBit)
+        brush = wx.Brush(self._color, wx.BRUSHSTYLE_SOLID)
+        dc.SetBackground(brush)
+        dc.Clear()
+        if msg is not None and msg != "":
+            # We only take the very first letter for
+            pattern={
+                "[red]": wx.RED,
+                "[green]": wx.GREEN,
+                "[blue]": wx.BLUE,
+                "[white]": wx.WHITE,
+                "[black]": wx.BLACK,
+            }
+            txt_color = wx.BLACK
+            for pat in pattern:
+                if msg.startswith(pat):
+                    txt_color = pattern[pat]
+                    msg = msg[len(pat):]
+            if ptsize is None:
+                ptsize = 12
+            font = wx.Font(
+                ptsize,
+                wx.FONTFAMILY_SWISS,
+                wx.FONTSTYLE_NORMAL,
+                wx.FONTWEIGHT_NORMAL,
+            )
+            dc.SetTextForeground(txt_color)
+            dc.SetFont(font)
+            (t_w, t_h) = dc.GetTextExtent(msg)
+            x = (self._size - t_w) / 2
+            y = (self._size - t_h) / 2
+            pt = wx.Point(x, y)
+            dc.DrawText(msg, pt)
+        # Now release dc
+        dc.SelectObject(wx.NullBitmap)
+        return imgBit
+
+    def GetBitmap(
+        self,
+        use_theme=True,
+        resize=None,
+        color=None,
+        rotate=None,
+        noadjustment=False,
+        keepalpha=False,
+    ):
+        """
+        Assumes greyscale icon black on transparent background using alpha for shading
+        Ready for Dark Theme
+        If color is provided, the black is changed to this
+        If color is close to background, alpha is removed and negative background added
+        so, we don't get black icon on black background or white on white background.
+
+        @param use_theme:
+        @param resize:
+        @param color:
+        @param rotate:
+        @param noadjustment: Disables size adjustment based on global factor
+        @param keepalpha: maintain the alpha from the original asset
+        @return:
+        """
+
+        image = self._image
+        if not noadjustment and _GLOBAL_FACTOR != 1.0:
+            oldresize = resize
+            wd, ht = image.GetSize()
+            if resize is not None:
+                if isinstance(resize, int) or isinstance(resize, float):
+                    resize *= _GLOBAL_FACTOR
+                    if 0 < _MIN_ICON_SIZE < oldresize:
+                        if resize < _MIN_ICON_SIZE:
+                            resize = _MIN_ICON_SIZE
+                elif isinstance(resize, tuple):  # (tuple wd ht)
+                    resize = [oldresize[0], oldresize[1]]
+                    for i in range(2):
+                        resize[i] *= _GLOBAL_FACTOR
+                        if 0 < _MIN_ICON_SIZE < oldresize[i]:
+                            if resize[i] < _MIN_ICON_SIZE:
+                                resize[i] = _MIN_ICON_SIZE
+            else:
+                resize = [wd, ht]
+                oldresize = (wd, ht)
+                for i in range(2):
+                    resize[i] *= _GLOBAL_FACTOR
+                    if 0 < _MIN_ICON_SIZE < oldresize[i]:
+                        if resize[i] < _MIN_ICON_SIZE:
+                            resize[i] = _MIN_ICON_SIZE
+            # print ("Will adjust from %s to %s (was: %s)" % ((wd, ht), resize, oldresize))
+
+        if resize is not None:
+            if isinstance(resize, int) or isinstance(resize, float):
+                image = image.Scale(int(resize), int(resize))
+            else:
+                image = image.Scale(int(resize[0]), int(resize[1]))
+        if rotate is not None:
+            if rotate == 1:
+                image = image.Rotate90()
+            elif rotate == 2:
+                image = image.Rotate180()
+            elif rotate == 3:
+                image = image.Rotate90(False)
+        if (
+            color is not None
+            and color.red is not None
+            and color.green is not None
+            and color.blue is not None
+        ):
+#            image.Replace(0, 0, 0, color.red, color.green, color.blue)
+            image.Replace(self._color.red, self._color.green, self._color.blue, color.red, color.green, color.blue)
+            if DARKMODE and use_theme:
+                reverse = color.distance_to("black") <= 200
+                black_bg = False
+            else:
+                reverse = color.distance_to("white") <= 200
+                black_bg = True
+            if reverse and not keepalpha:
+                self.RemoveAlpha(image, black_bg=black_bg)
+        elif DARKMODE and use_theme:
+            image.Replace(0, 0, 0, 255, 255, 255)
+        return wx.Bitmap(image)
+
+    def RemoveAlpha(self, image, black_bg=False):
+        if not image.HasAlpha():
+            return
+        bg_rgb = 0 if black_bg else 255
+        for x in range(image.GetWidth()):
+            for y in range(image.GetHeight()):
+                a = image.GetAlpha(x, y)
+                bg = int((255 - a) * bg_rgb / 255)
+                r = int(image.GetRed(x, y) * a / 255) + bg
+                g = int(image.GetGreen(x, y) * a / 255) + bg
+                b = int(image.GetBlue(x, y) * a / 255) + bg
+                image.SetRGB(x, y, r, g, b)
+                image.SetAlpha(x, y, wx.IMAGE_ALPHA_OPAQUE)
+        image.ClearAlpha()
+
+
+icons8_barcode_50 = PyEmbeddedImage(
+    b'iVBORw0KGgoAAAANSUhEUgAAADIAAAAyCAYAAAAeP4ixAAAABmJLR0QA/wD/AP+gvaeTAAAA'
+    b'4ElEQVRoge3Zuw3CMBSF4R9EzwIwAQswAgtkAjaABVgAqNLBBmnooKOkShcWSJmKCaBxkGXZ'
+    b'RkIUF+l8kmX5+nlqg4iIyPcGkdoOmHrjLXADlsAic1YDbIAJsA/mCtcfgHFkb+qOM3AE5sDa'
+    b'q7fAKvOW94OeXusfUQb1sF3dullkrtcl9qbuKF29COpN+Ojhp1T/QkGsURBrFMQaBbFGQaxR'
+    b'EGsUxBoFsUZBrFEQaxTEGgWxRkGsURBrFMSaUaR2Ae7euHV9DVSZs/o/i0dm3Yn4R0/qjtqb'
+    b'ryLrRUREfuIFnSA3JAyP8hcAAAAASUVORK5CYII=')
+
```

### Comparing `meerk40t-barcodes-0.2.0/setup.cfg` & `meerk40t-barcodes-0.2.1/setup.cfg`

 * *Files 24% similar despite different names*

```diff
@@ -1,69 +1,67 @@
-00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
-00000010: 203d 206d 6565 726b 3430 742d 6261 7263   = meerk40t-barc
-00000020: 6f64 6573 0d0a 7665 7273 696f 6e20 3d20  odes..version = 
-00000030: 302e 322e 300d 0a64 6573 6372 6970 7469  0.2.0..descripti
-00000040: 6f6e 203d 204d 6565 724b 3430 7420 4261  on = MeerK40t Ba
-00000050: 7263 6f64 6520 4578 7465 6e73 696f 6e0d  rcode Extension.
-00000060: 0a6c 6f6e 675f 6465 7363 7269 7074 696f  .long_descriptio
-00000070: 6e5f 636f 6e74 656e 745f 7479 7065 203d  n_content_type =
-00000080: 2074 6578 742f 6d61 726b 646f 776e 0d0a   text/markdown..
-00000090: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
-000000a0: 203d 2066 696c 653a 2052 4541 444d 452e   = file: README.
-000000b0: 6d64 0d0a 636c 6173 7369 6669 6572 7320  md..classifiers 
-000000c0: 3d20 0d0a 0944 6576 656c 6f70 6d65 6e74  = ...Development
-000000d0: 2053 7461 7475 7320 3a3a 2035 202d 2050   Status :: 5 - P
-000000e0: 726f 6475 6374 696f 6e2f 5374 6162 6c65  roduction/Stable
-000000f0: 0d0a 094c 6963 656e 7365 203a 3a20 4f53  ...License :: OS
-00000100: 4920 4170 7072 6f76 6564 203a 3a20 4d49  I Approved :: MI
-00000110: 5420 4c69 6365 6e73 650d 0a09 4f70 6572  T License...Oper
-00000120: 6174 696e 6720 5379 7374 656d 203a 3a20  ating System :: 
-00000130: 4f53 2049 6e64 6570 656e 6465 6e74 0d0a  OS Independent..
-00000140: 0950 726f 6772 616d 6d69 6e67 204c 616e  .Programming Lan
-00000150: 6775 6167 6520 3a3a 2050 7974 686f 6e0d  guage :: Python.
-00000160: 0a09 5072 6f67 7261 6d6d 696e 6720 4c61  ..Programming La
-00000170: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
-00000180: 203a 3a20 332e 360d 0a09 5072 6f67 7261   :: 3.6...Progra
-00000190: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
-000001a0: 3a20 5079 7468 6f6e 203a 3a20 332e 370d  : Python :: 3.7.
-000001b0: 0a09 5072 6f67 7261 6d6d 696e 6720 4c61  ..Programming La
-000001c0: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
-000001d0: 203a 3a20 332e 380d 0a09 5072 6f67 7261   :: 3.8...Progra
-000001e0: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
-000001f0: 3a20 5079 7468 6f6e 203a 3a20 332e 390d  : Python :: 3.9.
-00000200: 0a09 546f 7069 6320 3a3a 204d 756c 7469  ..Topic :: Multi
-00000210: 6d65 6469 6120 3a3a 2047 7261 7068 6963  media :: Graphic
-00000220: 730d 0a09 546f 7069 6320 3a3a 204d 756c  s...Topic :: Mul
-00000230: 7469 6d65 6469 6120 3a3a 2047 7261 7068  timedia :: Graph
-00000240: 6963 7320 3a3a 2045 6469 746f 7273 203a  ics :: Editors :
-00000250: 3a20 5665 6374 6f72 2d42 6173 6564 0d0a  : Vector-Based..
-00000260: 0954 6f70 6963 203a 3a20 5574 696c 6974  .Topic :: Utilit
-00000270: 6965 730d 0a6b 6579 776f 7264 7320 3d20  ies..keywords = 
-00000280: 6c61 7365 7263 7574 7465 722c 206c 6173  lasercutter, las
-00000290: 6572 2c20 7665 6374 6f72 2c20 7061 7273  er, vector, pars
-000002a0: 6572 0d0a 6175 7468 6f72 203d 206a 7069  er..author = jpi
-000002b0: 726e 6179 0d0a 6175 7468 6f72 5f65 6d61  rnay..author_ema
-000002c0: 696c 203d 2074 6174 6172 697a 6540 676d  il = tatarize@gm
-000002d0: 6169 6c2e 636f 6d0d 0a75 726c 203d 2068  ail.com..url = h
-000002e0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-000002f0: 6d2f 6d65 6572 6b34 3074 2f6d 6565 726b  m/meerk40t/meerk
-00000300: 3430 742d 6261 7263 6f64 6573 0d0a 6c69  40t-barcodes..li
-00000310: 6365 6e73 6520 3d20 4d49 540d 0a0d 0a5b  cense = MIT....[
-00000320: 6f70 7469 6f6e 735d 0d0a 7a69 705f 7361  options]..zip_sa
-00000330: 6665 203d 2054 7275 650d 0a69 6e63 6c75  fe = True..inclu
-00000340: 6465 5f70 6163 6b61 6765 5f64 6174 6120  de_package_data 
-00000350: 3d20 5472 7565 0d0a 7061 636b 6167 6573  = True..packages
-00000360: 203d 2066 696e 643a 0d0a 7061 636b 6167   = find:..packag
-00000370: 655f 6469 7220 3d20 0d0a 093d 202e 0d0a  e_dir = ...= ...
-00000380: 7465 7374 5f73 7569 7465 203d 2074 6573  test_suite = tes
-00000390: 740d 0a0d 0a5b 7065 7038 5d0d 0a6d 6178  t....[pep8]..max
-000003a0: 2d6c 696e 652d 6c65 6e67 7468 203d 2031  -line-length = 1
-000003b0: 3030 0d0a 0d0a 5b62 6469 7374 5f77 6865  00....[bdist_whe
-000003c0: 656c 5d0d 0a75 6e69 7665 7273 616c 203d  el]..universal =
-000003d0: 2031 0d0a 0d0a 5b6f 7074 696f 6e73 2e65   1....[options.e
-000003e0: 6e74 7279 5f70 6f69 6e74 735d 0d0a 6d65  ntry_points]..me
-000003f0: 6572 6b34 3074 2e65 7874 656e 7369 6f6e  erk40t.extension
-00000400: 203d 2045 7861 6d70 6c65 203d 2062 6172   = Example = bar
-00000410: 636f 6465 732e 6d61 696e 3a70 6c75 6769  codes.main:plugi
-00000420: 6e0d 0a0d 0a5b 6567 675f 696e 666f 5d0d  n....[egg_info].
-00000430: 0a74 6167 5f62 7569 6c64 203d 200d 0a74  .tag_build = ..t
-00000440: 6167 5f64 6174 6520 3d20 300d 0a0d 0a    ag_date = 0....
+00000000: 5b6d 6574 6164 6174 615d 0a6e 616d 6520  [metadata].name 
+00000010: 3d20 6d65 6572 6b34 3074 2d62 6172 636f  = meerk40t-barco
+00000020: 6465 730a 7665 7273 696f 6e20 3d20 302e  des.version = 0.
+00000030: 322e 310a 6465 7363 7269 7074 696f 6e20  2.1.description 
+00000040: 3d20 4d65 6572 4b34 3074 2042 6172 636f  = MeerK40t Barco
+00000050: 6465 2045 7874 656e 7369 6f6e 0a6c 6f6e  de Extension.lon
+00000060: 675f 6465 7363 7269 7074 696f 6e5f 636f  g_description_co
+00000070: 6e74 656e 745f 7479 7065 203d 2074 6578  ntent_type = tex
+00000080: 742f 6d61 726b 646f 776e 0a6c 6f6e 675f  t/markdown.long_
+00000090: 6465 7363 7269 7074 696f 6e20 3d20 6669  description = fi
+000000a0: 6c65 3a20 5245 4144 4d45 2e6d 640a 636c  le: README.md.cl
+000000b0: 6173 7369 6669 6572 7320 3d20 0a09 4465  assifiers = ..De
+000000c0: 7665 6c6f 706d 656e 7420 5374 6174 7573  velopment Status
+000000d0: 203a 3a20 3520 2d20 5072 6f64 7563 7469   :: 5 - Producti
+000000e0: 6f6e 2f53 7461 626c 650a 094c 6963 656e  on/Stable..Licen
+000000f0: 7365 203a 3a20 4f53 4920 4170 7072 6f76  se :: OSI Approv
+00000100: 6564 203a 3a20 4d49 5420 4c69 6365 6e73  ed :: MIT Licens
+00000110: 650a 094f 7065 7261 7469 6e67 2053 7973  e..Operating Sys
+00000120: 7465 6d20 3a3a 204f 5320 496e 6465 7065  tem :: OS Indepe
+00000130: 6e64 656e 740a 0950 726f 6772 616d 6d69  ndent..Programmi
+00000140: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
+00000150: 7974 686f 6e0a 0950 726f 6772 616d 6d69  ython..Programmi
+00000160: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
+00000170: 7974 686f 6e20 3a3a 2033 2e36 0a09 5072  ython :: 3.6..Pr
+00000180: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
+00000190: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
+000001a0: 332e 370a 0950 726f 6772 616d 6d69 6e67  3.7..Programming
+000001b0: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
+000001c0: 686f 6e20 3a3a 2033 2e38 0a09 5072 6f67  hon :: 3.8..Prog
+000001d0: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
+000001e0: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
+000001f0: 390a 0954 6f70 6963 203a 3a20 4d75 6c74  9..Topic :: Mult
+00000200: 696d 6564 6961 203a 3a20 4772 6170 6869  imedia :: Graphi
+00000210: 6373 0a09 546f 7069 6320 3a3a 204d 756c  cs..Topic :: Mul
+00000220: 7469 6d65 6469 6120 3a3a 2047 7261 7068  timedia :: Graph
+00000230: 6963 7320 3a3a 2045 6469 746f 7273 203a  ics :: Editors :
+00000240: 3a20 5665 6374 6f72 2d42 6173 6564 0a09  : Vector-Based..
+00000250: 546f 7069 6320 3a3a 2055 7469 6c69 7469  Topic :: Utiliti
+00000260: 6573 0a6b 6579 776f 7264 7320 3d20 6c61  es.keywords = la
+00000270: 7365 7263 7574 7465 722c 206c 6173 6572  sercutter, laser
+00000280: 2c20 7665 6374 6f72 2c20 7061 7273 6572  , vector, parser
+00000290: 0a61 7574 686f 7220 3d20 6a70 6972 6e61  .author = jpirna
+000002a0: 790a 6175 7468 6f72 5f65 6d61 696c 203d  y.author_email =
+000002b0: 2074 6174 6172 697a 6540 676d 6169 6c2e   tatarize@gmail.
+000002c0: 636f 6d0a 7572 6c20 3d20 6874 7470 733a  com.url = https:
+000002d0: 2f2f 6769 7468 7562 2e63 6f6d 2f6d 6565  //github.com/mee
+000002e0: 726b 3430 742f 6d65 6572 6b34 3074 2d62  rk40t/meerk40t-b
+000002f0: 6172 636f 6465 730a 6c69 6365 6e73 6520  arcodes.license 
+00000300: 3d20 4d49 540a 0a5b 6f70 7469 6f6e 735d  = MIT..[options]
+00000310: 0a7a 6970 5f73 6166 6520 3d20 5472 7565  .zip_safe = True
+00000320: 0a69 6e63 6c75 6465 5f70 6163 6b61 6765  .include_package
+00000330: 5f64 6174 6120 3d20 5472 7565 0a70 6163  _data = True.pac
+00000340: 6b61 6765 7320 3d20 6669 6e64 3a0a 7061  kages = find:.pa
+00000350: 636b 6167 655f 6469 7220 3d20 0a09 3d20  ckage_dir = ..= 
+00000360: 2e0a 7465 7374 5f73 7569 7465 203d 2074  ..test_suite = t
+00000370: 6573 740a 0a5b 7065 7038 5d0a 6d61 782d  est..[pep8].max-
+00000380: 6c69 6e65 2d6c 656e 6774 6820 3d20 3130  line-length = 10
+00000390: 300a 0a5b 6264 6973 745f 7768 6565 6c5d  0..[bdist_wheel]
+000003a0: 0a75 6e69 7665 7273 616c 203d 2031 0a0a  .universal = 1..
+000003b0: 5b6f 7074 696f 6e73 2e65 6e74 7279 5f70  [options.entry_p
+000003c0: 6f69 6e74 735d 0a6d 6565 726b 3430 742e  oints].meerk40t.
+000003d0: 6578 7465 6e73 696f 6e20 3d20 4578 616d  extension = Exam
+000003e0: 706c 6520 3d20 6261 7263 6f64 6573 2e6d  ple = barcodes.m
+000003f0: 6169 6e3a 706c 7567 696e 0a0a 5b65 6767  ain:plugin..[egg
+00000400: 5f69 6e66 6f5d 0a74 6167 5f62 7569 6c64  _info].tag_build
+00000410: 203d 200a 7461 675f 6461 7465 203d 2030   = .tag_date = 0
+00000420: 0a0a                                     ..
```

