# Comparing `tmp/galaxypad-1.0.3-py3-none-any.whl.zip` & `tmp/galaxypad-1.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 7815 bytes, number of entries: 8
--rw-rw-rw-  2.0 fat       67 b- defN 23-Apr-17 15:54 galaxypad/__init__.py
--rw-rw-rw-  2.0 fat     1517 b- defN 23-Apr-10 17:18 galaxypad/__main__.py
+Zip file size: 8149 bytes, number of entries: 8
+-rw-rw-rw-  2.0 fat       67 b- defN 23-Aug-04 17:06 galaxypad/__init__.py
+-rw-rw-rw-  2.0 fat     1893 b- defN 23-Aug-04 17:07 galaxypad/__main__.py
 -rw-rw-rw-  2.0 fat    13660 b- defN 23-Apr-17 15:55 galaxypad/pad.py
--rw-rw-rw-  2.0 fat     4575 b- defN 23-Apr-17 15:56 galaxypad-1.0.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-17 15:56 galaxypad-1.0.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       54 b- defN 23-Apr-17 15:56 galaxypad-1.0.3.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat       10 b- defN 23-Apr-17 15:56 galaxypad-1.0.3.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      631 b- defN 23-Apr-17 15:56 galaxypad-1.0.3.dist-info/RECORD
-8 files, 20606 bytes uncompressed, 6713 bytes compressed:  67.4%
+-rw-rw-rw-  2.0 fat     4974 b- defN 23-Aug-04 17:09 galaxypad-1.0.4.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Aug-04 17:09 galaxypad-1.0.4.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       54 b- defN 23-Aug-04 17:09 galaxypad-1.0.4.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat       10 b- defN 23-Aug-04 17:09 galaxypad-1.0.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      631 b- defN 23-Aug-04 17:09 galaxypad-1.0.4.dist-info/RECORD
+8 files, 21381 bytes uncompressed, 7047 bytes compressed:  67.0%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: galaxypad/__main__.py
 Comment: 
 
 Filename: galaxypad/pad.py
 Comment: 
 
-Filename: galaxypad-1.0.3.dist-info/METADATA
+Filename: galaxypad-1.0.4.dist-info/METADATA
 Comment: 
 
-Filename: galaxypad-1.0.3.dist-info/WHEEL
+Filename: galaxypad-1.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: galaxypad-1.0.3.dist-info/entry_points.txt
+Filename: galaxypad-1.0.4.dist-info/entry_points.txt
 Comment: 
 
-Filename: galaxypad-1.0.3.dist-info/top_level.txt
+Filename: galaxypad-1.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: galaxypad-1.0.3.dist-info/RECORD
+Filename: galaxypad-1.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## galaxypad/__init__.py

```diff
@@ -1,4 +1,4 @@
-__version__ = "1.0.3"
+__version__ = "1.0.4"
 __author__ = "Aurum"
 
 from .pad import *
```

## galaxypad/__main__.py

```diff
@@ -10,14 +10,20 @@
     except ValueError:
         print("Error! Address has an unknown number format!", file=sys.stderr)
         return
 
     print("Welcome to galaxypad! To find out how to set up the PAD recorder in a galaxy, please refer to the GitHub\n"
           "repository's README file! If you want to cancel the tool's execution, press CTRL+C any time. To stop\n"
           "recording, press 2 on the first player's Wiimote!\n"
+          "\n"
+          "NOTE: If the recording process terminates due to a synchronization error, you should try the following\n"
+          "things before recording again:\n"
+          "- Close unnecessary programs and processes.\n"
+          "- Give the galaxypad process a higher priority.\n"
+          "- Reduce the emulation's execution speed (less than 100%).\n"
           "------------------------------------------------------------------------------")
     try:
         pad.record_pad_from_dolphin(args.output_folder_path, addr_pad_recorder_info_ptr)
     except KeyboardInterrupt:
         print("Execution canceled.")
     except RuntimeError as e:
         print(f"An error occurred: {str(e)}")
```

## Comparing `galaxypad-1.0.3.dist-info/METADATA` & `galaxypad-1.0.4.dist-info/METADATA`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galaxypad
-Version: 1.0.3
+Version: 1.0.4
 Summary: Python tool to record PAD playback for Super Mario Galaxy 2
 Home-page: https://github.com/SunakazeKun/galaxypad
 Author: Aurum
 License: gpl-3.0
 Keywords: nintendo,super-mario-galaxy-2,pad,dolphin,modding
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
@@ -69,7 +69,15 @@
 Waiting for PadRecordHelper...
 Started recording for spawn ID 0 in RedBlueExGalaxy!
 Stopped recording!
 Dumped 3075 KPAD frames (approx. 51 seconds) to '.\RedBlueExGalaxy\Dreamer0.pad'.
 ```
 
 After recording, you can build a Ghost.arc containing the PAD file. However, this is beyond the scope of this tool. In final releases of your levels, you don't want players to interact with PadRecordHelper objects, so make sure to remove them once they are not needed anymore.
+
+## Synchronization Error
+If the recording process terminates due to a synchronization error, you should try the following things before recording again:
+- Close unnecessary programs and processes.
+- Give the galaxypad process a higher priority.
+- Reduce the emulation's execution speed (less than 100%).
+
+If the error persists, try cutting down the emulator's execution speed even further.
```

