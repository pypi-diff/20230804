# Comparing `tmp/zarrview-0.1.1.tar.gz` & `tmp/zarrview-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zarrview-0.1.1.tar", last modified: Tue Aug  1 20:15:51 2023, max compression
+gzip compressed data, was "zarrview-0.1.2.tar", last modified: Fri Aug  4 15:46:11 2023, max compression
```

## Comparing `zarrview-0.1.1.tar` & `zarrview-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 marcel     (501) staff       (20)        0 2023-08-01 20:15:51.800491 zarrview-0.1.1/
--rw-r--r--   0 marcel     (501) staff       (20)     1077 2023-07-31 23:47:54.000000 zarrview-0.1.1/LICENSE
--rw-r--r--   0 marcel     (501) staff       (20)     3916 2023-08-01 20:15:51.799972 zarrview-0.1.1/PKG-INFO
--rw-r--r--   0 marcel     (501) staff       (20)     3114 2023-08-01 19:54:02.000000 zarrview-0.1.1/README.md
--rw-r--r--   0 marcel     (501) staff       (20)       38 2023-08-01 20:15:51.800588 zarrview-0.1.1/setup.cfg
--rw-r--r--   0 marcel     (501) staff       (20)     1316 2023-08-01 20:14:16.000000 zarrview-0.1.1/setup.py
-drwxr-xr-x   0 marcel     (501) staff       (20)        0 2023-08-01 20:15:51.797314 zarrview-0.1.1/zarrview/
--rw-------   0 marcel     (501) staff       (20)    50525 2023-08-01 17:00:31.000000 zarrview-0.1.1/zarrview/ZarrViewer.py
--rw-r--r--   0 marcel     (501) staff       (20)        0 2023-07-10 21:49:49.000000 zarrview-0.1.1/zarrview/__init__.py
--rw-r--r--   0 marcel     (501) staff       (20)      423 2023-08-01 18:30:36.000000 zarrview-0.1.1/zarrview/__main__.py
--rw-------   0 marcel     (501) staff       (20)    22926 2023-08-01 16:57:00.000000 zarrview-0.1.1/zarrview/zarr_path_utils.py
-drwxr-xr-x   0 marcel     (501) staff       (20)        0 2023-08-01 20:15:51.799471 zarrview-0.1.1/zarrview.egg-info/
--rw-r--r--   0 marcel     (501) staff       (20)     3916 2023-08-01 20:15:51.000000 zarrview-0.1.1/zarrview.egg-info/PKG-INFO
--rw-r--r--   0 marcel     (501) staff       (20)      278 2023-08-01 20:15:51.000000 zarrview-0.1.1/zarrview.egg-info/SOURCES.txt
--rw-r--r--   0 marcel     (501) staff       (20)        1 2023-08-01 20:15:51.000000 zarrview-0.1.1/zarrview.egg-info/dependency_links.txt
--rw-r--r--   0 marcel     (501) staff       (20)       78 2023-08-01 20:15:51.000000 zarrview-0.1.1/zarrview.egg-info/requires.txt
--rw-r--r--   0 marcel     (501) staff       (20)        9 2023-08-01 20:15:51.000000 zarrview-0.1.1/zarrview.egg-info/top_level.txt
+drwxr-xr-x   0 marcel     (501) staff       (20)        0 2023-08-04 15:46:11.321342 zarrview-0.1.2/
+-rw-r--r--   0 marcel     (501) staff       (20)     1077 2023-07-31 23:47:54.000000 zarrview-0.1.2/LICENSE
+-rw-r--r--   0 marcel     (501) staff       (20)    11611 2023-08-04 15:46:11.320479 zarrview-0.1.2/PKG-INFO
+-rw-r--r--   0 marcel     (501) staff       (20)    10809 2023-08-04 15:38:22.000000 zarrview-0.1.2/README.md
+-rw-r--r--   0 marcel     (501) staff       (20)       38 2023-08-04 15:46:11.321506 zarrview-0.1.2/setup.cfg
+-rw-r--r--   0 marcel     (501) staff       (20)     1316 2023-08-04 15:45:26.000000 zarrview-0.1.2/setup.py
+drwxr-xr-x   0 marcel     (501) staff       (20)        0 2023-08-04 15:46:11.316955 zarrview-0.1.2/zarrview/
+-rw-------   0 marcel     (501) staff       (20)    50529 2023-08-04 15:34:08.000000 zarrview-0.1.2/zarrview/ZarrViewer.py
+-rw-r--r--   0 marcel     (501) staff       (20)        0 2023-07-10 21:49:49.000000 zarrview-0.1.2/zarrview/__init__.py
+-rw-r--r--   0 marcel     (501) staff       (20)      933 2023-08-01 20:29:56.000000 zarrview-0.1.2/zarrview/__main__.py
+-rw-------   0 marcel     (501) staff       (20)    22926 2023-08-01 16:57:00.000000 zarrview-0.1.2/zarrview/zarr_path_utils.py
+drwxr-xr-x   0 marcel     (501) staff       (20)        0 2023-08-04 15:46:11.319567 zarrview-0.1.2/zarrview.egg-info/
+-rw-r--r--   0 marcel     (501) staff       (20)    11611 2023-08-04 15:46:11.000000 zarrview-0.1.2/zarrview.egg-info/PKG-INFO
+-rw-r--r--   0 marcel     (501) staff       (20)      278 2023-08-04 15:46:11.000000 zarrview-0.1.2/zarrview.egg-info/SOURCES.txt
+-rw-r--r--   0 marcel     (501) staff       (20)        1 2023-08-04 15:46:11.000000 zarrview-0.1.2/zarrview.egg-info/dependency_links.txt
+-rw-r--r--   0 marcel     (501) staff       (20)       78 2023-08-04 15:46:11.000000 zarrview-0.1.2/zarrview.egg-info/requires.txt
+-rw-r--r--   0 marcel     (501) staff       (20)        9 2023-08-04 15:46:11.000000 zarrview-0.1.2/zarrview.egg-info/top_level.txt
```

### Comparing `zarrview-0.1.1/LICENSE` & `zarrview-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `zarrview-0.1.1/setup.py` & `zarrview-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 setup(
 
     ### Metadata
 
     name='zarrview',
 
-    version='0.1.1',
+    version='0.1.2',
 
     description='PySide or PyQt tree model/view for a Zarr hierarchy.',
 
     long_description=(HERE / "README.md").read_text(),
     long_description_content_type = "text/markdown",
 
     url='https://github.com/marcel-goldschen-ohm/zarr-view',
```

### Comparing `zarrview-0.1.1/zarrview/ZarrViewer.py` & `zarrview-0.1.2/zarrview/ZarrViewer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1183,29 +1183,29 @@
         self.setStretchFactor(0, 2)
         self.setStretchFactor(1, 1)
 
         self.hierarchy_view.selectionModel().selectionChanged.connect(self.onSelectionChanged)
         self.hierarchy_model.infoChanged.connect(self.onInfoChanged)
         self.hierarchy_model.maxDepthChanged.connect(self.onMaxDepthChanged)
 
-        self.expandAll()
+        self.collapseAll()
     
     def setTree(self, root: zarr.hierarchy.Group | zarr.core.Array, path: str = None):
         self.hierarchy_model.reset_model(root, 
                                          path=path, 
                                          include_attrs=False, 
                                          include_arrays=True, 
                                          include_groups=True)
 
         self.hierarchy_view.selectionModel().clearSelection()
         self.hierarchy_view.selectionModel().selectionChanged.connect(self.onSelectionChanged)
 
         max_depth = self.hierarchy_model.max_depth()
         self.expandToDepthSpinBox.setMaximum(max_depth - 1)
-        self.expandAll()
+        self.collapseAll()
 
         self.attr_model.reset_model(root, 
                                     path=None, 
                                     include_attrs=True, 
                                     include_arrays=False, 
                                     include_groups=False)
         self.attr_view.expandAll()
```

### Comparing `zarrview-0.1.1/zarrview/zarr_path_utils.py` & `zarrview-0.1.2/zarrview/zarr_path_utils.py`

 * *Files identical despite different names*

