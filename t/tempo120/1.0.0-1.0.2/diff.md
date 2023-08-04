# Comparing `tmp/tempo120-1.0.0.tar.gz` & `tmp/tempo120-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\products\tempo120\github - Kopie\dist\.tmp-vimra197\tempo120-1.0.0.tar", last modified: Thu Aug  3 15:32:28 2023, max compression
+gzip compressed data, was "D:\products\tempo120\github - Kopie\dist\.tmp-2kzsfuo4\tempo120-1.0.2.tar", last modified: Fri Aug  4 19:25:25 2023, max compression
```

## Comparing `tempo120-1.0.0.tar` & `tempo120-1.0.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-08-03 15:32:28.571536 tempo120-1.0.0/
--rw-rw-rw-   0        0        0    35149 2023-07-11 18:42:22.000000 tempo120-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     4976 2023-08-03 15:32:28.570536 tempo120-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     3955 2023-08-03 14:52:04.000000 tempo120-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-08-03 15:32:28.515523 tempo120-1.0.0/gfx/
--rw-rw-rw-   0        0        0     6941 2023-07-08 15:23:15.000000 tempo120-1.0.0/gfx/car.png
--rw-rw-rw-   0        0        0   107076 2023-07-08 20:36:33.000000 tempo120-1.0.0/gfx/screenshot1.png
--rw-rw-rw-   0        0        0    29421 2023-07-08 20:36:19.000000 tempo120-1.0.0/gfx/screenshot2.png
--rw-rw-rw-   0        0        0    17458 2023-07-08 20:36:06.000000 tempo120-1.0.0/gfx/screenshot3.png
--rw-rw-rw-   0        0        0    16872 2023-07-08 20:35:55.000000 tempo120-1.0.0/gfx/screenshot4.png
--rw-rw-rw-   0        0        0    85199 2023-07-08 19:53:15.000000 tempo120-1.0.0/gfx/title.png
--rw-rw-rw-   0        0        0    30108 2023-08-02 17:31:30.000000 tempo120-1.0.0/gfx/track01.png
-drwxrwxrwx   0        0        0        0 2023-08-03 15:32:28.536529 tempo120-1.0.0/muzak/
--rw-rw-rw-   0        0        0    16512 2023-07-23 13:45:55.000000 tempo120-1.0.0/muzak/engine.ogg
--rw-rw-rw-   0        0        0  1955997 2023-07-08 18:57:12.000000 tempo120-1.0.0/muzak/track.ogg
-drwxrwxrwx   0        0        0        0 2023-08-03 15:32:28.563534 tempo120-1.0.0/scores/
--rw-rw-rw-   0        0        0       55 2023-07-10 18:10:59.000000 tempo120-1.0.0/scores/scores.txt
--rw-rw-rw-   0        0        0       42 2023-08-03 15:32:28.571536 tempo120-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     2069 2023-08-03 15:13:18.000000 tempo120-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-03 15:32:28.570536 tempo120-1.0.0/tempo120.egg-info/
--rw-rw-rw-   0        0        0     4976 2023-08-03 15:32:28.000000 tempo120-1.0.0/tempo120.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      374 2023-08-03 15:32:28.000000 tempo120-1.0.0/tempo120.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-03 15:32:28.000000 tempo120-1.0.0/tempo120.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2023-08-03 15:32:28.000000 tempo120-1.0.0/tempo120.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       26 2023-08-03 15:32:28.000000 tempo120-1.0.0/tempo120.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    17472 2023-08-03 15:14:17.000000 tempo120-1.0.0/tempo120.py
+drwxrwxrwx   0        0        0        0 2023-08-04 19:25:25.896750 tempo120-1.0.2/
+-rw-rw-rw-   0        0        0    35149 2023-07-11 18:42:22.000000 tempo120-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0     4879 2023-08-04 19:25:25.895750 tempo120-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3860 2023-08-04 19:25:07.000000 tempo120-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-08-04 19:25:25.852741 tempo120-1.0.2/gfx/
+-rw-rw-rw-   0        0        0     6941 2023-07-08 15:23:15.000000 tempo120-1.0.2/gfx/car.png
+-rw-rw-rw-   0        0        0   107076 2023-07-08 20:36:33.000000 tempo120-1.0.2/gfx/screenshot1.png
+-rw-rw-rw-   0        0        0    29421 2023-07-08 20:36:19.000000 tempo120-1.0.2/gfx/screenshot2.png
+-rw-rw-rw-   0        0        0    17458 2023-07-08 20:36:06.000000 tempo120-1.0.2/gfx/screenshot3.png
+-rw-rw-rw-   0        0        0    16872 2023-07-08 20:35:55.000000 tempo120-1.0.2/gfx/screenshot4.png
+-rw-rw-rw-   0        0        0    85199 2023-07-08 19:53:15.000000 tempo120-1.0.2/gfx/title.png
+-rw-rw-rw-   0        0        0    30108 2023-08-02 17:31:30.000000 tempo120-1.0.2/gfx/track01.png
+drwxrwxrwx   0        0        0        0 2023-08-04 19:25:25.870744 tempo120-1.0.2/muzak/
+-rw-rw-rw-   0        0        0    16512 2023-07-23 13:45:55.000000 tempo120-1.0.2/muzak/engine.ogg
+-rw-rw-rw-   0        0        0  1955997 2023-07-08 18:57:12.000000 tempo120-1.0.2/muzak/track.ogg
+drwxrwxrwx   0        0        0        0 2023-08-04 19:25:25.881749 tempo120-1.0.2/scores/
+-rw-rw-rw-   0        0        0       55 2023-07-10 18:10:59.000000 tempo120-1.0.2/scores/scores.txt
+-rw-rw-rw-   0        0        0       42 2023-08-04 19:25:25.896750 tempo120-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     2069 2023-08-04 19:23:18.000000 tempo120-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-04 19:25:25.893752 tempo120-1.0.2/tempo120.egg-info/
+-rw-rw-rw-   0        0        0     4879 2023-08-04 19:25:25.000000 tempo120-1.0.2/tempo120.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      374 2023-08-04 19:25:25.000000 tempo120-1.0.2/tempo120.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-04 19:25:25.000000 tempo120-1.0.2/tempo120.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2023-08-04 19:25:25.000000 tempo120-1.0.2/tempo120.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       26 2023-08-04 19:25:25.000000 tempo120-1.0.2/tempo120.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    17472 2023-08-03 15:14:17.000000 tempo120-1.0.2/tempo120.py
```

### Comparing `tempo120-1.0.0/LICENSE` & `tempo120-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tempo120-1.0.0/PKG-INFO` & `tempo120-1.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tempo120
-Version: 1.0.0
+Version: 1.0.2
 Summary: A party car racing game
 Home-page: https://dkrajzew.itch.io/tempo120
 Download-URL: http://pypi.python.org/pypi/tempo120
 Author: dkrajzew
 Author-email: d.krajzewicz@gmail.com
 License: GPLv3
 Project-URL: Source, https://github.com/dkrajzew/tempo120
@@ -27,16 +27,14 @@
 [![PyPI version](https://badge.fury.io/py/tempo120.svg)](https://pypi.python.org/pypi/tempo120)
 [![Downloads](https://pepy.tech/badge/tempo120)](https://pepy.tech/project/tempo120)
 [![Downloads](https://static.pepy.tech/badge/tempo120/week)](https://pepy.tech/project/tempo120)
 
 
 A racing game written using Python/pygame during the [bpb](https://www.bpb.de/) ([Bundeszentrale für politische Bildung](https://www.bpb.de/)) [game jam 2023](https://www.bpb.de/veranstaltungen/veranstaltungskalender/518950/bpb-game-jam-2023/). The game jam's topic was mobility.
 
-<img src="./gfx/screenshot1.png" width="40%"/> <img src="./gfx/screenshot3.png" width="40%"/>
-
 You may download an executable version on [itch.io](https://dkrajzew.itch.io/tempo120).
 
 # About
 
 __Tempo120__ is a very simple car racing game. You may control your vehicle using the cursor keys or WASD.
 
 The higher the speed the more difficult it is to control the vehicle. You do not need to accelerate all the time. The speed stays same unless you brake or drive besides the road.
```

### Comparing `tempo120-1.0.0/README.md` & `tempo120-1.0.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -4,16 +4,14 @@
 [![PyPI version](https://badge.fury.io/py/tempo120.svg)](https://pypi.python.org/pypi/tempo120)
 [![Downloads](https://pepy.tech/badge/tempo120)](https://pepy.tech/project/tempo120)
 [![Downloads](https://static.pepy.tech/badge/tempo120/week)](https://pepy.tech/project/tempo120)
 
 
 A racing game written using Python/pygame during the [bpb](https://www.bpb.de/) ([Bundeszentrale für politische Bildung](https://www.bpb.de/)) [game jam 2023](https://www.bpb.de/veranstaltungen/veranstaltungskalender/518950/bpb-game-jam-2023/). The game jam's topic was mobility.
 
-<img src="./gfx/screenshot1.png" width="40%"/> <img src="./gfx/screenshot3.png" width="40%"/>
-
 You may download an executable version on [itch.io](https://dkrajzew.itch.io/tempo120).
 
 # About
 
 __Tempo120__ is a very simple car racing game. You may control your vehicle using the cursor keys or WASD.
 
 The higher the speed the more difficult it is to control the vehicle. You do not need to accelerate all the time. The speed stays same unless you brake or drive besides the road.
```

### Comparing `tempo120-1.0.0/gfx/car.png` & `tempo120-1.0.2/gfx/car.png`

 * *Files identical despite different names*

### Comparing `tempo120-1.0.0/gfx/screenshot1.png` & `tempo120-1.0.2/gfx/screenshot1.png`

 * *Files identical despite different names*

### Comparing `tempo120-1.0.0/gfx/screenshot2.png` & `tempo120-1.0.2/gfx/screenshot2.png`

 * *Files identical despite different names*

### Comparing `tempo120-1.0.0/gfx/screenshot3.png` & `tempo120-1.0.2/gfx/screenshot3.png`

 * *Files identical despite different names*

### Comparing `tempo120-1.0.0/gfx/screenshot4.png` & `tempo120-1.0.2/gfx/screenshot4.png`

 * *Files identical despite different names*

### Comparing `tempo120-1.0.0/gfx/title.png` & `tempo120-1.0.2/gfx/title.png`

 * *Files identical despite different names*

### Comparing `tempo120-1.0.0/gfx/track01.png` & `tempo120-1.0.2/gfx/track01.png`

 * *Files identical despite different names*

### Comparing `tempo120-1.0.0/muzak/engine.ogg` & `tempo120-1.0.2/muzak/engine.ogg`

 * *Files identical despite different names*

### Comparing `tempo120-1.0.0/muzak/track.ogg` & `tempo120-1.0.2/muzak/track.ogg`

 * *Files identical despite different names*

### Comparing `tempo120-1.0.0/setup.py` & `tempo120-1.0.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 # --- definitions ---------------------------------------------------
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="tempo120",
-    version="1.0.0",
+    version="1.0.2",
     author="dkrajzew",
     author_email="d.krajzewicz@gmail.com",
     description="A party car racing game",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://dkrajzew.itch.io/tempo120',
     download_url='http://pypi.python.org/pypi/tempo120',
```

### Comparing `tempo120-1.0.0/tempo120.egg-info/PKG-INFO` & `tempo120-1.0.2/tempo120.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tempo120
-Version: 1.0.0
+Version: 1.0.2
 Summary: A party car racing game
 Home-page: https://dkrajzew.itch.io/tempo120
 Download-URL: http://pypi.python.org/pypi/tempo120
 Author: dkrajzew
 Author-email: d.krajzewicz@gmail.com
 License: GPLv3
 Project-URL: Source, https://github.com/dkrajzew/tempo120
@@ -27,16 +27,14 @@
 [![PyPI version](https://badge.fury.io/py/tempo120.svg)](https://pypi.python.org/pypi/tempo120)
 [![Downloads](https://pepy.tech/badge/tempo120)](https://pepy.tech/project/tempo120)
 [![Downloads](https://static.pepy.tech/badge/tempo120/week)](https://pepy.tech/project/tempo120)
 
 
 A racing game written using Python/pygame during the [bpb](https://www.bpb.de/) ([Bundeszentrale für politische Bildung](https://www.bpb.de/)) [game jam 2023](https://www.bpb.de/veranstaltungen/veranstaltungskalender/518950/bpb-game-jam-2023/). The game jam's topic was mobility.
 
-<img src="./gfx/screenshot1.png" width="40%"/> <img src="./gfx/screenshot3.png" width="40%"/>
-
 You may download an executable version on [itch.io](https://dkrajzew.itch.io/tempo120).
 
 # About
 
 __Tempo120__ is a very simple car racing game. You may control your vehicle using the cursor keys or WASD.
 
 The higher the speed the more difficult it is to control the vehicle. You do not need to accelerate all the time. The speed stays same unless you brake or drive besides the road.
```

### Comparing `tempo120-1.0.0/tempo120.py` & `tempo120-1.0.2/tempo120.py`

 * *Files identical despite different names*

