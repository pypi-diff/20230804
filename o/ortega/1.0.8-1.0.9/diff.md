# Comparing `tmp/ortega-1.0.8.tar.gz` & `tmp/ortega-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ortega-1.0.8.tar", last modified: Tue Jul 18 03:29:16 2023, max compression
+gzip compressed data, was "ortega-1.0.9.tar", last modified: Fri Aug  4 01:20:19 2023, max compression
```

## Comparing `ortega-1.0.8.tar` & `ortega-1.0.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:29:16.847339 ortega-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-18 03:29:05.000000 ortega-1.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-18 03:29:16.847339 ortega-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-07-18 03:29:05.000000 ortega-1.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:29:16.843339 ortega-1.0.8/ortega/
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-07-18 03:29:05.000000 ortega-1.0.8/ortega/STPoint.py
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-18 03:29:05.000000 ortega-1.0.8/ortega/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-07-18 03:29:05.000000 ortega-1.0.8/ortega/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     8448 2023-07-18 03:29:05.000000 ortega-1.0.8/ortega/ellipses.py
--rw-r--r--   0 runner    (1001) docker     (123)    31036 2023-07-18 03:29:05.000000 ortega-1.0.8/ortega/ortega.py
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-07-18 03:29:05.000000 ortega-1.0.8/ortega/output.py
--rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-07-18 03:29:05.000000 ortega-1.0.8/ortega/visualization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:29:16.843339 ortega-1.0.8/ortega.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-18 03:29:16.000000 ortega-1.0.8/ortega.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-07-18 03:29:16.000000 ortega-1.0.8/ortega.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 03:29:16.000000 ortega-1.0.8/ortega.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-18 03:29:16.000000 ortega-1.0.8/ortega.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-18 03:29:16.000000 ortega-1.0.8/ortega.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 03:29:16.847339 ortega-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-07-18 03:29:05.000000 ortega-1.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 01:20:19.359900 ortega-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-08-04 01:20:03.000000 ortega-1.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-08-04 01:20:19.359900 ortega-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-08-04 01:20:03.000000 ortega-1.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 01:20:19.359900 ortega-1.0.9/ortega/
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-08-04 01:20:03.000000 ortega-1.0.9/ortega/STPoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-08-04 01:20:03.000000 ortega-1.0.9/ortega/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-08-04 01:20:03.000000 ortega-1.0.9/ortega/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8448 2023-08-04 01:20:03.000000 ortega-1.0.9/ortega/ellipses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31177 2023-08-04 01:20:03.000000 ortega-1.0.9/ortega/ortega.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-08-04 01:20:03.000000 ortega-1.0.9/ortega/output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-08-04 01:20:03.000000 ortega-1.0.9/ortega/visualization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 01:20:19.359900 ortega-1.0.9/ortega.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-08-04 01:20:19.000000 ortega-1.0.9/ortega.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-08-04 01:20:19.000000 ortega-1.0.9/ortega.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 01:20:19.000000 ortega-1.0.9/ortega.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-08-04 01:20:19.000000 ortega-1.0.9/ortega.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-04 01:20:19.000000 ortega-1.0.9/ortega.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 01:20:19.359900 ortega-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-08-04 01:20:03.000000 ortega-1.0.9/setup.py
```

### Comparing `ortega-1.0.8/LICENSE` & `ortega-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ortega-1.0.8/README.md` & `ortega-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `ortega-1.0.8/ortega/STPoint.py` & `ortega-1.0.9/ortega/STPoint.py`

 * *Files identical despite different names*

### Comparing `ortega-1.0.8/ortega/ellipses.py` & `ortega-1.0.9/ortega/ellipses.py`

 * *Files identical despite different names*

### Comparing `ortega-1.0.8/ortega/ortega.py` & `ortega-1.0.9/ortega/ortega.py`

 * *Files 3% similar despite different names*

```diff
@@ -62,38 +62,38 @@
     :return:
     """
 
     def columns_names(e: Ellipse, num: int):
         as_dict = e.to_dict()
 
         return {
-            f"P{num}": as_dict["pid"],
-            f"P{num}_t_start": as_dict["t0"],
-            f"P{num}_t_end": as_dict["t1"],
-            f"P{num}_startlat": as_dict["last_lat"],
-            f"P{num}_startlon": as_dict["last_lon"],
-            f"P{num}_endlat": as_dict["lat"],
-            f"P{num}_endlon": as_dict["lon"],
-            f"P{num}_speed": as_dict["speed"],
-            f"P{num}_direction": as_dict["direction"]
+            f"p{num}": as_dict["pid"],
+            f"p{num}_t_start": as_dict["t0"],
+            f"p{num}_t_end": as_dict["t1"],
+            f"p{num}_startlat": as_dict["last_lat"],
+            f"p{num}_startlon": as_dict["last_lon"],
+            f"p{num}_endlat": as_dict["lat"],
+            f"p{num}_endlon": as_dict["lon"],
+            f"p{num}_speed": as_dict["speed"],
+            f"p{num}_direction": as_dict["direction"]
         }
 
     return pd.DataFrame(
         [
             {**columns_names(item, 1), **columns_names(item2, 2)}
             for item, item2 in intersection_df
         ]
     )
 
 
 def check_continuous(df: pd.DataFrame, id1: int, id2: int):
-    p1start = df['P1_t_start'].tolist()
-    p1end = df['P1_t_end'].tolist()
-    p2start = df['P2_t_start'].tolist()
-    p2end = df['P2_t_end'].tolist()
+    p1start = df['p1_t_start'].tolist()
+    p1end = df['p1_t_end'].tolist()
+    p2start = df['p2_t_start'].tolist()
+    p2end = df['p2_t_end'].tolist()
     p1_start_time, p1_end_time, p2_start_time, p2_end_time = [], [], [], []
     p1_start_index, p1_end_index = [], []
     p1_start_time.append(p1start[0])
     p1_start_index.append(0)
     for i in range(1, len(p1start)):
         if datetime.strptime(str(p1start[i]), '%Y-%m-%d %H:%M:%S') == datetime.strptime(str(p1start[i - 1]),
                                                                                         '%Y-%m-%d %H:%M:%S'):
@@ -169,35 +169,37 @@
     for i in range(0, len(p2_start_time_list)):
         for j in range(0, len(p2_start_time_list[i])):
             p1_start_column.append(p1_start_time[i])
             p1_end_column.append(p1_end_time[i])
             p2_start_column.append((p2_start_time_list[i])[j])
             p2_end_column.append((p2_end_time_list[i])[j])
 
-    d = {'P1 start': p1_start_column, 'P1 end': p1_end_column,
-         'P2 start': p2_start_column, 'P2 end': p2_end_column}
+    d = {'p1_start': p1_start_column, 'p1_end': p1_end_column,
+         'p2_start': p2_start_column, 'p2_end': p2_end_column}
     df_new = pd.DataFrame(d)
     diff_list = []
     for i in range(0, len(p1_start_column)):
         diff = pd.Timedelta(p2_start_column[i] - p1_start_column[i]).total_seconds()/60
         diff_list.append(diff)
-    df_new['Difference'] = diff_list
-    return df_new
+    df_new['difference'] = diff_list
+    df_new['p1'] = id1
+    df_new['p2'] = id2
+    return df_new[['p1', 'p2', 'p1_start', 'p1_end', 'p2_start', 'p2_end', 'difference']]
 
 
 def __merge_continuous_incident(df: pd.DataFrame, id1: int, id2: int):
     """
     Merge continuous interaction incidents after estimating duration
     :param df:
     :param id1:
     :param id2:
     :return:
     """
-    pstart = df['Start'].tolist()
-    pend = df['End'].tolist()
+    pstart = df['start'].tolist()
+    pend = df['end'].tolist()
     finalstart, finalend = [], []
     tag = []
     for i in range(0, len(pstart) - 1):
         if pend[i] >= pstart[i + 1]:
             tag.append(1)
         else:
             tag.append(0)
@@ -218,37 +220,37 @@
                 finalsub.append([pstart[j], pend[j]])
             subq = []
         j += 1
     for item in finalsub:
         finalstart.append(min(item))
         finalend.append(max(item))
 
-    df_new = pd.DataFrame(list(zip(finalstart, finalend)), columns=['Start', 'End'])
-    df_new['P1'] = id1
-    df_new['P2'] = id2
-    df_new['No'] = np.arange(df_new.shape[0]) + 1
-    df_new['Duration'] = df_new['End'] - df_new['Start']
-    df_new['Duration'] = df_new['Duration'].dt.total_seconds().div(60)
-    return df_new[['No', 'P1', 'P2', 'Start', 'End', 'Duration']]
+    df_new = pd.DataFrame(list(zip(finalstart, finalend)), columns=['start', 'end'])
+    df_new['p1'] = id1
+    df_new['p2'] = id2
+    df_new['no'] = np.arange(df_new.shape[0]) + 1
+    df_new['duration'] = df_new['ed'] - df_new['start']
+    df_new['duration'] = df_new['duration'].dt.total_seconds().div(60)
+    return df_new[['no', 'p1', 'p2', 'start', 'end', 'duration']]
 
 
 def durationEstimator(df: pd.DataFrame, id1: int, id2: int):
     """
     estimate duration of interation
     :param id2:
     :param id1:
     :param df:
     :return:
     """
-    p1start = df['P1_t_start'].tolist()
-    p1end = df['P1_t_end'].tolist()
-    p2start = df['P2_t_start'].tolist()
-    p2end = df['P2_t_end'].tolist()
+    p1start = df['p1_t_start'].tolist()
+    p1end = df['p1_t_end'].tolist()
+    p2start = df['p2_t_start'].tolist()
+    p2end = df['p2_t_end'].tolist()
     final_start, final_end, subsequenceOfInteraction = [], [], []
-    time_difference = [(df['P2_t_start'] - df['P1_t_start']) / pd.Timedelta(hours=1)]
+    time_difference = [(df['p2_t_start'] - df['p1_t_start']) / pd.Timedelta(hours=1)]
     time_group, diff_mean = [], []
     for i in range(0, len(p1start) - 1):  # identify subsequence of continuous interaction
         if datetime.strptime(str(p1start[i]), '%Y-%m-%d %H:%M:%S') == datetime.strptime(str(p1start[i + 1]),
                                                                                         '%Y-%m-%d %H:%M:%S'):
             subsequenceOfInteraction.extend([p1start[i], p1end[i], p1end[i + 1], p2start[i], p2end[i], p2start[i + 1],
                                              p2end[i + 1]])  # append all time in a candidate pool
             time_group.append(time_difference[0][i])
@@ -277,34 +279,34 @@
         final_end.append(max(subsequenceOfInteraction))
     if len(p1start) == 1:
         i = 0
         subsequenceOfInteraction.extend(
             [p1start[i], p1end[i], p2start[i], p2end[i]])  # append all time in a candidate pool
         final_start.append(min(subsequenceOfInteraction))
         final_end.append(max(subsequenceOfInteraction))
-    df_new = pd.DataFrame(list(zip(final_start, final_end)), columns=['Start', 'End'])
-    df_new['P1'] = id1
-    df_new['P2'] = id2
-    df_new['No'] = np.arange(df_new.shape[0]) + 1
-    df_new['Duration'] = df_new['End'] - df_new['Start']
-    df_new['Duration'] = df_new['Duration'].dt.total_seconds().div(60)
+    df_new = pd.DataFrame(list(zip(final_start, final_end)), columns=['start', 'end'])
+    df_new['p1'] = id1
+    df_new['p2'] = id2
+    df_new['no'] = np.arange(df_new.shape[0]) + 1
+    df_new['duration'] = df_new['end'] - df_new['start']
+    df_new['duration'] = df_new['duration'].dt.total_seconds().div(60)
     df_new = __merge_continuous_incident(df_new, id1, id2)
     #df_new['Mean_delay'] = diff_mean
-    return df_new[['No', 'P1', 'P2', 'Start', 'End', 'Duration']]
+    return df_new[['no', 'p1', 'p2', 'start', 'end', 'duration']]
 
 
 def interaction_compute_speed_diff(df: pd.DataFrame):
     """
     compute the percentage difference in speed between two moving entities
     this speed is based on the instant speed between two points not the average speed over a kernel
     :param df:
     :return:
     """
-    df['diff_speed'] = (df['P2_speed'] - df['P1_speed']).abs() / (
-            (df['P1_speed'] + df['P2_speed']) / 2)
+    df['diff_speed'] = (df['p2_speed'] - df['p1_speed']).abs() / (
+            (df['p1_speed'] + df['p2_speed']) / 2)
     # a higher value of percentage difference in speed indicates that two interacting entities move at
     # more different speeds
     return df
 
 
 def interaction_compute_direction_diff(df: pd.DataFrame):
     """
@@ -320,21 +322,21 @@
     #     if x[a] >= 180:
     #         x[a] -= 360
     #     if x[a] < -180:
     #         x[a] += 360
     #     x[a] = abs(x[a])
     #     return x
 
-    df['diff_direction'] = df['P2_direction'] - df['P1_direction']
+    df['diff_direction'] = df['p2_direction'] - df['p1_direction']
     df['diff_direction'] = df['diff_direction'].apply(math.cos)
     return df
 
 
 def interaction_compute_time_diff(df: pd.DataFrame):
-    df['diff_time'] = (df['P2_t_start'] - df['P1_t_start'])/ pd.Timedelta(minutes=1)
+    df['diff_time'] = (df['p2_t_start'] - df['p1_t_start'])/ pd.Timedelta(minutes=1)
     return df
 
 
 class ORTEGA:
     # ORTEGA is the main class for interaction analysis, users need to initialize this object at the very beginning
     def __init__(
             self,
@@ -557,17 +559,17 @@
             df_all_intersection_pairs = intersect_ellipse_todataframe(all_intersection_pairs)
             df_all_intersection_pairs = interaction_compute_speed_diff(df_all_intersection_pairs)
             df_all_intersection_pairs = interaction_compute_direction_diff(df_all_intersection_pairs)
             df_all_intersection_pairs = interaction_compute_time_diff(df_all_intersection_pairs)
             results.set_df_all_intersection_pairs(df_all_intersection_pairs)
 
             # compute duration of interaction and output as a dataframe - df_duration
-            print(datetime.now(), 'Compute continues events...')
+            print(datetime.now(), 'Compute continuous interaction events...')
             df_continues = check_continuous(df_all_intersection_pairs, self.id1, self.id2)
-            print(datetime.now(), f'Complete! {df_continues.shape[0]} interaction events identified!')
+            print(datetime.now(), f'Complete! {df_continues.shape[0]} continuous interaction events identified!')
             if df_continues.shape[0] != 0:
                 results.set_df_interaction_events(df_continues)
                 return results
             else:
                 return None
 
     def interaction_analysis2(self):
```

### Comparing `ortega-1.0.8/ortega/output.py` & `ortega-1.0.9/ortega/output.py`

 * *Files 17% similar despite different names*

```diff
@@ -21,9 +21,11 @@
     def set_df_all_intersection_pairs(self, row: pd.DataFrame):
         self.df_all_intersection_pairs = row
 
     def set_df_interaction_events(self, row: pd.DataFrame):
         self.df_interaction_events = row
 
     def compute_interaction_duration(self):
-        self.df_interaction_events['Duration'] = self.df_interaction_events[["P1 end", "P2 end"]].max(axis=1) - self.df_interaction_events[["P1 start", "P2 start"]].min(axis=1)
-        self.df_interaction_events['Duration'] = self.df_interaction_events['Duration'].dt.total_seconds().div(60)
+        self.df_interaction_events['duration'] = self.df_interaction_events[["p1_end", "p2_end"]].max(axis=1) - self.df_interaction_events[["p1_start", "p2_start"]].min(axis=1)
+        self.df_interaction_events['duration'] = self.df_interaction_events['duration'].dt.total_seconds().div(60)
+        print(datetime.now(), f'Computing interaction duration complete!')
+
```

### Comparing `ortega-1.0.8/ortega/visualization.py` & `ortega-1.0.9/ortega/visualization.py`

 * *Files identical despite different names*

### Comparing `ortega-1.0.8/setup.py` & `ortega-1.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 if __name__ == "__main__":
     setup(
         name='ortega',
-        version='1.0.8',
+        version='1.0.9',
         author='MOVE lab@UCSB',
         author_email="rongxiangsu@ucsb.edu",
         packages=["ortega"],
         url='https://github.com/move-ucsb/ORTEGA',
         license='MIT',
         description='ORTEGA',
         install_requires=[
```

