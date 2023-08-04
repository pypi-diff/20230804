# Comparing `tmp/pepsift-0.0.2.tar.gz` & `tmp/pepsift-0.0.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pepsift-0.0.2.tar", last modified: Fri Aug  4 14:10:51 2023, max compression
+gzip compressed data, was "pepsift-0.0.2.post1.tar", last modified: Fri Aug  4 14:13:42 2023, max compression
```

## Comparing `pepsift-0.0.2.tar` & `pepsift-0.0.2.post1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-08-04 14:10:51.401904 pepsift-0.0.2/
--rw-rw-rw-   0        0        0     1102 2023-03-28 08:39:04.000000 pepsift-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     4833 2023-08-04 14:10:51.402908 pepsift-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     4046 2023-06-15 07:35:45.000000 pepsift-0.0.2/README.md
--rw-rw-rw-   0        0        0     1126 2023-08-04 14:10:51.409922 pepsift-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      123 2023-02-15 14:15:02.000000 pepsift-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-04 14:10:51.361877 pepsift-0.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-08-04 14:10:51.382545 pepsift-0.0.2/src/pepsift/
--rw-rw-rw-   0        0        0      159 2023-08-04 14:09:49.000000 pepsift-0.0.2/src/pepsift/__init__.py
--rw-rw-rw-   0        0        0     1868 2023-04-05 06:10:20.000000 pepsift-0.0.2/src/pepsift/natural-aa.json
--rw-rw-rw-   0        0        0    12648 2023-08-04 13:56:29.000000 pepsift-0.0.2/src/pepsift/pepsift.py
--rw-rw-rw-   0        0        0     1613 2023-04-05 08:35:53.000000 pepsift-0.0.2/src/pepsift/utils.py
-drwxrwxrwx   0        0        0        0 2023-08-04 14:10:51.400904 pepsift-0.0.2/src/pepsift.egg-info/
--rw-rw-rw-   0        0        0     4833 2023-08-04 14:10:51.000000 pepsift-0.0.2/src/pepsift.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      328 2023-08-04 14:10:51.000000 pepsift-0.0.2/src/pepsift.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-04 14:10:51.000000 pepsift-0.0.2/src/pepsift.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       88 2023-08-04 14:10:51.000000 pepsift-0.0.2/src/pepsift.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-08-04 14:10:51.000000 pepsift-0.0.2/src/pepsift.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-08-04 14:10:51.401904 pepsift-0.0.2/tests/
--rw-rw-rw-   0        0        0    11109 2023-08-04 12:05:37.000000 pepsift-0.0.2/tests/test_pepsift.py
+drwxrwxrwx   0        0        0        0 2023-08-04 14:13:42.805058 pepsift-0.0.2.post1/
+-rw-rw-rw-   0        0        0     1102 2023-03-28 08:39:04.000000 pepsift-0.0.2.post1/LICENSE
+-rw-rw-rw-   0        0        0     4839 2023-08-04 14:13:42.805058 pepsift-0.0.2.post1/PKG-INFO
+-rw-rw-rw-   0        0        0     4046 2023-06-15 07:35:45.000000 pepsift-0.0.2.post1/README.md
+-rw-rw-rw-   0        0        0     1126 2023-08-04 14:13:42.810571 pepsift-0.0.2.post1/setup.cfg
+-rw-rw-rw-   0        0        0      123 2023-02-15 14:15:02.000000 pepsift-0.0.2.post1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-04 14:13:42.782906 pepsift-0.0.2.post1/src/
+drwxrwxrwx   0        0        0        0 2023-08-04 14:13:42.789970 pepsift-0.0.2.post1/src/pepsift/
+-rw-rw-rw-   0        0        0      165 2023-08-04 14:13:10.000000 pepsift-0.0.2.post1/src/pepsift/__init__.py
+-rw-rw-rw-   0        0        0     1868 2023-04-05 06:10:20.000000 pepsift-0.0.2.post1/src/pepsift/natural-aa.json
+-rw-rw-rw-   0        0        0    12559 2023-08-04 14:12:33.000000 pepsift-0.0.2.post1/src/pepsift/pepsift.py
+-rw-rw-rw-   0        0        0     1613 2023-04-05 08:35:53.000000 pepsift-0.0.2.post1/src/pepsift/utils.py
+drwxrwxrwx   0        0        0        0 2023-08-04 14:13:42.804056 pepsift-0.0.2.post1/src/pepsift.egg-info/
+-rw-rw-rw-   0        0        0     4839 2023-08-04 14:13:42.000000 pepsift-0.0.2.post1/src/pepsift.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      328 2023-08-04 14:13:42.000000 pepsift-0.0.2.post1/src/pepsift.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-04 14:13:42.000000 pepsift-0.0.2.post1/src/pepsift.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       88 2023-08-04 14:13:42.000000 pepsift-0.0.2.post1/src/pepsift.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-08-04 14:13:42.000000 pepsift-0.0.2.post1/src/pepsift.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-04 14:13:42.804056 pepsift-0.0.2.post1/tests/
+-rw-rw-rw-   0        0        0    11109 2023-08-04 12:05:37.000000 pepsift-0.0.2.post1/tests/test_pepsift.py
```

### Comparing `pepsift-0.0.2/LICENSE` & `pepsift-0.0.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `pepsift-0.0.2/PKG-INFO` & `pepsift-0.0.2.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pepsift
-Version: 0.0.2
+Version: 0.0.2.post1
 Summary: Identify peptides and derivatives from small molecule datasets
 Home-page: https://github.com/OlivierBeq/pepsift
 Author: Olivier J. M. Béquignon
 Author-email: "olivier.bequignon.maintainer@gmail.com"
 Maintainer: Olivier J. M. Béquignon
 Maintainer-email: "olivier.bequignon.maintainer@gmail.com"
 Keywords: peptides,cheminformatics,filtering
```

### Comparing `pepsift-0.0.2/README.md` & `pepsift-0.0.2.post1/README.md`

 * *Files identical despite different names*

### Comparing `pepsift-0.0.2/setup.cfg` & `pepsift-0.0.2.post1/setup.cfg`

 * *Files identical despite different names*

### Comparing `pepsift-0.0.2/src/pepsift/natural-aa.json` & `pepsift-0.0.2.post1/src/pepsift/natural-aa.json`

 * *Files identical despite different names*

### Comparing `pepsift-0.0.2/src/pepsift/pepsift.py` & `pepsift-0.0.2.post1/src/pepsift/pepsift.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,18 +73,15 @@
             mol.UpdatePropertyCache()
             _ = Chem.GetSymmSSSR(mol)
             prods = rxn.RunReactants((mol,))[0]
             for prod in prods:
                 prod.UpdatePropertyCache()
                 _ = Chem.GetSymmSSSR(prod)
             mol = AllChem.CombineMols(*prods)
-            try:
-                Chem.SanitizeMol(mol)
-            except:
-                print(Chem.MolToSmiles(mol))
+            Chem.SanitizeMol(mol)
         return mol
 
     @classmethod
     def _neutralize(cls, mol: Chem.Mol):
         """Neutralize a molecule by adding or removing atoms.
 
         Adapted by Vincent Scalfani to the RDKit from Noel O’Boyle’s nocharge code.
```

### Comparing `pepsift-0.0.2/src/pepsift/utils.py` & `pepsift-0.0.2.post1/src/pepsift/utils.py`

 * *Files identical despite different names*

### Comparing `pepsift-0.0.2/src/pepsift.egg-info/PKG-INFO` & `pepsift-0.0.2.post1/src/pepsift.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pepsift
-Version: 0.0.2
+Version: 0.0.2.post1
 Summary: Identify peptides and derivatives from small molecule datasets
 Home-page: https://github.com/OlivierBeq/pepsift
 Author: Olivier J. M. Béquignon
 Author-email: "olivier.bequignon.maintainer@gmail.com"
 Maintainer: Olivier J. M. Béquignon
 Maintainer-email: "olivier.bequignon.maintainer@gmail.com"
 Keywords: peptides,cheminformatics,filtering
```

### Comparing `pepsift-0.0.2/tests/test_pepsift.py` & `pepsift-0.0.2.post1/tests/test_pepsift.py`

 * *Files identical despite different names*

