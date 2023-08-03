# Comparing `tmp/e-models-1.5.2.1.tar.gz` & `tmp/e-models-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "e-models-1.5.2.1.tar", last modified: Thu Jul 27 16:35:03 2023, max compression
+gzip compressed data, was "e-models-1.5.3.tar", last modified: Thu Aug  3 22:16:04 2023, max compression
```

## Comparing `e-models-1.5.2.1.tar` & `e-models-1.5.3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-07-27 16:35:03.443218 e-models-1.5.2.1/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     1501 2023-03-30 21:13:00.000000 e-models-1.5.2.1/LICENSE
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     3504 2023-07-27 16:35:03.443218 e-models-1.5.2.1/PKG-INFO
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     2928 2023-07-25 17:58:30.000000 e-models-1.5.2.1/README.md
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-07-27 16:35:03.439218 e-models-1.5.2.1/e_models.egg-info/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     3504 2023-07-27 16:35:03.000000 e-models-1.5.2.1/e_models.egg-info/PKG-INFO
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      655 2023-07-27 16:35:03.000000 e-models-1.5.2.1/e_models.egg-info/SOURCES.txt
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        1 2023-07-27 16:35:03.000000 e-models-1.5.2.1/e_models.egg-info/dependency_links.txt
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       83 2023-07-27 16:35:03.000000 e-models-1.5.2.1/e_models.egg-info/requires.txt
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        8 2023-07-27 16:35:03.000000 e-models-1.5.2.1/e_models.egg-info/top_level.txt
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-07-27 16:35:03.439218 e-models-1.5.2.1/emodels/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       24 2023-07-27 16:34:30.000000 e-models-1.5.2.1/emodels/__init__.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      319 2023-07-26 22:24:33.000000 e-models-1.5.2.1/emodels/config.py
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-07-27 16:35:03.443218 e-models-1.5.2.1/emodels/datasets/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        0 2023-06-23 18:11:59.000000 e-models-1.5.2.1/emodels/datasets/__init__.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)    12135 2023-07-27 14:36:45.000000 e-models-1.5.2.1/emodels/datasets/models.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     1929 2023-07-05 14:16:56.000000 e-models-1.5.2.1/emodels/datasets/tokenizers.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     6935 2023-07-27 13:48:16.000000 e-models-1.5.2.1/emodels/datasets/utils.py
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-07-27 16:35:03.443218 e-models-1.5.2.1/emodels/html2text/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)    35479 2023-07-21 16:26:32.000000 e-models-1.5.2.1/emodels/html2text/__init__.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     3873 2023-05-04 18:51:26.000000 e-models-1.5.2.1/emodels/html2text/config.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      423 2023-05-04 18:51:26.000000 e-models-1.5.2.1/emodels/html2text/elements.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       71 2023-05-04 18:51:26.000000 e-models-1.5.2.1/emodels/html2text/typing.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     8034 2023-05-04 18:51:26.000000 e-models-1.5.2.1/emodels/html2text/utils.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        0 2023-05-04 18:51:26.000000 e-models-1.5.2.1/emodels/py.typed
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-07-27 16:35:03.443218 e-models-1.5.2.1/emodels/scrapyutils/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      137 2023-06-23 22:04:28.000000 e-models-1.5.2.1/emodels/scrapyutils/__init__.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     2575 2023-07-26 22:24:33.000000 e-models-1.5.2.1/emodels/scrapyutils/loader.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     6000 2023-07-21 19:40:03.000000 e-models-1.5.2.1/emodels/scrapyutils/response.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       31 2023-03-30 21:32:48.000000 e-models-1.5.2.1/pyproject.toml
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       38 2023-07-27 16:35:03.443218 e-models-1.5.2.1/setup.cfg
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     1056 2023-07-27 16:34:23.000000 e-models-1.5.2.1/setup.py
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-07-27 16:35:03.443218 e-models-1.5.2.1/tests/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     6346 2023-07-21 17:31:24.000000 e-models-1.5.2.1/tests/test_html2text.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     8234 2023-07-26 22:27:27.000000 e-models-1.5.2.1/tests/test_scrapyutils.py
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-08-03 22:16:04.049945 e-models-1.5.3/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     1501 2023-03-30 21:13:00.000000 e-models-1.5.3/LICENSE
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     3502 2023-08-03 22:16:04.049945 e-models-1.5.3/PKG-INFO
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     2928 2023-07-25 17:58:30.000000 e-models-1.5.3/README.md
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-08-03 22:16:04.045946 e-models-1.5.3/e_models.egg-info/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     3502 2023-08-03 22:16:03.000000 e-models-1.5.3/e_models.egg-info/PKG-INFO
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      655 2023-08-03 22:16:04.000000 e-models-1.5.3/e_models.egg-info/SOURCES.txt
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        1 2023-08-03 22:16:03.000000 e-models-1.5.3/e_models.egg-info/dependency_links.txt
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       97 2023-08-03 22:16:03.000000 e-models-1.5.3/e_models.egg-info/requires.txt
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        8 2023-08-03 22:16:03.000000 e-models-1.5.3/e_models.egg-info/top_level.txt
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-08-03 22:16:04.045946 e-models-1.5.3/emodels/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       22 2023-08-03 22:15:34.000000 e-models-1.5.3/emodels/__init__.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      319 2023-07-26 22:24:33.000000 e-models-1.5.3/emodels/config.py
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-08-03 22:16:04.045946 e-models-1.5.3/emodels/datasets/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        0 2023-06-23 18:11:59.000000 e-models-1.5.3/emodels/datasets/__init__.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)    12168 2023-07-27 20:27:24.000000 e-models-1.5.3/emodels/datasets/models.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     1929 2023-07-05 14:16:56.000000 e-models-1.5.3/emodels/datasets/tokenizers.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     8402 2023-08-03 22:13:54.000000 e-models-1.5.3/emodels/datasets/utils.py
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-08-03 22:16:04.049945 e-models-1.5.3/emodels/html2text/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)    35479 2023-07-21 16:26:32.000000 e-models-1.5.3/emodels/html2text/__init__.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     3873 2023-05-04 18:51:26.000000 e-models-1.5.3/emodels/html2text/config.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      423 2023-05-04 18:51:26.000000 e-models-1.5.3/emodels/html2text/elements.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       71 2023-05-04 18:51:26.000000 e-models-1.5.3/emodels/html2text/typing.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     8034 2023-05-04 18:51:26.000000 e-models-1.5.3/emodels/html2text/utils.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        0 2023-05-04 18:51:26.000000 e-models-1.5.3/emodels/py.typed
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-08-03 22:16:04.049945 e-models-1.5.3/emodels/scrapyutils/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      137 2023-06-23 22:04:28.000000 e-models-1.5.3/emodels/scrapyutils/__init__.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     2575 2023-07-26 22:24:33.000000 e-models-1.5.3/emodels/scrapyutils/loader.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     6000 2023-07-21 19:40:03.000000 e-models-1.5.3/emodels/scrapyutils/response.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       31 2023-03-30 21:32:48.000000 e-models-1.5.3/pyproject.toml
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       38 2023-08-03 22:16:04.049945 e-models-1.5.3/setup.cfg
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     1079 2023-08-03 22:15:45.000000 e-models-1.5.3/setup.py
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-08-03 22:16:04.049945 e-models-1.5.3/tests/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     6346 2023-07-21 17:31:24.000000 e-models-1.5.3/tests/test_html2text.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     8016 2023-08-03 22:14:56.000000 e-models-1.5.3/tests/test_scrapyutils.py
```

### Comparing `e-models-1.5.2.1/LICENSE` & `e-models-1.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `e-models-1.5.2.1/PKG-INFO` & `e-models-1.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: e-models
-Version: 1.5.2.1
+Version: 1.5.3
 Summary: Tools for helping build of extraction models with scrapy spiders.
 Home-page: https://github.com/kalessin/emodels
 Author: Martin Olveyra
 Author-email: molveyra@gmail.com
 License: BSD
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `e-models-1.5.2.1/README.md` & `e-models-1.5.3/README.md`

 * *Files identical despite different names*

### Comparing `e-models-1.5.2.1/e_models.egg-info/PKG-INFO` & `e-models-1.5.3/e_models.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: e-models
-Version: 1.5.2.1
+Version: 1.5.3
 Summary: Tools for helping build of extraction models with scrapy spiders.
 Home-page: https://github.com/kalessin/emodels
 Author: Martin Olveyra
 Author-email: molveyra@gmail.com
 License: BSD
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `e-models-1.5.2.1/e_models.egg-info/SOURCES.txt` & `e-models-1.5.3/e_models.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `e-models-1.5.2.1/emodels/datasets/models.py` & `e-models-1.5.3/emodels/datasets/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 """
 import logging
 from abc import abstractmethod
-from typing import Generator, List, TypedDict, Any, Protocol, Tuple
+from typing import Generator, List, Any, Protocol, Tuple
 
 import joblib
 from scrapy.http import HtmlResponse
 import pandas as pd
 from sklearn.metrics import (
     accuracy_score,
     recall_score,
@@ -15,14 +15,15 @@
     confusion_matrix,
 )
 from sklearn.feature_extraction.text import TfidfVectorizer
 from sklearn.svm import SVC
 from sentencepiece import SentencePieceProcessor
 from shub_workflow.deliver.futils import FSHelper
 from shub_workflow.utils import get_project_settings
+from typing_extensions import Self
 
 from emodels.datasets.utils import (
     build_response_from_sample_data,
     ResponseConverter,
     Filename,
     DatasetFilename,
 )
@@ -43,24 +44,46 @@
     pass
 
 
 class VectorizerFilename(Filename):
     pass
 
 
-class DatasetsDict(TypedDict):
+class DatasetsPandas:
     X_train: pd.DataFrame
     X_test: pd.Series
     Y_train: pd.DataFrame
     Y_test: pd.Series
 
+    @classmethod
+    def from_datasetfilename(cls, filename: DatasetFilename, features: Tuple[str, ...], target_label: str) -> Self:
+        df = pd.read_json(filename, lines=True, compression="gzip")
+        df = df[~df[target_label].isnull()]
+
+        df_train = df[df.dataset_bucket == "train"].drop("dataset_bucket", axis=1)
+        df_test = df[df.dataset_bucket == "test"].drop("dataset_bucket", axis=1)
+
+        df_X_train = df_train[list(features)]
+        df_Y_train = df_train[target_label]
+
+        df_X_test = df_test[list(features)]
+        df_Y_test = df_test[target_label]
+
+        obj = cls()
+        obj.X_train = df_X_train
+        obj.X_test = df_X_test
+        obj.Y_train = df_Y_train
+        obj.Y_test = df_Y_test
+
+        return obj
+
 
 class ModelWithDataset(Protocol):
-    FSHELPER: FSHelper = None
-    datasets: DatasetsDict | None = None
+    FSHELPER: FSHelper | None = None
+    datasets: DatasetsPandas | None = None
 
     dataset_repository: DatasetFilename
     features: Tuple[str, ...]
     target_label: str
     project: str
 
     def __init__(self):
@@ -75,51 +98,30 @@
     def _fshelper(cls) -> FSHelper:
         if cls.FSHELPER is None:
             settings = get_project_settings()
             cls.FSHELPER = cls.build_fshelper(settings)
         return cls.FSHELPER
 
     @classmethod
-    def get_dataset_from_filename(cls, filename: DatasetFilename) -> DatasetsDict:
-        df = pd.read_json(filename, lines=True, compression="gzip")
-        df = df[~df[cls.target_label].isnull()]
-
-        df_train = df[df.dataset_bucket == "train"].drop("dataset_bucket", axis=1)
-        df_test = df[df.dataset_bucket == "test"].drop("dataset_bucket", axis=1)
-
-        df_X_train = df_train[list(cls.features)]
-        df_Y_train = df_train[cls.target_label]
-
-        df_X_test = df_test[list(cls.features)]
-        df_Y_test = df_test[cls.target_label]
-
-        return {
-            "X_train": df_X_train,
-            "X_test": df_X_test,
-            "Y_train": df_Y_train,
-            "Y_test": df_Y_test,
-        }
-
-    @classmethod
-    def load_dataset(cls) -> DatasetsDict:
+    def load_dataset(cls) -> DatasetsPandas:
         dataset_local: DatasetFilename = DatasetFilename(cls.dataset_repository).local(cls.project)
 
         if cls._fshelper().exists(dataset_local):
             LOGGER.info(f"Found local copy of datasets {dataset_local}.")
         elif cls._fshelper().exists(cls.dataset_repository):
             LOGGER.info("Downloading datasets...")
             cls._fshelper().download_file(cls.dataset_repository, dataset_local)
         else:
             LOGGER.info("Generating datasets...")
             cls.download_labelled_samples(dataset_local)
             cls._fshelper().upload_file(dataset_local, cls.dataset_repository)
-        return cls.get_dataset_from_filename(dataset_local)
+        return DatasetsPandas.from_datasetfilename(dataset_local, cls.features, cls.target_label)
 
     @classmethod
-    def get_dataset(cls) -> DatasetsDict:
+    def get_dataset(cls) -> DatasetsPandas:
         if cls.datasets is None:
             cls.datasets = cls.load_dataset()
         return cls.datasets
 
     @classmethod
     def reset(cls):
         pass
@@ -210,16 +212,15 @@
         elif cls._fshelper().exists(cls.vectorizer_repository):
             LOGGER.info("Downloading vectorizer model...")
             cls._fshelper().download_file(cls.vectorizer_repository, vectorizer_local)
         else:
             LOGGER.info("Training vectorizer...")
             vectorizer = TfidfVectorizer(min_df=10, max_df=0.7, ngram_range=(1, 3))
             datasets = cls.load_dataset()
-            X_train = datasets["X_train"]
-            vectorizer.fit(cls.get_dataset_features(X_train))
+            vectorizer.fit(cls.get_dataset_features(datasets.X_train))
             joblib.dump(vectorizer, vectorizer_local)
             cls._fshelper().upload_file(vectorizer_local, cls.vectorizer_repository)
         return joblib.load(vectorizer_local)
 
     @classmethod
     def get_vectorizer(cls) -> TfidfVectorizer:
         if cls.vectorizer is None:
@@ -285,16 +286,16 @@
     @classmethod
     def predict(cls, df: pd.DataFrame) -> pd.Series:
         return df.apply(cls.classify_from_row, axis=1)
 
     @classmethod
     def evaluate(cls):
         datasets = cls.get_dataset()
-        predicted = cls.predict(datasets["X_train"])
-        y_train = datasets["Y_train"]
+        predicted = cls.predict(datasets.X_train)
+        y_train = datasets.Y_train
 
         def _stat(score_func, target, predicted):
             return str(round(score_func(target, predicted) * 100, 2)) + "%"
 
         def _print_confusion_matrix(target, predicted):
             cm = confusion_matrix(target, predicted)
             result = f"TN={cm[0, 0]} FP={cm[0, 1]}\n"
@@ -306,16 +307,16 @@
         print("Recall:", _stat(recall_score, y_train, predicted))
         print("Precision:", _stat(precision_score, y_train, predicted))
         print("Accuracy:", _stat(accuracy_score, y_train, predicted))
         print("Roc Auc:", _stat(roc_auc_score, y_train, predicted))
         print("Confusion matrix:\n", _print_confusion_matrix(y_train, predicted))
         print()
 
-        predicted = cls.predict(datasets["X_test"])
-        y_test = datasets["Y_test"]
+        predicted = cls.predict(datasets.X_test)
+        y_test = datasets.Y_test
 
         print("Test set scores")
         print("---------------")
         print("Recall:", _stat(recall_score, y_test, predicted))
         print("Precision:", _stat(precision_score, y_test, predicted))
         print("Accuracy:", _stat(accuracy_score, y_test, predicted))
         print("Roc Auc:", _stat(roc_auc_score, y_test, predicted))
@@ -329,16 +330,16 @@
     @classmethod
     def train(cls) -> None:
         vectorizer = cls.get_vectorizer()
 
         LOGGER.info("Training SVM classifier...")
         model = SVC(kernel="rbf", C=cls.C, gamma=cls.gamma)
         datasets = cls.load_dataset()
-        vfeatures = vectorizer.transform(cls.get_dataset_features(datasets["X_train"]))
-        model.fit(vfeatures, datasets["Y_train"])
+        vfeatures = vectorizer.transform(cls.get_dataset_features(datasets.X_train))
+        model.fit(vfeatures, datasets.Y_train)
         return model
 
     @classmethod
     def classify_response(cls, response: HtmlResponse) -> bool:
         """ """
 
         vectorizer = cls.get_vectorizer()
```

### Comparing `e-models-1.5.2.1/emodels/datasets/tokenizers.py` & `e-models-1.5.3/emodels/datasets/tokenizers.py`

 * *Files identical despite different names*

### Comparing `e-models-1.5.2.1/emodels/datasets/utils.py` & `e-models-1.5.3/emodels/datasets/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,29 @@
 """
 """
 import os
 import abc
 import gzip
 import json
 import logging
+from functools import partial
 from random import random
-from typing import List, Literal, Tuple, Protocol, cast, Dict, Any, IO, Optional
+from typing import List, Literal, Tuple, Protocol, cast, Dict, Any, IO, Optional, TypedDict
 
-from typing_extensions import Self, TypedDict
-from shub_workflow.deliver.futils import exists
+from typing_extensions import Self
 from scrapy.http import TextResponse
 import lxml.html
 
+try:
+    from datasets import Dataset as HuggingFaceDataset, DatasetDict as HuggingFaceDatasetDict
+except ImportError:
+    pass
+
 from emodels.config import EMODELS_DIR, EMODELS_ITEMS_DIR
+from emodels.scrapyutils.response import ExtractTextResponse
 
 
 LOGGER = logging.getLogger(__name__)
 LOGGER.setLevel(logging.INFO)
 
 NO_TEXT_TAGS = ["script", "style", "noscript"]
 
@@ -99,14 +105,16 @@
         return json.loads(line)
 
     def append(self, data: Dict[str, Any]):
         assert not self._file, "Already opened."
         with self.open("at") as fz:
             print(json.dumps(data), file=fz)
 
+
+class ItemsDatasetFilename(DatasetFilename):
     @classmethod
     def build_from_items(
         cls,
         name: str,
         project: str,
         classes: Optional[Tuple[str]] = None,
         dataset_ratio: Tuple[float, ...] = DEFAULT_DATASET_RATIO,
@@ -117,27 +125,52 @@
         - project is the name of the project the dataset belongs to. It will determine the storing filename.
         - If classes is a tuple of strings, select only the specified
         item subfolders.
         - dataset_ratio is the same for get_random_dataset() and determines how samples are distributed
           among train, test and validation buckets.
         """
         result = cls.local_by_name(name, project)
-        if exists(result):
+        if os.path.exists(result):
             raise ValueError(
                 "Output file already exists. "
                 f'open with {cls.__name__}.local_by_name("{name}", "{project}") or remove it for rebuilding'
             )
         for sf in os.listdir(EMODELS_ITEMS_DIR):
             for f in os.listdir(os.path.join(EMODELS_ITEMS_DIR, sf)):
                 df = DatasetFilename(os.path.join(EMODELS_ITEMS_DIR, sf, f))
                 for sample in df:
                     sample["dataset_bucket"] = get_random_dataset(dataset_ratio)
                     result.append(sample)
         return result
 
+    def to_hfdataset(self) -> HuggingFaceDatasetDict:
+        """
+        Convert to HuggingFace Dataset suitable for usage in transformers
+        """
+
+        def _generator(bucket: DatasetBucket):
+            for sample in self:
+                if sample["dataset_bucket"] != bucket:
+                    continue
+                for key, idx in sample["indexes"].items():
+                    if idx is None:
+                        continue
+                    yield {
+                        "markdown": sample["markdown"],
+                        "attribute": key,
+                        "start": idx[0],
+                        "end": idx[1],
+                    }
+
+        train = HuggingFaceDataset.from_generator(partial(_generator, "train"))
+        test = HuggingFaceDataset.from_generator(partial(_generator, "test"))
+
+        ds = HuggingFaceDatasetDict({"train": train, "test": test})
+        return ds
+
 
 class WebsiteSampleData(TypedDict):
     url: str
     body: str
     status: int
 
 
@@ -203,23 +236,30 @@
                 continue
             text = element.text.strip()
             if text:
                 texts.append(text)
         return texts
 
 
-def build_response_from_sample_data(sampledata: WebsiteSampleData) -> TextResponse:
-    response = TextResponse(
+def build_response_from_sample_data(sampledata: WebsiteSampleData) -> ExtractTextResponse:
+    response = ExtractTextResponse(
         url=sampledata["url"],
         body=sampledata["body"].encode("utf8"),
         status=sampledata["status"],
     )
     return response
 
 
 def build_sample_data_from_response(response: TextResponse) -> WebsiteSampleData:
     sampledata: WebsiteSampleData = {
         "url": response.url,
         "body": response.text,
         "status": response.status,
     }
     return sampledata
+
+
+def save_sample_data_from_response(response: TextResponse, filename: str | WebsiteDatasetFilename):
+    sampledata = build_sample_data_from_response(response)
+    if not isinstance(filename, WebsiteDatasetFilename):
+        filename = WebsiteDatasetFilename(filename)
+    filename.append(dict(sampledata))
```

### Comparing `e-models-1.5.2.1/emodels/html2text/__init__.py` & `e-models-1.5.3/emodels/html2text/__init__.py`

 * *Files identical despite different names*

### Comparing `e-models-1.5.2.1/emodels/html2text/config.py` & `e-models-1.5.3/emodels/html2text/config.py`

 * *Files identical despite different names*

### Comparing `e-models-1.5.2.1/emodels/html2text/utils.py` & `e-models-1.5.3/emodels/html2text/utils.py`

 * *Files identical despite different names*

### Comparing `e-models-1.5.2.1/emodels/scrapyutils/loader.py` & `e-models-1.5.3/emodels/scrapyutils/loader.py`

 * *Files identical despite different names*

### Comparing `e-models-1.5.2.1/emodels/scrapyutils/response.py` & `e-models-1.5.3/emodels/scrapyutils/response.py`

 * *Files identical despite different names*

### Comparing `e-models-1.5.2.1/setup.py` & `e-models-1.5.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 # Automatically created by: shub deploy
 
 from setuptools import setup, find_packages
 
 setup(
     name         = 'e-models',
-    version      = '1.5.2.1',
+    version      = '1.5.3',
     description  = 'Tools for helping build of extraction models with scrapy spiders.',
     long_description = open('README.md').read(),
     long_description_content_type = 'text/markdown',
     license      = 'BSD',
     author       = 'Martin Olveyra',
     author_email = 'molveyra@gmail.com',
     url          = 'https://github.com/kalessin/emodels',
     packages     = find_packages(),
     install_requires=(
         "scikit-learn",
         "scrapy",
         "sentencepiece",
+        "shub-workflow",
     ),
     extras_require = {
         "with-transformers": ["datasets", "torch", "transformers"],
     },
     scripts = [],
     classifiers = [
         'Development Status :: 3 - Alpha',
```

### Comparing `e-models-1.5.2.1/tests/test_html2text.py` & `e-models-1.5.3/tests/test_html2text.py`

 * *Files identical despite different names*

### Comparing `e-models-1.5.2.1/tests/test_scrapyutils.py` & `e-models-1.5.3/tests/test_scrapyutils.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from itemloaders.processors import TakeFirst
 from scrapy import Item, Field
 from scrapy.http import TextResponse
 
 from emodels import config
 from emodels.scrapyutils.loader import ExtractItemLoader
-from emodels.scrapyutils.response import COMMENT_RE, ExtractTextResponse
+from emodels.scrapyutils.response import COMMENT_RE
 from emodels.datasets.utils import DatasetFilename, build_response_from_sample_data
 
 
 class JobItemTest(Item):
     job_title = Field()
     description = Field()
     url = Field()
@@ -72,25 +72,23 @@
             try:
                 for f in os.listdir(dname):
                     os.remove(os.path.join(dname, f))
             except FileNotFoundError:
                 pass
 
     def test_case_one(self):
-        tresponse = self.samples["https://careers.und.edu/jobs/job21.html"]
-        loader = JobItemLoader(response=tresponse)
+        response = self.samples["https://careers.und.edu/jobs/job21.html"]
+        loader = JobItemLoader(response=response)
         loader.add_text_re("job_title", tid="#job_title_2_2")
         loader.add_text_re("employment_type", tid="#employment_type_2_2_0_0")
         loader.add_text_re("job_id", tid="#requisition_identifier_2_2_0")
         loader.add_text_re("description", r"(###\s+.+?)\*\*apply now\*\*", flags=re.S | re.I)
 
         item = loader.load_item()
 
-        response = loader.context["response"]
-
         self.assertFalse(COMMENT_RE.findall(item["description"]))
         self.assertEqual(COMMENT_RE.sub("", response.markdown_ids), response.markdown)
         self.assertEqual(COMMENT_RE.sub("", response.markdown_classes), response.markdown)
 
         self.assertEqual(
             item["description"][:80],
             "###  Student Athlete Support Services Coord \n\n  * __ 492556 \n\n\n\n  * __ Grand For",
@@ -117,15 +115,15 @@
         self.assertEqual(data["markdown"][slice(*data["indexes"]["employment_type"])], "Full-time Staff")
 
         self.assertEqual(data["markdown"][slice(*data["indexes"]["description"])], item["description"])
 
         self.assertTrue(response.text_re(tid=".job-field job-title"))
 
     def test_case_two(self):
-        response = self.samples["https://yell.com/result.html"].replace(cls=ExtractTextResponse)
+        response = self.samples["https://yell.com/result.html"]
 
         for r in response.css_split(".businessCapsule--mainRow"):
             loader = BusinessSearchItemLoader(response=r)
             loader.add_text_re("name", r"##(.+)")
             loader.add_text_re("phone", r"Tel([\s\d]+)", tid="#telephone")
             loader.add_text_re("website", r"Website\]\((.+?)\)")
             loader.add_text_re("address", r"\[(?:.+\|)?(.+)\]\(.+view=map")
@@ -169,22 +167,21 @@
             extracted[5]["profile_url"], "https://yell.com/biz/jack-gowans-and-marc-dickson-inverness-901395225/"
         )
         self.assertEqual(extracted[6]["locality"], "Inverness")
         self.assertEqual(extracted[7]["street"], "York House, 20, Church St")
         self.assertEqual(extracted[8]["postal_code"], "IV1 1DF")
 
     def test_case_three(self):
-        response = self.samples["https://npc.isolvedhire.com/jobs/857557.html"].replace(cls=ExtractTextResponse)
+        response = self.samples["https://npc.isolvedhire.com/jobs/857557.html"]
         self.assertEqual(
             response.text_re(tid=".job-items"),
             [("Holbrook, AZ, USA", 461, 478), ("13.85", 487, 492), ("Hourly", 501, 507), ("Part Time", 516, 525)],
         )
 
-        tresponse = self.samples["https://npc.isolvedhire.com/jobs/857557.html"]
-        loader = JobItemLoader(response=tresponse)
+        loader = JobItemLoader(response=response)
 
         loader.add_text_re("locality", tid=".job-items")
         loader.add_text_re("employment_type", tid=".job-items", idx=3)
 
         item = loader.load_item()
         self.assertEqual(item["locality"], "Holbrook, AZ, USA")
         self.assertEqual(item["employment_type"], "Part Time")
```

