# Comparing `tmp/willow-1.6.tar.gz` & `tmp/willow-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "willow-1.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "willow-1.6.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `willow-1.6.tar` & `willow-1.6.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1545 2023-07-13 18:09:19.277441 willow-1.6/LICENSE
--rw-r--r--   0        0        0      101 2023-07-13 18:09:19.281442 willow-1.6/MANIFEST.in
--rw-r--r--   0        0        0     3686 2023-07-13 18:09:19.281442 willow-1.6/README.md
--rw-r--r--   0        0        0     2810 2023-07-13 18:09:19.281442 willow-1.6/pyproject.toml
--rw-r--r--   0        0        0     1703 2023-07-13 18:09:19.297442 willow-1.6/willow/__init__.py
--rw-r--r--   0        0        0   837462 2023-07-13 18:09:19.301442 willow-1.6/willow/data/cascades/haarcascade_frontalface_alt2.xml
--rw-r--r--   0        0        0     9210 2023-07-13 18:09:19.301442 willow-1.6/willow/image.py
--rw-r--r--   0        0        0      219 2023-07-13 18:09:19.301442 willow-1.6/willow/optimizers/__init__.py
--rw-r--r--   0        0        0     1615 2023-07-13 18:09:19.301442 willow-1.6/willow/optimizers/base.py
--rw-r--r--   0        0        0      947 2023-07-13 18:09:19.301442 willow-1.6/willow/optimizers/cwebp.py
--rw-r--r--   0        0        0      508 2023-07-13 18:09:19.301442 willow-1.6/willow/optimizers/gifsicle.py
--rw-r--r--   0        0        0      600 2023-07-13 18:09:19.301442 willow-1.6/willow/optimizers/jpegoptim.py
--rw-r--r--   0        0        0      535 2023-07-13 18:09:19.301442 willow-1.6/willow/optimizers/optipng.py
--rw-r--r--   0        0        0      648 2023-07-13 18:09:19.301442 willow-1.6/willow/optimizers/pngquant.py
--rw-r--r--   0        0        0        0 2023-07-13 18:09:19.301442 willow-1.6/willow/plugins/__init__.py
--rw-r--r--   0        0        0     3787 2023-07-13 18:09:19.301442 willow-1.6/willow/plugins/opencv.py
--rw-r--r--   0        0        0    12289 2023-07-13 18:09:19.301442 willow-1.6/willow/plugins/pillow.py
--rw-r--r--   0        0        0     9276 2023-07-13 18:09:19.301442 willow-1.6/willow/plugins/wand.py
--rw-r--r--   0        0        0    15273 2023-07-13 18:09:19.301442 willow-1.6/willow/registry.py
--rw-r--r--   0        0        0    11803 2023-07-13 18:09:19.301442 willow-1.6/willow/svg.py
--rw-r--r--   0        0        0        0 2023-07-13 18:09:19.301442 willow-1.6/willow/utils/__init__.py
--rw-r--r--   0        0        0       61 2023-07-13 18:09:19.301442 willow-1.6/willow/utils/deprecation.py
--rw-r--r--   0        0        0     5601 1970-01-01 00:00:00.000000 willow-1.6/PKG-INFO
+-rw-r--r--   0        0        0     1545 2023-08-04 15:45:43.523447 willow-1.6.1/LICENSE
+-rw-r--r--   0        0        0      101 2023-08-04 15:45:43.523447 willow-1.6.1/MANIFEST.in
+-rw-r--r--   0        0        0     3686 2023-08-04 15:45:43.523447 willow-1.6.1/README.md
+-rw-r--r--   0        0        0     2810 2023-08-04 15:45:43.523447 willow-1.6.1/pyproject.toml
+-rw-r--r--   0        0        0     1705 2023-08-04 15:45:43.547447 willow-1.6.1/willow/__init__.py
+-rw-r--r--   0        0        0   837462 2023-08-04 15:45:43.551447 willow-1.6.1/willow/data/cascades/haarcascade_frontalface_alt2.xml
+-rw-r--r--   0        0        0     9210 2023-08-04 15:45:43.551447 willow-1.6.1/willow/image.py
+-rw-r--r--   0        0        0      219 2023-08-04 15:45:43.551447 willow-1.6.1/willow/optimizers/__init__.py
+-rw-r--r--   0        0        0     1615 2023-08-04 15:45:43.551447 willow-1.6.1/willow/optimizers/base.py
+-rw-r--r--   0        0        0      947 2023-08-04 15:45:43.551447 willow-1.6.1/willow/optimizers/cwebp.py
+-rw-r--r--   0        0        0      508 2023-08-04 15:45:43.551447 willow-1.6.1/willow/optimizers/gifsicle.py
+-rw-r--r--   0        0        0      600 2023-08-04 15:45:43.551447 willow-1.6.1/willow/optimizers/jpegoptim.py
+-rw-r--r--   0        0        0      535 2023-08-04 15:45:43.551447 willow-1.6.1/willow/optimizers/optipng.py
+-rw-r--r--   0        0        0      648 2023-08-04 15:45:43.551447 willow-1.6.1/willow/optimizers/pngquant.py
+-rw-r--r--   0        0        0        0 2023-08-04 15:45:43.551447 willow-1.6.1/willow/plugins/__init__.py
+-rw-r--r--   0        0        0     3787 2023-08-04 15:45:43.551447 willow-1.6.1/willow/plugins/opencv.py
+-rw-r--r--   0        0        0    12289 2023-08-04 15:45:43.551447 willow-1.6.1/willow/plugins/pillow.py
+-rw-r--r--   0        0        0     9276 2023-08-04 15:45:43.551447 willow-1.6.1/willow/plugins/wand.py
+-rw-r--r--   0        0        0    15273 2023-08-04 15:45:43.551447 willow-1.6.1/willow/registry.py
+-rw-r--r--   0        0        0    11884 2023-08-04 15:45:43.551447 willow-1.6.1/willow/svg.py
+-rw-r--r--   0        0        0        0 2023-08-04 15:45:43.551447 willow-1.6.1/willow/utils/__init__.py
+-rw-r--r--   0        0        0       61 2023-08-04 15:45:43.551447 willow-1.6.1/willow/utils/deprecation.py
+-rw-r--r--   0        0        0     5603 1970-01-01 00:00:00.000000 willow-1.6.1/PKG-INFO
```

### Comparing `willow-1.6/LICENSE` & `willow-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `willow-1.6/README.md` & `willow-1.6.1/README.md`

 * *Files identical despite different names*

### Comparing `willow-1.6/pyproject.toml` & `willow-1.6.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `willow-1.6/willow/__init__.py` & `willow-1.6.1/willow/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,8 +49,8 @@
     # namespaces, e.g. "<ns0:svg ..."
     ElementTree.register_namespace("", "http://www.w3.org/2000/svg")
 
 
 setup()
 
 
-__version__ = "1.6"
+__version__ = "1.6.1"
```

### Comparing `willow-1.6/willow/data/cascades/haarcascade_frontalface_alt2.xml` & `willow-1.6.1/willow/data/cascades/haarcascade_frontalface_alt2.xml`

 * *Files identical despite different names*

### Comparing `willow-1.6/willow/image.py` & `willow-1.6.1/willow/image.py`

 * *Files identical despite different names*

### Comparing `willow-1.6/willow/optimizers/base.py` & `willow-1.6.1/willow/optimizers/base.py`

 * *Files identical despite different names*

### Comparing `willow-1.6/willow/optimizers/cwebp.py` & `willow-1.6.1/willow/optimizers/cwebp.py`

 * *Files identical despite different names*

### Comparing `willow-1.6/willow/optimizers/jpegoptim.py` & `willow-1.6.1/willow/optimizers/jpegoptim.py`

 * *Files identical despite different names*

### Comparing `willow-1.6/willow/optimizers/optipng.py` & `willow-1.6.1/willow/optimizers/optipng.py`

 * *Files identical despite different names*

### Comparing `willow-1.6/willow/optimizers/pngquant.py` & `willow-1.6.1/willow/optimizers/pngquant.py`

 * *Files identical despite different names*

### Comparing `willow-1.6/willow/plugins/opencv.py` & `willow-1.6.1/willow/plugins/opencv.py`

 * *Files identical despite different names*

### Comparing `willow-1.6/willow/plugins/pillow.py` & `willow-1.6.1/willow/plugins/pillow.py`

 * *Files identical despite different names*

### Comparing `willow-1.6/willow/plugins/wand.py` & `willow-1.6.1/willow/plugins/wand.py`

 * *Files identical despite different names*

### Comparing `willow-1.6/willow/registry.py` & `willow-1.6.1/willow/registry.py`

 * *Files identical despite different names*

### Comparing `willow-1.6/willow/svg.py` & `willow-1.6.1/willow/svg.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,17 +113,18 @@
 
 
 class SvgWrapper:
     # https://developer.mozilla.org/en-US/docs/Web/SVG/Content_type#length
     UNIT_RE = re.compile(r"(?:em|ex|px|in|cm|mm|pt|pc|%)$")
 
     # https://www.w3.org/TR/SVG11/types.html#DataTypeNumber
+    # https://www.w3.org/TR/2013/WD-SVG2-20130409/types.html#DataTypeNumber
     # This will exclude some inputs that Python will accept (e.g. "1.e9", "1."),
     # but for integration with other tools, we should adhere to the spec
-    NUMBER_PATTERN = r"([+-]?(?:\d*\.)?\d+(?:[Ee]\d+)?)"
+    NUMBER_PATTERN = r"([+-]?(?:\d*\.)?\d+(?:[Ee][+-]?\d+)?)"
 
     # https://www.w3.org/Graphics/SVG/1.1/coords.html#ViewBoxAttribute
     VIEW_BOX_RE = re.compile(
         rf"^{NUMBER_PATTERN}(?:,\s*|\s+){NUMBER_PATTERN}(?:,\s*|\s+)"
         rf"{NUMBER_PATTERN}(?:,\s*|\s+){NUMBER_PATTERN}$"
     )
```

### Comparing `willow-1.6/PKG-INFO` & `willow-1.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Willow
-Version: 1.6
+Version: 1.6.1
 Summary: A Python image library that sits on top of Pillow, Wand and OpenCV
 Keywords: Imaging
 Author-email: Karl Hobley <karl@kaed.uk>
 Maintainer-email: Wagtail Core team <hello@wagtail.org>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
```

