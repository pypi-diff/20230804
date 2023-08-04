# Comparing `tmp/easybioinfo-0.3.0.tar.gz` & `tmp/easybioinfo-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easybioinfo-0.3.0.tar", last modified: Wed Aug  2 10:10:31 2023, max compression
+gzip compressed data, was "easybioinfo-0.3.1.tar", last modified: Fri Aug  4 19:39:32 2023, max compression
```

## Comparing `easybioinfo-0.3.0.tar` & `easybioinfo-0.3.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-08-02 10:10:31.047585 easybioinfo-0.3.0/
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     1071 2021-11-16 15:00:00.000000 easybioinfo-0.3.0/LICENSE
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      700 2023-08-02 10:10:31.047585 easybioinfo-0.3.0/PKG-INFO
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      241 2021-11-16 15:00:02.000000 easybioinfo-0.3.0/README.md
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      104 2021-11-16 15:00:02.000000 easybioinfo-0.3.0/pyproject.toml
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      681 2023-08-02 10:10:31.047585 easybioinfo-0.3.0/setup.cfg
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       69 2021-11-16 15:00:00.000000 easybioinfo-0.3.0/setup.py
-drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-08-02 10:10:31.043585 easybioinfo-0.3.0/src/
-drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-08-02 10:10:31.047585 easybioinfo-0.3.0/src/easybioinfo/
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       26 2021-11-16 15:00:02.000000 easybioinfo-0.3.0/src/easybioinfo/__init__.py
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)    24679 2023-08-02 10:07:47.000000 easybioinfo-0.3.0/src/easybioinfo/sequences.py
-drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-08-02 10:10:31.047585 easybioinfo-0.3.0/src/easybioinfo.egg-info/
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      700 2023-08-02 10:10:31.000000 easybioinfo-0.3.0/src/easybioinfo.egg-info/PKG-INFO
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      264 2023-08-02 10:10:31.000000 easybioinfo-0.3.0/src/easybioinfo.egg-info/SOURCES.txt
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)        1 2023-08-02 10:10:31.000000 easybioinfo-0.3.0/src/easybioinfo.egg-info/dependency_links.txt
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       12 2023-08-02 10:10:31.000000 easybioinfo-0.3.0/src/easybioinfo.egg-info/top_level.txt
+drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-08-04 19:39:32.645097 easybioinfo-0.3.1/
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     1071 2021-11-16 15:00:00.000000 easybioinfo-0.3.1/LICENSE
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      700 2023-08-04 19:39:32.645097 easybioinfo-0.3.1/PKG-INFO
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      241 2021-11-16 15:00:02.000000 easybioinfo-0.3.1/README.md
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      104 2021-11-16 15:00:02.000000 easybioinfo-0.3.1/pyproject.toml
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      681 2023-08-04 19:39:32.645097 easybioinfo-0.3.1/setup.cfg
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       69 2021-11-16 15:00:00.000000 easybioinfo-0.3.1/setup.py
+drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-08-04 19:39:32.641097 easybioinfo-0.3.1/src/
+drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-08-04 19:39:32.645097 easybioinfo-0.3.1/src/easybioinfo/
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       26 2021-11-16 15:00:02.000000 easybioinfo-0.3.1/src/easybioinfo/__init__.py
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)    24706 2023-08-04 19:38:05.000000 easybioinfo-0.3.1/src/easybioinfo/sequences.py
+drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-08-04 19:39:32.645097 easybioinfo-0.3.1/src/easybioinfo.egg-info/
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      700 2023-08-04 19:39:32.000000 easybioinfo-0.3.1/src/easybioinfo.egg-info/PKG-INFO
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      264 2023-08-04 19:39:32.000000 easybioinfo-0.3.1/src/easybioinfo.egg-info/SOURCES.txt
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)        1 2023-08-04 19:39:32.000000 easybioinfo-0.3.1/src/easybioinfo.egg-info/dependency_links.txt
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       12 2023-08-04 19:39:32.000000 easybioinfo-0.3.1/src/easybioinfo.egg-info/top_level.txt
```

### Comparing `easybioinfo-0.3.0/LICENSE` & `easybioinfo-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `easybioinfo-0.3.0/PKG-INFO` & `easybioinfo-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easybioinfo
-Version: 0.3.0
+Version: 0.3.1
 Summary: Convenient python functions for bioinformatics
 Home-page: https://github.com/marco-mariotti/easybioinfo
 Author: Marco Mariotti
 Author-email: marco.mariotti@ub.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `easybioinfo-0.3.0/setup.cfg` & `easybioinfo-0.3.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = easybioinfo
-version = 0.3.0
+version = 0.3.1
 author = Marco Mariotti
 author_email = marco.mariotti@ub.edu
 description = Convenient python functions for bioinformatics
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/marco-mariotti/easybioinfo
 project_urls =
```

### Comparing `easybioinfo-0.3.0/src/easybioinfo/sequences.py` & `easybioinfo-0.3.1/src/easybioinfo/sequences.py`

 * *Files 1% similar despite different names*

```diff
@@ -163,15 +163,15 @@
 def clear_kmer_memory():
     global kmer_codon_tables
     kmer_codon_tables.clear()
 
 def get_kmer_codon_table(genetic_code, k):
     if not (genetic_code, k) in kmer_codon_tables:
         all_codons=[c for c in genetic_codes['1'].keys()]
-        codon_table_multik={multicodon : translate(multicodon)
+        codon_table_multik={multicodon : translate(multicodon, genetic_code=genetic_code)
                             for multicodon in map(''.join, itertools.product( *(all_codons for i in range(k))))}
         kmer_codon_tables[(genetic_code, k)]=codon_table_multik
 
     return kmer_codon_tables[(genetic_code, k)]
 
 codon2sitecount = {}  # store computed data per codon
```

### Comparing `easybioinfo-0.3.0/src/easybioinfo.egg-info/PKG-INFO` & `easybioinfo-0.3.1/src/easybioinfo.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easybioinfo
-Version: 0.3.0
+Version: 0.3.1
 Summary: Convenient python functions for bioinformatics
 Home-page: https://github.com/marco-mariotti/easybioinfo
 Author: Marco Mariotti
 Author-email: marco.mariotti@ub.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

