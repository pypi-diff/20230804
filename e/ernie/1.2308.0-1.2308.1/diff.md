# Comparing `tmp/ernie-1.2308.0-py3-none-any.whl.zip` & `tmp/ernie-1.2308.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,19 @@
-Zip file size: 18199 bytes, number of entries: 17
--rw-rw-r--  2.0 unx     1061 b- defN 23-Aug-01 18:07 ernie/__init__.py
+Zip file size: 18196 bytes, number of entries: 17
+-rw-rw-r--  2.0 unx     1061 b- defN 23-Aug-04 07:32 ernie/__init__.py
 -rw-rw-r--  2.0 unx     1934 b- defN 23-Jul-31 18:23 ernie/aggregation_strategies.py
--rw-rw-r--  2.0 unx    13388 b- defN 23-Aug-02 05:34 ernie/ernie.py
+-rw-rw-r--  2.0 unx    13420 b- defN 23-Aug-04 07:09 ernie/ernie.py
 -rw-rw-r--  2.0 unx     3026 b- defN 23-Aug-02 05:33 ernie/helper.py
 -rw-rw-r--  2.0 unx     1758 b- defN 23-Jul-31 18:23 ernie/models.py
 -rw-rw-r--  2.0 unx     4314 b- defN 23-Jul-31 18:23 ernie/split_strategies.py
 -rw-rw-r--  2.0 unx       87 b- defN 23-Jul-31 18:24 test/__init__.py
 -rw-rw-r--  2.0 unx     1414 b- defN 23-Jul-31 18:24 test/dump_load.py
 -rw-rw-r--  2.0 unx      775 b- defN 23-Jul-31 18:24 test/load_csv.py
 -rw-rw-r--  2.0 unx      973 b- defN 23-Jul-31 18:24 test/load_model.py
 -rw-rw-r--  2.0 unx      714 b- defN 23-Jul-31 18:25 test/predict.py
 -rw-rw-r--  2.0 unx    18131 b- defN 23-Jul-31 18:26 test/split_aggregate.py
--rw-rw-r--  2.0 unx    11358 b- defN 23-Aug-02 11:14 ernie-1.2308.0.dist-info/LICENSE
--rw-rw-r--  2.0 unx     1016 b- defN 23-Aug-02 11:14 ernie-1.2308.0.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Aug-02 11:14 ernie-1.2308.0.dist-info/WHEEL
--rw-rw-r--  2.0 unx       11 b- defN 23-Aug-02 11:14 ernie-1.2308.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1295 b- defN 23-Aug-02 11:14 ernie-1.2308.0.dist-info/RECORD
-17 files, 61347 bytes uncompressed, 16113 bytes compressed:  73.7%
+-rw-rw-r--  2.0 unx    11358 b- defN 23-Aug-04 07:57 ernie-1.2308.1.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     1016 b- defN 23-Aug-04 07:57 ernie-1.2308.1.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Aug-04 07:57 ernie-1.2308.1.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       11 b- defN 23-Aug-04 07:57 ernie-1.2308.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1295 b- defN 23-Aug-04 07:57 ernie-1.2308.1.dist-info/RECORD
+17 files, 61379 bytes uncompressed, 16110 bytes compressed:  73.8%
```

## zipnote {}

```diff
@@ -30,23 +30,23 @@
 
 Filename: test/predict.py
 Comment: 
 
 Filename: test/split_aggregate.py
 Comment: 
 
-Filename: ernie-1.2308.0.dist-info/LICENSE
+Filename: ernie-1.2308.1.dist-info/LICENSE
 Comment: 
 
-Filename: ernie-1.2308.0.dist-info/METADATA
+Filename: ernie-1.2308.1.dist-info/METADATA
 Comment: 
 
-Filename: ernie-1.2308.0.dist-info/WHEEL
+Filename: ernie-1.2308.1.dist-info/WHEEL
 Comment: 
 
-Filename: ernie-1.2308.0.dist-info/top_level.txt
+Filename: ernie-1.2308.1.dist-info/top_level.txt
 Comment: 
 
-Filename: ernie-1.2308.0.dist-info/RECORD
+Filename: ernie-1.2308.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ernie/__init__.py

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 from .ernie import *  # noqa: F401, F403
 from tensorflow.python.client import device_lib
 import logging
 
-__version__ = '1.2308.0'
+__version__ = '1.2308.1'
 
 logging.getLogger().setLevel(logging.WARNING)
 logging.getLogger("transformers.tokenization_utils").setLevel(logging.ERROR)
 logging.basicConfig(
     format='%(asctime)-15s [%(levelname)s] %(message)s',
     datefmt='%Y-%m-%d %H:%M:%S'
 )
```

## ernie/ernie.py

```diff
@@ -297,15 +297,18 @@
                     softmax(logit_prediction)
                     for logit_prediction in logit_predictions[0]
                 ]
             )
 
     def _list_to_padded_array(self, items):
         array = np.array(items)
-        padded_array = np.zeros(self._tokenizer.model_max_length, dtype=np.int)
+        padded_array = np.zeros(
+            self._tokenizer.model_max_length,
+            dtype=int,
+        )
         padded_array[:array.shape[0]] = array
         return padded_array
 
     def _get_temporary_path(self, name=''):
         return f'{AUTOSAVE_PATH}{name}/{int(round(time.time() * 1000))}'
 
     def _reload_model(self):
```

## Comparing `ernie-1.2308.0.dist-info/LICENSE` & `ernie-1.2308.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `ernie-1.2308.0.dist-info/METADATA` & `ernie-1.2308.1.dist-info/METADATA`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ernie
-Version: 1.2308.0
+Version: 1.2308.1
 Summary: An Accessible Python Library for State-of-the-art Natural Language Processing. Built with HuggingFace's Transformers.
 Home-page: https://github.com/labteral/ernie
 Author: Rodrigo Martínez Castaño
 Author-email: dev@brunneis.com
 License: Apache License (Version 2.0)
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

## Comparing `ernie-1.2308.0.dist-info/RECORD` & `ernie-1.2308.1.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-ernie/__init__.py,sha256=ZWSMckk9bZ7qWINJLgvnZKiPMw3NdLnKR71JRxkqyv0,1061
+ernie/__init__.py,sha256=1b3F8tq3ORvwA9af9Fw4RFbVSC6iF2XmzBjZ-vdHTXM,1061
 ernie/aggregation_strategies.py,sha256=4UfPoHUdzhVWmZxQhUu9Ma6pHbvKyB9-VP7J13KzTOI,1934
-ernie/ernie.py,sha256=HO4JPzV3OTyAZnvCYSXmn45c7R6UC_E7IKRBbzl54hE,13388
+ernie/ernie.py,sha256=-sc2-tA-Nx1nQns8KewTsm3xRQw5RDRd_50M6zLl1Y4,13420
 ernie/helper.py,sha256=8-d0rF8SepFOxhE9oJgr9Vl5AHEop8af3KjVi6W-LNI,3026
 ernie/models.py,sha256=17CrjhCrNUP3_OKEBRlRimhs38dIfUmAoZOiIqRFJ9k,1758
 ernie/split_strategies.py,sha256=MJMsZ9Xis4Ffzx3MESiJpem2X_6Tg0eFGqxOIAeUbHs,4314
 test/__init__.py,sha256=Vy72ITAa99WGby_RFX9sxvC-QUj3J3FrgDTOAovqAOM,87
 test/dump_load.py,sha256=tdd_OLWidDZtDEqGeWABPqP6Wi9D0VSUw7olebX2Ytg,1414
 test/load_csv.py,sha256=Z7Ka3PH44axCV4Ll44bSr7hLKr5n-h5mx-N_yYDOucs,775
 test/load_model.py,sha256=oN9mKif0GrvTdjmeOS4ReJJCCw12DfaWRqJR4ZpCoag,973
 test/predict.py,sha256=Me2bBayH-nHGfxEGcUo2jrlTNq5-IOS-OxONnQqOfrE,714
 test/split_aggregate.py,sha256=6l_318O8SO1Jt2nMvxQTskznd6aS1xGWX1cqr4Yj_84,18131
-ernie-1.2308.0.dist-info/LICENSE,sha256=z8d0m5b2O9McPEK1xHG_dWgUBT6EfBDz6wA0F7xSPTA,11358
-ernie-1.2308.0.dist-info/METADATA,sha256=dRrTpILOkaprEY_CxOcairNhfuoxb7ueSKY8oQ9uLB4,1016
-ernie-1.2308.0.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-ernie-1.2308.0.dist-info/top_level.txt,sha256=IHK6af4HA-M8LcMpdIUJTH0DG1QRIai_1zA3kGcbwqI,11
-ernie-1.2308.0.dist-info/RECORD,,
+ernie-1.2308.1.dist-info/LICENSE,sha256=z8d0m5b2O9McPEK1xHG_dWgUBT6EfBDz6wA0F7xSPTA,11358
+ernie-1.2308.1.dist-info/METADATA,sha256=9p6Q7qPTlLCARcNkOQ-lDwxDXuXcPwMKxwHTgnUZCxg,1016
+ernie-1.2308.1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+ernie-1.2308.1.dist-info/top_level.txt,sha256=IHK6af4HA-M8LcMpdIUJTH0DG1QRIai_1zA3kGcbwqI,11
+ernie-1.2308.1.dist-info/RECORD,,
```

