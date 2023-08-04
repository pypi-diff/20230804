# Comparing `tmp/bioat-0.2.7.tar.gz` & `tmp/bioat-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bioat-0.2.7.tar", max compression
+gzip compressed data, was "bioat-0.2.8.tar", max compression
```

## Comparing `bioat-0.2.7.tar` & `bioat-0.2.8.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0     1080 2022-10-12 10:28:48.000000 bioat-0.2.7/LICENSE
--rw-r--r--   0        0        0      915 2023-05-26 06:22:16.476980 bioat-0.2.7/README.md
--rw-r--r--   0        0        0     1115 2023-08-04 15:03:39.373097 bioat-0.2.7/pyproject.toml
--rw-r--r--   0        0        0      637 2023-06-23 18:19:23.000000 bioat-0.2.7/src/bioat/__init__.py
--rw-r--r--   0        0        0      451 2023-06-17 10:35:36.080629 bioat-0.2.7/src/bioat/__main__.py
--rw-r--r--   0        0        0      508 2023-05-26 06:02:39.222570 bioat-0.2.7/src/bioat/about.py
--rw-r--r--   0        0        0    13916 2023-06-17 12:05:22.520338 bioat-0.2.7/src/bioat/bamtools.py
--rw-r--r--   0        0        0      738 2023-06-17 09:21:50.061008 bioat-0.2.7/src/bioat/bedtools.py
--rw-r--r--   0        0        0     1833 2023-06-17 10:35:16.669568 bioat-0.2.7/src/bioat/cli.py
--rw-r--r--   0        0        0    14545 2023-04-19 14:58:31.765837 bioat-0.2.7/src/bioat/detect_seq.py
--rw-r--r--   0        0        0      151 2023-06-23 18:19:23.000000 bioat-0.2.7/src/bioat/exceptions.py
--rw-r--r--   0        0        0    11024 2023-05-26 05:45:47.350133 bioat-0.2.7/src/bioat/fastxtools.py
--rw-r--r--   0        0        0      818 2023-03-13 04:16:15.365909 bioat-0.2.7/src/bioat/genome.py
--rw-r--r--   0        0        0     5940 2023-06-17 09:21:44.490936 bioat-0.2.7/src/bioat/hictools.py
--rw-r--r--   0        0        0        0 2023-04-01 12:21:31.028419 bioat-0.2.7/src/bioat/lib/__init__.py
--rw-r--r--   0        0        0      854 2023-04-08 13:49:32.058220 bioat-0.2.7/src/bioat/lib/_dev_tools.py
--rw-r--r--   0        0        0     9873 2023-05-11 14:17:36.000000 bioat-0.2.7/src/bioat/lib/circos/example_data_barplot.csv
--rw-r--r--   0        0        0    30782 2023-05-11 14:17:36.000000 bioat-0.2.7/src/bioat/lib/circos/example_data_chromosome_cytoband.csv
--rw-r--r--   0        0        0      427 2023-05-11 14:17:36.000000 bioat-0.2.7/src/bioat/lib/circos/example_data_chromosome_general.csv
--rw-r--r--   0        0        0     5143 2023-05-11 14:17:36.000000 bioat-0.2.7/src/bioat/lib/circos/example_data_links.csv
--rw-r--r--   0        0        0     9856 2023-05-11 14:17:36.000000 bioat-0.2.7/src/bioat/lib/circos/example_data_point.csv
--rw-r--r--   0        0        0     9107 2023-05-11 14:17:36.000000 bioat-0.2.7/src/bioat/lib/circos/example_data_rect_gradual.csv
--rw-r--r--   0        0        0      450 2023-05-11 14:17:36.000000 bioat-0.2.7/src/bioat/lib/circos/hg38/chromosome_length_hg38.csv
--rw-r--r--   0        0        0    31637 2023-05-11 14:17:36.000000 bioat-0.2.7/src/bioat/lib/circos/hg38/cytoBand_hg38.csv
--rw-r--r--   0        0        0     6274 2023-04-13 16:27:56.000000 bioat-0.2.7/src/bioat/lib/libalignment.py
--rw-r--r--   0        0        0    77322 2023-07-27 07:39:03.827893 bioat-0.2.7/src/bioat/lib/libcircos.py
--rw-r--r--   0        0        0     4460 2023-07-14 09:35:07.000000 bioat-0.2.7/src/bioat/lib/libcolor.py
--rw-r--r--   0        0        0     6571 2023-06-17 09:16:08.912240 bioat-0.2.7/src/bioat/lib/libcrispr.py
--rw-r--r--   0        0        0      787 2023-07-07 13:34:23.740347 bioat-0.2.7/src/bioat/lib/libdataclasses.py
--rw-r--r--   0        0        0   155206 2023-04-19 14:58:47.513136 bioat-0.2.7/src/bioat/lib/libdetect_seq.py
--rw-r--r--   0        0        0     1340 2023-08-04 15:02:57.183427 bioat-0.2.7/src/bioat/lib/libpandas.py
--rw-r--r--   0        0        0       42 2023-08-04 14:39:42.964547 bioat-0.2.7/src/bioat/lib/libpath.py
--rw-r--r--   0        0        0     1720 2023-04-25 18:24:40.767945 bioat-0.2.7/src/bioat/lib/libplot.py
--rw-r--r--   0        0        0      509 2023-05-11 14:37:34.152762 bioat-0.2.7/src/bioat/lib/libsnakemake.py
--rw-r--r--   0        0        0     1604 2023-04-17 08:05:06.992591 bioat-0.2.7/src/bioat/logger.py
--rw-r--r--   0        0        0      717 2023-06-17 09:22:39.495970 bioat-0.2.7/src/bioat/mgitools.py
--rw-r--r--   0        0        0     5748 2023-05-26 05:47:35.184115 bioat-0.2.7/src/bioat/systemtools.py
--rw-r--r--   0        0        0     3280 2023-06-17 09:26:06.543411 bioat-0.2.7/src/bioat/tabletools.py
--rw-r--r--   0        0        0    81594 2023-06-23 18:19:23.000000 bioat-0.2.7/src/bioat/target_seq.py
--rw-r--r--   0        0        0      519 2023-08-04 15:03:25.923909 bioat-0.2.7/src/bioat/version.py
--rw-r--r--   0        0        0     2079 1970-01-01 00:00:00.000000 bioat-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0     1080 2022-10-12 10:28:48.000000 bioat-0.2.8/LICENSE
+-rw-r--r--   0        0        0      915 2023-05-26 06:22:16.476980 bioat-0.2.8/README.md
+-rw-r--r--   0        0        0     1135 2023-08-04 15:14:13.409572 bioat-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0      637 2023-06-23 18:19:23.000000 bioat-0.2.8/src/bioat/__init__.py
+-rw-r--r--   0        0        0      451 2023-06-17 10:35:36.080629 bioat-0.2.8/src/bioat/__main__.py
+-rw-r--r--   0        0        0      508 2023-05-26 06:02:39.222570 bioat-0.2.8/src/bioat/about.py
+-rw-r--r--   0        0        0    13916 2023-06-17 12:05:22.520338 bioat-0.2.8/src/bioat/bamtools.py
+-rw-r--r--   0        0        0      738 2023-06-17 09:21:50.061008 bioat-0.2.8/src/bioat/bedtools.py
+-rw-r--r--   0        0        0     1833 2023-06-17 10:35:16.669568 bioat-0.2.8/src/bioat/cli.py
+-rw-r--r--   0        0        0    14545 2023-04-19 14:58:31.765837 bioat-0.2.8/src/bioat/detect_seq.py
+-rw-r--r--   0        0        0      151 2023-06-23 18:19:23.000000 bioat-0.2.8/src/bioat/exceptions.py
+-rw-r--r--   0        0        0    11024 2023-05-26 05:45:47.350133 bioat-0.2.8/src/bioat/fastxtools.py
+-rw-r--r--   0        0        0      818 2023-03-13 04:16:15.365909 bioat-0.2.8/src/bioat/genome.py
+-rw-r--r--   0        0        0     5940 2023-06-17 09:21:44.490936 bioat-0.2.8/src/bioat/hictools.py
+-rw-r--r--   0        0        0        0 2023-04-01 12:21:31.028419 bioat-0.2.8/src/bioat/lib/__init__.py
+-rw-r--r--   0        0        0      854 2023-04-08 13:49:32.058220 bioat-0.2.8/src/bioat/lib/_dev_tools.py
+-rw-r--r--   0        0        0     9873 2023-05-11 14:17:36.000000 bioat-0.2.8/src/bioat/lib/circos/example_data_barplot.csv
+-rw-r--r--   0        0        0    30782 2023-05-11 14:17:36.000000 bioat-0.2.8/src/bioat/lib/circos/example_data_chromosome_cytoband.csv
+-rw-r--r--   0        0        0      427 2023-05-11 14:17:36.000000 bioat-0.2.8/src/bioat/lib/circos/example_data_chromosome_general.csv
+-rw-r--r--   0        0        0     5143 2023-05-11 14:17:36.000000 bioat-0.2.8/src/bioat/lib/circos/example_data_links.csv
+-rw-r--r--   0        0        0     9856 2023-05-11 14:17:36.000000 bioat-0.2.8/src/bioat/lib/circos/example_data_point.csv
+-rw-r--r--   0        0        0     9107 2023-05-11 14:17:36.000000 bioat-0.2.8/src/bioat/lib/circos/example_data_rect_gradual.csv
+-rw-r--r--   0        0        0      450 2023-05-11 14:17:36.000000 bioat-0.2.8/src/bioat/lib/circos/hg38/chromosome_length_hg38.csv
+-rw-r--r--   0        0        0    31637 2023-05-11 14:17:36.000000 bioat-0.2.8/src/bioat/lib/circos/hg38/cytoBand_hg38.csv
+-rw-r--r--   0        0        0     6274 2023-04-13 16:27:56.000000 bioat-0.2.8/src/bioat/lib/libalignment.py
+-rw-r--r--   0        0        0    77322 2023-07-27 07:39:03.827893 bioat-0.2.8/src/bioat/lib/libcircos.py
+-rw-r--r--   0        0        0     4460 2023-07-14 09:35:07.000000 bioat-0.2.8/src/bioat/lib/libcolor.py
+-rw-r--r--   0        0        0     6571 2023-06-17 09:16:08.912240 bioat-0.2.8/src/bioat/lib/libcrispr.py
+-rw-r--r--   0        0        0      787 2023-07-07 13:34:23.740347 bioat-0.2.8/src/bioat/lib/libdataclasses.py
+-rw-r--r--   0        0        0   155206 2023-04-19 14:58:47.513136 bioat-0.2.8/src/bioat/lib/libdetect_seq.py
+-rw-r--r--   0        0        0     1369 2023-08-04 15:10:16.572271 bioat-0.2.8/src/bioat/lib/libpandas.py
+-rw-r--r--   0        0        0       42 2023-08-04 14:39:42.964547 bioat-0.2.8/src/bioat/lib/libpath.py
+-rw-r--r--   0        0        0     1720 2023-04-25 18:24:40.767945 bioat-0.2.8/src/bioat/lib/libplot.py
+-rw-r--r--   0        0        0      509 2023-05-11 14:37:34.152762 bioat-0.2.8/src/bioat/lib/libsnakemake.py
+-rw-r--r--   0        0        0     1604 2023-04-17 08:05:06.992591 bioat-0.2.8/src/bioat/logger.py
+-rw-r--r--   0        0        0      717 2023-06-17 09:22:39.495970 bioat-0.2.8/src/bioat/mgitools.py
+-rw-r--r--   0        0        0     5748 2023-05-26 05:47:35.184115 bioat-0.2.8/src/bioat/systemtools.py
+-rw-r--r--   0        0        0     3280 2023-06-17 09:26:06.543411 bioat-0.2.8/src/bioat/tabletools.py
+-rw-r--r--   0        0        0    81594 2023-06-23 18:19:23.000000 bioat-0.2.8/src/bioat/target_seq.py
+-rw-r--r--   0        0        0      519 2023-08-04 15:13:40.478272 bioat-0.2.8/src/bioat/version.py
+-rw-r--r--   0        0        0     2070 1970-01-01 00:00:00.000000 bioat-0.2.8/PKG-INFO
```

### Comparing `bioat-0.2.7/LICENSE` & `bioat-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `bioat-0.2.7/README.md` & `bioat-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `bioat-0.2.7/pyproject.toml` & `bioat-0.2.8/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 [tool.poetry]
 name = "bioat"
-version = "0.2.7"
+version = "0.2.8"
 description = "Bioinformatic toolkit with python (It's still under development!)"
 license = "MIT"
 authors = ["Herman Zhao <hermanzhaozzzz@gmail.com>"]
 repository = "https://github.com/hermanzhaozzzz/BioinformaticAnalysisTools"
 homepage = "https://github.com/hermanzhaozzzz/BioinformaticAnalysisTools"
 # README file(s) are used as the package description
 readme = "README.md"
 
 
 [tool.poetry.dependencies]
 # Compatible Python versions
-python = ">=3.8.0,<3.11"
+python = ">=3.9.0,<3.11"
 pandas = "^1.5.3"
 numpy = "^1.24.1"
 tqdm = "^4.64.1"
 fire = "^0.5.0"
 cython = "^0.29.33"
 pysam = "^0.20.0"
 biopython = "^1.80"
 pandarallel = "^1.6.4"
 matplotlib = "^3.7.1"
 tabulate = "^0.9.0"
 scipy = "^1.8.0"
 statsmodels = "^0.13.5"
+ipython = "^8.14.0"
 
 [tool.poetry.scripts]
 bioat = "bioat.__main__:main"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.1.3"
 pytest-cov = "^3.0"
```

### Comparing `bioat-0.2.7/src/bioat/__init__.py` & `bioat-0.2.8/src/bioat/__init__.py`

 * *Files identical despite different names*

### Comparing `bioat-0.2.7/src/bioat/bamtools.py` & `bioat-0.2.8/src/bioat/bamtools.py`

 * *Files identical despite different names*

### Comparing `bioat-0.2.7/src/bioat/bedtools.py` & `bioat-0.2.8/src/bioat/bedtools.py`

 * *Files identical despite different names*

### Comparing `bioat-0.2.7/src/bioat/cli.py` & `bioat-0.2.8/src/bioat/cli.py`

 * *Files identical despite different names*

### Comparing `bioat-0.2.7/src/bioat/detect_seq.py` & `bioat-0.2.8/src/bioat/detect_seq.py`

 * *Files identical despite different names*

### Comparing `bioat-0.2.7/src/bioat/fastxtools.py` & `bioat-0.2.8/src/bioat/fastxtools.py`

 * *Files identical despite different names*

### Comparing `bioat-0.2.7/src/bioat/genome.py` & `bioat-0.2.8/src/bioat/genome.py`

 * *Files identical despite different names*

### Comparing `bioat-0.2.7/src/bioat/hictools.py` & `bioat-0.2.8/src/bioat/hictools.py`

 * *Files identical despite different names*

### Comparing `bioat-0.2.7/src/bioat/lib/_dev_tools.py` & `bioat-0.2.8/src/bioat/lib/_dev_tools.py`

 * *Files identical despite different names*

### Comparing `bioat-0.2.7/src/bioat/lib/circos/example_data_barplot.csv` & `bioat-0.2.8/src/bioat/lib/circos/example_data_barplot.csv`

 * *Files identical despite different names*

### Comparing `bioat-0.2.7/src/bioat/lib/circos/example_data_chromosome_cytoband.csv` & `bioat-0.2.8/src/bioat/lib/circos/example_data_chromosome_cytoband.csv`

 * *Files identical despite different names*

### Comparing `bioat-0.2.7/src/bioat/lib/circos/example_data_links.csv` & `bioat-0.2.8/src/bioat/lib/circos/example_data_links.csv`

 * *Files identical despite different names*

### Comparing `bioat-0.2.7/src/bioat/lib/circos/example_data_point.csv` & `bioat-0.2.8/src/bioat/lib/circos/example_data_point.csv`

 * *Files identical despite different names*

### Comparing `bioat-0.2.7/src/bioat/lib/circos/example_data_rect_gradual.csv` & `bioat-0.2.8/src/bioat/lib/circos/example_data_rect_gradual.csv`

 * *Files identical despite different names*

### Comparing `bioat-0.2.7/src/bioat/lib/circos/hg38/cytoBand_hg38.csv` & `bioat-0.2.8/src/bioat/lib/circos/hg38/cytoBand_hg38.csv`

 * *Files identical despite different names*

### Comparing `bioat-0.2.7/src/bioat/lib/libalignment.py` & `bioat-0.2.8/src/bioat/lib/libalignment.py`

 * *Files identical despite different names*

### Comparing `bioat-0.2.7/src/bioat/lib/libcircos.py` & `bioat-0.2.8/src/bioat/lib/libcircos.py`

 * *Files identical despite different names*

### Comparing `bioat-0.2.7/src/bioat/lib/libcolor.py` & `bioat-0.2.8/src/bioat/lib/libcolor.py`

 * *Files identical despite different names*

### Comparing `bioat-0.2.7/src/bioat/lib/libcrispr.py` & `bioat-0.2.8/src/bioat/lib/libcrispr.py`

 * *Files identical despite different names*

### Comparing `bioat-0.2.7/src/bioat/lib/libdataclasses.py` & `bioat-0.2.8/src/bioat/lib/libdataclasses.py`

 * *Files identical despite different names*

### Comparing `bioat-0.2.7/src/bioat/lib/libdetect_seq.py` & `bioat-0.2.8/src/bioat/lib/libdetect_seq.py`

 * *Files identical despite different names*

### Comparing `bioat-0.2.7/src/bioat/lib/libpandas.py` & `bioat-0.2.8/src/bioat/lib/libpandas.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from __future__ import absolute_import
 import pandas as pd
 import logging
 import sys
 from bioat.logger import set_logging_level
 
+__all__ = ['set_option']
+
 
 def set_option(max_colwidth: int = 40, display_width: int = 120, display_max_columns: int = None,
-               display_max_rows: int = 50, log_level: str='INFO',**kwargs):
+               display_max_rows: int = 50, log_level: str = 'INFO', **kwargs):
     # set logger
     if log_level in ['CRITICAL', 'ERROR', 'WARNING', 'INFO', 'DEBUG', 'NOTSET']:
         set_logging_level(level=log_level)
     else:
         raise KeyError("log_level must be element in ['CRITICAL', 'ERROR', 'WARNING', 'INFO', 'DEBUG', 'NOTSET']")
 
     lib_name = __name__
```

### Comparing `bioat-0.2.7/src/bioat/lib/libplot.py` & `bioat-0.2.8/src/bioat/lib/libplot.py`

 * *Files identical despite different names*

### Comparing `bioat-0.2.7/src/bioat/logger.py` & `bioat-0.2.8/src/bioat/logger.py`

 * *Files identical despite different names*

### Comparing `bioat-0.2.7/src/bioat/mgitools.py` & `bioat-0.2.8/src/bioat/mgitools.py`

 * *Files identical despite different names*

### Comparing `bioat-0.2.7/src/bioat/systemtools.py` & `bioat-0.2.8/src/bioat/systemtools.py`

 * *Files identical despite different names*

### Comparing `bioat-0.2.7/src/bioat/tabletools.py` & `bioat-0.2.8/src/bioat/tabletools.py`

 * *Files identical despite different names*

### Comparing `bioat-0.2.7/src/bioat/target_seq.py` & `bioat-0.2.8/src/bioat/target_seq.py`

 * *Files identical despite different names*

### Comparing `bioat-0.2.7/src/bioat/version.py` & `bioat-0.2.8/src/bioat/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,14 @@
 import bioat
 import datetime
 import os
 
 project_toml: str = os.path.join(bioat.__path__[0], 'version.py')
 sec = os.path.getmtime(project_toml)
 __upgrade_date__ = datetime.date.fromtimestamp(sec)
-__version__ = "0.2.7"
+__version__ = "0.2.8"
 
 __author__ = 'Hua-nan ZHAO @ Tsinghua University'
 __email__ = 'hermanzhaozzzz@gmail.com'
 __doc_format__ = "restructuredtext"
 __doc_address__ = "https://github.com/hermanzhaozzzz/bioat/tree/master/docs"
 __repo_address__ = "https://github.com/hermanzhaozzzz/bioat"
```

### Comparing `bioat-0.2.7/PKG-INFO` & `bioat-0.2.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: bioat
-Version: 0.2.7
+Version: 0.2.8
 Summary: Bioinformatic toolkit with python (It's still under development!)
 Home-page: https://github.com/hermanzhaozzzz/BioinformaticAnalysisTools
 License: MIT
 Author: Herman Zhao
 Author-email: hermanzhaozzzz@gmail.com
-Requires-Python: >=3.8.0,<3.11
+Requires-Python: >=3.9.0,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: biopython (>=1.80,<2.0)
 Requires-Dist: cython (>=0.29.33,<0.30.0)
 Requires-Dist: fire (>=0.5.0,<0.6.0)
+Requires-Dist: ipython (>=8.14.0,<9.0.0)
 Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
 Requires-Dist: numpy (>=1.24.1,<2.0.0)
 Requires-Dist: pandarallel (>=1.6.4,<2.0.0)
 Requires-Dist: pandas (>=1.5.3,<2.0.0)
 Requires-Dist: pysam (>=0.20.0,<0.21.0)
 Requires-Dist: scipy (>=1.8.0,<2.0.0)
 Requires-Dist: statsmodels (>=0.13.5,<0.14.0)
```

