# Comparing `tmp/inviz-0.2.4.tar.gz` & `tmp/inviz-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inviz-0.2.4.tar", last modified: Wed Jul 19 02:04:55 2023, max compression
+gzip compressed data, was "inviz-0.2.5.tar", last modified: Fri Aug  4 04:41:17 2023, max compression
```

## Comparing `inviz-0.2.4.tar` & `inviz-0.2.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 jswen     (1000) jswen     (1000)        0 2023-07-19 02:04:55.539195 inviz-0.2.4/
--rw-r--r--   0 jswen     (1000) jswen     (1000)     1066 2023-03-27 21:46:04.000000 inviz-0.2.4/LICENSE
--rw-r--r--   0 jswen     (1000) jswen     (1000)       42 2023-03-27 21:46:04.000000 inviz-0.2.4/MANIFEST.in
--rw-r--r--   0 jswen     (1000) jswen     (1000)     2163 2023-07-19 02:04:55.539195 inviz-0.2.4/PKG-INFO
--rw-r--r--   0 jswen     (1000) jswen     (1000)     1642 2023-07-13 22:19:19.000000 inviz-0.2.4/README.md
-drwxr-xr-x   0 jswen     (1000) jswen     (1000)        0 2023-07-19 02:04:55.539195 inviz-0.2.4/inviz/
-drwxr-xr-x   0 jswen     (1000) jswen     (1000)        0 2023-07-19 02:04:55.539195 inviz-0.2.4/inviz/inviz.egg-info/
--rw-r--r--   0 jswen     (1000) jswen     (1000)     2163 2023-07-19 02:04:55.000000 inviz-0.2.4/inviz/inviz.egg-info/PKG-INFO
--rw-r--r--   0 jswen     (1000) jswen     (1000)      227 2023-07-19 02:04:55.000000 inviz-0.2.4/inviz/inviz.egg-info/SOURCES.txt
--rw-r--r--   0 jswen     (1000) jswen     (1000)        1 2023-07-19 02:04:55.000000 inviz-0.2.4/inviz/inviz.egg-info/dependency_links.txt
--rw-r--r--   0 jswen     (1000) jswen     (1000)      103 2023-07-19 02:04:55.000000 inviz-0.2.4/inviz/inviz.egg-info/requires.txt
--rw-r--r--   0 jswen     (1000) jswen     (1000)        6 2023-07-19 02:04:55.000000 inviz-0.2.4/inviz/inviz.egg-info/top_level.txt
--rwxr-xr-x   0 jswen     (1000) jswen     (1000)    10791 2023-07-19 02:02:33.000000 inviz-0.2.4/inviz/inviz.py
--rw-r--r--   0 jswen     (1000) jswen     (1000)       38 2023-07-19 02:04:55.539195 inviz-0.2.4/setup.cfg
--rw-r--r--   0 jswen     (1000) jswen     (1000)     1139 2023-07-19 02:02:33.000000 inviz-0.2.4/setup.py
+drwxr-xr-x   0 jswen     (1000) jswen     (1000)        0 2023-08-04 04:41:17.619294 inviz-0.2.5/
+-rw-r--r--   0 jswen     (1000) jswen     (1000)     1066 2023-03-27 21:46:04.000000 inviz-0.2.5/LICENSE
+-rw-r--r--   0 jswen     (1000) jswen     (1000)       42 2023-03-27 21:46:04.000000 inviz-0.2.5/MANIFEST.in
+-rw-r--r--   0 jswen     (1000) jswen     (1000)     2163 2023-08-04 04:41:17.609294 inviz-0.2.5/PKG-INFO
+-rw-r--r--   0 jswen     (1000) jswen     (1000)     1642 2023-07-13 22:19:19.000000 inviz-0.2.5/README.md
+drwxr-xr-x   0 jswen     (1000) jswen     (1000)        0 2023-08-04 04:41:17.609294 inviz-0.2.5/inviz/
+drwxr-xr-x   0 jswen     (1000) jswen     (1000)        0 2023-08-04 04:41:17.609294 inviz-0.2.5/inviz/inviz.egg-info/
+-rw-r--r--   0 jswen     (1000) jswen     (1000)     2163 2023-08-04 04:41:17.000000 inviz-0.2.5/inviz/inviz.egg-info/PKG-INFO
+-rw-r--r--   0 jswen     (1000) jswen     (1000)      227 2023-08-04 04:41:17.000000 inviz-0.2.5/inviz/inviz.egg-info/SOURCES.txt
+-rw-r--r--   0 jswen     (1000) jswen     (1000)        1 2023-08-04 04:41:17.000000 inviz-0.2.5/inviz/inviz.egg-info/dependency_links.txt
+-rw-r--r--   0 jswen     (1000) jswen     (1000)      119 2023-08-04 04:41:17.000000 inviz-0.2.5/inviz/inviz.egg-info/requires.txt
+-rw-r--r--   0 jswen     (1000) jswen     (1000)        6 2023-08-04 04:41:17.000000 inviz-0.2.5/inviz/inviz.egg-info/top_level.txt
+-rwxr-xr-x   0 jswen     (1000) jswen     (1000)    11241 2023-08-04 04:36:54.000000 inviz-0.2.5/inviz/inviz.py
+-rw-r--r--   0 jswen     (1000) jswen     (1000)       38 2023-08-04 04:41:17.619294 inviz-0.2.5/setup.cfg
+-rw-r--r--   0 jswen     (1000) jswen     (1000)     1180 2023-08-04 04:36:54.000000 inviz-0.2.5/setup.py
```

### Comparing `inviz-0.2.4/LICENSE` & `inviz-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `inviz-0.2.4/PKG-INFO` & `inviz-0.2.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inviz
-Version: 0.2.4
+Version: 0.2.5
 Summary: An interactive visualizer to help explore high-dimensional data and its observables.
 Home-page: http://packages.python.org/inviz
 Author: James Wen
 Author-email: jswen@usc.edu
 License: MIT
 Keywords: interactive visualizer cosmology
 Classifier: Programming Language :: Python :: 3
```

### Comparing `inviz-0.2.4/README.md` & `inviz-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `inviz-0.2.4/inviz/inviz.egg-info/PKG-INFO` & `inviz-0.2.5/inviz/inviz.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inviz
-Version: 0.2.4
+Version: 0.2.5
 Summary: An interactive visualizer to help explore high-dimensional data and its observables.
 Home-page: http://packages.python.org/inviz
 Author: James Wen
 Author-email: jswen@usc.edu
 License: MIT
 Keywords: interactive visualizer cosmology
 Classifier: Programming Language :: Python :: 3
```

### Comparing `inviz-0.2.4/inviz/inviz.py` & `inviz-0.2.5/inviz/inviz.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,14 +7,39 @@
 from bokeh.models import HoverTool
 from typing import List, Callable, Union
 
 hv.extension('bokeh')
 pn.extension()
 
 
+# unpacks the nested data. handles the two supported datatypes
+def unpacker(dataset, index):
+    if isinstance(dataset, dict):
+        unpacked_data = {key: dataset[key][index] for key in dataset.keys()}
+    if isinstance(dataset, pd.core.frame.DataFrame):
+        columns = dataset.columns
+        dataseries = dataset.iloc[index]
+        unpacked_data = pd.DataFrame({columns[item]: dataseries[columns[item]] for item in range(len(columns))})
+    return unpacked_data
+
+
+#  given a param name, find corresponding latex-formatted param name
+def lookup_latex_label(param, latex_dict):
+    # handle default case of no latex paramname dictionary
+    if latex_dict is None:
+        latex_dict = dict()
+    try:
+        latex_param = latex_dict[param]
+        label = r'$${}$$'.format(latex_param)
+        return label
+    except KeyError:
+        label = param
+        return label
+    
+
 class Observable:
     """
     Observable class for InViz.
     
     Parameters
     ----------
     name: string or list of strings
@@ -26,30 +51,30 @@
 
     latex_labels: dict or list of dicts
         key: value -> parameter label: latex version. parameter label must match the
         corresponding one in the parameters dict
 
     myfunc: callable
         a user-provided function that returns parameters. can return more than one
-        set of parameters if the "grouped" option is True
+        set of parameters.
 
     myfunc_args: tuple
         arguments for user-provided function
 
     plot_type: string
         specifies how the data should be visualized. currently can pick either 'Curve'
         or 'Scatter'
 
     plot_opts: holoviews Options object
         customization options for the observable plot. see Holoviews documentation
     """
     
     def __init__(
         self, 
-        name: Union[str, List[str]] = None, 
+        name: Union[str, List[str]], 
         parameters: Union[dict, List[dict]] = None, 
         myfunc: Callable = None,
         myfunc_args: tuple = None, 
         plot_type: Union[str, List[str]] = None,
         plot_opts: Union[opts, List[opts]] = None,
         latex_labels: dict = None
     ):
@@ -88,27 +113,26 @@
         if self.myfunc and self.myfunc_args is not None:
             computed_data = self.myfunc(index, *self.myfunc_args)
             self.number = len(computed_data)
         for i in range(0, self.number):
             hv_element = getattr(hv, self.plot_type[i])
             if self.parameters is not None:
                 dataset = self.parameters[i]
-                kdim = list(dataset.keys())[0]
-                vdim = list(dataset.keys())[1]
-                indexed_data = (dataset[kdim][index], dataset[vdim][index])
-                plot = hv_element(indexed_data, kdim, vdim, label=self.name[i])
+                unpacked_data = unpacker(dataset, index)
+                kdim, vdim = unpacked_data.keys()
+                plot = hv_element(unpacked_data, kdim, vdim, label=self.name[i])
             elif computed_data:
                 dataset = computed_data[i]
-                kdim = list(dataset.keys())[0]
-                vdim = list(dataset.keys())[1]
+                kdim, vdim = dataset.keys()
                 plot = hv_element(dataset, kdim, vdim, label=self.name[i])
             # set defaults
             plot.opts(
                 height=400,
                 width=500,
+                padding=0.1,
                 fontscale=1.1,
                 xlabel=lookup_latex_label(kdim, self.latex_labels), 
                 ylabel=lookup_latex_label(vdim, self.latex_labels),
                 framewise=True
             )
             # add user defined customizations
             if self.plot_opts and self.plot_opts[i] is not None:
@@ -117,48 +141,35 @@
         return self.plots_list
         
     def draw_plot(self, index):
         layout = hv.Layout(self.generate_plot(index))
         return layout.opts(shared_axes=False)
         
 
-#  given a param name, find corresponding latex-formatted param name
-def lookup_latex_label(param, latex_dict):
-    # handle default case of no latex paramname dictionary
-    if latex_dict is None:
-        latex_dict = dict()
-    try:
-        latex_param = latex_dict[param]
-        label = r'$${}$$'.format(latex_param)
-        return label
-    except KeyError:
-        label = param
-        return label
-
-
+# generate the visualization
 def viz(
     data, 
     observables: list = None, 
     show_observables: bool = True, 
     latex_dict: dict = None
 ):
     # setting Panel widgets for user interaction
     variables = data.columns.values.tolist()
     var1 = pn.widgets.Select(
-        value=variables[1], 
+        value=variables[0], 
         name='Horizontal Axis', 
         options=variables
     )
     var2 = pn.widgets.Select(
-        value=variables[2], 
+        value=variables[1], 
         name='Vertical Axis', 
         options=variables
     )
     cmap_var = pn.widgets.Select(
-        value=variables[0], 
+        value=variables[2], 
         name='Colormapped Parameter', 
         options=variables
     )
     cmap_option = pn.widgets.Checkbox(
         value=True, 
         name='Show Colormap', 
         align='end'
@@ -228,14 +239,16 @@
     
     #table_stream = streams.Selection1D(source=selected_table)
     
     # handles the null selection case and multiple selections
     plots = {}
     # get total number of plots to draw from list of observables
     plotting_info = {}
+    if observables is None:
+        observables = []
     for each in observables:
         for i in range(len(each.name)):
             if each.plot_opts is None:
                 specific_opts = None
             elif each.plot_opts[i] is not None:
                 specific_opts = each.plot_opts[i]
             plotting_info[each.name[i]] = {'type': each.plot_type[i], 'opts': specific_opts}
```

### Comparing `inviz-0.2.4/setup.py` & `inviz-0.2.5/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "inviz",
-    version = "0.2.4",
+    version = "0.2.5",
     author = "James Wen",
     author_email = "jswen@usc.edu",
     description = ("An interactive visualizer to help explore high-dimensional data and its observables."),
     license = "MIT",
     keywords = "interactive visualizer cosmology",
     url = "http://packages.python.org/inviz",
     py_modules=["inviz"],
@@ -23,13 +23,14 @@
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: POSIX :: Linux",
     ],
     python_requires='>=3.8',
     install_requires=["holoviews==1.15.4",
                       "panel==0.14.4",
-                      "spatialpandas==0.4.7",
+                      "spatialpandas==0.4.8",
+                      "dask<=2023.5.0",
                       "param==1.13.0",
-                      "numpy>=1.20, <1.24",
+                      "numpy>=1.21, <=1.24",
                       "matplotlib==3.7.1"]
     )
```

