# Comparing `tmp/napari-gemspa-0.0.3.tar.gz` & `tmp/napari-gemspa-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-gemspa-0.0.3.tar", last modified: Sun Jun  4 00:07:09 2023, max compression
+gzip compressed data, was "napari-gemspa-0.0.4.tar", last modified: Fri Aug  4 17:54:17 2023, max compression
```

## Comparing `napari-gemspa-0.0.3.tar` & `napari-gemspa-0.0.4.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 sarahkeegan   (501) staff       (20)        0 2023-06-04 00:07:09.946341 napari-gemspa-0.0.3/
--rw-r--r--   0 sarahkeegan   (501) staff       (20)     1512 2023-04-13 14:56:39.000000 napari-gemspa-0.0.3/LICENSE
--rw-r--r--   0 sarahkeegan   (501) staff       (20)       96 2023-04-02 00:08:59.000000 napari-gemspa-0.0.3/MANIFEST.in
--rw-r--r--   0 sarahkeegan   (501) staff       (20)    11015 2023-06-04 00:07:09.946491 napari-gemspa-0.0.3/PKG-INFO
--rw-r--r--   0 sarahkeegan   (501) staff       (20)     9741 2023-06-04 00:05:29.000000 napari-gemspa-0.0.3/README.md
--rw-r--r--   0 sarahkeegan   (501) staff       (20)      130 2023-06-03 16:24:39.000000 napari-gemspa-0.0.3/pyproject.toml
--rw-r--r--   0 sarahkeegan   (501) staff       (20)     1761 2023-06-04 00:07:09.946987 napari-gemspa-0.0.3/setup.cfg
-drwxr-xr-x   0 sarahkeegan   (501) staff       (20)        0 2023-06-04 00:07:09.939971 napari-gemspa-0.0.3/src/
-drwxr-xr-x   0 sarahkeegan   (501) staff       (20)        0 2023-06-04 00:07:09.941502 napari-gemspa-0.0.3/src/_tests/
--rw-------   0 sarahkeegan   (501) staff       (20)        0 2023-06-03 16:24:39.000000 napari-gemspa-0.0.3/src/_tests/__init__.py
--rw-r--r--   0 sarahkeegan   (501) staff       (20)     1777 2023-06-03 16:24:39.000000 napari-gemspa-0.0.3/src/_tests/run_napari.py
--rw-r--r--   0 sarahkeegan   (501) staff       (20)     3224 2023-06-03 16:24:39.000000 napari-gemspa-0.0.3/src/_tests/test_gemspa_locate_worker.py
-drwxr-xr-x   0 sarahkeegan   (501) staff       (20)        0 2023-06-04 00:07:09.945159 napari-gemspa-0.0.3/src/napari_gemspa/
--rw-r--r--   0 sarahkeegan   (501) staff       (20)      320 2023-05-29 19:40:41.000000 napari-gemspa-0.0.3/src/napari_gemspa/__init__.py
--rw-r--r--   0 sarahkeegan   (501) staff       (20)    25898 2023-06-03 16:24:39.000000 napari-gemspa-0.0.3/src/napari_gemspa/_gemspa_analyze_widget.py
--rw-r--r--   0 sarahkeegan   (501) staff       (20)    19439 2023-06-03 18:51:07.000000 napari-gemspa-0.0.3/src/napari_gemspa/_gemspa_data_views.py
--rw-r--r--   0 sarahkeegan   (501) staff       (20)     8770 2023-06-03 16:24:39.000000 napari-gemspa-0.0.3/src/napari_gemspa/_gemspa_file_import_widget.py
--rw-r--r--   0 sarahkeegan   (501) staff       (20)     6596 2023-06-03 16:24:39.000000 napari-gemspa-0.0.3/src/napari_gemspa/_gemspa_filter_links_widget.py
--rw-r--r--   0 sarahkeegan   (501) staff       (20)     6021 2023-06-03 16:24:39.000000 napari-gemspa-0.0.3/src/napari_gemspa/_gemspa_link_widget.py
--rw-r--r--   0 sarahkeegan   (501) staff       (20)     8503 2023-06-03 16:24:39.000000 napari-gemspa-0.0.3/src/napari_gemspa/_gemspa_locate_widget.py
--rw-r--r--   0 sarahkeegan   (501) staff       (20)    10201 2023-06-03 16:24:39.000000 napari-gemspa-0.0.3/src/napari_gemspa/_gemspa_plugin.py
--rw-r--r--   0 sarahkeegan   (501) staff       (20)     7789 2023-06-03 16:24:39.000000 napari-gemspa-0.0.3/src/napari_gemspa/_gemspa_widget.py
--rw-r--r--   0 sarahkeegan   (501) staff       (20)     2582 2023-05-22 18:46:47.000000 napari-gemspa-0.0.3/src/napari_gemspa/_reader.py
--rw-r--r--   0 sarahkeegan   (501) staff       (20)     1764 2023-05-24 21:55:19.000000 napari-gemspa-0.0.3/src/napari_gemspa/_utils.py
--rw-r--r--   0 sarahkeegan   (501) staff       (20)     3553 2023-06-03 16:24:39.000000 napari-gemspa-0.0.3/src/napari_gemspa/_writer.py
--rw-r--r--   0 sarahkeegan   (501) staff       (20)     1352 2023-05-29 19:40:41.000000 napari-gemspa-0.0.3/src/napari_gemspa/napari.yaml
-drwxr-xr-x   0 sarahkeegan   (501) staff       (20)        0 2023-06-04 00:07:09.946182 napari-gemspa-0.0.3/src/napari_gemspa.egg-info/
--rw-r--r--   0 sarahkeegan   (501) staff       (20)    11015 2023-06-04 00:07:09.000000 napari-gemspa-0.0.3/src/napari_gemspa.egg-info/PKG-INFO
--rw-r--r--   0 sarahkeegan   (501) staff       (20)      873 2023-06-04 00:07:09.000000 napari-gemspa-0.0.3/src/napari_gemspa.egg-info/SOURCES.txt
--rw-r--r--   0 sarahkeegan   (501) staff       (20)        1 2023-06-04 00:07:09.000000 napari-gemspa-0.0.3/src/napari_gemspa.egg-info/dependency_links.txt
--rw-r--r--   0 sarahkeegan   (501) staff       (20)       60 2023-06-04 00:07:09.000000 napari-gemspa-0.0.3/src/napari_gemspa.egg-info/entry_points.txt
--rw-r--r--   0 sarahkeegan   (501) staff       (20)      137 2023-06-04 00:07:09.000000 napari-gemspa-0.0.3/src/napari_gemspa.egg-info/requires.txt
--rw-r--r--   0 sarahkeegan   (501) staff       (20)       21 2023-06-04 00:07:09.000000 napari-gemspa-0.0.3/src/napari_gemspa.egg-info/top_level.txt
+drwxr-xr-x   0 snk218   (1170528910) 1222563772        0 2023-08-04 17:54:17.243265 napari-gemspa-0.0.4/
+-rw-r--r--   0 snk218   (1170528910) 1222563772     1512 2023-04-18 13:13:15.000000 napari-gemspa-0.0.4/LICENSE
+-rw-r--r--   0 snk218   (1170528910) 1222563772       96 2023-04-04 20:43:40.000000 napari-gemspa-0.0.4/MANIFEST.in
+-rw-r--r--   0 snk218   (1170528910) 1222563772    11015 2023-08-04 17:54:17.243429 napari-gemspa-0.0.4/PKG-INFO
+-rw-r--r--   0 snk218   (1170528910) 1222563772     9741 2023-08-04 14:45:13.000000 napari-gemspa-0.0.4/README.md
+-rw-r--r--   0 snk218   (1170528910) 1222563772      130 2023-06-01 23:01:19.000000 napari-gemspa-0.0.4/pyproject.toml
+-rw-r--r--   0 snk218   (1170528910) 1222563772     1761 2023-08-04 17:54:17.244816 napari-gemspa-0.0.4/setup.cfg
+drwxr-xr-x   0 snk218   (1170528910) 1222563772        0 2023-08-04 17:54:17.225688 napari-gemspa-0.0.4/src/
+drwxr-xr-x   0 snk218   (1170528910) 1222563772        0 2023-08-04 17:54:17.229556 napari-gemspa-0.0.4/src/_tests/
+-rw-------   0 snk218   (1170528910) 1222563772        0 2023-05-30 13:17:53.000000 napari-gemspa-0.0.4/src/_tests/__init__.py
+-rw-r--r--   0 snk218   (1170528910) 1222563772     1777 2023-06-01 18:19:26.000000 napari-gemspa-0.0.4/src/_tests/run_napari.py
+-rw-r--r--   0 snk218   (1170528910) 1222563772     3224 2023-06-01 18:14:19.000000 napari-gemspa-0.0.4/src/_tests/test_gemspa_locate_worker.py
+drwxr-xr-x   0 snk218   (1170528910) 1222563772        0 2023-08-04 17:54:17.239628 napari-gemspa-0.0.4/src/napari_gemspa/
+-rw-r--r--   0 snk218   (1170528910) 1222563772      323 2023-08-04 17:47:31.000000 napari-gemspa-0.0.4/src/napari_gemspa/__init__.py
+-rw-r--r--   0 snk218   (1170528910) 1222563772    26204 2023-08-04 14:45:13.000000 napari-gemspa-0.0.4/src/napari_gemspa/_gemspa_analyze_widget.py
+-rw-r--r--   0 snk218   (1170528910) 1222563772    19439 2023-08-04 14:45:13.000000 napari-gemspa-0.0.4/src/napari_gemspa/_gemspa_data_views.py
+-rw-r--r--   0 snk218   (1170528910) 1222563772     8775 2023-08-04 14:45:13.000000 napari-gemspa-0.0.4/src/napari_gemspa/_gemspa_file_import_widget.py
+-rw-r--r--   0 snk218   (1170528910) 1222563772     6910 2023-08-04 14:45:13.000000 napari-gemspa-0.0.4/src/napari_gemspa/_gemspa_filter_links_widget.py
+-rw-r--r--   0 snk218   (1170528910) 1222563772     6512 2023-08-04 14:45:13.000000 napari-gemspa-0.0.4/src/napari_gemspa/_gemspa_link_widget.py
+-rw-r--r--   0 snk218   (1170528910) 1222563772     9333 2023-08-04 17:08:38.000000 napari-gemspa-0.0.4/src/napari_gemspa/_gemspa_locate_widget.py
+-rw-r--r--   0 snk218   (1170528910) 1222563772    10201 2023-05-30 21:44:24.000000 napari-gemspa-0.0.4/src/napari_gemspa/_gemspa_plugin.py
+-rw-r--r--   0 snk218   (1170528910) 1222563772     7273 2023-08-04 14:45:13.000000 napari-gemspa-0.0.4/src/napari_gemspa/_gemspa_widget.py
+-rw-r--r--   0 snk218   (1170528910) 1222563772     2582 2023-05-23 14:36:23.000000 napari-gemspa-0.0.4/src/napari_gemspa/_reader.py
+-rw-r--r--   0 snk218   (1170528910) 1222563772     1764 2023-05-25 15:54:36.000000 napari-gemspa-0.0.4/src/napari_gemspa/_utils.py
+-rw-r--r--   0 snk218   (1170528910) 1222563772     3553 2023-06-01 18:19:26.000000 napari-gemspa-0.0.4/src/napari_gemspa/_writer.py
+-rw-r--r--   0 snk218   (1170528910) 1222563772     1352 2023-05-30 13:17:53.000000 napari-gemspa-0.0.4/src/napari_gemspa/napari.yaml
+drwxr-xr-x   0 snk218   (1170528910) 1222563772        0 2023-08-04 17:54:17.242882 napari-gemspa-0.0.4/src/napari_gemspa.egg-info/
+-rw-r--r--   0 snk218   (1170528910) 1222563772    11015 2023-08-04 17:54:17.000000 napari-gemspa-0.0.4/src/napari_gemspa.egg-info/PKG-INFO
+-rw-r--r--   0 snk218   (1170528910) 1222563772      873 2023-08-04 17:54:17.000000 napari-gemspa-0.0.4/src/napari_gemspa.egg-info/SOURCES.txt
+-rw-r--r--   0 snk218   (1170528910) 1222563772        1 2023-08-04 17:54:17.000000 napari-gemspa-0.0.4/src/napari_gemspa.egg-info/dependency_links.txt
+-rw-r--r--   0 snk218   (1170528910) 1222563772       60 2023-08-04 17:54:17.000000 napari-gemspa-0.0.4/src/napari_gemspa.egg-info/entry_points.txt
+-rw-r--r--   0 snk218   (1170528910) 1222563772      137 2023-08-04 17:54:17.000000 napari-gemspa-0.0.4/src/napari_gemspa.egg-info/requires.txt
+-rw-r--r--   0 snk218   (1170528910) 1222563772       21 2023-08-04 17:54:17.000000 napari-gemspa-0.0.4/src/napari_gemspa.egg-info/top_level.txt
```

### Comparing `napari-gemspa-0.0.3/LICENSE` & `napari-gemspa-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-gemspa-0.0.3/PKG-INFO` & `napari-gemspa-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-gemspa
-Version: 0.0.3
+Version: 0.0.4
 Summary: A plugin for analysis of single particle tracking experiments
 Home-page: https://github.com/liamholtlab/napari-gemspa
 Author: Sarah Keegan
 Author-email: sarah.keegan@nyulangone.org
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/liamholtlab/napari-gemspa/issues
 Project-URL: Documentation, https://github.com/liamholtlab/napari-gemspa#README.md
```

### Comparing `napari-gemspa-0.0.3/README.md` & `napari-gemspa-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `napari-gemspa-0.0.3/setup.cfg` & `napari-gemspa-0.0.4/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = napari-gemspa
-version = 0.0.3
+version = 0.0.4
 description = A plugin for analysis of single particle tracking experiments
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/liamholtlab/napari-gemspa
 author = Sarah Keegan
 author_email = sarah.keegan@nyulangone.org
 license = BSD-3-Clause
```

### Comparing `napari-gemspa-0.0.3/src/_tests/run_napari.py` & `napari-gemspa-0.0.4/src/_tests/run_napari.py`

 * *Files identical despite different names*

### Comparing `napari-gemspa-0.0.3/src/_tests/test_gemspa_locate_worker.py` & `napari-gemspa-0.0.4/src/_tests/test_gemspa_locate_worker.py`

 * *Files identical despite different names*

### Comparing `napari-gemspa-0.0.3/src/napari_gemspa/_gemspa_analyze_widget.py` & `napari-gemspa-0.0.4/src/napari_gemspa/_gemspa_analyze_widget.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,20 +16,23 @@
 from ._gemspa_widget import GEMspaWidget, GEMspaWorker
 from ._utils import convert_to_float, convert_to_int, remove_outside_mask, show_error
 
 
 class GEMspaAnalyzeWorker(GEMspaWorker):
     """Worker for the Analyze plugin"""
 
-    def __init__(self):
+    def __init__(self, *args, **kwargs):
         super().__init__()
+        self.args = args
+        self.kwargs = kwargs
 
     @Slot(dict)
-    def run(self, state):
+    def run(self):
         """Execute the processing"""
+        state = self.args[0]
 
         input_params = state["inputs"]
         state_params = state["parameters"]
 
         batch = state_params["batch"]
         track_id = state_params["track_id"]
         microns_per_pixel = state_params["microns_per_pixel"]
@@ -70,15 +73,15 @@
         # *note* this function is not implemented for 3D (z-dimensional) data
         # *note* if not run in batch mode (only analyze a single track), the labels layer is ignored
         if batch and "labels_layer_data" in input_params:
             labeled_mask = input_params["labels_layer_data"]
             track_data_df = remove_outside_mask(
                 track_data_df, labeled_mask, id_column="track_id"
             )
-            self.log.emit(
+            self.signals.log.emit(
                 f"Removed particles outside of mask region, number of particles: {track_data_df['track_id'].nunique()}"
             )
 
         # Create the gemspa-spt class object for performing analysis
         if not z_col:
             # ParticleTracks class expects a column for z-dimension
             tracks = ParticleTracks(np.insert(track_data_df.to_numpy(), 2, 0, axis=1))
@@ -154,15 +157,15 @@
             tracks.fit_msd_all_tracks(
                 linear_fit=False,
                 min_len=min_len_fit,
                 max_lagtime=max_lagtime_fit,
                 err=error_term_fit,
             )
 
-            self.log.emit(
+            self.signals.log.emit(
                 f"Total number of tracks: {len(tracks.track_ids)}\n"
                 + f"After length filter, number of tracks: {len(tracks.linear_fit_results)}\n"
             )
 
             # Gather the fit data and r-of-g
             all_fit_data = np.concatenate(
                 [tracks.linear_fit_results, tracks.loglog_fit_results[:, 2:]],
@@ -361,18 +364,17 @@
 
                 out_data = {
                     "df": track_data_df,
                     "summary_data": summary_data,
                     "batch": batch,
                 }
             else:
-                self.log.emit(f"Track id {track_id} not found.")
+                self.signals.log.emit(f"Track id {track_id} not found.")
 
-        self.update_data.emit(out_data)
-        super().run()
+        self.signals.update_data.emit(out_data)
 
 
 class GEMspaAnalyzeWidget(GEMspaWidget):
     """Widget for Analysis plugin"""
 
     name = "GEMspaAnalyzeWidget"
 
@@ -481,16 +483,19 @@
 
         layout.addLayout(grid_layout)
         layout.addStretch()
         self.setLayout(layout)
 
     def start_task(self, layer_names, log_widget):
         # initialize worker and start task
-        self.worker = GEMspaAnalyzeWorker()
-        super().start_task(layer_names, log_widget)
+        self.worker = GEMspaAnalyzeWorker(self.state(layer_names))
+        self.worker.signals.log.connect(log_widget.add_log)
+        # once worker is done, do something with returned data
+        self.worker.signals.update_data.connect(self.update_data)
+        self.threadpool.start(self.worker)
 
     def check_inputs(self):
         # Special case for track id, it is required if batch is not checked
         keys = list(self._input_values.keys())
         required_keys = self._required_inputs[:]
         if self._batch_check.isChecked():
             # ignore track id completely
```

### Comparing `napari-gemspa-0.0.3/src/napari_gemspa/_gemspa_data_views.py` & `napari-gemspa-0.0.4/src/napari_gemspa/_gemspa_data_views.py`

 * *Files identical despite different names*

### Comparing `napari-gemspa-0.0.3/src/napari_gemspa/_gemspa_file_import_widget.py` & `napari-gemspa-0.0.4/src/napari_gemspa/_gemspa_file_import_widget.py`

 * *Files 1% similar despite different names*

```diff
@@ -199,15 +199,15 @@
                     break
 
         if not found_image:
             show_error("Cannot create labels layer: no selected image layer found.")
 
     def _load_image_file(self):
         filename, _ = QFileDialog.getOpenFileName(
-            self, "time-lapse movies (*.tif *.tiff *.nd2)"
+            self, "time-lapse movies (*.tif *.tiff *.nd2 *.dv)"
         )
         if filename:
             ext = os.path.splitext(filename)[1]
             if ext == ".nd2":
                 f = nd2.ND2File(filename)
                 images = f.asarray()
                 f.close()
```

### Comparing `napari-gemspa-0.0.3/src/napari_gemspa/_gemspa_filter_links_widget.py` & `napari-gemspa-0.0.4/src/napari_gemspa/_gemspa_filter_links_widget.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,20 +7,23 @@
 from ._gemspa_widget import GEMspaWidget, GEMspaWorker
 from ._utils import convert_to_float, convert_to_int, show_error
 
 
 class GEMspaFilterLinksWorker(GEMspaWorker):
     """Worker for the Link Features plugin"""
 
-    def __init__(self):
+    def __init__(self, *args, **kwargs):
         super().__init__()
+        self.args = args
+        self.kwargs = kwargs
 
     @Slot(dict)
-    def run(self, state):
+    def run(self):
         """Execute the processing"""
+        state = self.args[0]
 
         input_params = state["inputs"]
         state_params = state["parameters"]
 
         min_frames = state_params["min_frames"]
         min_mass = state_params["min_mass"]
         max_mass = state_params["max_mass"]
@@ -33,22 +36,22 @@
         scale = input_params["tracks_layer_scale"]
         tracks_layer_props = input_params["tracks_layer_props"]
 
         # Make trackpy table from layer data
         out_data = dict()
         t = self._make_trackpy_table("tracks", tracks_layer_data, tracks_layer_props)
         if t is not None:
-            self.log.emit(f"Number of particles: {t['particle'].nunique()}")
+            self.signals.log.emit(f"Number of particles: {t['particle'].nunique()}")
 
             tp.quiet()
 
             # filter by min frames
             if min_frames is not None and min_frames > 1:
                 t = tp.filter_stubs(t, threshold=min_frames)
-                self.log.emit(
+                self.signals.log.emit(
                     f"After filter for Min frames, number of particles: {t['particle'].nunique()}"
                 )
 
             # filter by mass, size, eccentricity
             mean_t = t.groupby("particle").mean()
 
             if min_mass is not None and min_mass > 0:
@@ -63,35 +66,34 @@
 
             if min_ecc is not None and min_ecc > 0:
                 mean_t = mean_t[mean_t["ecc"] >= min_ecc]
             if max_ecc is not None and max_ecc < 1:
                 mean_t = mean_t[mean_t["ecc"] <= max_ecc]
 
             t = t[t["particle"].isin(mean_t.index)]
-            self.log.emit(
+            self.signals.log.emit(
                 f"After filter for mass/size/eccentricity, number of particles: {t['particle'].nunique()}"
             )
 
             # emit the output data after sorting by track_id (particle) and frame (needed for tracks layer)
             t.index.name = (
                 "index"  # pandas complains when index name and column name are the same
             )
             t = t.sort_values(by=["particle", "frame"], axis=0, ascending=True)
 
             # change column name from 'particle' to 'track_id' to identify the track for consistency with napari layer
             t.rename(columns={"particle": "track_id"}, inplace=True)
 
             out_data = {"df": t, "scale": scale}
         else:
-            self.log.emit(
+            self.signals.log.emit(
                 "Error: The tracks layer properties do not contain the required columns for filtering."
             )
 
-        self.update_data.emit(out_data)
-        super().run()
+        self.signals.update_data.emit(out_data)
 
 
 class GEMspaFilterLinksWidget(GEMspaWidget):
     """Widget for Filter links plugin"""
 
     name = "GEMspaFilterLinksWidget"
 
@@ -110,16 +112,19 @@
 
         self._required_inputs = []
 
         self.init_ui()
 
     def start_task(self, layer_names, log_widget):
         # initialize worker and start task
-        self.worker = GEMspaFilterLinksWorker()
-        super().start_task(layer_names, log_widget)
+        self.worker = GEMspaFilterLinksWorker(self.state(layer_names))
+        self.worker.signals.log.connect(log_widget.add_log)
+        # once worker is done, do something with returned data
+        self.worker.signals.update_data.connect(self.update_data)
+        self.threadpool.start(self.worker)
 
     def state(self, layer_names) -> dict:
         return {
             "name": self.name,
             "inputs": {
                 "tracks_layer_name": layer_names["tracks"],
                 "tracks_layer_data": self.viewer.layers[layer_names["tracks"]].data,
```

### Comparing `napari-gemspa-0.0.3/src/napari_gemspa/_gemspa_link_widget.py` & `napari-gemspa-0.0.4/src/napari_gemspa/_gemspa_link_widget.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,20 +9,23 @@
 from ._gemspa_widget import GEMspaWidget, GEMspaWorker
 from ._utils import convert_to_float, convert_to_int, show_error
 
 
 class GEMspaLinkWorker(GEMspaWorker):
     """Worker for the Link Features plugin"""
 
-    def __init__(self):
+    def __init__(self, *args, **kwargs):
         super().__init__()
+        self.args = args
+        self.kwargs = kwargs
 
     @Slot(dict)
-    def run(self, state):
+    def run(self):
         """Execute the processing"""
+        state = self.args[0]
 
         input_params = state["inputs"]
         state_params = state["parameters"]
 
         search_range = state_params["search_range"]
 
         memory = state_params["memory"]
@@ -50,42 +53,47 @@
                 # Break on
                 # __THE_PROCESS_HAS_FORKED_AND_YOU_CANNOT_USE_THIS_COREFOUNDATION_FUNCTIONALITY___YOU_MUST_EXEC__()
                 # to debug.
                 warnings.filterwarnings("ignore", module="trackpy")
 
                 # perform linking
                 t = tp.link(f, search_range=search_range, memory=memory)
-                self.log.emit(f"Number of particles: {t['particle'].nunique()}")
+                self.signals.log.emit(
+                    f"Number of particles: {t['particle'].nunique()}"
+                )
 
                 # Filter spurious trajectories
                 if min_frames is not None and min_frames > 1:
                     t = tp.filter_stubs(t, threshold=min_frames)
-                    self.log.emit(
+                    self.signals.log.emit(
                         f"After filter for Min frames, number of particles: {t['particle'].nunique()}"
                     )
 
                 # emit the output data after sorting by track_id (particle) and frame (needed for tracks layer)
                 t.index.name = "index"  # pandas complains when index name and column name are the same
-                t = t.sort_values(by=["particle", "frame"], axis=0, ascending=True)
+                t = t.sort_values(
+                    by=["particle", "frame"], axis=0, ascending=True
+                )
 
                 # change column name from 'particle' to 'track_id' to identify the track for consistency with napari
                 t.rename(columns={"particle": "track_id"}, inplace=True)
 
                 warnings.resetwarnings()
 
                 out_data = {"df": t, "scale": scale}
             else:
-                self.log.emit(
+                self.signals.log.emit(
                     "Error: The points layer properties do not contain the required columns for linking."
                 )
         else:
-            self.log.emit("The data does not have a dimension for linking.")
+            self.signals.log.emit(
+                "The data does not have a dimension for linking."
+            )
 
-        self.update_data.emit(out_data)
-        super().run()
+        self.signals.update_data.emit(out_data)
 
 
 class GEMspaLinkWidget(GEMspaWidget):
     """Widget for Link features plugin"""
 
     name = "GEMspaLinkWidget"
 
@@ -102,35 +110,43 @@
         self._required_inputs = [
             "Link range",
         ]
 
         self.init_ui()
 
     def start_task(self, layer_names, log_widget):
-        # initialize worker and start task
-        self.worker = GEMspaLinkWorker()
-        super().start_task(layer_names, log_widget)
+        self.worker = GEMspaLinkWorker(self.state(layer_names))
+        self.worker.signals.log.connect(log_widget.add_log)
+        # once worker is done, do something with returned data
+        self.worker.signals.update_data.connect(self.update_data)
+        self.threadpool.start(self.worker)
 
     def state(self, layer_names) -> dict:
         return {
             "name": self.name,
             "inputs": {
                 "points_layer_name": layer_names["points"],
-                "points_layer_data": self.viewer.layers[layer_names["points"]].data,
-                "points_layer_scale": self.viewer.layers[layer_names["points"]].scale,
+                "points_layer_data": self.viewer.layers[
+                    layer_names["points"]
+                ].data,
+                "points_layer_scale": self.viewer.layers[
+                    layer_names["points"]
+                ].scale,
                 "points_layer_props": self.viewer.layers[
                     layer_names["points"]
                 ].properties,
             },
             "parameters": {
                 "search_range": convert_to_float(
                     self._input_values["Link range"].text()
                 ),
                 "memory": convert_to_int(self._input_values["Memory"].text()),
-                "min_frames": convert_to_int(self._input_values["Min frames"].text()),
+                "min_frames": convert_to_int(
+                    self._input_values["Min frames"].text()
+                ),
             },
         }
 
     def update_data(self, out_dict):
         """Set the worker outputs to napari layers"""
 
         if "df" in out_dict:
```

### Comparing `napari-gemspa-0.0.3/src/napari_gemspa/_gemspa_locate_widget.py` & `napari-gemspa-0.0.4/src/napari_gemspa/_gemspa_locate_widget.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,44 @@
 """Defines: GEMspaLocateWidget, GEMspaLocateWorker"""
 
 import warnings
 
 import trackpy as tp
 from qtpy.QtCore import Slot
-from qtpy.QtWidgets import QCheckBox, QGridLayout, QLabel, QLineEdit, QVBoxLayout
+from qtpy.QtWidgets import (
+    QCheckBox,
+    QGridLayout,
+    QLabel,
+    QLineEdit,
+    QVBoxLayout,
+)
 
 from ._gemspa_widget import GEMspaWidget, GEMspaWorker
 from ._utils import (
     convert_to_float,
     convert_to_int,
     fix_frame_limits,
     remove_outside_mask,
     show_error,
 )
 
 
 class GEMspaLocateWorker(GEMspaWorker):
     """Worker for the Locate Features plugin"""
 
-    def __init__(self):
+    def __init__(self, *args, **kwargs):
         super().__init__()
+        self.args = args
+        self.kwargs = kwargs
 
-    @Slot(dict)
-    def run(self, state):
+    @Slot()
+    def run(self):
         """Execute the processing"""
+        # for now, assume that the first argument is the 'state'
+        state = self.args[0]
 
         input_params = state["inputs"]
         state_params = state["parameters"]
 
         current_frame = state_params["current_frame"]
         del state_params["current_frame"]
 
@@ -61,45 +71,46 @@
 
         if current_frame:
             # Only process the current frame
             t = input_params["frame"]
             f = tp.locate(image[t], diameter, **state_params)
             if "frame" not in f.columns:
                 f["frame"] = t
-            self.log.emit(f"Processed frame {t}, number of particles: {len(f)}")
+            self.signals.log.emit(
+                f"Processed frame {t}, number of particles: {len(f)}"
+            )
         else:
             # process the entire movie - limited by frame start/end
             frame_offset = 0
             if len(image.shape) >= 3:
                 frame_start, frame_end = fix_frame_limits(
                     frame_start, frame_end, len(image)
                 )
                 image = image[frame_start : frame_end + 1]
                 frame_offset = frame_start
             f = tp.batch(image, diameter, **state_params)
             if "frame" in f.columns:
                 f["frame"] = f["frame"] + frame_offset
-            self.log.emit(
+            self.signals.log.emit(
                 f"Processed {len(image)} frames, number of particles: {len(f)}"
             )
 
         warnings.resetwarnings()
 
         # if labels layer was chosen, remove all points that are outside labeled regions
         if "labels_layer_data" in input_params:
             labeled_mask = input_params["labels_layer_data"]
             f = remove_outside_mask(f, labeled_mask)
-            self.log.emit(
+            self.signals.log.emit(
                 f"Removed particles outside of mask region, number of particles: {len(f)}"
             )
 
         out_data = {"df": f, "scale": scale, "diameter": diameter}
 
-        self.update_data.emit(out_data)
-        super().run()
+        self.signals.update_data.emit(out_data)
 
 
 class GEMspaLocateWidget(GEMspaWidget):
     """Widget for Locate Features plugin"""
 
     name = "GEMspaLocateWidget"
 
@@ -156,17 +167,21 @@
         grid_layout.addWidget(self._preprocess_check, i, 0, 1, 2)
 
         layout.addLayout(grid_layout)
         layout.addStretch()
         self.setLayout(layout)
 
     def start_task(self, layer_names, log_widget):
+        """this method overloads the parent implementation"""
         # initialize worker and start task
-        self.worker = GEMspaLocateWorker()
-        super().start_task(layer_names, log_widget)
+        self.worker = GEMspaLocateWorker(self.state(layer_names))
+        self.worker.signals.log.connect(log_widget.add_log)
+        # once worker is done, do something with returned data
+        self.worker.signals.update_data.connect(self.update_data)
+        self.threadpool.start(self.worker)
 
     def state(self, layer_names) -> dict:
         inputs_dict = {
             "image_layer_name": layer_names["image"],
             "image_layer_data": self.viewer.layers[layer_names["image"]].data,
             "image_layer_scale": self.viewer.layers[layer_names["image"]].scale,
             "frame": self.viewer.dims.current_step[0],
@@ -177,26 +192,44 @@
                 layer_names["labels"]
             ].data
 
         return {
             "name": self.name,
             "inputs": inputs_dict,
             "parameters": {
-                "frame_start": convert_to_int(self._input_values["Frame start"].text()),
-                "frame_end": convert_to_int(self._input_values["Frame end"].text()),
-                "diameter": convert_to_float(self._input_values["Diameter"].text()),
-                "minmass": convert_to_float(self._input_values["Min mass"].text()),
-                "maxsize": convert_to_float(self._input_values["Max size"].text()),
-                "separation": convert_to_float(self._input_values["Separation"].text()),
-                "noise_size": convert_to_float(self._input_values["Noise size"].text()),
+                "frame_start": convert_to_int(
+                    self._input_values["Frame start"].text()
+                ),
+                "frame_end": convert_to_int(
+                    self._input_values["Frame end"].text()
+                ),
+                "diameter": convert_to_float(
+                    self._input_values["Diameter"].text()
+                ),
+                "minmass": convert_to_float(
+                    self._input_values["Min mass"].text()
+                ),
+                "maxsize": convert_to_float(
+                    self._input_values["Max size"].text()
+                ),
+                "separation": convert_to_float(
+                    self._input_values["Separation"].text()
+                ),
+                "noise_size": convert_to_float(
+                    self._input_values["Noise size"].text()
+                ),
                 "smoothing_size": convert_to_float(
                     self._input_values["Smoothing size"].text()
                 ),
-                "threshold": convert_to_float(self._input_values["Threshold"].text()),
-                "percentile": convert_to_float(self._input_values["Percentile"].text()),
+                "threshold": convert_to_float(
+                    self._input_values["Threshold"].text()
+                ),
+                "percentile": convert_to_float(
+                    self._input_values["Percentile"].text()
+                ),
                 "topn": convert_to_float(self._input_values["Top n"].text()),
                 "invert": self._invert_check.isChecked(),
                 "preprocess": self._preprocess_check.isChecked(),
                 "current_frame": self._current_frame_check.isChecked(),
             },
         }
 
@@ -205,15 +238,15 @@
 
         if "df" in out_dict:
             kwargs = {
                 "scale": out_dict["scale"],
                 "size": out_dict["diameter"],
                 "name": "Feature Locations",
                 "face_color": "transparent",
-                "edge_color": "red",
+                "edge_color": "magenta",
             }
             df = out_dict["df"]
 
             if len(df) == 0:
                 show_error("No particles were located!")
             else:
                 layer = self._add_napari_layer("points", df, **kwargs)
```

### Comparing `napari-gemspa-0.0.3/src/napari_gemspa/_gemspa_plugin.py` & `napari-gemspa-0.0.4/src/napari_gemspa/_gemspa_plugin.py`

 * *Files identical despite different names*

### Comparing `napari-gemspa-0.0.3/src/napari_gemspa/_gemspa_widget.py` & `napari-gemspa-0.0.4/src/napari_gemspa/_gemspa_widget.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,45 @@
 """Defines: GEMspaWidget, GEMspaWorker, GEMspaLogWidget"""
 
 import numpy as np
 import pandas as pd
-from qtpy.QtCore import QObject, QThread, Signal
+from qtpy.QtCore import (
+    QObject,
+    QThread,
+    Signal,
+    QRunnable,
+    Signal,
+    Slot,
+    QThreadPool,
+)
 from qtpy.QtWidgets import QGridLayout, QLabel, QTextEdit, QVBoxLayout, QWidget
 
 from ._gemspa_data_views import GEMspaPlottingWindow, GEMspaTableWindow
 from ._utils import show_error
 
 
-class GEMspaWorker(QObject):
+class GEMspaSignals(QObject):
+    """defines custom signals available from a working worker thread"""
+
+    finished = Signal()
+    error = Signal(str)
+    log = Signal(str)
+    update_data = Signal(dict)
+
+
+class GEMspaWorker(QRunnable):
     """Definition of a GEMspaWorker
 
     Receives and Sends input/output as a dictionary
 
     """
 
-    # Worker can send these signals
-    finished = Signal()
-    update_data = Signal(dict)
-    log = Signal(str)
-
     def __init__(self):
         super().__init__()
+        self.signals = GEMspaSignals()
 
     @staticmethod
     def _make_trackpy_table(layer_type, data, props):
         req_cols = ["mass", "size", "ecc", "signal", "raw_mass", "ep"]
         for col in req_cols:
             if col not in props.keys():
                 return None
@@ -60,31 +73,33 @@
                 if col != "track_id":
                     df[col] = props[col]
         else:
             raise ValueError(f"Invalid layer type: {layer_type}")
 
         return df
 
+    @Slot()
     def run(self):
-        """Exec the data processing"""
-
-        self.finished.emit()
+        """Exec the data processing
+        Each GEMspaWorker sub-class needs to implement this method
+        """
+        self.signals.finished.emit()
 
 
 class GEMspaWidget(QWidget):
     """Definition of a GEMspa napari widget"""
 
     name = "GEMspaWidget"
 
     def __init__(self, napari_viewer, title=None):
         super().__init__()
 
         self.viewer = napari_viewer
         self.title = title
-        self.thread = None
+        self.threadpool = QThreadPool()
         self.worker = None
 
         # viewers for feature properties
         self.properties_viewers = []
 
         # viewers for the graphical output
         self.plots_viewers = []
@@ -128,22 +143,26 @@
             viewer.deleteLater()
 
         while self.properties_viewers:
             viewer = self.properties_viewers.pop()
             viewer.close()
             viewer.deleteLater()
 
-    def _new_plots_viewer(self, title="Plot view", figsize=(8, 3), close_last=True):
+    def _new_plots_viewer(
+        self, title="Plot view", figsize=(8, 3), close_last=True
+    ):
         if close_last and len(self.plots_viewers) >= 1:
             viewer = self.plots_viewers.pop()
             viewer.close()
             viewer.deleteLater()
 
         i = len(self.plots_viewers)
-        self.plots_viewers.append(GEMspaPlottingWindow(self.viewer, figsize=figsize))
+        self.plots_viewers.append(
+            GEMspaPlottingWindow(self.viewer, figsize=figsize)
+        )
         self.plots_viewers[i].setWindowTitle(title)
         return self.plots_viewers[i]
 
     def _new_properties_viewer(self, title="Table view", close_last=True):
         if close_last and len(self.properties_viewers) >= 1:
             viewer = self.properties_viewers.pop()
             viewer.close()
@@ -151,35 +170,16 @@
 
         i = len(self.properties_viewers)
         self.properties_viewers.append(GEMspaTableWindow(self.viewer))
         self.properties_viewers[i].setWindowTitle(title)
         return self.properties_viewers[i]
 
     def start_task(self, layer_names, log_widget):
-        # Perform startup tasks and start thread: worker must be initialized before this function is called
-
-        # Thread for this worker
-        self.thread = QThread()
-        self.worker.moveToThread(self.thread)
-
-        # connect worker log signal to the GEMspaLogWidget all_log method
-        self.worker.log.connect(log_widget.add_log)
-
-        # when thread is started, worker is run with the current state of the widget as input
-        self.thread.started.connect(lambda: self.worker.run(self.state(layer_names)))
-
-        # when the worker sends update_data signal, update_data of the widget will execute to update the GUI
-        self.worker.update_data.connect(self.update_data)
-
-        # Cleanup (as chatGPT suggested)
-        self.worker.finished.connect(self.thread.quit)
-        self.worker.finished.connect(self.worker.deleteLater)
-        self.thread.finished.connect(self.thread.deleteLater)
-
-        self.thread.start()
+        """must be implemented as overloaded method in subclasses"""
+        pass
 
     def check_inputs(self):
         valid = True
         for key in self._input_values.keys():
             text = self._input_values[key].text()
             if key in self._required_inputs or text:
                 # if input is not blank, check it is a number
```

### Comparing `napari-gemspa-0.0.3/src/napari_gemspa/_reader.py` & `napari-gemspa-0.0.4/src/napari_gemspa/_reader.py`

 * *Files identical despite different names*

### Comparing `napari-gemspa-0.0.3/src/napari_gemspa/_utils.py` & `napari-gemspa-0.0.4/src/napari_gemspa/_utils.py`

 * *Files identical despite different names*

### Comparing `napari-gemspa-0.0.3/src/napari_gemspa/_writer.py` & `napari-gemspa-0.0.4/src/napari_gemspa/_writer.py`

 * *Files identical despite different names*

### Comparing `napari-gemspa-0.0.3/src/napari_gemspa/napari.yaml` & `napari-gemspa-0.0.4/src/napari_gemspa/napari.yaml`

 * *Files identical despite different names*

### Comparing `napari-gemspa-0.0.3/src/napari_gemspa.egg-info/PKG-INFO` & `napari-gemspa-0.0.4/src/napari_gemspa.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-gemspa
-Version: 0.0.3
+Version: 0.0.4
 Summary: A plugin for analysis of single particle tracking experiments
 Home-page: https://github.com/liamholtlab/napari-gemspa
 Author: Sarah Keegan
 Author-email: sarah.keegan@nyulangone.org
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/liamholtlab/napari-gemspa/issues
 Project-URL: Documentation, https://github.com/liamholtlab/napari-gemspa#README.md
```

### Comparing `napari-gemspa-0.0.3/src/napari_gemspa.egg-info/SOURCES.txt` & `napari-gemspa-0.0.4/src/napari_gemspa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

