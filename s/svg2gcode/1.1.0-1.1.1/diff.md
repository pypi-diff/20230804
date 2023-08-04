# Comparing `tmp/svg2gcode-1.1.0.tar.gz` & `tmp/svg2gcode-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "svg2gcode-1.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "svg2gcode-1.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `svg2gcode-1.1.0.tar` & `svg2gcode-1.1.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0    32422 2023-06-11 09:44:38.507409 svg2gcode-1.1.0/LICENSE
--rw-r--r--   0        0        0     3448 2023-06-11 11:11:11.122900 svg2gcode-1.1.0/README.md
--rw-r--r--   0        0        0      702 2023-06-11 13:24:21.470767 svg2gcode-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     3448 2023-06-11 11:17:10.801949 svg2gcode-1.1.0/svg2gcode/README.md
--rw-r--r--   0        0        0       98 2023-07-23 10:21:53.304874 svg2gcode-1.1.0/svg2gcode/__init__.py
--rw-r--r--   0        0        0     4253 2023-06-11 13:20:54.086229 svg2gcode-1.1.0/svg2gcode/__main__.py
--rw-r--r--   0        0        0     8196 2023-06-11 09:52:22.536377 svg2gcode-1.1.0/svg2gcode/svg_to_gcode/.DS_Store
--rw-r--r--   0        0        0     7933 2023-06-11 09:52:22.536377 svg2gcode-1.1.0/svg2gcode/svg_to_gcode/__init__.py
--rw-r--r--   0        0        0      145 2023-06-11 10:12:09.289095 svg2gcode-1.1.0/svg2gcode/svg_to_gcode/compiler/__init__.py
--rw-r--r--   0        0        0    17300 2023-06-11 10:36:56.473595 svg2gcode-1.1.0/svg2gcode/svg_to_gcode/compiler/_compiler.py
--rw-r--r--   0        0        0      249 2023-06-11 10:26:29.844685 svg2gcode-1.1.0/svg2gcode/svg_to_gcode/compiler/interfaces/__init__.py
--rw-r--r--   0        0        0     5468 2023-06-11 09:52:22.546377 svg2gcode-1.1.0/svg2gcode/svg_to_gcode/compiler/interfaces/_abstract_interface.py
--rw-r--r--   0        0        0     1180 2023-06-11 10:27:25.285322 svg2gcode-1.1.0/svg2gcode/svg_to_gcode/compiler/interfaces/_fan_controlled_gcode.py
--rw-r--r--   0        0        0     9041 2023-06-11 10:26:57.364996 svg2gcode-1.1.0/svg2gcode/svg_to_gcode/compiler/interfaces/_gcode.py
--rw-r--r--   0        0        0     5016 2023-06-11 10:29:16.096710 svg2gcode-1.1.0/svg2gcode/svg_to_gcode/formulas.py
--rw-r--r--   0        0        0     1357 2023-06-11 10:15:31.283161 svg2gcode-1.1.0/svg2gcode/svg_to_gcode/geometry/__init__.py
--rw-r--r--   0        0        0     3314 2023-06-11 10:20:54.809706 svg2gcode-1.1.0/svg2gcode/svg_to_gcode/geometry/_abstract_chain.py
--rw-r--r--   0        0        0     3117 2023-06-11 10:20:03.218660 svg2gcode-1.1.0/svg2gcode/svg_to_gcode/geometry/_abstract_curve.py
--rw-r--r--   0        0        0     3066 2023-06-11 10:19:35.908107 svg2gcode-1.1.0/svg2gcode/svg_to_gcode/geometry/_circular_arc.py
--rw-r--r--   0        0        0     1074 2023-06-11 10:19:09.947581 svg2gcode-1.1.0/svg2gcode/svg_to_gcode/geometry/_cubic_bazier.py
--rw-r--r--   0        0        0     2312 2023-06-11 10:18:52.107220 svg2gcode-1.1.0/svg2gcode/svg_to_gcode/geometry/_elliptical_arc.py
--rw-r--r--   0        0        0      918 2023-06-11 10:17:51.856001 svg2gcode-1.1.0/svg2gcode/svg_to_gcode/geometry/_line.py
--rw-r--r--   0        0        0     3272 2023-06-11 10:18:20.966590 svg2gcode-1.1.0/svg2gcode/svg_to_gcode/geometry/_line_segment_chain.py
--rw-r--r--   0        0        0     3171 2023-06-11 10:17:08.525125 svg2gcode-1.1.0/svg2gcode/svg_to_gcode/geometry/_matrix.py
--rw-r--r--   0        0        0      963 2023-06-11 10:21:55.460936 svg2gcode-1.1.0/svg2gcode/svg_to_gcode/geometry/_quadratic_bazier.py
--rw-r--r--   0        0        0     1095 2023-06-11 10:16:36.264473 svg2gcode-1.1.0/svg2gcode/svg_to_gcode/geometry/_raster_image.py
--rw-r--r--   0        0        0     2487 2023-06-11 10:21:34.210505 svg2gcode-1.1.0/svg2gcode/svg_to_gcode/geometry/_smooth_arc_chain.py
--rw-r--r--   0        0        0     1498 2023-06-11 09:52:22.566377 svg2gcode-1.1.0/svg2gcode/svg_to_gcode/geometry/_vector.py
--rw-r--r--   0        0        0      601 2023-06-11 10:22:45.041942 svg2gcode-1.1.0/svg2gcode/svg_to_gcode/svg_parser/__init__.py
--rw-r--r--   0        0        0    10578 2023-07-23 10:07:16.010830 svg2gcode-1.1.0/svg2gcode/svg_to_gcode/svg_parser/_parser_methods.py
--rw-r--r--   0        0        0    13401 2023-06-11 10:23:12.132492 svg2gcode-1.1.0/svg2gcode/svg_to_gcode/svg_parser/_path.py
--rw-r--r--   0        0        0     5577 2023-06-11 10:23:46.893089 svg2gcode-1.1.0/svg2gcode/svg_to_gcode/svg_parser/_transformation.py
--rw-r--r--   0        0        0     2440 2023-06-11 10:24:16.853348 svg2gcode-1.1.0/svg2gcode/svg_to_gcode/svg_parser/debug_methods.py
--rw-r--r--   0        0        0     4007 1970-01-01 00:00:00.000000 svg2gcode-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0    32422 2023-06-11 09:44:38.507409 svg2gcode-1.1.1/LICENSE
+-rw-r--r--   0        0        0     3448 2023-06-11 11:11:11.122900 svg2gcode-1.1.1/README.md
+-rw-r--r--   0        0        0      702 2023-06-11 13:24:21.470767 svg2gcode-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3448 2023-06-11 11:17:10.801949 svg2gcode-1.1.1/svg2gcode/README.md
+-rw-r--r--   0        0        0       98 2023-08-04 21:17:57.591838 svg2gcode-1.1.1/svg2gcode/__init__.py
+-rw-r--r--   0        0        0     4255 2023-08-04 21:17:44.181565 svg2gcode-1.1.1/svg2gcode/__main__.py
+-rw-r--r--   0        0        0     8196 2023-06-11 09:52:22.536377 svg2gcode-1.1.1/svg2gcode/svg_to_gcode/.DS_Store
+-rw-r--r--   0        0        0     7933 2023-06-11 09:52:22.536377 svg2gcode-1.1.1/svg2gcode/svg_to_gcode/__init__.py
+-rw-r--r--   0        0        0      145 2023-06-11 10:12:09.289095 svg2gcode-1.1.1/svg2gcode/svg_to_gcode/compiler/__init__.py
+-rw-r--r--   0        0        0    17300 2023-06-11 10:36:56.473595 svg2gcode-1.1.1/svg2gcode/svg_to_gcode/compiler/_compiler.py
+-rw-r--r--   0        0        0      249 2023-06-11 10:26:29.844685 svg2gcode-1.1.1/svg2gcode/svg_to_gcode/compiler/interfaces/__init__.py
+-rw-r--r--   0        0        0     5468 2023-06-11 09:52:22.546377 svg2gcode-1.1.1/svg2gcode/svg_to_gcode/compiler/interfaces/_abstract_interface.py
+-rw-r--r--   0        0        0     1180 2023-06-11 10:27:25.285322 svg2gcode-1.1.1/svg2gcode/svg_to_gcode/compiler/interfaces/_fan_controlled_gcode.py
+-rw-r--r--   0        0        0     9041 2023-06-11 10:26:57.364996 svg2gcode-1.1.1/svg2gcode/svg_to_gcode/compiler/interfaces/_gcode.py
+-rw-r--r--   0        0        0     5016 2023-06-11 10:29:16.096710 svg2gcode-1.1.1/svg2gcode/svg_to_gcode/formulas.py
+-rw-r--r--   0        0        0     1357 2023-06-11 10:15:31.283161 svg2gcode-1.1.1/svg2gcode/svg_to_gcode/geometry/__init__.py
+-rw-r--r--   0        0        0     3314 2023-06-11 10:20:54.809706 svg2gcode-1.1.1/svg2gcode/svg_to_gcode/geometry/_abstract_chain.py
+-rw-r--r--   0        0        0     3117 2023-06-11 10:20:03.218660 svg2gcode-1.1.1/svg2gcode/svg_to_gcode/geometry/_abstract_curve.py
+-rw-r--r--   0        0        0     3066 2023-06-11 10:19:35.908107 svg2gcode-1.1.1/svg2gcode/svg_to_gcode/geometry/_circular_arc.py
+-rw-r--r--   0        0        0     1074 2023-06-11 10:19:09.947581 svg2gcode-1.1.1/svg2gcode/svg_to_gcode/geometry/_cubic_bazier.py
+-rw-r--r--   0        0        0     2312 2023-06-11 10:18:52.107220 svg2gcode-1.1.1/svg2gcode/svg_to_gcode/geometry/_elliptical_arc.py
+-rw-r--r--   0        0        0      918 2023-06-11 10:17:51.856001 svg2gcode-1.1.1/svg2gcode/svg_to_gcode/geometry/_line.py
+-rw-r--r--   0        0        0     3272 2023-06-11 10:18:20.966590 svg2gcode-1.1.1/svg2gcode/svg_to_gcode/geometry/_line_segment_chain.py
+-rw-r--r--   0        0        0     3171 2023-06-11 10:17:08.525125 svg2gcode-1.1.1/svg2gcode/svg_to_gcode/geometry/_matrix.py
+-rw-r--r--   0        0        0      963 2023-06-11 10:21:55.460936 svg2gcode-1.1.1/svg2gcode/svg_to_gcode/geometry/_quadratic_bazier.py
+-rw-r--r--   0        0        0     1095 2023-06-11 10:16:36.264473 svg2gcode-1.1.1/svg2gcode/svg_to_gcode/geometry/_raster_image.py
+-rw-r--r--   0        0        0     2487 2023-06-11 10:21:34.210505 svg2gcode-1.1.1/svg2gcode/svg_to_gcode/geometry/_smooth_arc_chain.py
+-rw-r--r--   0        0        0     1498 2023-06-11 09:52:22.566377 svg2gcode-1.1.1/svg2gcode/svg_to_gcode/geometry/_vector.py
+-rw-r--r--   0        0        0      601 2023-06-11 10:22:45.041942 svg2gcode-1.1.1/svg2gcode/svg_to_gcode/svg_parser/__init__.py
+-rw-r--r--   0        0        0    10578 2023-07-23 10:07:16.010830 svg2gcode-1.1.1/svg2gcode/svg_to_gcode/svg_parser/_parser_methods.py
+-rw-r--r--   0        0        0    13401 2023-06-11 10:23:12.132492 svg2gcode-1.1.1/svg2gcode/svg_to_gcode/svg_parser/_path.py
+-rw-r--r--   0        0        0     5577 2023-06-11 10:23:46.893089 svg2gcode-1.1.1/svg2gcode/svg_to_gcode/svg_parser/_transformation.py
+-rw-r--r--   0        0        0     2440 2023-06-11 10:24:16.853348 svg2gcode-1.1.1/svg2gcode/svg_to_gcode/svg_parser/debug_methods.py
+-rw-r--r--   0        0        0     4007 1970-01-01 00:00:00.000000 svg2gcode-1.1.1/PKG-INFO
```

### Comparing `svg2gcode-1.1.0/LICENSE` & `svg2gcode-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `svg2gcode-1.1.0/README.md` & `svg2gcode-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `svg2gcode-1.1.0/pyproject.toml` & `svg2gcode-1.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `svg2gcode-1.1.0/svg2gcode/README.md` & `svg2gcode-1.1.1/svg2gcode/README.md`

 * *Files identical despite different names*

### Comparing `svg2gcode-1.1.0/svg2gcode/__main__.py` & `svg2gcode-1.1.1/svg2gcode/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,15 @@
     parser.add_argument('--imagespeed', default=imagespeed_default, metavar="<default:" + str(imagespeed_default)+">",
         type=int, help='image draw speed in mm/min')
     parser.add_argument('--cuttingspeed', default=cuttingspeed_default, metavar="<default:" + str(cuttingspeed_default)+">",
         type=int, help='cutting speed in mm/min')
     parser.add_argument('--imagepower', default=imagepower_default, metavar="<default:" +str(imagepower_default)+ ">",
         type=int, help="maximum laser power while drawing an image (as a rule of thumb set to 1/3 of the machine maximum)")
     parser.add_argument('--cuttingpower', default=cuttingpower_default, metavar="<default:" +str(cuttingpower_default)+ ">",
-        type=int, help="percentage of maximum laser power for line drawings/cutting")
+        type=float, help="percentage of maximum laser power for line drawings/cutting")
     parser.add_argument('--maxlaserpower', default=maxlaserpower_default, metavar="<default:" +str(maxlaserpower_default)+ ">",
         type=int, help="maximum laser power of laser cutter")
     parser.add_argument('--rapidmove', action='store_true', default=True, help='generate inbetween G0 moves' )
     parser.add_argument('--xmaxtravel', default=xmaxtravel_default, metavar="<default:" +str(xmaxtravel_default)+ ">",
         type=int, help="machine x-axis lengh in mm")
     parser.add_argument('--ymaxtravel', default=ymaxtravel_default, metavar="<default:" +str(ymaxtravel_default)+ ">",
         type=int, help="machine y-axis lengh in mm")
```

### Comparing `svg2gcode-1.1.0/svg2gcode/svg_to_gcode/.DS_Store` & `svg2gcode-1.1.1/svg2gcode/svg_to_gcode/.DS_Store`

 * *Files identical despite different names*

### Comparing `svg2gcode-1.1.0/svg2gcode/svg_to_gcode/__init__.py` & `svg2gcode-1.1.1/svg2gcode/svg_to_gcode/__init__.py`

 * *Files identical despite different names*

### Comparing `svg2gcode-1.1.0/svg2gcode/svg_to_gcode/compiler/_compiler.py` & `svg2gcode-1.1.1/svg2gcode/svg_to_gcode/compiler/_compiler.py`

 * *Files identical despite different names*

### Comparing `svg2gcode-1.1.0/svg2gcode/svg_to_gcode/compiler/interfaces/_abstract_interface.py` & `svg2gcode-1.1.1/svg2gcode/svg_to_gcode/compiler/interfaces/_abstract_interface.py`

 * *Files identical despite different names*

### Comparing `svg2gcode-1.1.0/svg2gcode/svg_to_gcode/compiler/interfaces/_fan_controlled_gcode.py` & `svg2gcode-1.1.1/svg2gcode/svg_to_gcode/compiler/interfaces/_fan_controlled_gcode.py`

 * *Files identical despite different names*

### Comparing `svg2gcode-1.1.0/svg2gcode/svg_to_gcode/compiler/interfaces/_gcode.py` & `svg2gcode-1.1.1/svg2gcode/svg_to_gcode/compiler/interfaces/_gcode.py`

 * *Files identical despite different names*

### Comparing `svg2gcode-1.1.0/svg2gcode/svg_to_gcode/formulas.py` & `svg2gcode-1.1.1/svg2gcode/svg_to_gcode/formulas.py`

 * *Files identical despite different names*

### Comparing `svg2gcode-1.1.0/svg2gcode/svg_to_gcode/geometry/__init__.py` & `svg2gcode-1.1.1/svg2gcode/svg_to_gcode/geometry/__init__.py`

 * *Files identical despite different names*

### Comparing `svg2gcode-1.1.0/svg2gcode/svg_to_gcode/geometry/_abstract_chain.py` & `svg2gcode-1.1.1/svg2gcode/svg_to_gcode/geometry/_abstract_chain.py`

 * *Files identical despite different names*

### Comparing `svg2gcode-1.1.0/svg2gcode/svg_to_gcode/geometry/_abstract_curve.py` & `svg2gcode-1.1.1/svg2gcode/svg_to_gcode/geometry/_abstract_curve.py`

 * *Files identical despite different names*

### Comparing `svg2gcode-1.1.0/svg2gcode/svg_to_gcode/geometry/_circular_arc.py` & `svg2gcode-1.1.1/svg2gcode/svg_to_gcode/geometry/_circular_arc.py`

 * *Files identical despite different names*

### Comparing `svg2gcode-1.1.0/svg2gcode/svg_to_gcode/geometry/_cubic_bazier.py` & `svg2gcode-1.1.1/svg2gcode/svg_to_gcode/geometry/_cubic_bazier.py`

 * *Files identical despite different names*

### Comparing `svg2gcode-1.1.0/svg2gcode/svg_to_gcode/geometry/_elliptical_arc.py` & `svg2gcode-1.1.1/svg2gcode/svg_to_gcode/geometry/_elliptical_arc.py`

 * *Files identical despite different names*

### Comparing `svg2gcode-1.1.0/svg2gcode/svg_to_gcode/geometry/_line.py` & `svg2gcode-1.1.1/svg2gcode/svg_to_gcode/geometry/_line.py`

 * *Files identical despite different names*

### Comparing `svg2gcode-1.1.0/svg2gcode/svg_to_gcode/geometry/_line_segment_chain.py` & `svg2gcode-1.1.1/svg2gcode/svg_to_gcode/geometry/_line_segment_chain.py`

 * *Files identical despite different names*

### Comparing `svg2gcode-1.1.0/svg2gcode/svg_to_gcode/geometry/_matrix.py` & `svg2gcode-1.1.1/svg2gcode/svg_to_gcode/geometry/_matrix.py`

 * *Files identical despite different names*

### Comparing `svg2gcode-1.1.0/svg2gcode/svg_to_gcode/geometry/_quadratic_bazier.py` & `svg2gcode-1.1.1/svg2gcode/svg_to_gcode/geometry/_quadratic_bazier.py`

 * *Files identical despite different names*

### Comparing `svg2gcode-1.1.0/svg2gcode/svg_to_gcode/geometry/_raster_image.py` & `svg2gcode-1.1.1/svg2gcode/svg_to_gcode/geometry/_raster_image.py`

 * *Files identical despite different names*

### Comparing `svg2gcode-1.1.0/svg2gcode/svg_to_gcode/geometry/_smooth_arc_chain.py` & `svg2gcode-1.1.1/svg2gcode/svg_to_gcode/geometry/_smooth_arc_chain.py`

 * *Files identical despite different names*

### Comparing `svg2gcode-1.1.0/svg2gcode/svg_to_gcode/geometry/_vector.py` & `svg2gcode-1.1.1/svg2gcode/svg_to_gcode/geometry/_vector.py`

 * *Files identical despite different names*

### Comparing `svg2gcode-1.1.0/svg2gcode/svg_to_gcode/svg_parser/__init__.py` & `svg2gcode-1.1.1/svg2gcode/svg_to_gcode/svg_parser/__init__.py`

 * *Files identical despite different names*

### Comparing `svg2gcode-1.1.0/svg2gcode/svg_to_gcode/svg_parser/_parser_methods.py` & `svg2gcode-1.1.1/svg2gcode/svg_to_gcode/svg_parser/_parser_methods.py`

 * *Files identical despite different names*

### Comparing `svg2gcode-1.1.0/svg2gcode/svg_to_gcode/svg_parser/_path.py` & `svg2gcode-1.1.1/svg2gcode/svg_to_gcode/svg_parser/_path.py`

 * *Files identical despite different names*

### Comparing `svg2gcode-1.1.0/svg2gcode/svg_to_gcode/svg_parser/_transformation.py` & `svg2gcode-1.1.1/svg2gcode/svg_to_gcode/svg_parser/_transformation.py`

 * *Files identical despite different names*

### Comparing `svg2gcode-1.1.0/svg2gcode/svg_to_gcode/svg_parser/debug_methods.py` & `svg2gcode-1.1.1/svg2gcode/svg_to_gcode/svg_parser/debug_methods.py`

 * *Files identical despite different names*

### Comparing `svg2gcode-1.1.0/PKG-INFO` & `svg2gcode-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: svg2gcode
-Version: 1.1.0
+Version: 1.1.1
 Summary: svg2gcode: convert an SVG (Scalable Vector Graphic) image to gcode.
 Keywords: scalable vector graphics,svg,image,laser cutter,laser engraving
 Author-email: Johannes Noordanus <mailjohannes.mailnoordanus@gmail.com>
 Requires-Python: >=3.10.6
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Requires-Dist: numpy >= 1.24.3
```

