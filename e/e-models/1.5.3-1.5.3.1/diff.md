# Comparing `tmp/e-models-1.5.3.tar.gz` & `tmp/e-models-1.5.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "e-models-1.5.3.tar", last modified: Thu Aug  3 22:16:04 2023, max compression
+gzip compressed data, was "e-models-1.5.3.1.tar", last modified: Thu Aug  3 22:35:33 2023, max compression
```

## Comparing `e-models-1.5.3.tar` & `e-models-1.5.3.1.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-08-03 22:16:04.049945 e-models-1.5.3/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     1501 2023-03-30 21:13:00.000000 e-models-1.5.3/LICENSE
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     3502 2023-08-03 22:16:04.049945 e-models-1.5.3/PKG-INFO
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     2928 2023-07-25 17:58:30.000000 e-models-1.5.3/README.md
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-08-03 22:16:04.045946 e-models-1.5.3/e_models.egg-info/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     3502 2023-08-03 22:16:03.000000 e-models-1.5.3/e_models.egg-info/PKG-INFO
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      655 2023-08-03 22:16:04.000000 e-models-1.5.3/e_models.egg-info/SOURCES.txt
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        1 2023-08-03 22:16:03.000000 e-models-1.5.3/e_models.egg-info/dependency_links.txt
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       97 2023-08-03 22:16:03.000000 e-models-1.5.3/e_models.egg-info/requires.txt
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        8 2023-08-03 22:16:03.000000 e-models-1.5.3/e_models.egg-info/top_level.txt
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-08-03 22:16:04.045946 e-models-1.5.3/emodels/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       22 2023-08-03 22:15:34.000000 e-models-1.5.3/emodels/__init__.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      319 2023-07-26 22:24:33.000000 e-models-1.5.3/emodels/config.py
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-08-03 22:16:04.045946 e-models-1.5.3/emodels/datasets/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        0 2023-06-23 18:11:59.000000 e-models-1.5.3/emodels/datasets/__init__.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)    12168 2023-07-27 20:27:24.000000 e-models-1.5.3/emodels/datasets/models.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     1929 2023-07-05 14:16:56.000000 e-models-1.5.3/emodels/datasets/tokenizers.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     8402 2023-08-03 22:13:54.000000 e-models-1.5.3/emodels/datasets/utils.py
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-08-03 22:16:04.049945 e-models-1.5.3/emodels/html2text/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)    35479 2023-07-21 16:26:32.000000 e-models-1.5.3/emodels/html2text/__init__.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     3873 2023-05-04 18:51:26.000000 e-models-1.5.3/emodels/html2text/config.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      423 2023-05-04 18:51:26.000000 e-models-1.5.3/emodels/html2text/elements.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       71 2023-05-04 18:51:26.000000 e-models-1.5.3/emodels/html2text/typing.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     8034 2023-05-04 18:51:26.000000 e-models-1.5.3/emodels/html2text/utils.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        0 2023-05-04 18:51:26.000000 e-models-1.5.3/emodels/py.typed
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-08-03 22:16:04.049945 e-models-1.5.3/emodels/scrapyutils/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      137 2023-06-23 22:04:28.000000 e-models-1.5.3/emodels/scrapyutils/__init__.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     2575 2023-07-26 22:24:33.000000 e-models-1.5.3/emodels/scrapyutils/loader.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     6000 2023-07-21 19:40:03.000000 e-models-1.5.3/emodels/scrapyutils/response.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       31 2023-03-30 21:32:48.000000 e-models-1.5.3/pyproject.toml
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       38 2023-08-03 22:16:04.049945 e-models-1.5.3/setup.cfg
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     1079 2023-08-03 22:15:45.000000 e-models-1.5.3/setup.py
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-08-03 22:16:04.049945 e-models-1.5.3/tests/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     6346 2023-07-21 17:31:24.000000 e-models-1.5.3/tests/test_html2text.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     8016 2023-08-03 22:14:56.000000 e-models-1.5.3/tests/test_scrapyutils.py
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-08-03 22:35:33.054305 e-models-1.5.3.1/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     1501 2023-03-30 21:13:00.000000 e-models-1.5.3.1/LICENSE
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     3504 2023-08-03 22:35:33.050305 e-models-1.5.3.1/PKG-INFO
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     2928 2023-07-25 17:58:30.000000 e-models-1.5.3.1/README.md
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-08-03 22:35:33.050305 e-models-1.5.3.1/e_models.egg-info/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     3504 2023-08-03 22:35:32.000000 e-models-1.5.3.1/e_models.egg-info/PKG-INFO
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      683 2023-08-03 22:35:33.000000 e-models-1.5.3.1/e_models.egg-info/SOURCES.txt
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        1 2023-08-03 22:35:32.000000 e-models-1.5.3.1/e_models.egg-info/dependency_links.txt
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       97 2023-08-03 22:35:32.000000 e-models-1.5.3.1/e_models.egg-info/requires.txt
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        8 2023-08-03 22:35:32.000000 e-models-1.5.3.1/e_models.egg-info/top_level.txt
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-08-03 22:35:33.050305 e-models-1.5.3.1/emodels/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       24 2023-08-03 22:35:17.000000 e-models-1.5.3.1/emodels/__init__.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      319 2023-07-26 22:24:33.000000 e-models-1.5.3.1/emodels/config.py
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-08-03 22:35:33.050305 e-models-1.5.3.1/emodels/datasets/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        0 2023-06-23 18:11:59.000000 e-models-1.5.3.1/emodels/datasets/__init__.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     2754 2023-08-03 22:28:42.000000 e-models-1.5.3.1/emodels/datasets/hugging.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)    12168 2023-07-27 20:27:24.000000 e-models-1.5.3.1/emodels/datasets/models.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     1929 2023-07-05 14:16:56.000000 e-models-1.5.3.1/emodels/datasets/tokenizers.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     5824 2023-08-03 22:33:57.000000 e-models-1.5.3.1/emodels/datasets/utils.py
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-08-03 22:35:33.050305 e-models-1.5.3.1/emodels/html2text/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)    35479 2023-07-21 16:26:32.000000 e-models-1.5.3.1/emodels/html2text/__init__.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     3873 2023-05-04 18:51:26.000000 e-models-1.5.3.1/emodels/html2text/config.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      423 2023-05-04 18:51:26.000000 e-models-1.5.3.1/emodels/html2text/elements.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       71 2023-05-04 18:51:26.000000 e-models-1.5.3.1/emodels/html2text/typing.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     8034 2023-05-04 18:51:26.000000 e-models-1.5.3.1/emodels/html2text/utils.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        0 2023-05-04 18:51:26.000000 e-models-1.5.3.1/emodels/py.typed
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-08-03 22:35:33.050305 e-models-1.5.3.1/emodels/scrapyutils/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      137 2023-06-23 22:04:28.000000 e-models-1.5.3.1/emodels/scrapyutils/__init__.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     2575 2023-07-26 22:24:33.000000 e-models-1.5.3.1/emodels/scrapyutils/loader.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     6000 2023-07-21 19:40:03.000000 e-models-1.5.3.1/emodels/scrapyutils/response.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       31 2023-03-30 21:32:48.000000 e-models-1.5.3.1/pyproject.toml
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       38 2023-08-03 22:35:33.054305 e-models-1.5.3.1/setup.cfg
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     1081 2023-08-03 22:35:08.000000 e-models-1.5.3.1/setup.py
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-08-03 22:35:33.050305 e-models-1.5.3.1/tests/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     6346 2023-07-21 17:31:24.000000 e-models-1.5.3.1/tests/test_html2text.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     8016 2023-08-03 22:14:56.000000 e-models-1.5.3.1/tests/test_scrapyutils.py
```

### Comparing `e-models-1.5.3/LICENSE` & `e-models-1.5.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `e-models-1.5.3/PKG-INFO` & `e-models-1.5.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: e-models
-Version: 1.5.3
+Version: 1.5.3.1
 Summary: Tools for helping build of extraction models with scrapy spiders.
 Home-page: https://github.com/kalessin/emodels
 Author: Martin Olveyra
 Author-email: molveyra@gmail.com
 License: BSD
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `e-models-1.5.3/README.md` & `e-models-1.5.3.1/README.md`

 * *Files identical despite different names*

### Comparing `e-models-1.5.3/e_models.egg-info/PKG-INFO` & `e-models-1.5.3.1/e_models.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: e-models
-Version: 1.5.3
+Version: 1.5.3.1
 Summary: Tools for helping build of extraction models with scrapy spiders.
 Home-page: https://github.com/kalessin/emodels
 Author: Martin Olveyra
 Author-email: molveyra@gmail.com
 License: BSD
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `e-models-1.5.3/e_models.egg-info/SOURCES.txt` & `e-models-1.5.3.1/e_models.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 e_models.egg-info/dependency_links.txt
 e_models.egg-info/requires.txt
 e_models.egg-info/top_level.txt
 emodels/__init__.py
 emodels/config.py
 emodels/py.typed
 emodels/datasets/__init__.py
+emodels/datasets/hugging.py
 emodels/datasets/models.py
 emodels/datasets/tokenizers.py
 emodels/datasets/utils.py
 emodels/html2text/__init__.py
 emodels/html2text/config.py
 emodels/html2text/elements.py
 emodels/html2text/typing.py
```

### Comparing `e-models-1.5.3/emodels/datasets/models.py` & `e-models-1.5.3.1/emodels/datasets/models.py`

 * *Files identical despite different names*

### Comparing `e-models-1.5.3/emodels/datasets/tokenizers.py` & `e-models-1.5.3.1/emodels/datasets/tokenizers.py`

 * *Files identical despite different names*

### Comparing `e-models-1.5.3/emodels/datasets/utils.py` & `e-models-1.5.3.1/emodels/datasets/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,22 @@
 """
 """
 import os
 import abc
 import gzip
 import json
 import logging
-from functools import partial
 from random import random
-from typing import List, Literal, Tuple, Protocol, cast, Dict, Any, IO, Optional, TypedDict
+from typing import List, Literal, Tuple, Protocol, cast, Dict, Any, IO, TypedDict
 
 from typing_extensions import Self
 from scrapy.http import TextResponse
 import lxml.html
 
-try:
-    from datasets import Dataset as HuggingFaceDataset, DatasetDict as HuggingFaceDatasetDict
-except ImportError:
-    pass
-
-from emodels.config import EMODELS_DIR, EMODELS_ITEMS_DIR
+from emodels.config import EMODELS_DIR
 from emodels.scrapyutils.response import ExtractTextResponse
 
 
 LOGGER = logging.getLogger(__name__)
 LOGGER.setLevel(logging.INFO)
 
 NO_TEXT_TAGS = ["script", "style", "noscript"]
@@ -106,72 +100,14 @@
 
     def append(self, data: Dict[str, Any]):
         assert not self._file, "Already opened."
         with self.open("at") as fz:
             print(json.dumps(data), file=fz)
 
 
-class ItemsDatasetFilename(DatasetFilename):
-    @classmethod
-    def build_from_items(
-        cls,
-        name: str,
-        project: str,
-        classes: Optional[Tuple[str]] = None,
-        dataset_ratio: Tuple[float, ...] = DEFAULT_DATASET_RATIO,
-    ) -> Self:
-        """
-        Build a dataset dict from extracted items in user dataset folder.
-        - name is a name for the dataset. It will determine the storing filename.
-        - project is the name of the project the dataset belongs to. It will determine the storing filename.
-        - If classes is a tuple of strings, select only the specified
-        item subfolders.
-        - dataset_ratio is the same for get_random_dataset() and determines how samples are distributed
-          among train, test and validation buckets.
-        """
-        result = cls.local_by_name(name, project)
-        if os.path.exists(result):
-            raise ValueError(
-                "Output file already exists. "
-                f'open with {cls.__name__}.local_by_name("{name}", "{project}") or remove it for rebuilding'
-            )
-        for sf in os.listdir(EMODELS_ITEMS_DIR):
-            for f in os.listdir(os.path.join(EMODELS_ITEMS_DIR, sf)):
-                df = DatasetFilename(os.path.join(EMODELS_ITEMS_DIR, sf, f))
-                for sample in df:
-                    sample["dataset_bucket"] = get_random_dataset(dataset_ratio)
-                    result.append(sample)
-        return result
-
-    def to_hfdataset(self) -> HuggingFaceDatasetDict:
-        """
-        Convert to HuggingFace Dataset suitable for usage in transformers
-        """
-
-        def _generator(bucket: DatasetBucket):
-            for sample in self:
-                if sample["dataset_bucket"] != bucket:
-                    continue
-                for key, idx in sample["indexes"].items():
-                    if idx is None:
-                        continue
-                    yield {
-                        "markdown": sample["markdown"],
-                        "attribute": key,
-                        "start": idx[0],
-                        "end": idx[1],
-                    }
-
-        train = HuggingFaceDataset.from_generator(partial(_generator, "train"))
-        test = HuggingFaceDataset.from_generator(partial(_generator, "test"))
-
-        ds = HuggingFaceDatasetDict({"train": train, "test": test})
-        return ds
-
-
 class WebsiteSampleData(TypedDict):
     url: str
     body: str
     status: int
 
 
 class WebsiteDatasetFilename(DatasetFilename):
```

### Comparing `e-models-1.5.3/emodels/html2text/__init__.py` & `e-models-1.5.3.1/emodels/html2text/__init__.py`

 * *Files identical despite different names*

### Comparing `e-models-1.5.3/emodels/html2text/config.py` & `e-models-1.5.3.1/emodels/html2text/config.py`

 * *Files identical despite different names*

### Comparing `e-models-1.5.3/emodels/html2text/utils.py` & `e-models-1.5.3.1/emodels/html2text/utils.py`

 * *Files identical despite different names*

### Comparing `e-models-1.5.3/emodels/scrapyutils/loader.py` & `e-models-1.5.3.1/emodels/scrapyutils/loader.py`

 * *Files identical despite different names*

### Comparing `e-models-1.5.3/emodels/scrapyutils/response.py` & `e-models-1.5.3.1/emodels/scrapyutils/response.py`

 * *Files identical despite different names*

### Comparing `e-models-1.5.3/setup.py` & `e-models-1.5.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Automatically created by: shub deploy
 
 from setuptools import setup, find_packages
 
 setup(
     name         = 'e-models',
-    version      = '1.5.3',
+    version      = '1.5.3.1',
     description  = 'Tools for helping build of extraction models with scrapy spiders.',
     long_description = open('README.md').read(),
     long_description_content_type = 'text/markdown',
     license      = 'BSD',
     author       = 'Martin Olveyra',
     author_email = 'molveyra@gmail.com',
     url          = 'https://github.com/kalessin/emodels',
```

### Comparing `e-models-1.5.3/tests/test_html2text.py` & `e-models-1.5.3.1/tests/test_html2text.py`

 * *Files identical despite different names*

### Comparing `e-models-1.5.3/tests/test_scrapyutils.py` & `e-models-1.5.3.1/tests/test_scrapyutils.py`

 * *Files identical despite different names*

