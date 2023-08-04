# Comparing `tmp/fileformats_medimage_extras-0.1.2.tar.gz` & `tmp/fileformats_medimage_extras-0.1.3.tar.gz`

## Comparing `fileformats_medimage_extras-0.1.2.tar` & `fileformats_medimage_extras-0.1.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.2/.codespell-ignorewords
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.2/.flake8
--rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.2/conftest.py
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.2/pytest.ini
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.2/.github/workflows/publish.yml
--rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.2/.github/workflows/tests.yml
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.2/fileformats/extras/medimage/__init__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.2/fileformats/extras/medimage/_version.py
--rw-r--r--   0        0        0     6922 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.2/fileformats/extras/medimage/converters.py
--rw-r--r--   0        0        0     1913 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.2/fileformats/extras/medimage/dicom.py
--rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.2/fileformats/extras/medimage/diffusion.py
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.2/fileformats/extras/medimage/mrtrix3.py
--rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.2/fileformats/extras/medimage/nifti.py
--rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.2/fileformats/extras/medimage/tests/test_neuro_converters.py
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.2/.gitignore
--rw-r--r--   0        0        0    14222 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.2/LICENSE
--rw-r--r--   0        0        0     2151 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.2/README.rst
--rw-r--r--   0        0        0     2232 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.2/pyproject.toml
--rw-r--r--   0        0        0    18991 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.3/.codespell-ignorewords
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.3/.flake8
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.3/conftest.py
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.3/pytest.ini
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.3/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.3/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.3/fileformats/extras/medimage/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.3/fileformats/extras/medimage/_version.py
+-rw-r--r--   0        0        0     7017 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.3/fileformats/extras/medimage/converters.py
+-rw-r--r--   0        0        0     1913 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.3/fileformats/extras/medimage/dicom.py
+-rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.3/fileformats/extras/medimage/diffusion.py
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.3/fileformats/extras/medimage/mrtrix3.py
+-rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.3/fileformats/extras/medimage/nifti.py
+-rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.3/fileformats/extras/medimage/tests/test_neuro_converters.py
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.3/.gitignore
+-rw-r--r--   0        0        0    14222 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.3/LICENSE
+-rw-r--r--   0        0        0     2151 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.3/README.rst
+-rw-r--r--   0        0        0     2232 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0    18991 2020-02-02 00:00:00.000000 fileformats_medimage_extras-0.1.3/PKG-INFO
```

### Comparing `fileformats_medimage_extras-0.1.2/.pre-commit-config.yaml` & `fileformats_medimage_extras-0.1.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `fileformats_medimage_extras-0.1.2/conftest.py` & `fileformats_medimage_extras-0.1.3/conftest.py`

 * *Files identical despite different names*

### Comparing `fileformats_medimage_extras-0.1.2/.github/workflows/publish.yml` & `fileformats_medimage_extras-0.1.3/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `fileformats_medimage_extras-0.1.2/.github/workflows/tests.yml` & `fileformats_medimage_extras-0.1.3/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `fileformats_medimage_extras-0.1.2/fileformats/extras/medimage/converters.py` & `fileformats_medimage_extras-0.1.3/fileformats/extras/medimage/converters.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,18 @@
     NiftiXBvec,
     NiftiBvec,
     NiftiGzBvec,
     NiftiGzXBvec,
 )
 import jq
 import pydra
-from pydra.tasks.mrtrix3.utils import MRConvert
+try:
+    from pydra.tasks.mrtrix3.utils import MRConvert
+except ImportError:
+    from pydra.tasks.mrtrix3.latest import mrconvert as MRConvert
 from pydra.tasks.dcm2niix import Dcm2Niix
 
 
 @mark.converter(source_format=MedicalImage, target_format=Analyze, out_ext=Analyze.ext)
 @mark.converter(
     source_format=MedicalImage, target_format=MrtrixImage, out_ext=MrtrixImage.ext
 )
```

### Comparing `fileformats_medimage_extras-0.1.2/fileformats/extras/medimage/dicom.py` & `fileformats_medimage_extras-0.1.3/fileformats/extras/medimage/dicom.py`

 * *Files identical despite different names*

### Comparing `fileformats_medimage_extras-0.1.2/fileformats/extras/medimage/diffusion.py` & `fileformats_medimage_extras-0.1.3/fileformats/extras/medimage/diffusion.py`

 * *Files identical despite different names*

### Comparing `fileformats_medimage_extras-0.1.2/fileformats/extras/medimage/nifti.py` & `fileformats_medimage_extras-0.1.3/fileformats/extras/medimage/nifti.py`

 * *Files identical despite different names*

### Comparing `fileformats_medimage_extras-0.1.2/fileformats/extras/medimage/tests/test_neuro_converters.py` & `fileformats_medimage_extras-0.1.3/fileformats/extras/medimage/tests/test_neuro_converters.py`

 * *Files identical despite different names*

### Comparing `fileformats_medimage_extras-0.1.2/LICENSE` & `fileformats_medimage_extras-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fileformats_medimage_extras-0.1.2/README.rst` & `fileformats_medimage_extras-0.1.3/README.rst`

 * *Files identical despite different names*

### Comparing `fileformats_medimage_extras-0.1.2/pyproject.toml` & `fileformats_medimage_extras-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fileformats_medimage_extras-0.1.2/PKG-INFO` & `fileformats_medimage_extras-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fileformats-medimage-extras
-Version: 0.1.2
+Version: 0.1.3
 Summary: Classes for representing different file formats in Python classes for use in type hinting in data workflows
 Project-URL: repository, https://github.com/ArcanaFramework/fileformats-medimage-extras
 Author-email: "Thomas G. Close" <tom.g.close@gmail.com>
 Maintainer-email: "Thomas G. Close" <tom.g.close@gmail.com>
 License: Creative Commons Attribution 4.0 International Public License
         By exercising the Licensed Rights (defined below), You accept and agree to be bound by the terms and conditions of this Creative Commons Attribution 4.0 International Public License ("Public License"). To the extent this Public License may be interpreted as a contract, You are granted the Licensed Rights in consideration of Your acceptance of these terms and conditions, and the Licensor grants You such rights in consideration of benefits the Licensor receives from making the Licensed Material available under these terms and conditions.
```

