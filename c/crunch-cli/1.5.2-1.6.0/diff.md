# Comparing `tmp/crunch-cli-1.5.2.tar.gz` & `tmp/crunch-cli-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crunch-cli-1.5.2.tar", last modified: Tue Jul  4 11:12:20 2023, max compression
+gzip compressed data, was "crunch-cli-1.6.0.tar", last modified: Fri Aug  4 14:54:44 2023, max compression
```

## Comparing `crunch-cli-1.5.2.tar` & `crunch-cli-1.6.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 11:12:20.901894 crunch-cli-1.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-07-04 11:12:20.901894 crunch-cli-1.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-04 11:12:15.000000 crunch-cli-1.5.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 11:12:20.897894 crunch-cli-1.5.2/crunch/
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-04 11:12:15.000000 crunch-cli-1.5.2/crunch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-04 11:12:15.000000 crunch-cli-1.5.2/crunch/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-07-04 11:12:15.000000 crunch-cli-1.5.2/crunch/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 11:12:20.897894 crunch-cli-1.5.2/crunch/command/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-04 11:12:15.000000 crunch-cli-1.5.2/crunch/command/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-07-04 11:12:15.000000 crunch-cli-1.5.2/crunch/command/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-07-04 11:12:15.000000 crunch-cli-1.5.2/crunch/command/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-07-04 11:12:15.000000 crunch-cli-1.5.2/crunch/command/push.py
--rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-07-04 11:12:15.000000 crunch-cli-1.5.2/crunch/command/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-07-04 11:12:15.000000 crunch-cli-1.5.2/crunch/command/test.py
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-07-04 11:12:15.000000 crunch-cli-1.5.2/crunch/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 11:12:20.897894 crunch-cli-1.5.2/crunch/demo-project/
--rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-07-04 11:12:15.000000 crunch-cli-1.5.2/crunch/demo-project/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-04 11:12:15.000000 crunch-cli-1.5.2/crunch/demo-project/files.json
--rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-07-04 11:12:15.000000 crunch-cli-1.5.2/crunch/demo-project/main.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-04 11:12:15.000000 crunch-cli-1.5.2/crunch/demo-project/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-07-04 11:12:15.000000 crunch-cli-1.5.2/crunch/ensure.py
--rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-07-04 11:12:15.000000 crunch-cli-1.5.2/crunch/inline.py
--rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-07-04 11:12:15.000000 crunch-cli-1.5.2/crunch/library.py
--rw-r--r--   0 runner    (1001) docker     (123)     6465 2023-07-04 11:12:15.000000 crunch-cli-1.5.2/crunch/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-07-04 11:12:15.000000 crunch-cli-1.5.2/crunch/tester.py
--rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-07-04 11:12:15.000000 crunch-cli-1.5.2/crunch/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 11:12:20.901894 crunch-cli-1.5.2/crunch_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-07-04 11:12:20.000000 crunch-cli-1.5.2/crunch_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-04 11:12:20.000000 crunch-cli-1.5.2/crunch_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 11:12:20.000000 crunch-cli-1.5.2/crunch_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-04 11:12:20.000000 crunch-cli-1.5.2/crunch_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 11:12:20.000000 crunch-cli-1.5.2/crunch_cli.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-04 11:12:20.000000 crunch-cli-1.5.2/crunch_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-04 11:12:20.000000 crunch-cli-1.5.2/crunch_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 11:12:20.901894 crunch-cli-1.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-07-04 11:12:15.000000 crunch-cli-1.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 14:54:44.492797 crunch-cli-1.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-08-04 14:54:44.492797 crunch-cli-1.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-08-04 14:54:35.000000 crunch-cli-1.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 14:54:44.488798 crunch-cli-1.6.0/crunch/
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-08-04 14:54:35.000000 crunch-cli-1.6.0/crunch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-08-04 14:54:35.000000 crunch-cli-1.6.0/crunch/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-08-04 14:54:35.000000 crunch-cli-1.6.0/crunch/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 14:54:44.492797 crunch-cli-1.6.0/crunch/command/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-08-04 14:54:35.000000 crunch-cli-1.6.0/crunch/command/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-08-04 14:54:35.000000 crunch-cli-1.6.0/crunch/command/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-08-04 14:54:35.000000 crunch-cli-1.6.0/crunch/command/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-08-04 14:54:35.000000 crunch-cli-1.6.0/crunch/command/push.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-08-04 14:54:35.000000 crunch-cli-1.6.0/crunch/command/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-08-04 14:54:35.000000 crunch-cli-1.6.0/crunch/command/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-08-04 14:54:35.000000 crunch-cli-1.6.0/crunch/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 14:54:44.492797 crunch-cli-1.6.0/crunch/demo-project/
+-rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-08-04 14:54:35.000000 crunch-cli-1.6.0/crunch/demo-project/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-04 14:54:35.000000 crunch-cli-1.6.0/crunch/demo-project/files.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-08-04 14:54:35.000000 crunch-cli-1.6.0/crunch/demo-project/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-04 14:54:35.000000 crunch-cli-1.6.0/crunch/demo-project/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-08-04 14:54:35.000000 crunch-cli-1.6.0/crunch/ensure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-08-04 14:54:35.000000 crunch-cli-1.6.0/crunch/inline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-08-04 14:54:35.000000 crunch-cli-1.6.0/crunch/library.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6465 2023-08-04 14:54:35.000000 crunch-cli-1.6.0/crunch/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-08-04 14:54:35.000000 crunch-cli-1.6.0/crunch/tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-08-04 14:54:35.000000 crunch-cli-1.6.0/crunch/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 14:54:44.492797 crunch-cli-1.6.0/crunch_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-08-04 14:54:44.000000 crunch-cli-1.6.0/crunch_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-08-04 14:54:44.000000 crunch-cli-1.6.0/crunch_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 14:54:44.000000 crunch-cli-1.6.0/crunch_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-08-04 14:54:44.000000 crunch-cli-1.6.0/crunch_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 14:54:44.000000 crunch-cli-1.6.0/crunch_cli.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-04 14:54:44.000000 crunch-cli-1.6.0/crunch_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-04 14:54:44.000000 crunch-cli-1.6.0/crunch_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 14:54:44.492797 crunch-cli-1.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-08-04 14:54:35.000000 crunch-cli-1.6.0/setup.py
```

### Comparing `crunch-cli-1.5.2/crunch/command/convert.py` & `crunch-cli-1.6.0/crunch/command/convert.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.5.2/crunch/command/download.py` & `crunch-cli-1.6.0/crunch/command/download.py`

 * *Files 10% similar despite different names*

```diff
@@ -66,21 +66,23 @@
         signed = data_file["signed"]
 
         return DataFile(url, path, size, signed)
 
     x_train = get_file("xTrain", "X_train")
     y_train = get_file("yTrain", "y_train")
     x_test = get_file("xTest", "X_test")
+    y_test = get_file("yTest", "y_test")
 
     return (
         embargo,
         moon_column_name,
         x_train,
         y_train,
-        x_test
+        x_test,
+        y_test
     )
 
 
 def _download(data_file: DataFile, force: bool):
     print(f"download {data_file.path} from {cut_url(data_file.url)}")
 
     exists = os.path.exists(data_file.path)
@@ -115,27 +117,30 @@
     os.makedirs(constants.DOT_DATA_DIRECTORY, exist_ok=True)
 
     (
         embargo,
         moon_column_name,
         x_train,
         y_train,
-        x_test
+        x_test,
+        y_test
     ) = get_data_urls(session, constants.DOT_DATA_DIRECTORY, push_token)
 
     _download(x_train, force)
     _download(y_train, force)
     _download(x_test, force)
+    _download(y_test, force)
 
     return (
         embargo,
         moon_column_name,
         x_train.path,
         y_train.path,
-        x_test.path
+        x_test.path,
+        y_test.path
     )
 
 
 def download_no_data_available():
     today = datetime.date.today()
 
     print("\n---")
```

### Comparing `crunch-cli-1.5.2/crunch/command/push.py` & `crunch-cli-1.6.0/crunch/command/push.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.5.2/crunch/command/setup.py` & `crunch-cli-1.6.0/crunch/command/setup.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.5.2/crunch/command/test.py` & `crunch-cli-1.6.0/crunch/command/test.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.5.2/crunch/constants.py` & `crunch-cli-1.6.0/crunch/constants.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.5.2/crunch/demo-project/.gitignore` & `crunch-cli-1.6.0/crunch/demo-project/.gitignore`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.5.2/crunch/demo-project/main.py` & `crunch-cli-1.6.0/crunch/demo-project/main.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.5.2/crunch/ensure.py` & `crunch-cli-1.6.0/crunch/ensure.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.5.2/crunch/inline.py` & `crunch-cli-1.6.0/crunch/inline.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,19 +22,20 @@
         )
 
         print(f"loaded inline runner with module: {module}")
 
     def load_data(self) -> typing.Tuple[pandas.DataFrame, pandas.DataFrame, pandas.DataFrame]:
         try:
             (
-                _,
-                _,
+                _, # embargo
+                _, # moon_column_name
                 x_train_path,
                 y_train_path,
-                x_test_path
+                x_test_path,
+                _ # y_test_path
             ) = command.download(self.session)
         except api.CurrentCrunchNotFoundException:
             command.download_no_data_available()
             raise click.Abort()
 
         x_train = utils.read(x_train_path)
         y_train = utils.read(y_train_path)
```

### Comparing `crunch-cli-1.5.2/crunch/library.py` & `crunch-cli-1.6.0/crunch/library.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.5.2/crunch/main.py` & `crunch-cli-1.6.0/crunch/main.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.5.2/crunch/tester.py` & `crunch-cli-1.6.0/crunch/tester.py`

 * *Files 10% similar despite different names*

```diff
@@ -62,49 +62,59 @@
 
     try:
         (
             embargo,
             moon_column_name,
             x_train_path,
             y_train_path,
-            x_test_path
+            x_test_path,
+            y_test_path
         ) = command.download(session)
     except api.CurrentCrunchNotFoundException:
         command.download_no_data_available()
         raise click.Abort()
 
-    x_train = utils.read(x_train_path)
-    y_train = utils.read(y_train_path)
     x_test = utils.read(x_test_path)
-
     moons = x_test[moon_column_name].unique()
     moons.sort()
 
-    for dataframe in [x_train, y_train, x_test]:
+    full_x = pandas.concat([
+        utils.read(x_train_path),
+        x_test,
+    ])
+
+    full_y = pandas.concat([
+        utils.read(y_train_path),
+        utils.read(y_test_path),
+    ])
+
+    for dataframe in [full_x, full_y]:
         dataframe.set_index(moon_column_name, drop=True, inplace=True)
 
+    del x_test
+
     os.makedirs(model_directory_path, exist_ok=True)
 
     predictions: typing.List[pandas.DataFrame] = []
 
     for index, moon in enumerate(moons):
         train = (force_first_train and index == 0) or (train_frequency != 0 and moon % train_frequency == 0)
 
         logging.warn('---')
         logging.warn('loop: moon=%s train=%s (%s/%s)', moon, train, index + 1, len(moons))
 
         if train:
-            logging.warn('handler: train(%s, %s, %s)', x_train_path, y_train_path, model_directory_path)
-            x_train_loop = x_train[x_train.index < moon - embargo].reset_index()
-            y_train_loop = y_train[y_train.index < moon - embargo].reset_index()
-            train_handler(x_train_loop, y_train_loop, model_directory_path)
-
-        logging.warn('handler: infer(%s, %s)', x_test_path, model_directory_path)
-        x_test_loop = x_test[x_test.index == moon].reset_index()
-        prediction = infer_handler(x_test_loop, model_directory_path)
+            logging.warn('call: train')
+            x_train = full_x[full_x.index < moon - embargo].reset_index()
+            y_train = full_y[full_y.index < moon - embargo].reset_index()
+            train_handler(x_train, y_train, model_directory_path)
+
+        logging.warn('call: infer')
+        x_test = full_x[full_x.index == moon].reset_index()
+        prediction = infer_handler(x_test, model_directory_path)
         prediction = ensure.return_infer(prediction)
 
         predictions.append(prediction)
 
     prediction = pandas.concat(predictions)
     prediction_path = os.path.join(constants.DOT_DATA_DIRECTORY, "prediction.csv")
     utils.write(prediction, prediction_path)
```

### Comparing `crunch-cli-1.5.2/crunch/utils.py` & `crunch-cli-1.6.0/crunch/utils.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.5.2/crunch_cli.egg-info/SOURCES.txt` & `crunch-cli-1.6.0/crunch_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.5.2/setup.py` & `crunch-cli-1.6.0/setup.py`

 * *Files identical despite different names*

