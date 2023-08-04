# Comparing `tmp/mass_analytics-1.0.9.tar.gz` & `tmp/mass_analytics-1.1.0.tar.gz`

## Comparing `mass_analytics-1.0.9.tar` & `mass_analytics-1.1.0.tar`

### file list

```diff
@@ -1,8 +1,10 @@
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 mass_analytics-1.0.9/src/mass_analytics/__init__.py
--rw-r--r--   0        0        0     7191 2020-02-02 00:00:00.000000 mass_analytics-1.0.9/src/mass_analytics/data_frame_util.py
--rw-r--r--   0        0        0     4946 2020-02-02 00:00:00.000000 mass_analytics-1.0.9/src/mass_analytics/date.py
--rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 mass_analytics-1.0.9/src/mass_analytics/reader.py
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 mass_analytics-1.0.9/LICENSE.txt
--rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 mass_analytics-1.0.9/README.md
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 mass_analytics-1.0.9/pyproject.toml
--rw-r--r--   0        0        0     2327 2020-02-02 00:00:00.000000 mass_analytics-1.0.9/PKG-INFO
+-rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 mass_analytics-1.1.0/src/mass_analytics/__init__.py
+-rw-r--r--   0        0        0    12870 2020-02-02 00:00:00.000000 mass_analytics-1.1.0/src/mass_analytics/data_frame_util.py
+-rw-r--r--   0        0        0    12675 2020-02-02 00:00:00.000000 mass_analytics-1.1.0/src/mass_analytics/data_overview.py
+-rw-r--r--   0        0        0     9881 2020-02-02 00:00:00.000000 mass_analytics-1.1.0/src/mass_analytics/date.py
+-rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 mass_analytics-1.1.0/src/mass_analytics/plotting.py
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 mass_analytics-1.1.0/src/mass_analytics/reader.py
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 mass_analytics-1.1.0/LICENSE.txt
+-rw-r--r--   0        0        0     1449 2020-02-02 00:00:00.000000 mass_analytics-1.1.0/README.md
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 mass_analytics-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2080 2020-02-02 00:00:00.000000 mass_analytics-1.1.0/PKG-INFO
```

### Comparing `mass_analytics-1.0.9/LICENSE.txt` & `mass_analytics-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mass_analytics-1.0.9/pyproject.toml` & `mass_analytics-1.1.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 00000010: 7265 7175 6972 6573 203d 205b 2268 6174  requires = ["hat
 00000020: 6368 6c69 6e67 225d 0d0a 6275 696c 642d  chling"]..build-
 00000030: 6261 636b 656e 6420 3d20 2268 6174 6368  backend = "hatch
 00000040: 6c69 6e67 2e62 7569 6c64 220d 0a0d 0a5b  ling.build"....[
 00000050: 7072 6f6a 6563 745d 0d0a 6e61 6d65 203d  project]..name =
 00000060: 2022 6d61 7373 5f61 6e61 6c79 7469 6373   "mass_analytics
 00000070: 220d 0a76 6572 7369 6f6e 203d 2022 312e  "..version = "1.
-00000080: 302e 3922 0d0a 6175 7468 6f72 7320 3d20  0.9"..authors = 
+00000080: 312e 3022 0d0a 6175 7468 6f72 7320 3d20  1.0"..authors = 
 00000090: 5b0d 0a20 207b 206e 616d 653d 2253 656c  [..  { name="Sel
 000000a0: 696d 222c 2065 6d61 696c 3d22 7365 6c69  im", email="seli
 000000b0: 6d2e 616c 6f75 696e 6940 6d61 7373 2d61  m.alouini@mass-a
 000000c0: 6e61 6c79 7469 6373 2e63 6f6d 2220 7d2c  nalytics.com" },
 000000d0: 0d0a 5d0d 0a64 6573 6372 6970 7469 6f6e  ..]..description
 000000e0: 203d 2022 5374 7265 616d 6c69 6e65 2064   = "Streamline d
 000000f0: 6174 6120 7072 6570 726f 6365 7373 696e  ata preprocessin
@@ -36,8 +36,13 @@
 00000230: 3d3d 312e 3235 2e31 222c 0d0a 2020 2020  ==1.25.1",..    
 00000240: 2020 2020 2270 616e 6461 733d 3d32 2e30      "pandas==2.0
 00000250: 2e33 222c 0d0a 2020 2020 2020 2020 2270  .3",..        "p
 00000260: 6c6f 746c 793d 3d35 2e31 352e 3022 2c0d  lotly==5.15.0",.
 00000270: 0a20 2020 2020 2020 2022 7374 7265 616d  .        "stream
 00000280: 6c69 743d 3d31 2e32 342e 3122 2c0d 0a20  lit==1.24.1",.. 
 00000290: 2020 2020 2020 2022 6f70 656e 7079 786c         "openpyxl
-000002a0: 220d 0a20 2020 205d 0d0a                 "..    ]..
+000002a0: 222c 0d0a 2020 2020 2020 2020 2274 7164  ",..        "tqd
+000002b0: 6d22 2c0d 0a20 2020 2020 2020 2022 6675  m",..        "fu
+000002c0: 7a7a 7977 757a 7a79 222c 0d0a 2020 2020  zzywuzzy",..    
+000002d0: 2020 2020 2270 7974 686f 6e2d 4c65 7665      "python-Leve
+000002e0: 6e73 6874 6569 6e22 0d0a 2020 2020 5d0d  nshtein"..    ].
+000002f0: 0a                                       .
```

### Comparing `mass_analytics-1.0.9/PKG-INFO` & `mass_analytics-1.1.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 Metadata-Version: 2.1
 Name: mass_analytics
-Version: 1.0.9
+Version: 1.1.0
 Summary: Streamline data preprocessing and enhance analysis with our Powerful Data Preparation Package.
 Author-email: Selim <selim.alouini@mass-analytics.com>
 License-File: LICENSE.txt
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
+Requires-Dist: fuzzywuzzy
 Requires-Dist: numpy==1.25.1
 Requires-Dist: openpyxl
 Requires-Dist: pandas==2.0.3
 Requires-Dist: plotly==5.15.0
+Requires-Dist: python-levenshtein
 Requires-Dist: streamlit==1.24.1
+Requires-Dist: tqdm
 Description-Content-Type: text/markdown
 
-<div align="center">
-  <img src="https://scontent.ftun10-1.fna.fbcdn.net/v/t39.30808-6/332904748_897461364866284_4163373948614352887_n.png?_nc_cat=111&ccb=1-7&_nc_sid=e3f864&_nc_ohc=mOs26BnW5rYAX_0w3ot&_nc_ht=scontent.ftun10-1.fna&oh=00_AfAlZswU__xPYbBsm3NHsnfhP13luB_BTBSUGJsITrSyNw&oe=64C273EC"><br>
-</div>
 
------------------
 # Mass-Analytics: Data Preparation Made Easy
 
 [![PyPI Version](https://img.shields.io/pypi/v/mass-analytics.svg)](https://pypi.org/project/mass-analytics/)
 [![Python Versions](https://img.shields.io/pypi/pyversions/mass-analytics.svg)](https://pypi.org/project/mass-analytics/)
 
 ## Overview
```

