# Comparing `tmp/galaxygst-1.0.0-py3-none-any.whl.zip` & `tmp/galaxygst-1.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 21274 bytes, number of entries: 9
--rw-rw-rw-  2.0 fat       67 b- defN 23-Apr-13 14:28 galaxygst/__init__.py
--rw-rw-rw-  2.0 fat     1522 b- defN 23-Apr-18 12:20 galaxygst/__main__.py
+Zip file size: 21614 bytes, number of entries: 9
+-rw-rw-rw-  2.0 fat       67 b- defN 23-Aug-04 17:04 galaxygst/__init__.py
+-rw-rw-rw-  2.0 fat     1898 b- defN 23-Aug-04 17:07 galaxygst/__main__.py
 -rw-rw-rw-  2.0 fat    20384 b- defN 23-Apr-18 12:14 galaxygst/gst.py
--rw-rw-rw-  2.0 fat    35823 b- defN 23-Apr-18 15:36 galaxygst-1.0.0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     4221 b- defN 23-Apr-18 15:36 galaxygst-1.0.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-18 15:36 galaxygst-1.0.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       54 b- defN 23-Apr-18 15:36 galaxygst-1.0.0.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat       10 b- defN 23-Apr-18 15:36 galaxygst-1.0.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      722 b- defN 23-Apr-18 15:36 galaxygst-1.0.0.dist-info/RECORD
-9 files, 62895 bytes uncompressed, 20030 bytes compressed:  68.2%
+-rw-rw-rw-  2.0 fat    35823 b- defN 23-Aug-04 17:16 galaxygst-1.0.1.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     4620 b- defN 23-Aug-04 17:16 galaxygst-1.0.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Aug-04 17:16 galaxygst-1.0.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       54 b- defN 23-Aug-04 17:16 galaxygst-1.0.1.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat       10 b- defN 23-Aug-04 17:16 galaxygst-1.0.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      722 b- defN 23-Aug-04 17:16 galaxygst-1.0.1.dist-info/RECORD
+9 files, 63670 bytes uncompressed, 20370 bytes compressed:  68.0%
```

## zipnote {}

```diff
@@ -3,26 +3,26 @@
 
 Filename: galaxygst/__main__.py
 Comment: 
 
 Filename: galaxygst/gst.py
 Comment: 
 
-Filename: galaxygst-1.0.0.dist-info/LICENSE
+Filename: galaxygst-1.0.1.dist-info/LICENSE
 Comment: 
 
-Filename: galaxygst-1.0.0.dist-info/METADATA
+Filename: galaxygst-1.0.1.dist-info/METADATA
 Comment: 
 
-Filename: galaxygst-1.0.0.dist-info/WHEEL
+Filename: galaxygst-1.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: galaxygst-1.0.0.dist-info/entry_points.txt
+Filename: galaxygst-1.0.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: galaxygst-1.0.0.dist-info/top_level.txt
+Filename: galaxygst-1.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: galaxygst-1.0.0.dist-info/RECORD
+Filename: galaxygst-1.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## galaxygst/__init__.py

```diff
@@ -1,4 +1,4 @@
-__version__ = "1.0.0"
+__version__ = "1.0.1"
 __author__ = "Aurum"
 
 from .gst import *
```

## galaxygst/__main__.py

```diff
@@ -10,14 +10,20 @@
     except ValueError:
         print("Error! Address has an unknown number format!", file=sys.stderr)
         return
 
     print("Welcome to galaxygst! To find out how to set up the GST recorder in a galaxy, please refer to the GitHub\n"
           "repository's README file! If you want to cancel the tool's execution, press CTRL+C any time. To stop\n"
           "recording, press 2 on the first player's Wiimote!\n"
+          "\n"
+          "NOTE: If the recording process terminates due to a synchronization error, you should try the following\n"
+          "things before recording again:\n"
+          "- Close unnecessary programs and processes.\n"
+          "- Give the galaxygst process a higher priority.\n"
+          "- Reduce the emulation's execution speed (less than 100%).\n"
           "------------------------------------------------------------------------------")
     try:
         gst.record_gst_from_dolphin(args.output_folder_path, addr_gst_recorder_info_ptr)
     except KeyboardInterrupt:
         print("Execution canceled.")
     except RuntimeError as e:
         print(f"An error occurred: {str(e)}")
```

## Comparing `galaxygst-1.0.0.dist-info/LICENSE` & `galaxygst-1.0.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `galaxygst-1.0.0.dist-info/METADATA` & `galaxygst-1.0.1.dist-info/METADATA`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galaxygst
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python tool to record GST object motion for Super Mario Galaxy 2
 Home-page: https://github.com/SunakazeKun/galaxygst
 Author: Aurum
 License: gpl-3.0
 Keywords: nintendo,super-mario-galaxy-2,gst,dolphin,modding
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
@@ -62,7 +62,15 @@
 Waiting for GstRecordHelper...
 Started recording for GhostAttackGhost in RedBlueExGalaxy Star 1!
 Stopped recording!
 Dumped 619 ghost frames (approx. 10 seconds) to '.\RedBlueExGalaxy\GhostAttackGhostData01.gst'.
 ```
 
 After recording, you can build a Ghost.arc containing the GST file. However, this is beyond the scope of this tool. In final releases of your levels, you don't want players to interact with GstRecordHelper objects, so make sure to remove them once they are not needed anymore.
+
+## Synchronization Error
+If the recording process terminates due to a synchronization error, you should try the following things before recording again:
+- Close unnecessary programs and processes.
+- Give the galaxygst process a higher priority.
+- Reduce the emulation's execution speed (less than 100%).
+
+If the error persists, try cutting down the emulator's execution speed even further.
```

