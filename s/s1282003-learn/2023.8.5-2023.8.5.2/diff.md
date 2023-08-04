# Comparing `tmp/s1282003_learn-2023.8.5.tar.gz` & `tmp/s1282003_learn-2023.8.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "s1282003_learn-2023.8.5.tar", last modified: Fri Aug  4 06:52:25 2023, max compression
+gzip compressed data, was "s1282003_learn-2023.8.5.2.tar", last modified: Fri Aug  4 07:05:04 2023, max compression
```

## Comparing `s1282003_learn-2023.8.5.tar` & `s1282003_learn-2023.8.5.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 s1282003 (18588) uday      (1000)        0 2023-08-04 06:52:25.030649 s1282003_learn-2023.8.5/
--rw-r--r--   0 s1282003 (18588) uday      (1000)    35823 2023-08-04 06:01:52.000000 s1282003_learn-2023.8.5/LICENSE
--rw-r--r--   0 s1282003 (18588) uday      (1000)      717 2023-08-04 06:52:25.030649 s1282003_learn-2023.8.5/PKG-INFO
--rw-r--r--   0 s1282003 (18588) uday      (1000)       16 2023-08-04 06:01:51.000000 s1282003_learn-2023.8.5/README.md
-drwxr-xr-x   0 s1282003 (18588) uday      (1000)        0 2023-08-04 06:52:25.030649 s1282003_learn-2023.8.5/s1282003_learn/
--rw-r--r--   0 s1282003 (18588) uday      (1000)        0 2023-08-04 06:02:15.000000 s1282003_learn-2023.8.5/s1282003_learn/__init__.py
-drwxr-xr-x   0 s1282003 (18588) uday      (1000)        0 2023-08-04 06:52:25.030649 s1282003_learn-2023.8.5/s1282003_learn/statistics/
--rw-r--r--   0 s1282003 (18588) uday      (1000)        0 2023-08-04 06:02:22.000000 s1282003_learn-2023.8.5/s1282003_learn/statistics/__init__.py
--rw-r--r--   0 s1282003 (18588) uday      (1000)     2284 2023-08-04 06:02:22.000000 s1282003_learn-2023.8.5/s1282003_learn/statistics/frequenciesOfItems.py
-drwxr-xr-x   0 s1282003 (18588) uday      (1000)        0 2023-08-04 06:52:25.030649 s1282003_learn-2023.8.5/s1282003_learn/visualization/
--rw-r--r--   0 s1282003 (18588) uday      (1000)        0 2023-08-04 06:02:33.000000 s1282003_learn-2023.8.5/s1282003_learn/visualization/__init__.py
--rw-r--r--   0 s1282003 (18588) uday      (1000)     4754 2023-08-04 06:46:00.000000 s1282003_learn-2023.8.5/s1282003_learn/visualization/heatMapItemsFrequencies.py
-drwxr-xr-x   0 s1282003 (18588) uday      (1000)        0 2023-08-04 06:52:25.030649 s1282003_learn-2023.8.5/s1282003_learn.egg-info/
--rw-r--r--   0 s1282003 (18588) uday      (1000)      717 2023-08-04 06:52:25.000000 s1282003_learn-2023.8.5/s1282003_learn.egg-info/PKG-INFO
--rw-r--r--   0 s1282003 (18588) uday      (1000)      425 2023-08-04 06:52:25.000000 s1282003_learn-2023.8.5/s1282003_learn.egg-info/SOURCES.txt
--rw-r--r--   0 s1282003 (18588) uday      (1000)        1 2023-08-04 06:52:25.000000 s1282003_learn-2023.8.5/s1282003_learn.egg-info/dependency_links.txt
--rw-r--r--   0 s1282003 (18588) uday      (1000)      194 2023-08-04 06:52:25.000000 s1282003_learn-2023.8.5/s1282003_learn.egg-info/requires.txt
--rw-r--r--   0 s1282003 (18588) uday      (1000)       15 2023-08-04 06:52:25.000000 s1282003_learn-2023.8.5/s1282003_learn.egg-info/top_level.txt
--rw-r--r--   0 s1282003 (18588) uday      (1000)       38 2023-08-04 06:52:25.030649 s1282003_learn-2023.8.5/setup.cfg
--rw-r--r--   0 s1282003 (18588) uday      (1000)     1302 2023-08-04 06:51:45.000000 s1282003_learn-2023.8.5/setup.py
+drwxr-xr-x   0 s1282003 (18588) uday      (1000)        0 2023-08-04 07:05:04.663482 s1282003_learn-2023.8.5.2/
+-rw-r--r--   0 s1282003 (18588) uday      (1000)    35823 2023-08-04 06:01:52.000000 s1282003_learn-2023.8.5.2/LICENSE
+-rw-r--r--   0 s1282003 (18588) uday      (1000)      719 2023-08-04 07:05:04.663482 s1282003_learn-2023.8.5.2/PKG-INFO
+-rw-r--r--   0 s1282003 (18588) uday      (1000)       16 2023-08-04 06:01:51.000000 s1282003_learn-2023.8.5.2/README.md
+drwxr-xr-x   0 s1282003 (18588) uday      (1000)        0 2023-08-04 07:05:04.663482 s1282003_learn-2023.8.5.2/s1282003_learn/
+-rw-r--r--   0 s1282003 (18588) uday      (1000)        0 2023-08-04 06:02:15.000000 s1282003_learn-2023.8.5.2/s1282003_learn/__init__.py
+drwxr-xr-x   0 s1282003 (18588) uday      (1000)        0 2023-08-04 07:05:04.663482 s1282003_learn-2023.8.5.2/s1282003_learn/statistics/
+-rw-r--r--   0 s1282003 (18588) uday      (1000)        0 2023-08-04 06:02:22.000000 s1282003_learn-2023.8.5.2/s1282003_learn/statistics/__init__.py
+-rw-r--r--   0 s1282003 (18588) uday      (1000)     2284 2023-08-04 06:02:22.000000 s1282003_learn-2023.8.5.2/s1282003_learn/statistics/frequenciesOfItems.py
+drwxr-xr-x   0 s1282003 (18588) uday      (1000)        0 2023-08-04 07:05:04.663482 s1282003_learn-2023.8.5.2/s1282003_learn/visualization/
+-rw-r--r--   0 s1282003 (18588) uday      (1000)        0 2023-08-04 06:02:33.000000 s1282003_learn-2023.8.5.2/s1282003_learn/visualization/__init__.py
+-rw-r--r--   0 s1282003 (18588) uday      (1000)     4591 2023-08-04 07:04:09.000000 s1282003_learn-2023.8.5.2/s1282003_learn/visualization/heatMapItemsFrequencies.py
+drwxr-xr-x   0 s1282003 (18588) uday      (1000)        0 2023-08-04 07:05:04.663482 s1282003_learn-2023.8.5.2/s1282003_learn.egg-info/
+-rw-r--r--   0 s1282003 (18588) uday      (1000)      719 2023-08-04 07:05:04.000000 s1282003_learn-2023.8.5.2/s1282003_learn.egg-info/PKG-INFO
+-rw-r--r--   0 s1282003 (18588) uday      (1000)      425 2023-08-04 07:05:04.000000 s1282003_learn-2023.8.5.2/s1282003_learn.egg-info/SOURCES.txt
+-rw-r--r--   0 s1282003 (18588) uday      (1000)        1 2023-08-04 07:05:04.000000 s1282003_learn-2023.8.5.2/s1282003_learn.egg-info/dependency_links.txt
+-rw-r--r--   0 s1282003 (18588) uday      (1000)      194 2023-08-04 07:05:04.000000 s1282003_learn-2023.8.5.2/s1282003_learn.egg-info/requires.txt
+-rw-r--r--   0 s1282003 (18588) uday      (1000)       15 2023-08-04 07:05:04.000000 s1282003_learn-2023.8.5.2/s1282003_learn.egg-info/top_level.txt
+-rw-r--r--   0 s1282003 (18588) uday      (1000)       38 2023-08-04 07:05:04.663482 s1282003_learn-2023.8.5.2/setup.cfg
+-rw-r--r--   0 s1282003 (18588) uday      (1000)     1304 2023-08-04 07:04:37.000000 s1282003_learn-2023.8.5.2/setup.py
```

### Comparing `s1282003_learn-2023.8.5/LICENSE` & `s1282003_learn-2023.8.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `s1282003_learn-2023.8.5/PKG-INFO` & `s1282003_learn-2023.8.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: s1282003_learn
-Version: 2023.8.5
+Version: 2023.8.5.2
 Summary: This software is being developed at the University of Aizu, Aizu-Wakamatsu, Fukushima, Japan
 Home-page: https://github.com/angelitagozaly/s1282003_learn
 Author: Angelita Gozaly
 Author-email: s1282003@u-aizu.ac.jp
 License: GPLv3
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `s1282003_learn-2023.8.5/s1282003_learn/statistics/frequenciesOfItems.py` & `s1282003_learn-2023.8.5.2/s1282003_learn/statistics/frequenciesOfItems.py`

 * *Files identical despite different names*

### Comparing `s1282003_learn-2023.8.5/s1282003_learn/visualization/heatMapItemsFrequencies.py` & `s1282003_learn-2023.8.5.2/s1282003_learn/visualization/heatMapItemsFrequencies.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import plotly.express as px
-from s1282003_learn.statistics.frequenciesOfItems import frequenciesOfItems
-
+from s1282003_learn.visualization.heatMapItemsFrequencies import frequenciesOfItems
 
 class HeatMapItemsFrequencies:
     """
     A class to create a heatmap of item frequencies at specific geographical coordinates.
 
     Attributes
     ----------
@@ -20,27 +19,27 @@
     extract_coordinates_from_point(point_str)
         Extracts latitude and longitude coordinates from the given point string.
     process_file()
         Processes the CSV file and gets the items frequencies dictionary.
     plot_heatmap()
         Plots a heatmap using Plotly Express based on the items frequencies dictionary.
     """
-
+    
     def __init__(self, filename, separator):
         """
         Initializes the HeatMapItemsFrequencies class.
 
         Parameters
         ----------
         filename
             The name of the CSV file containing transactional database.
         separator
             The separator used in the CSV file to separate values.
         """
-
+        
         self.filename = filename
         self.separator = separator
 
     def extract_coordinates_from_point(self, point_str):
         """
         Extracts latitude and longitude coordinates from the given point string in the frequency dictionary.
 
@@ -52,15 +51,15 @@
         Returns
         -------
         coordinates
             A list of tuples containing latitude and longitude coordinates.
         """
 
         # Separate each points and extract the coordinates
-        points = point_str.split("\t")
+        points = point_str.split('\t')
         coordinates = []
         for point in points:
             lon, lat = map(float, point[6:-3].split())
             coordinates.append((lon, lat))
         return coordinates
 
     def process_file(self):
@@ -68,26 +67,24 @@
         Use the frequenciesOfItem class to process the transactional database and gets the items frequencies dictionary.
 
         Returns
         -------
         items_frequencies_dict
             A dictionary containing items as keys and their corresponding frequencies as values.
         """
-
+        
         # Call the process_file() method of the frequenciesOfItems class to get the output dictionary
-        items_frequencies_dict = frequenciesOfItems(
-            self.filename, self.separator
-        ).process_file()
+        items_frequencies_dict = frequenciesOfItems(self.filename, self.separator).process_file()
         return items_frequencies_dict
 
     def plot_heatmap(self):
         """
         Plots a heatmap using Plotly Express based on the items frequencies dictionary.
         """
-
+        
         # Call the process_file() method to get the output dictionary
         items_frequencies_dict = self.process_file()
 
         if items_frequencies_dict is not None:
             # Extract latitude and longitude from the dictionary keys
             latitudes = []
             longitudes = []
@@ -99,42 +96,31 @@
                 for lon, lat in coordinates:
                     longitudes.append(lon)
                     latitudes.append(lat)
                     frequencies.append(frequency)
 
             # Create a DataFrame to be used by Plotly Express
             import pandas as pd
-
-            data = pd.DataFrame(
-                {
-                    "Latitude": latitudes,
-                    "Longitude": longitudes,
-                    "Frequency": frequencies,
-                }
-            )
+            data = pd.DataFrame({'Latitude': latitudes, 'Longitude': longitudes, 'Frequency': frequencies})
 
             # Create a heatmap on an OpenStreetMap using Plotly Express
             fig = px.density_mapbox(
-                data,
-                lat="Latitude",
-                lon="Longitude",
-                z="Frequency",
+                data, lat='Latitude', lon='Longitude', z='Frequency',
                 radius=10,
-                center={"lat": 36.686567, "lon": 135.52000},
+                center={'lat':36.686567, 'lon':135.52000},
                 zoom=3.8,
                 height=600,
                 width=800,
-                mapbox_style="open-street-map",
+                mapbox_style="open-street-map"
             )
 
             # Show the plot
             fig.show()
 
         else:
             print("Error occurred while processing the file.")
 
-
 if __name__ == "__main__":
-    filename = "PM24HeavyPollutionRecordingSensors.csv"
-    separator = "\t"
+    filename = 'PM24HeavyPollutionRecordingSensors.csv'
+    separator = '\t'
     heatmap = HeatMapItemsFrequencies(filename, separator)
     heatmap.plot_heatmap()
```

### Comparing `s1282003_learn-2023.8.5/s1282003_learn.egg-info/PKG-INFO` & `s1282003_learn-2023.8.5.2/s1282003_learn.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: s1282003-learn
-Version: 2023.8.5
+Version: 2023.8.5.2
 Summary: This software is being developed at the University of Aizu, Aizu-Wakamatsu, Fukushima, Japan
 Home-page: https://github.com/angelitagozaly/s1282003_learn
 Author: Angelita Gozaly
 Author-email: s1282003@u-aizu.ac.jp
 License: GPLv3
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `s1282003_learn-2023.8.5/setup.py` & `s1282003_learn-2023.8.5.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="s1282003_learn",
-    version="2023.08.05",
+    version="2023.08.05.2",
     author="Angelita Gozaly",
     author_email="s1282003@u-aizu.ac.jp",
     description="This software is being developed at the University of Aizu, Aizu-Wakamatsu, Fukushima, Japan",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     url="https://github.com/angelitagozaly/s1282003_learn",
```

