# Comparing `tmp/ndtiff-2.2.0.tar.gz` & `tmp/ndtiff-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ndtiff-2.2.0.tar", last modified: Mon Jul 31 17:12:21 2023, max compression
+gzip compressed data, was "ndtiff-2.2.1.tar", last modified: Fri Aug  4 12:26:33 2023, max compression
```

## Comparing `ndtiff-2.2.0.tar` & `ndtiff-2.2.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:12:21.884292 ndtiff-2.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-31 17:12:21.884292 ndtiff-2.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-31 17:12:07.000000 ndtiff-2.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:12:21.884292 ndtiff-2.2.0/ndtiff/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-31 17:12:07.000000 ndtiff-2.2.0/ndtiff/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-07-31 17:12:07.000000 ndtiff-2.2.0/ndtiff/_superclass.py
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-31 17:12:07.000000 ndtiff-2.2.0/ndtiff/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-07-31 17:12:07.000000 ndtiff-2.2.0/ndtiff/file_io.py
--rw-r--r--   0 runner    (1001) docker     (123)    43626 2023-07-31 17:12:07.000000 ndtiff-2.2.0/ndtiff/nd_tiff_current.py
--rw-r--r--   0 runner    (1001) docker     (123)    28685 2023-07-31 17:12:07.000000 ndtiff-2.2.0/ndtiff/nd_tiff_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)    44915 2023-07-31 17:12:07.000000 ndtiff-2.2.0/ndtiff/ndtiff_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:12:21.884292 ndtiff-2.2.0/ndtiff/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 17:12:07.000000 ndtiff-2.2.0/ndtiff/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-31 17:12:07.000000 ndtiff-2.2.0/ndtiff/test/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4812 2023-07-31 17:12:07.000000 ndtiff-2.2.0/ndtiff/test/data_loading_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-07-31 17:12:07.000000 ndtiff-2.2.0/ndtiff/test/test_custom_io.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:12:21.884292 ndtiff-2.2.0/ndtiff.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-31 17:12:21.000000 ndtiff-2.2.0/ndtiff.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-07-31 17:12:21.000000 ndtiff-2.2.0/ndtiff.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 17:12:21.000000 ndtiff-2.2.0/ndtiff.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-31 17:12:21.000000 ndtiff-2.2.0/ndtiff.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-31 17:12:21.000000 ndtiff-2.2.0/ndtiff.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-31 17:12:07.000000 ndtiff-2.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 17:12:21.884292 ndtiff-2.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-07-31 17:12:07.000000 ndtiff-2.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:26:33.059784 ndtiff-2.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-08-04 12:26:33.059784 ndtiff-2.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-04 12:26:24.000000 ndtiff-2.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:26:33.059784 ndtiff-2.2.1/ndtiff/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-08-04 12:26:24.000000 ndtiff-2.2.1/ndtiff/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-08-04 12:26:24.000000 ndtiff-2.2.1/ndtiff/_superclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-08-04 12:26:24.000000 ndtiff-2.2.1/ndtiff/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-08-04 12:26:24.000000 ndtiff-2.2.1/ndtiff/file_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43637 2023-08-04 12:26:24.000000 ndtiff-2.2.1/ndtiff/nd_tiff_current.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28685 2023-08-04 12:26:24.000000 ndtiff-2.2.1/ndtiff/nd_tiff_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44915 2023-08-04 12:26:24.000000 ndtiff-2.2.1/ndtiff/ndtiff_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:26:33.059784 ndtiff-2.2.1/ndtiff/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 12:26:24.000000 ndtiff-2.2.1/ndtiff/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-08-04 12:26:24.000000 ndtiff-2.2.1/ndtiff/test/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7271 2023-08-04 12:26:24.000000 ndtiff-2.2.1/ndtiff/test/data_loading_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-08-04 12:26:24.000000 ndtiff-2.2.1/ndtiff/test/test_custom_io.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:26:33.059784 ndtiff-2.2.1/ndtiff.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-08-04 12:26:33.000000 ndtiff-2.2.1/ndtiff.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-08-04 12:26:33.000000 ndtiff-2.2.1/ndtiff.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:26:33.000000 ndtiff-2.2.1/ndtiff.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-08-04 12:26:33.000000 ndtiff-2.2.1/ndtiff.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-04 12:26:33.000000 ndtiff-2.2.1/ndtiff.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-08-04 12:26:24.000000 ndtiff-2.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:26:33.059784 ndtiff-2.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-08-04 12:26:24.000000 ndtiff-2.2.1/setup.py
```

### Comparing `ndtiff-2.2.0/PKG-INFO` & `ndtiff-2.2.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ndtiff
-Version: 2.2.0
+Version: 2.2.1
 Summary: Python libraries for NDTiff datasets
 Home-page: https://github.com/micro-manager/NDTiffStorage
 Author: Henry Pinkard
 Author-email: henry.pinkard@gmail.com
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `ndtiff-2.2.0/ndtiff/_superclass.py` & `ndtiff-2.2.1/ndtiff/_superclass.py`

 * *Files identical despite different names*

### Comparing `ndtiff-2.2.0/ndtiff/file_io.py` & `ndtiff-2.2.1/ndtiff/file_io.py`

 * *Files identical despite different names*

### Comparing `ndtiff-2.2.0/ndtiff/nd_tiff_current.py` & `ndtiff-2.2.1/ndtiff/nd_tiff_current.py`

 * *Files 0% similar despite different names*

```diff
@@ -565,15 +565,15 @@
         ) = struct.unpack("IIIIIIII", data[position : position + 32])
         position += 32
         entries[frozenset(axes.items())] = index_entry
         return position, axes, index_entry
 
     def read_index(self, path):
         print("\rReading index...          ", end="")
-        with self.file_io.open(path + os.sep + "NDTiff.index", "rb") as index_file:
+        with self.file_io.open(path + "NDTiff.index", "rb") as index_file:
             data = index_file.read()
         entries = {}
         position = 0
         while position < len(data):
             print(
                 "\rReading index... {:.1f}%       ".format(
                     100 * (1 - (len(data) - position) / len(data))
@@ -622,15 +622,15 @@
 
     def close(self):
         for reader in self._readers_by_filename.values():
             reader.close()
 
     def _read_one_image(self, block_id, axes_to_stack=None, axes_to_slice=None, stitched=False, rgb=False):
         # a function that reads in one chunk of data
-        axes = {key: block_id[i] for i, key in enumerate(axes_to_stack.keys())}
+        axes = {key: axes_to_stack[key][block_id[i]] for i, key in enumerate(axes_to_stack.keys())}
         if stitched:
             # Combine all rows and cols into one stitched image
             # get spatial layout of position indices
             row_values = np.array(list(self.axes["row"]))
             column_values = np.array(list(self.axes["column"]))
             # fill in missing values
             row_values = np.arange(np.min(row_values), np.max(row_values) + 1)
```

### Comparing `ndtiff-2.2.0/ndtiff/nd_tiff_v2.py` & `ndtiff-2.2.1/ndtiff/nd_tiff_v2.py`

 * *Files identical despite different names*

### Comparing `ndtiff-2.2.0/ndtiff/ndtiff_v1.py` & `ndtiff-2.2.1/ndtiff/ndtiff_v1.py`

 * *Files identical despite different names*

### Comparing `ndtiff-2.2.0/ndtiff/test/data_loading_test.py` & `ndtiff-2.2.1/ndtiff/test/data_loading_test.py`

 * *Files 24% similar despite different names*

```diff
@@ -104,9 +104,81 @@
     assert(np.sum(np.array(dataset.as_array(stitched=True)[0])) > 0)
 
 def test_v3_2_no_magellan_explore_no_channels(test_data_path):
     data_path = os.path.join(test_data_path, 'v3', 'no_magellan_explore_no_channel')
     dataset = Dataset(data_path)
     assert(np.sum(np.array(dataset.as_array(stitched=True)[0])) > 0)
 
+def test_labeled_positions(test_data_path):
+    """
+    This dataset was acquired with the following events:
 
+    events = [
+        {'axes': {'position': 'Pos2'}, 'x': 0, 'y': 0},
+        {'axes': {'position': 'Pos0'}, 'x': 0, 'y': 1},
+        {'axes': {'position': 'Pos1'}, 'x': 0, 'y': 2}
+    ]
 
+    Further, images at position ('Pos2', 'Pos0', 'Pos1') have (0, 0) pixels
+    equal to (0, 1, 2).
+
+    Here we test that the axis and image order of the dataset is as expected.
+    """
+
+    data_path = os.path.join(test_data_path, 'v3', 'labeled_positions_1')
+    position_names = ('Pos2', 'Pos0', 'Pos1')
+
+    dataset = Dataset(data_path)
+    data = np.asarray(dataset.as_array())
+
+    # ndtiff sorts the dataset axes. Check that the position axis is correctly
+    # sorted
+    assert dataset.axes['position'] == set(('Pos0', 'Pos1', 'Pos2'))
+
+    # Check that the image metadata includes the position name
+    for position_name in position_names:
+        metadata = dataset.read_metadata(position=position_name)
+        assert metadata['PositionName'] == position_name
+
+    # Check that data is in the ('Pos0', 'Pos1', 'Pos2') order
+    pixel_00 = (1, 2, 0)
+    for idx, image in enumerate(data):
+        assert image[0, 0] == pixel_00[idx]
+
+def test_unordered_z_axis(test_data_path):
+    """
+    This dataset was acquired with the following events:
+
+    events1 = [{'axes': {'z': z_idx}, 'z': z_idx} for z_idx in range(10)]
+    events2 = [{'axes': {'z': z_idx}, 'z': z_idx} for z_idx in range(-10, 0)]
+
+    and the following image process hook function:
+
+    def fun(image, metadata):
+        if not hasattr(fun, "idx"):
+            fun.idx = 0
+
+        image[0, 0] = np.uint16(fun.idx)
+
+        fun.idx += 1
+
+        return image, metadata
+
+    Here we test that the axis and image order of the dataset is as expected.
+    """
+
+    data_path = os.path.join(test_data_path, 'v3', 'unordered_z_1')
+    acquisition_z_axis = list(range(10)) + list(range(-10, 0))
+    sorting_index = np.argsort(acquisition_z_axis)
+    sorted_z_axis = np.sort(acquisition_z_axis)
+
+    dataset = Dataset(data_path)
+    data = np.asarray(dataset.as_array())
+
+    # ndtiff sorts the dataset axes. Check that the position axis is correctly
+    # sorted
+    assert dataset.axes['z'] == set(sorted_z_axis)
+
+    # Check that data is in the sorted(acquisition_z_axis) order
+    pixel_00 = sorting_index
+    for idx, image in enumerate(data):
+        assert image[0, 0] == pixel_00[idx]
```

### Comparing `ndtiff-2.2.0/ndtiff/test/test_custom_io.py` & `ndtiff-2.2.1/ndtiff/test/test_custom_io.py`

 * *Files identical despite different names*

### Comparing `ndtiff-2.2.0/ndtiff.egg-info/PKG-INFO` & `ndtiff-2.2.1/ndtiff.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ndtiff
-Version: 2.2.0
+Version: 2.2.1
 Summary: Python libraries for NDTiff datasets
 Home-page: https://github.com/micro-manager/NDTiffStorage
 Author: Henry Pinkard
 Author-email: henry.pinkard@gmail.com
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `ndtiff-2.2.0/setup.py` & `ndtiff-2.2.1/setup.py`

 * *Files identical despite different names*

