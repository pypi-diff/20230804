# Comparing `tmp/twinstop-0.1.0.tar.gz` & `tmp/twinstop-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twinstop-0.1.0.tar", last modified: Fri Jul 28 19:48:38 2023, max compression
+gzip compressed data, was "twinstop-0.1.2.tar", last modified: Fri Aug  4 19:46:16 2023, max compression
```

## Comparing `twinstop-0.1.0.tar` & `twinstop-0.1.2.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-07-28 19:48:38.736694 twinstop-0.1.0/
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     1071 2023-07-25 10:35:28.000000 twinstop-0.1.0/LICENSE
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      633 2023-07-28 19:48:38.736694 twinstop-0.1.0/PKG-INFO
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      132 2023-07-25 10:35:28.000000 twinstop-0.1.0/README.md
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      104 2021-06-11 14:00:42.000000 twinstop-0.1.0/pyproject.toml
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     1065 2023-07-28 19:48:38.736694 twinstop-0.1.0/setup.cfg
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       69 2021-06-14 10:13:07.000000 twinstop-0.1.0/setup.py
-drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-07-28 19:48:38.736694 twinstop-0.1.0/src/
-drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-07-28 19:48:38.736694 twinstop-0.1.0/src/twinstop/
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       93 2023-07-25 10:19:10.000000 twinstop-0.1.0/src/twinstop/__init__.py
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       20 2023-07-28 16:05:53.000000 twinstop-0.1.0/src/twinstop/_version.py
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     4156 2023-07-26 09:06:02.000000 twinstop-0.1.0/src/twinstop/block_selection.py
-drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-07-28 19:48:38.736694 twinstop-0.1.0/src/twinstop/data_files/
--rw-r--r--   0 mmariotti  (1000) mmariotti  (1000)     2003 2023-07-25 13:30:48.000000 twinstop-0.1.0/src/twinstop/data_files/Matrix_BLOSUM62sel.txt
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     1461 2023-07-25 14:46:08.000000 twinstop-0.1.0/src/twinstop/data_files/logistic_regression_model.def.pkl
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     1461 2023-07-25 14:46:08.000000 twinstop-0.1.0/src/twinstop/data_files/logistic_regression_model.pre.pkl
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     1462 2023-07-25 14:46:08.000000 twinstop-0.1.0/src/twinstop/data_files/logistic_regression_model.sen.pkl
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     4142 2023-07-25 14:46:08.000000 twinstop-0.1.0/src/twinstop/data_files/scaler.pkl
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)   111812 2023-07-25 14:44:05.000000 twinstop-0.1.0/src/twinstop/denovo_selenoproteins_h3.bkp2.py
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)   119028 2023-07-28 16:09:29.000000 twinstop-0.1.0/src/twinstop/denovo_selenoproteins_h3.py
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     6979 2023-07-25 13:13:21.000000 twinstop-0.1.0/src/twinstop/test_alignment_methods.py
-drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-07-28 19:48:38.736694 twinstop-0.1.0/src/twinstop.egg-info/
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      633 2023-07-28 19:48:38.000000 twinstop-0.1.0/src/twinstop.egg-info/PKG-INFO
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      694 2023-07-28 19:48:38.000000 twinstop-0.1.0/src/twinstop.egg-info/SOURCES.txt
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)        1 2023-07-28 19:48:38.000000 twinstop-0.1.0/src/twinstop.egg-info/dependency_links.txt
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      217 2023-07-28 19:48:38.000000 twinstop-0.1.0/src/twinstop.egg-info/requires.txt
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)        9 2023-07-28 19:48:38.000000 twinstop-0.1.0/src/twinstop.egg-info/top_level.txt
+drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-08-04 19:46:16.246145 twinstop-0.1.2/
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     1071 2023-07-25 10:35:28.000000 twinstop-0.1.2/LICENSE
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      745 2023-08-04 19:46:16.246145 twinstop-0.1.2/PKG-INFO
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      244 2023-07-28 19:58:25.000000 twinstop-0.1.2/README.md
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      104 2021-06-11 14:00:42.000000 twinstop-0.1.2/pyproject.toml
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     1054 2023-08-04 19:46:16.246145 twinstop-0.1.2/setup.cfg
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       69 2021-06-14 10:13:07.000000 twinstop-0.1.2/setup.py
+drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-08-04 19:46:16.242145 twinstop-0.1.2/src/
+drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-08-04 19:46:16.246145 twinstop-0.1.2/src/twinstop/
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       93 2023-07-25 10:19:10.000000 twinstop-0.1.2/src/twinstop/__init__.py
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       20 2023-08-04 19:45:45.000000 twinstop-0.1.2/src/twinstop/_version.py
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     4218 2023-07-28 21:23:19.000000 twinstop-0.1.2/src/twinstop/block_selection.py
+drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-08-04 19:46:16.246145 twinstop-0.1.2/src/twinstop/data_files/
+-rw-r--r--   0 mmariotti  (1000) mmariotti  (1000)     2003 2023-07-25 13:30:48.000000 twinstop-0.1.2/src/twinstop/data_files/Matrix_BLOSUM62sel.txt
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     1461 2023-07-25 14:46:08.000000 twinstop-0.1.2/src/twinstop/data_files/logistic_regression_model.def.pkl
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     1461 2023-07-25 14:46:08.000000 twinstop-0.1.2/src/twinstop/data_files/logistic_regression_model.pre.pkl
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     1462 2023-07-25 14:46:08.000000 twinstop-0.1.2/src/twinstop/data_files/logistic_regression_model.sen.pkl
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     4142 2023-07-25 14:46:08.000000 twinstop-0.1.2/src/twinstop/data_files/scaler.pkl
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)   111812 2023-07-25 14:44:05.000000 twinstop-0.1.2/src/twinstop/denovo_selenoproteins_h3.bkp2.py
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)   120533 2023-07-28 21:22:59.000000 twinstop-0.1.2/src/twinstop/denovo_selenoproteins_h3.bkp3.py
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)   131351 2023-08-04 19:44:16.000000 twinstop-0.1.2/src/twinstop/denovo_selenoproteins_h3.py
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     6950 2023-07-28 21:23:28.000000 twinstop-0.1.2/src/twinstop/test_alignment_methods.py
+drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-08-04 19:46:16.246145 twinstop-0.1.2/src/twinstop.egg-info/
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      745 2023-08-04 19:46:16.000000 twinstop-0.1.2/src/twinstop.egg-info/PKG-INFO
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      740 2023-08-04 19:46:16.000000 twinstop-0.1.2/src/twinstop.egg-info/SOURCES.txt
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)        1 2023-08-04 19:46:16.000000 twinstop-0.1.2/src/twinstop.egg-info/dependency_links.txt
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      206 2023-08-04 19:46:16.000000 twinstop-0.1.2/src/twinstop.egg-info/requires.txt
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)        9 2023-08-04 19:46:16.000000 twinstop-0.1.2/src/twinstop.egg-info/top_level.txt
```

### Comparing `twinstop-0.1.0/LICENSE` & `twinstop-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `twinstop-0.1.0/PKG-INFO` & `twinstop-0.1.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,28 @@
 Metadata-Version: 2.1
 Name: twinstop
-Version: 0.1.0
+Version: 0.1.2
 Summary: twinstop identifies selenoproteins in close related transcriptomes
 Home-page: https://github.com/marco-mariotti/twinstop
 Author: Marco Mariotti and Sergio Sanchez Moragues
 Author-email: marco.mariotti@ub.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # twinstop
 Twinstop identifies selenoproteins in close related transcriptomes
 
+# Installation
+conda install -c conda-forge -c bioconda -c mmariotti    twinstop
+
+# Usage
+Run:
+
+  twinstop -h
+
+
 # Authors
-Marco Mariotti and Sergio Sanchez Moragues
+Sergio Sanchez Moragues and Marco Mariotti
```

### Comparing `twinstop-0.1.0/setup.cfg` & `twinstop-0.1.2/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -19,16 +19,16 @@
 package_dir = 
 	= src
 packages = find:
 python_requires = >=3.7
 install_requires = 
 	biopython >= 1.78, <=1.81
 	easyterm >= 1.0.0
-	easybioinfo >= 0.2.1
-	extend-orfs-pyranges >= 0.1.5
+	easybioinfo >= 0.3.1
+	orf_tools >= 0.0.1
 	file-chunk-iterators >= 0.0.1
 	pyranges >= 0.0.120
 	pandas >= 1.3.5
 	pyfaidx >= 0.7.2
 	multiprocess >= 0.70.14
 	numpy >= 1.21.5
 	scikit-learn >= 1.3.0
```

### Comparing `twinstop-0.1.0/src/twinstop/block_selection.py` & `twinstop-0.1.2/src/twinstop/block_selection.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 # -*- coding: utf-8 -*-
 
 import os
-twinstop_libpath=os.path.dirname(os.path.realpath(__file__)) +"/data_files/"
+
+twinstop_libpath = os.path.dirname(os.path.realpath(__file__)) + "/data_files/"
+
+
 def block_dict(query_seq, subj_seq, dictionary):
-    '''
-    Takes two protein sequences (one from the query and the other from the subject), 
-    divides them into blocks according to the stops '*' present in both and then 
+    """
+    Takes two protein sequences (one from the query and the other from the subject),
+    divides them into blocks according to the stops '*' present in both and then
     saves in a list of dictionaries the start, end and score (matrix Blosum62)
     of each block. Afterward, the block with better score is selected and the
     data of the score, start, end and sequence from both query and subject is
     updated in the general dataframe.
 
     Parameters
     ----------
@@ -20,49 +23,54 @@
     dictionary : Dictionary of tuples
         Matrix Blosum62 values
 
     Returns
     -------
     best_block[0] : Dictionary with the 'Start', 'End' and 'Score' values of the
     best scored fragment of each alignment.
-    '''
+    """
 
-    list_stops = list() # create a list to save stops index
+    list_stops = list()  # create a list to save stops index
 
     for index, x in enumerate(query_seq):
         # we count the start and the end of the sequence always as stops
         if index == 0 or index == len(query_seq) - 1:
             # if x != '*' and subj_seq[index] != '*':
             list_stops.append(index)
             continue
         # save all the indexes of stops
-        if x == '*' or subj_seq[index] == '*':
+        if x == "*" or subj_seq[index] == "*":
             list_stops.append(index)
 
-    block_dict_list = list() # creates a list
+    block_dict_list = list()  # creates a list
     for idx, x in enumerate(list_stops):
         if x == list_stops[-1]:
-            break # necessary to skip an error
-        block_dict = dict() # creates a dictionary
+            break  # necessary to skip an error
+        block_dict = dict()  # creates a dictionary
         # we skip the 1st and last index of the fragments (stops)
         ######################################
         #### MM: never scoring the first and last position --> fix it
-        block_dict['Align_Start'] = x + 1
-        block_dict['Align_End'] = list_stops[idx + 1]
-        block_dict['Score'] = score(query_seq[x: list_stops[idx + 1]], subj_seq[x: list_stops[idx + 1]], dictionary)
-        block_dict_list.append(block_dict) # create a list of dictionaries
+        block_dict["Align_Start"] = x + 1
+        block_dict["Align_End"] = list_stops[idx + 1]
+        block_dict["Score"] = score(
+            query_seq[x : list_stops[idx + 1]],
+            subj_seq[x : list_stops[idx + 1]],
+            dictionary,
+        )
+        block_dict_list.append(block_dict)  # create a list of dictionaries
     # dictionaries of each alignment are sorted by 'Score'
     # reverse=True to have the best scored one at the beginning
     # lambda input: output
-    best_block = sorted(block_dict_list, key=lambda x: x['Score'], reverse=True)
+    best_block = sorted(block_dict_list, key=lambda x: x["Score"], reverse=True)
+
+    return best_block[0]  # return the dictionary with the values of the best fragment
 
-    return best_block[0] # return the dictionary with the values of the best fragment 
 
 def score(query_frag, subj_frag, dictionary):
-    '''
+    """
     Calculates the score using matrix Blosum62
 
     Parameters
     ----------
     query_frag : String
         Protein sequence from the query
     subj_frag : String
@@ -70,40 +78,41 @@
     dictionary : Dictionary
         Matrix Blosum Values
 
     Returns
     -------
     Score : Int
         Value according to matrix Blosum62
-    '''
+    """
 
     score = 0
     for index, x in enumerate(query_frag):
-        if x == '-' or subj_frag[index] == '-':
+        if x == "-" or subj_frag[index] == "-":
             continue
         score += dictionary[(x, subj_frag[index])]
 
     return score
 
+
 def dictionary_seleno():
-    '''
+    """
     Creates a dictionary of tuples with the values of the BLOSUM62 Matrix.
 
     Returns
     -------
     dictionary_sel : <dict>
         Dictionary of tuples with the values of the BLOSUM62 Matrix.
-    '''
+    """
 
     dictionary_sel = dict()
 
-    with open(twinstop_libpath+'Matrix_BLOSUM62sel.txt', 'r') as fr:
+    with open(twinstop_libpath + "Matrix_BLOSUM62sel.txt", "r") as fr:
         for index, row in enumerate(fr):
             # creates a list, using ' ' as sep.
-            spt = row.split(' ')
+            spt = row.split(" ")
             # deletes blank spaces.
             spt = list(filter(None, spt))
             if index == 0:
                 # delete empty spaces.
                 header = [x.strip() for x in spt]
                 continue
             # deletes '\n' characters.
```

### Comparing `twinstop-0.1.0/src/twinstop/data_files/Matrix_BLOSUM62sel.txt` & `twinstop-0.1.2/src/twinstop/data_files/Matrix_BLOSUM62sel.txt`

 * *Files identical despite different names*

### Comparing `twinstop-0.1.0/src/twinstop/data_files/logistic_regression_model.def.pkl` & `twinstop-0.1.2/src/twinstop/data_files/logistic_regression_model.def.pkl`

 * *Files identical despite different names*

### Comparing `twinstop-0.1.0/src/twinstop/data_files/logistic_regression_model.pre.pkl` & `twinstop-0.1.2/src/twinstop/data_files/logistic_regression_model.pre.pkl`

 * *Files identical despite different names*

### Comparing `twinstop-0.1.0/src/twinstop/data_files/logistic_regression_model.sen.pkl` & `twinstop-0.1.2/src/twinstop/data_files/logistic_regression_model.sen.pkl`

 * *Files identical despite different names*

### Comparing `twinstop-0.1.0/src/twinstop/data_files/scaler.pkl` & `twinstop-0.1.2/src/twinstop/data_files/scaler.pkl`

 * *Files identical despite different names*

### Comparing `twinstop-0.1.0/src/twinstop/denovo_selenoproteins_h3.bkp2.py` & `twinstop-0.1.2/src/twinstop/denovo_selenoproteins_h3.bkp2.py`

 * *Files identical despite different names*

### Comparing `twinstop-0.1.0/src/twinstop/denovo_selenoproteins_h3.py` & `twinstop-0.1.2/src/twinstop/denovo_selenoproteins_h3.bkp3.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # -*- coding: utf-8 -*-
 """
 Created on Thu Jun 23 11:55:40 2022
 
 @author: Sergio Sánchez Moragues and Marco Mariotti
 """
 
-help_msg = """Twinstop is a de novo selenoprotein identification pipeline.
+help_msg = '='*80+"""
+Twinstop is a de novo selenoprotein identification pipeline.
 It is based on the evolutionary conservation around the UGA-coding selenocysteine between two homologous
 selenoproteins from two closely related transcriptomes.
 
 ### Compulsory Inputs/Outputs arguments:
 -q <str>   query file path: a transcriptome in fasta format
 -s <str>   subject file path: a nucleotide transcriptome in fasta format, with with makeblastdb run beforehand
 -o <str>   output folder path, where files generated by Twinstop will be saved
@@ -23,60 +24,80 @@
 -force <int>  controls the rerun of the phases of Twinstop. By default, it runs phases for which no output is detected.
               Provide a number, representing the phase from which Twinstop will start the rerun
               For information about phases, run:  twinstop -h phases
 
 #    Output: these switches control the optional output files written for candidates
 -cds_q <bool>  fasta file with CDS sequences of query.       Default: False
 -cds_s <bool>  fasta file with CDS sequences of subject.     Default: False
--pep_q <bool>  fasta file with protein sequences of query.   Default: True
--pep_s <bool>  fasta file with protein sequences of subject. Default: False
--gff_q <bool>  GFF file with coordinates on query.           Default: True
--gff_s <bool>  GFF file with coordinates on subject.         Default: False
+-pep_q <bool>  fasta file with protein sequences of query.   Default: False
+-pep_s <bool>  fasta file with protein sequences of subject. Default: True
+-gff_q <bool>  GFF file with coordinates on query.           Default: False
+-gff_s <bool>  GFF file with coordinates on subject.         Default: True
 
 #    Optional phase 7, annotation of candidates:
 -ann <bool>    perform the annotation of candidates (Phase 7). Requires -ann_db
 -ann_db <str>  path to database (protein fasta) to annotate candidates; recommended: Uniref50.
                Note: makeblastdb must have been run on this file beforehand to use it
 
-### Advanced:
+### Other options:
+-print_opt <bool>   print currently active options
+-h | --help <bool>  print this help and exit. For a full list of options, run: 
+                    twinstop -h full"""
+
+full_help="""### Advanced usage:
 # Twinstop can be very memory intensive, so it splits tables into chunks which are load and processed serially.
 -n_chunks <int> nº of chunks in which to divide the input file of phases 1,2,5.
                 Dividing in chunks reduces the memory but increases time. Default: 10
 -n_lines <int>  Chunk size (number of lines) used in phases 3,4. Default: 2500000
 -par_fct <int>  In phases 3,4,5, chunks are further divided in subchunks, processed in parallel.
                 This option sets the parallelization factor: the nº of subchunks per chunk is
                 determined as par_fct * N_CPUs. Default: 1
 # When performing pairwise alignments with the Biopython, some get stuck and take forever, so:
 -timeout <float>   Sets the maximum time for the execution of a pairwise alignment (phase 5).
                    The alignments exceeding the timeout are computed using MAFFT instead. Default: 2.0
 # Developer options
 -debug <bool>     Creates files with all filtered and filtered_out candidates for filtering phases: 3, 4, 6, 7
 -benchmark <bool> Developer option; activates benchmarking. See details with: twinstop -h benchmark
+"""
 
-### Other options:
--print_opt: print currently active options
--h | --help: print this help and exit"""
+titles_of_phases={
+    0:'TBLASTX',
+    1:'EXTRACT SEQS',
+    2:'FRAGMENTATION',
+    3:'OVERLAPPING FILTER',
+    4:'EXTEND ORFS',
+    5:'PAIRWISE ALIGNMENT',
+    6:'UGA ALIGNMENT FILTER',
+    7:'FINAL FILTER',
+    8:'BLASTP FOR ANNOTATION',
+    9:'OUTPUT'}
 
+colors={'phase':'green', 'count':'magenta'}
+
+def write_phase(n):
+    write(f'\n### PHASE {n}: {titles_of_phases[n]}', how=colors['phase'])
 
 description_of_phases={
     0:'Running tblastx between the transcriptomes',
     1:'Extracting CDS sequences and translating to get protein sequences',
     2:'Partitioning in UGA-containing ORFs, selecting best one per candidate',
     3:'Removing redundancy due to overlapping blast hits',
-    4:'Extending to have complete UGA-containing ORFs, then removing duplicates',
+    4:'Extending to have complete ORFs, then removing duplicates and non-UGA containing ORFs',
     5:'Performing pairwise alignments between complete UGA-containing ORFs',
     6:'Filtering out candidates that do not have UGA-UGA alignments',
     7:'Filtering candidates based on sequence conservation and other features',
     8:'Annotating candidates through blastp',
     9:'Producing output files'
 }
 
-phases_help="""
-TBD
-"""
+m=max([len(i) for i in titles_of_phases.values()])
+phases_help=("""\n### Description of phases """+
+             '\n'.join([f'PHASE {n}: {titles_of_phases[n]:<{m}}' + f' = {description_of_phases[n]}'
+                        for n in sorted(titles_of_phases.keys())])
+             )
 
 benchmark_help="""
 ### Benchmark usage: these are required if -benchmark is active
 # Benchmarking is performed counting how many of the selenoproteins expected on the subject are recovered
 # Note: it is generous, in the sense that only selenoprotein families that are expected in both subject 
 #  and query and counted, since they are the only ones that twinstop can, at best, predict.
 # Analogously, some selenoprotein families are always excluded since they have a terminal Sec, which
@@ -92,60 +113,62 @@
 -benchmark_query <str>  path to tabular file describing selenoproteins expected in query. 
                         Format: no header; fields: ['Chromosome', 'sel_family', 'id', 'subj_id']
 
 -unavailable_families <list>  list of selenoprotein families that are always excluded from benchmarking. 
                               These have C-terminal Sec residues. Default: SelK SelKi SelO SelS TR
 """
 
+advanced_help_dict={'phases':phases_help,
+                    'benchmark':benchmark_help,
+                    'full':full_help}
+
 def_opt = {
     'q': '',
     's': '',
     'o': 'twinstop_out/',
     'c': 1,
     'par_fct': 1,
     'n_chunks': 10,
     'n_lines': 2500000,
     'cds_q': False,
     'cds_s': False,
     'pep_q': False,
-    'pep_s': False,
+    'pep_s': True,
     'gff_q': False,
-    'gff_s': False,
+    'gff_s': True,
     'ann_db': '',
     'force': 1000,
     'ann': False,
     'benchmark_subject_gff': '',
     'benchmark_query': '',
     'unavailable_families':['SelK', 'SelKi', 'SelO', 'SelS', 'TR'],
     'benchmark': False,
     'debug': False,
     'timeout': 2.0,
     'time_mem': False,
     'model': 'd'
 }
 
 
-
-
 # packages:
 import os
 import pyranges as pr
 import subprocess
 import shlex
 import pandas as pd
 from sklearn.linear_model import LogisticRegression
 from sklearn.metrics import confusion_matrix
 import pickle
 import multiprocess as mp
 import numpy as np
 from datetime import datetime
-from easyterm import command_line_options, check_file_presence, write
-from easybioinfo import count_coding_changes, count_coding_sites, translate
 from Bio import pairwise2
 
+from easyterm import command_line_options, check_file_presence, write
+from easybioinfo import count_coding_changes, count_coding_sites, translate
 from extend_orfs_pyranges import extend_orfs
 from file_chunk_iterators import (
     iterate_file_in_chunks, iterate_file_in_chunks_with_key, buf_count_newlines_gen)
 
 # external scripts:
 from ._version import __version__
 from .block_selection import dictionary_seleno, score, block_dict
@@ -1800,26 +1823,33 @@
     if IsQueryGFFileReturned:
         query_df = selenocandidates_df.copy()
         query_df.drop(['Chromosome', 'Start', 'End', 'Strand'],
                       axis=1, inplace=True)
         query_df = query_df.rename(
             columns={'Q_ID': 'Chromosome', 'Q_align_s': 'Start',
                      'Q_align_e': 'End', 'Q_Strand': 'Strand'})
+        cols=['Chromosome', 'Source', 'Feature', 'Start', 'End',
+                'Strand', 'Score', 'Gene_ID']
+        if 'Annot_Title' in query_df:
+            cols.append('Annot_Title')
         query_df_reduced = query_df.loc[
-            :, ['Chromosome', 'Source', 'Feature', 'Start', 'End',
-                'Strand', 'Score', 'Gene_ID', 'Annot_Title']]
+            :, cols]
 
         py_query = pr.PyRanges(query_df_reduced)
         write(f'Output: query GFF --> {path_query_gff}')
         py_query.to_gff3(path=path_query_gff)
 
     if IsTargetGFFileReturned:
+        cols=['Chromosome', 'Source', 'Feature', 'Start', 'End',
+                'Strand', 'Score', 'Gene_ID']
+        if 'Annot_Title' in selenocandidates_df:
+            cols.append('Annot_Title')
+        
         candidates_reduced = selenocandidates_df.loc[
-            :, ['Chromosome', 'Source', 'Feature', 'Start', 'End',
-                'Strand', 'Score', 'Gene_ID', 'Annot_Title']]
+            :, cols]
 
         py_subj = pr.PyRanges(candidates_reduced)
         write(f'Output: subject GFF --> {path_subj_gff}')
         py_subj.to_gff3(path=path_subj_gff)
 
 def get_proc_status(keys=None):
     '''
@@ -2038,15 +2068,15 @@
 def main():
 
     initial_time = datetime.now()
     # .strftime method allows to put a datetime object in clock format '%H:%M:%S'
 
     # easyterm method to create a dictionary with command line input parameters and a help message
     opt = command_line_options(def_opt, help_msg,
-                               advanced_help_msg={'phases':phases_help}
+                               advanced_help_msg=advanced_help_dict
     )
     # os.path.abspath(relative/absolute path) gets the absolute path of a file
     q_file = os.path.abspath(opt['q'])
     # checks if query file exists
     check_file_presence(q_file, 'Given path for query file does not exist')
     subj_file = os.path.abspath(opt['s'])
     # checks if subject file exists
@@ -2095,16 +2125,14 @@
     n_section =  opt['force']
     time_memory_control = opt['time_mem']
     # benchmark variable is defined as global to use it all across the script without the need of being imported
     global benchmark, debugging
     benchmark = opt['benchmark']
     debugging = opt['debug']
 
-    colors={'phase':'green', 'count':'magenta'}
-
     if benchmark:
         # read table of the Selenoprofiles4 selenocysteines prediction for subject (control selenoproteins)
         sp4_subj_gff = pd.read_csv(opt['benchmark_subject_gff'], sep="\t", header=None, index_col=False)
         sp4_subj_gff.columns = ['Chromosome', 'source', 'feature', 'sec_start', 'sec_end',
                                 'score', 'strand', 'frame', 'attribute', 'subj_id']
         sp4_prediction_subj = pd.DataFrame()
         sp4_prediction_subj['Transcript'] = sp4_subj_gff.Chromosome
@@ -2134,85 +2162,87 @@
         # keeps the rest of selenos
         available_selenos = selenos_annot[~selenos_annot.Sel_family.isin(unavailable_Sel_families)]
         if available_selenos.shape[0] != selenos_annot.shape[0]:
             unavailable_sel = selenos_annot[selenos_annot.Sel_family.isin(unavailable_Sel_families)]
             write(f'Unavailable Selenoprotein families predicted by Selenoprofiles 4:\n\n{unavailable_sel}')
         del selenos_annot
 
-    write('\n### PHASE 0: TBLASTX', how=colors['phase'])
- 
+    #write('\n### PHASE 0: TBLASTX', how=colors['phase'])
+    write_phase(0)
+
     # first phase of the script is to run a tblastx between the query and subject transcriptomes to get the best
     # alignments among the transcripts.
     if not os.path.exists(path_tblastx_outfile) or n_section==0:
         write(description_of_phases[0])
         run_tblastx(q_file, subj_file, n_cpu, True, #n_section==0,
                     path_tblastx_outfile+'.tmp')
         os.rename(path_tblastx_outfile+'.tmp', path_tblastx_outfile)
         
         write(f'tblastx file created --> {path_tblastx_outfile}')
     else:
         write(f'File found: {path_tblastx_outfile}')
-    write(f'Nº of tBLASTx hits: {buf_count_newlines_gen(path_tblastx_outfile)}', how=colors['count'])
 
+    # we read the last phase outfile 'Chromosome' column (Subject transcripts ID)
+    trans_candidates = pd.read_csv(path_postchunking_outfile, usecols=['Chromosome'],
+                                   sep="\t", header=0, index_col=False)['Chromosome']
+    #write(f'Nº of tBLASTx hits: {buf_count_newlines_gen(path_tblastx_outfile)}', how=colors['count'])
+    write(f'After tBLASTx, Nº of hits: {len(trans_candidates)}', how=colors['count'])    
+    write(f'After tBLASTx, Nº of unique subject transcripts: {len(trans_candidates.unique())}', how=colors['count'])
+
+    if  benchmark:
+        # and we check how many expected selenoprotein transcripts have successfully passed the filter
+        write(f'TP: {available_selenos.Transcript.isin(trans_candidates).sum()}/{len(available_selenos)}')
+    del trans_candidates
+    
     if time_memory_control:
         time_mem_usage(initial_time)
         initial_time = datetime.now()
 
-    write('\n### PHASE 1: EXTRACT SEQS', how=colors['phase'])
-
+    #write('\n### PHASE 1: EXTRACT SEQS', how=colors['phase'])
+    write_phase(1)
+    
     def mp_join_dfs(x):
         return join_dfs(x, subj_file, q_file)
 
-    run_phase1=False
     # if the output file already exists, we can force any phase rerun with 'n_section' variable
     if not os.path.exists(path_postchunking_outfile) or n_section < 2:
         write(description_of_phases[1])
         # chunking function allows to open files as iterators, so only a chunk is charged into memory at a time
         chunking(path_tblastx_outfile, n_chunks, 0, mp_join_dfs, 
                  n_cpu, None, path_postchunking_outfile+'.tmp', n)
         os.rename(path_postchunking_outfile+'.tmp', path_postchunking_outfile)
         write(f'Table including sequences created --> {path_postchunking_outfile}')
-        run_phase1=True
 
     else:
         write(f'File found: {path_postchunking_outfile}')
 
-    if run_phase1 or benchmark:
-        # we read the last phase outfile 'Chromosome' column (Subject transcripts ID)
-        trans_candidates = pd.read_csv(path_postchunking_outfile, usecols=['Chromosome'],
-                                       sep="\t", header=0, index_col=False)['Chromosome']
-        write(f'Nº of unique subject transcripts: {len(trans_candidates.unique())}', how=colors['count'])
-
-        if benchmark:
-            # and we check how many expected selenoprotein transcripts have successfully passed the filter
-            write(f'TP: {available_selenos.Transcript.isin(trans_candidates).sum()}/{len(available_selenos)}')
-
-        del trans_candidates
 
     # using time_memory_control==True we can know the time and memory (current and peak) in each phase
     if time_memory_control:
         time_mem_usage(initial_time)
         initial_time = datetime.now()
 
-    write('\n### PHASE 2: FRAGMENTATION', how=colors['phase'])
+    #write('\n### PHASE 2: FRAGMENTATION', how=colors['phase'])
+    write_phase(2)
 
     if not os.path.exists(path_fragmentation_outfile) or n_section < 3:
         write(description_of_phases[2])
         chunking(path_postchunking_outfile, n_chunks, 0, fragmentation,
                  n_cpu, None, path_fragmentation_outfile+'.tmp', n)
         os.rename(path_fragmentation_outfile+'.tmp', path_fragmentation_outfile)
         write(f'Table with best ORFs selected (for query and subject) per candidate --> {path_fragmentation_outfile}')
     else:
         write(f'File found: {path_fragmentation_outfile}')
 
     if time_memory_control:
         time_mem_usage(initial_time)
         initial_time = datetime.now()
 
-    write('\n### PHASE 3: OVERLAPPING FILTER', how=colors['phase'])
+    #write('\n### PHASE 3: OVERLAPPING FILTER', how=colors['phase'])
+    write_phase(3)
 
     run_phase3=False
     if not os.path.exists(path_overlapping_outfile) or n_section < 4:
         write(description_of_phases[3])
         chunking(path_fragmentation_outfile, 0, n_lines, 
                  lambda x: overlapping_filter(x, n_cpu), n_cpu, None,
                  path_overlapping_outfile+'.tmp', n, overlapping=True, chunk_by_key=True)
@@ -2233,45 +2263,47 @@
             write(f'\nTP: {available_selenos.Transcript.isin(trans_candidates).sum()}/{len(available_selenos)}')
         del trans_candidates
 
     if time_memory_control:
         time_mem_usage(initial_time)
         initial_time = datetime.now()
 
-    write('\n### PHASE 4: EXTEND ORFS', how=colors['phase'])
+    #write('\n### PHASE 4: EXTEND ORFS', how=colors['phase'])
+    write_phase(4)
 
     def mp_ext_orfs(x):
         return run_extend(x, q_file, subj_file)
 
     run_phase4=False
     if not os.path.exists(path_extend_outfile) or n_section < 5:
         write(description_of_phases[4])
 
         chunking(path_overlapping_outfile, 0, n_lines, mp_ext_orfs, n_cpu,
                  None, path_extend_outfile+'.tmp', n, ext_orfs=True, chunk_by_key=True)
         os.rename(path_extend_outfile+'.tmp', path_extend_outfile)
         run_phase4=True
         write(f'Table with non-identical extended ORFs --> {path_extend_outfile}')
-        write(f'Nº of hits with non-identical extended ORFs: {buf_count_newlines_gen(path_extend_outfile)}', how=colors['count'])
+        write(f'After extending ORFs and removing duplicates, Nº of hits: {buf_count_newlines_gen(path_extend_outfile)}', how=colors['count'])
     else:
         write(f'File found: {path_extend_outfile}')
 
     if run_phase4 or benchmark:
         trans_candidates = pd.read_csv(path_extend_outfile, sep="\t", header=0,
                                    index_col=False, usecols=['Chromosome'])['Chromosome']
-        write(f'Nº of unique subject transcripts: {len(trans_candidates.unique())}', how=colors['count'])
+        write(f'After extending ORFs and removing duplicates, Nº of unique subject transcripts: {len(trans_candidates.unique())}', how=colors['count'])
         if benchmark:
             write(f'\nTP: {available_selenos.Transcript.isin(trans_candidates).sum()}/{len(available_selenos)}')
         del trans_candidates        
 
     if time_memory_control:
         time_mem_usage(initial_time)
         initial_time = datetime.now()
 
-    write('\n### PHASE 5: PAIRWISE ALIGNMENT', how=colors['phase'])
+    #write('\n### PHASE 5: PAIRWISE ALIGNMENT', how=colors['phase'])
+    write_phase(5)
 
     if not os.path.exists(path_pairwise_outfile) or n_section < 6:
         write(description_of_phases[5])
         
         chunking(path_extend_outfile, n_chunks, 0, pairwise_alignment, n_cpu,
                  opt['timeout'], path_pairwise_outfile+'.tmp', n, pairwise=True)
         os.rename(path_pairwise_outfile+'.tmp', path_pairwise_outfile)
@@ -2279,15 +2311,16 @@
     else:
         write(f'File found: {path_pairwise_outfile}')
 
     if time_memory_control:
         time_mem_usage(initial_time)
         initial_time = datetime.now()
 
-    write('\n### PHASE 6: UGA ALIGNMENT FILTER', how=colors['phase'])
+    #write('\n### PHASE 6: UGA ALIGNMENT FILTER', how=colors['phase'])
+    write_phase(6)
 
     run_phase6=False
     # from this point we stop using chunking(). Now, dataframes are read at once.
     if not os.path.exists(path_candidates_outfile) or n_section < 7:
         write(description_of_phases[6])
         # as we are not using chunking(), pre-phase file must be read to pass it as arg to the next phase function
         aln_orfs = pd.read_csv(path_pairwise_outfile, sep='\t', header=0, index_col=False)
@@ -2318,24 +2351,25 @@
         #     .drop_duplicates('Chromosome', ignore_index=True)
         # candidates_df.to_csv(path_or_buf=path_candidates_outfile, sep='\t', index=False)
         # here there is a control to prevent empty dfs to be passed to the next phase causing an error
         if len(candidates_df) == 0:
             write(f'Empty file {candidates_df}')
 
     if run_phase6 or benchmark:
-        write(f'After the first filter, Nº of candidates: {buf_count_newlines_gen(path_candidates_outfile)}', how=colors['count'])
-        write(f'Nº of unique subject transcripts: {len(candidates_df.Chromosome.unique())}')
+        write(f'After the UGA alignment filter, Nº of candidates: {buf_count_newlines_gen(path_candidates_outfile)}', how=colors['count'])
+        write(f'After the UGA alignment filter, Nº of unique subject transcripts: {len(candidates_df.Chromosome.unique())}', how=colors['count'])
         if benchmark:
             write(f'\nTP: {available_selenos.Transcript.isin(candidates_df.Chromosome).sum()}/{len(available_selenos)}')
 
     if time_memory_control:
         time_mem_usage(initial_time)
         initial_time = datetime.now()
 
-    write('\n### PHASE 7: FINAL FILTER', how=colors['phase'])
+    #write('\n### PHASE 7: FINAL FILTER', how=colors['phase'])
+    write_phase(7)
 
     # if not os.path.exists(path_selenocandidates_outfile) or n_section < 8:
     #     candidates_df = evo_conservation(candidates_df, opt['selective_pressure'],
     #                                      opt['max_prot_changes'], opt['dNdS_filter'],
     #                                      opt['cons_up'], opt['cons_down'], q_file, subj_file)
     #     candidates_df.to_csv(path_or_buf=path_selenocandidates_outfile, sep='\t', index=False)
     # else:
@@ -2388,24 +2422,26 @@
             write(f'\nSensitivity_lr: {recall_ml}\n')
             write(f'\nPrecision Twinstop: {precision_ml}')
             write(f'\nSensitivity Twinstop: {recall * recall_ml}\n')
     else:
         candidates_df = pd.read_csv(path_selenocandidates_outfile, sep='\t', header=0, index_col=False)
         write(f'File found: {path_selenocandidates_outfile}')
         
-    write(f'After final filter, Nº of candidates: {buf_count_newlines_gen(path_selenocandidates_outfile)}', how=colors['count'])
-    # write(f'\nNº of unique subject transcripts: {len(candidates_df.Chromosome.unique())}')
+    #write(f'After final filter, Nº of candidates: {buf_count_newlines_gen(path_selenocandidates_outfile)}', how=colors['count'])
+    write(f'After final filter, Nº of candidates: {len(candidates_df)}', how=colors['count'])
+    write(f'After final filter, Nº of unique subject transcripts: {len(candidates_df.Chromosome.unique())}', how=colors['count']) 
     # write(f'\nTP: {available_selenos.Transcript.isin(candidates_df.Chromosome).sum()}/{len(available_selenos)}')
 
     if time_memory_control:
         time_mem_usage(initial_time)
         initial_time = datetime.now()
 
     if opt['ann']:
-        write('\n### PHASE 8: BLASTP FOR ANNOTATION', how=colors['phase'])
+        #write('\n### PHASE 8: BLASTP FOR ANNOTATION', how=colors['phase'])
+        write_phase(8)
     else:
         write('\n### Skipping PHASE 8 because not requested...')
 
     if not 'Annot_Title' in candidates_df and opt['ann']:
         write(description_of_phases[8])
         candidates_df = run_blastp(candidates_df, opt['ann_db'], n_cpu,
                                    path_blastp_outfile, path_fasta_query_prot_seq)
@@ -2415,16 +2451,17 @@
         # write(f'\nNº of unique subject transcripts: {len(candidates_df.Chromosome.unique())}')
         # write(f'\nTP: {available_selenos.Transcript.isin(candidates_df.Chromosome).sum()}/{len(available_selenos)}')
 
     if time_memory_control:
         time_mem_usage(initial_time)
         initial_time = datetime.now()
 
-    write('\n### PHASE 9: OUTPUTS', how=colors['phase'])
-
+    #write('\n### PHASE 9: OUTPUT', how=colors['phase'])
+    write_phase(9)
+    
     write(description_of_phases[9])
     candidates_pretty = pretty_output(candidates_df)
     write(f'Output file with user-readable alignments created --> {path_pretty_outfile}')
     with open(path_pretty_outfile, 'w') as fw:
         fw.write(candidates_pretty)
 
     make_outputs(candidates_df, opt['cds_q'], path_cds_q, opt['cds_s'], path_cds_t,
```

### Comparing `twinstop-0.1.0/src/twinstop/test_alignment_methods.py` & `twinstop-0.1.2/src/twinstop/test_alignment_methods.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,69 +3,73 @@
 """
 Created on Thu May 12 12:18:00 2022
 
 @author: Toño
 """
 
 from easyterm import command_line_options, write
+
 # from Bio import pairwise2
 import pandas as pd, subprocess, shlex, multiprocess as mp, numpy as np, os
+
 # from Bio.SubsMat import MatrixInfo as matlist
 # from denovo_selenoproteins import dictionary_seleno
 
+
 def mafft(joined_df):
     # out_mafft = '/users-d2/EGB4-guest/seleno_prediction/outputs/out_mafft'
     # mafft alignment
     assert len(joined_df) == 1
     i = joined_df.index[0]
-    out_temp = 'fasta_mafft_' + str(i)
-    #for i in joined_df.index:
+    out_temp = "fasta_mafft_" + str(i)
+    # for i in joined_df.index:
     # to run mafft we need a fasta file with the subject and query
     # protein sequences.
-    with open(out_temp, 'w') as fw:
+    with open(out_temp, "w") as fw:
         fw.write(f">Subject\n")
         fw.write(f"{joined_df.at[i, 'Subj_align_prot_seq']}\n")
         fw.write(f">Query\n")
         fw.write(f"{joined_df.at[i, 'Q_align_prot_seq']}\n")
     # --anysymbol is used to recognize 'U'
     # ???
     # print(joined_df.loc[i, 'Subj_align_prot_seq'])
     # print(joined_df.loc[i, 'Q_align_prot_seq'])
     # print(f'Out temp = {out_temp}')
-    mafft_subj = 'mafft --auto --anysymbol ' + out_temp
+    mafft_subj = "mafft --auto --anysymbol " + out_temp
     subj_mafft_list = shlex.split(mafft_subj)
     y = subprocess.run(subj_mafft_list, capture_output=True)
     if y.returncode != 0:
         print(y.stderr, y.stdout)
         raise Exception()
     os.remove(out_temp)
     # we need to decode() the standard output to get the results.
-    outfile = y.stdout.decode().split('\n')
+    outfile = y.stdout.decode().split("\n")
     # print(outfile)
-    temp_mafft = ''
+    temp_mafft = ""
     for x in outfile:
-        if x == '>Subject' or x == '':
+        if x == ">Subject" or x == "":
             continue
-        elif x == '>Query':
-            temp_mafft += f'\n'
+        elif x == ">Query":
+            temp_mafft += f"\n"
         else:
-            temp_mafft += f'{x}'
+            temp_mafft += f"{x}"
     # print(f'Temp mafft = {temp_mafft}')
-    list_mafft = temp_mafft.split('\n')
+    list_mafft = temp_mafft.split("\n")
     # print(f'List mafft = {list_mafft}')
     # substitute the sequences without gaps for the new one with gaps.
     try:
-        joined_df.at[i, 'Subj_align_prot_seq'] = list_mafft[0]
-        joined_df.at[i, 'Q_align_prot_seq'] = list_mafft[1]
+        joined_df.at[i, "Subj_align_prot_seq"] = list_mafft[0]
+        joined_df.at[i, "Q_align_prot_seq"] = list_mafft[1]
     except:
-        print(f'Joined_df = {joined_df}')
+        print(f"Joined_df = {joined_df}")
         raise SystemExit
 
     return joined_df
 
+
 # def pairwise_alignment(extended_hits_df, matrix):
 #     '''
 #     This function runs Pairwise global alignment tool to insert gaps in the aligned
 #     protein sequences.
 #
 #     Parameters
 #     ----------
@@ -126,53 +130,55 @@
 #     #         print(f'Second pairwise worked with timeout {timeout}')
 #     # else:
 #     #     post_df = pd.concat(results, axis=0, ignore_index=True)
 #     #     print(f'Second pairwise worked with timeout {timeout}')
 #
 #     return results
 
+
 def multiprocessing(chunkdf, func, n_cpu, timeout):
     with mp.Pool(processes=n_cpu) as pool:
         # lock = mp.Manager().Lock()
         # shared_list = manager.list()
         results = []
         completed_results = []
         for row in np.array_split(chunkdf, len(chunkdf)):
             result = pool.apply_async(func, args=(row,))
             results.append(result)
         for result in results:
             try:
                 completed_results.append(result.get(timeout=timeout))
             except mp.context.TimeoutError:
-                print(f'A result took too long')
+                print(f"A result took too long")
                 pass
 
         df_chunk = pd.concat(completed_results, axis=0, ignore_index=True)
     return df_chunk
 
+
 # def main():
 #     help_msg = """ This program allows us to test which alignment
 #     method is faster.
 #
 #     ### Input/Output:
 #     -df : dataframe with the sequences to align
 #
 #     ### Options:
 #     -print_opt: print currently active options
 #     -h | --help: print this help and exit"""
 #
 #     def_opt = {'pre_df': '/home/ssanchez/seleno_prediction/outputs/Mus_musculus_vs_Homo_sapiens/ext_orfs.tsv',
 #                'post_df': '/home/ssanchez/seleno_prediction/outputs/Mus_musculus_vs_Homo_sapiens/aln_orfs.tsv'}
 
-    # opt = command_line_options(def_opt, help_msg)
+# opt = command_line_options(def_opt, help_msg)
 
-    # pre_df = pd.read_csv(opt['pre_df'],
-    #                      sep='\t', header=0, index_col=False)
-    # post_df = pd.read_csv(opt['post_df'],
-    #                       sep='\t', header=0, index_col=False)
-    #
-    # output = missing_alignments(pre_df, post_df, 2.5)
-    # output.to_csv('/home/ssanchez/seleno_prediction/outputs/recovered_align.tsv',
-    #               sep='\t', header=0, index=False)
+# pre_df = pd.read_csv(opt['pre_df'],
+#                      sep='\t', header=0, index_col=False)
+# post_df = pd.read_csv(opt['post_df'],
+#                       sep='\t', header=0, index_col=False)
+#
+# output = missing_alignments(pre_df, post_df, 2.5)
+# output.to_csv('/home/ssanchez/seleno_prediction/outputs/recovered_align.tsv',
+#               sep='\t', header=0, index=False)
 
 # if __name__ == '__main__':
 #     main()
```

### Comparing `twinstop-0.1.0/src/twinstop.egg-info/PKG-INFO` & `twinstop-0.1.2/src/twinstop.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,28 @@
 Metadata-Version: 2.1
 Name: twinstop
-Version: 0.1.0
+Version: 0.1.2
 Summary: twinstop identifies selenoproteins in close related transcriptomes
 Home-page: https://github.com/marco-mariotti/twinstop
 Author: Marco Mariotti and Sergio Sanchez Moragues
 Author-email: marco.mariotti@ub.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # twinstop
 Twinstop identifies selenoproteins in close related transcriptomes
 
+# Installation
+conda install -c conda-forge -c bioconda -c mmariotti    twinstop
+
+# Usage
+Run:
+
+  twinstop -h
+
+
 # Authors
-Marco Mariotti and Sergio Sanchez Moragues
+Sergio Sanchez Moragues and Marco Mariotti
```

### Comparing `twinstop-0.1.0/src/twinstop.egg-info/SOURCES.txt` & `twinstop-0.1.2/src/twinstop.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 pyproject.toml
 setup.cfg
 setup.py
 src/twinstop/__init__.py
 src/twinstop/_version.py
 src/twinstop/block_selection.py
 src/twinstop/denovo_selenoproteins_h3.bkp2.py
+src/twinstop/denovo_selenoproteins_h3.bkp3.py
 src/twinstop/denovo_selenoproteins_h3.py
 src/twinstop/test_alignment_methods.py
 src/twinstop.egg-info/PKG-INFO
 src/twinstop.egg-info/SOURCES.txt
 src/twinstop.egg-info/dependency_links.txt
 src/twinstop.egg-info/requires.txt
 src/twinstop.egg-info/top_level.txt
```

