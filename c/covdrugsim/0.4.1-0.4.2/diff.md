# Comparing `tmp/covdrugsim-0.4.1.tar.gz` & `tmp/covdrugsim-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "covdrugsim-0.4.1.tar", max compression
+gzip compressed data, was "covdrugsim-0.4.2.tar", max compression
```

## Comparing `covdrugsim-0.4.1.tar` & `covdrugsim-0.4.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0     1082 2023-07-08 09:40:33.598644 covdrugsim-0.4.1/LICENSE
--rw-r--r--   0        0        0     6588 2023-07-08 09:40:33.598644 covdrugsim-0.4.1/README.md
--rw-r--r--   0        0        0     1956 2023-07-08 09:41:19.290949 covdrugsim-0.4.1/pyproject.toml
--rw-r--r--   0        0        0      733 2023-07-08 09:41:19.290949 covdrugsim-0.4.1/setup.py
--rw-r--r--   0        0        0     1410 2023-07-08 09:40:33.602644 covdrugsim-0.4.1/src/covdrugsim/__init__.py
--rw-r--r--   0        0        0        0 2023-07-08 09:40:33.602644 covdrugsim-0.4.1/src/covdrugsim/data/__init__.py
--rw-r--r--   0        0        0      170 2023-07-08 09:40:33.602644 covdrugsim-0.4.1/src/covdrugsim/data/chargesExample.txt
--rw-r--r--   0        0        0     4449 2023-07-08 09:40:33.602644 covdrugsim-0.4.1/src/covdrugsim/data/energyLevellerExample.inp
--rw-r--r--   0        0        0   592600 2023-07-08 09:40:33.606644 covdrugsim-0.4.1/src/covdrugsim/data/exampleGaussianOutputs/example1.out
--rw-r--r--   0        0        0   565812 2023-07-08 09:40:33.606644 covdrugsim-0.4.1/src/covdrugsim/data/exampleGaussianOutputs/example2.out
--rw-r--r--   0        0        0  1069703 2023-07-08 09:40:33.614644 covdrugsim-0.4.1/src/covdrugsim/data/exampleGaussianOutputs/example3.out
--rw-r--r--   0        0        0      984 2023-07-08 09:40:33.614644 covdrugsim-0.4.1/src/covdrugsim/data/exampleXYZs/example1.xyz
--rw-r--r--   0        0        0      739 2023-07-08 09:40:33.614644 covdrugsim-0.4.1/src/covdrugsim/data/exampleXYZs/example2.xyz
--rw-r--r--   0        0        0     1327 2023-07-08 09:40:33.614644 covdrugsim-0.4.1/src/covdrugsim/data/exampleXYZs/example3.xyz
--rw-r--r--   0        0        0      866 2023-07-08 09:40:33.614644 covdrugsim-0.4.1/src/covdrugsim/datasets.py
--rw-r--r--   0        0        0      241 2023-07-08 09:40:33.614644 covdrugsim-0.4.1/src/covdrugsim/main.py
--rw-r--r--   0        0        0     3839 2023-07-08 09:40:33.614644 covdrugsim-0.4.1/src/covdrugsim/mdsim/SCbondDist.py
--rw-r--r--   0        0        0        0 2023-07-08 09:40:33.614644 covdrugsim-0.4.1/src/covdrugsim/mdsim/__init__.py
--rw-r--r--   0        0        0     8141 2023-07-08 09:40:33.614644 covdrugsim-0.4.1/src/covdrugsim/mdsim/baseID.py
--rw-r--r--   0        0        0     6071 2023-07-08 09:40:33.614644 covdrugsim-0.4.1/src/covdrugsim/mdsim/bbRMSD.py
--rw-r--r--   0        0        0      331 2023-07-08 09:40:33.614644 covdrugsim-0.4.1/src/covdrugsim/mdsim/config.py
--rw-r--r--   0        0        0     3084 2023-07-08 09:40:33.614644 covdrugsim-0.4.1/src/covdrugsim/mdsim/hbondAnalysis.py
--rw-r--r--   0        0        0     3917 2023-07-08 09:40:33.614644 covdrugsim-0.4.1/src/covdrugsim/mdsim/ligDihedral.py
--rw-r--r--   0        0        0      769 2023-07-08 09:40:33.614644 covdrugsim-0.4.1/src/covdrugsim/mdsim/mdAnalyse.py
--rw-r--r--   0        0        0     5644 2023-07-08 09:40:33.614644 covdrugsim-0.4.1/src/covdrugsim/mdsim/prepMTB.py
--rw-r--r--   0        0        0        0 2023-07-08 09:40:33.614644 covdrugsim-0.4.1/src/covdrugsim/qmcalc/__init__.py
--rw-r--r--   0        0        0     2525 2023-07-08 09:40:33.614644 covdrugsim-0.4.1/src/covdrugsim/qmcalc/admin.py
--rw-r--r--   0        0        0     1313 2023-07-08 09:40:33.614644 covdrugsim-0.4.1/src/covdrugsim/qmcalc/constants.py
--rw-r--r--   0        0        0    10364 2023-07-08 09:40:33.614644 covdrugsim-0.4.1/src/covdrugsim/qmcalc/genScripts.py
--rw-r--r--   0        0        0     1605 2023-07-08 09:40:33.614644 covdrugsim-0.4.1/src/covdrugsim/qmcalc/gsub.sh
--rw-r--r--   0        0        0     4958 2023-07-08 09:40:33.614644 covdrugsim-0.4.1/src/covdrugsim/qmcalc/tabulate.py
--rw-r--r--   0        0        0     4280 2023-07-08 09:40:33.614644 covdrugsim-0.4.1/src/covdrugsim/qmcalc/unitConv.py
--rw-r--r--   0        0        0        0 2023-07-08 09:40:33.614644 covdrugsim-0.4.1/src/covdrugsim/qmcalc/visAnalysis/__init__.py
--rw-r--r--   0        0        0    17951 2023-07-08 09:40:33.614644 covdrugsim-0.4.1/src/covdrugsim/qmcalc/visAnalysis/energyLeveller.py
--rw-r--r--   0        0        0    11782 2023-07-08 09:40:33.614644 covdrugsim-0.4.1/src/covdrugsim/qmcalc/visAnalysis/plotConfig.py
--rw-r--r--   0        0        0    13749 2023-07-08 09:40:33.614644 covdrugsim-0.4.1/src/covdrugsim/qmcalc/visAnalysis/plotFigs.py
--rw-r--r--   0        0        0     3882 2023-07-08 09:40:33.614644 covdrugsim-0.4.1/tests/test_covdrugsim.py
--rw-r--r--   0        0        0     7725 1970-01-01 00:00:00.000000 covdrugsim-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-08-04 10:07:01.696871 covdrugsim-0.4.2/LICENSE
+-rw-r--r--   0        0        0     6588 2023-08-04 10:07:01.696871 covdrugsim-0.4.2/README.md
+-rw-r--r--   0        0        0     1956 2023-08-04 10:07:41.388705 covdrugsim-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0      733 2023-08-04 10:07:41.388705 covdrugsim-0.4.2/setup.py
+-rw-r--r--   0        0        0     1410 2023-08-04 10:07:01.700871 covdrugsim-0.4.2/src/covdrugsim/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-04 10:07:01.700871 covdrugsim-0.4.2/src/covdrugsim/data/__init__.py
+-rw-r--r--   0        0        0      170 2023-08-04 10:07:01.700871 covdrugsim-0.4.2/src/covdrugsim/data/chargesExample.txt
+-rw-r--r--   0        0        0     4449 2023-08-04 10:07:01.700871 covdrugsim-0.4.2/src/covdrugsim/data/energyLevellerExample.inp
+-rw-r--r--   0        0        0   592600 2023-08-04 10:07:01.704871 covdrugsim-0.4.2/src/covdrugsim/data/exampleGaussianOutputs/example1.out
+-rw-r--r--   0        0        0   565812 2023-08-04 10:07:01.704871 covdrugsim-0.4.2/src/covdrugsim/data/exampleGaussianOutputs/example2.out
+-rw-r--r--   0        0        0  1069703 2023-08-04 10:07:01.708871 covdrugsim-0.4.2/src/covdrugsim/data/exampleGaussianOutputs/example3.out
+-rw-r--r--   0        0        0      984 2023-08-04 10:07:01.708871 covdrugsim-0.4.2/src/covdrugsim/data/exampleXYZs/example1.xyz
+-rw-r--r--   0        0        0      739 2023-08-04 10:07:01.708871 covdrugsim-0.4.2/src/covdrugsim/data/exampleXYZs/example2.xyz
+-rw-r--r--   0        0        0     1327 2023-08-04 10:07:01.712871 covdrugsim-0.4.2/src/covdrugsim/data/exampleXYZs/example3.xyz
+-rw-r--r--   0        0        0      866 2023-08-04 10:07:01.712871 covdrugsim-0.4.2/src/covdrugsim/datasets.py
+-rw-r--r--   0        0        0      241 2023-08-04 10:07:01.712871 covdrugsim-0.4.2/src/covdrugsim/main.py
+-rw-r--r--   0        0        0     3839 2023-08-04 10:07:01.712871 covdrugsim-0.4.2/src/covdrugsim/mdsim/SCbondDist.py
+-rw-r--r--   0        0        0        0 2023-08-04 10:07:01.712871 covdrugsim-0.4.2/src/covdrugsim/mdsim/__init__.py
+-rw-r--r--   0        0        0     8141 2023-08-04 10:07:01.712871 covdrugsim-0.4.2/src/covdrugsim/mdsim/baseID.py
+-rw-r--r--   0        0        0     6071 2023-08-04 10:07:01.712871 covdrugsim-0.4.2/src/covdrugsim/mdsim/bbRMSD.py
+-rw-r--r--   0        0        0      331 2023-08-04 10:07:01.712871 covdrugsim-0.4.2/src/covdrugsim/mdsim/config.py
+-rw-r--r--   0        0        0     3084 2023-08-04 10:07:01.712871 covdrugsim-0.4.2/src/covdrugsim/mdsim/hbondAnalysis.py
+-rw-r--r--   0        0        0     3917 2023-08-04 10:07:01.712871 covdrugsim-0.4.2/src/covdrugsim/mdsim/ligDihedral.py
+-rw-r--r--   0        0        0      769 2023-08-04 10:07:01.712871 covdrugsim-0.4.2/src/covdrugsim/mdsim/mdAnalyse.py
+-rw-r--r--   0        0        0     5644 2023-08-04 10:07:01.712871 covdrugsim-0.4.2/src/covdrugsim/mdsim/prepMTB.py
+-rw-r--r--   0        0        0        0 2023-08-04 10:07:01.712871 covdrugsim-0.4.2/src/covdrugsim/qmcalc/__init__.py
+-rw-r--r--   0        0        0     2525 2023-08-04 10:07:01.712871 covdrugsim-0.4.2/src/covdrugsim/qmcalc/admin.py
+-rw-r--r--   0        0        0     1313 2023-08-04 10:07:01.712871 covdrugsim-0.4.2/src/covdrugsim/qmcalc/constants.py
+-rw-r--r--   0        0        0    10364 2023-08-04 10:07:01.712871 covdrugsim-0.4.2/src/covdrugsim/qmcalc/genScripts.py
+-rw-r--r--   0        0        0     1605 2023-08-04 10:07:01.712871 covdrugsim-0.4.2/src/covdrugsim/qmcalc/gsub.sh
+-rw-r--r--   0        0        0     4958 2023-08-04 10:07:01.712871 covdrugsim-0.4.2/src/covdrugsim/qmcalc/tabulate.py
+-rw-r--r--   0        0        0     4280 2023-08-04 10:07:01.712871 covdrugsim-0.4.2/src/covdrugsim/qmcalc/unitConv.py
+-rw-r--r--   0        0        0        0 2023-08-04 10:07:01.712871 covdrugsim-0.4.2/src/covdrugsim/qmcalc/visAnalysis/__init__.py
+-rw-r--r--   0        0        0    17951 2023-08-04 10:07:01.712871 covdrugsim-0.4.2/src/covdrugsim/qmcalc/visAnalysis/energyLeveller.py
+-rw-r--r--   0        0        0    11782 2023-08-04 10:07:01.712871 covdrugsim-0.4.2/src/covdrugsim/qmcalc/visAnalysis/plotConfig.py
+-rw-r--r--   0        0        0    13749 2023-08-04 10:07:01.712871 covdrugsim-0.4.2/src/covdrugsim/qmcalc/visAnalysis/plotFigs.py
+-rw-r--r--   0        0        0     3882 2023-08-04 10:07:01.712871 covdrugsim-0.4.2/tests/test_covdrugsim.py
+-rw-r--r--   0        0        0     7725 1970-01-01 00:00:00.000000 covdrugsim-0.4.2/PKG-INFO
```

### Comparing `covdrugsim-0.4.1/LICENSE` & `covdrugsim-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `covdrugsim-0.4.1/README.md` & `covdrugsim-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `covdrugsim-0.4.1/pyproject.toml` & `covdrugsim-0.4.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "covdrugsim"
-version = "0.4.1"
+version = "0.4.2"
 description = "Package to automate quantum mechanical calculations and molecular dynamics simulations of covalent drugs."
 authors = ["Jonathan Yik Chang Ting <jonting97@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/Jon-Ting/covdrugsim"
 repository = "https://github.com/Jon-Ting/covdrugsim"
 documentation = "https://covdrugsim.readthedocs.io/en/latest/"
```

### Comparing `covdrugsim-0.4.1/setup.py` & `covdrugsim-0.4.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import setuptools
 
 
-__version__ = '0.4.1'
+__version__ = '0.4.2'
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="covdrugsim",
     version=__version__,
     author="Jonathan Yik Chang Ting",
```

### Comparing `covdrugsim-0.4.1/src/covdrugsim/__init__.py` & `covdrugsim-0.4.2/src/covdrugsim/__init__.py`

 * *Files identical despite different names*

### Comparing `covdrugsim-0.4.1/src/covdrugsim/data/energyLevellerExample.inp` & `covdrugsim-0.4.2/src/covdrugsim/data/energyLevellerExample.inp`

 * *Files identical despite different names*

### Comparing `covdrugsim-0.4.1/src/covdrugsim/data/exampleGaussianOutputs/example1.out` & `covdrugsim-0.4.2/src/covdrugsim/data/exampleGaussianOutputs/example1.out`

 * *Files identical despite different names*

### Comparing `covdrugsim-0.4.1/src/covdrugsim/data/exampleGaussianOutputs/example2.out` & `covdrugsim-0.4.2/src/covdrugsim/data/exampleGaussianOutputs/example2.out`

 * *Files identical despite different names*

### Comparing `covdrugsim-0.4.1/src/covdrugsim/data/exampleGaussianOutputs/example3.out` & `covdrugsim-0.4.2/src/covdrugsim/data/exampleGaussianOutputs/example3.out`

 * *Files identical despite different names*

### Comparing `covdrugsim-0.4.1/src/covdrugsim/data/exampleXYZs/example1.xyz` & `covdrugsim-0.4.2/src/covdrugsim/data/exampleXYZs/example1.xyz`

 * *Files identical despite different names*

### Comparing `covdrugsim-0.4.1/src/covdrugsim/data/exampleXYZs/example2.xyz` & `covdrugsim-0.4.2/src/covdrugsim/data/exampleXYZs/example2.xyz`

 * *Files identical despite different names*

### Comparing `covdrugsim-0.4.1/src/covdrugsim/data/exampleXYZs/example3.xyz` & `covdrugsim-0.4.2/src/covdrugsim/data/exampleXYZs/example3.xyz`

 * *Files identical despite different names*

### Comparing `covdrugsim-0.4.1/src/covdrugsim/datasets.py` & `covdrugsim-0.4.2/src/covdrugsim/datasets.py`

 * *Files identical despite different names*

### Comparing `covdrugsim-0.4.1/src/covdrugsim/mdsim/SCbondDist.py` & `covdrugsim-0.4.2/src/covdrugsim/mdsim/SCbondDist.py`

 * *Files identical despite different names*

### Comparing `covdrugsim-0.4.1/src/covdrugsim/mdsim/baseID.py` & `covdrugsim-0.4.2/src/covdrugsim/mdsim/baseID.py`

 * *Files identical despite different names*

### Comparing `covdrugsim-0.4.1/src/covdrugsim/mdsim/bbRMSD.py` & `covdrugsim-0.4.2/src/covdrugsim/mdsim/bbRMSD.py`

 * *Files identical despite different names*

### Comparing `covdrugsim-0.4.1/src/covdrugsim/mdsim/hbondAnalysis.py` & `covdrugsim-0.4.2/src/covdrugsim/mdsim/hbondAnalysis.py`

 * *Files identical despite different names*

### Comparing `covdrugsim-0.4.1/src/covdrugsim/mdsim/ligDihedral.py` & `covdrugsim-0.4.2/src/covdrugsim/mdsim/ligDihedral.py`

 * *Files identical despite different names*

### Comparing `covdrugsim-0.4.1/src/covdrugsim/mdsim/mdAnalyse.py` & `covdrugsim-0.4.2/src/covdrugsim/mdsim/mdAnalyse.py`

 * *Files identical despite different names*

### Comparing `covdrugsim-0.4.1/src/covdrugsim/mdsim/prepMTB.py` & `covdrugsim-0.4.2/src/covdrugsim/mdsim/prepMTB.py`

 * *Files identical despite different names*

### Comparing `covdrugsim-0.4.1/src/covdrugsim/qmcalc/admin.py` & `covdrugsim-0.4.2/src/covdrugsim/qmcalc/admin.py`

 * *Files identical despite different names*

### Comparing `covdrugsim-0.4.1/src/covdrugsim/qmcalc/constants.py` & `covdrugsim-0.4.2/src/covdrugsim/qmcalc/constants.py`

 * *Files identical despite different names*

### Comparing `covdrugsim-0.4.1/src/covdrugsim/qmcalc/genScripts.py` & `covdrugsim-0.4.2/src/covdrugsim/qmcalc/genScripts.py`

 * *Files identical despite different names*

### Comparing `covdrugsim-0.4.1/src/covdrugsim/qmcalc/gsub.sh` & `covdrugsim-0.4.2/src/covdrugsim/qmcalc/gsub.sh`

 * *Files identical despite different names*

### Comparing `covdrugsim-0.4.1/src/covdrugsim/qmcalc/tabulate.py` & `covdrugsim-0.4.2/src/covdrugsim/qmcalc/tabulate.py`

 * *Files identical despite different names*

### Comparing `covdrugsim-0.4.1/src/covdrugsim/qmcalc/unitConv.py` & `covdrugsim-0.4.2/src/covdrugsim/qmcalc/unitConv.py`

 * *Files identical despite different names*

### Comparing `covdrugsim-0.4.1/src/covdrugsim/qmcalc/visAnalysis/energyLeveller.py` & `covdrugsim-0.4.2/src/covdrugsim/qmcalc/visAnalysis/energyLeveller.py`

 * *Files identical despite different names*

### Comparing `covdrugsim-0.4.1/src/covdrugsim/qmcalc/visAnalysis/plotConfig.py` & `covdrugsim-0.4.2/src/covdrugsim/qmcalc/visAnalysis/plotConfig.py`

 * *Files identical despite different names*

### Comparing `covdrugsim-0.4.1/src/covdrugsim/qmcalc/visAnalysis/plotFigs.py` & `covdrugsim-0.4.2/src/covdrugsim/qmcalc/visAnalysis/plotFigs.py`

 * *Files identical despite different names*

### Comparing `covdrugsim-0.4.1/tests/test_covdrugsim.py` & `covdrugsim-0.4.2/tests/test_covdrugsim.py`

 * *Files identical despite different names*

### Comparing `covdrugsim-0.4.1/PKG-INFO` & `covdrugsim-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: covdrugsim
-Version: 0.4.1
+Version: 0.4.2
 Summary: Package to automate quantum mechanical calculations and molecular dynamics simulations of covalent drugs.
 Home-page: https://github.com/Jon-Ting/covdrugsim
 License: MIT
 Keywords: covalent,drug,quantum,mechanic,molecular,dynamics,simulation
 Author: Jonathan Yik Chang Ting
 Author-email: jonting97@gmail.com
 Requires-Python: >=3.9
```

