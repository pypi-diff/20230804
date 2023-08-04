# Comparing `tmp/tracebloc_package-dev-0.5.4.tar.gz` & `tmp/tracebloc_package-dev-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tracebloc_package-dev-0.5.4.tar", last modified: Fri Jul 21 14:53:11 2023, max compression
+gzip compressed data, was "tracebloc_package-dev-0.5.5.tar", last modified: Fri Aug  4 11:43:54 2023, max compression
```

## Comparing `tracebloc_package-dev-0.5.4.tar` & `tracebloc_package-dev-0.5.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 hasan      (501) staff       (20)        0 2023-07-21 14:53:11.395840 tracebloc_package-dev-0.5.4/
--rw-r--r--   0 hasan      (501) staff       (20)     1048 2022-05-16 08:30:43.000000 tracebloc_package-dev-0.5.4/LICENSE.txt
--rw-r--r--   0 hasan      (501) staff       (20)      577 2023-07-21 14:53:11.395934 tracebloc_package-dev-0.5.4/PKG-INFO
--rw-r--r--   0 hasan      (501) staff       (20)      188 2022-05-16 08:30:43.000000 tracebloc_package-dev-0.5.4/README.md
--rw-r--r--   0 hasan      (501) staff       (20)       78 2023-07-21 14:53:11.396320 tracebloc_package-dev-0.5.4/setup.cfg
--rw-r--r--   0 hasan      (501) staff       (20)      949 2023-07-21 14:48:57.000000 tracebloc_package-dev-0.5.4/setup.py
-drwxr-xr-x   0 hasan      (501) staff       (20)        0 2023-07-21 14:53:11.394341 tracebloc_package-dev-0.5.4/tracebloc_package/
--rw-r--r--   0 hasan      (501) staff       (20)       67 2023-06-07 12:41:07.000000 tracebloc_package-dev-0.5.4/tracebloc_package/__init__.py
--rw-r--r--   0 hasan      (501) staff       (20)     5669 2023-06-07 12:41:07.000000 tracebloc_package-dev-0.5.4/tracebloc_package/check_parameters.py
--rw-r--r--   0 hasan      (501) staff       (20)    26592 2023-07-21 14:48:29.000000 tracebloc_package-dev-0.5.4/tracebloc_package/functional_test.py
--rw-r--r--   0 hasan      (501) staff       (20)    58421 2023-07-19 08:56:18.000000 tracebloc_package-dev-0.5.4/tracebloc_package/linkModelDataSet.py
--rw-r--r--   0 hasan      (501) staff       (20)     7100 2023-06-26 09:31:51.000000 tracebloc_package-dev-0.5.4/tracebloc_package/messages.py
--rw-r--r--   0 hasan      (501) staff       (20)    11021 2023-07-21 14:48:30.000000 tracebloc_package-dev-0.5.4/tracebloc_package/upload.py
--rw-r--r--   0 hasan      (501) staff       (20)    10427 2023-06-26 09:31:51.000000 tracebloc_package-dev-0.5.4/tracebloc_package/user.py
--rw-r--r--   0 hasan      (501) staff       (20)     6857 2023-07-21 14:48:30.000000 tracebloc_package-dev-0.5.4/tracebloc_package/utils.py
--rw-r--r--   0 hasan      (501) staff       (20)     3200 2023-06-09 12:24:04.000000 tracebloc_package-dev-0.5.4/tracebloc_package/weights.py
-drwxr-xr-x   0 hasan      (501) staff       (20)        0 2023-07-21 14:53:11.395642 tracebloc_package-dev-0.5.4/tracebloc_package_dev.egg-info/
--rw-r--r--   0 hasan      (501) staff       (20)      577 2023-07-21 14:53:11.000000 tracebloc_package-dev-0.5.4/tracebloc_package_dev.egg-info/PKG-INFO
--rw-r--r--   0 hasan      (501) staff       (20)      591 2023-07-21 14:53:11.000000 tracebloc_package-dev-0.5.4/tracebloc_package_dev.egg-info/SOURCES.txt
--rw-r--r--   0 hasan      (501) staff       (20)        1 2023-07-21 14:53:11.000000 tracebloc_package-dev-0.5.4/tracebloc_package_dev.egg-info/dependency_links.txt
--rw-r--r--   0 hasan      (501) staff       (20)        1 2023-07-21 14:53:11.000000 tracebloc_package-dev-0.5.4/tracebloc_package_dev.egg-info/not-zip-safe
--rw-r--r--   0 hasan      (501) staff       (20)      119 2023-07-21 14:53:11.000000 tracebloc_package-dev-0.5.4/tracebloc_package_dev.egg-info/requires.txt
--rw-r--r--   0 hasan      (501) staff       (20)       18 2023-07-21 14:53:11.000000 tracebloc_package-dev-0.5.4/tracebloc_package_dev.egg-info/top_level.txt
+drwxr-xr-x   0 divyasingh   (501) staff       (20)        0 2023-08-04 11:43:54.937171 tracebloc_package-dev-0.5.5/
+-rw-r--r--   0 divyasingh   (501) staff       (20)     1048 2022-05-03 09:10:47.000000 tracebloc_package-dev-0.5.5/LICENSE.txt
+-rw-r--r--   0 divyasingh   (501) staff       (20)      558 2023-08-04 11:43:54.937263 tracebloc_package-dev-0.5.5/PKG-INFO
+-rw-r--r--   0 divyasingh   (501) staff       (20)      188 2022-05-03 09:10:47.000000 tracebloc_package-dev-0.5.5/README.md
+-rw-r--r--   0 divyasingh   (501) staff       (20)       78 2023-08-04 11:43:54.937573 tracebloc_package-dev-0.5.5/setup.cfg
+-rw-r--r--   0 divyasingh   (501) staff       (20)      949 2023-08-04 11:43:45.000000 tracebloc_package-dev-0.5.5/setup.py
+drwxr-xr-x   0 divyasingh   (501) staff       (20)        0 2023-08-04 11:43:54.935561 tracebloc_package-dev-0.5.5/tracebloc_package/
+-rw-r--r--   0 divyasingh   (501) staff       (20)       67 2023-06-05 16:08:49.000000 tracebloc_package-dev-0.5.5/tracebloc_package/__init__.py
+-rw-r--r--   0 divyasingh   (501) staff       (20)     5669 2023-06-05 16:08:49.000000 tracebloc_package-dev-0.5.5/tracebloc_package/check_parameters.py
+-rw-r--r--   0 divyasingh   (501) staff       (20)    29559 2023-08-04 06:55:34.000000 tracebloc_package-dev-0.5.5/tracebloc_package/functional_test.py
+-rw-r--r--   0 divyasingh   (501) staff       (20)    58421 2023-08-02 07:41:20.000000 tracebloc_package-dev-0.5.5/tracebloc_package/linkModelDataSet.py
+-rw-r--r--   0 divyasingh   (501) staff       (20)     7100 2022-07-01 07:02:58.000000 tracebloc_package-dev-0.5.5/tracebloc_package/messages.py
+-rw-r--r--   0 divyasingh   (501) staff       (20)    11477 2023-08-04 06:55:34.000000 tracebloc_package-dev-0.5.5/tracebloc_package/upload.py
+-rw-r--r--   0 divyasingh   (501) staff       (20)    10427 2023-06-09 08:04:05.000000 tracebloc_package-dev-0.5.5/tracebloc_package/user.py
+-rw-r--r--   0 divyasingh   (501) staff       (20)     6860 2023-08-03 15:22:24.000000 tracebloc_package-dev-0.5.5/tracebloc_package/utils.py
+-rw-r--r--   0 divyasingh   (501) staff       (20)     3200 2023-06-09 08:04:05.000000 tracebloc_package-dev-0.5.5/tracebloc_package/weights.py
+drwxr-xr-x   0 divyasingh   (501) staff       (20)        0 2023-08-04 11:43:54.936993 tracebloc_package-dev-0.5.5/tracebloc_package_dev.egg-info/
+-rw-r--r--   0 divyasingh   (501) staff       (20)      558 2023-08-04 11:43:54.000000 tracebloc_package-dev-0.5.5/tracebloc_package_dev.egg-info/PKG-INFO
+-rw-r--r--   0 divyasingh   (501) staff       (20)      591 2023-08-04 11:43:54.000000 tracebloc_package-dev-0.5.5/tracebloc_package_dev.egg-info/SOURCES.txt
+-rw-r--r--   0 divyasingh   (501) staff       (20)        1 2023-08-04 11:43:54.000000 tracebloc_package-dev-0.5.5/tracebloc_package_dev.egg-info/dependency_links.txt
+-rw-r--r--   0 divyasingh   (501) staff       (20)        1 2023-08-04 11:43:54.000000 tracebloc_package-dev-0.5.5/tracebloc_package_dev.egg-info/not-zip-safe
+-rw-r--r--   0 divyasingh   (501) staff       (20)      119 2023-08-04 11:43:54.000000 tracebloc_package-dev-0.5.5/tracebloc_package_dev.egg-info/requires.txt
+-rw-r--r--   0 divyasingh   (501) staff       (20)       18 2023-08-04 11:43:54.000000 tracebloc_package-dev-0.5.5/tracebloc_package_dev.egg-info/top_level.txt
```

### Comparing `tracebloc_package-dev-0.5.4/LICENSE.txt` & `tracebloc_package-dev-0.5.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tracebloc_package-dev-0.5.4/PKG-INFO` & `tracebloc_package-dev-0.5.5/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 Metadata-Version: 2.1
 Name: tracebloc_package-dev
-Version: 0.5.4
+Version: 0.5.5
 Summary: Package required to run Tracebloc jupyter notebook to create experiment
 Home-page: https://gitlab.com/tracebloc/tracebloc-py-package/-/tree/dev
 Author: Tracebloc
 Author-email: info@tracebloc.io
 License: MIT
-Platform: UNKNOWN
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Tracebloc package
 This packeg is pre-requiste to run tracebloc jupyter notebook.
 
 
 This package helps to create and start the experiment for training ML models in 
 tracebloc environment.
-
```

### Comparing `tracebloc_package-dev-0.5.4/setup.py` & `tracebloc_package-dev-0.5.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name="tracebloc_package-dev",
-    version="0.5.4",
+    version="0.5.5",
     description="Package required to run Tracebloc jupyter notebook to create experiment",
     url="https://gitlab.com/tracebloc/tracebloc-py-package/-/tree/dev",
     license="MIT",
     python_requires=">=3",
     packages=["tracebloc_package"],
     author="Tracebloc",
     author_email="info@tracebloc.io",
```

### Comparing `tracebloc_package-dev-0.5.4/tracebloc_package/check_parameters.py` & `tracebloc_package-dev-0.5.5/tracebloc_package/check_parameters.py`

 * *Files identical despite different names*

### Comparing `tracebloc_package-dev-0.5.4/tracebloc_package/functional_test.py` & `tracebloc_package-dev-0.5.5/tracebloc_package/functional_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -407,38 +407,45 @@
         """
         for layer in self.model.layers:
             if not isinstance(layer, tf.keras.layers.Layer):
                 self.message = "\nLayers in Model are not supported by Tensorflow"  # pragma: no cover
                 raise Exception("invalid layer")  # pragma: no cover
         self.progress_bar_update()
 
-    def small_training_loop(self, custom_loss=None):
+    def small_training_loop(self, weight_filename, custom_loss=None):
         try:
             # mock dataset for small training
             classes = 1  # get output classes from model
             training_dataset = mock_dataset(classes)
             if custom_loss:
                 # check for custom loss
                 loss = custom_loss["value"]
-
             else:
-                loss = tf.keras.losses.CategoricalCrossentropy()
+                loss = tf.keras.losses.BinaryCrossentropy()
             self.model.compile(
                 optimizer=tf.keras.optimizers.Adam(),
                 loss=loss,
             )
             self.model.fit(training_dataset, epochs=1, verbose=0)
-            # dump weights from trained model will be used in averaging check
-            get_model_parameters(
-                model=self.model,
-                weight_file_path=self.tmp_path,
-                weights_file_name=TRAINED_WEIGHTS_FILENAME,
-                framework=TENSORFLOW_FRAMEWORK,
-            )
-            self.progress_bar_update()
+            if weight_filename == PRETRAINED_WEIGHTS_FILENAME:
+                get_model_parameters(
+                    model=self.model,
+                    weight_file_path=self.tmp_path,
+                    weights_file_name=PRETRAINED_WEIGHTS_FILENAME,
+                    framework=TENSORFLOW_FRAMEWORK,
+                )
+            else:
+                # dump weights from trained model will be used in averaging check
+                get_model_parameters(
+                    model=self.model,
+                    weight_file_path=self.tmp_path,
+                    weights_file_name=TRAINED_WEIGHTS_FILENAME,
+                    framework=TENSORFLOW_FRAMEWORK,
+                )
+                self.progress_bar_update()
         except Exception as e:  # pragma: no cover
             self.message = (
                 "\nModel not support training on image classification dataset."
             )
             raise
 
     def check_original_model_channels(self):
@@ -449,20 +456,36 @@
         if model_channel.input_shape[3] != 3:
             self.message = (
                 "\nPlease provide model input shape with 3 channels"  # pragma: no cover
             )
             raise Exception("invalid input shape")  # pragma: no cover
         self.progress_bar_update()
 
+    def resize_weight_arrays(self, weights_list_tuple):
+        # Find the maximum shape among all weight arrays in the tuple
+        max_shape = np.array(max(w.shape for w in weights_list_tuple))
+
+        # Broadcast each weight array to the maximum shape
+        resized_weights_list = []
+        for w in weights_list_tuple:
+            if w.shape == ():
+                # Convert 0-dimensional array to 1-dimensional array
+                broadcasted_w = np.broadcast_to(w, (1,))
+            else:
+                broadcasted_w = np.broadcast_to(w, max_shape)
+            resized_weights_list.append(broadcasted_w)
+
+        return resized_weights_list
+
     def average_weights(self):
         weights = []
         new_weights = []
         no_images_array = [20, 20]
         weights_file_path_1 = os.path.join(
-            self.tmp_path, f"{UNTRAINED_WEIGHTS_FILENAME}.pkl"
+            self.tmp_path, f"{PRETRAINED_WEIGHTS_FILENAME}.pkl"
         )
         weights_file_path_2 = os.path.join(
             self.tmp_path, f"{TRAINED_WEIGHTS_FILENAME}.pkl"
         )
         self.average_weights_file_path = os.path.join(
             self.tmp_path, f"{AVERAGED_WEIGHTS_PATH}.pkl"
         )
@@ -475,15 +498,15 @@
         except Exception as e:
             raise
         try:
             new_weights = [
                 np.array(
                     [
                         np.average(np.array(w), weights=no_images_array, axis=0)
-                        for w in zip(*weights_list_tuple)
+                        for w in zip(*self.resize_weight_arrays(weights_list_tuple))
                     ]
                 )
                 for weights_list_tuple in zip(*weights)
             ]
             del weights
             del no_images_array
         except Exception as e:
@@ -505,15 +528,19 @@
             raise
 
     def is_model_eligible(self):
         try:
             self.is_model_supported()
             self.check_original_model_channels()
             self.layer_instance_check()
-            self.small_training_loop()
+            if not os.path.exists(
+                os.path.join(self.tmp_path, f"{PRETRAINED_WEIGHTS_FILENAME}.pkl")
+            ):
+                self.small_training_loop(PRETRAINED_WEIGHTS_FILENAME)
+            self.small_training_loop(TRAINED_WEIGHTS_FILENAME)
             self.average_weights()
             self.load_averaged_weights()
             self.message = "all check passed"
         except Exception as e:  # pragma: no cover
             self.message = f"\nModel checks failed with error as {e}"
             return False, self.message
         return True, self.message
@@ -556,20 +583,20 @@
         """
         model = self.model
         if not hasattr(model, "forward"):
             self.message = "\nModel file not provided as per docs: forward function not found in  Model"
             raise Exception("forward func missing")
         self.progress_bar.update(1)
 
-    def small_training_loop(self, custom_loss=None):
+    def small_training_loop(self, weight_filename, custom_loss=None):
         try:
             # Define the number of fake images and other properties
             num_images = 100
             num_channels = 3
-            num_classes = 1
+            num_classes = 2
             # Create fake image data
             train_dataset = datasets.FakeData(
                 size=num_images,
                 image_size=(num_channels, self.image_size, self.image_size),
                 num_classes=num_classes,
                 transform=transforms.ToTensor(),
             )
@@ -595,31 +622,55 @@
                     loss = criterion(outputs, labels)
                     loss.backward()
                     optimizer.step()
 
                     # print statistics
                     running_loss += loss.item()
             # dump weights from trained model will be used in averaging check
-            get_model_parameters(
-                model=self.model,
-                weight_file_path=self.tmp_path,
-                weights_file_name=TRAINED_WEIGHTS_FILENAME,
-                framework=PYTORCH_FRAMEWORK,
-            )
-            self.progress_bar.update(1)
+            if weight_filename == PRETRAINED_WEIGHTS_FILENAME:
+                get_model_parameters(
+                    model=self.model,
+                    weight_file_path=self.tmp_path,
+                    weights_file_name=PRETRAINED_WEIGHTS_FILENAME,
+                    framework=PYTORCH_FRAMEWORK,
+                )
+            else:
+                get_model_parameters(
+                    model=self.model,
+                    weight_file_path=self.tmp_path,
+                    weights_file_name=TRAINED_WEIGHTS_FILENAME,
+                    framework=PYTORCH_FRAMEWORK,
+                )
+                self.progress_bar.update(1)
         except Exception as e:  # pragma: no cover
             self.message = f"\nModel not support training on image classification dataset as there is error {e} "
             raise
 
+    def resize_weight_arrays(self, weights_list_tuple):
+        # Find the maximum shape among all weight arrays in the tuple
+        max_shape = np.array(max(w.shape for w in weights_list_tuple))
+
+        # Broadcast each weight array to the maximum shape
+        resized_weights_list = []
+        for w in weights_list_tuple:
+            if w.shape == ():
+                # Convert 0-dimensional array to 1-dimensional array
+                broadcasted_w = np.broadcast_to(w, (1,))
+            else:
+                broadcasted_w = np.broadcast_to(w, max_shape)
+            resized_weights_list.append(broadcasted_w)
+
+        return resized_weights_list
+
     def average_weights(self):
         weights = []
         new_weights = []
-        no_images_array = [20, 20]
+        no_images_array = [100, 100]
         weights_file_path_1 = os.path.join(
-            self.tmp_path, f"{UNTRAINED_WEIGHTS_FILENAME}.pkl"
+            self.tmp_path, f"{PRETRAINED_WEIGHTS_FILENAME}.pkl"
         )
         weights_file_path_2 = os.path.join(
             self.tmp_path, f"{TRAINED_WEIGHTS_FILENAME}.pkl"
         )
         self.average_weights_file_path = os.path.join(
             self.tmp_path, f"{AVERAGED_WEIGHTS_PATH}.pkl"
         )
@@ -632,49 +683,62 @@
         except Exception as e:
             raise
         try:
             new_weights = [
                 np.array(
                     [
                         np.average(np.array(w), weights=no_images_array, axis=0)
-                        for w in zip(*weights_list_tuple)
+                        for w in zip(*self.resize_weight_arrays(weights_list_tuple))
                     ]
                 )
                 for weights_list_tuple in zip(*weights)
             ]
             del weights
             del no_images_array
         except Exception as e:
             raise
         try:
             with open(self.average_weights_file_path, "wb") as f:
                 pickle.dump(new_weights, f)
             del new_weights
         except Exception as e:
-            raise
+            raise e
 
     def load_averaged_weights(self):
         try:
             with open(self.average_weights_file_path, "rb") as f:
                 parameters = pickle.load(f)
             params_dict = zip(self.model.state_dict().keys(), parameters)
             state_dict = OrderedDict({k: torch.tensor(v) for k, v in params_dict})
             self.model.load_state_dict(state_dict, strict=True)
+            self.progress_bar.update(1)
             del params_dict
             del state_dict
             del parameters
         except Exception as e:
             raise
 
     def model_func_checks(self):
         # check if model is eligible
         try:
             self.is_model_supported()
-            self.progress_bar.update(2)
-            self.small_training_loop()
+            if os.path.exists(
+                os.path.join(self.tmp_path, f"{PRETRAINED_WEIGHTS_FILENAME}.pth")
+            ):
+                get_model_parameters(
+                    model=self.model,
+                    weight_file_path=self.tmp_path,
+                    weights_file_name=PRETRAINED_WEIGHTS_FILENAME,
+                    framework=PYTORCH_FRAMEWORK,
+                )
+                self.progress_bar.update(1)
+            else:
+                self.small_training_loop(PRETRAINED_WEIGHTS_FILENAME)
+                self.progress_bar.update(1)
+            self.small_training_loop(TRAINED_WEIGHTS_FILENAME)
             self.average_weights()
             self.load_averaged_weights()
             self.message = "all check passed"
             eligible = True
         except Exception as e:  # pragma: no cover
             self.message = f"\nModel checks failed with error as {e}"
             eligible = False
```

### Comparing `tracebloc_package-dev-0.5.4/tracebloc_package/linkModelDataSet.py` & `tracebloc_package-dev-0.5.5/tracebloc_package/linkModelDataSet.py`

 * *Files identical despite different names*

### Comparing `tracebloc_package-dev-0.5.4/tracebloc_package/messages.py` & `tracebloc_package-dev-0.5.5/tracebloc_package/messages.py`

 * *Files identical despite different names*

### Comparing `tracebloc_package-dev-0.5.4/tracebloc_package/upload.py` & `tracebloc_package-dev-0.5.5/tracebloc_package/upload.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import pickletools
+import shutil
 import sys
 import torch
 import requests, json, pickle
 from importlib.machinery import SourceFileLoader
 from termcolor import colored
 import os
 import rich
@@ -120,20 +121,31 @@
                 self.progress_bar.close()
                 return None
             loaded_model = model_checks_generic.model
             self.__framework = model_checks_generic.framework
             self.__image_size = int(model_checks_generic.image_size)
             self.__batch_size = int(model_checks_generic.batch_size)
             # dump weights from non-trained model will be used in averaging check
-            get_model_parameters(
-                model=loaded_model,
-                weight_file_path=model_checks_generic.tmp_file_path,
-                weights_file_name=UNTRAINED_WEIGHTS_FILENAME,
-                framework=self.__framework,
-            )
+            if self.weights:
+                if self.__framework == PYTORCH_FRAMEWORK:
+                    shutil.copy2(
+                        self.__weights_path,
+                        os.path.join(
+                            model_checks_generic.tmp_file_path,
+                            PRETRAINED_WEIGHTS_FILENAME + ".pth",
+                        ),
+                    )
+                else:
+                    shutil.copy2(
+                        self.__weights_path,
+                        os.path.join(
+                            model_checks_generic.tmp_file_path,
+                            PRETRAINED_WEIGHTS_FILENAME + ".pkl",
+                        ),
+                    )
             if self.__framework == PYTORCH_FRAMEWORK:
                 self.model_check_class = TorchChecks(
                     model=loaded_model,
                     model_name=model_name,
                     message=message,
                     progress_bar=self.progress_bar,
                     image_size=self.__image_size,
```

### Comparing `tracebloc_package-dev-0.5.4/tracebloc_package/user.py` & `tracebloc_package-dev-0.5.5/tracebloc_package/user.py`

 * *Files identical despite different names*

### Comparing `tracebloc_package-dev-0.5.4/tracebloc_package/utils.py` & `tracebloc_package-dev-0.5.5/tracebloc_package/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 CONSTANT = "constant"
 STANDARD = "standard"
 ADAPTIVE = "adaptive"
 CUSTOM = "custom"
 TYPE = "type"
 FUNCTION = "function"
 VALUE = "value"
-UNTRAINED_WEIGHTS_FILENAME = "untrained_weights"
+PRETRAINED_WEIGHTS_FILENAME = "pretrained_weights"
 TRAINED_WEIGHTS_FILENAME = "trained_weights"
 AVERAGED_WEIGHTS_PATH = "averaged"
 
 
 def check_MyModel(filename, path):
     try:
         # check if file contains the MyModel function
@@ -143,15 +143,15 @@
     count = 0
     for key in images_count.keys():
         count += images_count[key]
     return count
 
 
 def mock_dataset(classes):
-    num_examples = 3
+    num_examples = 20
 
     def as_dataset(self, *args, **kwargs):
         return tf.data.Dataset.from_generator(  # pragma: no cover
             lambda: (
                 {
                     "image": np.ones(shape=(256, 256, 3), dtype=np.uint8),
                     "label": classes,
```

### Comparing `tracebloc_package-dev-0.5.4/tracebloc_package/weights.py` & `tracebloc_package-dev-0.5.5/tracebloc_package/weights.py`

 * *Files identical despite different names*

### Comparing `tracebloc_package-dev-0.5.4/tracebloc_package_dev.egg-info/PKG-INFO` & `tracebloc_package-dev-0.5.5/tracebloc_package_dev.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 Metadata-Version: 2.1
 Name: tracebloc-package-dev
-Version: 0.5.4
+Version: 0.5.5
 Summary: Package required to run Tracebloc jupyter notebook to create experiment
 Home-page: https://gitlab.com/tracebloc/tracebloc-py-package/-/tree/dev
 Author: Tracebloc
 Author-email: info@tracebloc.io
 License: MIT
-Platform: UNKNOWN
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Tracebloc package
 This packeg is pre-requiste to run tracebloc jupyter notebook.
 
 
 This package helps to create and start the experiment for training ML models in 
 tracebloc environment.
-
```

### Comparing `tracebloc_package-dev-0.5.4/tracebloc_package_dev.egg-info/SOURCES.txt` & `tracebloc_package-dev-0.5.5/tracebloc_package_dev.egg-info/SOURCES.txt`

 * *Files identical despite different names*

