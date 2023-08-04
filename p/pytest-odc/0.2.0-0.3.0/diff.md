# Comparing `tmp/pytest-odc-0.2.0.tar.gz` & `tmp/pytest-odc-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-odc-0.2.0.tar", last modified: Tue Jul 18 06:51:15 2023, max compression
+gzip compressed data, was "pytest-odc-0.3.0.tar", last modified: Fri Aug  4 02:13:42 2023, max compression
```

## Comparing `pytest-odc-0.2.0.tar` & `pytest-odc-0.3.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 omad      (1000) omad      (1000)        0 2023-07-18 06:51:15.929176 pytest-odc-0.2.0/
--rw-rw-r--   0 omad      (1000) omad      (1000)    11357 2023-06-20 23:48:32.000000 pytest-odc-0.2.0/LICENSE
--rw-rw-r--   0 omad      (1000) omad      (1000)       97 2023-07-13 06:48:28.000000 pytest-odc-0.2.0/MANIFEST.in
--rw-rw-r--   0 omad      (1000) omad      (1000)     5382 2023-07-18 06:51:15.929176 pytest-odc-0.2.0/PKG-INFO
--rw-rw-r--   0 omad      (1000) omad      (1000)     4317 2023-07-18 06:49:25.000000 pytest-odc-0.2.0/README.md
-drwxrwxr-x   0 omad      (1000) omad      (1000)        0 2023-07-18 06:51:15.929176 pytest-odc-0.2.0/odc/
-drwxrwxr-x   0 omad      (1000) omad      (1000)        0 2023-07-18 06:51:15.929176 pytest-odc-0.2.0/odc/testing/
--rw-rw-r--   0 omad      (1000) omad      (1000)        0 2023-06-20 03:11:34.000000 pytest-odc-0.2.0/odc/testing/__init__.py
--rw-rw-r--   0 omad      (1000) omad      (1000)     8858 2023-07-18 06:24:56.000000 pytest-odc-0.2.0/odc/testing/database.py
--rw-rw-r--   0 omad      (1000) omad      (1000)     1291 2023-07-18 06:47:07.000000 pytest-odc-0.2.0/pyproject.toml
-drwxrwxr-x   0 omad      (1000) omad      (1000)        0 2023-07-18 06:51:15.929176 pytest-odc-0.2.0/pytest_odc.egg-info/
--rw-rw-r--   0 omad      (1000) omad      (1000)     5382 2023-07-18 06:51:15.000000 pytest-odc-0.2.0/pytest_odc.egg-info/PKG-INFO
--rw-rw-r--   0 omad      (1000) omad      (1000)      329 2023-07-18 06:51:15.000000 pytest-odc-0.2.0/pytest_odc.egg-info/SOURCES.txt
--rw-rw-r--   0 omad      (1000) omad      (1000)        1 2023-07-18 06:51:15.000000 pytest-odc-0.2.0/pytest_odc.egg-info/dependency_links.txt
--rw-rw-r--   0 omad      (1000) omad      (1000)       54 2023-07-18 06:51:15.000000 pytest-odc-0.2.0/pytest_odc.egg-info/entry_points.txt
--rw-rw-r--   0 omad      (1000) omad      (1000)       21 2023-07-18 06:51:15.000000 pytest-odc-0.2.0/pytest_odc.egg-info/requires.txt
--rw-rw-r--   0 omad      (1000) omad      (1000)        4 2023-07-18 06:51:15.000000 pytest-odc-0.2.0/pytest_odc.egg-info/top_level.txt
--rw-rw-r--   0 omad      (1000) omad      (1000)       38 2023-07-18 06:51:15.929176 pytest-odc-0.2.0/setup.cfg
--rw-rw-r--   0 omad      (1000) omad      (1000)       42 2023-07-18 03:28:47.000000 pytest-odc-0.2.0/setup.py
-drwxrwxr-x   0 omad      (1000) omad      (1000)        0 2023-07-18 06:51:15.929176 pytest-odc-0.2.0/tests/
--rw-rw-r--   0 omad      (1000) omad      (1000)      695 2023-06-22 02:28:13.000000 pytest-odc-0.2.0/tests/test_example.py
+drwxrwxr-x   0 omad      (1000) omad      (1000)        0 2023-08-04 02:13:42.407426 pytest-odc-0.3.0/
+-rw-rw-r--   0 omad      (1000) omad      (1000)    11357 2023-06-20 23:48:32.000000 pytest-odc-0.3.0/LICENSE
+-rw-rw-r--   0 omad      (1000) omad      (1000)       97 2023-07-13 06:48:28.000000 pytest-odc-0.3.0/MANIFEST.in
+-rw-rw-r--   0 omad      (1000) omad      (1000)     5432 2023-08-04 02:13:42.407426 pytest-odc-0.3.0/PKG-INFO
+-rw-rw-r--   0 omad      (1000) omad      (1000)     4367 2023-08-04 02:12:53.000000 pytest-odc-0.3.0/README.md
+drwxrwxr-x   0 omad      (1000) omad      (1000)        0 2023-08-04 02:13:42.403427 pytest-odc-0.3.0/odc/
+drwxrwxr-x   0 omad      (1000) omad      (1000)        0 2023-08-04 02:13:42.407426 pytest-odc-0.3.0/odc/testing/
+-rw-rw-r--   0 omad      (1000) omad      (1000)        0 2023-06-20 03:11:34.000000 pytest-odc-0.3.0/odc/testing/__init__.py
+-rw-rw-r--   0 omad      (1000) omad      (1000)     8766 2023-08-04 02:10:20.000000 pytest-odc-0.3.0/odc/testing/database.py
+-rw-rw-r--   0 omad      (1000) omad      (1000)     1291 2023-08-04 02:13:15.000000 pytest-odc-0.3.0/pyproject.toml
+drwxrwxr-x   0 omad      (1000) omad      (1000)        0 2023-08-04 02:13:42.407426 pytest-odc-0.3.0/pytest_odc.egg-info/
+-rw-rw-r--   0 omad      (1000) omad      (1000)     5432 2023-08-04 02:13:42.000000 pytest-odc-0.3.0/pytest_odc.egg-info/PKG-INFO
+-rw-rw-r--   0 omad      (1000) omad      (1000)      329 2023-08-04 02:13:42.000000 pytest-odc-0.3.0/pytest_odc.egg-info/SOURCES.txt
+-rw-rw-r--   0 omad      (1000) omad      (1000)        1 2023-08-04 02:13:42.000000 pytest-odc-0.3.0/pytest_odc.egg-info/dependency_links.txt
+-rw-rw-r--   0 omad      (1000) omad      (1000)       54 2023-08-04 02:13:42.000000 pytest-odc-0.3.0/pytest_odc.egg-info/entry_points.txt
+-rw-rw-r--   0 omad      (1000) omad      (1000)       21 2023-08-04 02:13:42.000000 pytest-odc-0.3.0/pytest_odc.egg-info/requires.txt
+-rw-rw-r--   0 omad      (1000) omad      (1000)        4 2023-08-04 02:13:42.000000 pytest-odc-0.3.0/pytest_odc.egg-info/top_level.txt
+-rw-rw-r--   0 omad      (1000) omad      (1000)       38 2023-08-04 02:13:42.407426 pytest-odc-0.3.0/setup.cfg
+-rw-rw-r--   0 omad      (1000) omad      (1000)       42 2023-07-18 03:28:47.000000 pytest-odc-0.3.0/setup.py
+drwxrwxr-x   0 omad      (1000) omad      (1000)        0 2023-08-04 02:13:42.407426 pytest-odc-0.3.0/tests/
+-rw-rw-r--   0 omad      (1000) omad      (1000)      695 2023-06-22 02:28:13.000000 pytest-odc-0.3.0/tests/test_example.py
```

### Comparing `pytest-odc-0.2.0/LICENSE` & `pytest-odc-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-odc-0.2.0/PKG-INFO` & `pytest-odc-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-odc
-Version: 0.2.0
+Version: 0.3.0
 Summary: A pytest plugin for simplifying ODC database tests
 Author: Open Data Cube
 Project-URL: Homepage, https://www.opendatacube.org/
 Project-URL: Repository, https://github.com/opendatacube/pytest-odc
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
@@ -129,12 +129,14 @@
 issue](https://github.com/omad/pytest-odc/issues) along
 with a detailed description.
 
 Release Process
 ---------------
 
 ```
+# Update version number!
+git tag {version_number}
 rm -rf dist/
 python -m build
 twine upload --repository testpypi dist/*
 twine upload dist/*
 ```
```

### Comparing `pytest-odc-0.2.0/README.md` & `pytest-odc-0.3.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -104,12 +104,14 @@
 issue](https://github.com/omad/pytest-odc/issues) along
 with a detailed description.
 
 Release Process
 ---------------
 
 ```
+# Update version number!
+git tag {version_number}
 rm -rf dist/
 python -m build
 twine upload --repository testpypi dist/*
 twine upload dist/*
 ```
```

### Comparing `pytest-odc-0.2.0/odc/testing/database.py` & `pytest-odc-0.3.0/odc/testing/database.py`

 * *Files 3% similar despite different names*

```diff
@@ -214,17 +214,16 @@
 
     dataset_count = Counter()
     if hasattr(request.module, "DATASETS"):
         create_dataset = Doc2Dataset(odc_test_db.index)
         for filename in request.module.DATASETS:
             filename = data_path / filename
             for _, doc in read_documents(filename):
-                label = doc["ga_label"] if ("ga_label" in doc) else doc["id"]
                 dataset, err = create_dataset(
-                    doc, f"file://example.com/test_dataset/{label}"
+                    doc, filename.absolute().as_uri()
                 )
                 assert dataset is not None, err
                 created = odc_test_db.index.datasets.add(dataset)
                 assert created.uris
                 dataset_count[created.type.name] += 1
 
             print(f"Loaded Datasets: {dataset_count}")
```

### Comparing `pytest-odc-0.2.0/pyproject.toml` & `pytest-odc-0.3.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=58.0.4", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pytest-odc"
-version = "0.2.0"
+version = "0.3.0"
 authors = [
     {name = "Open Data Cube"}
 ]
 #license = "Apache Software License 2.0"
 description = "A pytest plugin for simplifying ODC database tests"
 readme = "README.md"
 #packages = ["odc.testing"]
```

### Comparing `pytest-odc-0.2.0/pytest_odc.egg-info/PKG-INFO` & `pytest-odc-0.3.0/pytest_odc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-odc
-Version: 0.2.0
+Version: 0.3.0
 Summary: A pytest plugin for simplifying ODC database tests
 Author: Open Data Cube
 Project-URL: Homepage, https://www.opendatacube.org/
 Project-URL: Repository, https://github.com/opendatacube/pytest-odc
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
@@ -129,12 +129,14 @@
 issue](https://github.com/omad/pytest-odc/issues) along
 with a detailed description.
 
 Release Process
 ---------------
 
 ```
+# Update version number!
+git tag {version_number}
 rm -rf dist/
 python -m build
 twine upload --repository testpypi dist/*
 twine upload dist/*
 ```
```

### Comparing `pytest-odc-0.2.0/tests/test_example.py` & `pytest-odc-0.3.0/tests/test_example.py`

 * *Files identical despite different names*

