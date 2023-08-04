# Comparing `tmp/distool-0.1.9.1.tar.gz` & `tmp/distool-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "distool-0.1.9.1.tar", last modified: Sun Jul 30 14:30:01 2023, max compression
+gzip compressed data, was "distool-1.0.0.tar", last modified: Fri Aug  4 21:53:29 2023, max compression
```

## Comparing `distool-0.1.9.1.tar` & `distool-1.0.0.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-07-30 14:30:01.248784 distool-0.1.9.1/
--rw-r--r--   0 michilegorov   (501) staff       (20)     1068 2023-07-16 22:12:30.000000 distool-0.1.9.1/LICENSE.txt
--rw-r--r--   0 michilegorov   (501) staff       (20)     5975 2023-07-30 14:30:01.248965 distool-0.1.9.1/PKG-INFO
--rw-r--r--   0 michilegorov   (501) staff       (20)     5129 2023-07-16 22:12:30.000000 distool-0.1.9.1/README.md
-drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-07-30 14:30:01.226158 distool-0.1.9.1/distool/
--rw-r--r--   0 michilegorov   (501) staff       (20)      836 2023-07-16 22:12:30.000000 distool-0.1.9.1/distool/__init__.py
-drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-07-30 14:30:01.229639 distool-0.1.9.1/distool/base/
--rw-r--r--   0 michilegorov   (501) staff       (20)      248 2023-07-16 22:12:30.000000 distool-0.1.9.1/distool/base/__init__.py
--rw-r--r--   0 michilegorov   (501) staff       (20)     2511 2023-07-16 22:12:30.000000 distool-0.1.9.1/distool/base/estimators.py
-drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-07-30 14:30:01.230414 distool-0.1.9.1/distool/data/
--rw-r--r--   0 michilegorov   (501) staff       (20)   240820 2023-07-16 22:12:30.000000 distool-0.1.9.1/distool/data/symptoms.json
-drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-07-30 14:30:01.232741 distool-0.1.9.1/distool/estimators/
--rw-r--r--   0 michilegorov   (501) staff       (20)      441 2023-07-16 22:12:30.000000 distool-0.1.9.1/distool/estimators/__init__.py
--rw-r--r--   0 michilegorov   (501) staff       (20)     4943 2023-07-16 22:12:30.000000 distool-0.1.9.1/distool/estimators/classifiers.py
-drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-07-30 14:30:01.236264 distool-0.1.9.1/distool/feature_extraction/
--rw-r--r--   0 michilegorov   (501) staff       (20)      586 2023-07-16 22:12:30.000000 distool-0.1.9.1/distool/feature_extraction/__init__.py
--rw-r--r--   0 michilegorov   (501) staff       (20)     3880 2023-07-16 22:12:30.000000 distool-0.1.9.1/distool/feature_extraction/anamnesis.py
--rw-r--r--   0 michilegorov   (501) staff       (20)     2000 2023-07-16 22:12:30.000000 distool-0.1.9.1/distool/feature_extraction/dumb_extractor.py
--rw-r--r--   0 michilegorov   (501) staff       (20)     6538 2023-07-16 22:12:30.000000 distool-0.1.9.1/distool/feature_extraction/smart_extractor.py
--rw-r--r--   0 michilegorov   (501) staff       (20)      917 2023-07-16 22:12:30.000000 distool-0.1.9.1/distool/feature_extraction/symptom.py
--rw-r--r--   0 michilegorov   (501) staff       (20)     3525 2023-07-16 22:12:30.000000 distool-0.1.9.1/distool/feature_extraction/symptom_collection.py
--rw-r--r--   0 michilegorov   (501) staff       (20)      547 2023-07-16 22:12:30.000000 distool-0.1.9.1/distool/feature_extraction/symptom_status.py
-drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-07-30 14:30:01.237249 distool-0.1.9.1/distool/interpretation/
--rw-r--r--   0 michilegorov   (501) staff       (20)      279 2023-07-16 22:12:30.000000 distool-0.1.9.1/distool/interpretation/__init__.py
--rw-r--r--   0 michilegorov   (501) staff       (20)     3442 2023-07-16 22:12:30.000000 distool-0.1.9.1/distool/interpretation/explainer.py
-drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-07-30 14:30:01.238114 distool-0.1.9.1/distool/metrics/
--rw-r--r--   0 michilegorov   (501) staff       (20)        0 2023-07-16 22:12:30.000000 distool-0.1.9.1/distool/metrics/__init__.py
-drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-07-30 14:30:01.239994 distool-0.1.9.1/distool/metrics/extractor/
--rw-r--r--   0 michilegorov   (501) staff       (20)        0 2023-07-16 22:12:30.000000 distool-0.1.9.1/distool/metrics/extractor/__init__.py
--rw-r--r--   0 michilegorov   (501) staff       (20)     2475 2023-07-16 22:12:30.000000 distool-0.1.9.1/distool/metrics/extractor/compute.py
--rw-r--r--   0 michilegorov   (501) staff       (20)     7709 2023-07-16 22:12:30.000000 distool-0.1.9.1/distool/metrics/extractor/create_showcase.py
-drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-07-30 14:30:01.243215 distool-0.1.9.1/distool/models/
--rw-r--r--   0 michilegorov   (501) staff       (20)      152 2023-07-16 22:12:30.000000 distool-0.1.9.1/distool/models/__init__.py
--rw-r--r--   0 michilegorov   (501) staff       (20)     3360 2023-07-16 22:12:30.000000 distool-0.1.9.1/distool/models/urgency_classifier.py
-drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-07-30 14:30:01.244670 distool-0.1.9.1/distool/tests/
--rw-r--r--   0 michilegorov   (501) staff       (20)        0 2023-07-16 22:12:30.000000 distool-0.1.9.1/distool/tests/__init__.py
--rw-r--r--   0 michilegorov   (501) staff       (20)      959 2023-07-16 22:12:30.000000 distool-0.1.9.1/distool/tests/conftest.py
-drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-07-30 14:30:01.245863 distool-0.1.9.1/distool/tests/estimators/
--rw-r--r--   0 michilegorov   (501) staff       (20)        0 2023-07-16 22:12:30.000000 distool-0.1.9.1/distool/tests/estimators/__init__.py
--rw-r--r--   0 michilegorov   (501) staff       (20)      419 2023-07-16 22:12:30.000000 distool-0.1.9.1/distool/tests/estimators/test_classifier.py
--rw-r--r--   0 michilegorov   (501) staff       (20)      787 2023-07-16 22:12:30.000000 distool-0.1.9.1/distool/tests/estimators/test_fedot_classifier.py
-drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-07-30 14:30:01.246626 distool-0.1.9.1/distool/tests/explainer/
--rw-r--r--   0 michilegorov   (501) staff       (20)        0 2023-07-16 22:12:30.000000 distool-0.1.9.1/distool/tests/explainer/__init__.py
--rw-r--r--   0 michilegorov   (501) staff       (20)     1346 2023-07-16 22:12:30.000000 distool-0.1.9.1/distool/tests/explainer/test_explainer.py
-drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-07-30 14:30:01.247480 distool-0.1.9.1/distool/tests/extractors/
--rw-r--r--   0 michilegorov   (501) staff       (20)        0 2023-07-16 22:12:30.000000 distool-0.1.9.1/distool/tests/extractors/__init__.py
--rw-r--r--   0 michilegorov   (501) staff       (20)     1630 2023-07-16 22:12:30.000000 distool-0.1.9.1/distool/tests/extractors/test_symptom_extractor.py
--rw-r--r--   0 michilegorov   (501) staff       (20)       37 2023-07-16 22:12:30.000000 distool-0.1.9.1/distool/tests/test_base.py
-drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-07-30 14:30:01.228407 distool-0.1.9.1/distool.egg-info/
--rw-r--r--   0 michilegorov   (501) staff       (20)     5975 2023-07-30 14:30:01.000000 distool-0.1.9.1/distool.egg-info/PKG-INFO
--rw-r--r--   0 michilegorov   (501) staff       (20)     1384 2023-07-30 14:30:01.000000 distool-0.1.9.1/distool.egg-info/SOURCES.txt
--rw-r--r--   0 michilegorov   (501) staff       (20)        1 2023-07-30 14:30:01.000000 distool-0.1.9.1/distool.egg-info/dependency_links.txt
--rw-r--r--   0 michilegorov   (501) staff       (20)       64 2023-07-30 14:30:01.000000 distool-0.1.9.1/distool.egg-info/requires.txt
--rw-r--r--   0 michilegorov   (501) staff       (20)       17 2023-07-30 14:30:01.000000 distool-0.1.9.1/distool.egg-info/top_level.txt
-drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-07-30 14:30:01.248342 distool-0.1.9.1/examples/
--rw-r--r--   0 michilegorov   (501) staff       (20)        0 2023-02-04 10:03:31.000000 distool-0.1.9.1/examples/__init__.py
--rw-r--r--   0 michilegorov   (501) staff       (20)     1116 2023-07-16 22:12:30.000000 distool-0.1.9.1/examples/pipeline_example.py
--rw-r--r--   0 michilegorov   (501) staff       (20)      295 2023-07-30 14:29:57.000000 distool-0.1.9.1/pyproject.toml
--rw-r--r--   0 michilegorov   (501) staff       (20)       79 2023-07-30 14:30:01.249551 distool-0.1.9.1/setup.cfg
--rw-r--r--   0 michilegorov   (501) staff       (20)     1332 2023-07-30 14:23:43.000000 distool-0.1.9.1/setup.py
+drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-08-04 21:53:29.171783 distool-1.0.0/
+-rw-r--r--   0 michilegorov   (501) staff       (20)     1068 2023-07-16 22:12:30.000000 distool-1.0.0/LICENSE.txt
+-rw-r--r--   0 michilegorov   (501) staff       (20)     5993 2023-08-04 21:53:29.171907 distool-1.0.0/PKG-INFO
+-rw-r--r--   0 michilegorov   (501) staff       (20)     5129 2023-07-16 22:12:30.000000 distool-1.0.0/README.md
+drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-08-04 21:53:29.156892 distool-1.0.0/distool/
+-rw-r--r--   0 michilegorov   (501) staff       (20)      836 2023-07-16 22:12:30.000000 distool-1.0.0/distool/__init__.py
+drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-08-04 21:53:29.158407 distool-1.0.0/distool/base/
+-rw-r--r--   0 michilegorov   (501) staff       (20)      248 2023-07-16 22:12:30.000000 distool-1.0.0/distool/base/__init__.py
+-rw-r--r--   0 michilegorov   (501) staff       (20)     2511 2023-07-16 22:12:30.000000 distool-1.0.0/distool/base/estimators.py
+drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-08-04 21:53:29.160168 distool-1.0.0/distool/data/
+-rw-r--r--   0 michilegorov   (501) staff       (20)   240820 2023-07-16 22:12:30.000000 distool-1.0.0/distool/data/symptoms.json
+drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-08-04 21:53:29.161354 distool-1.0.0/distool/estimators/
+-rw-r--r--   0 michilegorov   (501) staff       (20)      441 2023-07-16 22:12:30.000000 distool-1.0.0/distool/estimators/__init__.py
+-rw-r--r--   0 michilegorov   (501) staff       (20)     5101 2023-08-04 12:38:28.000000 distool-1.0.0/distool/estimators/classifiers.py
+drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-08-04 21:53:29.165607 distool-1.0.0/distool/feature_extraction/
+-rw-r--r--   0 michilegorov   (501) staff       (20)      586 2023-07-16 22:12:30.000000 distool-1.0.0/distool/feature_extraction/__init__.py
+-rw-r--r--   0 michilegorov   (501) staff       (20)     3880 2023-07-16 22:12:30.000000 distool-1.0.0/distool/feature_extraction/anamnesis.py
+-rw-r--r--   0 michilegorov   (501) staff       (20)     2000 2023-07-16 22:12:30.000000 distool-1.0.0/distool/feature_extraction/dumb_extractor.py
+-rw-r--r--   0 michilegorov   (501) staff       (20)     6538 2023-07-16 22:12:30.000000 distool-1.0.0/distool/feature_extraction/smart_extractor.py
+-rw-r--r--   0 michilegorov   (501) staff       (20)      917 2023-07-16 22:12:30.000000 distool-1.0.0/distool/feature_extraction/symptom.py
+-rw-r--r--   0 michilegorov   (501) staff       (20)     3525 2023-07-16 22:12:30.000000 distool-1.0.0/distool/feature_extraction/symptom_collection.py
+-rw-r--r--   0 michilegorov   (501) staff       (20)      547 2023-07-16 22:12:30.000000 distool-1.0.0/distool/feature_extraction/symptom_status.py
+drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-08-04 21:53:29.166078 distool-1.0.0/distool/interpretation/
+-rw-r--r--   0 michilegorov   (501) staff       (20)      279 2023-07-16 22:12:30.000000 distool-1.0.0/distool/interpretation/__init__.py
+-rw-r--r--   0 michilegorov   (501) staff       (20)     3446 2023-08-04 13:21:06.000000 distool-1.0.0/distool/interpretation/explainer.py
+drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-08-04 21:53:29.166407 distool-1.0.0/distool/metrics/
+-rw-r--r--   0 michilegorov   (501) staff       (20)        0 2023-07-16 22:12:30.000000 distool-1.0.0/distool/metrics/__init__.py
+drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-08-04 21:53:29.167094 distool-1.0.0/distool/metrics/extractor/
+-rw-r--r--   0 michilegorov   (501) staff       (20)        0 2023-07-16 22:12:30.000000 distool-1.0.0/distool/metrics/extractor/__init__.py
+-rw-r--r--   0 michilegorov   (501) staff       (20)     2475 2023-07-16 22:12:30.000000 distool-1.0.0/distool/metrics/extractor/compute.py
+-rw-r--r--   0 michilegorov   (501) staff       (20)     7709 2023-07-16 22:12:30.000000 distool-1.0.0/distool/metrics/extractor/create_showcase.py
+drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-08-04 21:53:29.168209 distool-1.0.0/distool/models/
+-rw-r--r--   0 michilegorov   (501) staff       (20)      152 2023-07-16 22:12:30.000000 distool-1.0.0/distool/models/__init__.py
+-rw-r--r--   0 michilegorov   (501) staff       (20)     3360 2023-07-16 22:12:30.000000 distool-1.0.0/distool/models/urgency_classifier.py
+drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-08-04 21:53:29.169141 distool-1.0.0/distool/tests/
+-rw-r--r--   0 michilegorov   (501) staff       (20)        0 2023-07-16 22:12:30.000000 distool-1.0.0/distool/tests/__init__.py
+-rw-r--r--   0 michilegorov   (501) staff       (20)      959 2023-07-16 22:12:30.000000 distool-1.0.0/distool/tests/conftest.py
+drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-08-04 21:53:29.170144 distool-1.0.0/distool/tests/estimators/
+-rw-r--r--   0 michilegorov   (501) staff       (20)        0 2023-07-16 22:12:30.000000 distool-1.0.0/distool/tests/estimators/__init__.py
+-rw-r--r--   0 michilegorov   (501) staff       (20)      419 2023-07-16 22:12:30.000000 distool-1.0.0/distool/tests/estimators/test_classifier.py
+-rw-r--r--   0 michilegorov   (501) staff       (20)      787 2023-07-16 22:12:30.000000 distool-1.0.0/distool/tests/estimators/test_fedot_classifier.py
+drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-08-04 21:53:29.170638 distool-1.0.0/distool/tests/explainer/
+-rw-r--r--   0 michilegorov   (501) staff       (20)        0 2023-07-16 22:12:30.000000 distool-1.0.0/distool/tests/explainer/__init__.py
+-rw-r--r--   0 michilegorov   (501) staff       (20)     1346 2023-07-16 22:12:30.000000 distool-1.0.0/distool/tests/explainer/test_explainer.py
+drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-08-04 21:53:29.171111 distool-1.0.0/distool/tests/extractors/
+-rw-r--r--   0 michilegorov   (501) staff       (20)        0 2023-07-16 22:12:30.000000 distool-1.0.0/distool/tests/extractors/__init__.py
+-rw-r--r--   0 michilegorov   (501) staff       (20)     1630 2023-07-16 22:12:30.000000 distool-1.0.0/distool/tests/extractors/test_symptom_extractor.py
+-rw-r--r--   0 michilegorov   (501) staff       (20)       37 2023-07-16 22:12:30.000000 distool-1.0.0/distool/tests/test_base.py
+drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-08-04 21:53:29.157845 distool-1.0.0/distool.egg-info/
+-rw-r--r--   0 michilegorov   (501) staff       (20)     5993 2023-08-04 21:53:29.000000 distool-1.0.0/distool.egg-info/PKG-INFO
+-rw-r--r--   0 michilegorov   (501) staff       (20)     1384 2023-08-04 21:53:29.000000 distool-1.0.0/distool.egg-info/SOURCES.txt
+-rw-r--r--   0 michilegorov   (501) staff       (20)        1 2023-08-04 21:53:29.000000 distool-1.0.0/distool.egg-info/dependency_links.txt
+-rw-r--r--   0 michilegorov   (501) staff       (20)       64 2023-08-04 21:53:29.000000 distool-1.0.0/distool.egg-info/requires.txt
+-rw-r--r--   0 michilegorov   (501) staff       (20)       17 2023-08-04 21:53:29.000000 distool-1.0.0/distool.egg-info/top_level.txt
+drwxr-xr-x   0 michilegorov   (501) staff       (20)        0 2023-08-04 21:53:29.171529 distool-1.0.0/examples/
+-rw-r--r--   0 michilegorov   (501) staff       (20)        0 2023-02-04 10:03:31.000000 distool-1.0.0/examples/__init__.py
+-rw-r--r--   0 michilegorov   (501) staff       (20)     1116 2023-07-16 22:12:30.000000 distool-1.0.0/examples/pipeline_example.py
+-rw-r--r--   0 michilegorov   (501) staff       (20)      293 2023-08-04 21:52:40.000000 distool-1.0.0/pyproject.toml
+-rw-r--r--   0 michilegorov   (501) staff       (20)       79 2023-08-04 21:53:29.172497 distool-1.0.0/setup.cfg
+-rw-r--r--   0 michilegorov   (501) staff       (20)     1330 2023-08-04 21:53:26.000000 distool-1.0.0/setup.py
```

### Comparing `distool-0.1.9.1/LICENSE.txt` & `distool-1.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `distool-0.1.9.1/PKG-INFO` & `distool-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: distool
-Version: 0.1.9.1
+Version: 1.0.0
 Summary: Disease processing tool kit in Russian
 Home-page: https://github.com/nirma-patient-intake/disease/
-Download-URL: https://github.com/NIRMA-PATIENT-INTAKE/disease/archive/refs/tags/distool.tar.gz
 Author: NIRMA Team of ITMO University
 Author-email: egorovmichil9@gmail.com
 License: MIT
+Download-URL: https://github.com/NIRMA-PATIENT-INTAKE/disease/archive/refs/tags/distool.tar.gz
 Keywords: NLP,Disease,Health Condition
+Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -103,7 +104,9 @@
 [<img src="https://images.weserv.nl/?url=avatars.githubusercontent.com/u/56276056?v=4&h=200&w=200&fit=cover&mask=circle&maxage=7d" width="30" /> Айталина Кривошапкина](https://github.com/aytakr) </br> разработчик
 
 [<img src="https://images.weserv.nl/?url=avatars.githubusercontent.com/u/109297759?v=4&h=200&w=200&fit=cover&mask=circle&maxage=7d" width="30" /> Мария Якубова](https://github.com/Shentorin) </br> аналитик
 
 ## Обратная связь
 
 Если у Вас есть какие-то вопросы, можете обращаться к нам по адресу: patientintake@yandex.ru
+
+
```

### Comparing `distool-0.1.9.1/README.md` & `distool-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `distool-0.1.9.1/distool/__init__.py` & `distool-1.0.0/distool/__init__.py`

 * *Files identical despite different names*

### Comparing `distool-0.1.9.1/distool/base/estimators.py` & `distool-1.0.0/distool/base/estimators.py`

 * *Files identical despite different names*

### Comparing `distool-0.1.9.1/distool/data/symptoms.json` & `distool-1.0.0/distool/data/symptoms.json`

 * *Files identical despite different names*

### Comparing `distool-0.1.9.1/distool/estimators/classifiers.py` & `distool-1.0.0/distool/estimators/classifiers.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import joblib
 import numpy as np
 from fedot.api.main import Fedot
 from sklearn.linear_model import LogisticRegression
 
 from distool.base.estimators import BaseEstimator
 
 
@@ -41,14 +42,19 @@
         log_reg: A Logistic Regression classifier.
     """
 
     def __init__(self):
         """Initializes a new instance of the DiseaseClassifier class."""
         self.log_reg = LogisticRegression()
 
+    @staticmethod
+    def load(path: str) -> 'DiseaseClassifier':
+        """ Load model from joblib path """
+        return joblib.load(path)
+
     def fit(self, features: np.array, y: np.array) -> "BaseDiseaseClassifier":
         """Fit the model according to the given training data.
 
         Args:
             features: array-like, shape (n_samples, n_features)
                 Training vector, where n_samples is the number of samples and n_features is the number of features.
             y: array-like, shape (n_samples,)
```

### Comparing `distool-0.1.9.1/distool/feature_extraction/__init__.py` & `distool-1.0.0/distool/feature_extraction/__init__.py`

 * *Files identical despite different names*

### Comparing `distool-0.1.9.1/distool/feature_extraction/anamnesis.py` & `distool-1.0.0/distool/feature_extraction/anamnesis.py`

 * *Files identical despite different names*

### Comparing `distool-0.1.9.1/distool/feature_extraction/dumb_extractor.py` & `distool-1.0.0/distool/feature_extraction/dumb_extractor.py`

 * *Files identical despite different names*

### Comparing `distool-0.1.9.1/distool/feature_extraction/smart_extractor.py` & `distool-1.0.0/distool/feature_extraction/smart_extractor.py`

 * *Files identical despite different names*

### Comparing `distool-0.1.9.1/distool/feature_extraction/symptom.py` & `distool-1.0.0/distool/feature_extraction/symptom.py`

 * *Files identical despite different names*

### Comparing `distool-0.1.9.1/distool/feature_extraction/symptom_collection.py` & `distool-1.0.0/distool/feature_extraction/symptom_collection.py`

 * *Files identical despite different names*

### Comparing `distool-0.1.9.1/distool/feature_extraction/symptom_status.py` & `distool-1.0.0/distool/feature_extraction/symptom_status.py`

 * *Files identical despite different names*

### Comparing `distool-0.1.9.1/distool/interpretation/explainer.py` & `distool-1.0.0/distool/interpretation/explainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,17 +57,17 @@
         no_symptoms = [
             s.id_name for s, f in symptom_analysis if f == SymptomStatus.NO.value
         ]
 
         return (
             f"Наблюдается {disease_name} с вероятностью {round(disease_proba * 100)}%.\n"
             f"Это потому что у вас наблюдаются следующие симптомы: "
-            f"{''.join(has_symptoms)}\n"
+            f"{', '.join(has_symptoms)}\n"
             f"И отрицаются следующие: "
-            f"{''.join(no_symptoms)}"
+            f"{', '.join(no_symptoms)}"
         )
 
 
 class FedotBasedExplainer(BaseExplainer):
     """
     An explainer based on the FEDOT framework.
```

### Comparing `distool-0.1.9.1/distool/metrics/extractor/compute.py` & `distool-1.0.0/distool/metrics/extractor/compute.py`

 * *Files identical despite different names*

### Comparing `distool-0.1.9.1/distool/metrics/extractor/create_showcase.py` & `distool-1.0.0/distool/metrics/extractor/create_showcase.py`

 * *Files identical despite different names*

### Comparing `distool-0.1.9.1/distool/models/urgency_classifier.py` & `distool-1.0.0/distool/models/urgency_classifier.py`

 * *Files identical despite different names*

### Comparing `distool-0.1.9.1/distool/tests/conftest.py` & `distool-1.0.0/distool/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `distool-0.1.9.1/distool/tests/estimators/test_fedot_classifier.py` & `distool-1.0.0/distool/tests/estimators/test_fedot_classifier.py`

 * *Files identical despite different names*

### Comparing `distool-0.1.9.1/distool/tests/explainer/test_explainer.py` & `distool-1.0.0/distool/tests/explainer/test_explainer.py`

 * *Files identical despite different names*

### Comparing `distool-0.1.9.1/distool/tests/extractors/test_symptom_extractor.py` & `distool-1.0.0/distool/tests/extractors/test_symptom_extractor.py`

 * *Files identical despite different names*

### Comparing `distool-0.1.9.1/distool.egg-info/PKG-INFO` & `distool-1.0.0/distool.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: distool
-Version: 0.1.9.1
+Version: 1.0.0
 Summary: Disease processing tool kit in Russian
 Home-page: https://github.com/nirma-patient-intake/disease/
-Download-URL: https://github.com/NIRMA-PATIENT-INTAKE/disease/archive/refs/tags/distool.tar.gz
 Author: NIRMA Team of ITMO University
 Author-email: egorovmichil9@gmail.com
 License: MIT
+Download-URL: https://github.com/NIRMA-PATIENT-INTAKE/disease/archive/refs/tags/distool.tar.gz
 Keywords: NLP,Disease,Health Condition
+Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -103,7 +104,9 @@
 [<img src="https://images.weserv.nl/?url=avatars.githubusercontent.com/u/56276056?v=4&h=200&w=200&fit=cover&mask=circle&maxage=7d" width="30" /> Айталина Кривошапкина](https://github.com/aytakr) </br> разработчик
 
 [<img src="https://images.weserv.nl/?url=avatars.githubusercontent.com/u/109297759?v=4&h=200&w=200&fit=cover&mask=circle&maxage=7d" width="30" /> Мария Якубова](https://github.com/Shentorin) </br> аналитик
 
 ## Обратная связь
 
 Если у Вас есть какие-то вопросы, можете обращаться к нам по адресу: patientintake@yandex.ru
+
+
```

### Comparing `distool-0.1.9.1/distool.egg-info/SOURCES.txt` & `distool-1.0.0/distool.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `distool-0.1.9.1/examples/pipeline_example.py` & `distool-1.0.0/examples/pipeline_example.py`

 * *Files identical despite different names*

### Comparing `distool-0.1.9.1/setup.py` & `distool-1.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     name="distool",
     description="Disease processing tool kit in Russian",
     packages=find_packages(),
     package_data={"distool": ["data/symptoms.json"]},
     include_package_data=True,
     long_description=open("./README.md").read(),
     long_description_content_type="text/markdown",
-    # version="0.1.9",
+    version="1.0.0",
     license="MIT",
     author="NIRMA Team of ITMO University",
     author_email="egorovmichil9@gmail.com",
     url="https://github.com/nirma-patient-intake/disease/",
     download_url="https://github.com/NIRMA-PATIENT-INTAKE/disease/archive/refs/tags/distool.tar.gz",
     keywords=[
         "NLP",
```

