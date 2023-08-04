# Comparing `tmp/pymca-5.8.8-py2.py3-none-any.whl.zip` & `tmp/pymca-5.8.9-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 5531 bytes, number of entries: 7
--rw-rw-rw-  2.0 fat     5996 b- defN 23-Aug-02 14:58 pymca-5.8.8.data/scripts/pymca_launcher
--rw-rw-rw-  2.0 fat       31 b- defN 16-Dec-03 05:23 pymca-5.8.8.data/scripts/pymca_launcher.bat
--rw-rw-rw-  2.0 fat     1817 b- defN 23-Aug-02 14:58 pymca-5.8.8.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1775 b- defN 23-Aug-02 14:58 pymca-5.8.8.dist-info/METADATA
--rw-rw-rw-  2.0 fat      110 b- defN 23-Aug-02 14:58 pymca-5.8.8.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        6 b- defN 23-Aug-02 14:58 pymca-5.8.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      570 b- defN 23-Aug-02 14:58 pymca-5.8.8.dist-info/RECORD
-7 files, 10305 bytes uncompressed, 4515 bytes compressed:  56.2%
+Zip file size: 5529 bytes, number of entries: 7
+-rw-rw-rw-  2.0 fat     5996 b- defN 23-Aug-04 15:06 pymca-5.8.9.data/scripts/pymca_launcher
+-rw-rw-rw-  2.0 fat       31 b- defN 16-Dec-03 05:23 pymca-5.8.9.data/scripts/pymca_launcher.bat
+-rw-rw-rw-  2.0 fat     1817 b- defN 23-Aug-04 15:06 pymca-5.8.9.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1775 b- defN 23-Aug-04 15:06 pymca-5.8.9.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      110 b- defN 23-Aug-04 15:06 pymca-5.8.9.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        6 b- defN 23-Aug-04 15:06 pymca-5.8.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      570 b- defN 23-Aug-04 15:06 pymca-5.8.9.dist-info/RECORD
+7 files, 10305 bytes uncompressed, 4513 bytes compressed:  56.2%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
-Filename: pymca-5.8.8.data/scripts/pymca_launcher
+Filename: pymca-5.8.9.data/scripts/pymca_launcher
 Comment: 
 
-Filename: pymca-5.8.8.data/scripts/pymca_launcher.bat
+Filename: pymca-5.8.9.data/scripts/pymca_launcher.bat
 Comment: 
 
-Filename: pymca-5.8.8.dist-info/LICENSE
+Filename: pymca-5.8.9.dist-info/LICENSE
 Comment: 
 
-Filename: pymca-5.8.8.dist-info/METADATA
+Filename: pymca-5.8.9.dist-info/METADATA
 Comment: 
 
-Filename: pymca-5.8.8.dist-info/WHEEL
+Filename: pymca-5.8.9.dist-info/WHEEL
 Comment: 
 
-Filename: pymca-5.8.8.dist-info/top_level.txt
+Filename: pymca-5.8.9.dist-info/top_level.txt
 Comment: 
 
-Filename: pymca-5.8.8.dist-info/RECORD
+Filename: pymca-5.8.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `pymca-5.8.8.data/scripts/pymca_launcher` & `pymca-5.8.9.data/scripts/pymca_launcher`

 * *Files identical despite different names*

## Comparing `pymca-5.8.8.dist-info/LICENSE` & `pymca-5.8.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pymca-5.8.8.dist-info/METADATA` & `pymca-5.8.9.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymca
-Version: 5.8.8
+Version: 5.8.9
 Summary: pymca
 Author: V.A. Sole - ESRF
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: MacOS X
 Classifier: Environment :: Win32 (MS Windows)
 Classifier: Intended Audience :: Education
@@ -20,15 +20,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 License-File: LICENSE
-Requires-Dist: PyMca5 (>=5.8.8)
+Requires-Dist: PyMca5 (>=5.8.9)
 Requires-Dist: h5py
 Requires-Dist: numpy
 Requires-Dist: matplotlib
 
 pymca
 =====
```

