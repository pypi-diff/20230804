# Comparing `tmp/pepmatch-0.9.3.tar.gz` & `tmp/pepmatch-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pepmatch-0.9.3.tar", last modified: Mon Jul  3 06:43:04 2023, max compression
+gzip compressed data, was "pepmatch-0.9.4.tar", last modified: Fri Aug  4 05:06:04 2023, max compression
```

## Comparing `pepmatch-0.9.3.tar` & `pepmatch-0.9.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 dmarrama (2118653919) LIAI_AD\Domain Users (1127120232)        0 2023-07-03 06:43:04.270998 pepmatch-0.9.3/
--rw-r--r--   0 dmarrama (2118653919) LIAI_AD\Domain Users (1127120232)    11757 2023-03-01 21:01:30.000000 pepmatch-0.9.3/LICENSE
--rw-r--r--   0 dmarrama (2118653919) LIAI_AD\Domain Users (1127120232)     4839 2023-07-03 06:43:04.270619 pepmatch-0.9.3/PKG-INFO
--rw-r--r--   0 dmarrama (2118653919) LIAI_AD\Domain Users (1127120232)     4508 2023-05-30 05:21:03.000000 pepmatch-0.9.3/README.md
-drwxr-xr-x   0 dmarrama (2118653919) LIAI_AD\Domain Users (1127120232)        0 2023-07-03 06:43:04.264990 pepmatch-0.9.3/pepmatch/
--rw-r--r--   0 dmarrama (2118653919) LIAI_AD\Domain Users (1127120232)      207 2023-05-30 05:21:03.000000 pepmatch-0.9.3/pepmatch/__init__.py
--rw-r--r--   0 dmarrama (2118653919) LIAI_AD\Domain Users (1127120232)     2096 2023-05-30 05:21:03.000000 pepmatch-0.9.3/pepmatch/benchmarker.py
--rw-r--r--   0 dmarrama (2118653919) LIAI_AD\Domain Users (1127120232)     2015 2023-05-30 05:21:03.000000 pepmatch-0.9.3/pepmatch/helpers.py
--rwxr-xr-x   0 dmarrama (2118653919) LIAI_AD\Domain Users (1127120232)    32023 2023-07-03 06:41:59.000000 pepmatch-0.9.3/pepmatch/matcher.py
--rwxr-xr-x   0 dmarrama (2118653919) LIAI_AD\Domain Users (1127120232)    10818 2023-05-30 05:21:03.000000 pepmatch-0.9.3/pepmatch/preprocessor.py
--rw-r--r--   0 dmarrama (2118653919) LIAI_AD\Domain Users (1127120232)       22 2023-07-03 06:42:22.000000 pepmatch-0.9.3/pepmatch/version.py
-drwxr-xr-x   0 dmarrama (2118653919) LIAI_AD\Domain Users (1127120232)        0 2023-07-03 06:43:04.267766 pepmatch-0.9.3/pepmatch.egg-info/
--rw-r--r--   0 dmarrama (2118653919) LIAI_AD\Domain Users (1127120232)     4839 2023-07-03 06:43:02.000000 pepmatch-0.9.3/pepmatch.egg-info/PKG-INFO
--rw-r--r--   0 dmarrama (2118653919) LIAI_AD\Domain Users (1127120232)      486 2023-07-03 06:43:03.000000 pepmatch-0.9.3/pepmatch.egg-info/SOURCES.txt
--rw-r--r--   0 dmarrama (2118653919) LIAI_AD\Domain Users (1127120232)        1 2023-07-03 06:43:02.000000 pepmatch-0.9.3/pepmatch.egg-info/dependency_links.txt
--rw-r--r--   0 dmarrama (2118653919) LIAI_AD\Domain Users (1127120232)      104 2023-07-03 06:43:02.000000 pepmatch-0.9.3/pepmatch.egg-info/entry_points.txt
--rw-r--r--   0 dmarrama (2118653919) LIAI_AD\Domain Users (1127120232)        1 2023-03-03 04:38:29.000000 pepmatch-0.9.3/pepmatch.egg-info/not-zip-safe
--rw-r--r--   0 dmarrama (2118653919) LIAI_AD\Domain Users (1127120232)       80 2023-07-03 06:43:02.000000 pepmatch-0.9.3/pepmatch.egg-info/requires.txt
--rw-r--r--   0 dmarrama (2118653919) LIAI_AD\Domain Users (1127120232)        9 2023-07-03 06:43:02.000000 pepmatch-0.9.3/pepmatch.egg-info/top_level.txt
--rw-r--r--   0 dmarrama (2118653919) LIAI_AD\Domain Users (1127120232)       38 2023-07-03 06:43:04.271113 pepmatch-0.9.3/setup.cfg
--rwxr-xr-x   0 dmarrama (2118653919) LIAI_AD\Domain Users (1127120232)      999 2023-05-30 05:21:03.000000 pepmatch-0.9.3/setup.py
-drwxr-xr-x   0 dmarrama (2118653919) LIAI_AD\Domain Users (1127120232)        0 2023-07-03 06:43:04.269865 pepmatch-0.9.3/test/
--rw-r--r--   0 dmarrama (2118653919) LIAI_AD\Domain Users (1127120232)     1769 2023-05-30 05:21:03.000000 pepmatch-0.9.3/test/test_best_match.py
--rw-r--r--   0 dmarrama (2118653919) LIAI_AD\Domain Users (1127120232)      569 2023-05-30 05:21:03.000000 pepmatch-0.9.3/test/test_discontinuous_search.py
--rw-r--r--   0 dmarrama (2118653919) LIAI_AD\Domain Users (1127120232)     1743 2023-05-30 05:21:03.000000 pepmatch-0.9.3/test/test_exact_match.py
--rw-r--r--   0 dmarrama (2118653919) LIAI_AD\Domain Users (1127120232)     1785 2023-05-30 05:21:03.000000 pepmatch-0.9.3/test/test_mismatch.py
+drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2023-08-04 05:06:04.602626 pepmatch-0.9.4/
+-rw-r--r--   0 dan       (1000) dan       (1000)    11757 2021-03-17 17:44:53.000000 pepmatch-0.9.4/LICENSE
+-rw-r--r--   0 dan       (1000) dan       (1000)     4839 2023-08-04 05:06:04.602626 pepmatch-0.9.4/PKG-INFO
+-rw-r--r--   0 dan       (1000) dan       (1000)     4508 2023-05-30 01:05:06.000000 pepmatch-0.9.4/README.md
+drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2023-08-04 05:06:04.602626 pepmatch-0.9.4/pepmatch/
+-rw-r--r--   0 dan       (1000) dan       (1000)      207 2023-05-29 18:43:11.000000 pepmatch-0.9.4/pepmatch/__init__.py
+-rw-r--r--   0 dan       (1000) dan       (1000)     2096 2023-05-30 00:23:28.000000 pepmatch-0.9.4/pepmatch/benchmarker.py
+-rw-r--r--   0 dan       (1000) dan       (1000)     2040 2023-07-05 05:57:41.000000 pepmatch-0.9.4/pepmatch/helpers.py
+-rwxr-xr-x   0 dan       (1000) dan       (1000)    32329 2023-07-27 04:43:15.000000 pepmatch-0.9.4/pepmatch/matcher.py
+-rwxr-xr-x   0 dan       (1000) dan       (1000)    10818 2023-05-30 00:46:42.000000 pepmatch-0.9.4/pepmatch/preprocessor.py
+-rw-r--r--   0 dan       (1000) dan       (1000)       22 2023-08-04 05:03:03.000000 pepmatch-0.9.4/pepmatch/version.py
+drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2023-08-04 05:06:04.602626 pepmatch-0.9.4/pepmatch.egg-info/
+-rw-r--r--   0 dan       (1000) dan       (1000)     4839 2023-08-04 05:06:04.000000 pepmatch-0.9.4/pepmatch.egg-info/PKG-INFO
+-rw-r--r--   0 dan       (1000) dan       (1000)      486 2023-08-04 05:06:04.000000 pepmatch-0.9.4/pepmatch.egg-info/SOURCES.txt
+-rw-r--r--   0 dan       (1000) dan       (1000)        1 2023-08-04 05:06:04.000000 pepmatch-0.9.4/pepmatch.egg-info/dependency_links.txt
+-rw-r--r--   0 dan       (1000) dan       (1000)      104 2023-08-04 05:06:04.000000 pepmatch-0.9.4/pepmatch.egg-info/entry_points.txt
+-rw-r--r--   0 dan       (1000) dan       (1000)        1 2021-01-26 17:40:31.000000 pepmatch-0.9.4/pepmatch.egg-info/not-zip-safe
+-rw-r--r--   0 dan       (1000) dan       (1000)       80 2023-08-04 05:06:04.000000 pepmatch-0.9.4/pepmatch.egg-info/requires.txt
+-rw-r--r--   0 dan       (1000) dan       (1000)        9 2023-08-04 05:06:04.000000 pepmatch-0.9.4/pepmatch.egg-info/top_level.txt
+-rw-r--r--   0 dan       (1000) dan       (1000)       38 2023-08-04 05:06:04.602626 pepmatch-0.9.4/setup.cfg
+-rwxr-xr-x   0 dan       (1000) dan       (1000)      999 2023-05-30 00:22:00.000000 pepmatch-0.9.4/setup.py
+drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2023-08-04 05:06:04.602626 pepmatch-0.9.4/test/
+-rw-r--r--   0 dan       (1000) dan       (1000)     1769 2023-05-29 19:07:02.000000 pepmatch-0.9.4/test/test_best_match.py
+-rw-r--r--   0 dan       (1000) dan       (1000)      569 2023-07-27 04:01:52.000000 pepmatch-0.9.4/test/test_discontinuous_search.py
+-rw-r--r--   0 dan       (1000) dan       (1000)     1743 2023-05-29 19:04:07.000000 pepmatch-0.9.4/test/test_exact_match.py
+-rw-r--r--   0 dan       (1000) dan       (1000)     1785 2023-05-29 19:04:57.000000 pepmatch-0.9.4/test/test_mismatch.py
```

### Comparing `pepmatch-0.9.3/LICENSE` & `pepmatch-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pepmatch-0.9.3/PKG-INFO` & `pepmatch-0.9.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pepmatch
-Version: 0.9.3
+Version: 0.9.4
 Summary: Search tool for peptides and epitopes within a proteome, while considering potential residue substitutions.
 Home-page: https://github.com/IEDB/PEPMatch
 Author: Daniel Marrama
 Author-email: dmarrama@lji.org
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pepmatch-0.9.3/README.md` & `pepmatch-0.9.4/README.md`

 * *Files identical despite different names*

### Comparing `pepmatch-0.9.3/pepmatch/benchmarker.py` & `pepmatch-0.9.4/pepmatch/benchmarker.py`

 * *Files identical despite different names*

### Comparing `pepmatch-0.9.3/pepmatch/helpers.py` & `pepmatch-0.9.4/pepmatch/helpers.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,19 +31,19 @@
   Args: 
     record: protein SeqRecord from proteome FASTA file.
   """
   regexes = {
       'protein_id': re.compile(r"\|([^|]*)\|"),     # between | and |
       'protein_name': re.compile(r"\s(.+?)\sOS"),   # between space and space before OS
       'species': re.compile(r"OS=(.+?)\sOX"),       # between OS= and space before OX
-      'taxon_id': re.compile(r"OX=(.+?)\s"),        # between OX= and space
-      'gene': re.compile(r"GN=(.+?)\s"),            # between GN= and space
-      'pe_level': re.compile(r"PE=(.+?)\s"),        # between PE= and space
-      'sequence_version': re.compile(r"SV=(.+?)\s"),# between SV= and space
-      'gene_priority': re.compile(r"GP=(.+?)\s"),   # between GP= and space
+      'taxon_id': re.compile(r"OX=(.+?)(\s|$)"),         # between OX= and space
+      'gene': re.compile(r"GN=(.+?)(\s|$)"),             # between GN= and space
+      'pe_level': re.compile(r"PE=(.+?)(\s|$)"),         # between PE= and space
+      'sequence_version': re.compile(r"SV=(.+?)(\s|$)"), # between SV= and space
+      'gene_priority': re.compile(r"GP=(.+?)(\s|$)"),    # between GP= and space
   }
   metadata = []
   for key in regexes: # loop through compiled regexes to extract metadata
     match = regexes[key].search(str(record.description))
     
     if match:
       metadata.append(match.group(1))
```

### Comparing `pepmatch-0.9.3/pepmatch/matcher.py` & `pepmatch-0.9.4/pepmatch/matcher.py`

 * *Files 0% similar despite different names*

```diff
@@ -699,48 +699,58 @@
       
       # reset batched peptides
       self.batched_peptides = {0: self.query}
 
     return all_matches
 
   def discontinuous_search(self) -> list:
-    """Find matches for discontinuous epitopes."""
+    """Find matches for discontinuous epitopes. Loops through every protein
+    in the proteome and checks if the residues at the given positions match
+    the query epitope residues up to the maximum number of mismatches.
+    """
     all_matches = []
     for dis_epitope in self.discontinuous_epitopes:
+      match = False
       for protein_record in parse_fasta(self.proteome):
         try:
           residue_matches = sum(
             [x[0] == protein_record.seq[x[1] - 1] for x in dis_epitope]
           )
           if residue_matches >= (len(dis_epitope) - self.max_mismatches):
+            match = True
             metadata = extract_metadata(protein_record)
             match_data = (
               ', '.join(                                    # query epitope
                 [x[0] + str(x[1]) for x in dis_epitope]),
               ', '.join(                                    # matched epitope
                 [protein_record.seq[x[1] - 1] + str(x[1]) for x in dis_epitope]), 
               metadata[0],                                  # protein ID
               metadata[1],                                  # protein name
               metadata[2],                                  # species
               metadata[3],                                  # taxon ID
               metadata[4],                                  # gene symbol
               len(dis_epitope) - residue_matches,           # mismatches count
-                                                            # mutated positions
+              # mutated positions
               [x[1] for x in dis_epitope if x[0] != protein_record.seq[x[1] - 1]],
               dis_epitope[0][1],                            # index start
               dis_epitope[-1][1],                           # index end
               metadata[5],                                  # protein existence level
               metadata[6],                                  # sequence version
               metadata[7])                                  # gene priority flag
             
             all_matches.append(match_data)
         
         except IndexError:
           continue
-    
+
+      if not match:
+        all_matches.append(
+          (', '.join([x[0] + str(x[1]) for x in dis_epitope]),) + (np.nan,) * 13
+        )
+
     return all_matches
 
   def _dataframe_matches(self, all_matches: list) -> pd.DataFrame:
     """Return Pandas dataframe of the results.
     
     Args:
       all_matches: the list of all matches for all peptides.
@@ -853,9 +863,10 @@
 
   return args
 
 def run():
   args = parse_arguments()
 
   Matcher(args.query, args.proteome_file, args.max_mismatches, 
-          args.kmer_size, args.preprocessed_files_path, 
-          args.best_match, args.output_format, args.output_name).match()
+    args.kmer_size, args.preprocessed_files_path, 
+    args.best_match, args.output_format, args.output_name
+  ).match()
```

### Comparing `pepmatch-0.9.3/pepmatch/preprocessor.py` & `pepmatch-0.9.4/pepmatch/preprocessor.py`

 * *Files identical despite different names*

### Comparing `pepmatch-0.9.3/pepmatch.egg-info/PKG-INFO` & `pepmatch-0.9.4/pepmatch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pepmatch
-Version: 0.9.3
+Version: 0.9.4
 Summary: Search tool for peptides and epitopes within a proteome, while considering potential residue substitutions.
 Home-page: https://github.com/IEDB/PEPMatch
 Author: Daniel Marrama
 Author-email: dmarrama@lji.org
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pepmatch-0.9.3/setup.py` & `pepmatch-0.9.4/setup.py`

 * *Files identical despite different names*

### Comparing `pepmatch-0.9.3/test/test_best_match.py` & `pepmatch-0.9.4/test/test_best_match.py`

 * *Files identical despite different names*

### Comparing `pepmatch-0.9.3/test/test_discontinuous_search.py` & `pepmatch-0.9.4/test/test_discontinuous_search.py`

 * *Files 20% similar despite different names*

```diff
@@ -17,8 +17,8 @@
   df = Matcher(
     query=[
       'R377, Q408, Q432, H433, F436, V441, S442, S464, K467, K489, I491, S492, N497'],
     proteome_file=proteome_fasta,
     max_mismatches=0,
     output_format='dataframe').match()
 
-  assert df['Protein ID'].iloc[0] == 'P00533.1'
+  assert df['Protein ID'].iloc[0] == 'P00533.2'
```

### Comparing `pepmatch-0.9.3/test/test_exact_match.py` & `pepmatch-0.9.4/test/test_exact_match.py`

 * *Files identical despite different names*

### Comparing `pepmatch-0.9.3/test/test_mismatch.py` & `pepmatch-0.9.4/test/test_mismatch.py`

 * *Files identical despite different names*

