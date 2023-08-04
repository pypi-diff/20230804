# Comparing `tmp/linkpreview-0.6.5.tar.gz` & `tmp/linkpreview-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linkpreview-0.6.5.tar", last modified: Thu Apr  6 21:17:18 2023, max compression
+gzip compressed data, was "linkpreview-0.7.0.tar", last modified: Fri Aug  4 03:04:53 2023, max compression
```

## Comparing `linkpreview-0.6.5.tar` & `linkpreview-0.7.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 21:17:18.970196 linkpreview-0.6.5/
--rw-r--r--   0 runner    (1001) docker     (122)     1062 2023-04-06 21:16:48.000000 linkpreview-0.6.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     4576 2023-04-06 21:17:18.970196 linkpreview-0.6.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2906 2023-04-06 21:16:48.000000 linkpreview-0.6.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 21:17:18.970196 linkpreview-0.6.5/linkpreview/
--rw-r--r--   0 runner    (1001) docker     (122)      275 2023-04-06 21:16:48.000000 linkpreview-0.6.5/linkpreview/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      512 2023-04-06 21:16:48.000000 linkpreview-0.6.5/linkpreview/compose.py
--rw-r--r--   0 runner    (1001) docker     (122)      231 2023-04-06 21:16:48.000000 linkpreview-0.6.5/linkpreview/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     2254 2023-04-06 21:16:48.000000 linkpreview-0.6.5/linkpreview/grabber.py
--rw-r--r--   0 runner    (1001) docker     (122)      962 2023-04-06 21:16:48.000000 linkpreview-0.6.5/linkpreview/helpers.py
--rw-r--r--   0 runner    (1001) docker     (122)     1068 2023-04-06 21:16:48.000000 linkpreview-0.6.5/linkpreview/link.py
--rw-r--r--   0 runner    (1001) docker     (122)     2388 2023-04-06 21:16:48.000000 linkpreview-0.6.5/linkpreview/linkpreview.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 21:17:18.970196 linkpreview-0.6.5/linkpreview/preview/
--rw-r--r--   0 runner    (1001) docker     (122)      242 2023-04-06 21:16:48.000000 linkpreview-0.6.5/linkpreview/preview/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      511 2023-04-06 21:16:48.000000 linkpreview-0.6.5/linkpreview/preview/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     1894 2023-04-06 21:16:48.000000 linkpreview-0.6.5/linkpreview/preview/generic.py
--rw-r--r--   0 runner    (1001) docker     (122)     1002 2023-04-06 21:16:48.000000 linkpreview-0.6.5/linkpreview/preview/jsonld.py
--rw-r--r--   0 runner    (1001) docker     (122)      455 2023-04-06 21:16:48.000000 linkpreview-0.6.5/linkpreview/preview/metabase.py
--rw-r--r--   0 runner    (1001) docker     (122)     1190 2023-04-06 21:16:48.000000 linkpreview-0.6.5/linkpreview/preview/microdata.py
--rw-r--r--   0 runner    (1001) docker     (122)      596 2023-04-06 21:16:48.000000 linkpreview-0.6.5/linkpreview/preview/opengraph.py
--rw-r--r--   0 runner    (1001) docker     (122)     1356 2023-04-06 21:16:48.000000 linkpreview-0.6.5/linkpreview/preview/schemabase.py
--rw-r--r--   0 runner    (1001) docker     (122)      601 2023-04-06 21:16:48.000000 linkpreview-0.6.5/linkpreview/preview/twittercard.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 21:17:18.970196 linkpreview-0.6.5/linkpreview.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     4576 2023-04-06 21:17:18.000000 linkpreview-0.6.5/linkpreview.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      654 2023-04-06 21:17:18.000000 linkpreview-0.6.5/linkpreview.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-06 21:17:18.000000 linkpreview-0.6.5/linkpreview.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       39 2023-04-06 21:17:18.000000 linkpreview-0.6.5/linkpreview.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       12 2023-04-06 21:17:18.000000 linkpreview-0.6.5/linkpreview.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-06 21:17:18.970196 linkpreview-0.6.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1290 2023-04-06 21:16:48.000000 linkpreview-0.6.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 03:04:53.392225 linkpreview-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     1062 2023-08-04 03:04:23.000000 linkpreview-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     4576 2023-08-04 03:04:53.392225 linkpreview-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2906 2023-08-04 03:04:23.000000 linkpreview-0.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 03:04:53.392225 linkpreview-0.7.0/linkpreview/
+-rw-r--r--   0 runner    (1001) docker     (122)      275 2023-08-04 03:04:23.000000 linkpreview-0.7.0/linkpreview/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      512 2023-08-04 03:04:23.000000 linkpreview-0.7.0/linkpreview/compose.py
+-rw-r--r--   0 runner    (1001) docker     (122)      231 2023-08-04 03:04:23.000000 linkpreview-0.7.0/linkpreview/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2254 2023-08-04 03:04:23.000000 linkpreview-0.7.0/linkpreview/grabber.py
+-rw-r--r--   0 runner    (1001) docker     (122)      962 2023-08-04 03:04:23.000000 linkpreview-0.7.0/linkpreview/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1068 2023-08-04 03:04:23.000000 linkpreview-0.7.0/linkpreview/link.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2673 2023-08-04 03:04:23.000000 linkpreview-0.7.0/linkpreview/linkpreview.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 03:04:53.392225 linkpreview-0.7.0/linkpreview/preview/
+-rw-r--r--   0 runner    (1001) docker     (122)      242 2023-08-04 03:04:23.000000 linkpreview-0.7.0/linkpreview/preview/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      511 2023-08-04 03:04:23.000000 linkpreview-0.7.0/linkpreview/preview/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1894 2023-08-04 03:04:23.000000 linkpreview-0.7.0/linkpreview/preview/generic.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1002 2023-08-04 03:04:23.000000 linkpreview-0.7.0/linkpreview/preview/jsonld.py
+-rw-r--r--   0 runner    (1001) docker     (122)      455 2023-08-04 03:04:23.000000 linkpreview-0.7.0/linkpreview/preview/metabase.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1190 2023-08-04 03:04:23.000000 linkpreview-0.7.0/linkpreview/preview/microdata.py
+-rw-r--r--   0 runner    (1001) docker     (122)      596 2023-08-04 03:04:23.000000 linkpreview-0.7.0/linkpreview/preview/opengraph.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1356 2023-08-04 03:04:23.000000 linkpreview-0.7.0/linkpreview/preview/schemabase.py
+-rw-r--r--   0 runner    (1001) docker     (122)      601 2023-08-04 03:04:23.000000 linkpreview-0.7.0/linkpreview/preview/twittercard.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 03:04:53.392225 linkpreview-0.7.0/linkpreview.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     4576 2023-08-04 03:04:53.000000 linkpreview-0.7.0/linkpreview.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      654 2023-08-04 03:04:53.000000 linkpreview-0.7.0/linkpreview.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-04 03:04:53.000000 linkpreview-0.7.0/linkpreview.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       39 2023-08-04 03:04:53.000000 linkpreview-0.7.0/linkpreview.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2023-08-04 03:04:53.000000 linkpreview-0.7.0/linkpreview.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-08-04 03:04:53.392225 linkpreview-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1290 2023-08-04 03:04:23.000000 linkpreview-0.7.0/setup.py
```

### Comparing `linkpreview-0.6.5/LICENSE` & `linkpreview-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `linkpreview-0.6.5/PKG-INFO` & `linkpreview-0.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linkpreview
-Version: 0.6.5
+Version: 0.7.0
 Summary: Get link (URL) preview
 Home-page: UNKNOWN
 Author: MeyT
 License: MIT
 Description: # linkpreview
         
         [![Build Status](https://github.com/meyt/linkpreview/actions/workflows/main.yaml/badge.svg)](https://github.com/meyt/linkpreview/actions)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: linkpreview Version: 0.6.5 Summary: Get link (URL)
+Metadata-Version: 2.1 Name: linkpreview Version: 0.7.0 Summary: Get link (URL)
 preview Home-page: UNKNOWN Author: MeyT License: MIT Description: # linkpreview
 [![Build Status](https://github.com/meyt/linkpreview/actions/workflows/
 main.yaml/badge.svg)](https://github.com/meyt/linkpreview/actions) [![Coverage
 Status](https://coveralls.io/repos/github/meyt/linkpreview/
 badge.svg?branch=master)](https://coveralls.io/github/meyt/
 linkpreview?branch=master) [![pypi](https://img.shields.io/pypi/pyversions/
 linkpreview.svg)](https://pypi.python.org/pypi/linkpreview) Get link preview in
```

### Comparing `linkpreview-0.6.5/README.md` & `linkpreview-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `linkpreview-0.6.5/linkpreview/compose.py` & `linkpreview-0.7.0/linkpreview/compose.py`

 * *Files identical despite different names*

### Comparing `linkpreview-0.6.5/linkpreview/grabber.py` & `linkpreview-0.7.0/linkpreview/grabber.py`

 * *Files identical despite different names*

### Comparing `linkpreview-0.6.5/linkpreview/helpers.py` & `linkpreview-0.7.0/linkpreview/helpers.py`

 * *Files identical despite different names*

### Comparing `linkpreview-0.6.5/linkpreview/link.py` & `linkpreview-0.7.0/linkpreview/link.py`

 * *Files identical despite different names*

### Comparing `linkpreview-0.6.5/linkpreview/linkpreview.py` & `linkpreview-0.7.0/linkpreview/linkpreview.py`

 * *Files 7% similar despite different names*

```diff
@@ -84,7 +84,17 @@
             exploded = self.link.path.split("/")[-1].split(".")
             if len(exploded) > 1:
                 return titleize(".".join(exploded[:-1]))
 
         link = self.link.copy()
         link.netloc = link.netloc.split("@")[-1]
         return link.url[len(self.link.scheme) + 3 :]
+
+    def to_dict(self):
+        return dict(
+            site_name=self.site_name,
+            title=self.title,
+            description=self.description,
+            image=self.image,
+            absolute_image=self.absolute_image,
+            force_title=self.force_title,
+        )
```

### Comparing `linkpreview-0.6.5/linkpreview/preview/generic.py` & `linkpreview-0.7.0/linkpreview/preview/generic.py`

 * *Files identical despite different names*

### Comparing `linkpreview-0.6.5/linkpreview/preview/jsonld.py` & `linkpreview-0.7.0/linkpreview/preview/jsonld.py`

 * *Files identical despite different names*

### Comparing `linkpreview-0.6.5/linkpreview/preview/microdata.py` & `linkpreview-0.7.0/linkpreview/preview/microdata.py`

 * *Files identical despite different names*

### Comparing `linkpreview-0.6.5/linkpreview/preview/opengraph.py` & `linkpreview-0.7.0/linkpreview/preview/opengraph.py`

 * *Files identical despite different names*

### Comparing `linkpreview-0.6.5/linkpreview/preview/schemabase.py` & `linkpreview-0.7.0/linkpreview/preview/schemabase.py`

 * *Files identical despite different names*

### Comparing `linkpreview-0.6.5/linkpreview/preview/twittercard.py` & `linkpreview-0.7.0/linkpreview/preview/twittercard.py`

 * *Files identical despite different names*

### Comparing `linkpreview-0.6.5/linkpreview.egg-info/PKG-INFO` & `linkpreview-0.7.0/linkpreview.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linkpreview
-Version: 0.6.5
+Version: 0.7.0
 Summary: Get link (URL) preview
 Home-page: UNKNOWN
 Author: MeyT
 License: MIT
 Description: # linkpreview
         
         [![Build Status](https://github.com/meyt/linkpreview/actions/workflows/main.yaml/badge.svg)](https://github.com/meyt/linkpreview/actions)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: linkpreview Version: 0.6.5 Summary: Get link (URL)
+Metadata-Version: 2.1 Name: linkpreview Version: 0.7.0 Summary: Get link (URL)
 preview Home-page: UNKNOWN Author: MeyT License: MIT Description: # linkpreview
 [![Build Status](https://github.com/meyt/linkpreview/actions/workflows/
 main.yaml/badge.svg)](https://github.com/meyt/linkpreview/actions) [![Coverage
 Status](https://coveralls.io/repos/github/meyt/linkpreview/
 badge.svg?branch=master)](https://coveralls.io/github/meyt/
 linkpreview?branch=master) [![pypi](https://img.shields.io/pypi/pyversions/
 linkpreview.svg)](https://pypi.python.org/pypi/linkpreview) Get link preview in
```

### Comparing `linkpreview-0.6.5/linkpreview.egg-info/SOURCES.txt` & `linkpreview-0.7.0/linkpreview.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `linkpreview-0.6.5/setup.py` & `linkpreview-0.7.0/setup.py`

 * *Files identical despite different names*

