# Comparing `tmp/cnmfsns-1.7.0.tar.gz` & `tmp/cnmfsns-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cnmfsns-1.7.0.tar", last modified: Mon Jul 31 21:04:29 2023, max compression
+gzip compressed data, was "cnmfsns-1.7.1.tar", last modified: Fri Aug  4 18:10:42 2023, max compression
```

## Comparing `cnmfsns-1.7.0.tar` & `cnmfsns-1.7.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 21:04:29.608713 cnmfsns-1.7.0/
--rw-rw-rw-   0        0        0     1090 2023-04-24 20:31:27.000000 cnmfsns-1.7.0/LICENSE
--rw-rw-rw-   0        0        0     4361 2023-07-31 21:04:29.608713 cnmfsns-1.7.0/PKG-INFO
--rw-rw-rw-   0        0        0     3846 2023-07-31 21:01:55.000000 cnmfsns-1.7.0/README.md
--rw-rw-rw-   0        0        0       86 2023-04-24 20:31:27.000000 cnmfsns-1.7.0/pyproject.toml
--rw-rw-rw-   0        0        0      980 2023-07-31 21:04:29.609714 cnmfsns-1.7.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-31 21:04:29.560163 cnmfsns-1.7.0/src/
-drwxrwxrwx   0        0        0        0 2023-07-31 21:04:29.579732 cnmfsns-1.7.0/src/cnmfsns/
--rw-rw-rw-   0        0        0      513 2023-05-12 18:06:16.000000 cnmfsns-1.7.0/src/cnmfsns/__init__.py
--rw-rw-rw-   0        0        0    52741 2023-07-31 21:02:15.000000 cnmfsns-1.7.0/src/cnmfsns/cli.py
--rw-rw-rw-   0        0        0    39682 2023-07-24 22:05:31.000000 cnmfsns-1.7.0/src/cnmfsns/cnmf.py
--rw-rw-rw-   0        0        0    16061 2023-04-24 20:31:27.000000 cnmfsns-1.7.0/src/cnmfsns/colors.py
--rw-rw-rw-   0        0        0     3204 2023-07-31 19:07:44.000000 cnmfsns-1.7.0/src/cnmfsns/config.py
--rw-rw-rw-   0        0        0    36443 2023-07-31 19:07:55.000000 cnmfsns-1.7.0/src/cnmfsns/dataset.py
--rw-rw-rw-   0        0        0    22552 2023-07-31 20:58:13.000000 cnmfsns-1.7.0/src/cnmfsns/integration.py
--rw-rw-rw-   0        0        0    62028 2023-07-31 20:59:13.000000 cnmfsns-1.7.0/src/cnmfsns/plots.py
--rw-rw-rw-   0        0        0    41881 2023-07-28 20:18:37.000000 cnmfsns-1.7.0/src/cnmfsns/sns.py
--rw-rw-rw-   0        0        0     2767 2023-07-10 02:54:46.000000 cnmfsns-1.7.0/src/cnmfsns/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-31 21:04:29.607714 cnmfsns-1.7.0/src/cnmfsns.egg-info/
--rw-rw-rw-   0        0        0     4361 2023-07-31 21:04:29.000000 cnmfsns-1.7.0/src/cnmfsns.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      472 2023-07-31 21:04:29.000000 cnmfsns-1.7.0/src/cnmfsns.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 21:04:29.000000 cnmfsns-1.7.0/src/cnmfsns.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-07-31 21:04:29.000000 cnmfsns-1.7.0/src/cnmfsns.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      189 2023-07-31 21:04:29.000000 cnmfsns-1.7.0/src/cnmfsns.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-31 21:04:29.000000 cnmfsns-1.7.0/src/cnmfsns.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-04 18:10:42.788743 cnmfsns-1.7.1/
+-rw-rw-rw-   0        0        0     1090 2023-04-24 20:31:27.000000 cnmfsns-1.7.1/LICENSE
+-rw-rw-rw-   0        0        0     4361 2023-08-04 18:10:42.788743 cnmfsns-1.7.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3846 2023-08-04 18:10:00.000000 cnmfsns-1.7.1/README.md
+-rw-rw-rw-   0        0        0       86 2023-04-24 20:31:27.000000 cnmfsns-1.7.1/pyproject.toml
+-rw-rw-rw-   0        0        0      980 2023-08-04 18:10:42.791745 cnmfsns-1.7.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-04 18:10:42.690036 cnmfsns-1.7.1/src/
+drwxrwxrwx   0        0        0        0 2023-08-04 18:10:42.742529 cnmfsns-1.7.1/src/cnmfsns/
+-rw-rw-rw-   0        0        0      513 2023-05-12 18:06:16.000000 cnmfsns-1.7.1/src/cnmfsns/__init__.py
+-rw-rw-rw-   0        0        0    52741 2023-08-02 21:16:19.000000 cnmfsns-1.7.1/src/cnmfsns/cli.py
+-rw-rw-rw-   0        0        0    39682 2023-07-24 22:05:31.000000 cnmfsns-1.7.1/src/cnmfsns/cnmf.py
+-rw-rw-rw-   0        0        0    16061 2023-08-04 17:48:43.000000 cnmfsns-1.7.1/src/cnmfsns/colors.py
+-rw-rw-rw-   0        0        0     3204 2023-07-31 19:07:44.000000 cnmfsns-1.7.1/src/cnmfsns/config.py
+-rw-rw-rw-   0        0        0    36570 2023-08-04 18:07:59.000000 cnmfsns-1.7.1/src/cnmfsns/dataset.py
+-rw-rw-rw-   0        0        0    22552 2023-07-31 20:58:13.000000 cnmfsns-1.7.1/src/cnmfsns/integration.py
+-rw-rw-rw-   0        0        0    63702 2023-08-04 18:08:04.000000 cnmfsns-1.7.1/src/cnmfsns/plots.py
+-rw-rw-rw-   0        0        0    41881 2023-07-28 20:18:37.000000 cnmfsns-1.7.1/src/cnmfsns/sns.py
+-rw-rw-rw-   0        0        0     2767 2023-07-10 02:54:46.000000 cnmfsns-1.7.1/src/cnmfsns/utils.py
+drwxrwxrwx   0        0        0        0 2023-08-04 18:10:42.787745 cnmfsns-1.7.1/src/cnmfsns.egg-info/
+-rw-rw-rw-   0        0        0     4361 2023-08-04 18:10:42.000000 cnmfsns-1.7.1/src/cnmfsns.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      472 2023-08-04 18:10:42.000000 cnmfsns-1.7.1/src/cnmfsns.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-04 18:10:42.000000 cnmfsns-1.7.1/src/cnmfsns.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-08-04 18:10:42.000000 cnmfsns-1.7.1/src/cnmfsns.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      189 2023-08-04 18:10:42.000000 cnmfsns-1.7.1/src/cnmfsns.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-08-04 18:10:42.000000 cnmfsns-1.7.1/src/cnmfsns.egg-info/top_level.txt
```

### Comparing `cnmfsns-1.7.0/LICENSE` & `cnmfsns-1.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cnmfsns-1.7.0/PKG-INFO` & `cnmfsns-1.7.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cnmfsns
-Version: 1.7.0
+Version: 1.7.1
 Summary: cNMF Solution Network Space
 Home-page: https://github.com/MorrissyLab/cNMF-SNS
 Author: Ted Verhey
 Author-email: tbverhey@ucalgary.ca
 Project-URL: Bug Tracker, https://github.com/MorrissyLab/cNMF-SNS/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -16,15 +16,15 @@
 
 ![cNMF-SNS logo](logo.png)
 
 -----------------
 
 # cNMF-SNS: powerful factorization-based multi-omics integration toolkit
 
-![version badge](https://img.shields.io/badge/version-1.7.0-blue)
+![version badge](https://img.shields.io/badge/version-1.7.1-blue)
 [![PyPI Latest Release](https://img.shields.io/pypi/v/cnmfsns.svg)](https://pypi.org/project/cnmfsns/)
 [![Conda Latest Release](https://img.shields.io/conda/vn/conda-forge/cnmfsns)](https://anaconda.org/conda-forge/cnmfsns/)
 [![Documentation status](https://readthedocs.org/projects/cnmf-sns/badge/?version=latest&style=flat)]()
 [![Downloads](https://static.pepy.tech/badge/cnmfsns)](https://pepy.tech/project/cnmfsns)
 [![License](https://img.shields.io/pypi/l/cnmfsns.svg)](https://github.com/MorrissyLab/cNMF-SNS/blob/main/LICENSE)
 
 Authors: [Ted Verhey](https://github.com/verheytb), [Heewon Seo](https://github.com/lootpiz), [Sorana Morrissy](https://github.com/ancasorana)
```

### Comparing `cnmfsns-1.7.0/README.md` & `cnmfsns-1.7.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 00000040: 2070 6f77 6572 6675 6c20 6661 6374 6f72   powerful factor
 00000050: 697a 6174 696f 6e2d 6261 7365 6420 6d75  ization-based mu
 00000060: 6c74 692d 6f6d 6963 7320 696e 7465 6772  lti-omics integr
 00000070: 6174 696f 6e20 746f 6f6c 6b69 740d 0a0d  ation toolkit...
 00000080: 0a21 5b76 6572 7369 6f6e 2062 6164 6765  .![version badge
 00000090: 5d28 6874 7470 733a 2f2f 696d 672e 7368  ](https://img.sh
 000000a0: 6965 6c64 732e 696f 2f62 6164 6765 2f76  ields.io/badge/v
-000000b0: 6572 7369 6f6e 2d31 2e37 2e30 2d62 6c75  ersion-1.7.0-blu
+000000b0: 6572 7369 6f6e 2d31 2e37 2e31 2d62 6c75  ersion-1.7.1-blu
 000000c0: 6529 0d0a 5b21 5b50 7950 4920 4c61 7465  e)..[![PyPI Late
 000000d0: 7374 2052 656c 6561 7365 5d28 6874 7470  st Release](http
 000000e0: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
 000000f0: 696f 2f70 7970 692f 762f 636e 6d66 736e  io/pypi/v/cnmfsn
 00000100: 732e 7376 6729 5d28 6874 7470 733a 2f2f  s.svg)](https://
 00000110: 7079 7069 2e6f 7267 2f70 726f 6a65 6374  pypi.org/project
 00000120: 2f63 6e6d 6673 6e73 2f29 0d0a 5b21 5b43  /cnmfsns/)..[![C
```

### Comparing `cnmfsns-1.7.0/setup.cfg` & `cnmfsns-1.7.1/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2063 6e6d 6673 6e73 0d0a 7665 7273   = cnmfsns..vers
-00000020: 696f 6e20 3d20 312e 372e 300d 0a61 7574  ion = 1.7.0..aut
+00000020: 696f 6e20 3d20 312e 372e 310d 0a61 7574  ion = 1.7.1..aut
 00000030: 686f 7220 3d20 5465 6420 5665 7268 6579  hor = Ted Verhey
 00000040: 0d0a 6175 7468 6f72 5f65 6d61 696c 203d  ..author_email =
 00000050: 2074 6276 6572 6865 7940 7563 616c 6761   tbverhey@ucalga
 00000060: 7279 2e63 610d 0a64 6573 6372 6970 7469  ry.ca..descripti
 00000070: 6f6e 203d 2063 4e4d 4620 536f 6c75 7469  on = cNMF Soluti
 00000080: 6f6e 204e 6574 776f 726b 2053 7061 6365  on Network Space
 00000090: 0d0a 6c6f 6e67 5f64 6573 6372 6970 7469  ..long_descripti
```

### Comparing `cnmfsns-1.7.0/src/cnmfsns/__init__.py` & `cnmfsns-1.7.1/src/cnmfsns/__init__.py`

 * *Files identical despite different names*

### Comparing `cnmfsns-1.7.0/src/cnmfsns/cli.py` & `cnmfsns-1.7.1/src/cnmfsns/cli.py`

 * *Files identical despite different names*

### Comparing `cnmfsns-1.7.0/src/cnmfsns/cnmf.py` & `cnmfsns-1.7.1/src/cnmfsns/cnmf.py`

 * *Files identical despite different names*

### Comparing `cnmfsns-1.7.0/src/cnmfsns/colors.py` & `cnmfsns-1.7.1/src/cnmfsns/colors.py`

 * *Files identical despite different names*

### Comparing `cnmfsns-1.7.0/src/cnmfsns/config.py` & `cnmfsns-1.7.1/src/cnmfsns/config.py`

 * *Files identical despite different names*

### Comparing `cnmfsns-1.7.0/src/cnmfsns/dataset.py` & `cnmfsns-1.7.1/src/cnmfsns/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -497,1782 +497,1790 @@
 00001f00: 2020 2020 2020 203a 7265 7475 726e 3a20         :return: 
 00001f10: 5472 7565 2069 6620 6461 7461 7365 7420  True if dataset 
 00001f20: 636f 6e74 6169 6e73 206e 6f72 6d61 6c69  contains normali
 00001f30: 7a65 6420 6461 7461 2c20 4661 6c73 6520  zed data, False 
 00001f40: 6966 2069 7420 6973 2072 6177 2064 6174  if it is raw dat
 00001f50: 612e 0d0a 2020 2020 2020 2020 3a72 7479  a...        :rty
 00001f60: 7065 3a20 626f 6f6c 0d0a 2020 2020 2020  pe: bool..      
-00001f70: 2020 2222 220d 0a20 2020 2020 2020 2072    """..        r
-00001f80: 6574 7572 6e20 7365 6c66 2e61 6461 7461  eturn self.adata
-00001f90: 2e75 6e73 5b22 7061 7469 656e 745f 6964  .uns["patient_id
-00001fa0: 5f63 6f6c 225d 0d0a 2020 2020 0d0a 2020  _col"]..    ..  
-00001fb0: 2020 4070 6174 6965 6e74 5f69 645f 636f    @patient_id_co
-00001fc0: 6c2e 7365 7474 6572 0d0a 2020 2020 6465  l.setter..    de
-00001fd0: 6620 7061 7469 656e 745f 6964 5f63 6f6c  f patient_id_col
-00001fe0: 2873 656c 662c 2076 616c 7565 3a20 7374  (self, value: st
-00001ff0: 7229 3a0d 0a20 2020 2020 2020 200d 0a20  r):..        .. 
-00002000: 2020 2020 2020 2069 6620 7661 6c75 6520         if value 
-00002010: 6973 206e 6f74 204e 6f6e 6520 616e 6420  is not None and 
-00002020: 7661 6c75 6520 6e6f 7420 696e 2073 656c  value not in sel
-00002030: 662e 6164 6174 612e 6f62 732e 636f 6c75  f.adata.obs.colu
-00002040: 6d6e 733a 0d0a 2020 2020 2020 2020 2020  mns:..          
-00002050: 2020 6176 6169 6c5f 636f 6c75 6d6e 7320    avail_columns 
-00002060: 3d20 222c 2022 2e6a 6f69 6e28 7365 6c66  = ", ".join(self
-00002070: 2e61 6461 7461 2e6f 6273 2e63 6f6c 756d  .adata.obs.colum
-00002080: 6e73 290d 0a20 2020 2020 2020 2020 2020  ns)..           
-00002090: 2072 6169 7365 2056 616c 7565 4572 726f   raise ValueErro
-000020a0: 7228 6622 7b76 616c 7565 7d20 6973 206e  r(f"{value} is n
-000020b0: 6f74 2061 2076 616c 6964 2063 6f6c 756d  ot a valid colum
-000020c0: 6e20 696e 2074 6865 206d 6574 6164 6174  n in the metadat
-000020d0: 6120 6d61 7472 6978 2e20 4176 6169 6c61  a matrix. Availa
-000020e0: 626c 6520 636f 6c75 6d6e 7320 6172 653a  ble columns are:
-000020f0: 207b 6176 6169 6c5f 636f 6c75 6d6e 737d   {avail_columns}
-00002100: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
-00002110: 2e61 6461 7461 2e75 6e73 5b22 7061 7469  .adata.uns["pati
-00002120: 656e 745f 6964 5f63 6f6c 225d 203d 2076  ent_id_col"] = v
-00002130: 616c 7565 0d0a 0d0a 2020 2020 4070 726f  alue....    @pro
-00002140: 7065 7274 790d 0a20 2020 2064 6566 2063  perty..    def c
-00002150: 6e6d 6673 6e73 5f76 6572 7369 6f6e 2873  nmfsns_version(s
-00002160: 656c 6629 3a0d 0a20 2020 2020 2020 2022  elf):..        "
-00002170: 2222 634e 4d46 2d53 4e53 2076 6572 7369  ""cNMF-SNS versi
-00002180: 6f6e 2075 7365 6420 746f 2063 7265 6174  on used to creat
-00002190: 6520 7468 6520 6461 7461 7365 740d 0a0d  e the dataset...
-000021a0: 0a20 2020 2020 2020 203a 7265 7475 726e  .        :return
-000021b0: 3a20 7665 7273 696f 6e0d 0a20 2020 2020  : version..     
-000021c0: 2020 203a 7274 7970 653a 2073 7472 0d0a     :rtype: str..
-000021d0: 2020 2020 2020 2020 2222 220d 0a20 2020          """..   
-000021e0: 2020 2020 2069 6620 2263 6e6d 6673 6e73       if "cnmfsns
-000021f0: 5f76 6572 7369 6f6e 2220 696e 2073 656c  _version" in sel
-00002200: 662e 6164 6174 612e 756e 733a 0d0a 2020  f.adata.uns:..  
-00002210: 2020 2020 2020 2020 2020 7665 7273 696f            versio
-00002220: 6e20 3d20 7365 6c66 2e61 6461 7461 2e75  n = self.adata.u
-00002230: 6e73 5b22 636e 6d66 736e 735f 7665 7273  ns["cnmfsns_vers
-00002240: 696f 6e22 5d0d 0a20 2020 2020 2020 2065  ion"]..        e
-00002250: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
-00002260: 2020 7665 7273 696f 6e20 3d20 4e6f 6e65    version = None
-00002270: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-00002280: 2076 6572 7369 6f6e 0d0a 2020 2020 2020   version..      
-00002290: 2020 0d0a 2020 2020 4070 726f 7065 7274    ..    @propert
-000022a0: 790d 0a20 2020 2064 6566 2068 6173 5f63  y..    def has_c
-000022b0: 6e6d 665f 7265 7375 6c74 7328 7365 6c66  nmf_results(self
-000022c0: 293a 0d0a 2020 2020 2020 2020 2222 2254  ):..        """T
-000022d0: 6573 7420 666f 7220 7765 6874 6865 7220  est for wehther 
-000022e0: 4461 7461 7365 7420 636f 6e74 6169 6e73  Dataset contains
-000022f0: 2063 4e4d 4620 7265 7375 6c74 7320 666f   cNMF results fo
-00002300: 7220 7468 6520 6461 7461 7365 740d 0a0d  r the dataset...
-00002310: 0a20 2020 2020 2020 203a 7265 7475 726e  .        :return
-00002320: 3a20 5768 6574 6865 7220 636f 6d70 6c65  : Whether comple
-00002330: 7465 2063 4e4d 4620 7265 7375 6c74 7320  te cNMF results 
-00002340: 6172 6520 636f 6e74 6169 6e65 6420 666f  are contained fo
-00002350: 7220 6174 206c 6561 7374 2031 2072 616e  r at least 1 ran
-00002360: 6b20 286b 290d 0a20 2020 2020 2020 203a  k (k)..        :
-00002370: 7274 7970 653a 2062 6f6f 6c0d 0a20 2020  rtype: bool..   
-00002380: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
-00002390: 2020 6d61 7472 6978 5f63 6865 636b 7320    matrix_checks 
-000023a0: 3d20 5b0d 0a20 2020 2020 2020 2020 2020  = [..           
-000023b0: 2022 636e 6d66 5f75 7361 6765 2220 696e   "cnmf_usage" in
-000023c0: 2073 656c 662e 6164 6174 612e 6f62 736d   self.adata.obsm
-000023d0: 2c0d 0a20 2020 2020 2020 2020 2020 2022  ,..            "
-000023e0: 636e 6d66 5f67 6570 5f73 636f 7265 2220  cnmf_gep_score" 
-000023f0: 696e 2073 656c 662e 6164 6174 612e 7661  in self.adata.va
-00002400: 726d 2c0d 0a20 2020 2020 2020 2020 2020  rm,..           
-00002410: 2022 636e 6d66 5f67 6570 5f74 706d 2220   "cnmf_gep_tpm" 
-00002420: 696e 2073 656c 662e 6164 6174 612e 7661  in self.adata.va
-00002430: 726d 2c0d 0a20 2020 2020 2020 2020 2020  rm,..           
-00002440: 2022 636e 6d66 5f67 6570 5f72 6177 2220   "cnmf_gep_raw" 
-00002450: 696e 2073 656c 662e 6164 6174 612e 7661  in self.adata.va
-00002460: 726d 2c0d 0a20 2020 2020 2020 2020 2020  rm,..           
-00002470: 2022 6b76 616c 7322 2069 6e20 7365 6c66   "kvals" in self
-00002480: 2e61 6461 7461 2e75 6e73 0d0a 2020 2020  .adata.uns..    
-00002490: 2020 2020 5d0d 0a20 2020 2020 2020 2072      ]..        r
-000024a0: 6574 7572 6e20 616c 6c28 6d61 7472 6978  eturn all(matrix
-000024b0: 5f63 6865 636b 7329 0d0a 2020 2020 2020  _checks)..      
-000024c0: 2020 0d0a 2020 2020 4070 726f 7065 7274    ..    @propert
-000024d0: 790d 0a20 2020 2064 6566 206f 7665 7264  y..    def overd
-000024e0: 6973 7065 7273 6564 5f67 656e 6573 2873  ispersed_genes(s
-000024f0: 656c 6629 3a0d 0a20 2020 2020 2020 2022  elf):..        "
-00002500: 2222 4f76 6572 6469 7370 6572 7365 6420  ""Overdispersed 
-00002510: 6765 6e65 206c 6973 7420 7573 6564 2066  gene list used f
-00002520: 6f72 2063 4e4d 460d 0a0d 0a20 2020 2020  or cNMF....     
-00002530: 2020 203a 7265 7475 726e 3a20 6765 6e65     :return: gene
-00002540: 206c 6973 740d 0a20 2020 2020 2020 203a   list..        :
-00002550: 7274 7970 653a 206c 6973 740d 0a20 2020  rtype: list..   
-00002560: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
-00002570: 2020 7265 7475 726e 2073 656c 662e 6164    return self.ad
-00002580: 6174 612e 756e 735b 2267 656e 655f 6c69  ata.uns["gene_li
-00002590: 7374 225d 0d0a 0d0a 0d0a 2020 2020 4063  st"]......    @c
-000025a0: 6e6d 6673 6e73 5f76 6572 7369 6f6e 2e73  nmfsns_version.s
-000025b0: 6574 7465 720d 0a20 2020 2064 6566 2063  etter..    def c
-000025c0: 6e6d 6673 6e73 5f76 6572 7369 6f6e 2873  nmfsns_version(s
-000025d0: 656c 662c 2076 616c 7565 3a20 626f 6f6c  elf, value: bool
-000025e0: 293a 0d0a 2020 2020 2020 2020 7365 6c66  ):..        self
-000025f0: 2e61 6461 7461 2e75 6e73 5b22 636e 6d66  .adata.uns["cnmf
-00002600: 736e 735f 7665 7273 696f 6e22 5d20 3d20  sns_version"] = 
-00002610: 7661 6c75 650d 0a0d 0a20 2020 2020 2020  value....       
-00002620: 200d 0a20 2020 2064 6566 2075 7064 6174   ..    def updat
-00002630: 655f 6f62 7328 7365 6c66 2c20 6f62 7329  e_obs(self, obs)
-00002640: 3a0d 0a20 2020 2020 2020 2022 2222 5570  :..        """Up
-00002650: 6461 7465 2074 6865 206f 6273 6572 7661  date the observa
-00002660: 7469 6f6e 206d 6574 6164 6174 6120 7769  tion metadata wi
-00002670: 7468 2061 206e 6577 206d 6574 6164 6174  th a new metadat
-00002680: 6120 6d61 7472 6978 0d0a 0d0a 2020 2020  a matrix....    
-00002690: 2020 2020 3a70 6172 616d 206f 6273 3a20      :param obs: 
-000026a0: 416e 206f 6273 6572 7661 7469 6f6e 7320  An observations 
-000026b0: c397 206d 6574 6164 6174 6120 6d61 7472  .. metadata matr
-000026c0: 6978 2c20 6465 6661 756c 7473 2074 6f20  ix, defaults to 
-000026d0: 4e6f 6e65 0d0a 2020 2020 2020 2020 3a74  None..        :t
-000026e0: 7970 6520 6f62 733a 2060 7064 2e44 6174  ype obs: `pd.Dat
-000026f0: 6146 7261 6d65 602c 206f 7074 696f 6e61  aFrame`, optiona
-00002700: 6c0d 0a20 2020 2020 2020 2022 2222 0d0a  l..        """..
-00002710: 2020 2020 2020 2020 2320 636f 6e76 6572          # conver
-00002720: 7420 276f 626a 6563 7427 2064 7479 7065  t 'object' dtype
-00002730: 2074 6f20 6361 7465 676f 7269 6361 6c2c   to categorical,
-00002740: 2063 6f6e 7665 7274 696e 6720 626f 6f6c   converting bool
-00002750: 2076 616c 7565 7320 746f 2073 7472 696e   values to strin
-00002760: 6773 2061 7320 7468 6573 6520 6172 6520  gs as these are 
-00002770: 6e6f 7420 7375 7070 6f72 7465 6420 6279  not supported by
-00002780: 2041 6e6e 4461 7461 206f 6e2d 6469 736b   AnnData on-disk
-00002790: 2066 6f72 6d61 740d 0a20 2020 2020 2020   format..       
-000027a0: 2066 6f72 2063 6f6c 2069 6e20 6f62 732e   for col in obs.
-000027b0: 7365 6c65 6374 5f64 7479 7065 7328 696e  select_dtypes(in
-000027c0: 636c 7564 653d 2822 626f 6f6c 222c 2022  clude=("bool", "
-000027d0: 6f62 6a65 6374 2229 292e 636f 6c75 6d6e  object")).column
-000027e0: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
-000027f0: 6f62 735b 636f 6c5d 203d 206f 6273 5b63  obs[col] = obs[c
-00002800: 6f6c 5d2e 6173 7479 7065 2822 7374 7222  ol].astype("str"
-00002810: 292e 6173 7479 7065 2822 6361 7465 676f  ).astype("catego
-00002820: 7279 2229 0d0a 2020 2020 2020 2020 6d69  ry")..        mi
-00002830: 7373 696e 675f 7361 6d70 6c65 735f 696e  ssing_samples_in
-00002840: 5f58 203d 206f 6273 2e69 6e64 6578 2e64  _X = obs.index.d
-00002850: 6966 6665 7265 6e63 6528 7365 6c66 2e61  ifference(self.a
-00002860: 6461 7461 2e6f 6273 2e69 6e64 6578 292e  data.obs.index).
-00002870: 6173 7479 7065 2873 7472 292e 746f 5f6c  astype(str).to_l
-00002880: 6973 7428 290d 0a20 2020 2020 2020 2069  ist()..        i
-00002890: 6620 6d69 7373 696e 675f 7361 6d70 6c65  f missing_sample
-000028a0: 735f 696e 5f58 3a0d 0a20 2020 2020 2020  s_in_X:..       
-000028b0: 2020 2020 206c 6f67 6769 6e67 2e77 6172       logging.war
-000028c0: 6e69 6e67 2822 5468 6520 666f 6c6c 6f77  ning("The follow
-000028d0: 696e 6720 7361 6d70 6c65 7320 696e 2074  ing samples in t
-000028e0: 6865 206d 6574 6164 6174 6120 7765 7265  he metadata were
-000028f0: 206e 6f74 2070 7265 7365 6e74 2069 6e20   not present in 
-00002900: 7468 6520 6461 7461 2028 6061 6461 7461  the data (`adata
-00002910: 2e58 6029 3a5c 6e20 202d 2022 202b 2022  .X`):\n  - " + "
-00002920: 5c6e 2020 2d20 222e 6a6f 696e 286d 6973  \n  - ".join(mis
-00002930: 7369 6e67 5f73 616d 706c 6573 5f69 6e5f  sing_samples_in_
-00002940: 5829 290d 0a20 2020 2020 2020 206d 6973  X))..        mis
-00002950: 7369 6e67 5f73 616d 706c 6573 5f69 6e5f  sing_samples_in_
-00002960: 6d64 203d 2073 656c 662e 6164 6174 612e  md = self.adata.
-00002970: 6f62 732e 696e 6465 782e 6469 6666 6572  obs.index.differ
-00002980: 656e 6365 286f 6273 2e69 6e64 6578 292e  ence(obs.index).
-00002990: 6173 7479 7065 2873 7472 292e 746f 5f6c  astype(str).to_l
-000029a0: 6973 7428 290d 0a20 2020 2020 2020 2069  ist()..        i
-000029b0: 6620 6d69 7373 696e 675f 7361 6d70 6c65  f missing_sample
-000029c0: 735f 696e 5f6d 643a 0d0a 2020 2020 2020  s_in_md:..      
-000029d0: 2020 2020 2020 6c6f 6767 696e 672e 7761        logging.wa
-000029e0: 726e 696e 6728 2254 6865 2066 6f6c 6c6f  rning("The follo
-000029f0: 7769 6e67 2073 616d 706c 6573 2069 6e20  wing samples in 
-00002a00: 7468 6520 6461 7461 2028 6061 6461 7461  the data (`adata
-00002a10: 2e58 6029 2077 6572 6520 6162 7365 6e74  .X`) were absent
-00002a20: 2069 6e20 7468 6520 6d65 7461 6461 7461   in the metadata
-00002a30: 3a5c 6e20 202d 2022 202b 2022 5c6e 2020  :\n  - " + "\n  
-00002a40: 2d20 222e 6a6f 696e 286d 6973 7369 6e67  - ".join(missing
-00002a50: 5f73 616d 706c 6573 5f69 6e5f 6d64 2929  _samples_in_md))
-00002a60: 0d0a 2020 2020 2020 2020 7365 6c66 2e61  ..        self.a
-00002a70: 6461 7461 2e6f 6273 203d 206f 6273 2e72  data.obs = obs.r
-00002a80: 6569 6e64 6578 2873 656c 662e 6164 6174  eindex(self.adat
-00002a90: 612e 6f62 732e 696e 6465 7829 0d0a 2020  a.obs.index)..  
-00002aa0: 2020 0d0a 2020 2020 6465 6620 6765 745f    ..    def get_
-00002ab0: 6d65 7461 6461 7461 5f74 7970 655f 7375  metadata_type_su
-00002ac0: 6d6d 6172 7928 7365 6c66 293a 0d0a 2020  mmary(self):..  
-00002ad0: 2020 2020 2020 2222 2252 6574 7572 6e20        """Return 
-00002ae0: 6120 7072 696e 7461 626c 6520 7375 6d6d  a printable summ
-00002af0: 6172 7920 6f66 206d 6574 6164 6174 6120  ary of metadata 
-00002b00: 616e 6420 7661 6c75 6520 7479 7065 7320  and value types 
-00002b10: 666f 7220 6561 6368 206d 6574 6164 6174  for each metadat
-00002b20: 6120 6c61 7965 722e 0d0a 0d0a 2020 2020  a layer.....    
-00002b30: 2020 2020 3a72 6574 7572 6e3a 2053 756d      :return: Sum
-00002b40: 6d61 7279 206f 6620 6d65 7461 6461 7461  mary of metadata
-00002b50: 0d0a 2020 2020 2020 2020 3a72 7479 7065  ..        :rtype
-00002b60: 3a20 7374 720d 0a20 2020 2020 2020 2022  : str..        "
-00002b70: 2222 0d0a 2020 2020 2020 2020 6d73 6720  ""..        msg 
-00002b80: 3d20 2222 0d0a 2020 2020 2020 2020 666f  = ""..        fo
-00002b90: 7220 636f 6c20 696e 2073 656c 662e 6164  r col in self.ad
-00002ba0: 6174 612e 6f62 732e 636f 6c75 6d6e 733a  ata.obs.columns:
-00002bb0: 0d0a 2020 2020 2020 2020 2020 2020 6d73  ..            ms
-00002bc0: 6720 2b3d 2022 2020 2020 436f 6c75 6d6e  g += "    Column
-00002bd0: 3a20 2220 2b20 636f 6c20 2b20 225c 6e22  : " + col + "\n"
-00002be0: 0d0a 2020 2020 2020 2020 2020 2020 666f  ..            fo
-00002bf0: 7220 7661 6c75 655f 7479 7065 2c20 636f  r value_type, co
-00002c00: 756e 7420 696e 2073 656c 662e 6164 6174  unt in self.adat
-00002c10: 612e 6f62 735b 636f 6c5d 2e64 726f 706e  a.obs[col].dropn
-00002c20: 6128 292e 6d61 7028 7479 7065 292e 7661  a().map(type).va
-00002c30: 6c75 655f 636f 756e 7473 2829 2e69 7465  lue_counts().ite
-00002c40: 6d73 2829 3a0d 0a20 2020 2020 2020 2020  ms():..         
-00002c50: 2020 2020 2020 206d 7367 202b 3d20 6622         msg += f"
-00002c60: 2020 2020 2020 2020 7b76 616c 7565 5f74          {value_t
-00002c70: 7970 657d 3a20 7b63 6f75 6e74 7d5c 6e22  ype}: {count}\n"
-00002c80: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-00002c90: 206d 7367 0d0a 2020 2020 0d0a 2020 2020   msg..    ..    
-00002ca0: 6465 6620 7772 6974 655f 6835 6164 2873  def write_h5ad(s
-00002cb0: 656c 662c 0d0a 2020 2020 2020 2020 2020  elf,..          
-00002cc0: 2020 2020 2020 2020 2066 696c 656e 616d           filenam
-00002cd0: 653a 2073 7472 293a 0d0a 2020 2020 2020  e: str):..      
-00002ce0: 2020 2222 2257 7269 7465 2064 6174 6173    """Write datas
-00002cf0: 6574 2074 6f20 2e68 3561 6420 6669 6c65  et to .h5ad file
-00002d00: 2e0d 0a0d 0a20 2020 2020 2020 203a 7061  .....        :pa
-00002d10: 7261 6d20 6669 6c65 6e61 6d65 3a20 6669  ram filename: fi
-00002d20: 6c65 7061 7468 0d0a 2020 2020 2020 2020  lepath..        
-00002d30: 3a74 7970 6520 6669 6c65 6e61 6d65 3a20  :type filename: 
-00002d40: 7374 720d 0a20 2020 2020 2020 2022 2222  str..        """
-00002d50: 0d0a 2020 2020 2020 2020 6669 6c65 6e61  ..        filena
-00002d60: 6d65 203d 206f 732e 7061 7468 2e61 6273  me = os.path.abs
-00002d70: 7061 7468 2866 696c 656e 616d 6529 0d0a  path(filename)..
-00002d80: 2020 2020 2020 2020 6c6f 6767 696e 672e          logging.
-00002d90: 696e 666f 2866 2257 7269 7469 6e67 2074  info(f"Writing t
-00002da0: 6f20 7b66 696c 656e 616d 657d 2229 0d0a  o {filename}")..
-00002db0: 2020 2020 2020 2020 7365 6c66 2e61 6461          self.ada
-00002dc0: 7461 2e77 7269 7465 5f68 3561 6428 6669  ta.write_h5ad(fi
-00002dd0: 6c65 6e61 6d65 290d 0a20 2020 2020 2020  lename)..       
-00002de0: 206c 6f67 6769 6e67 2e69 6e66 6f28 6622   logging.info(f"
-00002df0: 446f 6e65 2229 0d0a 2020 2020 0d0a 2020  Done")..    ..  
-00002e00: 2020 6465 6620 746f 5f64 6628 7365 6c66    def to_df(self
-00002e10: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00002e20: 206e 6f72 6d61 6c69 7a65 643a 2062 6f6f   normalized: boo
-00002e30: 6c20 3d20 4661 6c73 6529 3a0d 0a20 2020  l = False):..   
-00002e40: 2020 2020 2022 2222 4765 7420 6461 7461       """Get data
-00002e50: 206d 6174 7269 7820 6173 2061 2060 7064   matrix as a `pd
-00002e60: 2e44 6174 6146 7261 6d65 600d 0a0d 0a20  .DataFrame`.... 
-00002e70: 2020 2020 2020 203a 7061 7261 6d20 6e6f         :param no
-00002e80: 726d 616c 697a 6564 3a20 5365 7420 7472  rmalized: Set tr
-00002e90: 7565 2066 6f72 2054 504d 206e 6f72 6d61  ue for TPM norma
-00002ea0: 6c69 7a65 6420 6f75 7470 7574 2c20 6465  lized output, de
-00002eb0: 6661 756c 7473 2074 6f20 4661 6c73 650d  faults to False.
-00002ec0: 0a20 2020 2020 2020 203a 7479 7065 206e  .        :type n
-00002ed0: 6f72 6d61 6c69 7a65 643a 2062 6f6f 6c2c  ormalized: bool,
-00002ee0: 206f 7074 696f 6e61 6c0d 0a20 2020 2020   optional..     
-00002ef0: 2020 203a 7265 7475 726e 3a20 6f62 7365     :return: obse
-00002f00: 7276 6174 696f 6e73 20c3 9720 7661 7269  rvations .. vari
-00002f10: 6162 6c65 7320 6461 7461 206d 6174 7269  ables data matri
-00002f20: 780d 0a20 2020 2020 2020 203a 7274 7970  x..        :rtyp
-00002f30: 653a 2070 642e 4461 7461 4672 616d 650d  e: pd.DataFrame.
-00002f40: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
-00002f50: 2020 2020 2020 6466 203d 2073 656c 662e        df = self.
-00002f60: 6164 6174 612e 746f 5f64 6628 290d 0a20  adata.to_df().. 
-00002f70: 2020 2020 2020 2069 6620 6e6f 726d 616c         if normal
-00002f80: 697a 6564 2061 6e64 206e 6f74 2073 656c  ized and not sel
-00002f90: 662e 6973 5f6e 6f72 6d61 6c69 7a65 643a  f.is_normalized:
-00002fa0: 0d0a 2020 2020 2020 2020 2020 2020 6466  ..            df
-00002fb0: 203d 2064 662e 6469 7628 6466 2e73 756d   = df.div(df.sum
-00002fc0: 2861 7869 733d 3129 2c20 6178 6973 3d30  (axis=1), axis=0
-00002fd0: 2920 2a20 3165 3620 2023 2054 504d 206e  ) * 1e6  # TPM n
-00002fe0: 6f72 6d61 6c69 7a61 7469 6f6e 0d0a 2020  ormalization..  
-00002ff0: 2020 2020 2020 7265 7475 726e 2064 660d        return df.
-00003000: 0a20 2020 2020 2020 200d 0a20 2020 2064  .        ..    d
-00003010: 6566 2072 656d 6f76 655f 756e 6661 6374  ef remove_unfact
-00003020: 6f72 697a 6162 6c65 5f67 656e 6573 2873  orizable_genes(s
-00003030: 656c 6629 3a0d 0a20 2020 2020 2020 2022  elf):..        "
-00003040: 2222 5265 6d6f 7665 7320 6765 6e65 7320  ""Removes genes 
-00003050: 7769 7468 206d 6973 7369 6e67 2076 616c  with missing val
-00003060: 7565 7320 6f72 207a 6572 6f20 7661 7269  ues or zero vari
-00003070: 616e 6365 2066 726f 6d20 7468 6520 6461  ance from the da
-00003080: 7461 206d 6174 7269 782e 0d0a 2020 2020  ta matrix...    
-00003090: 2020 2020 2222 220d 0a20 2020 2020 2020      """..       
-000030a0: 2064 6620 3d20 7365 6c66 2e74 6f5f 6466   df = self.to_df
-000030b0: 286e 6f72 6d61 6c69 7a65 643d 4661 6c73  (normalized=Fals
-000030c0: 6529 0d0a 2020 2020 2020 2020 2320 4368  e)..        # Ch
-000030d0: 6563 6b20 666f 7220 7661 7269 6162 6c65  eck for variable
-000030e0: 7320 7769 7468 206d 6973 7369 6e67 2076  s with missing v
-000030f0: 616c 7565 730d 0a20 2020 2020 2020 2067  alues..        g
-00003100: 656e 6573 5f77 6974 685f 6d69 7373 696e  enes_with_missin
-00003110: 6776 616c 7565 7320 3d20 6466 2e69 736e  gvalues = df.isn
-00003120: 756c 6c28 292e 616e 7928 290d 0a20 2020  ull().any()..   
-00003130: 2020 2020 200d 0a20 2020 2020 2020 2069       ..        i
-00003140: 6620 6765 6e65 735f 7769 7468 5f6d 6973  f genes_with_mis
-00003150: 7369 6e67 7661 6c75 6573 2e61 6e79 2829  singvalues.any()
-00003160: 3a0d 0a20 2020 2020 2020 2020 2020 206e  :..            n
-00003170: 5f6d 6973 7369 6e67 203d 2067 656e 6573  _missing = genes
-00003180: 5f77 6974 685f 6d69 7373 696e 6776 616c  _with_missingval
-00003190: 7565 732e 7375 6d28 290d 0a20 2020 2020  ues.sum()..     
-000031a0: 2020 2020 2020 206c 6f67 6769 6e67 2e77         logging.w
-000031b0: 6172 6e69 6e67 2866 227b 6e5f 6d69 7373  arning(f"{n_miss
-000031c0: 696e 677d 206f 6620 7b73 656c 662e 6164  ing} of {self.ad
-000031d0: 6174 612e 6e5f 7661 7273 7d20 7661 7269  ata.n_vars} vari
-000031e0: 6162 6c65 7320 6172 6520 6d69 7373 696e  ables are missin
-000031f0: 6720 7661 6c75 6573 2028 6061 6461 7461  g values (`adata
-00003200: 2e58 6029 2e22 290d 0a20 2020 2020 2020  .X`).")..       
-00003210: 2020 2020 206c 6f67 6769 6e67 2e77 6172       logging.war
-00003220: 6e69 6e67 2866 2253 7562 7365 7474 696e  ning(f"Subsettin
-00003230: 6720 7661 7269 6162 6c65 7320 746f 2074  g variables to t
-00003240: 686f 7365 2077 6974 6820 6e6f 206d 6973  hose with no mis
-00003250: 7369 6e67 2076 616c 7565 732e 2229 0d0a  sing values.")..
-00003260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003270: 0d0a 2020 2020 2020 2020 2320 4368 6563  ..        # Chec
-00003280: 6b20 666f 7220 6765 6e65 7320 7769 7468  k for genes with
-00003290: 207a 6572 6f20 7661 7269 616e 6365 0d0a   zero variance..
-000032a0: 2020 2020 2020 2020 7a65 726f 7661 7267          zerovarg
-000032b0: 656e 6573 203d 2028 6466 2e76 6172 2829  enes = (df.var()
-000032c0: 203d 3d20 3029 0d0a 2020 2020 2020 2020   == 0)..        
-000032d0: 6966 207a 6572 6f76 6172 6765 6e65 732e  if zerovargenes.
-000032e0: 616e 7928 293a 0d0a 2020 2020 2020 2020  any():..        
-000032f0: 2020 2020 6e5f 7a65 726f 7661 7220 3d20      n_zerovar = 
-00003300: 7a65 726f 7661 7267 656e 6573 2e73 756d  zerovargenes.sum
-00003310: 2829 0d0a 2020 2020 2020 2020 2020 2020  ()..            
-00003320: 6c6f 6767 696e 672e 7761 726e 696e 6728  logging.warning(
-00003330: 6622 7b6e 5f7a 6572 6f76 6172 7d20 6f66  f"{n_zerovar} of
-00003340: 207b 7365 6c66 2e61 6461 7461 2e6e 5f76   {self.adata.n_v
-00003350: 6172 737d 2076 6172 6961 626c 6573 2068  ars} variables h
-00003360: 6176 6520 6120 7661 7269 616e 6365 206f  ave a variance o
-00003370: 6620 7a65 726f 2069 6e20 636f 756e 7473  f zero in counts
-00003380: 2064 6174 6120 2860 6164 6174 612e 7261   data (`adata.ra
-00003390: 772e 5860 292e 2229 0d0a 2020 2020 2020  w.X`).")..      
-000033a0: 2020 2020 2020 6c6f 6767 696e 672e 7761        logging.wa
-000033b0: 726e 696e 6728 6622 5375 6273 6574 7469  rning(f"Subsetti
-000033c0: 6e67 2076 6172 6961 626c 6573 2074 6f20  ng variables to 
-000033d0: 7468 6f73 6520 7769 7468 206e 6f6e 7a65  those with nonze
-000033e0: 726f 2076 6172 6961 6e63 652e 2229 0d0a  ro variance.")..
-000033f0: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-00003400: 2020 6765 6e65 735f 746f 5f6b 6565 7020    genes_to_keep 
-00003410: 3d20 287e 6765 6e65 735f 7769 7468 5f6d  = (~genes_with_m
-00003420: 6973 7369 6e67 7661 6c75 6573 2920 2620  issingvalues) & 
-00003430: 287e 7a65 726f 7661 7267 656e 6573 290d  (~zerovargenes).
-00003440: 0a20 2020 2020 2020 200d 0a20 2020 2020  .        ..     
-00003450: 2020 2073 656c 662e 6164 6174 6120 3d20     self.adata = 
-00003460: 7365 6c66 2e61 6461 7461 5b3a 2c67 656e  self.adata[:,gen
-00003470: 6573 5f74 6f5f 6b65 6570 5d0d 0a0d 0a20  es_to_keep].... 
-00003480: 2020 2064 6566 2063 6f6d 7075 7465 5f67     def compute_g
-00003490: 656e 655f 7374 6174 7328 7365 6c66 2c20  ene_stats(self, 
-000034a0: 6f64 675f 6465 6661 756c 745f 7370 6c69  odg_default_spli
-000034b0: 6e65 5f64 6567 7265 653a 2069 6e74 203d  ne_degree: int =
-000034c0: 2033 2c20 6f64 675f 6465 6661 756c 745f   3, odg_default_
-000034d0: 646f 663a 2069 6e74 203d 2038 293a 0d0a  dof: int = 8):..
-000034e0: 2020 2020 2020 2020 2222 220d 0a20 2020          """..   
-000034f0: 2020 2020 2043 6f6d 7075 7465 7320 6765       Computes ge
-00003500: 6e65 2073 7461 7469 7374 6963 7320 616e  ne statistics an
-00003510: 6420 6669 7473 2074 776f 206d 6f64 656c  d fits two model
-00003520: 7320 6f66 206d 6561 6e20 616e 6420 7661  s of mean and va
-00003530: 7269 616e 6365 206f 6620 6765 6e65 7320  riance of genes 
-00003540: 696e 2074 6865 2064 6174 6173 6574 2e20  in the dataset. 
-00003550: 5468 6520 6669 7273 7420 6d65 7468 6f64  The first method
-00003560: 2069 7320 7468 650d 0a20 2020 2020 2020   is the..       
-00003570: 2067 656e 6572 616c 697a 6564 2061 6464   generalized add
-00003580: 6974 6976 6520 6d6f 6465 6c20 7769 7468  itive model with
-00003590: 2073 6d6f 6f74 6820 636f 6d70 6f6e 656e   smooth componen
-000035a0: 7473 2028 422d 7370 6c69 6e65 7329 2074  ts (B-splines) t
-000035b0: 6f20 6d6f 6465 6c20 7468 6520 7265 6c61  o model the rela
-000035c0: 7469 6f6e 7368 6970 206f 6620 6d65 616e  tionship of mean
-000035d0: 2061 6e64 2076 6172 6961 6e63 650d 0a20   and variance.. 
-000035e0: 2020 2020 2020 2062 6574 7765 656e 2067         between g
-000035f0: 656e 6573 2069 6e20 7468 6520 6461 7461  enes in the data
-00003600: 7365 742e 2049 7420 7072 6f64 7563 6573  set. It produces
-00003610: 2061 6e20 6f64 7363 6f72 6520 6d65 7472   an odscore metr
-00003620: 6963 2066 6f72 206f 7665 7264 6973 7065  ic for overdispe
-00003630: 7273 696f 6e2e 2054 6865 2073 6563 6f6e  rsion. The secon
-00003640: 6420 6973 2074 6865 2063 6f75 6e74 2d73  d is the count-s
-00003650: 7461 7469 7374 6963 730d 0a20 2020 2020  tatistics..     
-00003660: 2020 206d 6574 686f 6420 666f 756e 6420     method found 
-00003670: 696e 2074 6865 2063 4e4d 4620 7061 636b  in the cNMF pack
-00003680: 6167 652c 2077 6869 6368 2070 726f 6475  age, which produ
-00003690: 6365 7320 6120 6d6f 6469 6669 6564 2076  ces a modified v
-000036a0: 2d73 636f 7265 206d 6574 7269 632e 2041  -score metric. A
-000036b0: 6c6c 2067 656e 6520 7374 6174 6973 7469  ll gene statisti
-000036c0: 6373 2061 7265 2073 746f 7265 6420 7769  cs are stored wi
-000036d0: 7468 696e 2074 6865 0d0a 2020 2020 2020  thin the..      
-000036e0: 2020 6461 7461 7365 7420 6f62 6a65 6374    dataset object
-000036f0: 2061 6e64 2061 7265 2061 6363 6573 7369   and are accessi
-00003700: 626c 6520 7573 696e 6720 6064 6174 6173  ble using `datas
-00003710: 6574 2e61 6e6e 6461 7461 2e76 6172 602e  et.anndata.var`.
-00003720: 0d0a 0d0a 2020 2020 2020 2020 3a70 6172  ....        :par
-00003730: 616d 206f 6467 5f64 6566 6175 6c74 5f73  am odg_default_s
-00003740: 706c 696e 655f 6465 6772 6565 3a20 422d  pline_degree: B-
-00003750: 5370 6c69 6e65 2064 6567 7265 6520 666f  Spline degree fo
-00003760: 7220 474c 4d2d 4741 4d20 6d6f 6465 6c6c  r GLM-GAM modell
-00003770: 696e 6720 6f66 206d 6561 6e2d 7661 7269  ing of mean-vari
-00003780: 616e 6365 2072 656c 6174 696f 6e73 6869  ance relationshi
-00003790: 702c 2064 6566 6175 6c74 7320 746f 2033  p, defaults to 3
-000037a0: 0d0a 2020 2020 2020 2020 3a74 7970 6520  ..        :type 
-000037b0: 6f64 675f 6465 6661 756c 745f 7370 6c69  odg_default_spli
-000037c0: 6e65 5f64 6567 7265 653a 2069 6e74 2c20  ne_degree: int, 
-000037d0: 6f70 7469 6f6e 616c 0d0a 2020 2020 2020  optional..      
-000037e0: 2020 3a70 6172 616d 206f 6467 5f64 6566    :param odg_def
-000037f0: 6175 6c74 5f64 6f66 3a20 4465 6772 6565  ault_dof: Degree
-00003800: 7320 6f66 2066 7265 6564 6f6d 2066 6f72  s of freedom for
-00003810: 2047 4c4d 2d47 414d 206d 6f64 656c 6c69   GLM-GAM modelli
-00003820: 6e67 206f 6620 6d65 616e 2d76 6172 616e  ng of mean-varan
-00003830: 6365 2c20 6465 6661 756c 7473 2074 6f20  ce, defaults to 
-00003840: 380d 0a20 2020 2020 2020 203a 7479 7065  8..        :type
-00003850: 206f 6467 5f64 6566 6175 6c74 5f64 6f66   odg_default_dof
-00003860: 3a20 696e 742c 206f 7074 696f 6e61 6c0d  : int, optional.
-00003870: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
-00003880: 2020 2020 2020 6461 7461 5f72 6177 203d        data_raw =
-00003890: 2073 656c 662e 746f 5f64 6628 290d 0a20   self.to_df().. 
-000038a0: 2020 2020 2020 2064 6174 615f 6e6f 726d         data_norm
-000038b0: 616c 697a 6564 203d 2073 656c 662e 746f  alized = self.to
-000038c0: 5f64 6628 6e6f 726d 616c 697a 6564 3d54  _df(normalized=T
-000038d0: 7275 6529 0d0a 2020 2020 2020 2020 0d0a  rue)..        ..
-000038e0: 2020 2020 2020 2020 2320 6372 6561 7465          # create
-000038f0: 2064 6174 6166 7261 6d65 206f 6620 7065   dataframe of pe
-00003900: 722d 6765 6e65 2073 7461 7469 7374 6963  r-gene statistic
-00003910: 730d 0a20 2020 2020 2020 2073 656c 662e  s..        self.
-00003920: 6164 6174 612e 7661 725b 226d 6561 6e22  adata.var["mean"
-00003930: 5d20 3d20 6461 7461 5f6e 6f72 6d61 6c69  ] = data_normali
-00003940: 7a65 642e 6d65 616e 2829 0d0a 2020 2020  zed.mean()..    
-00003950: 2020 2020 7365 6c66 2e61 6461 7461 2e76      self.adata.v
-00003960: 6172 5b22 7261 6e6b 5f6d 6561 6e22 5d20  ar["rank_mean"] 
-00003970: 3d20 7365 6c66 2e61 6461 7461 2e76 6172  = self.adata.var
-00003980: 5b22 6d65 616e 225d 2e72 616e 6b28 290d  ["mean"].rank().
-00003990: 0a20 2020 2020 2020 2073 656c 662e 6164  .        self.ad
-000039a0: 6174 612e 7661 725b 2276 6172 6961 6e63  ata.var["varianc
-000039b0: 6522 5d20 3d20 6461 7461 5f6e 6f72 6d61  e"] = data_norma
-000039c0: 6c69 7a65 642e 7661 7228 290d 0a20 2020  lized.var()..   
-000039d0: 2020 2020 2073 656c 662e 6164 6174 612e       self.adata.
-000039e0: 7661 725b 2273 6422 5d20 3d20 6461 7461  var["sd"] = data
-000039f0: 5f6e 6f72 6d61 6c69 7a65 642e 7374 6428  _normalized.std(
-00003a00: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00003a10: 6164 6174 612e 7661 725b 226d 6973 7369  adata.var["missi
-00003a20: 6e67 6e65 7373 225d 203d 2064 6174 615f  ngness"] = data_
-00003a30: 6e6f 726d 616c 697a 6564 2e69 736e 756c  normalized.isnul
-00003a40: 6c28 292e 7375 6d28 2920 2f20 6461 7461  l().sum() / data
-00003a50: 5f6e 6f72 6d61 6c69 7a65 642e 7368 6170  _normalized.shap
-00003a60: 655b 305d 0d0a 2020 2020 2020 2020 7365  e[0]..        se
-00003a70: 6c66 2e61 6461 7461 2e76 6172 5b5b 226c  lf.adata.var[["l
-00003a80: 6f67 5f6d 6561 6e22 2c20 226c 6f67 5f76  og_mean", "log_v
-00003a90: 6172 6961 6e63 6522 5d5d 203d 206e 702e  ariance"]] = np.
-00003aa0: 6c6f 6731 3028 7365 6c66 2e61 6461 7461  log10(self.adata
-00003ab0: 2e76 6172 5b5b 226d 6561 6e22 2c20 2276  .var[["mean", "v
-00003ac0: 6172 6961 6e63 6522 5d5d 290d 0a20 2020  ariance"]])..   
-00003ad0: 2020 2020 2073 656c 662e 6164 6174 612e       self.adata.
-00003ae0: 7661 725b 226d 6561 6e5f 636f 756e 7473  var["mean_counts
-00003af0: 225d 203d 2064 6174 615f 7261 772e 6d65  "] = data_raw.me
-00003b00: 616e 2829 0d0a 2020 2020 2020 2020 7365  an()..        se
-00003b10: 6c66 2e61 6461 7461 2e76 6172 5b22 6f64  lf.adata.var["od
-00003b20: 7363 6f72 655f 6578 636c 7564 6564 225d  score_excluded"]
-00003b30: 203d 2028 2873 656c 662e 6164 6174 612e   = ((self.adata.
-00003b40: 7661 725b 226d 6973 7369 6e67 6e65 7373  var["missingness
-00003b50: 225d 203e 2030 2920 7c0d 0a20 2020 2020  "] > 0) |..     
-00003b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003b80: 2020 2020 2020 2020 2073 656c 662e 6164           self.ad
-00003b90: 6174 612e 7661 725b 226c 6f67 5f6d 6561  ata.var["log_mea
-00003ba0: 6e22 5d2e 6973 6e75 6c6c 2829 207c 0d0a  n"].isnull() |..
-00003bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001f70: 2020 2222 220d 0a20 2020 2020 2020 2069    """..        i
+00001f80: 6620 2270 6174 6965 6e74 5f69 645f 636f  f "patient_id_co
+00001f90: 6c22 2069 6e20 7365 6c66 2e61 6461 7461  l" in self.adata
+00001fa0: 2e75 6e73 3a0d 0a20 2020 2020 2020 2020  .uns:..         
+00001fb0: 2020 2072 6574 7572 6e20 7365 6c66 2e61     return self.a
+00001fc0: 6461 7461 2e75 6e73 5b22 7061 7469 656e  data.uns["patien
+00001fd0: 745f 6964 5f63 6f6c 225d 0d0a 2020 2020  t_id_col"]..    
+00001fe0: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
+00001ff0: 2020 2020 2020 2072 6574 7572 6e20 4e6f         return No
+00002000: 6e65 0d0a 2020 2020 0d0a 2020 2020 4070  ne..    ..    @p
+00002010: 6174 6965 6e74 5f69 645f 636f 6c2e 7365  atient_id_col.se
+00002020: 7474 6572 0d0a 2020 2020 6465 6620 7061  tter..    def pa
+00002030: 7469 656e 745f 6964 5f63 6f6c 2873 656c  tient_id_col(sel
+00002040: 662c 2076 616c 7565 3a20 7374 7229 3a0d  f, value: str):.
+00002050: 0a20 2020 2020 2020 200d 0a20 2020 2020  .        ..     
+00002060: 2020 2069 6620 7661 6c75 6520 6973 206e     if value is n
+00002070: 6f74 204e 6f6e 6520 616e 6420 7661 6c75  ot None and valu
+00002080: 6520 6e6f 7420 696e 2073 656c 662e 6164  e not in self.ad
+00002090: 6174 612e 6f62 732e 636f 6c75 6d6e 733a  ata.obs.columns:
+000020a0: 0d0a 2020 2020 2020 2020 2020 2020 6176  ..            av
+000020b0: 6169 6c5f 636f 6c75 6d6e 7320 3d20 222c  ail_columns = ",
+000020c0: 2022 2e6a 6f69 6e28 7365 6c66 2e61 6461   ".join(self.ada
+000020d0: 7461 2e6f 6273 2e63 6f6c 756d 6e73 290d  ta.obs.columns).
+000020e0: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
+000020f0: 7365 2056 616c 7565 4572 726f 7228 6622  se ValueError(f"
+00002100: 7b76 616c 7565 7d20 6973 206e 6f74 2061  {value} is not a
+00002110: 2076 616c 6964 2063 6f6c 756d 6e20 696e   valid column in
+00002120: 2074 6865 206d 6574 6164 6174 6120 6d61   the metadata ma
+00002130: 7472 6978 2e20 4176 6169 6c61 626c 6520  trix. Available 
+00002140: 636f 6c75 6d6e 7320 6172 653a 207b 6176  columns are: {av
+00002150: 6169 6c5f 636f 6c75 6d6e 737d 2229 0d0a  ail_columns}")..
+00002160: 2020 2020 2020 2020 7365 6c66 2e61 6461          self.ada
+00002170: 7461 2e75 6e73 5b22 7061 7469 656e 745f  ta.uns["patient_
+00002180: 6964 5f63 6f6c 225d 203d 2076 616c 7565  id_col"] = value
+00002190: 0d0a 0d0a 2020 2020 4070 726f 7065 7274  ....    @propert
+000021a0: 790d 0a20 2020 2064 6566 2063 6e6d 6673  y..    def cnmfs
+000021b0: 6e73 5f76 6572 7369 6f6e 2873 656c 6629  ns_version(self)
+000021c0: 3a0d 0a20 2020 2020 2020 2022 2222 634e  :..        """cN
+000021d0: 4d46 2d53 4e53 2076 6572 7369 6f6e 2075  MF-SNS version u
+000021e0: 7365 6420 746f 2063 7265 6174 6520 7468  sed to create th
+000021f0: 6520 6461 7461 7365 740d 0a0d 0a20 2020  e dataset....   
+00002200: 2020 2020 203a 7265 7475 726e 3a20 7665       :return: ve
+00002210: 7273 696f 6e0d 0a20 2020 2020 2020 203a  rsion..        :
+00002220: 7274 7970 653a 2073 7472 0d0a 2020 2020  rtype: str..    
+00002230: 2020 2020 2222 220d 0a20 2020 2020 2020      """..       
+00002240: 2069 6620 2263 6e6d 6673 6e73 5f76 6572   if "cnmfsns_ver
+00002250: 7369 6f6e 2220 696e 2073 656c 662e 6164  sion" in self.ad
+00002260: 6174 612e 756e 733a 0d0a 2020 2020 2020  ata.uns:..      
+00002270: 2020 2020 2020 7665 7273 696f 6e20 3d20        version = 
+00002280: 7365 6c66 2e61 6461 7461 2e75 6e73 5b22  self.adata.uns["
+00002290: 636e 6d66 736e 735f 7665 7273 696f 6e22  cnmfsns_version"
+000022a0: 5d0d 0a20 2020 2020 2020 2065 6c73 653a  ]..        else:
+000022b0: 0d0a 2020 2020 2020 2020 2020 2020 7665  ..            ve
+000022c0: 7273 696f 6e20 3d20 4e6f 6e65 0d0a 2020  rsion = None..  
+000022d0: 2020 2020 2020 7265 7475 726e 2076 6572        return ver
+000022e0: 7369 6f6e 0d0a 2020 2020 2020 2020 0d0a  sion..        ..
+000022f0: 2020 2020 4070 726f 7065 7274 790d 0a20      @property.. 
+00002300: 2020 2064 6566 2068 6173 5f63 6e6d 665f     def has_cnmf_
+00002310: 7265 7375 6c74 7328 7365 6c66 293a 0d0a  results(self):..
+00002320: 2020 2020 2020 2020 2222 2254 6573 7420          """Test 
+00002330: 666f 7220 7765 6874 6865 7220 4461 7461  for wehther Data
+00002340: 7365 7420 636f 6e74 6169 6e73 2063 4e4d  set contains cNM
+00002350: 4620 7265 7375 6c74 7320 666f 7220 7468  F results for th
+00002360: 6520 6461 7461 7365 740d 0a0d 0a20 2020  e dataset....   
+00002370: 2020 2020 203a 7265 7475 726e 3a20 5768       :return: Wh
+00002380: 6574 6865 7220 636f 6d70 6c65 7465 2063  ether complete c
+00002390: 4e4d 4620 7265 7375 6c74 7320 6172 6520  NMF results are 
+000023a0: 636f 6e74 6169 6e65 6420 666f 7220 6174  contained for at
+000023b0: 206c 6561 7374 2031 2072 616e 6b20 286b   least 1 rank (k
+000023c0: 290d 0a20 2020 2020 2020 203a 7274 7970  )..        :rtyp
+000023d0: 653a 2062 6f6f 6c0d 0a20 2020 2020 2020  e: bool..       
+000023e0: 2022 2222 0d0a 2020 2020 2020 2020 6d61   """..        ma
+000023f0: 7472 6978 5f63 6865 636b 7320 3d20 5b0d  trix_checks = [.
+00002400: 0a20 2020 2020 2020 2020 2020 2022 636e  .            "cn
+00002410: 6d66 5f75 7361 6765 2220 696e 2073 656c  mf_usage" in sel
+00002420: 662e 6164 6174 612e 6f62 736d 2c0d 0a20  f.adata.obsm,.. 
+00002430: 2020 2020 2020 2020 2020 2022 636e 6d66             "cnmf
+00002440: 5f67 6570 5f73 636f 7265 2220 696e 2073  _gep_score" in s
+00002450: 656c 662e 6164 6174 612e 7661 726d 2c0d  elf.adata.varm,.
+00002460: 0a20 2020 2020 2020 2020 2020 2022 636e  .            "cn
+00002470: 6d66 5f67 6570 5f74 706d 2220 696e 2073  mf_gep_tpm" in s
+00002480: 656c 662e 6164 6174 612e 7661 726d 2c0d  elf.adata.varm,.
+00002490: 0a20 2020 2020 2020 2020 2020 2022 636e  .            "cn
+000024a0: 6d66 5f67 6570 5f72 6177 2220 696e 2073  mf_gep_raw" in s
+000024b0: 656c 662e 6164 6174 612e 7661 726d 2c0d  elf.adata.varm,.
+000024c0: 0a20 2020 2020 2020 2020 2020 2022 6b76  .            "kv
+000024d0: 616c 7322 2069 6e20 7365 6c66 2e61 6461  als" in self.ada
+000024e0: 7461 2e75 6e73 0d0a 2020 2020 2020 2020  ta.uns..        
+000024f0: 5d0d 0a20 2020 2020 2020 2072 6574 7572  ]..        retur
+00002500: 6e20 616c 6c28 6d61 7472 6978 5f63 6865  n all(matrix_che
+00002510: 636b 7329 0d0a 2020 2020 2020 2020 0d0a  cks)..        ..
+00002520: 2020 2020 4070 726f 7065 7274 790d 0a20      @property.. 
+00002530: 2020 2064 6566 206f 7665 7264 6973 7065     def overdispe
+00002540: 7273 6564 5f67 656e 6573 2873 656c 6629  rsed_genes(self)
+00002550: 3a0d 0a20 2020 2020 2020 2022 2222 4f76  :..        """Ov
+00002560: 6572 6469 7370 6572 7365 6420 6765 6e65  erdispersed gene
+00002570: 206c 6973 7420 7573 6564 2066 6f72 2063   list used for c
+00002580: 4e4d 460d 0a0d 0a20 2020 2020 2020 203a  NMF....        :
+00002590: 7265 7475 726e 3a20 6765 6e65 206c 6973  return: gene lis
+000025a0: 740d 0a20 2020 2020 2020 203a 7274 7970  t..        :rtyp
+000025b0: 653a 206c 6973 740d 0a20 2020 2020 2020  e: list..       
+000025c0: 2022 2222 0d0a 2020 2020 2020 2020 7265   """..        re
+000025d0: 7475 726e 2073 656c 662e 6164 6174 612e  turn self.adata.
+000025e0: 756e 735b 2267 656e 655f 6c69 7374 225d  uns["gene_list"]
+000025f0: 0d0a 0d0a 0d0a 2020 2020 4063 6e6d 6673  ......    @cnmfs
+00002600: 6e73 5f76 6572 7369 6f6e 2e73 6574 7465  ns_version.sette
+00002610: 720d 0a20 2020 2064 6566 2063 6e6d 6673  r..    def cnmfs
+00002620: 6e73 5f76 6572 7369 6f6e 2873 656c 662c  ns_version(self,
+00002630: 2076 616c 7565 3a20 626f 6f6c 293a 0d0a   value: bool):..
+00002640: 2020 2020 2020 2020 7365 6c66 2e61 6461          self.ada
+00002650: 7461 2e75 6e73 5b22 636e 6d66 736e 735f  ta.uns["cnmfsns_
+00002660: 7665 7273 696f 6e22 5d20 3d20 7661 6c75  version"] = valu
+00002670: 650d 0a0d 0a20 2020 2020 2020 200d 0a20  e....        .. 
+00002680: 2020 2064 6566 2075 7064 6174 655f 6f62     def update_ob
+00002690: 7328 7365 6c66 2c20 6f62 7329 3a0d 0a20  s(self, obs):.. 
+000026a0: 2020 2020 2020 2022 2222 5570 6461 7465         """Update
+000026b0: 2074 6865 206f 6273 6572 7661 7469 6f6e   the observation
+000026c0: 206d 6574 6164 6174 6120 7769 7468 2061   metadata with a
+000026d0: 206e 6577 206d 6574 6164 6174 6120 6d61   new metadata ma
+000026e0: 7472 6978 0d0a 0d0a 2020 2020 2020 2020  trix....        
+000026f0: 3a70 6172 616d 206f 6273 3a20 416e 206f  :param obs: An o
+00002700: 6273 6572 7661 7469 6f6e 7320 c397 206d  bservations .. m
+00002710: 6574 6164 6174 6120 6d61 7472 6978 2c20  etadata matrix, 
+00002720: 6465 6661 756c 7473 2074 6f20 4e6f 6e65  defaults to None
+00002730: 0d0a 2020 2020 2020 2020 3a74 7970 6520  ..        :type 
+00002740: 6f62 733a 2060 7064 2e44 6174 6146 7261  obs: `pd.DataFra
+00002750: 6d65 602c 206f 7074 696f 6e61 6c0d 0a20  me`, optional.. 
+00002760: 2020 2020 2020 2022 2222 0d0a 2020 2020         """..    
+00002770: 2020 2020 2320 636f 6e76 6572 7420 276f      # convert 'o
+00002780: 626a 6563 7427 2064 7479 7065 2074 6f20  bject' dtype to 
+00002790: 6361 7465 676f 7269 6361 6c2c 2063 6f6e  categorical, con
+000027a0: 7665 7274 696e 6720 626f 6f6c 2076 616c  verting bool val
+000027b0: 7565 7320 746f 2073 7472 696e 6773 2061  ues to strings a
+000027c0: 7320 7468 6573 6520 6172 6520 6e6f 7420  s these are not 
+000027d0: 7375 7070 6f72 7465 6420 6279 2041 6e6e  supported by Ann
+000027e0: 4461 7461 206f 6e2d 6469 736b 2066 6f72  Data on-disk for
+000027f0: 6d61 740d 0a20 2020 2020 2020 2066 6f72  mat..        for
+00002800: 2063 6f6c 2069 6e20 6f62 732e 7365 6c65   col in obs.sele
+00002810: 6374 5f64 7479 7065 7328 696e 636c 7564  ct_dtypes(includ
+00002820: 653d 2822 626f 6f6c 222c 2022 6f62 6a65  e=("bool", "obje
+00002830: 6374 2229 292e 636f 6c75 6d6e 733a 0d0a  ct")).columns:..
+00002840: 2020 2020 2020 2020 2020 2020 6f62 735b              obs[
+00002850: 636f 6c5d 203d 206f 6273 5b63 6f6c 5d2e  col] = obs[col].
+00002860: 6173 7479 7065 2822 7374 7222 292e 6173  astype("str").as
+00002870: 7479 7065 2822 6361 7465 676f 7279 2229  type("category")
+00002880: 0d0a 2020 2020 2020 2020 6d69 7373 696e  ..        missin
+00002890: 675f 7361 6d70 6c65 735f 696e 5f58 203d  g_samples_in_X =
+000028a0: 206f 6273 2e69 6e64 6578 2e64 6966 6665   obs.index.diffe
+000028b0: 7265 6e63 6528 7365 6c66 2e61 6461 7461  rence(self.adata
+000028c0: 2e6f 6273 2e69 6e64 6578 292e 6173 7479  .obs.index).asty
+000028d0: 7065 2873 7472 292e 746f 5f6c 6973 7428  pe(str).to_list(
+000028e0: 290d 0a20 2020 2020 2020 2069 6620 6d69  )..        if mi
+000028f0: 7373 696e 675f 7361 6d70 6c65 735f 696e  ssing_samples_in
+00002900: 5f58 3a0d 0a20 2020 2020 2020 2020 2020  _X:..           
+00002910: 206c 6f67 6769 6e67 2e77 6172 6e69 6e67   logging.warning
+00002920: 2822 5468 6520 666f 6c6c 6f77 696e 6720  ("The following 
+00002930: 7361 6d70 6c65 7320 696e 2074 6865 206d  samples in the m
+00002940: 6574 6164 6174 6120 7765 7265 206e 6f74  etadata were not
+00002950: 2070 7265 7365 6e74 2069 6e20 7468 6520   present in the 
+00002960: 6461 7461 2028 6061 6461 7461 2e58 6029  data (`adata.X`)
+00002970: 3a5c 6e20 202d 2022 202b 2022 5c6e 2020  :\n  - " + "\n  
+00002980: 2d20 222e 6a6f 696e 286d 6973 7369 6e67  - ".join(missing
+00002990: 5f73 616d 706c 6573 5f69 6e5f 5829 290d  _samples_in_X)).
+000029a0: 0a20 2020 2020 2020 206d 6973 7369 6e67  .        missing
+000029b0: 5f73 616d 706c 6573 5f69 6e5f 6d64 203d  _samples_in_md =
+000029c0: 2073 656c 662e 6164 6174 612e 6f62 732e   self.adata.obs.
+000029d0: 696e 6465 782e 6469 6666 6572 656e 6365  index.difference
+000029e0: 286f 6273 2e69 6e64 6578 292e 6173 7479  (obs.index).asty
+000029f0: 7065 2873 7472 292e 746f 5f6c 6973 7428  pe(str).to_list(
+00002a00: 290d 0a20 2020 2020 2020 2069 6620 6d69  )..        if mi
+00002a10: 7373 696e 675f 7361 6d70 6c65 735f 696e  ssing_samples_in
+00002a20: 5f6d 643a 0d0a 2020 2020 2020 2020 2020  _md:..          
+00002a30: 2020 6c6f 6767 696e 672e 7761 726e 696e    logging.warnin
+00002a40: 6728 2254 6865 2066 6f6c 6c6f 7769 6e67  g("The following
+00002a50: 2073 616d 706c 6573 2069 6e20 7468 6520   samples in the 
+00002a60: 6461 7461 2028 6061 6461 7461 2e58 6029  data (`adata.X`)
+00002a70: 2077 6572 6520 6162 7365 6e74 2069 6e20   were absent in 
+00002a80: 7468 6520 6d65 7461 6461 7461 3a5c 6e20  the metadata:\n 
+00002a90: 202d 2022 202b 2022 5c6e 2020 2d20 222e   - " + "\n  - ".
+00002aa0: 6a6f 696e 286d 6973 7369 6e67 5f73 616d  join(missing_sam
+00002ab0: 706c 6573 5f69 6e5f 6d64 2929 0d0a 2020  ples_in_md))..  
+00002ac0: 2020 2020 2020 7365 6c66 2e61 6461 7461        self.adata
+00002ad0: 2e6f 6273 203d 206f 6273 2e72 6569 6e64  .obs = obs.reind
+00002ae0: 6578 2873 656c 662e 6164 6174 612e 6f62  ex(self.adata.ob
+00002af0: 732e 696e 6465 7829 0d0a 2020 2020 0d0a  s.index)..    ..
+00002b00: 2020 2020 6465 6620 6765 745f 6d65 7461      def get_meta
+00002b10: 6461 7461 5f74 7970 655f 7375 6d6d 6172  data_type_summar
+00002b20: 7928 7365 6c66 293a 0d0a 2020 2020 2020  y(self):..      
+00002b30: 2020 2222 2252 6574 7572 6e20 6120 7072    """Return a pr
+00002b40: 696e 7461 626c 6520 7375 6d6d 6172 7920  intable summary 
+00002b50: 6f66 206d 6574 6164 6174 6120 616e 6420  of metadata and 
+00002b60: 7661 6c75 6520 7479 7065 7320 666f 7220  value types for 
+00002b70: 6561 6368 206d 6574 6164 6174 6120 6c61  each metadata la
+00002b80: 7965 722e 0d0a 0d0a 2020 2020 2020 2020  yer.....        
+00002b90: 3a72 6574 7572 6e3a 2053 756d 6d61 7279  :return: Summary
+00002ba0: 206f 6620 6d65 7461 6461 7461 0d0a 2020   of metadata..  
+00002bb0: 2020 2020 2020 3a72 7479 7065 3a20 7374        :rtype: st
+00002bc0: 720d 0a20 2020 2020 2020 2022 2222 0d0a  r..        """..
+00002bd0: 2020 2020 2020 2020 6d73 6720 3d20 2222          msg = ""
+00002be0: 0d0a 2020 2020 2020 2020 666f 7220 636f  ..        for co
+00002bf0: 6c20 696e 2073 656c 662e 6164 6174 612e  l in self.adata.
+00002c00: 6f62 732e 636f 6c75 6d6e 733a 0d0a 2020  obs.columns:..  
+00002c10: 2020 2020 2020 2020 2020 6d73 6720 2b3d            msg +=
+00002c20: 2022 2020 2020 436f 6c75 6d6e 3a20 2220   "    Column: " 
+00002c30: 2b20 636f 6c20 2b20 225c 6e22 0d0a 2020  + col + "\n"..  
+00002c40: 2020 2020 2020 2020 2020 666f 7220 7661            for va
+00002c50: 6c75 655f 7479 7065 2c20 636f 756e 7420  lue_type, count 
+00002c60: 696e 2073 656c 662e 6164 6174 612e 6f62  in self.adata.ob
+00002c70: 735b 636f 6c5d 2e64 726f 706e 6128 292e  s[col].dropna().
+00002c80: 6d61 7028 7479 7065 292e 7661 6c75 655f  map(type).value_
+00002c90: 636f 756e 7473 2829 2e69 7465 6d73 2829  counts().items()
+00002ca0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00002cb0: 2020 206d 7367 202b 3d20 6622 2020 2020     msg += f"    
+00002cc0: 2020 2020 7b76 616c 7565 5f74 7970 657d      {value_type}
+00002cd0: 3a20 7b63 6f75 6e74 7d5c 6e22 0d0a 2020  : {count}\n"..  
+00002ce0: 2020 2020 2020 7265 7475 726e 206d 7367        return msg
+00002cf0: 0d0a 2020 2020 0d0a 2020 2020 6465 6620  ..    ..    def 
+00002d00: 7772 6974 655f 6835 6164 2873 656c 662c  write_h5ad(self,
+00002d10: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00002d20: 2020 2020 2066 696c 656e 616d 653a 2073       filename: s
+00002d30: 7472 293a 0d0a 2020 2020 2020 2020 2222  tr):..        ""
+00002d40: 2257 7269 7465 2064 6174 6173 6574 2074  "Write dataset t
+00002d50: 6f20 2e68 3561 6420 6669 6c65 2e0d 0a0d  o .h5ad file....
+00002d60: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+00002d70: 6669 6c65 6e61 6d65 3a20 6669 6c65 7061  filename: filepa
+00002d80: 7468 0d0a 2020 2020 2020 2020 3a74 7970  th..        :typ
+00002d90: 6520 6669 6c65 6e61 6d65 3a20 7374 720d  e filename: str.
+00002da0: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
+00002db0: 2020 2020 2020 6669 6c65 6e61 6d65 203d        filename =
+00002dc0: 206f 732e 7061 7468 2e61 6273 7061 7468   os.path.abspath
+00002dd0: 2866 696c 656e 616d 6529 0d0a 2020 2020  (filename)..    
+00002de0: 2020 2020 6c6f 6767 696e 672e 696e 666f      logging.info
+00002df0: 2866 2257 7269 7469 6e67 2074 6f20 7b66  (f"Writing to {f
+00002e00: 696c 656e 616d 657d 2229 0d0a 2020 2020  ilename}")..    
+00002e10: 2020 2020 7365 6c66 2e61 6461 7461 2e77      self.adata.w
+00002e20: 7269 7465 5f68 3561 6428 6669 6c65 6e61  rite_h5ad(filena
+00002e30: 6d65 290d 0a20 2020 2020 2020 206c 6f67  me)..        log
+00002e40: 6769 6e67 2e69 6e66 6f28 6622 446f 6e65  ging.info(f"Done
+00002e50: 2229 0d0a 2020 2020 0d0a 2020 2020 6465  ")..    ..    de
+00002e60: 6620 746f 5f64 6628 7365 6c66 2c0d 0a20  f to_df(self,.. 
+00002e70: 2020 2020 2020 2020 2020 2020 206e 6f72               nor
+00002e80: 6d61 6c69 7a65 643a 2062 6f6f 6c20 3d20  malized: bool = 
+00002e90: 4661 6c73 6529 3a0d 0a20 2020 2020 2020  False):..       
+00002ea0: 2022 2222 4765 7420 6461 7461 206d 6174   """Get data mat
+00002eb0: 7269 7820 6173 2061 2060 7064 2e44 6174  rix as a `pd.Dat
+00002ec0: 6146 7261 6d65 600d 0a0d 0a20 2020 2020  aFrame`....     
+00002ed0: 2020 203a 7061 7261 6d20 6e6f 726d 616c     :param normal
+00002ee0: 697a 6564 3a20 5365 7420 7472 7565 2066  ized: Set true f
+00002ef0: 6f72 2054 504d 206e 6f72 6d61 6c69 7a65  or TPM normalize
+00002f00: 6420 6f75 7470 7574 2c20 6465 6661 756c  d output, defaul
+00002f10: 7473 2074 6f20 4661 6c73 650d 0a20 2020  ts to False..   
+00002f20: 2020 2020 203a 7479 7065 206e 6f72 6d61       :type norma
+00002f30: 6c69 7a65 643a 2062 6f6f 6c2c 206f 7074  lized: bool, opt
+00002f40: 696f 6e61 6c0d 0a20 2020 2020 2020 203a  ional..        :
+00002f50: 7265 7475 726e 3a20 6f62 7365 7276 6174  return: observat
+00002f60: 696f 6e73 20c3 9720 7661 7269 6162 6c65  ions .. variable
+00002f70: 7320 6461 7461 206d 6174 7269 780d 0a20  s data matrix.. 
+00002f80: 2020 2020 2020 203a 7274 7970 653a 2070         :rtype: p
+00002f90: 642e 4461 7461 4672 616d 650d 0a20 2020  d.DataFrame..   
+00002fa0: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
+00002fb0: 2020 6466 203d 2073 656c 662e 6164 6174    df = self.adat
+00002fc0: 612e 746f 5f64 6628 290d 0a20 2020 2020  a.to_df()..     
+00002fd0: 2020 2069 6620 6e6f 726d 616c 697a 6564     if normalized
+00002fe0: 2061 6e64 206e 6f74 2073 656c 662e 6973   and not self.is
+00002ff0: 5f6e 6f72 6d61 6c69 7a65 643a 0d0a 2020  _normalized:..  
+00003000: 2020 2020 2020 2020 2020 6466 203d 2064            df = d
+00003010: 662e 6469 7628 6466 2e73 756d 2861 7869  f.div(df.sum(axi
+00003020: 733d 3129 2c20 6178 6973 3d30 2920 2a20  s=1), axis=0) * 
+00003030: 3165 3620 2023 2054 504d 206e 6f72 6d61  1e6  # TPM norma
+00003040: 6c69 7a61 7469 6f6e 0d0a 2020 2020 2020  lization..      
+00003050: 2020 7265 7475 726e 2064 660d 0a20 2020    return df..   
+00003060: 2020 2020 200d 0a20 2020 2064 6566 2072       ..    def r
+00003070: 656d 6f76 655f 756e 6661 6374 6f72 697a  emove_unfactoriz
+00003080: 6162 6c65 5f67 656e 6573 2873 656c 6629  able_genes(self)
+00003090: 3a0d 0a20 2020 2020 2020 2022 2222 5265  :..        """Re
+000030a0: 6d6f 7665 7320 6765 6e65 7320 7769 7468  moves genes with
+000030b0: 206d 6973 7369 6e67 2076 616c 7565 7320   missing values 
+000030c0: 6f72 207a 6572 6f20 7661 7269 616e 6365  or zero variance
+000030d0: 2066 726f 6d20 7468 6520 6461 7461 206d   from the data m
+000030e0: 6174 7269 782e 0d0a 2020 2020 2020 2020  atrix...        
+000030f0: 2222 220d 0a20 2020 2020 2020 2064 6620  """..        df 
+00003100: 3d20 7365 6c66 2e74 6f5f 6466 286e 6f72  = self.to_df(nor
+00003110: 6d61 6c69 7a65 643d 4661 6c73 6529 0d0a  malized=False)..
+00003120: 2020 2020 2020 2020 2320 4368 6563 6b20          # Check 
+00003130: 666f 7220 7661 7269 6162 6c65 7320 7769  for variables wi
+00003140: 7468 206d 6973 7369 6e67 2076 616c 7565  th missing value
+00003150: 730d 0a20 2020 2020 2020 2067 656e 6573  s..        genes
+00003160: 5f77 6974 685f 6d69 7373 696e 6776 616c  _with_missingval
+00003170: 7565 7320 3d20 6466 2e69 736e 756c 6c28  ues = df.isnull(
+00003180: 292e 616e 7928 290d 0a20 2020 2020 2020  ).any()..       
+00003190: 200d 0a20 2020 2020 2020 2069 6620 6765   ..        if ge
+000031a0: 6e65 735f 7769 7468 5f6d 6973 7369 6e67  nes_with_missing
+000031b0: 7661 6c75 6573 2e61 6e79 2829 3a0d 0a20  values.any():.. 
+000031c0: 2020 2020 2020 2020 2020 206e 5f6d 6973             n_mis
+000031d0: 7369 6e67 203d 2067 656e 6573 5f77 6974  sing = genes_wit
+000031e0: 685f 6d69 7373 696e 6776 616c 7565 732e  h_missingvalues.
+000031f0: 7375 6d28 290d 0a20 2020 2020 2020 2020  sum()..         
+00003200: 2020 206c 6f67 6769 6e67 2e77 6172 6e69     logging.warni
+00003210: 6e67 2866 227b 6e5f 6d69 7373 696e 677d  ng(f"{n_missing}
+00003220: 206f 6620 7b73 656c 662e 6164 6174 612e   of {self.adata.
+00003230: 6e5f 7661 7273 7d20 7661 7269 6162 6c65  n_vars} variable
+00003240: 7320 6172 6520 6d69 7373 696e 6720 7661  s are missing va
+00003250: 6c75 6573 2028 6061 6461 7461 2e58 6029  lues (`adata.X`)
+00003260: 2e22 290d 0a20 2020 2020 2020 2020 2020  .")..           
+00003270: 206c 6f67 6769 6e67 2e77 6172 6e69 6e67   logging.warning
+00003280: 2866 2253 7562 7365 7474 696e 6720 7661  (f"Subsetting va
+00003290: 7269 6162 6c65 7320 746f 2074 686f 7365  riables to those
+000032a0: 2077 6974 6820 6e6f 206d 6973 7369 6e67   with no missing
+000032b0: 2076 616c 7565 732e 2229 0d0a 2020 2020   values.")..    
+000032c0: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
+000032d0: 2020 2020 2020 2320 4368 6563 6b20 666f        # Check fo
+000032e0: 7220 6765 6e65 7320 7769 7468 207a 6572  r genes with zer
+000032f0: 6f20 7661 7269 616e 6365 0d0a 2020 2020  o variance..    
+00003300: 2020 2020 7a65 726f 7661 7267 656e 6573      zerovargenes
+00003310: 203d 2028 6466 2e76 6172 2829 203d 3d20   = (df.var() == 
+00003320: 3029 0d0a 2020 2020 2020 2020 6966 207a  0)..        if z
+00003330: 6572 6f76 6172 6765 6e65 732e 616e 7928  erovargenes.any(
+00003340: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+00003350: 6e5f 7a65 726f 7661 7220 3d20 7a65 726f  n_zerovar = zero
+00003360: 7661 7267 656e 6573 2e73 756d 2829 0d0a  vargenes.sum()..
+00003370: 2020 2020 2020 2020 2020 2020 6c6f 6767              logg
+00003380: 696e 672e 7761 726e 696e 6728 6622 7b6e  ing.warning(f"{n
+00003390: 5f7a 6572 6f76 6172 7d20 6f66 207b 7365  _zerovar} of {se
+000033a0: 6c66 2e61 6461 7461 2e6e 5f76 6172 737d  lf.adata.n_vars}
+000033b0: 2076 6172 6961 626c 6573 2068 6176 6520   variables have 
+000033c0: 6120 7661 7269 616e 6365 206f 6620 7a65  a variance of ze
+000033d0: 726f 2069 6e20 636f 756e 7473 2064 6174  ro in counts dat
+000033e0: 6120 2860 6164 6174 612e 7261 772e 5860  a (`adata.raw.X`
+000033f0: 292e 2229 0d0a 2020 2020 2020 2020 2020  ).")..          
+00003400: 2020 6c6f 6767 696e 672e 7761 726e 696e    logging.warnin
+00003410: 6728 6622 5375 6273 6574 7469 6e67 2076  g(f"Subsetting v
+00003420: 6172 6961 626c 6573 2074 6f20 7468 6f73  ariables to thos
+00003430: 6520 7769 7468 206e 6f6e 7a65 726f 2076  e with nonzero v
+00003440: 6172 6961 6e63 652e 2229 0d0a 2020 2020  ariance.")..    
+00003450: 2020 2020 0d0a 2020 2020 2020 2020 6765      ..        ge
+00003460: 6e65 735f 746f 5f6b 6565 7020 3d20 287e  nes_to_keep = (~
+00003470: 6765 6e65 735f 7769 7468 5f6d 6973 7369  genes_with_missi
+00003480: 6e67 7661 6c75 6573 2920 2620 287e 7a65  ngvalues) & (~ze
+00003490: 726f 7661 7267 656e 6573 290d 0a20 2020  rovargenes)..   
+000034a0: 2020 2020 200d 0a20 2020 2020 2020 2073       ..        s
+000034b0: 656c 662e 6164 6174 6120 3d20 7365 6c66  elf.adata = self
+000034c0: 2e61 6461 7461 5b3a 2c67 656e 6573 5f74  .adata[:,genes_t
+000034d0: 6f5f 6b65 6570 5d0d 0a0d 0a20 2020 2064  o_keep]....    d
+000034e0: 6566 2063 6f6d 7075 7465 5f67 656e 655f  ef compute_gene_
+000034f0: 7374 6174 7328 7365 6c66 2c20 6f64 675f  stats(self, odg_
+00003500: 6465 6661 756c 745f 7370 6c69 6e65 5f64  default_spline_d
+00003510: 6567 7265 653a 2069 6e74 203d 2033 2c20  egree: int = 3, 
+00003520: 6f64 675f 6465 6661 756c 745f 646f 663a  odg_default_dof:
+00003530: 2069 6e74 203d 2038 293a 0d0a 2020 2020   int = 8):..    
+00003540: 2020 2020 2222 220d 0a20 2020 2020 2020      """..       
+00003550: 2043 6f6d 7075 7465 7320 6765 6e65 2073   Computes gene s
+00003560: 7461 7469 7374 6963 7320 616e 6420 6669  tatistics and fi
+00003570: 7473 2074 776f 206d 6f64 656c 7320 6f66  ts two models of
+00003580: 206d 6561 6e20 616e 6420 7661 7269 616e   mean and varian
+00003590: 6365 206f 6620 6765 6e65 7320 696e 2074  ce of genes in t
+000035a0: 6865 2064 6174 6173 6574 2e20 5468 6520  he dataset. The 
+000035b0: 6669 7273 7420 6d65 7468 6f64 2069 7320  first method is 
+000035c0: 7468 650d 0a20 2020 2020 2020 2067 656e  the..        gen
+000035d0: 6572 616c 697a 6564 2061 6464 6974 6976  eralized additiv
+000035e0: 6520 6d6f 6465 6c20 7769 7468 2073 6d6f  e model with smo
+000035f0: 6f74 6820 636f 6d70 6f6e 656e 7473 2028  oth components (
+00003600: 422d 7370 6c69 6e65 7329 2074 6f20 6d6f  B-splines) to mo
+00003610: 6465 6c20 7468 6520 7265 6c61 7469 6f6e  del the relation
+00003620: 7368 6970 206f 6620 6d65 616e 2061 6e64  ship of mean and
+00003630: 2076 6172 6961 6e63 650d 0a20 2020 2020   variance..     
+00003640: 2020 2062 6574 7765 656e 2067 656e 6573     between genes
+00003650: 2069 6e20 7468 6520 6461 7461 7365 742e   in the dataset.
+00003660: 2049 7420 7072 6f64 7563 6573 2061 6e20   It produces an 
+00003670: 6f64 7363 6f72 6520 6d65 7472 6963 2066  odscore metric f
+00003680: 6f72 206f 7665 7264 6973 7065 7273 696f  or overdispersio
+00003690: 6e2e 2054 6865 2073 6563 6f6e 6420 6973  n. The second is
+000036a0: 2074 6865 2063 6f75 6e74 2d73 7461 7469   the count-stati
+000036b0: 7374 6963 730d 0a20 2020 2020 2020 206d  stics..        m
+000036c0: 6574 686f 6420 666f 756e 6420 696e 2074  ethod found in t
+000036d0: 6865 2063 4e4d 4620 7061 636b 6167 652c  he cNMF package,
+000036e0: 2077 6869 6368 2070 726f 6475 6365 7320   which produces 
+000036f0: 6120 6d6f 6469 6669 6564 2076 2d73 636f  a modified v-sco
+00003700: 7265 206d 6574 7269 632e 2041 6c6c 2067  re metric. All g
+00003710: 656e 6520 7374 6174 6973 7469 6373 2061  ene statistics a
+00003720: 7265 2073 746f 7265 6420 7769 7468 696e  re stored within
+00003730: 2074 6865 0d0a 2020 2020 2020 2020 6461   the..        da
+00003740: 7461 7365 7420 6f62 6a65 6374 2061 6e64  taset object and
+00003750: 2061 7265 2061 6363 6573 7369 626c 6520   are accessible 
+00003760: 7573 696e 6720 6064 6174 6173 6574 2e61  using `dataset.a
+00003770: 6e6e 6461 7461 2e76 6172 602e 0d0a 0d0a  nndata.var`.....
+00003780: 2020 2020 2020 2020 3a70 6172 616d 206f          :param o
+00003790: 6467 5f64 6566 6175 6c74 5f73 706c 696e  dg_default_splin
+000037a0: 655f 6465 6772 6565 3a20 422d 5370 6c69  e_degree: B-Spli
+000037b0: 6e65 2064 6567 7265 6520 666f 7220 474c  ne degree for GL
+000037c0: 4d2d 4741 4d20 6d6f 6465 6c6c 696e 6720  M-GAM modelling 
+000037d0: 6f66 206d 6561 6e2d 7661 7269 616e 6365  of mean-variance
+000037e0: 2072 656c 6174 696f 6e73 6869 702c 2064   relationship, d
+000037f0: 6566 6175 6c74 7320 746f 2033 0d0a 2020  efaults to 3..  
+00003800: 2020 2020 2020 3a74 7970 6520 6f64 675f        :type odg_
+00003810: 6465 6661 756c 745f 7370 6c69 6e65 5f64  default_spline_d
+00003820: 6567 7265 653a 2069 6e74 2c20 6f70 7469  egree: int, opti
+00003830: 6f6e 616c 0d0a 2020 2020 2020 2020 3a70  onal..        :p
+00003840: 6172 616d 206f 6467 5f64 6566 6175 6c74  aram odg_default
+00003850: 5f64 6f66 3a20 4465 6772 6565 7320 6f66  _dof: Degrees of
+00003860: 2066 7265 6564 6f6d 2066 6f72 2047 4c4d   freedom for GLM
+00003870: 2d47 414d 206d 6f64 656c 6c69 6e67 206f  -GAM modelling o
+00003880: 6620 6d65 616e 2d76 6172 616e 6365 2c20  f mean-varance, 
+00003890: 6465 6661 756c 7473 2074 6f20 380d 0a20  defaults to 8.. 
+000038a0: 2020 2020 2020 203a 7479 7065 206f 6467         :type odg
+000038b0: 5f64 6566 6175 6c74 5f64 6f66 3a20 696e  _default_dof: in
+000038c0: 742c 206f 7074 696f 6e61 6c0d 0a20 2020  t, optional..   
+000038d0: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
+000038e0: 2020 6461 7461 5f72 6177 203d 2073 656c    data_raw = sel
+000038f0: 662e 746f 5f64 6628 290d 0a20 2020 2020  f.to_df()..     
+00003900: 2020 2064 6174 615f 6e6f 726d 616c 697a     data_normaliz
+00003910: 6564 203d 2073 656c 662e 746f 5f64 6628  ed = self.to_df(
+00003920: 6e6f 726d 616c 697a 6564 3d54 7275 6529  normalized=True)
+00003930: 0d0a 2020 2020 2020 2020 0d0a 2020 2020  ..        ..    
+00003940: 2020 2020 2320 6372 6561 7465 2064 6174      # create dat
+00003950: 6166 7261 6d65 206f 6620 7065 722d 6765  aframe of per-ge
+00003960: 6e65 2073 7461 7469 7374 6963 730d 0a20  ne statistics.. 
+00003970: 2020 2020 2020 2073 656c 662e 6164 6174         self.adat
+00003980: 612e 7661 725b 226d 6561 6e22 5d20 3d20  a.var["mean"] = 
+00003990: 6461 7461 5f6e 6f72 6d61 6c69 7a65 642e  data_normalized.
+000039a0: 6d65 616e 2829 0d0a 2020 2020 2020 2020  mean()..        
+000039b0: 7365 6c66 2e61 6461 7461 2e76 6172 5b22  self.adata.var["
+000039c0: 7261 6e6b 5f6d 6561 6e22 5d20 3d20 7365  rank_mean"] = se
+000039d0: 6c66 2e61 6461 7461 2e76 6172 5b22 6d65  lf.adata.var["me
+000039e0: 616e 225d 2e72 616e 6b28 290d 0a20 2020  an"].rank()..   
+000039f0: 2020 2020 2073 656c 662e 6164 6174 612e       self.adata.
+00003a00: 7661 725b 2276 6172 6961 6e63 6522 5d20  var["variance"] 
+00003a10: 3d20 6461 7461 5f6e 6f72 6d61 6c69 7a65  = data_normalize
+00003a20: 642e 7661 7228 290d 0a20 2020 2020 2020  d.var()..       
+00003a30: 2073 656c 662e 6164 6174 612e 7661 725b   self.adata.var[
+00003a40: 2273 6422 5d20 3d20 6461 7461 5f6e 6f72  "sd"] = data_nor
+00003a50: 6d61 6c69 7a65 642e 7374 6428 290d 0a20  malized.std().. 
+00003a60: 2020 2020 2020 2073 656c 662e 6164 6174         self.adat
+00003a70: 612e 7661 725b 226d 6973 7369 6e67 6e65  a.var["missingne
+00003a80: 7373 225d 203d 2064 6174 615f 6e6f 726d  ss"] = data_norm
+00003a90: 616c 697a 6564 2e69 736e 756c 6c28 292e  alized.isnull().
+00003aa0: 7375 6d28 2920 2f20 6461 7461 5f6e 6f72  sum() / data_nor
+00003ab0: 6d61 6c69 7a65 642e 7368 6170 655b 305d  malized.shape[0]
+00003ac0: 0d0a 2020 2020 2020 2020 7365 6c66 2e61  ..        self.a
+00003ad0: 6461 7461 2e76 6172 5b5b 226c 6f67 5f6d  data.var[["log_m
+00003ae0: 6561 6e22 2c20 226c 6f67 5f76 6172 6961  ean", "log_varia
+00003af0: 6e63 6522 5d5d 203d 206e 702e 6c6f 6731  nce"]] = np.log1
+00003b00: 3028 7365 6c66 2e61 6461 7461 2e76 6172  0(self.adata.var
+00003b10: 5b5b 226d 6561 6e22 2c20 2276 6172 6961  [["mean", "varia
+00003b20: 6e63 6522 5d5d 290d 0a20 2020 2020 2020  nce"]])..       
+00003b30: 2073 656c 662e 6164 6174 612e 7661 725b   self.adata.var[
+00003b40: 226d 6561 6e5f 636f 756e 7473 225d 203d  "mean_counts"] =
+00003b50: 2064 6174 615f 7261 772e 6d65 616e 2829   data_raw.mean()
+00003b60: 0d0a 2020 2020 2020 2020 7365 6c66 2e61  ..        self.a
+00003b70: 6461 7461 2e76 6172 5b22 6f64 7363 6f72  data.var["odscor
+00003b80: 655f 6578 636c 7564 6564 225d 203d 2028  e_excluded"] = (
+00003b90: 2873 656c 662e 6164 6174 612e 7661 725b  (self.adata.var[
+00003ba0: 226d 6973 7369 6e67 6e65 7373 225d 203e  "missingness"] >
+00003bb0: 2030 2920 7c0d 0a20 2020 2020 2020 2020   0) |..         
 00003bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003bd0: 2020 2020 2020 2020 2020 2020 2020 2873                (s
-00003be0: 656c 662e 6164 6174 612e 7661 725b 226d  elf.adata.var["m
-00003bf0: 6561 6e22 5d20 3d3d 2030 2920 7c0d 0a20  ean"] == 0) |.. 
-00003c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003be0: 2020 2020 2073 656c 662e 6164 6174 612e       self.adata.
+00003bf0: 7661 725b 226c 6f67 5f6d 6561 6e22 5d2e  var["log_mean"].
+00003c00: 6973 6e75 6c6c 2829 207c 0d0a 2020 2020  isnull() |..    
 00003c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003c20: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00003c30: 662e 6164 6174 612e 7661 725b 226c 6f67  f.adata.var["log
-00003c40: 5f76 6172 6961 6e63 6522 5d2e 6973 6e75  _variance"].isnu
-00003c50: 6c6c 2829 290d 0a0d 0a20 2020 2020 2020  ll())....       
-00003c60: 2023 206d 6f64 656c 206d 6561 6e2d 7661   # model mean-va
-00003c70: 7269 616e 6365 2072 656c 6174 696f 6e73  riance relations
-00003c80: 6869 7020 7573 696e 6720 6765 6e65 7261  hip using genera
-00003c90: 6c69 7a65 6420 6164 6469 7469 7665 206d  lized additive m
-00003ca0: 6f64 656c 2077 6974 6820 736d 6f6f 7468  odel with smooth
-00003cb0: 2063 6f6d 706f 6e65 6e74 730d 0a20 2020   components..   
-00003cc0: 2020 2020 2064 665f 6d6f 6465 6c20 3d20       df_model = 
-00003cd0: 7365 6c66 2e61 6461 7461 2e76 6172 5b7e  self.adata.var[~
-00003ce0: 7365 6c66 2e61 6461 7461 2e76 6172 5b22  self.adata.var["
-00003cf0: 6f64 7363 6f72 655f 6578 636c 7564 6564  odscore_excluded
-00003d00: 225d 5d0d 0a20 2020 2020 2020 2062 7320  "]]..        bs 
-00003d10: 3d20 4253 706c 696e 6573 2864 665f 6d6f  = BSplines(df_mo
-00003d20: 6465 6c5b 226d 6561 6e22 5d2c 2064 663d  del["mean"], df=
-00003d30: 6f64 675f 6465 6661 756c 745f 646f 662c  odg_default_dof,
-00003d40: 2064 6567 7265 653d 6f64 675f 6465 6661   degree=odg_defa
-00003d50: 756c 745f 7370 6c69 6e65 5f64 6567 7265  ult_spline_degre
-00003d60: 6529 0d0a 2020 2020 2020 2020 6761 6d20  e)..        gam 
-00003d70: 3d20 474c 4d47 616d 2e66 726f 6d5f 666f  = GLMGam.from_fo
-00003d80: 726d 756c 6128 226c 6f67 5f76 6172 6961  rmula("log_varia
-00003d90: 6e63 6520 7e20 6c6f 675f 6d65 616e 222c  nce ~ log_mean",
-00003da0: 2064 6174 613d 6466 5f6d 6f64 656c 2c20   data=df_model, 
-00003db0: 736d 6f6f 7468 6572 3d62 7329 2e66 6974  smoother=bs).fit
-00003dc0: 2829 0d0a 2020 2020 2020 2020 7365 6c66  ()..        self
-00003dd0: 2e61 6461 7461 2e76 6172 5b22 7265 7369  .adata.var["resi
-00003de0: 645f 6c6f 675f 7661 7269 616e 6365 225d  d_log_variance"]
-00003df0: 203d 2067 616d 2e72 6573 6964 5f72 6573   = gam.resid_res
-00003e00: 706f 6e73 650d 0a20 2020 2020 2020 2073  ponse..        s
-00003e10: 656c 662e 6164 6174 612e 7661 725b 226f  elf.adata.var["o
-00003e20: 6473 636f 7265 225d 203d 206e 702e 7371  dscore"] = np.sq
-00003e30: 7274 2831 3020 2a2a 2073 656c 662e 6164  rt(10 ** self.ad
-00003e40: 6174 612e 7661 725b 2272 6573 6964 5f6c  ata.var["resid_l
-00003e50: 6f67 5f76 6172 6961 6e63 6522 5d29 0d0a  og_variance"])..
-00003e60: 2020 2020 2020 2020 7365 6c66 2e61 6461          self.ada
-00003e70: 7461 2e76 6172 5b22 6761 6d5f 6669 7474  ta.var["gam_fitt
-00003e80: 6564 7661 6c75 6573 225d 203d 2067 616d  edvalues"] = gam
-00003e90: 2e66 6974 7465 6476 616c 7565 730d 0a0d  .fittedvalues...
-00003ea0: 0a0d 0a20 2020 2020 2020 2023 206d 6f64  ...        # mod
-00003eb0: 656c 206d 6561 6e2d 7661 7269 616e 6365  el mean-variance
-00003ec0: 2072 656c 6174 696f 6e73 6869 7020 7573   relationship us
-00003ed0: 696e 6720 634e 4d46 2773 206d 6574 686f  ing cNMF's metho
-00003ee0: 6420 6261 7365 6420 6f6e 2076 2d73 636f  d based on v-sco
-00003ef0: 7265 2061 6e64 206d 696e 696d 756d 2065  re and minimum e
-00003f00: 7870 7265 7373 696f 6e20 7468 7265 7368  xpression thresh
-00003f10: 6f6c 640d 0a20 2020 2020 2020 2076 7363  old..        vsc
-00003f20: 6f72 655f 7374 6174 7320 3d20 7064 2e44  ore_stats = pd.D
-00003f30: 6174 6146 7261 6d65 2863 6e6d 662e 6765  ataFrame(cnmf.ge
-00003f40: 745f 6869 6768 7661 725f 6765 6e65 7328  t_highvar_genes(
-00003f50: 696e 7075 745f 636f 756e 7473 3d64 6174  input_counts=dat
-00003f60: 615f 6e6f 726d 616c 697a 6564 2e76 616c  a_normalized.val
-00003f70: 7565 732c 206d 696e 696d 616c 5f6d 6561  ues, minimal_mea
-00003f80: 6e3d 3029 5b30 5d29 0d0a 2020 2020 2020  n=0)[0])..      
-00003f90: 2020 7673 636f 7265 5f73 7461 7473 2e69    vscore_stats.i
-00003fa0: 6e64 6578 203d 2064 6174 615f 6e6f 726d  ndex = data_norm
-00003fb0: 616c 697a 6564 2e63 6f6c 756d 6e73 0d0a  alized.columns..
-00003fc0: 2020 2020 2020 2020 7365 6c66 2e61 6461          self.ada
-00003fd0: 7461 2e76 6172 5b22 7673 636f 7265 225d  ta.var["vscore"]
-00003fe0: 203d 2076 7363 6f72 655f 7374 6174 735b   = vscore_stats[
-00003ff0: 2266 616e 6f5f 7261 7469 6f22 5d0d 0a20  "fano_ratio"].. 
-00004000: 2020 2020 2020 2073 656c 662e 6164 6174         self.adat
-00004010: 612e 756e 735b 226f 6467 225d 5b22 6f64  a.uns["odg"]["od
-00004020: 675f 6465 6661 756c 745f 7370 6c69 6e65  g_default_spline
-00004030: 5f64 6567 7265 6522 5d20 3d20 6f64 675f  _degree"] = odg_
-00004040: 6465 6661 756c 745f 7370 6c69 6e65 5f64  default_spline_d
-00004050: 6567 7265 650d 0a20 2020 2020 2020 2073  egree..        s
-00004060: 656c 662e 6164 6174 612e 756e 735b 226f  elf.adata.uns["o
-00004070: 6467 225d 5b22 6f64 675f 6465 6661 756c  dg"]["odg_defaul
-00004080: 745f 646f 6622 5d20 3d20 6f64 675f 6465  t_dof"] = odg_de
-00004090: 6661 756c 745f 646f 660d 0a20 2020 2020  fault_dof..     
-000040a0: 2020 2073 656c 662e 6170 7065 6e64 5f74     self.append_t
-000040b0: 6f5f 6869 7374 6f72 7928 2247 656e 652d  o_history("Gene-
-000040c0: 6c65 7665 6c20 7374 6174 6973 7469 6373  level statistics
-000040d0: 2061 6e64 206f 7665 7264 6973 7065 7273   and overdispers
-000040e0: 696f 6e20 6d6f 6465 6c6c 696e 6720 636f  ion modelling co
-000040f0: 6d70 6c65 7465 642e 2229 0d0a 2020 2020  mpleted.")..    
-00004100: 2020 2020 0d0a 2020 2020 6465 6620 7365      ..    def se
-00004110: 6c65 6374 5f6f 7665 7264 6973 7065 7273  lect_overdispers
-00004120: 6564 5f67 656e 6573 5f66 726f 6d5f 6765  ed_genes_from_ge
-00004130: 6e65 6c69 7374 2873 656c 662c 2067 656e  nelist(self, gen
-00004140: 6573 3a20 436f 6c6c 6563 7469 6f6e 2c20  es: Collection, 
-00004150: 6d69 6e5f 6d65 616e 3d30 293a 0d0a 2020  min_mean=0):..  
-00004160: 2020 2020 2020 2222 2253 656c 6563 7420        """Select 
-00004170: 6f76 6572 6469 7370 6572 7365 6420 6765  overdispersed ge
-00004180: 6e65 732f 6665 6174 7572 6573 2075 7369  nes/features usi
-00004190: 6e67 2061 2063 7573 746f 6d20 6c69 7374  ng a custom list
-000041a0: 2e20 4765 6e65 732f 6665 6174 7572 6573  . Genes/features
-000041b0: 206e 6f74 2070 7265 7365 6e74 2069 6e20   not present in 
-000041c0: 7468 6520 6461 7461 7365 7420 6172 6520  the dataset are 
-000041d0: 6175 746f 6d61 7469 6361 6c6c 7920 6669  automatically fi
-000041e0: 6c74 6572 6564 206f 7574 2e0d 0a0d 0a20  ltered out..... 
-000041f0: 2020 2020 2020 203a 7061 7261 6d20 6765         :param ge
-00004200: 6e65 733a 2067 656e 6520 6c69 7374 0d0a  nes: gene list..
-00004210: 2020 2020 2020 2020 3a74 7970 6520 6765          :type ge
-00004220: 6e65 733a 2043 6f6c 6c65 6374 696f 6e0d  nes: Collection.
-00004230: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-00004240: 6d69 6e5f 6d65 616e 3a20 6d69 6e69 6d75  min_mean: minimu
-00004250: 6d20 6765 6e65 2065 7870 7265 7373 696f  m gene expressio
-00004260: 6e20 666f 7220 6765 6e65 7320 746f 2062  n for genes to b
-00004270: 6520 636f 756e 7465 6420 6173 206f 7665  e counted as ove
-00004280: 7264 6973 7065 7273 6564 2c20 6465 6661  rdispersed, defa
-00004290: 756c 7473 2074 6f20 300d 0a20 2020 2020  ults to 0..     
-000042a0: 2020 203a 7479 7065 206d 696e 5f6d 6561     :type min_mea
-000042b0: 6e3a 2069 6e74 2c20 6f70 7469 6f6e 616c  n: int, optional
-000042c0: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
-000042d0: 2020 2020 2020 2073 656c 662e 6164 6174         self.adat
-000042e0: 612e 7661 725b 2273 656c 6563 7465 6422  a.var["selected"
-000042f0: 5d20 3d20 7365 6c66 2e61 6461 7461 2e76  ] = self.adata.v
-00004300: 6172 2e69 6e64 6578 2e69 7369 6e28 6765  ar.index.isin(ge
-00004310: 6e65 7329 2026 2073 656c 662e 6164 6174  nes) & self.adat
-00004320: 612e 7661 725b 226d 6561 6e5f 636f 756e  a.var["mean_coun
-00004330: 7473 225d 203e 3d20 6d69 6e5f 6d65 616e  ts"] >= min_mean
-00004340: 0d0a 2020 2020 2020 2020 7365 6c66 2e61  ..        self.a
-00004350: 6461 7461 2e75 6e73 5b22 6f64 6722 5d5b  data.uns["odg"][
-00004360: 226f 7665 7264 6973 7065 7273 696f 6e5f  "overdispersion_
-00004370: 6d65 7472 6963 225d 203d 2022 220d 0a20  metric"] = "".. 
-00004380: 2020 2020 2020 2073 656c 662e 6164 6174         self.adat
-00004390: 612e 756e 735b 226f 6467 225d 5b22 6d69  a.uns["odg"]["mi
-000043a0: 6e5f 6d65 616e 225d 203d 206d 696e 5f6d  n_mean"] = min_m
-000043b0: 6561 6e0d 0a20 2020 2020 2020 2073 656c  ean..        sel
-000043c0: 662e 6164 6174 612e 756e 735b 226f 6467  f.adata.uns["odg
-000043d0: 225d 5b22 6d69 6e5f 7363 6f72 6522 5d20  "]["min_score"] 
-000043e0: 3d20 2222 0d0a 2020 2020 2020 2020 7365  = ""..        se
-000043f0: 6c66 2e61 6461 7461 2e75 6e73 5b22 6f64  lf.adata.uns["od
-00004400: 6722 5d5b 2274 6f70 5f6e 225d 203d 2022  g"]["top_n"] = "
-00004410: 220d 0a20 2020 2020 2020 2073 656c 662e  "..        self.
-00004420: 6164 6174 612e 756e 735b 226f 6467 225d  adata.uns["odg"]
-00004430: 5b22 7175 616e 7469 6c65 225d 203d 2022  ["quantile"] = "
-00004440: 220d 0a20 2020 2020 2020 2073 656c 662e  "..        self.
-00004450: 6170 7065 6e64 5f74 6f5f 6869 7374 6f72  append_to_histor
-00004460: 7928 224f 7665 7264 6973 7065 7273 6564  y("Overdispersed
-00004470: 2067 656e 6573 2073 656c 6563 7465 6420   genes selected 
-00004480: 6672 6f6d 2063 7573 746f 6d20 6765 6e65  from custom gene
-00004490: 206c 6973 7422 290d 0a20 2020 2020 2020   list")..       
-000044a0: 200d 0a20 2020 2064 6566 2073 656c 6563   ..    def selec
-000044b0: 745f 6f76 6572 6469 7370 6572 7365 645f  t_overdispersed_
-000044c0: 6765 6e65 7328 7365 6c66 2c0d 0a20 2020  genes(self,..   
-000044d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000044e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000044f0: 6f76 6572 6469 7370 6572 7369 6f6e 5f6d  overdispersion_m
-00004500: 6574 7269 633a 2073 7472 203d 2022 6f64  etric: str = "od
-00004510: 7363 6f72 6522 2c0d 0a20 2020 2020 2020  score",..       
-00004520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004530: 2020 2020 2020 2020 2020 2020 6d69 6e5f              min_
-00004540: 6d65 616e 3a20 666c 6f61 7420 3d20 302c  mean: float = 0,
-00004550: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00004560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004570: 2020 2020 206d 696e 5f73 636f 7265 3a20       min_score: 
-00004580: 666c 6f61 7420 3d20 312e 302c 0d0a 2020  float = 1.0,..  
-00004590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000045a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000045b0: 2074 6f70 5f6e 3a20 696e 7420 3d20 4e6f   top_n: int = No
-000045c0: 6e65 2c0d 0a20 2020 2020 2020 2020 2020  ne,..           
-000045d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000045e0: 2020 2020 2020 2020 7175 616e 7469 6c65          quantile
-000045f0: 3a20 666c 6f61 7420 3d20 4e6f 6e65 293a  : float = None):
-00004600: 0d0a 2020 2020 2020 2020 2222 2253 656c  ..        """Sel
-00004610: 6563 7420 6f76 6572 6469 7370 6572 7365  ect overdisperse
-00004620: 6420 6765 6e65 732f 6665 6174 7572 6573  d genes/features
-00004630: 2075 7369 6e67 2061 6e20 6f76 6572 6469   using an overdi
-00004640: 7370 6572 7369 6f6e 206d 6574 7269 632e  spersion metric.
-00004650: 204f 7074 696f 6e61 6c6c 7920 7365 7420   Optionally set 
-00004660: 6120 6d69 6e69 6d75 6d20 6765 6e65 2065  a minimum gene e
-00004670: 7870 7265 7373 696f 6e20 6c65 7665 6c2e  xpression level.
-00004680: 0d0a 2020 2020 2020 2020 5365 7420 6120  ..        Set a 
-00004690: 7468 7265 7368 6f6c 6420 7573 696e 6720  threshold using 
-000046a0: 7468 6520 746f 7020 4e20 2827 746f 705f  the top N ('top_
-000046b0: 6e27 292c 206d 696e 696d 756d 2073 636f  n'), minimum sco
-000046c0: 7265 2028 276d 696e 5f73 636f 7265 2729  re ('min_score')
-000046d0: 2c20 6f72 2070 726f 706f 7274 696f 6e20  , or proportion 
-000046e0: 6f66 2066 6561 7475 7265 7320 2827 7175  of features ('qu
-000046f0: 616e 7469 6c65 2729 206d 6574 686f 6473  antile') methods
-00004700: 2e0d 0a20 2020 2020 2020 204f 7665 7264  ...        Overd
-00004710: 6973 7065 7273 6564 2067 656e 6520 6c69  ispersed gene li
-00004720: 7374 2069 7320 7361 7665 6420 696e 2074  st is saved in t
-00004730: 6865 2044 6174 6173 6574 206f 626a 6563  he Dataset objec
-00004740: 742e 0d0a 0d0a 2020 2020 2020 2020 3a70  t.....        :p
-00004750: 6172 616d 206f 7665 7264 6973 7065 7273  aram overdispers
-00004760: 696f 6e5f 6d65 7472 6963 3a20 226f 6473  ion_metric: "ods
-00004770: 636f 7265 2220 6f72 2022 7673 636f 7265  core" or "vscore
-00004780: 222c 2064 6566 6175 6c74 7320 746f 2022  ", defaults to "
-00004790: 6f64 7363 6f72 6522 0d0a 2020 2020 2020  odscore"..      
-000047a0: 2020 3a74 7970 6520 6f76 6572 6469 7370    :type overdisp
-000047b0: 6572 7369 6f6e 5f6d 6574 7269 633a 2073  ersion_metric: s
-000047c0: 7472 2c20 6f70 7469 6f6e 616c 0d0a 2020  tr, optional..  
-000047d0: 2020 2020 2020 3a70 6172 616d 206d 696e        :param min
-000047e0: 5f6d 6561 6e3a 206d 696e 696d 756d 2067  _mean: minimum g
-000047f0: 656e 6520 6578 7072 6573 7369 6f6e 2066  ene expression f
-00004800: 6f72 2067 656e 6573 2074 6f20 6265 2063  or genes to be c
-00004810: 6f75 6e74 6564 2061 7320 6f76 6572 6469  ounted as overdi
-00004820: 7370 6572 7365 642c 2064 6566 6175 6c74  spersed, default
-00004830: 7320 746f 2030 0d0a 2020 2020 2020 2020  s to 0..        
-00004840: 3a74 7970 6520 6d69 6e5f 6d65 616e 3a20  :type min_mean: 
-00004850: 696e 742c 206f 7074 696f 6e61 6c0d 0a20  int, optional.. 
-00004860: 2020 2020 2020 203a 7061 7261 6d20 6d69         :param mi
-00004870: 6e5f 7363 6f72 653a 206d 696e 696d 756d  n_score: minimum
-00004880: 2073 636f 7265 2066 6f72 206f 7665 7264   score for overd
-00004890: 6973 7065 7273 696f 6e2c 2064 6566 6175  ispersion, defau
-000048a0: 6c74 7320 746f 2031 2e30 0d0a 2020 2020  lts to 1.0..    
-000048b0: 2020 2020 3a74 7970 6520 6d69 6e5f 7363      :type min_sc
-000048c0: 6f72 653a 2066 6c6f 6174 2c20 6f70 7469  ore: float, opti
-000048d0: 6f6e 616c 0d0a 2020 2020 2020 2020 3a70  onal..        :p
-000048e0: 6172 616d 2074 6f70 5f6e 3a20 4368 6f6f  aram top_n: Choo
-000048f0: 7365 2074 6865 2074 6f70 204e 206d 6f73  se the top N mos
-00004900: 7420 6f76 6572 6469 7370 6572 7365 6420  t overdispersed 
-00004910: 6765 6e65 732c 2064 6566 6175 6c74 7320  genes, defaults 
-00004920: 746f 204e 6f6e 650d 0a20 2020 2020 2020  to None..       
-00004930: 203a 7479 7065 2074 6f70 5f6e 3a20 696e   :type top_n: in
-00004940: 742c 206f 7074 696f 6e61 6c0d 0a20 2020  t, optional..   
-00004950: 2020 2020 203a 7061 7261 6d20 7175 616e       :param quan
-00004960: 7469 6c65 3a20 4368 6f6f 7365 2061 2071  tile: Choose a q
-00004970: 7561 6e74 696c 6520 6f66 206f 7665 7264  uantile of overd
-00004980: 6973 7065 7273 696f 6e2e 2046 6f72 2065  ispersion. For e
-00004990: 7861 6d70 6c65 2c20 7468 6520 746f 7020  xample, the top 
-000049a0: 3130 2520 6f66 206f 7665 7264 6973 7065  10% of overdispe
-000049b0: 7273 6564 2067 656e 6573 2077 6f75 6c64  rsed genes would
-000049c0: 2062 6520 302e 3130 2e20 4465 6661 756c   be 0.10. Defaul
-000049d0: 7473 2074 6f20 4e6f 6e65 0d0a 2020 2020  ts to None..    
-000049e0: 2020 2020 3a74 7970 6520 7175 616e 7469      :type quanti
-000049f0: 6c65 3a20 666c 6f61 742c 206f 7074 696f  le: float, optio
-00004a00: 6e61 6c0d 0a20 2020 2020 2020 203a 7261  nal..        :ra
-00004a10: 6973 6573 2056 616c 7565 4572 726f 723a  ises ValueError:
-00004a20: 2045 7272 6f72 2069 6620 696e 7661 6c69   Error if invali
-00004a30: 6420 6f76 6572 6469 7370 6572 7369 6f6e  d overdispersion
-00004a40: 206d 6574 7269 6320 6973 2063 686f 7365   metric is chose
-00004a50: 6e2e 0d0a 2020 2020 2020 2020 2222 220d  n...        """.
-00004a60: 0a20 2020 2020 2020 200d 0a20 2020 2020  .        ..     
-00004a70: 2020 2069 6620 6f76 6572 6469 7370 6572     if overdisper
-00004a80: 7369 6f6e 5f6d 6574 7269 6320 6e6f 7420  sion_metric not 
-00004a90: 696e 2073 656c 662e 6164 6174 612e 7661  in self.adata.va
-00004aa0: 722e 636f 6c75 6d6e 733a 0d0a 2020 2020  r.columns:..    
-00004ab0: 2020 2020 2020 2020 6966 206f 7665 7264          if overd
-00004ac0: 6973 7065 7273 696f 6e5f 6d65 7472 6963  ispersion_metric
-00004ad0: 2069 6e20 2822 6f64 7363 6f72 6522 2c20   in ("odscore", 
-00004ae0: 2276 7363 6f72 6522 293a 0d0a 2020 2020  "vscore"):..    
-00004af0: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-00004b00: 6520 5661 6c75 6545 7272 6f72 280d 0a20  e ValueError(.. 
-00004b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004b20: 2020 2066 227b 6f76 6572 6469 7370 6572     f"{overdisper
-00004b30: 7369 6f6e 5f6d 6574 7269 637d 2068 6173  sion_metric} has
-00004b40: 206e 6f74 2062 6565 6e20 6361 6c63 756c   not been calcul
-00004b50: 6174 6564 2066 6f72 2074 6869 7320 6461  ated for this da
-00004b60: 7461 7365 742e 2022 0d0a 2020 2020 2020  taset. "..      
-00004b70: 2020 2020 2020 2020 2020 2020 2020 2245                "E
-00004b80: 6e73 7572 6520 7468 6174 2079 6f75 2063  nsure that you c
-00004b90: 616c 6c20 7468 6520 6044 6174 6173 6574  all the `Dataset
-00004ba0: 2e63 6f6d 7075 7465 5f67 656e 655f 7374  .compute_gene_st
-00004bb0: 6174 7328 2960 2066 6972 7374 2e22 0d0a  ats()` first."..
-00004bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004bd0: 2020 2020 290d 0a20 2020 2020 2020 2020      )..         
-00004be0: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
-00004bf0: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-00004c00: 5661 6c75 6545 7272 6f72 280d 0a20 2020  ValueError(..   
-00004c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004c20: 2066 227b 6f76 6572 6469 7370 6572 7369   f"{overdispersi
-00004c30: 6f6e 5f6d 6574 7269 637d 2069 7320 6e6f  on_metric} is no
-00004c40: 7420 6120 7661 6c69 6420 6f76 6572 6469  t a valid overdi
-00004c50: 7370 6572 7369 6f6e 206d 6574 7269 632e  spersion metric.
-00004c60: 220d 0a20 2020 2020 2020 2020 2020 2020  "..             
-00004c70: 2020 2020 2020 2029 0d0a 2020 2020 2020         )..      
-00004c80: 2020 0d0a 2020 2020 2020 2020 2320 7761    ..        # wa
-00004c90: 726e 2069 6620 6d75 6c74 6970 6c65 206d  rn if multiple m
-00004ca0: 6574 686f 6473 2061 7265 2073 656c 6563  ethods are selec
-00004cb0: 7465 640d 0a20 2020 2020 2020 2073 656c  ted..        sel
-00004cc0: 6563 7465 645f 6d65 7468 6f64 7320 3d20  ected_methods = 
-00004cd0: 5b5d 0d0a 2020 2020 2020 2020 6966 206d  []..        if m
-00004ce0: 696e 5f73 636f 7265 2069 7320 6e6f 7420  in_score is not 
-00004cf0: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2020  None:..         
-00004d00: 2020 2073 656c 6563 7465 645f 6d65 7468     selected_meth
-00004d10: 6f64 732e 6170 7065 6e64 2822 6d69 6e5f  ods.append("min_
-00004d20: 7363 6f72 6522 290d 0a20 2020 2020 2020  score")..       
-00004d30: 2069 6620 746f 705f 6e20 6973 206e 6f74   if top_n is not
-00004d40: 204e 6f6e 653a 0d0a 2020 2020 2020 2020   None:..        
-00004d50: 2020 2020 7365 6c65 6374 6564 5f6d 6574      selected_met
-00004d60: 686f 6473 2e61 7070 656e 6428 2274 6f70  hods.append("top
-00004d70: 5f6e 2229 0d0a 2020 2020 2020 2020 6966  _n")..        if
-00004d80: 2071 7561 6e74 696c 6520 6973 206e 6f74   quantile is not
-00004d90: 204e 6f6e 653a 0d0a 2020 2020 2020 2020   None:..        
-00004da0: 2020 2020 7365 6c65 6374 6564 5f6d 6574      selected_met
-00004db0: 686f 6473 2e61 7070 656e 6428 2271 7561  hods.append("qua
-00004dc0: 6e74 696c 6522 290d 0a20 2020 2020 2020  ntile")..       
-00004dd0: 2069 6620 6c65 6e28 7365 6c65 6374 6564   if len(selected
-00004de0: 5f6d 6574 686f 6473 2920 3e20 313a 0d0a  _methods) > 1:..
-00004df0: 2020 2020 2020 2020 2020 2020 6d65 7468              meth
-00004e00: 6f64 7761 726e 7374 7220 3d20 222c 2022  odwarnstr = ", "
-00004e10: 2e6a 6f69 6e28 7365 6c65 6374 6564 5f6d  .join(selected_m
-00004e20: 6574 686f 6473 290d 0a20 2020 2020 2020  ethods)..       
-00004e30: 2020 2020 206c 6f67 6769 6e67 2e77 6172       logging.war
-00004e40: 6e69 6e67 2866 224d 756c 7469 706c 6520  ning(f"Multiple 
-00004e50: 636f 6e66 6c69 6374 696e 6720 6f76 6572  conflicting over
-00004e60: 6469 7370 6572 7365 6420 6765 6e65 2073  dispersed gene s
-00004e70: 656c 6563 7469 6f6e 2063 7269 7465 7269  election criteri
-00004e80: 6120 6861 7665 2062 6565 6e20 7365 6c65  a have been sele
-00004e90: 6374 6564 3a20 7b6d 6574 686f 6477 6172  cted: {methodwar
-00004ea0: 6e73 7472 7d2e 2022 0d0a 2020 2020 2020  nstr}. "..      
-00004eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004ec0: 2020 2020 2020 224f 6e6c 7920 7468 6520        "Only the 
-00004ed0: 696e 7465 7273 6563 7469 6f6e 206f 6620  intersection of 
-00004ee0: 7468 6573 6520 6d65 7468 6f64 7320 7769  these methods wi
-00004ef0: 6c6c 2062 6520 7365 6c65 6374 6564 2e22  ll be selected."
-00004f00: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00004f10: 2020 200d 0a20 2020 2020 2020 2023 206d     ..        # m
-00004f20: 696e 5f6d 6561 6e20 6669 6c74 6572 0d0a  in_mean filter..
-00004f30: 2020 2020 2020 2020 7365 6c65 6374 6564          selected
-00004f40: 5f67 656e 6573 203d 2073 656c 662e 6164  _genes = self.ad
-00004f50: 6174 612e 7661 725b 226d 6561 6e5f 636f  ata.var["mean_co
-00004f60: 756e 7473 225d 203e 3d20 6d69 6e5f 6d65  unts"] >= min_me
-00004f70: 616e 0d0a 2020 2020 2020 2020 2320 6d69  an..        # mi
-00004f80: 6e5f 7363 6f72 6520 6669 6c74 6572 0d0a  n_score filter..
-00004f90: 2020 2020 2020 2020 6966 206d 696e 5f73          if min_s
-00004fa0: 636f 7265 2069 7320 6e6f 7420 4e6f 6e65  core is not None
-00004fb0: 3a0d 0a20 2020 2020 2020 2020 2020 2073  :..            s
-00004fc0: 656c 6563 7465 645f 6765 6e65 7320 3d20  elected_genes = 
-00004fd0: 7365 6c65 6374 6564 5f67 656e 6573 2026  selected_genes &
-00004fe0: 2028 7365 6c66 2e61 6461 7461 2e76 6172   (self.adata.var
-00004ff0: 5b6f 7665 7264 6973 7065 7273 696f 6e5f  [overdispersion_
-00005000: 6d65 7472 6963 5d20 3e3d 206d 696e 5f73  metric] >= min_s
-00005010: 636f 7265 290d 0a20 2020 2020 2020 2023  core)..        #
-00005020: 2074 6f70 5f6e 2066 696c 7465 720d 0a20   top_n filter.. 
-00005030: 2020 2020 2020 2069 6620 746f 705f 6e20         if top_n 
-00005040: 6973 206e 6f74 204e 6f6e 653a 0d0a 2020  is not None:..  
-00005050: 2020 2020 2020 2020 2020 6765 6e65 7320            genes 
-00005060: 3d20 7365 6c66 2e61 6461 7461 2e76 6172  = self.adata.var
-00005070: 5b6f 7665 7264 6973 7065 7273 696f 6e5f  [overdispersion_
-00005080: 6d65 7472 6963 5d2e 736f 7274 5f76 616c  metric].sort_val
-00005090: 7565 7328 6173 6365 6e64 696e 673d 4661  ues(ascending=Fa
-000050a0: 6c73 6529 2e68 6561 6428 696e 7428 746f  lse).head(int(to
-000050b0: 705f 6e29 292e 696e 6465 780d 0a20 2020  p_n)).index..   
-000050c0: 2020 2020 2020 2020 2073 656c 6563 7465           selecte
-000050d0: 645f 6765 6e65 7320 3d20 7365 6c65 6374  d_genes = select
-000050e0: 6564 5f67 656e 6573 2026 2073 656c 662e  ed_genes & self.
-000050f0: 6164 6174 612e 7661 722e 696e 6465 782e  adata.var.index.
-00005100: 6973 696e 2867 656e 6573 290d 0a20 2020  isin(genes)..   
-00005110: 2020 2020 2023 2071 7561 6e74 696c 6520       # quantile 
-00005120: 6669 6c74 6572 0d0a 2020 2020 2020 2020  filter..        
-00005130: 6966 2071 7561 6e74 696c 6520 6973 206e  if quantile is n
-00005140: 6f74 204e 6f6e 653a 0d0a 2020 2020 2020  ot None:..      
-00005150: 2020 2020 2020 6e5f 746f 7461 6c5f 6765        n_total_ge
-00005160: 6e65 7320 3d20 7365 6c66 2e61 6461 7461  nes = self.adata
-00005170: 2e76 6172 5b6f 7665 7264 6973 7065 7273  .var[overdispers
-00005180: 696f 6e5f 6d65 7472 6963 5d2e 6e6f 746e  ion_metric].notn
-00005190: 756c 6c28 292e 7375 6d28 290d 0a20 2020  ull().sum()..   
-000051a0: 2020 2020 2020 2020 2067 656e 6573 203d           genes =
-000051b0: 2073 656c 662e 6164 6174 612e 7661 725b   self.adata.var[
-000051c0: 6f76 6572 6469 7370 6572 7369 6f6e 5f6d  overdispersion_m
-000051d0: 6574 7269 635d 2e73 6f72 745f 7661 6c75  etric].sort_valu
-000051e0: 6573 2861 7363 656e 6469 6e67 3d46 616c  es(ascending=Fal
-000051f0: 7365 292e 6865 6164 2869 6e74 2871 7561  se).head(int(qua
-00005200: 6e74 696c 6520 2a20 6e5f 746f 7461 6c5f  ntile * n_total_
-00005210: 6765 6e65 7329 292e 696e 6465 780d 0a20  genes)).index.. 
-00005220: 2020 2020 2020 2020 2020 2073 656c 6563             selec
-00005230: 7465 645f 6765 6e65 7320 3d20 7365 6c65  ted_genes = sele
-00005240: 6374 6564 5f67 656e 6573 2026 2073 656c  cted_genes & sel
-00005250: 662e 6164 6174 612e 7661 722e 696e 6465  f.adata.var.inde
-00005260: 782e 6973 696e 2867 656e 6573 290d 0a0d  x.isin(genes)...
-00005270: 0a20 2020 2020 2020 206e 5f73 656c 6563  .        n_selec
-00005280: 7465 645f 6765 6e65 7320 3d20 7365 6c65  ted_genes = sele
-00005290: 6374 6564 5f67 656e 6573 2e73 756d 2829  cted_genes.sum()
-000052a0: 0d0a 2020 2020 2020 2020 6c6f 6767 696e  ..        loggin
-000052b0: 672e 696e 666f 2866 227b 6e5f 7365 6c65  g.info(f"{n_sele
-000052c0: 6374 6564 5f67 656e 6573 7d20 6765 6e65  cted_genes} gene
-000052d0: 7320 7365 6c65 6374 6564 2066 6f72 2066  s selected for f
-000052e0: 6163 746f 7269 7a61 7469 6f6e 2229 0d0a  actorization")..
-000052f0: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-00005300: 2020 2320 6d61 6b65 2063 6861 6e67 6573    # make changes
-00005310: 2074 6f20 4461 7461 7365 7420 6f62 6a65   to Dataset obje
-00005320: 6374 0d0a 2020 2020 2020 2020 7365 6c66  ct..        self
-00005330: 2e61 6461 7461 2e76 6172 5b22 7365 6c65  .adata.var["sele
-00005340: 6374 6564 225d 203d 2073 656c 6563 7465  cted"] = selecte
-00005350: 645f 6765 6e65 730d 0a20 2020 2020 2020  d_genes..       
-00005360: 2073 656c 662e 6164 6174 612e 756e 735b   self.adata.uns[
-00005370: 226f 6467 225d 5b22 6f76 6572 6469 7370  "odg"]["overdisp
-00005380: 6572 7369 6f6e 5f6d 6574 7269 6322 5d20  ersion_metric"] 
-00005390: 3d20 6f76 6572 6469 7370 6572 7369 6f6e  = overdispersion
-000053a0: 5f6d 6574 7269 630d 0a20 2020 2020 2020  _metric..       
-000053b0: 2073 656c 662e 6164 6174 612e 756e 735b   self.adata.uns[
-000053c0: 226f 6467 225d 5b22 6d69 6e5f 6d65 616e  "odg"]["min_mean
-000053d0: 225d 203d 206d 696e 5f6d 6561 6e0d 0a20  "] = min_mean.. 
-000053e0: 2020 2020 2020 2073 656c 662e 6164 6174         self.adat
-000053f0: 612e 756e 735b 226f 6467 225d 5b22 6d69  a.uns["odg"]["mi
-00005400: 6e5f 7363 6f72 6522 5d20 3d20 6d69 6e5f  n_score"] = min_
-00005410: 7363 6f72 6520 6966 206d 696e 5f73 636f  score if min_sco
-00005420: 7265 2069 7320 6e6f 7420 4e6f 6e65 2065  re is not None e
-00005430: 6c73 6520 2222 0d0a 2020 2020 2020 2020  lse ""..        
-00005440: 7365 6c66 2e61 6461 7461 2e75 6e73 5b22  self.adata.uns["
-00005450: 6f64 6722 5d5b 2274 6f70 5f6e 225d 203d  odg"]["top_n"] =
-00005460: 2074 6f70 5f6e 2069 6620 746f 705f 6e20   top_n if top_n 
-00005470: 6973 206e 6f74 204e 6f6e 6520 656c 7365  is not None else
-00005480: 2022 220d 0a20 2020 2020 2020 2073 656c   ""..        sel
-00005490: 662e 6164 6174 612e 756e 735b 226f 6467  f.adata.uns["odg
-000054a0: 225d 5b22 7175 616e 7469 6c65 225d 203d  "]["quantile"] =
-000054b0: 2071 7561 6e74 696c 6520 6966 2071 7561   quantile if qua
-000054c0: 6e74 696c 6520 6973 206e 6f74 204e 6f6e  ntile is not Non
-000054d0: 6520 656c 7365 2022 220d 0a20 2020 2020  e else ""..     
-000054e0: 2020 2073 656c 662e 6170 7065 6e64 5f74     self.append_t
-000054f0: 6f5f 6869 7374 6f72 7928 224f 7665 7264  o_history("Overd
-00005500: 6973 7065 7273 6564 2067 656e 6573 2073  ispersed genes s
-00005510: 656c 6563 7465 6422 290d 0a20 2020 200d  elected")..    .
-00005520: 0a20 2020 2064 6566 2069 6e69 7469 616c  .    def initial
-00005530: 697a 655f 636e 6d66 2873 656c 662c 2063  ize_cnmf(self, c
-00005540: 6e6d 665f 6f75 7470 7574 5f64 6972 3a20  nmf_output_dir: 
-00005550: 7374 722c 0d0a 2020 2020 2020 2020 2020  str,..          
-00005560: 2020 2020 2020 2020 2020 2020 2020 636e                cn
-00005570: 6d66 5f6e 616d 653a 2073 7472 2c0d 0a20  mf_name: str,.. 
-00005580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005590: 2020 2020 2020 206b 7661 6c73 3a20 436f         kvals: Co
-000055a0: 6c6c 6563 7469 6f6e 203d 2072 616e 6765  llection = range
-000055b0: 2832 2c20 3631 292c 0d0a 2020 2020 2020  (2, 61),..      
-000055c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000055d0: 2020 6e5f 6974 6572 3a20 696e 7420 3d20    n_iter: int = 
-000055e0: 3230 302c 0d0a 2020 2020 2020 2020 2020  200,..          
-000055f0: 2020 2020 2020 2020 2020 2020 2020 6265                be
-00005600: 7461 5f6c 6f73 733a 2073 7472 203d 2022  ta_loss: str = "
-00005610: 6b75 6c6c 6261 636b 2d6c 6569 626c 6572  kullback-leibler
-00005620: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-00005630: 2020 2020 2020 2020 2020 2020 7365 6564              seed
-00005640: 3a20 4f70 7469 6f6e 616c 5b69 6e74 5d20  : Optional[int] 
-00005650: 3d20 4e6f 6e65 2920 2d3e 2063 6e6d 662e  = None) -> cnmf.
-00005660: 634e 4d46 3a0d 0a20 2020 2020 2020 2022  cNMF:..        "
-00005670: 2222 496e 6974 6961 6c69 7a65 2061 2063  ""Initialize a c
-00005680: 4e4d 4620 7275 6e20 666f 7220 7375 6273  NMF run for subs
-00005690: 6571 7565 6e74 2066 6163 746f 7269 7a61  equent factoriza
-000056a0: 7469 6f6e 2e0d 0a0d 0a20 2020 2020 2020  tion.....       
-000056b0: 203a 7061 7261 6d20 636e 6d66 5f6f 7574   :param cnmf_out
-000056c0: 7075 745f 6469 723a 204f 7574 7075 7420  put_dir: Output 
-000056d0: 6469 7265 6374 6f72 7920 666f 7220 634e  directory for cN
-000056e0: 4d46 2072 6573 756c 7473 0d0a 2020 2020  MF results..    
-000056f0: 2020 2020 3a74 7970 6520 636e 6d66 5f6f      :type cnmf_o
-00005700: 7574 7075 745f 6469 723a 2073 7472 0d0a  utput_dir: str..
-00005710: 2020 2020 2020 2020 3a70 6172 616d 2063          :param c
-00005720: 6e6d 665f 6e61 6d65 3a20 4e61 6d65 206f  nmf_name: Name o
-00005730: 6620 7468 6520 634e 4d46 2072 6573 756c  f the cNMF resul
-00005740: 7473 2e20 4669 6c65 7320 7769 6c6c 2062  ts. Files will b
-00005750: 6520 6f75 7470 7574 2074 6f20 5b63 6e6d  e output to [cnm
-00005760: 665f 6f75 7470 7574 5f64 6972 5d2f 5b63  f_output_dir]/[c
-00005770: 6e6d 665f 6e61 6d65 5d2f 0d0a 2020 2020  nmf_name]/..    
-00005780: 2020 2020 3a74 7970 6520 636e 6d66 5f6e      :type cnmf_n
-00005790: 616d 653a 2073 7472 0d0a 2020 2020 2020  ame: str..      
-000057a0: 2020 3a70 6172 616d 206b 7661 6c73 3a20    :param kvals: 
-000057b0: 5261 6e6b 7320 666f 7220 634e 4d46 2066  Ranks for cNMF f
-000057c0: 6163 746f 7269 7a61 7469 6f6e 2c20 6465  actorization, de
-000057d0: 6661 756c 7473 2074 6f20 7261 6e67 6528  faults to range(
-000057e0: 322c 2036 3129 0d0a 2020 2020 2020 2020  2, 61)..        
-000057f0: 3a74 7970 6520 6b76 616c 733a 2043 6f6c  :type kvals: Col
-00005800: 6c65 6374 696f 6e2c 206f 7074 696f 6e61  lection, optiona
-00005810: 6c0d 0a20 2020 2020 2020 203a 7061 7261  l..        :para
-00005820: 6d20 6e5f 6974 6572 3a20 4e75 6d62 6572  m n_iter: Number
-00005830: 206f 6620 6974 6572 6174 696f 6e73 2066   of iterations f
-00005840: 726f 6d20 7768 6963 6820 746f 2062 7569  rom which to bui
-00005850: 6c64 2061 2063 6f6e 7365 6e73 7573 2073  ld a consensus s
-00005860: 6f6c 7574 696f 6e2c 2064 6566 6175 6c74  olution, default
-00005870: 7320 746f 2032 3030 0d0a 2020 2020 2020  s to 200..      
-00005880: 2020 3a74 7970 6520 6e5f 6974 6572 3a20    :type n_iter: 
-00005890: 696e 742c 206f 7074 696f 6e61 6c0d 0a20  int, optional.. 
-000058a0: 2020 2020 2020 203a 7061 7261 6d20 6265         :param be
-000058b0: 7461 5f6c 6f73 733a 2062 6574 612d 6c6f  ta_loss: beta-lo
-000058c0: 7373 2066 756e 6374 696f 6e2c 2065 6974  ss function, eit
-000058d0: 6865 7220 226b 756c 6c62 6163 6b2d 6c65  her "kullback-le
-000058e0: 6962 6c65 7222 206f 7220 2266 726f 6265  ibler" or "frobe
-000058f0: 6e69 7573 222e 2044 6566 6175 6c74 7320  nius". Defaults 
-00005900: 746f 2022 6b75 6c6c 6261 636b 2d6c 6569  to "kullback-lei
-00005910: 626c 6572 220d 0a20 2020 2020 2020 203a  bler"..        :
-00005920: 7479 7065 2062 6574 615f 6c6f 7373 3a20  type beta_loss: 
-00005930: 7374 722c 206f 7074 696f 6e61 6c0d 0a20  str, optional.. 
-00005940: 2020 2020 2020 203a 7061 7261 6d20 7365         :param se
-00005950: 6564 3a20 5261 6e64 6f6d 2073 6565 6420  ed: Random seed 
-00005960: 666f 7220 7265 7072 6f64 7563 6962 696c  for reproducibil
-00005970: 6974 792c 2064 6566 6175 6c74 7320 746f  ity, defaults to
-00005980: 204e 6f6e 650d 0a20 2020 2020 2020 203a   None..        :
-00005990: 7479 7065 2073 6565 643a 204f 7074 696f  type seed: Optio
-000059a0: 6e61 6c5b 696e 745d 2c20 6f70 7469 6f6e  nal[int], option
-000059b0: 616c 0d0a 2020 2020 2020 2020 3a72 6574  al..        :ret
-000059c0: 7572 6e3a 2063 4e4d 4620 6f62 6a65 6374  urn: cNMF object
-000059d0: 0d0a 2020 2020 2020 2020 3a72 7479 7065  ..        :rtype
-000059e0: 3a20 3a63 6c61 7373 3a60 636e 6d66 736e  : :class:`cnmfsn
-000059f0: 732e 636e 6d66 2e63 4e4d 4660 0d0a 2020  s.cnmf.cNMF`..  
-00005a00: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
-00005a10: 2020 2063 6e6d 665f 6f62 6a20 3d20 636e     cnmf_obj = cn
-00005a20: 6d66 2e63 4e4d 4628 6f75 7470 7574 5f64  mf.cNMF(output_d
-00005a30: 6972 3d63 6e6d 665f 6f75 7470 7574 5f64  ir=cnmf_output_d
-00005a40: 6972 2c20 6e61 6d65 3d63 6e6d 665f 6e61  ir, name=cnmf_na
-00005a50: 6d65 290d 0a20 2020 2020 2020 200d 0a20  me)..        .. 
-00005a60: 2020 2020 2020 2023 2077 7269 7465 2054         # write T
-00005a70: 504d 2028 6e6f 726d 616c 697a 6564 2920  PM (normalized) 
-00005a80: 6461 7461 0d0a 2020 2020 2020 2020 7470  data..        tp
-00005a90: 6d20 3d20 6164 2e41 6e6e 4461 7461 2873  m = ad.AnnData(s
-00005aa0: 656c 662e 746f 5f64 6628 6e6f 726d 616c  elf.to_df(normal
-00005ab0: 697a 6564 3d54 7275 6529 290d 0a20 2020  ized=True))..   
-00005ac0: 2020 2020 2074 706d 2e77 7269 7465 5f68       tpm.write_h
-00005ad0: 3561 6428 636e 6d66 5f6f 626a 2e70 6174  5ad(cnmf_obj.pat
-00005ae0: 6873 5b22 7470 6d22 5d29 0d0a 0d0a 2020  hs["tpm"])....  
-00005af0: 2020 2020 2020 6765 6e65 5f74 706d 5f6d        gene_tpm_m
-00005b00: 6561 6e20 3d20 6e70 2e61 7272 6179 2874  ean = np.array(t
-00005b10: 706d 2e58 2e6d 6561 6e28 6178 6973 3d30  pm.X.mean(axis=0
-00005b20: 2929 2e72 6573 6861 7065 282d 3129 0d0a  )).reshape(-1)..
-00005b30: 2020 2020 2020 2020 6765 6e65 5f74 706d          gene_tpm
-00005b40: 5f73 7464 6465 7620 3d20 6e70 2e61 7272  _stddev = np.arr
-00005b50: 6179 2874 706d 2e58 2e73 7464 2861 7869  ay(tpm.X.std(axi
-00005b60: 733d 302c 2064 646f 663d 3029 292e 7265  s=0, ddof=0)).re
-00005b70: 7368 6170 6528 2d31 290d 0a20 2020 2020  shape(-1)..     
-00005b80: 2020 2069 6e70 7574 5f74 706d 5f73 7461     input_tpm_sta
-00005b90: 7473 203d 2070 642e 4461 7461 4672 616d  ts = pd.DataFram
-00005ba0: 6528 5b67 656e 655f 7470 6d5f 6d65 616e  e([gene_tpm_mean
-00005bb0: 2c20 6765 6e65 5f74 706d 5f73 7464 6465  , gene_tpm_stdde
-00005bc0: 765d 2c20 696e 6465 7820 3d20 5b27 5f5f  v], index = ['__
-00005bd0: 6d65 616e 272c 2027 5f5f 7374 6427 5d29  mean', '__std'])
-00005be0: 2e54 0d0a 2020 2020 2020 2020 7574 696c  .T..        util
-00005bf0: 732e 7361 7665 5f64 665f 746f 5f6e 707a  s.save_df_to_npz
-00005c00: 2869 6e70 7574 5f74 706d 5f73 7461 7473  (input_tpm_stats
-00005c10: 2c20 636e 6d66 5f6f 626a 2e70 6174 6873  , cnmf_obj.paths
-00005c20: 5b27 7470 6d5f 7374 6174 7327 5d29 0d0a  ['tpm_stats'])..
-00005c30: 2020 2020 2020 2020 6f76 6572 6469 7370          overdisp
-00005c40: 6572 7365 645f 6765 6e65 7320 3d20 7365  ersed_genes = se
-00005c50: 6c66 2e61 6461 7461 2e76 6172 5b22 7365  lf.adata.var["se
-00005c60: 6c65 6374 6564 225d 5b73 656c 662e 6164  lected"][self.ad
-00005c70: 6174 612e 7661 725b 2273 656c 6563 7465  ata.var["selecte
-00005c80: 6422 5d5d 2e69 6e64 6578 0d0a 2020 2020  d"]].index..    
-00005c90: 2020 2020 6e6f 726d 5f63 6f75 6e74 7320      norm_counts 
-00005ca0: 3d20 636e 6d66 5f6f 626a 2e67 6574 5f6e  = cnmf_obj.get_n
-00005cb0: 6f72 6d5f 636f 756e 7473 2873 656c 662e  orm_counts(self.
-00005cc0: 6164 6174 612c 2074 706d 2c20 6869 6768  adata, tpm, high
-00005cd0: 5f76 6172 6961 6e63 655f 6765 6e65 735f  _variance_genes_
-00005ce0: 6669 6c74 6572 3d6f 7665 7264 6973 7065  filter=overdispe
-00005cf0: 7273 6564 5f67 656e 6573 290d 0a20 2020  rsed_genes)..   
-00005d00: 2020 2020 2069 6620 6e6f 726d 5f63 6f75       if norm_cou
-00005d10: 6e74 732e 582e 6474 7970 6520 213d 206e  nts.X.dtype != n
-00005d20: 702e 666c 6f61 7436 343a 0d0a 2020 2020  p.float64:..    
-00005d30: 2020 2020 2020 2020 6e6f 726d 5f63 6f75          norm_cou
-00005d40: 6e74 732e 5820 3d20 6e6f 726d 5f63 6f75  nts.X = norm_cou
-00005d50: 6e74 732e 582e 6173 7479 7065 286e 702e  nts.X.astype(np.
-00005d60: 666c 6f61 7436 3429 0d0a 2020 2020 2020  float64)..      
-00005d70: 2020 636e 6d66 5f6f 626a 2e73 6176 655f    cnmf_obj.save_
-00005d80: 6e6f 726d 5f63 6f75 6e74 7328 6e6f 726d  norm_counts(norm
-00005d90: 5f63 6f75 6e74 7329 0d0a 0d0a 2020 2020  _counts)....    
-00005da0: 2020 2020 2320 7361 7665 2070 6172 616d      # save param
-00005db0: 6574 6572 7320 666f 7220 6661 6374 6f72  eters for factor
-00005dc0: 697a 6174 696f 6e20 7374 6570 0d0a 2020  ization step..  
-00005dd0: 2020 2020 2020 636e 6d66 5f6f 626a 2e73        cnmf_obj.s
-00005de0: 6176 655f 6e6d 665f 6974 6572 5f70 6172  ave_nmf_iter_par
-00005df0: 616d 7328 2a63 6e6d 665f 6f62 6a2e 6765  ams(*cnmf_obj.ge
-00005e00: 745f 6e6d 665f 6974 6572 5f70 6172 616d  t_nmf_iter_param
-00005e10: 7328 6b73 3d6b 7661 6c73 2c20 6e5f 6974  s(ks=kvals, n_it
-00005e20: 6572 3d6e 5f69 7465 722c 2072 616e 646f  er=n_iter, rando
-00005e30: 6d5f 7374 6174 655f 7365 6564 3d73 6565  m_state_seed=see
-00005e40: 642c 2062 6574 615f 6c6f 7373 3d62 6574  d, beta_loss=bet
-00005e50: 615f 6c6f 7373 2929 0d0a 0d0a 2020 2020  a_loss))....    
-00005e60: 2020 2020 2320 7361 7665 2070 6172 616d      # save param
-00005e70: 6574 6572 7320 696e 2041 6e6e 4461 7461  eters in AnnData
-00005e80: 206f 626a 6563 740d 0a20 2020 2020 2020   object..       
-00005e90: 2073 656c 662e 6164 6174 612e 756e 735b   self.adata.uns[
-00005ea0: 2263 6e6d 6622 5d20 3d20 636e 6d66 5f6f  "cnmf"] = cnmf_o
-00005eb0: 626a 2e67 6574 5f6e 6d66 5f69 7465 725f  bj.get_nmf_iter_
-00005ec0: 7061 7261 6d73 286b 733d 6b76 616c 732c  params(ks=kvals,
-00005ed0: 206e 5f69 7465 723d 6e5f 6974 6572 2c20   n_iter=n_iter, 
-00005ee0: 7261 6e64 6f6d 5f73 7461 7465 5f73 6565  random_state_see
-00005ef0: 643d 7365 6564 2c20 6265 7461 5f6c 6f73  d=seed, beta_los
-00005f00: 733d 6265 7461 5f6c 6f73 7329 5b31 5d20  s=beta_loss)[1] 
-00005f10: 2023 2064 6963 7420 6f66 2063 6e6d 6620   # dict of cnmf 
-00005f20: 7061 7261 6d65 7465 7273 0d0a 2020 2020  parameters..    
-00005f30: 2020 2020 0d0a 2020 2020 2020 2020 7365      ..        se
-00005f40: 6c66 2e61 7070 656e 645f 746f 5f68 6973  lf.append_to_his
-00005f50: 746f 7279 2866 2263 4e4d 4620 7061 7261  tory(f"cNMF para
-00005f60: 6d65 7465 7273 2061 6464 6564 2e20 634e  meters added. cN
-00005f70: 4d46 2069 6e70 7574 7320 696e 6974 6961  MF inputs initia
-00005f80: 6c69 7a65 6420 696e 207b 636e 6d66 5f6f  lized in {cnmf_o
-00005f90: 7574 7075 745f 6469 727d 2f7b 636e 6d66  utput_dir}/{cnmf
-00005fa0: 5f6e 616d 657d 2229 0d0a 2020 2020 2020  _name}")..      
-00005fb0: 2020 7265 7475 726e 2063 6e6d 665f 6f62    return cnmf_ob
-00005fc0: 6a0d 0a20 2020 200d 0a20 2020 2064 6566  j..    ..    def
-00005fd0: 2061 6464 5f63 6e6d 665f 7265 7375 6c74   add_cnmf_result
-00005fe0: 7328 7365 6c66 2c20 636e 6d66 5f6f 7574  s(self, cnmf_out
-00005ff0: 7075 745f 6469 722c 2063 6e6d 665f 6e61  put_dir, cnmf_na
-00006000: 6d65 2c20 6c6f 6361 6c5f 6465 6e73 6974  me, local_densit
-00006010: 795f 7468 7265 7368 6f6c 643a 2066 6c6f  y_threshold: flo
-00006020: 6174 203d 204e 6f6e 652c 206c 6f63 616c  at = None, local
-00006030: 5f6e 6569 6768 626f 7268 6f6f 645f 7369  _neighborhood_si
-00006040: 7a65 3a20 666c 6f61 7420 3d20 4e6f 6e65  ze: float = None
-00006050: 293a 0d0a 2020 2020 2020 2020 2222 220d  ):..        """.
-00006060: 0a20 2020 2020 2020 2041 6674 6572 2066  .        After f
-00006070: 6163 746f 7269 7a61 7469 6f6e 2c20 6164  actorization, ad
-00006080: 6420 636f 6d70 6c65 7465 6420 634e 4d46  d completed cNMF
-00006090: 2072 6573 756c 7473 2069 6e20 5b63 6e6d   results in [cnm
-000060a0: 665f 6f75 7470 7574 5f64 6972 5d2f 5b63  f_output_dir]/[c
-000060b0: 6e6d 665f 6e61 6d65 5d20 746f 2074 6865  nmf_name] to the
-000060c0: 2064 6174 6173 6574 206f 626a 6563 742e   dataset object.
-000060d0: 0d0a 0d0a 2020 2020 2020 2020 3a70 6172  ....        :par
-000060e0: 616d 2063 6e6d 665f 6f75 7470 7574 5f64  am cnmf_output_d
-000060f0: 6972 3a20 4f75 7470 7574 2064 6972 6563  ir: Output direc
-00006100: 746f 7279 2066 6f72 2063 4e4d 4620 7265  tory for cNMF re
-00006110: 7375 6c74 730d 0a20 2020 2020 2020 203a  sults..        :
-00006120: 7479 7065 2063 6e6d 665f 6f75 7470 7574  type cnmf_output
-00006130: 5f64 6972 3a20 7374 720d 0a20 2020 2020  _dir: str..     
-00006140: 2020 203a 7061 7261 6d20 636e 6d66 5f6e     :param cnmf_n
-00006150: 616d 653a 204e 616d 6520 6f66 2074 6865  ame: Name of the
-00006160: 2063 4e4d 4620 7265 7375 6c74 732e 2046   cNMF results. F
-00006170: 696c 6573 2077 696c 6c20 6265 206f 7574  iles will be out
-00006180: 7075 7420 746f 205b 636e 6d66 5f6f 7574  put to [cnmf_out
-00006190: 7075 745f 6469 725d 2f5b 636e 6d66 5f6e  put_dir]/[cnmf_n
-000061a0: 616d 655d 2f0d 0a20 2020 2020 2020 203a  ame]/..        :
-000061b0: 7479 7065 2063 6e6d 665f 6e61 6d65 3a20  type cnmf_name: 
-000061c0: 7374 720d 0a20 2020 2020 2020 203a 7061  str..        :pa
-000061d0: 7261 6d20 6c6f 6361 6c5f 6465 6e73 6974  ram local_densit
-000061e0: 795f 7468 7265 7368 6f6c 643a 2054 6872  y_threshold: Thr
-000061f0: 6573 686f 6c64 2066 6f72 2074 6865 206c  eshold for the l
-00006200: 6f63 616c 2064 656e 7369 7479 2066 696c  ocal density fil
-00006210: 7465 7269 6e67 2070 7269 6f72 2074 6f20  tering prior to 
-00006220: 4745 5020 636f 6e73 656e 7375 732e 2041  GEP consensus. A
-00006230: 6363 6570 7461 626c 6520 7468 7265 7368  cceptable thresh
-00006240: 6f6c 6473 2061 7265 203e 2030 2061 6e64  olds are > 0 and
-00006250: 203c 3d20 3220 2832 2e30 2069 7320 6e6f   <= 2 (2.0 is no
-00006260: 2066 696c 7465 7269 6e67 292e 2044 6566   filtering). Def
-00006270: 6175 6c74 7320 746f 204e 6f6e 652e 0d0a  aults to None...
-00006280: 2020 2020 2020 2020 3a74 7970 6520 6c6f          :type lo
-00006290: 6361 6c5f 6465 6e73 6974 795f 7468 7265  cal_density_thre
-000062a0: 7368 6f6c 643a 2066 6c6f 6174 2c20 6f70  shold: float, op
-000062b0: 7469 6f6e 616c 0d0a 2020 2020 2020 2020  tional..        
-000062c0: 3a70 6172 616d 206c 6f63 616c 5f6e 6569  :param local_nei
-000062d0: 6768 626f 7268 6f6f 645f 7369 7a65 3a20  ghborhood_size: 
-000062e0: 4672 6163 7469 6f6e 206f 6620 7468 6520  Fraction of the 
-000062f0: 6e75 6d62 6572 206f 6620 7265 706c 6963  number of replic
-00006300: 6174 6573 2074 6f20 7573 6520 6173 206e  ates to use as n
-00006310: 6561 7265 7374 206e 6569 6768 626f 7273  earest neighbors
-00006320: 2066 6f72 206c 6f63 616c 2064 656e 7369   for local densi
-00006330: 7479 2066 696c 7465 7269 6e67 2e20 4465  ty filtering. De
-00006340: 6661 756c 7473 2074 6f20 4e6f 6e65 0d0a  faults to None..
-00006350: 2020 2020 2020 2020 3a74 7970 6520 6c6f          :type lo
-00006360: 6361 6c5f 6e65 6967 6862 6f72 686f 6f64  cal_neighborhood
-00006370: 5f73 697a 653a 2066 6c6f 6174 2c20 6f70  _size: float, op
-00006380: 7469 6f6e 616c 0d0a 2020 2020 2020 2020  tional..        
-00006390: 2222 220d 0a20 2020 2020 2020 2073 656c  """..        sel
-000063a0: 662e 6164 6174 612e 756e 735b 2263 6e6d  f.adata.uns["cnm
-000063b0: 665f 6e61 6d65 225d 203d 2063 6e6d 665f  f_name"] = cnmf_
-000063c0: 6e61 6d65 0d0a 0d0a 2020 2020 2020 2020  name....        
-000063d0: 2320 696e 6665 7220 6672 6f6d 2066 696c  # infer from fil
-000063e0: 656e 616d 6573 2077 6869 6368 206c 6f63  enames which loc
-000063f0: 616c 2064 656e 7369 7479 2074 6872 6573  al density thres
-00006400: 686f 6c64 2077 6173 2075 7365 640d 0a20  hold was used.. 
-00006410: 2020 2020 2020 2073 656e 7365 645f 6c64         sensed_ld
-00006420: 7473 203d 2073 6574 2829 0d0a 2020 2020  ts = set()..    
-00006430: 2020 2020 666f 7220 666e 2069 6e20 676c      for fn in gl
-00006440: 6f62 286f 732e 7061 7468 2e6a 6f69 6e28  ob(os.path.join(
-00006450: 636e 6d66 5f6f 7574 7075 745f 6469 722c  cnmf_output_dir,
-00006460: 2063 6e6d 665f 6e61 6d65 2c20 6622 7b63   cnmf_name, f"{c
-00006470: 6e6d 665f 6e61 6d65 7d2a 2e2a 7370 6563  nmf_name}*.*spec
-00006480: 7472 612a 2e6b 5f2a 2229 293a 0d0a 2020  tra*.k_*")):..  
-00006490: 2020 2020 2020 2020 2020 6c64 745f 7374            ldt_st
-000064a0: 7220 3d20 6f73 2e70 6174 682e 6261 7365  r = os.path.base
-000064b0: 6e61 6d65 2866 6e29 2e73 706c 6974 2822  name(fn).split("
-000064c0: 2e22 295b 2d33 5d0d 0a20 2020 2020 2020  .")[-3]..       
-000064d0: 2020 2020 2074 7279 3a0d 0a20 2020 2020       try:..     
-000064e0: 2020 2020 2020 2020 2020 206c 6474 203d             ldt =
-000064f0: 2066 6c6f 6174 286c 6474 5f73 7472 2e72   float(ldt_str.r
-00006500: 6570 6c61 6365 2822 6474 5f22 2c20 2222  eplace("dt_", ""
-00006510: 292e 7265 706c 6163 6528 225f 222c 2022  ).replace("_", "
-00006520: 2e22 2929 0d0a 2020 2020 2020 2020 2020  ."))..          
-00006530: 2020 6578 6365 7074 2056 616c 7565 4572    except ValueEr
-00006540: 726f 723a 0d0a 2020 2020 2020 2020 2020  ror:..          
-00006550: 2020 2020 2020 7061 7373 0d0a 2020 2020        pass..    
-00006560: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
-00006570: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00006580: 656e 7365 645f 6c64 7473 2e61 6464 2828  ensed_ldts.add((
-00006590: 6c64 745f 7374 722c 206c 6474 2929 0d0a  ldt_str, ldt))..
-000065a0: 2020 2020 2020 2020 6966 206c 6f63 616c          if local
-000065b0: 5f64 656e 7369 7479 5f74 6872 6573 686f  _density_thresho
-000065c0: 6c64 2069 7320 4e6f 6e65 2061 6e64 206c  ld is None and l
-000065d0: 656e 2873 656e 7365 645f 6c64 7473 2920  en(sensed_ldts) 
-000065e0: 3d3d 2031 3a0d 0a20 2020 2020 2020 2020  == 1:..         
-000065f0: 2020 206c 6474 5f73 7472 2c20 6c64 7420     ldt_str, ldt 
-00006600: 3d20 7365 6e73 6564 5f6c 6474 732e 706f  = sensed_ldts.po
-00006610: 7028 290d 0a20 2020 2020 2020 2065 6c69  p()..        eli
-00006620: 6620 6c6f 6361 6c5f 6465 6e73 6974 795f  f local_density_
-00006630: 7468 7265 7368 6f6c 6420 696e 2028 6c64  threshold in (ld
-00006640: 745b 315d 2066 6f72 206c 6474 2069 6e20  t[1] for ldt in 
-00006650: 7365 6e73 6564 5f6c 6474 7329 3a0d 0a20  sensed_ldts):.. 
-00006660: 2020 2020 2020 2020 2020 206c 6474 5f73             ldt_s
-00006670: 7472 2c20 6c64 7420 3d20 5b28 6c64 745f  tr, ldt = [(ldt_
-00006680: 7374 722c 206c 6474 2920 666f 7220 6c64  str, ldt) for ld
-00006690: 745f 7374 722c 206c 6474 2069 6e20 7365  t_str, ldt in se
-000066a0: 6e73 6564 5f6c 6474 7320 6966 206c 6474  nsed_ldts if ldt
-000066b0: 203d 3d20 6c6f 6361 6c5f 6465 6e73 6974   == local_densit
-000066c0: 795f 7468 7265 7368 6f6c 645d 2e70 6f70  y_threshold].pop
-000066d0: 2829 0d0a 2020 2020 2020 2020 656c 7365  ()..        else
-000066e0: 3a0d 0a20 2020 2020 2020 2020 2020 206c  :..            l
-000066f0: 6f67 6769 6e67 2e65 7272 6f72 2866 226c  ogging.error(f"l
-00006700: 6f63 616c 5f64 656e 7369 7479 5f74 6872  ocal_density_thr
-00006710: 6573 686f 6c64 206f 6620 7b6c 6f63 616c  eshold of {local
-00006720: 5f64 656e 7369 7479 5f74 6872 6573 686f  _density_thresho
-00006730: 6c64 7d20 646f 6573 206e 6f74 206d 6174  ld} does not mat
-00006740: 6368 2077 6861 7420 6973 2069 6e20 7468  ch what is in th
-00006750: 6520 634e 4d46 2072 6573 756c 7420 6469  e cNMF result di
-00006760: 7265 6374 6f72 793a 207b 7365 6e73 6564  rectory: {sensed
-00006770: 5f6c 6474 737d 2229 0d0a 2020 2020 2020  _ldts}")..      
-00006780: 2020 2020 2020 7379 732e 6578 6974 2831        sys.exit(1
-00006790: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-000067a0: 6164 6174 612e 756e 735b 226c 6474 225d  adata.uns["ldt"]
-000067b0: 203d 206c 6474 0d0a 2020 2020 2020 2020   = ldt..        
-000067c0: 7365 6c66 2e61 6461 7461 2e75 6e73 5b22  self.adata.uns["
-000067d0: 6c6e 7322 5d20 3d20 6c6f 6361 6c5f 6e65  lns"] = local_ne
-000067e0: 6967 6862 6f72 686f 6f64 5f73 697a 650d  ighborhood_size.
-000067f0: 0a20 2020 2020 2020 2020 2020 200d 0a20  .            .. 
-00006800: 2020 2020 2020 2023 2049 6d70 6f72 7420         # Import 
-00006810: 4745 5073 0d0a 2020 2020 2020 2020 7265  GEPs..        re
-00006820: 7375 6c74 5f74 7970 6573 203d 207b 0d0a  sult_types = {..
-00006830: 2020 2020 2020 2020 2020 2020 2267 656e              "gen
-00006840: 655f 7370 6563 7472 615f 7363 6f72 6522  e_spectra_score"
-00006850: 3a20 2263 6e6d 665f 6765 705f 7363 6f72  : "cnmf_gep_scor
-00006860: 6522 2c0d 0a20 2020 2020 2020 2020 2020  e",..           
-00006870: 2022 6765 6e65 5f73 7065 6374 7261 5f74   "gene_spectra_t
-00006880: 706d 223a 2022 636e 6d66 5f67 6570 5f74  pm": "cnmf_gep_t
-00006890: 706d 222c 0d0a 2020 2020 2020 2020 2020  pm",..          
-000068a0: 2020 2273 7065 6374 7261 223a 2022 636e    "spectra": "cn
-000068b0: 6d66 5f67 6570 5f72 6177 220d 0a20 2020  mf_gep_raw"..   
-000068c0: 2020 2020 2020 2020 207d 0d0a 2020 2020           }..    
-000068d0: 2020 2020 666f 7220 6d61 7463 6873 7472      for matchstr
-000068e0: 2c20 7265 7375 6c74 5f74 7970 6520 696e  , result_type in
-000068f0: 2072 6573 756c 745f 7479 7065 732e 6974   result_types.it
-00006900: 656d 7328 293a 0d0a 2020 2020 2020 2020  ems():..        
-00006910: 2020 2020 6c6f 6767 696e 672e 696e 666f      logging.info
-00006920: 2866 2249 6d70 6f72 7469 6e67 2047 4550  (f"Importing GEP
-00006930: 733a 207b 6d61 7463 6873 7472 7d22 2920  s: {matchstr}") 
-00006940: 200d 0a20 2020 2020 2020 2020 2020 206d   ..            m
-00006950: 6574 615f 7720 3d20 5b5d 0d0a 2020 2020  eta_w = []..    
-00006960: 2020 2020 2020 2020 666f 7220 666e 2069          for fn i
-00006970: 6e20 676c 6f62 286f 732e 7061 7468 2e6a  n glob(os.path.j
-00006980: 6f69 6e28 636e 6d66 5f6f 7574 7075 745f  oin(cnmf_output_
-00006990: 6469 722c 2063 6e6d 665f 6e61 6d65 2c20  dir, cnmf_name, 
-000069a0: 6622 7b63 6e6d 665f 6e61 6d65 7d2a 2e7b  f"{cnmf_name}*.{
-000069b0: 6d61 7463 6873 7472 7d2e 6b5f 2a2e 7b6c  matchstr}.k_*.{l
-000069c0: 6474 5f73 7472 7d2e 2a74 7874 2229 293a  dt_str}.*txt")):
-000069d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000069e0: 2020 6b20 3d20 696e 7428 6f73 2e70 6174    k = int(os.pat
-000069f0: 682e 6261 7365 6e61 6d65 2866 6e29 2e72  h.basename(fn).r
-00006a00: 656d 6f76 6570 7265 6669 7828 6622 7b63  emoveprefix(f"{c
-00006a10: 6e6d 665f 6e61 6d65 7d2e 7b6d 6174 6368  nmf_name}.{match
-00006a20: 7374 727d 2e22 292e 7370 6c69 7428 222e  str}.").split(".
-00006a30: 2229 5b30 5d2e 7265 706c 6163 6528 226b  ")[0].replace("k
-00006a40: 5f22 2c20 2222 2929 0d0a 2020 2020 2020  _", ""))..      
-00006a50: 2020 2020 2020 2020 2020 7720 3d20 7064            w = pd
-00006a60: 2e72 6561 645f 7461 626c 6528 666e 2c20  .read_table(fn, 
-00006a70: 696e 6465 785f 636f 6c3d 3029 0d0a 2020  index_col=0)..  
-00006a80: 2020 2020 2020 2020 2020 2020 2020 772e                w.
-00006a90: 696e 6465 7820 3d20 7374 7228 6b29 202b  index = str(k) +
-00006aa0: 2022 2e22 202b 2077 2e69 6e64 6578 2e61   "." + w.index.a
-00006ab0: 7374 7970 6528 7374 7229 0d0a 2020 2020  stype(str)..    
-00006ac0: 2020 2020 2020 2020 2020 2020 6d65 7461              meta
-00006ad0: 5f77 2e61 7070 656e 6428 7729 0d0a 2020  _w.append(w)..  
-00006ae0: 2020 2020 2020 2020 2020 6d65 7461 5f77            meta_w
-00006af0: 203d 2070 642e 636f 6e63 6174 286d 6574   = pd.concat(met
-00006b00: 615f 772c 2061 7869 733d 3029 2e54 2e72  a_w, axis=0).T.r
-00006b10: 6569 6e64 6578 2873 656c 662e 6164 6174  eindex(self.adat
-00006b20: 612e 7661 722e 696e 6465 7829 2e72 656e  a.var.index).ren
-00006b30: 616d 655f 6178 6973 285b 226b 2e67 6570  ame_axis(["k.gep
-00006b40: 225d 2c20 6178 6973 3d31 290d 0a20 2020  "], axis=1)..   
-00006b50: 2020 2020 2020 2020 2073 656c 662e 6164           self.ad
-00006b60: 6174 612e 7661 726d 5b72 6573 756c 745f  ata.varm[result_
-00006b70: 7479 7065 5d20 3d20 6d65 7461 5f77 0d0a  type] = meta_w..
-00006b80: 0d0a 2020 2020 2020 2020 2320 496d 706f  ..        # Impo
-00006b90: 7274 2055 7361 6765 730d 0a20 2020 2020  rt Usages..     
-00006ba0: 2020 206c 6f67 6769 6e67 2e69 6e66 6f28     logging.info(
-00006bb0: 6622 496d 706f 7274 696e 6720 5573 6167  f"Importing Usag
-00006bc0: 6573 2229 2020 0d0a 2020 2020 2020 2020  es")  ..        
-00006bd0: 7573 6167 6520 3d20 5b5d 0d0a 2020 2020  usage = []..    
-00006be0: 2020 2020 666f 7220 666e 2069 6e20 676c      for fn in gl
-00006bf0: 6f62 286f 732e 7061 7468 2e6a 6f69 6e28  ob(os.path.join(
-00006c00: 636e 6d66 5f6f 7574 7075 745f 6469 722c  cnmf_output_dir,
-00006c10: 2063 6e6d 665f 6e61 6d65 2c20 6622 7b63   cnmf_name, f"{c
-00006c20: 6e6d 665f 6e61 6d65 7d2a 2e75 7361 6765  nmf_name}*.usage
-00006c30: 732e 6b5f 2a2e 7b6c 6474 5f73 7472 7d2e  s.k_*.{ldt_str}.
-00006c40: 2a74 7874 2229 293a 0d0a 2020 2020 2020  *txt")):..      
-00006c50: 2020 2020 2020 6b20 3d20 696e 7428 6f73        k = int(os
-00006c60: 2e70 6174 682e 6261 7365 6e61 6d65 2866  .path.basename(f
-00006c70: 6e29 2e72 656d 6f76 6570 7265 6669 7828  n).removeprefix(
-00006c80: 6622 7b63 6e6d 665f 6e61 6d65 7d2e 7573  f"{cnmf_name}.us
-00006c90: 6167 6573 2e22 292e 7370 6c69 7428 222e  ages.").split(".
-00006ca0: 2229 5b30 5d2e 7265 706c 6163 6528 226b  ")[0].replace("k
-00006cb0: 5f22 2c20 2222 2929 0d0a 2020 2020 2020  _", ""))..      
-00006cc0: 2020 2020 2020 6820 3d20 7064 2e72 6561        h = pd.rea
-00006cd0: 645f 7461 626c 6528 666e 2c20 696e 6465  d_table(fn, inde
-00006ce0: 785f 636f 6c3d 3029 0d0a 2020 2020 2020  x_col=0)..      
-00006cf0: 2020 2020 2020 682e 636f 6c75 6d6e 7320        h.columns 
-00006d00: 3d20 7374 7228 6b29 202b 2022 2e22 202b  = str(k) + "." +
-00006d10: 2068 2e63 6f6c 756d 6e73 2e61 7374 7970   h.columns.astyp
-00006d20: 6528 7374 7229 0d0a 2020 2020 2020 2020  e(str)..        
-00006d30: 2020 2020 7573 6167 652e 6170 7065 6e64      usage.append
-00006d40: 2868 290d 0a20 2020 2020 2020 2073 656c  (h)..        sel
-00006d50: 662e 6164 6174 612e 6f62 736d 5b22 636e  f.adata.obsm["cn
-00006d60: 6d66 5f75 7361 6765 225d 203d 2070 642e  mf_usage"] = pd.
-00006d70: 636f 6e63 6174 2875 7361 6765 2c20 6178  concat(usage, ax
-00006d80: 6973 3d31 292e 736f 7274 5f69 6e64 6578  is=1).sort_index
-00006d90: 2861 7869 733d 3129 2e72 656e 616d 655f  (axis=1).rename_
-00006da0: 6178 6973 285b 226b 2e67 6570 225d 2c20  axis(["k.gep"], 
-00006db0: 6178 6973 3d31 290d 0a20 2020 2020 2020  axis=1)..       
-00006dc0: 200d 0a20 2020 2020 2020 2023 2049 6d70   ..        # Imp
-00006dd0: 6f72 7420 6765 6e65 206c 6973 7420 7573  ort gene list us
-00006de0: 6564 2066 6f72 2066 6163 746f 7269 7a61  ed for factoriza
-00006df0: 7469 6f6e 0d0a 2020 2020 2020 2020 7769  tion..        wi
-00006e00: 7468 206f 7065 6e28 6f73 2e70 6174 682e  th open(os.path.
-00006e10: 6a6f 696e 2863 6e6d 665f 6f75 7470 7574  join(cnmf_output
-00006e20: 5f64 6972 2c20 636e 6d66 5f6e 616d 652c  _dir, cnmf_name,
-00006e30: 2066 227b 636e 6d66 5f6e 616d 657d 2e6f   f"{cnmf_name}.o
-00006e40: 7665 7264 6973 7065 7273 6564 5f67 656e  verdispersed_gen
-00006e50: 6573 2e74 7874 2229 2920 6173 2066 3a0d  es.txt")) as f:.
-00006e60: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00006e70: 662e 6164 6174 612e 756e 735b 2267 656e  f.adata.uns["gen
-00006e80: 655f 6c69 7374 225d 203d 205b 6c69 6e65  e_list"] = [line
-00006e90: 2e73 7472 6970 2829 2066 6f72 206c 696e  .strip() for lin
-00006ea0: 6520 696e 2066 2e72 6561 646c 696e 6573  e in f.readlines
-00006eb0: 2829 5d0d 0a0d 0a20 2020 2020 2020 2023  ()]....        #
-00006ec0: 2049 6d70 6f72 7420 4b2d 7365 6c65 6374   Import K-select
-00006ed0: 696f 6e20 7374 6174 730d 0a20 2020 2020  ion stats..     
-00006ee0: 2020 206b 7661 6c73 203d 2070 642e 4461     kvals = pd.Da
-00006ef0: 7461 4672 616d 6528 2a2a 6e70 2e6c 6f61  taFrame(**np.loa
-00006f00: 6428 6f73 2e70 6174 682e 6a6f 696e 2863  d(os.path.join(c
-00006f10: 6e6d 665f 6f75 7470 7574 5f64 6972 2c20  nmf_output_dir, 
-00006f20: 636e 6d66 5f6e 616d 652c 2066 227b 636e  cnmf_name, f"{cn
-00006f30: 6d66 5f6e 616d 657d 2e6b 5f73 656c 6563  mf_name}.k_selec
-00006f40: 7469 6f6e 5f73 7461 7473 2e64 662e 6e70  tion_stats.df.np
-00006f50: 7a22 292c 2061 6c6c 6f77 5f70 6963 6b6c  z"), allow_pickl
-00006f60: 653d 5472 7565 2929 2e73 6574 5f69 6e64  e=True)).set_ind
-00006f70: 6578 2822 6b22 295b 5b22 7374 6162 696c  ex("k")[["stabil
-00006f80: 6974 7922 2c20 2270 7265 6469 6374 696f  ity", "predictio
-00006f90: 6e5f 6572 726f 7222 5d5d 0d0a 2020 2020  n_error"]]..    
-00006fa0: 2020 2020 6b76 616c 732e 696e 6465 7820      kvals.index 
-00006fb0: 3d20 6b76 616c 732e 696e 6465 782e 6173  = kvals.index.as
-00006fc0: 7479 7065 2869 6e74 290d 0a20 2020 2020  type(int)..     
-00006fd0: 2020 2073 656c 662e 6164 6174 612e 756e     self.adata.un
-00006fe0: 735b 226b 7661 6c73 225d 203d 206b 7661  s["kvals"] = kva
-00006ff0: 6c73 0d0a 2020 2020 2020 2020 7365 6c66  ls..        self
-00007000: 2e61 7070 656e 645f 746f 5f68 6973 746f  .append_to_histo
-00007010: 7279 2822 634e 4d46 2072 6573 756c 7473  ry("cNMF results
-00007020: 2061 6464 6564 2066 726f 6d20 6f75 7470   added from outp
-00007030: 7574 2064 6972 6563 746f 7279 207b 636e  ut directory {cn
-00007040: 6d66 5f6f 7574 7075 745f 6469 727d 2f7b  mf_output_dir}/{
-00007050: 636e 6d66 5f6e 616d 657d 2229 0d0a 0d0a  cnmf_name}")....
-00007060: 2020 2020 6465 6620 7265 6d6f 7665 5f63      def remove_c
-00007070: 6e6d 665f 7265 7375 6c74 7328 7365 6c66  nmf_results(self
-00007080: 293a 0d0a 2020 2020 2020 2020 666f 7220  ):..        for 
-00007090: 7265 7375 6c74 5f74 7970 6520 696e 2028  result_type in (
-000070a0: 2263 6e6d 665f 6765 705f 7363 6f72 6522  "cnmf_gep_score"
-000070b0: 2c20 2263 6e6d 665f 6765 705f 7470 6d22  , "cnmf_gep_tpm"
-000070c0: 2c20 2263 6e6d 665f 6765 705f 7261 7722  , "cnmf_gep_raw"
-000070d0: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-000070e0: 7365 6c66 2e61 6461 7461 2e76 6172 6d2e  self.adata.varm.
-000070f0: 706f 7028 7265 7375 6c74 5f74 7970 6529  pop(result_type)
-00007100: 0d0a 2020 2020 2020 2020 7365 6c66 2e61  ..        self.a
-00007110: 6461 7461 2e6f 6273 6d2e 706f 7028 2263  data.obsm.pop("c
-00007120: 6e6d 665f 7573 6167 6522 290d 0a20 2020  nmf_usage")..   
-00007130: 2020 2020 2073 656c 662e 6164 6174 612e       self.adata.
-00007140: 756e 732e 706f 7028 2267 656e 655f 6c69  uns.pop("gene_li
-00007150: 7374 2229 0d0a 2020 2020 2020 2020 7365  st")..        se
-00007160: 6c66 2e61 6461 7461 2e75 6e73 2e70 6f70  lf.adata.uns.pop
-00007170: 2822 6b76 616c 7322 290d 0a20 2020 2020  ("kvals")..     
-00007180: 2020 2073 656c 662e 6170 7065 6e64 5f74     self.append_t
-00007190: 6f5f 6869 7374 6f72 7928 2263 4e4d 4620  o_history("cNMF 
-000071a0: 7265 7375 6c74 7320 7265 6d6f 7665 642e  results removed.
-000071b0: 2229 0d0a 0d0a 0d0a 2020 2020 6465 6620  ")......    def 
-000071c0: 6765 745f 7573 6167 6573 2873 656c 662c  get_usages(self,
-000071d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000071e0: 2020 2020 206b 3a20 556e 696f 6e5b 696e       k: Union[in
-000071f0: 742c 2049 7465 7261 626c 655d 203d 204e  t, Iterable] = N
-00007200: 6f6e 652c 0d0a 2020 2020 2020 2020 2020  one,..          
-00007210: 2020 2020 2020 2020 2064 6973 6372 6574           discret
-00007220: 697a 653a 2062 6f6f 6c20 3d20 4661 6c73  ize: bool = Fals
-00007230: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
-00007240: 2020 2020 2020 206e 6f72 6d61 6c69 7a65         normalize
-00007250: 3a20 626f 6f6c 203d 2046 616c 7365 0d0a  : bool = False..
-00007260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007270: 2020 2029 202d 3e20 7064 2e44 6174 6146     ) -> pd.DataF
-00007280: 7261 6d65 3a0d 0a20 2020 2020 2020 2022  rame:..        "
-00007290: 2222 0d0a 2020 2020 2020 2020 4361 6c63  ""..        Calc
-000072a0: 756c 6174 6520 7573 6167 6520 6f66 2065  ulate usage of e
-000072b0: 6163 6820 4745 5020 696e 2065 6163 6820  ach GEP in each 
-000072c0: 7361 6d70 6c65 2f6f 6273 6572 7661 7469  sample/observati
-000072d0: 6f6e 2e0d 0a0d 0a20 2020 2020 2020 203a  on.....        :
-000072e0: 7061 7261 6d20 6b3a 2049 6620 616e 2069  param k: If an i
-000072f0: 6e74 6567 6572 206f 7220 6c69 7374 206f  nteger or list o
-00007300: 6620 696e 7465 6765 7273 2c20 7265 7475  f integers, retu
-00007310: 726e 7320 7573 6167 6573 206f 6e6c 7920  rns usages only 
-00007320: 666f 7220 7370 6563 6966 6965 6420 7261  for specified ra
-00007330: 6e6b 732e 204f 7468 6572 7769 7365 2c20  nks. Otherwise, 
-00007340: 7265 7475 726e 7320 7573 6167 6520 6f66  returns usage of
-00007350: 2061 6c6c 2047 4550 7320 6163 726f 7373   all GEPs across
-00007360: 2072 616e 6b73 2e20 4465 6661 756c 7473   ranks. Defaults
-00007370: 2074 6f20 4e6f 6e65 0d0a 2020 2020 2020   to None..      
-00007380: 2020 3a74 7970 6520 6b3a 2069 6e74 2c20    :type k: int, 
-00007390: 6f70 7469 6f6e 616c 0d0a 2020 2020 2020  optional..      
-000073a0: 2020 3a70 6172 616d 2064 6973 6372 6574    :param discret
-000073b0: 697a 653a 2044 6973 6372 6574 697a 6573  ize: Discretizes
-000073c0: 2074 6865 2075 7361 6765 206d 6174 7269   the usage matri
-000073d0: 7820 7375 6368 2074 6861 7420 666f 7220  x such that for 
-000073e0: 6561 6368 2076 616c 7565 206f 6620 6b2c  each value of k,
-000073f0: 2065 6163 6820 7361 6d70 6c65 2068 6173   each sample has
-00007400: 2075 7361 6765 206f 6620 6f6e 6c79 2031   usage of only 1
-00007410: 2047 4550 2028 7468 6520 6f6e 6520 7769   GEP (the one wi
-00007420: 7468 2074 6865 206d 6178 696d 756d 2075  th the maximum u
-00007430: 7361 6765 292e 2044 6566 6175 6c74 7320  sage). Defaults 
-00007440: 746f 2046 616c 7365 0d0a 2020 2020 2020  to False..      
-00007450: 2020 3a74 7970 6520 6469 7363 7265 7469    :type discreti
-00007460: 7a65 3a20 626f 6f6c 2c20 6f70 7469 6f6e  ze: bool, option
-00007470: 616c 0d0a 2020 2020 2020 2020 3a70 6172  al..        :par
-00007480: 616d 206e 6f72 6d61 6c69 7a65 3a20 4e6f  am normalize: No
-00007490: 726d 616c 697a 6520 7468 6520 4745 5020  rmalize the GEP 
-000074a0: 7573 6167 6520 6d61 7472 6978 2073 7563  usage matrix suc
-000074b0: 6820 7468 6174 2066 6f72 2065 6163 6820  h that for each 
-000074c0: 7661 6c75 6520 6f66 206b 2c20 7573 6167  value of k, usag
-000074d0: 6520 6f66 2061 6c6c 2047 4550 7320 7375  e of all GEPs su
-000074e0: 6d73 2074 6f20 312e 2044 6566 6175 6c74  ms to 1. Default
-000074f0: 7320 746f 2046 616c 7365 0d0a 2020 2020  s to False..    
-00007500: 2020 2020 3a74 7970 6520 6e6f 726d 616c      :type normal
-00007510: 697a 653a 2062 6f6f 6c2c 206f 7074 696f  ize: bool, optio
-00007520: 6e61 6c0d 0a20 2020 2020 2020 203a 7265  nal..        :re
-00007530: 7475 726e 3a20 6f62 7365 7276 6174 696f  turn: observatio
-00007540: 6e20 c397 2047 4550 206d 6174 7269 780d  n .. GEP matrix.
-00007550: 0a20 2020 2020 2020 203a 7274 7970 653a  .        :rtype:
-00007560: 2070 642e 4461 7461 4672 616d 650d 0a20   pd.DataFrame.. 
-00007570: 2020 2020 2020 2022 2222 0d0a 2020 2020         """..    
-00007580: 2020 2020 6466 203d 2073 656c 662e 6164      df = self.ad
-00007590: 6174 612e 6f62 736d 5b22 636e 6d66 5f75  ata.obsm["cnmf_u
-000075a0: 7361 6765 225d 2e63 6f70 7928 290d 0a20  sage"].copy().. 
-000075b0: 2020 2020 2020 2064 662e 636f 6c75 6d6e         df.column
-000075c0: 7320 3d20 7064 2e4d 756c 7469 496e 6465  s = pd.MultiInde
-000075d0: 782e 6672 6f6d 5f74 7570 6c65 7328 6466  x.from_tuples(df
-000075e0: 2e63 6f6c 756d 6e73 2e73 7472 2e73 706c  .columns.str.spl
-000075f0: 6974 2822 2e22 292e 746f 5f6c 6973 7428  it(".").to_list(
-00007600: 2929 0d0a 2020 2020 2020 2020 6466 2e63  ))..        df.c
-00007610: 6f6c 756d 6e73 203d 2064 662e 636f 6c75  olumns = df.colu
-00007620: 6d6e 732e 7365 745f 6c65 7665 6c73 285b  mns.set_levels([
-00007630: 6c2e 6173 7479 7065 2822 696e 7422 2920  l.astype("int") 
-00007640: 666f 7220 6c20 696e 2064 662e 636f 6c75  for l in df.colu
-00007650: 6d6e 732e 6c65 7665 6c73 5d29 0d0a 2020  mns.levels])..  
-00007660: 2020 2020 2020 6966 206e 6f72 6d61 6c69        if normali
-00007670: 7a65 3a0d 0a20 2020 2020 2020 2020 2020  ze:..           
-00007680: 206e 6f72 6d61 6c69 7a65 6420 3d20 5b5d   normalized = []
-00007690: 0d0a 2020 2020 2020 2020 2020 2020 666f  ..            fo
-000076a0: 7220 5f2c 2073 7562 6466 2069 6e20 6466  r _, subdf in df
-000076b0: 2e67 726f 7570 6279 2861 7869 733d 312c  .groupby(axis=1,
-000076c0: 206c 6576 656c 3d30 293a 0d0a 2020 2020   level=0):..    
-000076d0: 2020 2020 2020 2020 2020 2020 6e6f 726d              norm
-000076e0: 616c 697a 6564 2e61 7070 656e 6428 7375  alized.append(su
-000076f0: 6264 662e 6469 7628 7375 6264 662e 7375  bdf.div(subdf.su
-00007700: 6d28 6178 6973 3d31 292c 2061 7869 733d  m(axis=1), axis=
-00007710: 3029 290d 0a20 2020 2020 2020 2020 2020  0))..           
-00007720: 2064 6620 3d20 7064 2e63 6f6e 6361 7428   df = pd.concat(
-00007730: 6e6f 726d 616c 697a 6564 2c20 6178 6973  normalized, axis
-00007740: 3d31 290d 0a20 2020 2020 2020 2069 6620  =1)..        if 
-00007750: 6469 7363 7265 7469 7a65 3a0d 0a20 2020  discretize:..   
-00007760: 2020 2020 2020 2020 2064 6973 6372 6574           discret
-00007770: 697a 6564 203d 205b 5d0d 0a20 2020 2020  ized = []..     
-00007780: 2020 2020 2020 2066 6f72 205f 2c20 7375         for _, su
-00007790: 6264 6620 696e 2064 662e 6772 6f75 7062  bdf in df.groupb
-000077a0: 7928 6178 6973 3d31 2c20 6c65 7665 6c3d  y(axis=1, level=
-000077b0: 3029 3a0d 0a20 2020 2020 2020 2020 2020  0):..           
-000077c0: 2020 2020 2064 6973 6372 6574 697a 6564       discretized
-000077d0: 2e61 7070 656e 6428 7375 6264 662e 6571  .append(subdf.eq
-000077e0: 2873 7562 6466 2e6d 6178 2861 7869 733d  (subdf.max(axis=
-000077f0: 3129 2c20 6178 6973 3d30 292e 6173 7479  1), axis=0).asty
-00007800: 7065 2869 6e74 2929 0d0a 2020 2020 2020  pe(int))..      
-00007810: 2020 2020 2020 6466 203d 2070 642e 636f        df = pd.co
-00007820: 6e63 6174 2864 6973 6372 6574 697a 6564  ncat(discretized
-00007830: 2c20 6178 6973 3d31 2920 2020 2020 2020  , axis=1)       
-00007840: 200d 0a20 2020 2020 2020 2069 6620 6b20   ..        if k 
-00007850: 6973 206e 6f74 204e 6f6e 653a 0d0a 2020  is not None:..  
-00007860: 2020 2020 2020 2020 2020 6466 203d 2064            df = d
-00007870: 662e 6c6f 635b 3a2c 206b 5d0d 0a20 2020  f.loc[:, k]..   
-00007880: 2020 2020 2064 6620 3d20 6466 2e73 6f72       df = df.sor
-00007890: 745f 696e 6465 7828 6178 6973 3d30 292e  t_index(axis=0).
-000078a0: 736f 7274 5f69 6e64 6578 2861 7869 733d  sort_index(axis=
-000078b0: 3129 2020 200d 0a20 2020 2020 2020 2072  1)   ..        r
-000078c0: 6574 7572 6e20 6466 0d0a 2020 2020 0d0a  eturn df..    ..
-000078d0: 2020 2020 6465 6620 6765 745f 6765 7073      def get_geps
-000078e0: 2873 656c 662c 0d0a 2020 2020 2020 2020  (self,..        
-000078f0: 2020 2020 2020 2020 206b 3a20 556e 696f           k: Unio
-00007900: 6e5b 696e 742c 2049 7465 7261 626c 655d  n[int, Iterable]
-00007910: 203d 204e 6f6e 652c 0d0a 2020 2020 2020   = None,..      
-00007920: 2020 2020 2020 2020 2020 2074 7970 653d             type=
-00007930: 2263 6e6d 665f 6765 705f 7363 6f72 6522  "cnmf_gep_score"
-00007940: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00007950: 2020 2029 202d 3e20 7064 2e44 6174 6146     ) -> pd.DataF
-00007960: 7261 6d65 3a0d 0a20 2020 2020 2020 2022  rame:..        "
-00007970: 2222 0d0a 2020 2020 2020 2020 4765 7420  ""..        Get 
-00007980: 4745 5073 2e0d 0a0d 0a20 2020 2020 2020  GEPs.....       
-00007990: 203a 7061 7261 6d20 6b3a 2049 6620 616e   :param k: If an
-000079a0: 2069 6e74 6567 6572 206f 7220 6c69 7374   integer or list
-000079b0: 206f 6620 696e 7465 6765 7273 2c20 7265   of integers, re
-000079c0: 7475 726e 7320 4745 5073 206f 6e6c 7920  turns GEPs only 
-000079d0: 666f 7220 7370 6563 6966 6965 6420 7261  for specified ra
-000079e0: 6e6b 732e 204f 7468 6572 7769 7365 2c20  nks. Otherwise, 
-000079f0: 7265 7475 726e 7320 4745 5073 2066 726f  returns GEPs fro
-00007a00: 6d20 616c 6c20 7261 6e6b 732e 2044 6566  m all ranks. Def
-00007a10: 6175 6c74 7320 746f 204e 6f6e 650d 0a20  aults to None.. 
-00007a20: 2020 2020 2020 203a 7479 7065 206b 3a20         :type k: 
-00007a30: 556e 696f 6e5b 696e 742c 2049 7465 7261  Union[int, Itera
-00007a40: 626c 655d 2c20 6f70 7469 6f6e 616c 0d0a  ble], optional..
-00007a50: 2020 2020 2020 2020 3a70 6172 616d 2074          :param t
-00007a60: 7970 653a 2022 636e 6d66 5f67 6570 5f73  ype: "cnmf_gep_s
-00007a70: 636f 7265 2220 6f72 2022 636e 6d66 5f67  core" or "cnmf_g
-00007a80: 6570 5f74 706d 222c 2064 6566 6175 6c74  ep_tpm", default
-00007a90: 7320 746f 2022 636e 6d66 5f67 6570 5f73  s to "cnmf_gep_s
-00007aa0: 636f 7265 220d 0a20 2020 2020 2020 203a  core"..        :
-00007ab0: 7479 7065 2074 7970 653a 2073 7472 2c20  type type: str, 
-00007ac0: 6f70 7469 6f6e 616c 0d0a 2020 2020 2020  optional..      
-00007ad0: 2020 3a72 6574 7572 6e3a 2066 6561 7475    :return: featu
-00007ae0: 7265 7320 c397 2047 4550 206d 6174 7269  res .. GEP matri
-00007af0: 780d 0a20 2020 2020 2020 203a 7274 7970  x..        :rtyp
-00007b00: 653a 2070 642e 4461 7461 4672 616d 650d  e: pd.DataFrame.
-00007b10: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
-00007b20: 2020 2020 2020 6466 203d 2073 656c 662e        df = self.
-00007b30: 6164 6174 612e 7661 726d 5b74 7970 655d  adata.varm[type]
-00007b40: 2e63 6f70 7928 290d 0a20 2020 2020 2020  .copy()..       
-00007b50: 2064 662e 636f 6c75 6d6e 7320 3d20 7064   df.columns = pd
-00007b60: 2e4d 756c 7469 496e 6465 782e 6672 6f6d  .MultiIndex.from
-00007b70: 5f74 7570 6c65 7328 6466 2e63 6f6c 756d  _tuples(df.colum
-00007b80: 6e73 2e73 7472 2e73 706c 6974 2822 2e22  ns.str.split("."
-00007b90: 292e 746f 5f6c 6973 7428 2929 0d0a 2020  ).to_list())..  
-00007ba0: 2020 2020 2020 6466 2e63 6f6c 756d 6e73        df.columns
-00007bb0: 203d 2064 662e 636f 6c75 6d6e 732e 7365   = df.columns.se
-00007bc0: 745f 6c65 7665 6c73 285b 6c2e 6173 7479  t_levels([l.asty
-00007bd0: 7065 2822 696e 7422 2920 666f 7220 6c20  pe("int") for l 
-00007be0: 696e 2064 662e 636f 6c75 6d6e 732e 6c65  in df.columns.le
-00007bf0: 7665 6c73 5d29 0d0a 2020 2020 2020 2020  vels])..        
-00007c00: 6966 2069 7369 6e73 7461 6e63 6528 6b2c  if isinstance(k,
-00007c10: 2028 696e 742c 2049 7465 7261 626c 6529   (int, Iterable)
-00007c20: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-00007c30: 6466 203d 2064 662e 6c6f 635b 3a2c 206b  df = df.loc[:, k
-00007c40: 5d0d 0a20 2020 2020 2020 2064 6620 3d20  ]..        df = 
-00007c50: 6466 2e73 6f72 745f 696e 6465 7828 6178  df.sort_index(ax
-00007c60: 6973 3d31 290d 0a20 2020 2020 2020 2072  is=1)..        r
-00007c70: 6574 7572 6e20 6466 0d0a 2020 2020 0d0a  eturn df..    ..
-00007c80: 2020 2020 6465 6620 6765 745f 6d65 7461      def get_meta
-00007c90: 6461 7461 5f64 6628 7365 6c66 2c0d 0a20  data_df(self,.. 
-00007ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007cb0: 2020 2020 2020 2069 6e63 6c75 6465 5f63         include_c
-00007cc0: 6174 6567 6f72 6963 616c 3a20 626f 6f6c  ategorical: bool
-00007cd0: 203d 2054 7275 652c 0d0a 2020 2020 2020   = True,..      
-00007ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007cf0: 2020 696e 636c 7564 655f 6e75 6d65 7269    include_numeri
-00007d00: 6361 6c3a 2062 6f6f 6c20 3d20 5472 7565  cal: bool = True
-00007d10: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00007d20: 2020 2020 2020 2020 2020 2920 2d3e 2070            ) -> p
-00007d30: 642e 4461 7461 4672 616d 653a 0d0a 2020  d.DataFrame:..  
-00007d40: 2020 2020 2020 2222 2247 6574 2073 616d        """Get sam
-00007d50: 706c 652f 6f62 7365 7276 6174 696f 6e20  ple/observation 
-00007d60: 6d65 7461 6461 7461 2e0d 0a0d 0a20 2020  metadata.....   
-00007d70: 2020 2020 203a 7061 7261 6d20 696e 636c       :param incl
-00007d80: 7564 655f 6361 7465 676f 7269 6361 6c3a  ude_categorical:
-00007d90: 2049 6e63 6c75 6465 2063 6174 6567 6f72   Include categor
-00007da0: 6963 616c 206d 6574 6164 6174 6120 6c61  ical metadata la
-00007db0: 7965 7273 2c20 6465 6661 756c 7473 2074  yers, defaults t
-00007dc0: 6f20 5472 7565 0d0a 2020 2020 2020 2020  o True..        
-00007dd0: 3a74 7970 6520 696e 636c 7564 655f 6361  :type include_ca
-00007de0: 7465 676f 7269 6361 6c3a 2062 6f6f 6c2c  tegorical: bool,
-00007df0: 206f 7074 696f 6e61 6c0d 0a20 2020 2020   optional..     
-00007e00: 2020 203a 7061 7261 6d20 696e 636c 7564     :param includ
-00007e10: 655f 6e75 6d65 7269 6361 6c3a 2049 6e63  e_numerical: Inc
-00007e20: 6c75 6465 206e 756d 6572 6963 616c 206d  lude numerical m
-00007e30: 6574 6164 6174 6120 6c61 7965 7273 2c20  etadata layers, 
-00007e40: 6465 6661 756c 7473 2074 6f20 5472 7565  defaults to True
-00007e50: 0d0a 2020 2020 2020 2020 3a74 7970 6520  ..        :type 
-00007e60: 696e 636c 7564 655f 6e75 6d65 7269 6361  include_numerica
-00007e70: 6c3a 2062 6f6f 6c2c 206f 7074 696f 6e61  l: bool, optiona
-00007e80: 6c0d 0a20 2020 2020 2020 203a 7261 6973  l..        :rais
-00007e90: 6573 2056 616c 7565 4572 726f 723a 2045  es ValueError: E
-00007ea0: 7272 6f72 2069 6620 6d65 7461 6461 7461  rror if metadata
-00007eb0: 2074 7970 6573 2061 7265 206e 6f74 2072   types are not r
-00007ec0: 6563 6f67 6e69 7a65 640d 0a20 2020 2020  ecognized..     
-00007ed0: 2020 203a 7265 7475 726e 3a20 6f62 7365     :return: obse
-00007ee0: 7276 6174 696f 6e73 20c3 9720 6d65 7461  rvations .. meta
-00007ef0: 6461 7461 206d 6174 7269 780d 0a20 2020  data matrix..   
-00007f00: 2020 2020 203a 7274 7970 653a 2070 642e       :rtype: pd.
-00007f10: 4461 7461 4672 616d 650d 0a20 2020 2020  DataFrame..     
-00007f20: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
-00007f30: 6474 7970 6573 203d 205b 5d0d 0a20 2020  dtypes = []..   
-00007f40: 2020 2020 2069 6620 696e 636c 7564 655f       if include_
-00007f50: 6361 7465 676f 7269 6361 6c3a 0d0a 2020  categorical:..  
-00007f60: 2020 2020 2020 2020 2020 6474 7970 6573            dtypes
-00007f70: 2e61 7070 656e 6428 2263 6174 6567 6f72  .append("categor
-00007f80: 7922 290d 0a20 2020 2020 2020 2069 6620  y")..        if 
-00007f90: 696e 636c 7564 655f 6e75 6d65 7269 6361  include_numerica
-00007fa0: 6c3a 0d0a 2020 2020 2020 2020 2020 2020  l:..            
-00007fb0: 6474 7970 6573 202b 3d20 5b22 666c 6f61  dtypes += ["floa
-00007fc0: 7422 2c20 2269 6e74 225d 0d0a 2020 2020  t", "int"]..    
-00007fd0: 2020 2020 756e 6578 706c 6169 6e65 645f      unexplained_
-00007fe0: 636f 6c73 203d 2073 656c 662e 6164 6174  cols = self.adat
-00007ff0: 612e 6f62 732e 7365 6c65 6374 5f64 7479  a.obs.select_dty
-00008000: 7065 7328 6578 636c 7564 653d 2822 6361  pes(exclude=("ca
-00008010: 7465 676f 7279 222c 2022 666c 6f61 7422  tegory", "float"
-00008020: 2c20 2269 6e74 2229 292e 636f 6c75 6d6e  , "int")).column
-00008030: 730d 0a20 2020 2020 2020 2069 6620 6c65  s..        if le
-00008040: 6e28 756e 6578 706c 6169 6e65 645f 636f  n(unexplained_co
-00008050: 6c73 2920 3e20 303a 0d0a 2020 2020 2020  ls) > 0:..      
-00008060: 2020 2020 2020 756e 6578 706c 6169 6e65        unexplaine
-00008070: 645f 636f 6c5f 7374 7220 3d20 222c 2022  d_col_str = ", "
-00008080: 2e6a 6f69 6e28 756e 6578 706c 6169 6e65  .join(unexplaine
-00008090: 645f 636f 6c73 290d 0a20 2020 2020 2020  d_cols)..       
-000080a0: 2020 2020 2072 6169 7365 2056 616c 7565       raise Value
-000080b0: 4572 726f 7228 6622 7b75 6e65 7870 6c61  Error(f"{unexpla
-000080c0: 696e 6564 5f63 6f6c 5f73 7472 7d20 6d65  ined_col_str} me
-000080d0: 7461 6461 7461 2063 6f6c 756d 6e73 2068  tadata columns h
-000080e0: 6176 6520 756e 7265 636f 676e 697a 6564  ave unrecognized
-000080f0: 2064 7479 7065 732e 2229 0d0a 2020 2020   dtypes.")..    
-00008100: 2020 2020 6466 203d 2073 656c 662e 6164      df = self.ad
-00008110: 6174 612e 6f62 732e 7365 6c65 6374 5f64  ata.obs.select_d
-00008120: 7479 7065 7328 696e 636c 7564 653d 6474  types(include=dt
-00008130: 7970 6573 290d 0a20 2020 2020 2020 2064  ypes)..        d
-00008140: 6620 3d20 6466 2e64 726f 706e 6128 6178  f = df.dropna(ax
-00008150: 6973 3d31 2c20 686f 773d 2261 6c6c 2229  is=1, how="all")
-00008160: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-00008170: 2064 660d 0a20 2020 200d 0a20 2020 2064   df..    ..    d
-00008180: 6566 2067 6574 5f63 6174 6567 6f72 795f  ef get_category_
-00008190: 6f76 6572 7265 7072 6573 656e 7461 7469  overrepresentati
-000081a0: 6f6e 2873 656c 662c 0d0a 2020 2020 2020  on(self,..      
-000081b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000081c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000081d0: 2020 6c61 7965 723a 2073 7472 2c0d 0a20    layer: str,.. 
-000081e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000081f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008200: 2020 2020 2020 2074 7275 6e63 6174 655f         truncate_
-00008210: 6e65 6761 7469 7665 3a20 626f 6f6c 203d  negative: bool =
-00008220: 2054 7275 650d 0a20 2020 2020 2020 2020   True..         
+00003c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003c30: 2020 2020 2020 2020 2020 2873 656c 662e            (self.
+00003c40: 6164 6174 612e 7661 725b 226d 6561 6e22  adata.var["mean"
+00003c50: 5d20 3d3d 2030 2920 7c0d 0a20 2020 2020  ] == 0) |..     
+00003c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003c80: 2020 2020 2020 2020 2073 656c 662e 6164           self.ad
+00003c90: 6174 612e 7661 725b 226c 6f67 5f76 6172  ata.var["log_var
+00003ca0: 6961 6e63 6522 5d2e 6973 6e75 6c6c 2829  iance"].isnull()
+00003cb0: 290d 0a0d 0a20 2020 2020 2020 2023 206d  )....        # m
+00003cc0: 6f64 656c 206d 6561 6e2d 7661 7269 616e  odel mean-varian
+00003cd0: 6365 2072 656c 6174 696f 6e73 6869 7020  ce relationship 
+00003ce0: 7573 696e 6720 6765 6e65 7261 6c69 7a65  using generalize
+00003cf0: 6420 6164 6469 7469 7665 206d 6f64 656c  d additive model
+00003d00: 2077 6974 6820 736d 6f6f 7468 2063 6f6d   with smooth com
+00003d10: 706f 6e65 6e74 730d 0a20 2020 2020 2020  ponents..       
+00003d20: 2064 665f 6d6f 6465 6c20 3d20 7365 6c66   df_model = self
+00003d30: 2e61 6461 7461 2e76 6172 5b7e 7365 6c66  .adata.var[~self
+00003d40: 2e61 6461 7461 2e76 6172 5b22 6f64 7363  .adata.var["odsc
+00003d50: 6f72 655f 6578 636c 7564 6564 225d 5d0d  ore_excluded"]].
+00003d60: 0a20 2020 2020 2020 2062 7320 3d20 4253  .        bs = BS
+00003d70: 706c 696e 6573 2864 665f 6d6f 6465 6c5b  plines(df_model[
+00003d80: 226d 6561 6e22 5d2c 2064 663d 6f64 675f  "mean"], df=odg_
+00003d90: 6465 6661 756c 745f 646f 662c 2064 6567  default_dof, deg
+00003da0: 7265 653d 6f64 675f 6465 6661 756c 745f  ree=odg_default_
+00003db0: 7370 6c69 6e65 5f64 6567 7265 6529 0d0a  spline_degree)..
+00003dc0: 2020 2020 2020 2020 6761 6d20 3d20 474c          gam = GL
+00003dd0: 4d47 616d 2e66 726f 6d5f 666f 726d 756c  MGam.from_formul
+00003de0: 6128 226c 6f67 5f76 6172 6961 6e63 6520  a("log_variance 
+00003df0: 7e20 6c6f 675f 6d65 616e 222c 2064 6174  ~ log_mean", dat
+00003e00: 613d 6466 5f6d 6f64 656c 2c20 736d 6f6f  a=df_model, smoo
+00003e10: 7468 6572 3d62 7329 2e66 6974 2829 0d0a  ther=bs).fit()..
+00003e20: 2020 2020 2020 2020 7365 6c66 2e61 6461          self.ada
+00003e30: 7461 2e76 6172 5b22 7265 7369 645f 6c6f  ta.var["resid_lo
+00003e40: 675f 7661 7269 616e 6365 225d 203d 2067  g_variance"] = g
+00003e50: 616d 2e72 6573 6964 5f72 6573 706f 6e73  am.resid_respons
+00003e60: 650d 0a20 2020 2020 2020 2073 656c 662e  e..        self.
+00003e70: 6164 6174 612e 7661 725b 226f 6473 636f  adata.var["odsco
+00003e80: 7265 225d 203d 206e 702e 7371 7274 2831  re"] = np.sqrt(1
+00003e90: 3020 2a2a 2073 656c 662e 6164 6174 612e  0 ** self.adata.
+00003ea0: 7661 725b 2272 6573 6964 5f6c 6f67 5f76  var["resid_log_v
+00003eb0: 6172 6961 6e63 6522 5d29 0d0a 2020 2020  ariance"])..    
+00003ec0: 2020 2020 7365 6c66 2e61 6461 7461 2e76      self.adata.v
+00003ed0: 6172 5b22 6761 6d5f 6669 7474 6564 7661  ar["gam_fittedva
+00003ee0: 6c75 6573 225d 203d 2067 616d 2e66 6974  lues"] = gam.fit
+00003ef0: 7465 6476 616c 7565 730d 0a0d 0a0d 0a20  tedvalues...... 
+00003f00: 2020 2020 2020 2023 206d 6f64 656c 206d         # model m
+00003f10: 6561 6e2d 7661 7269 616e 6365 2072 656c  ean-variance rel
+00003f20: 6174 696f 6e73 6869 7020 7573 696e 6720  ationship using 
+00003f30: 634e 4d46 2773 206d 6574 686f 6420 6261  cNMF's method ba
+00003f40: 7365 6420 6f6e 2076 2d73 636f 7265 2061  sed on v-score a
+00003f50: 6e64 206d 696e 696d 756d 2065 7870 7265  nd minimum expre
+00003f60: 7373 696f 6e20 7468 7265 7368 6f6c 640d  ssion threshold.
+00003f70: 0a20 2020 2020 2020 2076 7363 6f72 655f  .        vscore_
+00003f80: 7374 6174 7320 3d20 7064 2e44 6174 6146  stats = pd.DataF
+00003f90: 7261 6d65 2863 6e6d 662e 6765 745f 6869  rame(cnmf.get_hi
+00003fa0: 6768 7661 725f 6765 6e65 7328 696e 7075  ghvar_genes(inpu
+00003fb0: 745f 636f 756e 7473 3d64 6174 615f 6e6f  t_counts=data_no
+00003fc0: 726d 616c 697a 6564 2e76 616c 7565 732c  rmalized.values,
+00003fd0: 206d 696e 696d 616c 5f6d 6561 6e3d 3029   minimal_mean=0)
+00003fe0: 5b30 5d29 0d0a 2020 2020 2020 2020 7673  [0])..        vs
+00003ff0: 636f 7265 5f73 7461 7473 2e69 6e64 6578  core_stats.index
+00004000: 203d 2064 6174 615f 6e6f 726d 616c 697a   = data_normaliz
+00004010: 6564 2e63 6f6c 756d 6e73 0d0a 2020 2020  ed.columns..    
+00004020: 2020 2020 7365 6c66 2e61 6461 7461 2e76      self.adata.v
+00004030: 6172 5b22 7673 636f 7265 225d 203d 2076  ar["vscore"] = v
+00004040: 7363 6f72 655f 7374 6174 735b 2266 616e  score_stats["fan
+00004050: 6f5f 7261 7469 6f22 5d0d 0a20 2020 2020  o_ratio"]..     
+00004060: 2020 2073 656c 662e 6164 6174 612e 756e     self.adata.un
+00004070: 735b 226f 6467 225d 5b22 6f64 675f 6465  s["odg"]["odg_de
+00004080: 6661 756c 745f 7370 6c69 6e65 5f64 6567  fault_spline_deg
+00004090: 7265 6522 5d20 3d20 6f64 675f 6465 6661  ree"] = odg_defa
+000040a0: 756c 745f 7370 6c69 6e65 5f64 6567 7265  ult_spline_degre
+000040b0: 650d 0a20 2020 2020 2020 2073 656c 662e  e..        self.
+000040c0: 6164 6174 612e 756e 735b 226f 6467 225d  adata.uns["odg"]
+000040d0: 5b22 6f64 675f 6465 6661 756c 745f 646f  ["odg_default_do
+000040e0: 6622 5d20 3d20 6f64 675f 6465 6661 756c  f"] = odg_defaul
+000040f0: 745f 646f 660d 0a20 2020 2020 2020 2073  t_dof..        s
+00004100: 656c 662e 6170 7065 6e64 5f74 6f5f 6869  elf.append_to_hi
+00004110: 7374 6f72 7928 2247 656e 652d 6c65 7665  story("Gene-leve
+00004120: 6c20 7374 6174 6973 7469 6373 2061 6e64  l statistics and
+00004130: 206f 7665 7264 6973 7065 7273 696f 6e20   overdispersion 
+00004140: 6d6f 6465 6c6c 696e 6720 636f 6d70 6c65  modelling comple
+00004150: 7465 642e 2229 0d0a 2020 2020 2020 2020  ted.")..        
+00004160: 0d0a 2020 2020 6465 6620 7365 6c65 6374  ..    def select
+00004170: 5f6f 7665 7264 6973 7065 7273 6564 5f67  _overdispersed_g
+00004180: 656e 6573 5f66 726f 6d5f 6765 6e65 6c69  enes_from_geneli
+00004190: 7374 2873 656c 662c 2067 656e 6573 3a20  st(self, genes: 
+000041a0: 436f 6c6c 6563 7469 6f6e 2c20 6d69 6e5f  Collection, min_
+000041b0: 6d65 616e 3d30 293a 0d0a 2020 2020 2020  mean=0):..      
+000041c0: 2020 2222 2253 656c 6563 7420 6f76 6572    """Select over
+000041d0: 6469 7370 6572 7365 6420 6765 6e65 732f  dispersed genes/
+000041e0: 6665 6174 7572 6573 2075 7369 6e67 2061  features using a
+000041f0: 2063 7573 746f 6d20 6c69 7374 2e20 4765   custom list. Ge
+00004200: 6e65 732f 6665 6174 7572 6573 206e 6f74  nes/features not
+00004210: 2070 7265 7365 6e74 2069 6e20 7468 6520   present in the 
+00004220: 6461 7461 7365 7420 6172 6520 6175 746f  dataset are auto
+00004230: 6d61 7469 6361 6c6c 7920 6669 6c74 6572  matically filter
+00004240: 6564 206f 7574 2e0d 0a0d 0a20 2020 2020  ed out.....     
+00004250: 2020 203a 7061 7261 6d20 6765 6e65 733a     :param genes:
+00004260: 2067 656e 6520 6c69 7374 0d0a 2020 2020   gene list..    
+00004270: 2020 2020 3a74 7970 6520 6765 6e65 733a      :type genes:
+00004280: 2043 6f6c 6c65 6374 696f 6e0d 0a20 2020   Collection..   
+00004290: 2020 2020 203a 7061 7261 6d20 6d69 6e5f       :param min_
+000042a0: 6d65 616e 3a20 6d69 6e69 6d75 6d20 6765  mean: minimum ge
+000042b0: 6e65 2065 7870 7265 7373 696f 6e20 666f  ne expression fo
+000042c0: 7220 6765 6e65 7320 746f 2062 6520 636f  r genes to be co
+000042d0: 756e 7465 6420 6173 206f 7665 7264 6973  unted as overdis
+000042e0: 7065 7273 6564 2c20 6465 6661 756c 7473  persed, defaults
+000042f0: 2074 6f20 300d 0a20 2020 2020 2020 203a   to 0..        :
+00004300: 7479 7065 206d 696e 5f6d 6561 6e3a 2069  type min_mean: i
+00004310: 6e74 2c20 6f70 7469 6f6e 616c 0d0a 2020  nt, optional..  
+00004320: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
+00004330: 2020 2073 656c 662e 6164 6174 612e 7661     self.adata.va
+00004340: 725b 2273 656c 6563 7465 6422 5d20 3d20  r["selected"] = 
+00004350: 7365 6c66 2e61 6461 7461 2e76 6172 2e69  self.adata.var.i
+00004360: 6e64 6578 2e69 7369 6e28 6765 6e65 7329  ndex.isin(genes)
+00004370: 2026 2073 656c 662e 6164 6174 612e 7661   & self.adata.va
+00004380: 725b 226d 6561 6e5f 636f 756e 7473 225d  r["mean_counts"]
+00004390: 203e 3d20 6d69 6e5f 6d65 616e 0d0a 2020   >= min_mean..  
+000043a0: 2020 2020 2020 7365 6c66 2e61 6461 7461        self.adata
+000043b0: 2e75 6e73 5b22 6f64 6722 5d5b 226f 7665  .uns["odg"]["ove
+000043c0: 7264 6973 7065 7273 696f 6e5f 6d65 7472  rdispersion_metr
+000043d0: 6963 225d 203d 2022 220d 0a20 2020 2020  ic"] = ""..     
+000043e0: 2020 2073 656c 662e 6164 6174 612e 756e     self.adata.un
+000043f0: 735b 226f 6467 225d 5b22 6d69 6e5f 6d65  s["odg"]["min_me
+00004400: 616e 225d 203d 206d 696e 5f6d 6561 6e0d  an"] = min_mean.
+00004410: 0a20 2020 2020 2020 2073 656c 662e 6164  .        self.ad
+00004420: 6174 612e 756e 735b 226f 6467 225d 5b22  ata.uns["odg"]["
+00004430: 6d69 6e5f 7363 6f72 6522 5d20 3d20 2222  min_score"] = ""
+00004440: 0d0a 2020 2020 2020 2020 7365 6c66 2e61  ..        self.a
+00004450: 6461 7461 2e75 6e73 5b22 6f64 6722 5d5b  data.uns["odg"][
+00004460: 2274 6f70 5f6e 225d 203d 2022 220d 0a20  "top_n"] = "".. 
+00004470: 2020 2020 2020 2073 656c 662e 6164 6174         self.adat
+00004480: 612e 756e 735b 226f 6467 225d 5b22 7175  a.uns["odg"]["qu
+00004490: 616e 7469 6c65 225d 203d 2022 220d 0a20  antile"] = "".. 
+000044a0: 2020 2020 2020 2073 656c 662e 6170 7065         self.appe
+000044b0: 6e64 5f74 6f5f 6869 7374 6f72 7928 224f  nd_to_history("O
+000044c0: 7665 7264 6973 7065 7273 6564 2067 656e  verdispersed gen
+000044d0: 6573 2073 656c 6563 7465 6420 6672 6f6d  es selected from
+000044e0: 2063 7573 746f 6d20 6765 6e65 206c 6973   custom gene lis
+000044f0: 7422 290d 0a20 2020 2020 2020 200d 0a20  t")..        .. 
+00004500: 2020 2064 6566 2073 656c 6563 745f 6f76     def select_ov
+00004510: 6572 6469 7370 6572 7365 645f 6765 6e65  erdispersed_gene
+00004520: 7328 7365 6c66 2c0d 0a20 2020 2020 2020  s(self,..       
+00004530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004540: 2020 2020 2020 2020 2020 2020 6f76 6572              over
+00004550: 6469 7370 6572 7369 6f6e 5f6d 6574 7269  dispersion_metri
+00004560: 633a 2073 7472 203d 2022 6f64 7363 6f72  c: str = "odscor
+00004570: 6522 2c0d 0a20 2020 2020 2020 2020 2020  e",..           
+00004580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004590: 2020 2020 2020 2020 6d69 6e5f 6d65 616e          min_mean
+000045a0: 3a20 666c 6f61 7420 3d20 302c 0d0a 2020  : float = 0,..  
+000045b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000045c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000045d0: 206d 696e 5f73 636f 7265 3a20 666c 6f61   min_score: floa
+000045e0: 7420 3d20 312e 302c 0d0a 2020 2020 2020  t = 1.0,..      
+000045f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004600: 2020 2020 2020 2020 2020 2020 2074 6f70               top
+00004610: 5f6e 3a20 696e 7420 3d20 4e6f 6e65 2c0d  _n: int = None,.
+00004620: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004640: 2020 2020 7175 616e 7469 6c65 3a20 666c      quantile: fl
+00004650: 6f61 7420 3d20 4e6f 6e65 293a 0d0a 2020  oat = None):..  
+00004660: 2020 2020 2020 2222 2253 656c 6563 7420        """Select 
+00004670: 6f76 6572 6469 7370 6572 7365 6420 6765  overdispersed ge
+00004680: 6e65 732f 6665 6174 7572 6573 2075 7369  nes/features usi
+00004690: 6e67 2061 6e20 6f76 6572 6469 7370 6572  ng an overdisper
+000046a0: 7369 6f6e 206d 6574 7269 632e 204f 7074  sion metric. Opt
+000046b0: 696f 6e61 6c6c 7920 7365 7420 6120 6d69  ionally set a mi
+000046c0: 6e69 6d75 6d20 6765 6e65 2065 7870 7265  nimum gene expre
+000046d0: 7373 696f 6e20 6c65 7665 6c2e 0d0a 2020  ssion level...  
+000046e0: 2020 2020 2020 5365 7420 6120 7468 7265        Set a thre
+000046f0: 7368 6f6c 6420 7573 696e 6720 7468 6520  shold using the 
+00004700: 746f 7020 4e20 2827 746f 705f 6e27 292c  top N ('top_n'),
+00004710: 206d 696e 696d 756d 2073 636f 7265 2028   minimum score (
+00004720: 276d 696e 5f73 636f 7265 2729 2c20 6f72  'min_score'), or
+00004730: 2070 726f 706f 7274 696f 6e20 6f66 2066   proportion of f
+00004740: 6561 7475 7265 7320 2827 7175 616e 7469  eatures ('quanti
+00004750: 6c65 2729 206d 6574 686f 6473 2e0d 0a20  le') methods... 
+00004760: 2020 2020 2020 204f 7665 7264 6973 7065         Overdispe
+00004770: 7273 6564 2067 656e 6520 6c69 7374 2069  rsed gene list i
+00004780: 7320 7361 7665 6420 696e 2074 6865 2044  s saved in the D
+00004790: 6174 6173 6574 206f 626a 6563 742e 0d0a  ataset object...
+000047a0: 0d0a 2020 2020 2020 2020 3a70 6172 616d  ..        :param
+000047b0: 206f 7665 7264 6973 7065 7273 696f 6e5f   overdispersion_
+000047c0: 6d65 7472 6963 3a20 226f 6473 636f 7265  metric: "odscore
+000047d0: 2220 6f72 2022 7673 636f 7265 222c 2064  " or "vscore", d
+000047e0: 6566 6175 6c74 7320 746f 2022 6f64 7363  efaults to "odsc
+000047f0: 6f72 6522 0d0a 2020 2020 2020 2020 3a74  ore"..        :t
+00004800: 7970 6520 6f76 6572 6469 7370 6572 7369  ype overdispersi
+00004810: 6f6e 5f6d 6574 7269 633a 2073 7472 2c20  on_metric: str, 
+00004820: 6f70 7469 6f6e 616c 0d0a 2020 2020 2020  optional..      
+00004830: 2020 3a70 6172 616d 206d 696e 5f6d 6561    :param min_mea
+00004840: 6e3a 206d 696e 696d 756d 2067 656e 6520  n: minimum gene 
+00004850: 6578 7072 6573 7369 6f6e 2066 6f72 2067  expression for g
+00004860: 656e 6573 2074 6f20 6265 2063 6f75 6e74  enes to be count
+00004870: 6564 2061 7320 6f76 6572 6469 7370 6572  ed as overdisper
+00004880: 7365 642c 2064 6566 6175 6c74 7320 746f  sed, defaults to
+00004890: 2030 0d0a 2020 2020 2020 2020 3a74 7970   0..        :typ
+000048a0: 6520 6d69 6e5f 6d65 616e 3a20 696e 742c  e min_mean: int,
+000048b0: 206f 7074 696f 6e61 6c0d 0a20 2020 2020   optional..     
+000048c0: 2020 203a 7061 7261 6d20 6d69 6e5f 7363     :param min_sc
+000048d0: 6f72 653a 206d 696e 696d 756d 2073 636f  ore: minimum sco
+000048e0: 7265 2066 6f72 206f 7665 7264 6973 7065  re for overdispe
+000048f0: 7273 696f 6e2c 2064 6566 6175 6c74 7320  rsion, defaults 
+00004900: 746f 2031 2e30 0d0a 2020 2020 2020 2020  to 1.0..        
+00004910: 3a74 7970 6520 6d69 6e5f 7363 6f72 653a  :type min_score:
+00004920: 2066 6c6f 6174 2c20 6f70 7469 6f6e 616c   float, optional
+00004930: 0d0a 2020 2020 2020 2020 3a70 6172 616d  ..        :param
+00004940: 2074 6f70 5f6e 3a20 4368 6f6f 7365 2074   top_n: Choose t
+00004950: 6865 2074 6f70 204e 206d 6f73 7420 6f76  he top N most ov
+00004960: 6572 6469 7370 6572 7365 6420 6765 6e65  erdispersed gene
+00004970: 732c 2064 6566 6175 6c74 7320 746f 204e  s, defaults to N
+00004980: 6f6e 650d 0a20 2020 2020 2020 203a 7479  one..        :ty
+00004990: 7065 2074 6f70 5f6e 3a20 696e 742c 206f  pe top_n: int, o
+000049a0: 7074 696f 6e61 6c0d 0a20 2020 2020 2020  ptional..       
+000049b0: 203a 7061 7261 6d20 7175 616e 7469 6c65   :param quantile
+000049c0: 3a20 4368 6f6f 7365 2061 2071 7561 6e74  : Choose a quant
+000049d0: 696c 6520 6f66 206f 7665 7264 6973 7065  ile of overdispe
+000049e0: 7273 696f 6e2e 2046 6f72 2065 7861 6d70  rsion. For examp
+000049f0: 6c65 2c20 7468 6520 746f 7020 3130 2520  le, the top 10% 
+00004a00: 6f66 206f 7665 7264 6973 7065 7273 6564  of overdispersed
+00004a10: 2067 656e 6573 2077 6f75 6c64 2062 6520   genes would be 
+00004a20: 302e 3130 2e20 4465 6661 756c 7473 2074  0.10. Defaults t
+00004a30: 6f20 4e6f 6e65 0d0a 2020 2020 2020 2020  o None..        
+00004a40: 3a74 7970 6520 7175 616e 7469 6c65 3a20  :type quantile: 
+00004a50: 666c 6f61 742c 206f 7074 696f 6e61 6c0d  float, optional.
+00004a60: 0a20 2020 2020 2020 203a 7261 6973 6573  .        :raises
+00004a70: 2056 616c 7565 4572 726f 723a 2045 7272   ValueError: Err
+00004a80: 6f72 2069 6620 696e 7661 6c69 6420 6f76  or if invalid ov
+00004a90: 6572 6469 7370 6572 7369 6f6e 206d 6574  erdispersion met
+00004aa0: 7269 6320 6973 2063 686f 7365 6e2e 0d0a  ric is chosen...
+00004ab0: 2020 2020 2020 2020 2222 220d 0a20 2020          """..   
+00004ac0: 2020 2020 200d 0a20 2020 2020 2020 2069       ..        i
+00004ad0: 6620 6f76 6572 6469 7370 6572 7369 6f6e  f overdispersion
+00004ae0: 5f6d 6574 7269 6320 6e6f 7420 696e 2073  _metric not in s
+00004af0: 656c 662e 6164 6174 612e 7661 722e 636f  elf.adata.var.co
+00004b00: 6c75 6d6e 733a 0d0a 2020 2020 2020 2020  lumns:..        
+00004b10: 2020 2020 6966 206f 7665 7264 6973 7065      if overdispe
+00004b20: 7273 696f 6e5f 6d65 7472 6963 2069 6e20  rsion_metric in 
+00004b30: 2822 6f64 7363 6f72 6522 2c20 2276 7363  ("odscore", "vsc
+00004b40: 6f72 6522 293a 0d0a 2020 2020 2020 2020  ore"):..        
+00004b50: 2020 2020 2020 2020 7261 6973 6520 5661          raise Va
+00004b60: 6c75 6545 7272 6f72 280d 0a20 2020 2020  lueError(..     
+00004b70: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00004b80: 227b 6f76 6572 6469 7370 6572 7369 6f6e  "{overdispersion
+00004b90: 5f6d 6574 7269 637d 2068 6173 206e 6f74  _metric} has not
+00004ba0: 2062 6565 6e20 6361 6c63 756c 6174 6564   been calculated
+00004bb0: 2066 6f72 2074 6869 7320 6461 7461 7365   for this datase
+00004bc0: 742e 2022 0d0a 2020 2020 2020 2020 2020  t. "..          
+00004bd0: 2020 2020 2020 2020 2020 2245 6e73 7572            "Ensur
+00004be0: 6520 7468 6174 2079 6f75 2063 616c 6c20  e that you call 
+00004bf0: 7468 6520 6044 6174 6173 6574 2e63 6f6d  the `Dataset.com
+00004c00: 7075 7465 5f67 656e 655f 7374 6174 7328  pute_gene_stats(
+00004c10: 2960 2066 6972 7374 2e22 0d0a 2020 2020  )` first."..    
+00004c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004c30: 290d 0a20 2020 2020 2020 2020 2020 2065  )..            e
+00004c40: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
+00004c50: 2020 2020 2020 7261 6973 6520 5661 6c75        raise Valu
+00004c60: 6545 7272 6f72 280d 0a20 2020 2020 2020  eError(..       
+00004c70: 2020 2020 2020 2020 2020 2020 2066 227b               f"{
+00004c80: 6f76 6572 6469 7370 6572 7369 6f6e 5f6d  overdispersion_m
+00004c90: 6574 7269 637d 2069 7320 6e6f 7420 6120  etric} is not a 
+00004ca0: 7661 6c69 6420 6f76 6572 6469 7370 6572  valid overdisper
+00004cb0: 7369 6f6e 206d 6574 7269 632e 220d 0a20  sion metric.".. 
+00004cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004cd0: 2020 2029 0d0a 2020 2020 2020 2020 0d0a     )..        ..
+00004ce0: 2020 2020 2020 2020 2320 7761 726e 2069          # warn i
+00004cf0: 6620 6d75 6c74 6970 6c65 206d 6574 686f  f multiple metho
+00004d00: 6473 2061 7265 2073 656c 6563 7465 640d  ds are selected.
+00004d10: 0a20 2020 2020 2020 2073 656c 6563 7465  .        selecte
+00004d20: 645f 6d65 7468 6f64 7320 3d20 5b5d 0d0a  d_methods = []..
+00004d30: 2020 2020 2020 2020 6966 206d 696e 5f73          if min_s
+00004d40: 636f 7265 2069 7320 6e6f 7420 4e6f 6e65  core is not None
+00004d50: 3a0d 0a20 2020 2020 2020 2020 2020 2073  :..            s
+00004d60: 656c 6563 7465 645f 6d65 7468 6f64 732e  elected_methods.
+00004d70: 6170 7065 6e64 2822 6d69 6e5f 7363 6f72  append("min_scor
+00004d80: 6522 290d 0a20 2020 2020 2020 2069 6620  e")..        if 
+00004d90: 746f 705f 6e20 6973 206e 6f74 204e 6f6e  top_n is not Non
+00004da0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+00004db0: 7365 6c65 6374 6564 5f6d 6574 686f 6473  selected_methods
+00004dc0: 2e61 7070 656e 6428 2274 6f70 5f6e 2229  .append("top_n")
+00004dd0: 0d0a 2020 2020 2020 2020 6966 2071 7561  ..        if qua
+00004de0: 6e74 696c 6520 6973 206e 6f74 204e 6f6e  ntile is not Non
+00004df0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+00004e00: 7365 6c65 6374 6564 5f6d 6574 686f 6473  selected_methods
+00004e10: 2e61 7070 656e 6428 2271 7561 6e74 696c  .append("quantil
+00004e20: 6522 290d 0a20 2020 2020 2020 2069 6620  e")..        if 
+00004e30: 6c65 6e28 7365 6c65 6374 6564 5f6d 6574  len(selected_met
+00004e40: 686f 6473 2920 3e20 313a 0d0a 2020 2020  hods) > 1:..    
+00004e50: 2020 2020 2020 2020 6d65 7468 6f64 7761          methodwa
+00004e60: 726e 7374 7220 3d20 222c 2022 2e6a 6f69  rnstr = ", ".joi
+00004e70: 6e28 7365 6c65 6374 6564 5f6d 6574 686f  n(selected_metho
+00004e80: 6473 290d 0a20 2020 2020 2020 2020 2020  ds)..           
+00004e90: 206c 6f67 6769 6e67 2e77 6172 6e69 6e67   logging.warning
+00004ea0: 2866 224d 756c 7469 706c 6520 636f 6e66  (f"Multiple conf
+00004eb0: 6c69 6374 696e 6720 6f76 6572 6469 7370  licting overdisp
+00004ec0: 6572 7365 6420 6765 6e65 2073 656c 6563  ersed gene selec
+00004ed0: 7469 6f6e 2063 7269 7465 7269 6120 6861  tion criteria ha
+00004ee0: 7665 2062 6565 6e20 7365 6c65 6374 6564  ve been selected
+00004ef0: 3a20 7b6d 6574 686f 6477 6172 6e73 7472  : {methodwarnstr
+00004f00: 7d2e 2022 0d0a 2020 2020 2020 2020 2020  }. "..          
+00004f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004f20: 2020 224f 6e6c 7920 7468 6520 696e 7465    "Only the inte
+00004f30: 7273 6563 7469 6f6e 206f 6620 7468 6573  rsection of thes
+00004f40: 6520 6d65 7468 6f64 7320 7769 6c6c 2062  e methods will b
+00004f50: 6520 7365 6c65 6374 6564 2e22 290d 0a20  e selected.").. 
+00004f60: 2020 2020 2020 2020 2020 2020 2020 200d                 .
+00004f70: 0a20 2020 2020 2020 2023 206d 696e 5f6d  .        # min_m
+00004f80: 6561 6e20 6669 6c74 6572 0d0a 2020 2020  ean filter..    
+00004f90: 2020 2020 7365 6c65 6374 6564 5f67 656e      selected_gen
+00004fa0: 6573 203d 2073 656c 662e 6164 6174 612e  es = self.adata.
+00004fb0: 7661 725b 226d 6561 6e5f 636f 756e 7473  var["mean_counts
+00004fc0: 225d 203e 3d20 6d69 6e5f 6d65 616e 0d0a  "] >= min_mean..
+00004fd0: 2020 2020 2020 2020 2320 6d69 6e5f 7363          # min_sc
+00004fe0: 6f72 6520 6669 6c74 6572 0d0a 2020 2020  ore filter..    
+00004ff0: 2020 2020 6966 206d 696e 5f73 636f 7265      if min_score
+00005000: 2069 7320 6e6f 7420 4e6f 6e65 3a0d 0a20   is not None:.. 
+00005010: 2020 2020 2020 2020 2020 2073 656c 6563             selec
+00005020: 7465 645f 6765 6e65 7320 3d20 7365 6c65  ted_genes = sele
+00005030: 6374 6564 5f67 656e 6573 2026 2028 7365  cted_genes & (se
+00005040: 6c66 2e61 6461 7461 2e76 6172 5b6f 7665  lf.adata.var[ove
+00005050: 7264 6973 7065 7273 696f 6e5f 6d65 7472  rdispersion_metr
+00005060: 6963 5d20 3e3d 206d 696e 5f73 636f 7265  ic] >= min_score
+00005070: 290d 0a20 2020 2020 2020 2023 2074 6f70  )..        # top
+00005080: 5f6e 2066 696c 7465 720d 0a20 2020 2020  _n filter..     
+00005090: 2020 2069 6620 746f 705f 6e20 6973 206e     if top_n is n
+000050a0: 6f74 204e 6f6e 653a 0d0a 2020 2020 2020  ot None:..      
+000050b0: 2020 2020 2020 6765 6e65 7320 3d20 7365        genes = se
+000050c0: 6c66 2e61 6461 7461 2e76 6172 5b6f 7665  lf.adata.var[ove
+000050d0: 7264 6973 7065 7273 696f 6e5f 6d65 7472  rdispersion_metr
+000050e0: 6963 5d2e 736f 7274 5f76 616c 7565 7328  ic].sort_values(
+000050f0: 6173 6365 6e64 696e 673d 4661 6c73 6529  ascending=False)
+00005100: 2e68 6561 6428 696e 7428 746f 705f 6e29  .head(int(top_n)
+00005110: 292e 696e 6465 780d 0a20 2020 2020 2020  ).index..       
+00005120: 2020 2020 2073 656c 6563 7465 645f 6765       selected_ge
+00005130: 6e65 7320 3d20 7365 6c65 6374 6564 5f67  nes = selected_g
+00005140: 656e 6573 2026 2073 656c 662e 6164 6174  enes & self.adat
+00005150: 612e 7661 722e 696e 6465 782e 6973 696e  a.var.index.isin
+00005160: 2867 656e 6573 290d 0a20 2020 2020 2020  (genes)..       
+00005170: 2023 2071 7561 6e74 696c 6520 6669 6c74   # quantile filt
+00005180: 6572 0d0a 2020 2020 2020 2020 6966 2071  er..        if q
+00005190: 7561 6e74 696c 6520 6973 206e 6f74 204e  uantile is not N
+000051a0: 6f6e 653a 0d0a 2020 2020 2020 2020 2020  one:..          
+000051b0: 2020 6e5f 746f 7461 6c5f 6765 6e65 7320    n_total_genes 
+000051c0: 3d20 7365 6c66 2e61 6461 7461 2e76 6172  = self.adata.var
+000051d0: 5b6f 7665 7264 6973 7065 7273 696f 6e5f  [overdispersion_
+000051e0: 6d65 7472 6963 5d2e 6e6f 746e 756c 6c28  metric].notnull(
+000051f0: 292e 7375 6d28 290d 0a20 2020 2020 2020  ).sum()..       
+00005200: 2020 2020 2067 656e 6573 203d 2073 656c       genes = sel
+00005210: 662e 6164 6174 612e 7661 725b 6f76 6572  f.adata.var[over
+00005220: 6469 7370 6572 7369 6f6e 5f6d 6574 7269  dispersion_metri
+00005230: 635d 2e73 6f72 745f 7661 6c75 6573 2861  c].sort_values(a
+00005240: 7363 656e 6469 6e67 3d46 616c 7365 292e  scending=False).
+00005250: 6865 6164 2869 6e74 2871 7561 6e74 696c  head(int(quantil
+00005260: 6520 2a20 6e5f 746f 7461 6c5f 6765 6e65  e * n_total_gene
+00005270: 7329 292e 696e 6465 780d 0a20 2020 2020  s)).index..     
+00005280: 2020 2020 2020 2073 656c 6563 7465 645f         selected_
+00005290: 6765 6e65 7320 3d20 7365 6c65 6374 6564  genes = selected
+000052a0: 5f67 656e 6573 2026 2073 656c 662e 6164  _genes & self.ad
+000052b0: 6174 612e 7661 722e 696e 6465 782e 6973  ata.var.index.is
+000052c0: 696e 2867 656e 6573 290d 0a0d 0a20 2020  in(genes)....   
+000052d0: 2020 2020 206e 5f73 656c 6563 7465 645f       n_selected_
+000052e0: 6765 6e65 7320 3d20 7365 6c65 6374 6564  genes = selected
+000052f0: 5f67 656e 6573 2e73 756d 2829 0d0a 2020  _genes.sum()..  
+00005300: 2020 2020 2020 6c6f 6767 696e 672e 696e        logging.in
+00005310: 666f 2866 227b 6e5f 7365 6c65 6374 6564  fo(f"{n_selected
+00005320: 5f67 656e 6573 7d20 6765 6e65 7320 7365  _genes} genes se
+00005330: 6c65 6374 6564 2066 6f72 2066 6163 746f  lected for facto
+00005340: 7269 7a61 7469 6f6e 2229 0d0a 2020 2020  rization")..    
+00005350: 2020 2020 0d0a 2020 2020 2020 2020 2320      ..        # 
+00005360: 6d61 6b65 2063 6861 6e67 6573 2074 6f20  make changes to 
+00005370: 4461 7461 7365 7420 6f62 6a65 6374 0d0a  Dataset object..
+00005380: 2020 2020 2020 2020 7365 6c66 2e61 6461          self.ada
+00005390: 7461 2e76 6172 5b22 7365 6c65 6374 6564  ta.var["selected
+000053a0: 225d 203d 2073 656c 6563 7465 645f 6765  "] = selected_ge
+000053b0: 6e65 730d 0a20 2020 2020 2020 2073 656c  nes..        sel
+000053c0: 662e 6164 6174 612e 756e 735b 226f 6467  f.adata.uns["odg
+000053d0: 225d 5b22 6f76 6572 6469 7370 6572 7369  "]["overdispersi
+000053e0: 6f6e 5f6d 6574 7269 6322 5d20 3d20 6f76  on_metric"] = ov
+000053f0: 6572 6469 7370 6572 7369 6f6e 5f6d 6574  erdispersion_met
+00005400: 7269 630d 0a20 2020 2020 2020 2073 656c  ric..        sel
+00005410: 662e 6164 6174 612e 756e 735b 226f 6467  f.adata.uns["odg
+00005420: 225d 5b22 6d69 6e5f 6d65 616e 225d 203d  "]["min_mean"] =
+00005430: 206d 696e 5f6d 6561 6e0d 0a20 2020 2020   min_mean..     
+00005440: 2020 2073 656c 662e 6164 6174 612e 756e     self.adata.un
+00005450: 735b 226f 6467 225d 5b22 6d69 6e5f 7363  s["odg"]["min_sc
+00005460: 6f72 6522 5d20 3d20 6d69 6e5f 7363 6f72  ore"] = min_scor
+00005470: 6520 6966 206d 696e 5f73 636f 7265 2069  e if min_score i
+00005480: 7320 6e6f 7420 4e6f 6e65 2065 6c73 6520  s not None else 
+00005490: 2222 0d0a 2020 2020 2020 2020 7365 6c66  ""..        self
+000054a0: 2e61 6461 7461 2e75 6e73 5b22 6f64 6722  .adata.uns["odg"
+000054b0: 5d5b 2274 6f70 5f6e 225d 203d 2074 6f70  ]["top_n"] = top
+000054c0: 5f6e 2069 6620 746f 705f 6e20 6973 206e  _n if top_n is n
+000054d0: 6f74 204e 6f6e 6520 656c 7365 2022 220d  ot None else "".
+000054e0: 0a20 2020 2020 2020 2073 656c 662e 6164  .        self.ad
+000054f0: 6174 612e 756e 735b 226f 6467 225d 5b22  ata.uns["odg"]["
+00005500: 7175 616e 7469 6c65 225d 203d 2071 7561  quantile"] = qua
+00005510: 6e74 696c 6520 6966 2071 7561 6e74 696c  ntile if quantil
+00005520: 6520 6973 206e 6f74 204e 6f6e 6520 656c  e is not None el
+00005530: 7365 2022 220d 0a20 2020 2020 2020 2073  se ""..        s
+00005540: 656c 662e 6170 7065 6e64 5f74 6f5f 6869  elf.append_to_hi
+00005550: 7374 6f72 7928 224f 7665 7264 6973 7065  story("Overdispe
+00005560: 7273 6564 2067 656e 6573 2073 656c 6563  rsed genes selec
+00005570: 7465 6422 290d 0a20 2020 200d 0a20 2020  ted")..    ..   
+00005580: 2064 6566 2069 6e69 7469 616c 697a 655f   def initialize_
+00005590: 636e 6d66 2873 656c 662c 2063 6e6d 665f  cnmf(self, cnmf_
+000055a0: 6f75 7470 7574 5f64 6972 3a20 7374 722c  output_dir: str,
+000055b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000055c0: 2020 2020 2020 2020 2020 636e 6d66 5f6e            cnmf_n
+000055d0: 616d 653a 2073 7472 2c0d 0a20 2020 2020  ame: str,..     
+000055e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000055f0: 2020 206b 7661 6c73 3a20 436f 6c6c 6563     kvals: Collec
+00005600: 7469 6f6e 203d 2072 616e 6765 2832 2c20  tion = range(2, 
+00005610: 3631 292c 0d0a 2020 2020 2020 2020 2020  61),..          
+00005620: 2020 2020 2020 2020 2020 2020 2020 6e5f                n_
+00005630: 6974 6572 3a20 696e 7420 3d20 3230 302c  iter: int = 200,
+00005640: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00005650: 2020 2020 2020 2020 2020 6265 7461 5f6c            beta_l
+00005660: 6f73 733a 2073 7472 203d 2022 6b75 6c6c  oss: str = "kull
+00005670: 6261 636b 2d6c 6569 626c 6572 222c 0d0a  back-leibler",..
+00005680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005690: 2020 2020 2020 2020 7365 6564 3a20 4f70          seed: Op
+000056a0: 7469 6f6e 616c 5b69 6e74 5d20 3d20 4e6f  tional[int] = No
+000056b0: 6e65 2920 2d3e 2063 6e6d 662e 634e 4d46  ne) -> cnmf.cNMF
+000056c0: 3a0d 0a20 2020 2020 2020 2022 2222 496e  :..        """In
+000056d0: 6974 6961 6c69 7a65 2061 2063 4e4d 4620  itialize a cNMF 
+000056e0: 7275 6e20 666f 7220 7375 6273 6571 7565  run for subseque
+000056f0: 6e74 2066 6163 746f 7269 7a61 7469 6f6e  nt factorization
+00005700: 2e0d 0a0d 0a20 2020 2020 2020 203a 7061  .....        :pa
+00005710: 7261 6d20 636e 6d66 5f6f 7574 7075 745f  ram cnmf_output_
+00005720: 6469 723a 204f 7574 7075 7420 6469 7265  dir: Output dire
+00005730: 6374 6f72 7920 666f 7220 634e 4d46 2072  ctory for cNMF r
+00005740: 6573 756c 7473 0d0a 2020 2020 2020 2020  esults..        
+00005750: 3a74 7970 6520 636e 6d66 5f6f 7574 7075  :type cnmf_outpu
+00005760: 745f 6469 723a 2073 7472 0d0a 2020 2020  t_dir: str..    
+00005770: 2020 2020 3a70 6172 616d 2063 6e6d 665f      :param cnmf_
+00005780: 6e61 6d65 3a20 4e61 6d65 206f 6620 7468  name: Name of th
+00005790: 6520 634e 4d46 2072 6573 756c 7473 2e20  e cNMF results. 
+000057a0: 4669 6c65 7320 7769 6c6c 2062 6520 6f75  Files will be ou
+000057b0: 7470 7574 2074 6f20 5b63 6e6d 665f 6f75  tput to [cnmf_ou
+000057c0: 7470 7574 5f64 6972 5d2f 5b63 6e6d 665f  tput_dir]/[cnmf_
+000057d0: 6e61 6d65 5d2f 0d0a 2020 2020 2020 2020  name]/..        
+000057e0: 3a74 7970 6520 636e 6d66 5f6e 616d 653a  :type cnmf_name:
+000057f0: 2073 7472 0d0a 2020 2020 2020 2020 3a70   str..        :p
+00005800: 6172 616d 206b 7661 6c73 3a20 5261 6e6b  aram kvals: Rank
+00005810: 7320 666f 7220 634e 4d46 2066 6163 746f  s for cNMF facto
+00005820: 7269 7a61 7469 6f6e 2c20 6465 6661 756c  rization, defaul
+00005830: 7473 2074 6f20 7261 6e67 6528 322c 2036  ts to range(2, 6
+00005840: 3129 0d0a 2020 2020 2020 2020 3a74 7970  1)..        :typ
+00005850: 6520 6b76 616c 733a 2043 6f6c 6c65 6374  e kvals: Collect
+00005860: 696f 6e2c 206f 7074 696f 6e61 6c0d 0a20  ion, optional.. 
+00005870: 2020 2020 2020 203a 7061 7261 6d20 6e5f         :param n_
+00005880: 6974 6572 3a20 4e75 6d62 6572 206f 6620  iter: Number of 
+00005890: 6974 6572 6174 696f 6e73 2066 726f 6d20  iterations from 
+000058a0: 7768 6963 6820 746f 2062 7569 6c64 2061  which to build a
+000058b0: 2063 6f6e 7365 6e73 7573 2073 6f6c 7574   consensus solut
+000058c0: 696f 6e2c 2064 6566 6175 6c74 7320 746f  ion, defaults to
+000058d0: 2032 3030 0d0a 2020 2020 2020 2020 3a74   200..        :t
+000058e0: 7970 6520 6e5f 6974 6572 3a20 696e 742c  ype n_iter: int,
+000058f0: 206f 7074 696f 6e61 6c0d 0a20 2020 2020   optional..     
+00005900: 2020 203a 7061 7261 6d20 6265 7461 5f6c     :param beta_l
+00005910: 6f73 733a 2062 6574 612d 6c6f 7373 2066  oss: beta-loss f
+00005920: 756e 6374 696f 6e2c 2065 6974 6865 7220  unction, either 
+00005930: 226b 756c 6c62 6163 6b2d 6c65 6962 6c65  "kullback-leible
+00005940: 7222 206f 7220 2266 726f 6265 6e69 7573  r" or "frobenius
+00005950: 222e 2044 6566 6175 6c74 7320 746f 2022  ". Defaults to "
+00005960: 6b75 6c6c 6261 636b 2d6c 6569 626c 6572  kullback-leibler
+00005970: 220d 0a20 2020 2020 2020 203a 7479 7065  "..        :type
+00005980: 2062 6574 615f 6c6f 7373 3a20 7374 722c   beta_loss: str,
+00005990: 206f 7074 696f 6e61 6c0d 0a20 2020 2020   optional..     
+000059a0: 2020 203a 7061 7261 6d20 7365 6564 3a20     :param seed: 
+000059b0: 5261 6e64 6f6d 2073 6565 6420 666f 7220  Random seed for 
+000059c0: 7265 7072 6f64 7563 6962 696c 6974 792c  reproducibility,
+000059d0: 2064 6566 6175 6c74 7320 746f 204e 6f6e   defaults to Non
+000059e0: 650d 0a20 2020 2020 2020 203a 7479 7065  e..        :type
+000059f0: 2073 6565 643a 204f 7074 696f 6e61 6c5b   seed: Optional[
+00005a00: 696e 745d 2c20 6f70 7469 6f6e 616c 0d0a  int], optional..
+00005a10: 2020 2020 2020 2020 3a72 6574 7572 6e3a          :return:
+00005a20: 2063 4e4d 4620 6f62 6a65 6374 0d0a 2020   cNMF object..  
+00005a30: 2020 2020 2020 3a72 7479 7065 3a20 3a63        :rtype: :c
+00005a40: 6c61 7373 3a60 636e 6d66 736e 732e 636e  lass:`cnmfsns.cn
+00005a50: 6d66 2e63 4e4d 4660 0d0a 2020 2020 2020  mf.cNMF`..      
+00005a60: 2020 2222 220d 0a20 2020 2020 2020 2063    """..        c
+00005a70: 6e6d 665f 6f62 6a20 3d20 636e 6d66 2e63  nmf_obj = cnmf.c
+00005a80: 4e4d 4628 6f75 7470 7574 5f64 6972 3d63  NMF(output_dir=c
+00005a90: 6e6d 665f 6f75 7470 7574 5f64 6972 2c20  nmf_output_dir, 
+00005aa0: 6e61 6d65 3d63 6e6d 665f 6e61 6d65 290d  name=cnmf_name).
+00005ab0: 0a20 2020 2020 2020 200d 0a20 2020 2020  .        ..     
+00005ac0: 2020 2023 2077 7269 7465 2054 504d 2028     # write TPM (
+00005ad0: 6e6f 726d 616c 697a 6564 2920 6461 7461  normalized) data
+00005ae0: 0d0a 2020 2020 2020 2020 7470 6d20 3d20  ..        tpm = 
+00005af0: 6164 2e41 6e6e 4461 7461 2873 656c 662e  ad.AnnData(self.
+00005b00: 746f 5f64 6628 6e6f 726d 616c 697a 6564  to_df(normalized
+00005b10: 3d54 7275 6529 290d 0a20 2020 2020 2020  =True))..       
+00005b20: 2074 706d 2e77 7269 7465 5f68 3561 6428   tpm.write_h5ad(
+00005b30: 636e 6d66 5f6f 626a 2e70 6174 6873 5b22  cnmf_obj.paths["
+00005b40: 7470 6d22 5d29 0d0a 0d0a 2020 2020 2020  tpm"])....      
+00005b50: 2020 6765 6e65 5f74 706d 5f6d 6561 6e20    gene_tpm_mean 
+00005b60: 3d20 6e70 2e61 7272 6179 2874 706d 2e58  = np.array(tpm.X
+00005b70: 2e6d 6561 6e28 6178 6973 3d30 2929 2e72  .mean(axis=0)).r
+00005b80: 6573 6861 7065 282d 3129 0d0a 2020 2020  eshape(-1)..    
+00005b90: 2020 2020 6765 6e65 5f74 706d 5f73 7464      gene_tpm_std
+00005ba0: 6465 7620 3d20 6e70 2e61 7272 6179 2874  dev = np.array(t
+00005bb0: 706d 2e58 2e73 7464 2861 7869 733d 302c  pm.X.std(axis=0,
+00005bc0: 2064 646f 663d 3029 292e 7265 7368 6170   ddof=0)).reshap
+00005bd0: 6528 2d31 290d 0a20 2020 2020 2020 2069  e(-1)..        i
+00005be0: 6e70 7574 5f74 706d 5f73 7461 7473 203d  nput_tpm_stats =
+00005bf0: 2070 642e 4461 7461 4672 616d 6528 5b67   pd.DataFrame([g
+00005c00: 656e 655f 7470 6d5f 6d65 616e 2c20 6765  ene_tpm_mean, ge
+00005c10: 6e65 5f74 706d 5f73 7464 6465 765d 2c20  ne_tpm_stddev], 
+00005c20: 696e 6465 7820 3d20 5b27 5f5f 6d65 616e  index = ['__mean
+00005c30: 272c 2027 5f5f 7374 6427 5d29 2e54 0d0a  ', '__std']).T..
+00005c40: 2020 2020 2020 2020 7574 696c 732e 7361          utils.sa
+00005c50: 7665 5f64 665f 746f 5f6e 707a 2869 6e70  ve_df_to_npz(inp
+00005c60: 7574 5f74 706d 5f73 7461 7473 2c20 636e  ut_tpm_stats, cn
+00005c70: 6d66 5f6f 626a 2e70 6174 6873 5b27 7470  mf_obj.paths['tp
+00005c80: 6d5f 7374 6174 7327 5d29 0d0a 2020 2020  m_stats'])..    
+00005c90: 2020 2020 6f76 6572 6469 7370 6572 7365      overdisperse
+00005ca0: 645f 6765 6e65 7320 3d20 7365 6c66 2e61  d_genes = self.a
+00005cb0: 6461 7461 2e76 6172 5b22 7365 6c65 6374  data.var["select
+00005cc0: 6564 225d 5b73 656c 662e 6164 6174 612e  ed"][self.adata.
+00005cd0: 7661 725b 2273 656c 6563 7465 6422 5d5d  var["selected"]]
+00005ce0: 2e69 6e64 6578 0d0a 2020 2020 2020 2020  .index..        
+00005cf0: 6e6f 726d 5f63 6f75 6e74 7320 3d20 636e  norm_counts = cn
+00005d00: 6d66 5f6f 626a 2e67 6574 5f6e 6f72 6d5f  mf_obj.get_norm_
+00005d10: 636f 756e 7473 2873 656c 662e 6164 6174  counts(self.adat
+00005d20: 612c 2074 706d 2c20 6869 6768 5f76 6172  a, tpm, high_var
+00005d30: 6961 6e63 655f 6765 6e65 735f 6669 6c74  iance_genes_filt
+00005d40: 6572 3d6f 7665 7264 6973 7065 7273 6564  er=overdispersed
+00005d50: 5f67 656e 6573 290d 0a20 2020 2020 2020  _genes)..       
+00005d60: 2069 6620 6e6f 726d 5f63 6f75 6e74 732e   if norm_counts.
+00005d70: 582e 6474 7970 6520 213d 206e 702e 666c  X.dtype != np.fl
+00005d80: 6f61 7436 343a 0d0a 2020 2020 2020 2020  oat64:..        
+00005d90: 2020 2020 6e6f 726d 5f63 6f75 6e74 732e      norm_counts.
+00005da0: 5820 3d20 6e6f 726d 5f63 6f75 6e74 732e  X = norm_counts.
+00005db0: 582e 6173 7479 7065 286e 702e 666c 6f61  X.astype(np.floa
+00005dc0: 7436 3429 0d0a 2020 2020 2020 2020 636e  t64)..        cn
+00005dd0: 6d66 5f6f 626a 2e73 6176 655f 6e6f 726d  mf_obj.save_norm
+00005de0: 5f63 6f75 6e74 7328 6e6f 726d 5f63 6f75  _counts(norm_cou
+00005df0: 6e74 7329 0d0a 0d0a 2020 2020 2020 2020  nts)....        
+00005e00: 2320 7361 7665 2070 6172 616d 6574 6572  # save parameter
+00005e10: 7320 666f 7220 6661 6374 6f72 697a 6174  s for factorizat
+00005e20: 696f 6e20 7374 6570 0d0a 2020 2020 2020  ion step..      
+00005e30: 2020 636e 6d66 5f6f 626a 2e73 6176 655f    cnmf_obj.save_
+00005e40: 6e6d 665f 6974 6572 5f70 6172 616d 7328  nmf_iter_params(
+00005e50: 2a63 6e6d 665f 6f62 6a2e 6765 745f 6e6d  *cnmf_obj.get_nm
+00005e60: 665f 6974 6572 5f70 6172 616d 7328 6b73  f_iter_params(ks
+00005e70: 3d6b 7661 6c73 2c20 6e5f 6974 6572 3d6e  =kvals, n_iter=n
+00005e80: 5f69 7465 722c 2072 616e 646f 6d5f 7374  _iter, random_st
+00005e90: 6174 655f 7365 6564 3d73 6565 642c 2062  ate_seed=seed, b
+00005ea0: 6574 615f 6c6f 7373 3d62 6574 615f 6c6f  eta_loss=beta_lo
+00005eb0: 7373 2929 0d0a 0d0a 2020 2020 2020 2020  ss))....        
+00005ec0: 2320 7361 7665 2070 6172 616d 6574 6572  # save parameter
+00005ed0: 7320 696e 2041 6e6e 4461 7461 206f 626a  s in AnnData obj
+00005ee0: 6563 740d 0a20 2020 2020 2020 2073 656c  ect..        sel
+00005ef0: 662e 6164 6174 612e 756e 735b 2263 6e6d  f.adata.uns["cnm
+00005f00: 6622 5d20 3d20 636e 6d66 5f6f 626a 2e67  f"] = cnmf_obj.g
+00005f10: 6574 5f6e 6d66 5f69 7465 725f 7061 7261  et_nmf_iter_para
+00005f20: 6d73 286b 733d 6b76 616c 732c 206e 5f69  ms(ks=kvals, n_i
+00005f30: 7465 723d 6e5f 6974 6572 2c20 7261 6e64  ter=n_iter, rand
+00005f40: 6f6d 5f73 7461 7465 5f73 6565 643d 7365  om_state_seed=se
+00005f50: 6564 2c20 6265 7461 5f6c 6f73 733d 6265  ed, beta_loss=be
+00005f60: 7461 5f6c 6f73 7329 5b31 5d20 2023 2064  ta_loss)[1]  # d
+00005f70: 6963 7420 6f66 2063 6e6d 6620 7061 7261  ict of cnmf para
+00005f80: 6d65 7465 7273 0d0a 2020 2020 2020 2020  meters..        
+00005f90: 0d0a 2020 2020 2020 2020 7365 6c66 2e61  ..        self.a
+00005fa0: 7070 656e 645f 746f 5f68 6973 746f 7279  ppend_to_history
+00005fb0: 2866 2263 4e4d 4620 7061 7261 6d65 7465  (f"cNMF paramete
+00005fc0: 7273 2061 6464 6564 2e20 634e 4d46 2069  rs added. cNMF i
+00005fd0: 6e70 7574 7320 696e 6974 6961 6c69 7a65  nputs initialize
+00005fe0: 6420 696e 207b 636e 6d66 5f6f 7574 7075  d in {cnmf_outpu
+00005ff0: 745f 6469 727d 2f7b 636e 6d66 5f6e 616d  t_dir}/{cnmf_nam
+00006000: 657d 2229 0d0a 2020 2020 2020 2020 7265  e}")..        re
+00006010: 7475 726e 2063 6e6d 665f 6f62 6a0d 0a20  turn cnmf_obj.. 
+00006020: 2020 200d 0a20 2020 2064 6566 2061 6464     ..    def add
+00006030: 5f63 6e6d 665f 7265 7375 6c74 7328 7365  _cnmf_results(se
+00006040: 6c66 2c20 636e 6d66 5f6f 7574 7075 745f  lf, cnmf_output_
+00006050: 6469 722c 2063 6e6d 665f 6e61 6d65 2c20  dir, cnmf_name, 
+00006060: 6c6f 6361 6c5f 6465 6e73 6974 795f 7468  local_density_th
+00006070: 7265 7368 6f6c 643a 2066 6c6f 6174 203d  reshold: float =
+00006080: 204e 6f6e 652c 206c 6f63 616c 5f6e 6569   None, local_nei
+00006090: 6768 626f 7268 6f6f 645f 7369 7a65 3a20  ghborhood_size: 
+000060a0: 666c 6f61 7420 3d20 4e6f 6e65 293a 0d0a  float = None):..
+000060b0: 2020 2020 2020 2020 2222 220d 0a20 2020          """..   
+000060c0: 2020 2020 2041 6674 6572 2066 6163 746f       After facto
+000060d0: 7269 7a61 7469 6f6e 2c20 6164 6420 636f  rization, add co
+000060e0: 6d70 6c65 7465 6420 634e 4d46 2072 6573  mpleted cNMF res
+000060f0: 756c 7473 2069 6e20 5b63 6e6d 665f 6f75  ults in [cnmf_ou
+00006100: 7470 7574 5f64 6972 5d2f 5b63 6e6d 665f  tput_dir]/[cnmf_
+00006110: 6e61 6d65 5d20 746f 2074 6865 2064 6174  name] to the dat
+00006120: 6173 6574 206f 626a 6563 742e 0d0a 0d0a  aset object.....
+00006130: 2020 2020 2020 2020 3a70 6172 616d 2063          :param c
+00006140: 6e6d 665f 6f75 7470 7574 5f64 6972 3a20  nmf_output_dir: 
+00006150: 4f75 7470 7574 2064 6972 6563 746f 7279  Output directory
+00006160: 2066 6f72 2063 4e4d 4620 7265 7375 6c74   for cNMF result
+00006170: 730d 0a20 2020 2020 2020 203a 7479 7065  s..        :type
+00006180: 2063 6e6d 665f 6f75 7470 7574 5f64 6972   cnmf_output_dir
+00006190: 3a20 7374 720d 0a20 2020 2020 2020 203a  : str..        :
+000061a0: 7061 7261 6d20 636e 6d66 5f6e 616d 653a  param cnmf_name:
+000061b0: 204e 616d 6520 6f66 2074 6865 2063 4e4d   Name of the cNM
+000061c0: 4620 7265 7375 6c74 732e 2046 696c 6573  F results. Files
+000061d0: 2077 696c 6c20 6265 206f 7574 7075 7420   will be output 
+000061e0: 746f 205b 636e 6d66 5f6f 7574 7075 745f  to [cnmf_output_
+000061f0: 6469 725d 2f5b 636e 6d66 5f6e 616d 655d  dir]/[cnmf_name]
+00006200: 2f0d 0a20 2020 2020 2020 203a 7479 7065  /..        :type
+00006210: 2063 6e6d 665f 6e61 6d65 3a20 7374 720d   cnmf_name: str.
+00006220: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+00006230: 6c6f 6361 6c5f 6465 6e73 6974 795f 7468  local_density_th
+00006240: 7265 7368 6f6c 643a 2054 6872 6573 686f  reshold: Thresho
+00006250: 6c64 2066 6f72 2074 6865 206c 6f63 616c  ld for the local
+00006260: 2064 656e 7369 7479 2066 696c 7465 7269   density filteri
+00006270: 6e67 2070 7269 6f72 2074 6f20 4745 5020  ng prior to GEP 
+00006280: 636f 6e73 656e 7375 732e 2041 6363 6570  consensus. Accep
+00006290: 7461 626c 6520 7468 7265 7368 6f6c 6473  table thresholds
+000062a0: 2061 7265 203e 2030 2061 6e64 203c 3d20   are > 0 and <= 
+000062b0: 3220 2832 2e30 2069 7320 6e6f 2066 696c  2 (2.0 is no fil
+000062c0: 7465 7269 6e67 292e 2044 6566 6175 6c74  tering). Default
+000062d0: 7320 746f 204e 6f6e 652e 0d0a 2020 2020  s to None...    
+000062e0: 2020 2020 3a74 7970 6520 6c6f 6361 6c5f      :type local_
+000062f0: 6465 6e73 6974 795f 7468 7265 7368 6f6c  density_threshol
+00006300: 643a 2066 6c6f 6174 2c20 6f70 7469 6f6e  d: float, option
+00006310: 616c 0d0a 2020 2020 2020 2020 3a70 6172  al..        :par
+00006320: 616d 206c 6f63 616c 5f6e 6569 6768 626f  am local_neighbo
+00006330: 7268 6f6f 645f 7369 7a65 3a20 4672 6163  rhood_size: Frac
+00006340: 7469 6f6e 206f 6620 7468 6520 6e75 6d62  tion of the numb
+00006350: 6572 206f 6620 7265 706c 6963 6174 6573  er of replicates
+00006360: 2074 6f20 7573 6520 6173 206e 6561 7265   to use as neare
+00006370: 7374 206e 6569 6768 626f 7273 2066 6f72  st neighbors for
+00006380: 206c 6f63 616c 2064 656e 7369 7479 2066   local density f
+00006390: 696c 7465 7269 6e67 2e20 4465 6661 756c  iltering. Defaul
+000063a0: 7473 2074 6f20 4e6f 6e65 0d0a 2020 2020  ts to None..    
+000063b0: 2020 2020 3a74 7970 6520 6c6f 6361 6c5f      :type local_
+000063c0: 6e65 6967 6862 6f72 686f 6f64 5f73 697a  neighborhood_siz
+000063d0: 653a 2066 6c6f 6174 2c20 6f70 7469 6f6e  e: float, option
+000063e0: 616c 0d0a 2020 2020 2020 2020 2222 220d  al..        """.
+000063f0: 0a20 2020 2020 2020 2073 656c 662e 6164  .        self.ad
+00006400: 6174 612e 756e 735b 2263 6e6d 665f 6e61  ata.uns["cnmf_na
+00006410: 6d65 225d 203d 2063 6e6d 665f 6e61 6d65  me"] = cnmf_name
+00006420: 0d0a 0d0a 2020 2020 2020 2020 2320 696e  ....        # in
+00006430: 6665 7220 6672 6f6d 2066 696c 656e 616d  fer from filenam
+00006440: 6573 2077 6869 6368 206c 6f63 616c 2064  es which local d
+00006450: 656e 7369 7479 2074 6872 6573 686f 6c64  ensity threshold
+00006460: 2077 6173 2075 7365 640d 0a20 2020 2020   was used..     
+00006470: 2020 2073 656e 7365 645f 6c64 7473 203d     sensed_ldts =
+00006480: 2073 6574 2829 0d0a 2020 2020 2020 2020   set()..        
+00006490: 666f 7220 666e 2069 6e20 676c 6f62 286f  for fn in glob(o
+000064a0: 732e 7061 7468 2e6a 6f69 6e28 636e 6d66  s.path.join(cnmf
+000064b0: 5f6f 7574 7075 745f 6469 722c 2063 6e6d  _output_dir, cnm
+000064c0: 665f 6e61 6d65 2c20 6622 7b63 6e6d 665f  f_name, f"{cnmf_
+000064d0: 6e61 6d65 7d2a 2e2a 7370 6563 7472 612a  name}*.*spectra*
+000064e0: 2e6b 5f2a 2229 293a 0d0a 2020 2020 2020  .k_*")):..      
+000064f0: 2020 2020 2020 6c64 745f 7374 7220 3d20        ldt_str = 
+00006500: 6f73 2e70 6174 682e 6261 7365 6e61 6d65  os.path.basename
+00006510: 2866 6e29 2e73 706c 6974 2822 2e22 295b  (fn).split(".")[
+00006520: 2d33 5d0d 0a20 2020 2020 2020 2020 2020  -3]..           
+00006530: 2074 7279 3a0d 0a20 2020 2020 2020 2020   try:..         
+00006540: 2020 2020 2020 206c 6474 203d 2066 6c6f         ldt = flo
+00006550: 6174 286c 6474 5f73 7472 2e72 6570 6c61  at(ldt_str.repla
+00006560: 6365 2822 6474 5f22 2c20 2222 292e 7265  ce("dt_", "").re
+00006570: 706c 6163 6528 225f 222c 2022 2e22 2929  place("_", "."))
+00006580: 0d0a 2020 2020 2020 2020 2020 2020 6578  ..            ex
+00006590: 6365 7074 2056 616c 7565 4572 726f 723a  cept ValueError:
+000065a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000065b0: 2020 7061 7373 0d0a 2020 2020 2020 2020    pass..        
+000065c0: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
+000065d0: 2020 2020 2020 2020 2020 2073 656e 7365             sense
+000065e0: 645f 6c64 7473 2e61 6464 2828 6c64 745f  d_ldts.add((ldt_
+000065f0: 7374 722c 206c 6474 2929 0d0a 2020 2020  str, ldt))..    
+00006600: 2020 2020 6966 206c 6f63 616c 5f64 656e      if local_den
+00006610: 7369 7479 5f74 6872 6573 686f 6c64 2069  sity_threshold i
+00006620: 7320 4e6f 6e65 2061 6e64 206c 656e 2873  s None and len(s
+00006630: 656e 7365 645f 6c64 7473 2920 3d3d 2031  ensed_ldts) == 1
+00006640: 3a0d 0a20 2020 2020 2020 2020 2020 206c  :..            l
+00006650: 6474 5f73 7472 2c20 6c64 7420 3d20 7365  dt_str, ldt = se
+00006660: 6e73 6564 5f6c 6474 732e 706f 7028 290d  nsed_ldts.pop().
+00006670: 0a20 2020 2020 2020 2065 6c69 6620 6c6f  .        elif lo
+00006680: 6361 6c5f 6465 6e73 6974 795f 7468 7265  cal_density_thre
+00006690: 7368 6f6c 6420 696e 2028 6c64 745b 315d  shold in (ldt[1]
+000066a0: 2066 6f72 206c 6474 2069 6e20 7365 6e73   for ldt in sens
+000066b0: 6564 5f6c 6474 7329 3a0d 0a20 2020 2020  ed_ldts):..     
+000066c0: 2020 2020 2020 206c 6474 5f73 7472 2c20         ldt_str, 
+000066d0: 6c64 7420 3d20 5b28 6c64 745f 7374 722c  ldt = [(ldt_str,
+000066e0: 206c 6474 2920 666f 7220 6c64 745f 7374   ldt) for ldt_st
+000066f0: 722c 206c 6474 2069 6e20 7365 6e73 6564  r, ldt in sensed
+00006700: 5f6c 6474 7320 6966 206c 6474 203d 3d20  _ldts if ldt == 
+00006710: 6c6f 6361 6c5f 6465 6e73 6974 795f 7468  local_density_th
+00006720: 7265 7368 6f6c 645d 2e70 6f70 2829 0d0a  reshold].pop()..
+00006730: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
+00006740: 2020 2020 2020 2020 2020 2072 6169 7365             raise
+00006750: 2052 756e 7469 6d65 4572 726f 7228 6622   RuntimeError(f"
+00006760: 6c6f 6361 6c5f 6465 6e73 6974 795f 7468  local_density_th
+00006770: 7265 7368 6f6c 6420 6f66 207b 6c6f 6361  reshold of {loca
+00006780: 6c5f 6465 6e73 6974 795f 7468 7265 7368  l_density_thresh
+00006790: 6f6c 647d 2064 6f65 7320 6e6f 7420 6d61  old} does not ma
+000067a0: 7463 6820 7768 6174 2069 7320 696e 2074  tch what is in t
+000067b0: 6865 2063 4e4d 4620 7265 7375 6c74 2064  he cNMF result d
+000067c0: 6972 6563 746f 7279 3a20 7b73 656e 7365  irectory: {sense
+000067d0: 645f 6c64 7473 7d22 290d 0a20 2020 2020  d_ldts}")..     
+000067e0: 2020 2073 656c 662e 6164 6174 612e 756e     self.adata.un
+000067f0: 735b 226c 6474 225d 203d 206c 6474 0d0a  s["ldt"] = ldt..
+00006800: 2020 2020 2020 2020 7365 6c66 2e61 6461          self.ada
+00006810: 7461 2e75 6e73 5b22 6c6e 7322 5d20 3d20  ta.uns["lns"] = 
+00006820: 6c6f 6361 6c5f 6e65 6967 6862 6f72 686f  local_neighborho
+00006830: 6f64 5f73 697a 650d 0a20 2020 2020 2020  od_size..       
+00006840: 2020 2020 200d 0a20 2020 2020 2020 2023       ..        #
+00006850: 2049 6d70 6f72 7420 4745 5073 0d0a 2020   Import GEPs..  
+00006860: 2020 2020 2020 7265 7375 6c74 5f74 7970        result_typ
+00006870: 6573 203d 207b 0d0a 2020 2020 2020 2020  es = {..        
+00006880: 2020 2020 2267 656e 655f 7370 6563 7472      "gene_spectr
+00006890: 615f 7363 6f72 6522 3a20 2263 6e6d 665f  a_score": "cnmf_
+000068a0: 6765 705f 7363 6f72 6522 2c0d 0a20 2020  gep_score",..   
+000068b0: 2020 2020 2020 2020 2022 6765 6e65 5f73           "gene_s
+000068c0: 7065 6374 7261 5f74 706d 223a 2022 636e  pectra_tpm": "cn
+000068d0: 6d66 5f67 6570 5f74 706d 222c 0d0a 2020  mf_gep_tpm",..  
+000068e0: 2020 2020 2020 2020 2020 2273 7065 6374            "spect
+000068f0: 7261 223a 2022 636e 6d66 5f67 6570 5f72  ra": "cnmf_gep_r
+00006900: 6177 220d 0a20 2020 2020 2020 2020 2020  aw"..           
+00006910: 207d 0d0a 2020 2020 2020 2020 666f 7220   }..        for 
+00006920: 6d61 7463 6873 7472 2c20 7265 7375 6c74  matchstr, result
+00006930: 5f74 7970 6520 696e 2072 6573 756c 745f  _type in result_
+00006940: 7479 7065 732e 6974 656d 7328 293a 0d0a  types.items():..
+00006950: 2020 2020 2020 2020 2020 2020 6c6f 6767              logg
+00006960: 696e 672e 696e 666f 2866 2249 6d70 6f72  ing.info(f"Impor
+00006970: 7469 6e67 2047 4550 733a 207b 6d61 7463  ting GEPs: {matc
+00006980: 6873 7472 7d22 2920 200d 0a20 2020 2020  hstr}")  ..     
+00006990: 2020 2020 2020 206d 6574 615f 7720 3d20         meta_w = 
+000069a0: 5b5d 0d0a 2020 2020 2020 2020 2020 2020  []..            
+000069b0: 666f 7220 666e 2069 6e20 676c 6f62 286f  for fn in glob(o
+000069c0: 732e 7061 7468 2e6a 6f69 6e28 636e 6d66  s.path.join(cnmf
+000069d0: 5f6f 7574 7075 745f 6469 722c 2063 6e6d  _output_dir, cnm
+000069e0: 665f 6e61 6d65 2c20 6622 7b63 6e6d 665f  f_name, f"{cnmf_
+000069f0: 6e61 6d65 7d2a 2e7b 6d61 7463 6873 7472  name}*.{matchstr
+00006a00: 7d2e 6b5f 2a2e 7b6c 6474 5f73 7472 7d2e  }.k_*.{ldt_str}.
+00006a10: 2a74 7874 2229 293a 0d0a 2020 2020 2020  *txt")):..      
+00006a20: 2020 2020 2020 2020 2020 6b20 3d20 696e            k = in
+00006a30: 7428 6f73 2e70 6174 682e 6261 7365 6e61  t(os.path.basena
+00006a40: 6d65 2866 6e29 2e72 656d 6f76 6570 7265  me(fn).removepre
+00006a50: 6669 7828 6622 7b63 6e6d 665f 6e61 6d65  fix(f"{cnmf_name
+00006a60: 7d2e 7b6d 6174 6368 7374 727d 2e22 292e  }.{matchstr}.").
+00006a70: 7370 6c69 7428 222e 2229 5b30 5d2e 7265  split(".")[0].re
+00006a80: 706c 6163 6528 226b 5f22 2c20 2222 2929  place("k_", ""))
+00006a90: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00006aa0: 2020 7720 3d20 7064 2e72 6561 645f 7461    w = pd.read_ta
+00006ab0: 626c 6528 666e 2c20 696e 6465 785f 636f  ble(fn, index_co
+00006ac0: 6c3d 3029 0d0a 2020 2020 2020 2020 2020  l=0)..          
+00006ad0: 2020 2020 2020 772e 696e 6465 7820 3d20        w.index = 
+00006ae0: 7374 7228 6b29 202b 2022 2e22 202b 2077  str(k) + "." + w
+00006af0: 2e69 6e64 6578 2e61 7374 7970 6528 7374  .index.astype(st
+00006b00: 7229 0d0a 2020 2020 2020 2020 2020 2020  r)..            
+00006b10: 2020 2020 6d65 7461 5f77 2e61 7070 656e      meta_w.appen
+00006b20: 6428 7729 0d0a 2020 2020 2020 2020 2020  d(w)..          
+00006b30: 2020 6d65 7461 5f77 203d 2070 642e 636f    meta_w = pd.co
+00006b40: 6e63 6174 286d 6574 615f 772c 2061 7869  ncat(meta_w, axi
+00006b50: 733d 3029 2e54 2e72 6569 6e64 6578 2873  s=0).T.reindex(s
+00006b60: 656c 662e 6164 6174 612e 7661 722e 696e  elf.adata.var.in
+00006b70: 6465 7829 2e72 656e 616d 655f 6178 6973  dex).rename_axis
+00006b80: 285b 226b 2e67 6570 225d 2c20 6178 6973  (["k.gep"], axis
+00006b90: 3d31 290d 0a20 2020 2020 2020 2020 2020  =1)..           
+00006ba0: 2073 656c 662e 6164 6174 612e 7661 726d   self.adata.varm
+00006bb0: 5b72 6573 756c 745f 7479 7065 5d20 3d20  [result_type] = 
+00006bc0: 6d65 7461 5f77 0d0a 0d0a 2020 2020 2020  meta_w....      
+00006bd0: 2020 2320 496d 706f 7274 2055 7361 6765    # Import Usage
+00006be0: 730d 0a20 2020 2020 2020 206c 6f67 6769  s..        loggi
+00006bf0: 6e67 2e69 6e66 6f28 6622 496d 706f 7274  ng.info(f"Import
+00006c00: 696e 6720 5573 6167 6573 2229 2020 0d0a  ing Usages")  ..
+00006c10: 2020 2020 2020 2020 7573 6167 6520 3d20          usage = 
+00006c20: 5b5d 0d0a 2020 2020 2020 2020 666f 7220  []..        for 
+00006c30: 666e 2069 6e20 676c 6f62 286f 732e 7061  fn in glob(os.pa
+00006c40: 7468 2e6a 6f69 6e28 636e 6d66 5f6f 7574  th.join(cnmf_out
+00006c50: 7075 745f 6469 722c 2063 6e6d 665f 6e61  put_dir, cnmf_na
+00006c60: 6d65 2c20 6622 7b63 6e6d 665f 6e61 6d65  me, f"{cnmf_name
+00006c70: 7d2a 2e75 7361 6765 732e 6b5f 2a2e 7b6c  }*.usages.k_*.{l
+00006c80: 6474 5f73 7472 7d2e 2a74 7874 2229 293a  dt_str}.*txt")):
+00006c90: 0d0a 2020 2020 2020 2020 2020 2020 6b20  ..            k 
+00006ca0: 3d20 696e 7428 6f73 2e70 6174 682e 6261  = int(os.path.ba
+00006cb0: 7365 6e61 6d65 2866 6e29 2e72 656d 6f76  sename(fn).remov
+00006cc0: 6570 7265 6669 7828 6622 7b63 6e6d 665f  eprefix(f"{cnmf_
+00006cd0: 6e61 6d65 7d2e 7573 6167 6573 2e22 292e  name}.usages.").
+00006ce0: 7370 6c69 7428 222e 2229 5b30 5d2e 7265  split(".")[0].re
+00006cf0: 706c 6163 6528 226b 5f22 2c20 2222 2929  place("k_", ""))
+00006d00: 0d0a 2020 2020 2020 2020 2020 2020 6820  ..            h 
+00006d10: 3d20 7064 2e72 6561 645f 7461 626c 6528  = pd.read_table(
+00006d20: 666e 2c20 696e 6465 785f 636f 6c3d 3029  fn, index_col=0)
+00006d30: 0d0a 2020 2020 2020 2020 2020 2020 682e  ..            h.
+00006d40: 636f 6c75 6d6e 7320 3d20 7374 7228 6b29  columns = str(k)
+00006d50: 202b 2022 2e22 202b 2068 2e63 6f6c 756d   + "." + h.colum
+00006d60: 6e73 2e61 7374 7970 6528 7374 7229 0d0a  ns.astype(str)..
+00006d70: 2020 2020 2020 2020 2020 2020 7573 6167              usag
+00006d80: 652e 6170 7065 6e64 2868 290d 0a20 2020  e.append(h)..   
+00006d90: 2020 2020 2073 656c 662e 6164 6174 612e       self.adata.
+00006da0: 6f62 736d 5b22 636e 6d66 5f75 7361 6765  obsm["cnmf_usage
+00006db0: 225d 203d 2070 642e 636f 6e63 6174 2875  "] = pd.concat(u
+00006dc0: 7361 6765 2c20 6178 6973 3d31 292e 736f  sage, axis=1).so
+00006dd0: 7274 5f69 6e64 6578 2861 7869 733d 3129  rt_index(axis=1)
+00006de0: 2e72 656e 616d 655f 6178 6973 285b 226b  .rename_axis(["k
+00006df0: 2e67 6570 225d 2c20 6178 6973 3d31 290d  .gep"], axis=1).
+00006e00: 0a20 2020 2020 2020 200d 0a20 2020 2020  .        ..     
+00006e10: 2020 2023 2049 6d70 6f72 7420 6765 6e65     # Import gene
+00006e20: 206c 6973 7420 7573 6564 2066 6f72 2066   list used for f
+00006e30: 6163 746f 7269 7a61 7469 6f6e 0d0a 2020  actorization..  
+00006e40: 2020 2020 2020 7769 7468 206f 7065 6e28        with open(
+00006e50: 6f73 2e70 6174 682e 6a6f 696e 2863 6e6d  os.path.join(cnm
+00006e60: 665f 6f75 7470 7574 5f64 6972 2c20 636e  f_output_dir, cn
+00006e70: 6d66 5f6e 616d 652c 2066 227b 636e 6d66  mf_name, f"{cnmf
+00006e80: 5f6e 616d 657d 2e6f 7665 7264 6973 7065  _name}.overdispe
+00006e90: 7273 6564 5f67 656e 6573 2e74 7874 2229  rsed_genes.txt")
+00006ea0: 2920 6173 2066 3a0d 0a20 2020 2020 2020  ) as f:..       
+00006eb0: 2020 2020 2073 656c 662e 6164 6174 612e       self.adata.
+00006ec0: 756e 735b 2267 656e 655f 6c69 7374 225d  uns["gene_list"]
+00006ed0: 203d 205b 6c69 6e65 2e73 7472 6970 2829   = [line.strip()
+00006ee0: 2066 6f72 206c 696e 6520 696e 2066 2e72   for line in f.r
+00006ef0: 6561 646c 696e 6573 2829 5d0d 0a0d 0a20  eadlines()].... 
+00006f00: 2020 2020 2020 2023 2049 6d70 6f72 7420         # Import 
+00006f10: 4b2d 7365 6c65 6374 696f 6e20 7374 6174  K-selection stat
+00006f20: 730d 0a20 2020 2020 2020 206b 7661 6c73  s..        kvals
+00006f30: 203d 2070 642e 4461 7461 4672 616d 6528   = pd.DataFrame(
+00006f40: 2a2a 6e70 2e6c 6f61 6428 6f73 2e70 6174  **np.load(os.pat
+00006f50: 682e 6a6f 696e 2863 6e6d 665f 6f75 7470  h.join(cnmf_outp
+00006f60: 7574 5f64 6972 2c20 636e 6d66 5f6e 616d  ut_dir, cnmf_nam
+00006f70: 652c 2066 227b 636e 6d66 5f6e 616d 657d  e, f"{cnmf_name}
+00006f80: 2e6b 5f73 656c 6563 7469 6f6e 5f73 7461  .k_selection_sta
+00006f90: 7473 2e64 662e 6e70 7a22 292c 2061 6c6c  ts.df.npz"), all
+00006fa0: 6f77 5f70 6963 6b6c 653d 5472 7565 2929  ow_pickle=True))
+00006fb0: 2e73 6574 5f69 6e64 6578 2822 6b22 295b  .set_index("k")[
+00006fc0: 5b22 7374 6162 696c 6974 7922 2c20 2270  ["stability", "p
+00006fd0: 7265 6469 6374 696f 6e5f 6572 726f 7222  rediction_error"
+00006fe0: 5d5d 0d0a 2020 2020 2020 2020 6b76 616c  ]]..        kval
+00006ff0: 732e 696e 6465 7820 3d20 6b76 616c 732e  s.index = kvals.
+00007000: 696e 6465 782e 6173 7479 7065 2869 6e74  index.astype(int
+00007010: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+00007020: 6164 6174 612e 756e 735b 226b 7661 6c73  adata.uns["kvals
+00007030: 225d 203d 206b 7661 6c73 0d0a 2020 2020  "] = kvals..    
+00007040: 2020 2020 7365 6c66 2e61 7070 656e 645f      self.append_
+00007050: 746f 5f68 6973 746f 7279 2822 634e 4d46  to_history("cNMF
+00007060: 2072 6573 756c 7473 2061 6464 6564 2066   results added f
+00007070: 726f 6d20 6f75 7470 7574 2064 6972 6563  rom output direc
+00007080: 746f 7279 207b 636e 6d66 5f6f 7574 7075  tory {cnmf_outpu
+00007090: 745f 6469 727d 2f7b 636e 6d66 5f6e 616d  t_dir}/{cnmf_nam
+000070a0: 657d 2229 0d0a 0d0a 2020 2020 6465 6620  e}")....    def 
+000070b0: 7265 6d6f 7665 5f63 6e6d 665f 7265 7375  remove_cnmf_resu
+000070c0: 6c74 7328 7365 6c66 293a 0d0a 2020 2020  lts(self):..    
+000070d0: 2020 2020 666f 7220 7265 7375 6c74 5f74      for result_t
+000070e0: 7970 6520 696e 2028 2263 6e6d 665f 6765  ype in ("cnmf_ge
+000070f0: 705f 7363 6f72 6522 2c20 2263 6e6d 665f  p_score", "cnmf_
+00007100: 6765 705f 7470 6d22 2c20 2263 6e6d 665f  gep_tpm", "cnmf_
+00007110: 6765 705f 7261 7722 293a 0d0a 2020 2020  gep_raw"):..    
+00007120: 2020 2020 2020 2020 7365 6c66 2e61 6461          self.ada
+00007130: 7461 2e76 6172 6d2e 706f 7028 7265 7375  ta.varm.pop(resu
+00007140: 6c74 5f74 7970 6529 0d0a 2020 2020 2020  lt_type)..      
+00007150: 2020 7365 6c66 2e61 6461 7461 2e6f 6273    self.adata.obs
+00007160: 6d2e 706f 7028 2263 6e6d 665f 7573 6167  m.pop("cnmf_usag
+00007170: 6522 290d 0a20 2020 2020 2020 2073 656c  e")..        sel
+00007180: 662e 6164 6174 612e 756e 732e 706f 7028  f.adata.uns.pop(
+00007190: 2267 656e 655f 6c69 7374 2229 0d0a 2020  "gene_list")..  
+000071a0: 2020 2020 2020 7365 6c66 2e61 6461 7461        self.adata
+000071b0: 2e75 6e73 2e70 6f70 2822 6b76 616c 7322  .uns.pop("kvals"
+000071c0: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+000071d0: 6170 7065 6e64 5f74 6f5f 6869 7374 6f72  append_to_histor
+000071e0: 7928 2263 4e4d 4620 7265 7375 6c74 7320  y("cNMF results 
+000071f0: 7265 6d6f 7665 642e 2229 0d0a 0d0a 0d0a  removed.")......
+00007200: 2020 2020 6465 6620 6765 745f 7573 6167      def get_usag
+00007210: 6573 2873 656c 662c 0d0a 2020 2020 2020  es(self,..      
+00007220: 2020 2020 2020 2020 2020 2020 206b 3a20               k: 
+00007230: 556e 696f 6e5b 696e 742c 2049 7465 7261  Union[int, Itera
+00007240: 626c 655d 203d 204e 6f6e 652c 0d0a 2020  ble] = None,..  
+00007250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007260: 2064 6973 6372 6574 697a 653a 2062 6f6f   discretize: boo
+00007270: 6c20 3d20 4661 6c73 652c 0d0a 2020 2020  l = False,..    
+00007280: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+00007290: 6f72 6d61 6c69 7a65 3a20 626f 6f6c 203d  ormalize: bool =
+000072a0: 2046 616c 7365 0d0a 2020 2020 2020 2020   False..        
+000072b0: 2020 2020 2020 2020 2020 2029 202d 3e20             ) -> 
+000072c0: 7064 2e44 6174 6146 7261 6d65 3a0d 0a20  pd.DataFrame:.. 
+000072d0: 2020 2020 2020 2022 2222 0d0a 2020 2020         """..    
+000072e0: 2020 2020 4361 6c63 756c 6174 6520 7573      Calculate us
+000072f0: 6167 6520 6f66 2065 6163 6820 4745 5020  age of each GEP 
+00007300: 696e 2065 6163 6820 7361 6d70 6c65 2f6f  in each sample/o
+00007310: 6273 6572 7661 7469 6f6e 2e0d 0a0d 0a20  bservation..... 
+00007320: 2020 2020 2020 203a 7061 7261 6d20 6b3a         :param k:
+00007330: 2049 6620 616e 2069 6e74 6567 6572 206f   If an integer o
+00007340: 7220 6c69 7374 206f 6620 696e 7465 6765  r list of intege
+00007350: 7273 2c20 7265 7475 726e 7320 7573 6167  rs, returns usag
+00007360: 6573 206f 6e6c 7920 666f 7220 7370 6563  es only for spec
+00007370: 6966 6965 6420 7261 6e6b 732e 204f 7468  ified ranks. Oth
+00007380: 6572 7769 7365 2c20 7265 7475 726e 7320  erwise, returns 
+00007390: 7573 6167 6520 6f66 2061 6c6c 2047 4550  usage of all GEP
+000073a0: 7320 6163 726f 7373 2072 616e 6b73 2e20  s across ranks. 
+000073b0: 4465 6661 756c 7473 2074 6f20 4e6f 6e65  Defaults to None
+000073c0: 0d0a 2020 2020 2020 2020 3a74 7970 6520  ..        :type 
+000073d0: 6b3a 2069 6e74 2c20 6f70 7469 6f6e 616c  k: int, optional
+000073e0: 0d0a 2020 2020 2020 2020 3a70 6172 616d  ..        :param
+000073f0: 2064 6973 6372 6574 697a 653a 2044 6973   discretize: Dis
+00007400: 6372 6574 697a 6573 2074 6865 2075 7361  cretizes the usa
+00007410: 6765 206d 6174 7269 7820 7375 6368 2074  ge matrix such t
+00007420: 6861 7420 666f 7220 6561 6368 2076 616c  hat for each val
+00007430: 7565 206f 6620 6b2c 2065 6163 6820 7361  ue of k, each sa
+00007440: 6d70 6c65 2068 6173 2075 7361 6765 206f  mple has usage o
+00007450: 6620 6f6e 6c79 2031 2047 4550 2028 7468  f only 1 GEP (th
+00007460: 6520 6f6e 6520 7769 7468 2074 6865 206d  e one with the m
+00007470: 6178 696d 756d 2075 7361 6765 292e 2044  aximum usage). D
+00007480: 6566 6175 6c74 7320 746f 2046 616c 7365  efaults to False
+00007490: 0d0a 2020 2020 2020 2020 3a74 7970 6520  ..        :type 
+000074a0: 6469 7363 7265 7469 7a65 3a20 626f 6f6c  discretize: bool
+000074b0: 2c20 6f70 7469 6f6e 616c 0d0a 2020 2020  , optional..    
+000074c0: 2020 2020 3a70 6172 616d 206e 6f72 6d61      :param norma
+000074d0: 6c69 7a65 3a20 4e6f 726d 616c 697a 6520  lize: Normalize 
+000074e0: 7468 6520 4745 5020 7573 6167 6520 6d61  the GEP usage ma
+000074f0: 7472 6978 2073 7563 6820 7468 6174 2066  trix such that f
+00007500: 6f72 2065 6163 6820 7661 6c75 6520 6f66  or each value of
+00007510: 206b 2c20 7573 6167 6520 6f66 2061 6c6c   k, usage of all
+00007520: 2047 4550 7320 7375 6d73 2074 6f20 312e   GEPs sums to 1.
+00007530: 2044 6566 6175 6c74 7320 746f 2046 616c   Defaults to Fal
+00007540: 7365 0d0a 2020 2020 2020 2020 3a74 7970  se..        :typ
+00007550: 6520 6e6f 726d 616c 697a 653a 2062 6f6f  e normalize: boo
+00007560: 6c2c 206f 7074 696f 6e61 6c0d 0a20 2020  l, optional..   
+00007570: 2020 2020 203a 7265 7475 726e 3a20 6f62       :return: ob
+00007580: 7365 7276 6174 696f 6e20 c397 2047 4550  servation .. GEP
+00007590: 206d 6174 7269 780d 0a20 2020 2020 2020   matrix..       
+000075a0: 203a 7274 7970 653a 2070 642e 4461 7461   :rtype: pd.Data
+000075b0: 4672 616d 650d 0a20 2020 2020 2020 2022  Frame..        "
+000075c0: 2222 0d0a 2020 2020 2020 2020 6466 203d  ""..        df =
+000075d0: 2073 656c 662e 6164 6174 612e 6f62 736d   self.adata.obsm
+000075e0: 5b22 636e 6d66 5f75 7361 6765 225d 2e63  ["cnmf_usage"].c
+000075f0: 6f70 7928 290d 0a20 2020 2020 2020 2064  opy()..        d
+00007600: 662e 636f 6c75 6d6e 7320 3d20 7064 2e4d  f.columns = pd.M
+00007610: 756c 7469 496e 6465 782e 6672 6f6d 5f74  ultiIndex.from_t
+00007620: 7570 6c65 7328 6466 2e63 6f6c 756d 6e73  uples(df.columns
+00007630: 2e73 7472 2e73 706c 6974 2822 2e22 292e  .str.split(".").
+00007640: 746f 5f6c 6973 7428 2929 0d0a 2020 2020  to_list())..    
+00007650: 2020 2020 6466 2e63 6f6c 756d 6e73 203d      df.columns =
+00007660: 2064 662e 636f 6c75 6d6e 732e 7365 745f   df.columns.set_
+00007670: 6c65 7665 6c73 285b 6c2e 6173 7479 7065  levels([l.astype
+00007680: 2822 696e 7422 2920 666f 7220 6c20 696e  ("int") for l in
+00007690: 2064 662e 636f 6c75 6d6e 732e 6c65 7665   df.columns.leve
+000076a0: 6c73 5d29 0d0a 2020 2020 2020 2020 6966  ls])..        if
+000076b0: 206e 6f72 6d61 6c69 7a65 3a0d 0a20 2020   normalize:..   
+000076c0: 2020 2020 2020 2020 206e 6f72 6d61 6c69           normali
+000076d0: 7a65 6420 3d20 5b5d 0d0a 2020 2020 2020  zed = []..      
+000076e0: 2020 2020 2020 666f 7220 5f2c 2073 7562        for _, sub
+000076f0: 6466 2069 6e20 6466 2e67 726f 7570 6279  df in df.groupby
+00007700: 2861 7869 733d 312c 206c 6576 656c 3d30  (axis=1, level=0
+00007710: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+00007720: 2020 2020 6e6f 726d 616c 697a 6564 2e61      normalized.a
+00007730: 7070 656e 6428 7375 6264 662e 6469 7628  ppend(subdf.div(
+00007740: 7375 6264 662e 7375 6d28 6178 6973 3d31  subdf.sum(axis=1
+00007750: 292c 2061 7869 733d 3029 290d 0a20 2020  ), axis=0))..   
+00007760: 2020 2020 2020 2020 2064 6620 3d20 7064           df = pd
+00007770: 2e63 6f6e 6361 7428 6e6f 726d 616c 697a  .concat(normaliz
+00007780: 6564 2c20 6178 6973 3d31 290d 0a20 2020  ed, axis=1)..   
+00007790: 2020 2020 2069 6620 6469 7363 7265 7469       if discreti
+000077a0: 7a65 3a0d 0a20 2020 2020 2020 2020 2020  ze:..           
+000077b0: 2064 6973 6372 6574 697a 6564 203d 205b   discretized = [
+000077c0: 5d0d 0a20 2020 2020 2020 2020 2020 2066  ]..            f
+000077d0: 6f72 205f 2c20 7375 6264 6620 696e 2064  or _, subdf in d
+000077e0: 662e 6772 6f75 7062 7928 6178 6973 3d31  f.groupby(axis=1
+000077f0: 2c20 6c65 7665 6c3d 3029 3a0d 0a20 2020  , level=0):..   
+00007800: 2020 2020 2020 2020 2020 2020 2064 6973               dis
+00007810: 6372 6574 697a 6564 2e61 7070 656e 6428  cretized.append(
+00007820: 7375 6264 662e 6571 2873 7562 6466 2e6d  subdf.eq(subdf.m
+00007830: 6178 2861 7869 733d 3129 2c20 6178 6973  ax(axis=1), axis
+00007840: 3d30 292e 6173 7479 7065 2869 6e74 2929  =0).astype(int))
+00007850: 0d0a 2020 2020 2020 2020 2020 2020 6466  ..            df
+00007860: 203d 2070 642e 636f 6e63 6174 2864 6973   = pd.concat(dis
+00007870: 6372 6574 697a 6564 2c20 6178 6973 3d31  cretized, axis=1
+00007880: 2920 2020 2020 2020 200d 0a20 2020 2020  )        ..     
+00007890: 2020 2069 6620 6b20 6973 206e 6f74 204e     if k is not N
+000078a0: 6f6e 653a 0d0a 2020 2020 2020 2020 2020  one:..          
+000078b0: 2020 6466 203d 2064 662e 6c6f 635b 3a2c    df = df.loc[:,
+000078c0: 206b 5d0d 0a20 2020 2020 2020 2064 6620   k]..        df 
+000078d0: 3d20 6466 2e73 6f72 745f 696e 6465 7828  = df.sort_index(
+000078e0: 6178 6973 3d30 292e 736f 7274 5f69 6e64  axis=0).sort_ind
+000078f0: 6578 2861 7869 733d 3129 2020 200d 0a20  ex(axis=1)   .. 
+00007900: 2020 2020 2020 2072 6574 7572 6e20 6466         return df
+00007910: 0d0a 2020 2020 0d0a 2020 2020 6465 6620  ..    ..    def 
+00007920: 6765 745f 6765 7073 2873 656c 662c 0d0a  get_geps(self,..
+00007930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007940: 206b 3a20 556e 696f 6e5b 696e 742c 2049   k: Union[int, I
+00007950: 7465 7261 626c 655d 203d 204e 6f6e 652c  terable] = None,
+00007960: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00007970: 2020 2074 7970 653d 2263 6e6d 665f 6765     type="cnmf_ge
+00007980: 705f 7363 6f72 6522 0d0a 2020 2020 2020  p_score"..      
+00007990: 2020 2020 2020 2020 2020 2029 202d 3e20             ) -> 
+000079a0: 7064 2e44 6174 6146 7261 6d65 3a0d 0a20  pd.DataFrame:.. 
+000079b0: 2020 2020 2020 2022 2222 0d0a 2020 2020         """..    
+000079c0: 2020 2020 4765 7420 4745 5073 2e0d 0a0d      Get GEPs....
+000079d0: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+000079e0: 6b3a 2049 6620 616e 2069 6e74 6567 6572  k: If an integer
+000079f0: 206f 7220 6c69 7374 206f 6620 696e 7465   or list of inte
+00007a00: 6765 7273 2c20 7265 7475 726e 7320 4745  gers, returns GE
+00007a10: 5073 206f 6e6c 7920 666f 7220 7370 6563  Ps only for spec
+00007a20: 6966 6965 6420 7261 6e6b 732e 204f 7468  ified ranks. Oth
+00007a30: 6572 7769 7365 2c20 7265 7475 726e 7320  erwise, returns 
+00007a40: 4745 5073 2066 726f 6d20 616c 6c20 7261  GEPs from all ra
+00007a50: 6e6b 732e 2044 6566 6175 6c74 7320 746f  nks. Defaults to
+00007a60: 204e 6f6e 650d 0a20 2020 2020 2020 203a   None..        :
+00007a70: 7479 7065 206b 3a20 556e 696f 6e5b 696e  type k: Union[in
+00007a80: 742c 2049 7465 7261 626c 655d 2c20 6f70  t, Iterable], op
+00007a90: 7469 6f6e 616c 0d0a 2020 2020 2020 2020  tional..        
+00007aa0: 3a70 6172 616d 2074 7970 653a 2022 636e  :param type: "cn
+00007ab0: 6d66 5f67 6570 5f73 636f 7265 2220 6f72  mf_gep_score" or
+00007ac0: 2022 636e 6d66 5f67 6570 5f74 706d 222c   "cnmf_gep_tpm",
+00007ad0: 2064 6566 6175 6c74 7320 746f 2022 636e   defaults to "cn
+00007ae0: 6d66 5f67 6570 5f73 636f 7265 220d 0a20  mf_gep_score".. 
+00007af0: 2020 2020 2020 203a 7479 7065 2074 7970         :type typ
+00007b00: 653a 2073 7472 2c20 6f70 7469 6f6e 616c  e: str, optional
+00007b10: 0d0a 2020 2020 2020 2020 3a72 6574 7572  ..        :retur
+00007b20: 6e3a 2066 6561 7475 7265 7320 c397 2047  n: features .. G
+00007b30: 4550 206d 6174 7269 780d 0a20 2020 2020  EP matrix..     
+00007b40: 2020 203a 7274 7970 653a 2070 642e 4461     :rtype: pd.Da
+00007b50: 7461 4672 616d 650d 0a20 2020 2020 2020  taFrame..       
+00007b60: 2022 2222 0d0a 2020 2020 2020 2020 6466   """..        df
+00007b70: 203d 2073 656c 662e 6164 6174 612e 7661   = self.adata.va
+00007b80: 726d 5b74 7970 655d 2e63 6f70 7928 290d  rm[type].copy().
+00007b90: 0a20 2020 2020 2020 2064 662e 636f 6c75  .        df.colu
+00007ba0: 6d6e 7320 3d20 7064 2e4d 756c 7469 496e  mns = pd.MultiIn
+00007bb0: 6465 782e 6672 6f6d 5f74 7570 6c65 7328  dex.from_tuples(
+00007bc0: 6466 2e63 6f6c 756d 6e73 2e73 7472 2e73  df.columns.str.s
+00007bd0: 706c 6974 2822 2e22 292e 746f 5f6c 6973  plit(".").to_lis
+00007be0: 7428 2929 0d0a 2020 2020 2020 2020 6466  t())..        df
+00007bf0: 2e63 6f6c 756d 6e73 203d 2064 662e 636f  .columns = df.co
+00007c00: 6c75 6d6e 732e 7365 745f 6c65 7665 6c73  lumns.set_levels
+00007c10: 285b 6c2e 6173 7479 7065 2822 696e 7422  ([l.astype("int"
+00007c20: 2920 666f 7220 6c20 696e 2064 662e 636f  ) for l in df.co
+00007c30: 6c75 6d6e 732e 6c65 7665 6c73 5d29 0d0a  lumns.levels])..
+00007c40: 2020 2020 2020 2020 6966 2069 7369 6e73          if isins
+00007c50: 7461 6e63 6528 6b2c 2028 696e 742c 2049  tance(k, (int, I
+00007c60: 7465 7261 626c 6529 293a 0d0a 2020 2020  terable)):..    
+00007c70: 2020 2020 2020 2020 6466 203d 2064 662e          df = df.
+00007c80: 6c6f 635b 3a2c 206b 5d0d 0a20 2020 2020  loc[:, k]..     
+00007c90: 2020 2064 6620 3d20 6466 2e73 6f72 745f     df = df.sort_
+00007ca0: 696e 6465 7828 6178 6973 3d31 290d 0a20  index(axis=1).. 
+00007cb0: 2020 2020 2020 2072 6574 7572 6e20 6466         return df
+00007cc0: 0d0a 2020 2020 0d0a 2020 2020 6465 6620  ..    ..    def 
+00007cd0: 6765 745f 6d65 7461 6461 7461 5f64 6628  get_metadata_df(
+00007ce0: 7365 6c66 2c0d 0a20 2020 2020 2020 2020  self,..         
+00007cf0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00007d00: 6e63 6c75 6465 5f63 6174 6567 6f72 6963  nclude_categoric
+00007d10: 616c 3a20 626f 6f6c 203d 2054 7275 652c  al: bool = True,
+00007d20: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00007d30: 2020 2020 2020 2020 2020 696e 636c 7564            includ
+00007d40: 655f 6e75 6d65 7269 6361 6c3a 2062 6f6f  e_numerical: boo
+00007d50: 6c20 3d20 5472 7565 0d0a 2020 2020 2020  l = True..      
+00007d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007d70: 2020 2920 2d3e 2070 642e 4461 7461 4672    ) -> pd.DataFr
+00007d80: 616d 653a 0d0a 2020 2020 2020 2020 2222  ame:..        ""
+00007d90: 2247 6574 2073 616d 706c 652f 6f62 7365  "Get sample/obse
+00007da0: 7276 6174 696f 6e20 6d65 7461 6461 7461  rvation metadata
+00007db0: 2e0d 0a0d 0a20 2020 2020 2020 203a 7061  .....        :pa
+00007dc0: 7261 6d20 696e 636c 7564 655f 6361 7465  ram include_cate
+00007dd0: 676f 7269 6361 6c3a 2049 6e63 6c75 6465  gorical: Include
+00007de0: 2063 6174 6567 6f72 6963 616c 206d 6574   categorical met
+00007df0: 6164 6174 6120 6c61 7965 7273 2c20 6465  adata layers, de
+00007e00: 6661 756c 7473 2074 6f20 5472 7565 0d0a  faults to True..
+00007e10: 2020 2020 2020 2020 3a74 7970 6520 696e          :type in
+00007e20: 636c 7564 655f 6361 7465 676f 7269 6361  clude_categorica
+00007e30: 6c3a 2062 6f6f 6c2c 206f 7074 696f 6e61  l: bool, optiona
+00007e40: 6c0d 0a20 2020 2020 2020 203a 7061 7261  l..        :para
+00007e50: 6d20 696e 636c 7564 655f 6e75 6d65 7269  m include_numeri
+00007e60: 6361 6c3a 2049 6e63 6c75 6465 206e 756d  cal: Include num
+00007e70: 6572 6963 616c 206d 6574 6164 6174 6120  erical metadata 
+00007e80: 6c61 7965 7273 2c20 6465 6661 756c 7473  layers, defaults
+00007e90: 2074 6f20 5472 7565 0d0a 2020 2020 2020   to True..      
+00007ea0: 2020 3a74 7970 6520 696e 636c 7564 655f    :type include_
+00007eb0: 6e75 6d65 7269 6361 6c3a 2062 6f6f 6c2c  numerical: bool,
+00007ec0: 206f 7074 696f 6e61 6c0d 0a20 2020 2020   optional..     
+00007ed0: 2020 203a 7261 6973 6573 2056 616c 7565     :raises Value
+00007ee0: 4572 726f 723a 2045 7272 6f72 2069 6620  Error: Error if 
+00007ef0: 6d65 7461 6461 7461 2074 7970 6573 2061  metadata types a
+00007f00: 7265 206e 6f74 2072 6563 6f67 6e69 7a65  re not recognize
+00007f10: 640d 0a20 2020 2020 2020 203a 7265 7475  d..        :retu
+00007f20: 726e 3a20 6f62 7365 7276 6174 696f 6e73  rn: observations
+00007f30: 20c3 9720 6d65 7461 6461 7461 206d 6174   .. metadata mat
+00007f40: 7269 780d 0a20 2020 2020 2020 203a 7274  rix..        :rt
+00007f50: 7970 653a 2070 642e 4461 7461 4672 616d  ype: pd.DataFram
+00007f60: 650d 0a20 2020 2020 2020 2022 2222 0d0a  e..        """..
+00007f70: 2020 2020 2020 2020 6474 7970 6573 203d          dtypes =
+00007f80: 205b 5d0d 0a20 2020 2020 2020 2069 6620   []..        if 
+00007f90: 696e 636c 7564 655f 6361 7465 676f 7269  include_categori
+00007fa0: 6361 6c3a 0d0a 2020 2020 2020 2020 2020  cal:..          
+00007fb0: 2020 6474 7970 6573 2e61 7070 656e 6428    dtypes.append(
+00007fc0: 2263 6174 6567 6f72 7922 290d 0a20 2020  "category")..   
+00007fd0: 2020 2020 2069 6620 696e 636c 7564 655f       if include_
+00007fe0: 6e75 6d65 7269 6361 6c3a 0d0a 2020 2020  numerical:..    
+00007ff0: 2020 2020 2020 2020 6474 7970 6573 202b          dtypes +
+00008000: 3d20 5b22 666c 6f61 7422 2c20 2269 6e74  = ["float", "int
+00008010: 225d 0d0a 2020 2020 2020 2020 756e 6578  "]..        unex
+00008020: 706c 6169 6e65 645f 636f 6c73 203d 2073  plained_cols = s
+00008030: 656c 662e 6164 6174 612e 6f62 732e 7365  elf.adata.obs.se
+00008040: 6c65 6374 5f64 7479 7065 7328 6578 636c  lect_dtypes(excl
+00008050: 7564 653d 2822 6361 7465 676f 7279 222c  ude=("category",
+00008060: 2022 666c 6f61 7422 2c20 2269 6e74 2229   "float", "int")
+00008070: 292e 636f 6c75 6d6e 730d 0a20 2020 2020  ).columns..     
+00008080: 2020 2069 6620 6c65 6e28 756e 6578 706c     if len(unexpl
+00008090: 6169 6e65 645f 636f 6c73 2920 3e20 303a  ained_cols) > 0:
+000080a0: 0d0a 2020 2020 2020 2020 2020 2020 756e  ..            un
+000080b0: 6578 706c 6169 6e65 645f 636f 6c5f 7374  explained_col_st
+000080c0: 7220 3d20 222c 2022 2e6a 6f69 6e28 756e  r = ", ".join(un
+000080d0: 6578 706c 6169 6e65 645f 636f 6c73 290d  explained_cols).
+000080e0: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
+000080f0: 7365 2056 616c 7565 4572 726f 7228 6622  se ValueError(f"
+00008100: 7b75 6e65 7870 6c61 696e 6564 5f63 6f6c  {unexplained_col
+00008110: 5f73 7472 7d20 6d65 7461 6461 7461 2063  _str} metadata c
+00008120: 6f6c 756d 6e73 2068 6176 6520 756e 7265  olumns have unre
+00008130: 636f 676e 697a 6564 2064 7479 7065 732e  cognized dtypes.
+00008140: 2229 0d0a 2020 2020 2020 2020 6466 203d  ")..        df =
+00008150: 2073 656c 662e 6164 6174 612e 6f62 732e   self.adata.obs.
+00008160: 7365 6c65 6374 5f64 7479 7065 7328 696e  select_dtypes(in
+00008170: 636c 7564 653d 6474 7970 6573 290d 0a20  clude=dtypes).. 
+00008180: 2020 2020 2020 2064 6620 3d20 6466 2e64         df = df.d
+00008190: 726f 706e 6128 6178 6973 3d31 2c20 686f  ropna(axis=1, ho
+000081a0: 773d 2261 6c6c 2229 0d0a 2020 2020 2020  w="all")..      
+000081b0: 2020 7265 7475 726e 2064 660d 0a20 2020    return df..   
+000081c0: 200d 0a20 2020 2064 6566 2067 6574 5f63   ..    def get_c
+000081d0: 6174 6567 6f72 795f 6f76 6572 7265 7072  ategory_overrepr
+000081e0: 6573 656e 7461 7469 6f6e 2873 656c 662c  esentation(self,
+000081f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00008200: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008210: 2020 2020 2020 2020 2020 6c61 7965 723a            layer:
+00008220: 2073 7472 2c0d 0a20 2020 2020 2020 2020   str,..         
 00008230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008240: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-00008250: 202d 3e20 7064 2e44 6174 6146 7261 6d65   -> pd.DataFrame
-00008260: 3a0d 0a20 2020 2020 2020 2022 2222 4361  :..        """Ca
-00008270: 6c63 756c 6174 6520 5065 6172 736f 6e20  lculate Pearson 
-00008280: 7265 7369 6475 616c 206f 6620 6368 692d  residual of chi-
-00008290: 7371 7561 7265 6420 7465 7374 2c20 6173  squared test, as
-000082a0: 736f 6369 6174 696e 6720 4745 5073 2066  sociating GEPs f
-000082b0: 6f72 2065 6163 6820 7261 6e6b 2028 6b29  or each rank (k)
-000082c0: 2074 6f20 6361 7465 676f 7269 6573 206f   to categories o
-000082d0: 6620 7361 6d70 6c65 732f 6f62 7365 7276  f samples/observ
-000082e0: 6174 696f 6e73 2e20 4279 2064 6566 6175  ations. By defau
-000082f0: 6c74 2c20 7472 756e 6361 7465 7320 6e65  lt, truncates ne
-00008300: 6761 7469 7665 2076 616c 7565 732e 0d0a  gative values...
-00008310: 0d0a 2020 2020 2020 2020 3a70 6172 616d  ..        :param
-00008320: 206c 6179 6572 3a20 6e61 6d65 206f 6620   layer: name of 
-00008330: 6361 7465 676f 7269 6361 6c20 6461 7461  categorical data
-00008340: 206c 6179 6572 0d0a 2020 2020 2020 2020   layer..        
-00008350: 3a74 7970 6520 6c61 7965 723a 2073 7472  :type layer: str
-00008360: 0d0a 2020 2020 2020 2020 3a70 6172 616d  ..        :param
-00008370: 2074 7275 6e63 6174 655f 6e65 6761 7469   truncate_negati
-00008380: 7665 3a20 5472 756e 6361 7465 206e 6567  ve: Truncate neg
-00008390: 6174 6976 6520 7265 7369 6475 616c 7320  ative residuals 
-000083a0: 746f 2030 2c20 6465 6661 756c 7473 2074  to 0, defaults t
-000083b0: 6f20 5472 7565 0d0a 2020 2020 2020 2020  o True..        
-000083c0: 3a74 7970 6520 7472 756e 6361 7465 5f6e  :type truncate_n
-000083d0: 6567 6174 6976 653a 2062 6f6f 6c2c 206f  egative: bool, o
-000083e0: 7074 696f 6e61 6c0d 0a20 2020 2020 2020  ptional..       
-000083f0: 203a 7265 7475 726e 3a20 6361 7465 676f   :return: catego
-00008400: 7279 20c3 9720 4745 5020 6d61 7472 6978  ry .. GEP matrix
-00008410: 206f 6620 6f76 6572 7265 7072 6573 656e   of overrepresen
-00008420: 7461 7469 6f6e 2076 616c 7565 730d 0a20  tation values.. 
-00008430: 2020 2020 2020 203a 7274 7970 653a 2070         :rtype: p
-00008440: 642e 4461 7461 4672 616d 650d 0a20 2020  d.DataFrame..   
-00008450: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
-00008460: 2020 7573 6167 6520 3d20 7365 6c66 2e67    usage = self.g
-00008470: 6574 5f75 7361 6765 7328 6e6f 726d 616c  et_usages(normal
-00008480: 697a 653d 5472 7565 292e 636f 7079 2829  ize=True).copy()
-00008490: 0d0a 2020 2020 2020 2020 7361 6d70 6c65  ..        sample
-000084a0: 5f74 6f5f 636c 6173 7320 3d20 7365 6c66  _to_class = self
-000084b0: 2e67 6574 5f6d 6574 6164 6174 615f 6466  .get_metadata_df
-000084c0: 2829 5b6c 6179 6572 5d0d 0a20 2020 2020  ()[layer]..     
-000084d0: 2020 2075 7361 6765 2e69 6e64 6578 203d     usage.index =
-000084e0: 2075 7361 6765 2e69 6e64 6578 2e6d 6170   usage.index.map
-000084f0: 2873 616d 706c 655f 746f 5f63 6c61 7373  (sample_to_class
-00008500: 290d 0a20 2020 2020 2020 206f 6273 6572  )..        obser
-00008510: 7665 6420 3d20 7573 6167 652e 6772 6f75  ved = usage.grou
-00008520: 7062 7928 6178 6973 3d30 2c20 6c65 7665  pby(axis=0, leve
-00008530: 6c3d 3029 2e73 756d 2829 0d0a 0d0a 2020  l=0).sum()....  
-00008540: 2020 2020 2020 6e5f 6361 7465 676f 7269        n_categori
-00008550: 6573 203d 206f 6273 6572 7665 642e 7368  es = observed.sh
-00008560: 6170 655b 305d 0d0a 2020 2020 2020 2020  ape[0]..        
-00008570: 6966 206e 5f63 6174 6567 6f72 6965 7320  if n_categories 
-00008580: 3c20 323a 0d0a 2020 2020 2020 2020 2020  < 2:..          
-00008590: 2020 6c6f 6767 696e 672e 7761 726e 696e    logging.warnin
-000085a0: 6728 6622 4f76 6572 7265 7072 6573 656e  g(f"Overrepresen
-000085b0: 7461 7469 6f6e 2063 6f75 6c64 206e 6f74  tation could not
-000085c0: 2062 6520 6361 6c63 756c 6174 6564 2066   be calculated f
-000085d0: 6f72 206c 6179 6572 2027 7b6c 6179 6572  or layer '{layer
-000085e0: 7d27 2c20 6173 206f 6e6c 7920 7b6e 5f63  }', as only {n_c
-000085f0: 6174 6567 6f72 6965 737d 2063 6174 6567  ategories} categ
-00008600: 6f72 6965 7320 7765 7265 2066 6f75 6e64  ories were found
-00008610: 2069 6e20 7468 6520 6461 7461 2e20 220d   in the data. ".
-00008620: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00008630: 2020 2020 2020 2020 2020 2020 2066 224e               f"N
-00008640: 6f74 6520 7468 6174 2065 6d70 7479 2076  ote that empty v
-00008650: 616c 7565 7320 696e 2074 6865 206d 6574  alues in the met
-00008660: 6164 6174 6120 6172 6520 6e6f 7420 636f  adata are not co
-00008670: 6e73 6964 6572 6564 2061 2063 6174 6567  nsidered a categ
-00008680: 6f72 792e 2022 0d0a 2020 2020 2020 2020  ory. "..        
-00008690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000086a0: 2020 2020 6622 4f76 6572 7265 7072 6573      f"Overrepres
-000086b0: 656e 7461 7469 6f6e 2063 616e 6e6f 7420  entation cannot 
-000086c0: 6265 2063 616c 6375 6c61 7465 6420 7769  be calculated wi
-000086d0: 7468 2066 6577 6572 2074 6861 6e20 3220  th fewer than 2 
-000086e0: 6361 7465 676f 7269 6573 2066 6f72 2065  categories for e
-000086f0: 6163 6820 6c61 7965 722e 2022 290d 0a20  ach layer. ").. 
-00008700: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00008710: 6e20 7064 2e44 6174 6146 7261 6d65 286e  n pd.DataFrame(n
-00008720: 702e 4e61 4e2c 2069 6e64 6578 203d 206f  p.NaN, index = o
-00008730: 6273 6572 7665 642e 696e 6465 782c 2063  bserved.index, c
-00008740: 6f6c 756d 6e73 3d6f 6273 6572 7665 642e  olumns=observed.
-00008750: 636f 6c75 6d6e 7329 0d0a 2020 2020 2020  columns)..      
-00008760: 2020 6578 7065 6374 6564 203d 205b 5d0d    expected = [].
-00008770: 0a20 2020 2020 2020 2066 6f72 206b 2c20  .        for k, 
-00008780: 6f62 735f 6b20 696e 206f 6273 6572 7665  obs_k in observe
-00008790: 642e 6772 6f75 7062 7928 6178 6973 3d31  d.groupby(axis=1
-000087a0: 2c20 6c65 7665 6c3d 3129 3a0d 0a20 2020  , level=1):..   
-000087b0: 2020 2020 2020 2020 2065 7870 5f6b 203d           exp_k =
-000087c0: 2070 642e 4461 7461 4672 616d 6528 6f62   pd.DataFrame(ob
-000087d0: 735f 6b2e 7375 6d28 6178 6973 3d31 2929  s_k.sum(axis=1))
-000087e0: 2040 2070 642e 4461 7461 4672 616d 6528   @ pd.DataFrame(
-000087f0: 6f62 735f 6b2e 7375 6d28 6178 6973 3d30  obs_k.sum(axis=0
-00008800: 2929 2e54 202f 206f 6273 5f6b 2e73 756d  )).T / obs_k.sum
-00008810: 2829 2e73 756d 2829 0d0a 2020 2020 2020  ().sum()..      
-00008820: 2020 2020 2020 6578 7065 6374 6564 2e61        expected.a
-00008830: 7070 656e 6428 6578 705f 6b29 0d0a 2020  ppend(exp_k)..  
-00008840: 2020 2020 2020 6578 7065 6374 6564 203d        expected =
-00008850: 2070 642e 636f 6e63 6174 2865 7870 6563   pd.concat(expec
-00008860: 7465 642c 2061 7869 733d 3129 0d0a 2020  ted, axis=1)..  
-00008870: 2020 2020 2020 6368 6973 715f 7265 7369        chisq_resi
-00008880: 6420 3d20 286f 6273 6572 7665 6420 2d20  d = (observed - 
-00008890: 6578 7065 6374 6564 2920 2f20 6e70 2e73  expected) / np.s
-000088a0: 7172 7428 6578 7065 6374 6564 2920 2023  qrt(expected)  #
-000088b0: 2070 6561 7273 6f6e 2072 6573 6964 7561   pearson residua
-000088c0: 6c20 6f66 2063 6869 2d73 7175 6172 6564  l of chi-squared
-000088d0: 2074 6573 7420 6f66 2063 6f6e 7469 6e67   test of conting
-000088e0: 656e 6379 2074 6162 6c65 0d0a 2020 2020  ency table..    
-000088f0: 2020 2020 6966 2074 7275 6e63 6174 655f      if truncate_
-00008900: 6e65 6761 7469 7665 3a0d 0a20 2020 2020  negative:..     
-00008910: 2020 2020 2020 2063 6869 7371 5f72 6573         chisq_res
-00008920: 6964 203d 2063 6869 7371 5f72 6573 6964  id = chisq_resid
-00008930: 2e63 6c69 7028 6c6f 7765 723d 3029 0d0a  .clip(lower=0)..
-00008940: 2020 2020 2020 2020 7265 7475 726e 2063          return c
-00008950: 6869 7371 5f72 6573 6964 0d0a 2020 2020  hisq_resid..    
-00008960: 0d0a 2020 2020 2020 2020 0d0a 2020 2020  ..        ..    
-00008970: 6465 6620 6765 745f 6d65 7461 6461 7461  def get_metadata
-00008980: 5f63 6f72 7265 6c61 7469 6f6e 2873 656c  _correlation(sel
-00008990: 662c 200d 0a20 2020 2020 2020 2020 2020  f, ..           
-000089a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000089b0: 2020 2020 2020 6c61 7965 723a 2073 7472        layer: str
-000089c0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-000089d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000089e0: 2020 2020 6d65 7468 6f64 3a20 7374 7220      method: str 
-000089f0: 3d20 2270 6561 7273 6f6e 220d 0a20 2020  = "pearson"..   
-00008a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008a10: 2020 2020 2020 2020 2020 2020 2020 2920                ) 
-00008a20: 2d3e 2070 642e 5365 7269 6573 3a0d 0a20  -> pd.Series:.. 
-00008a30: 2020 2020 2020 2022 2222 4361 6c63 756c         """Calcul
-00008a40: 6174 6520 5065 6172 736f 6e20 636f 7272  ate Pearson corr
-00008a50: 656c 6174 696f 6e20 6f66 2047 4550 2075  elation of GEP u
-00008a60: 7361 6765 2074 6f20 6e75 6d65 7269 6361  sage to numerica
-00008a70: 6c20 6d65 7461 6461 7461 2061 6372 6f73  l metadata acros
-00008a80: 7320 7361 6d70 6c65 732f 6f62 7365 7276  s samples/observ
-00008a90: 6174 696f 6e73 2e0d 0a0d 0a20 2020 2020  ations.....     
-00008aa0: 2020 203a 7061 7261 6d20 6c61 7965 723a     :param layer:
-00008ab0: 206e 616d 6520 6f66 206e 756d 6572 6963   name of numeric
-00008ac0: 616c 2064 6174 6120 6c61 7965 720d 0a20  al data layer.. 
-00008ad0: 2020 2020 2020 203a 7479 7065 206c 6179         :type lay
-00008ae0: 6572 3a20 7374 720d 0a20 2020 2020 2020  er: str..       
-00008af0: 203a 7061 7261 6d20 6d65 7468 6f64 3a20   :param method: 
-00008b00: 436f 7272 656c 6174 696f 6e20 6d65 7468  Correlation meth
-00008b10: 6f64 3a20 2270 6561 7273 6f6e 222c 2022  od: "pearson", "
-00008b20: 7370 6561 726d 616e 222c 206f 7220 226b  spearman", or "k
-00008b30: 656e 6461 6c6c 222e 2044 6566 6175 6c74  endall". Default
-00008b40: 7320 746f 2022 7065 6172 736f 6e22 0d0a  s to "pearson"..
-00008b50: 2020 2020 2020 2020 3a74 7970 6520 6d65          :type me
-00008b60: 7468 6f64 3a20 7374 722c 206f 7074 696f  thod: str, optio
-00008b70: 6e61 6c0d 0a20 2020 2020 2020 203a 7265  nal..        :re
-00008b80: 7475 726e 3a20 636f 7272 656c 6174 696f  turn: correlatio
-00008b90: 6e20 6f66 2047 4550 2074 6f20 6d65 7461  n of GEP to meta
-00008ba0: 6461 7461 0d0a 2020 2020 2020 2020 3a72  data..        :r
-00008bb0: 7479 7065 3a20 7064 2e53 6572 6965 730d  type: pd.Series.
-00008bc0: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
-00008bd0: 2020 2020 2020 7573 6167 6520 3d20 7365        usage = se
-00008be0: 6c66 2e67 6574 5f75 7361 6765 7328 292e  lf.get_usages().
-00008bf0: 636f 7079 2829 0d0a 2020 2020 2020 2020  copy()..        
-00008c00: 6d65 7461 6461 7461 203d 2073 656c 662e  metadata = self.
-00008c10: 6765 745f 6d65 7461 6461 7461 5f64 6628  get_metadata_df(
-00008c20: 295b 6c61 7965 725d 0d0a 2020 2020 2020  )[layer]..      
-00008c30: 2020 6d64 5f63 6f72 7220 3d20 7573 6167    md_corr = usag
-00008c40: 652e 636f 7272 7769 7468 286d 6574 6164  e.corrwith(metad
-00008c50: 6174 612c 206d 6574 686f 643d 6d65 7468  ata, method=meth
-00008c60: 6f64 290d 0a20 2020 2020 2020 2072 6574  od)..        ret
-00008c70: 7572 6e20 6d64 5f63 6f72 720d 0a20 2020  urn md_corr..   
-00008c80: 2020 2020 200d 0a20 2020 2064 6566 2061       ..    def a
-00008c90: 7070 656e 645f 746f 5f68 6973 746f 7279  ppend_to_history
-00008ca0: 2873 656c 662c 2065 6e74 7279 293a 0d0a  (self, entry):..
-00008cb0: 2020 2020 2020 2020 2222 2241 6464 2065          """Add e
-00008cc0: 6e74 7279 2074 6f20 4461 7461 7365 7420  ntry to Dataset 
-00008cd0: 6869 7374 6f72 792e 0d0a 0d0a 2020 2020  history.....    
-00008ce0: 2020 2020 3a70 6172 616d 2065 6e74 7279      :param entry
-00008cf0: 3a20 4465 7363 7269 7074 696f 6e20 6f66  : Description of
-00008d00: 2065 7665 6e74 2074 6f20 7265 636f 7264   event to record
-00008d10: 2069 6e20 7468 6520 6869 7374 6f72 792e   in the history.
-00008d20: 0d0a 2020 2020 2020 2020 3a74 7970 6520  ..        :type 
-00008d30: 656e 7472 793a 2073 7472 0d0a 2020 2020  entry: str..    
-00008d40: 2020 2020 2222 220d 0a20 2020 2020 2020      """..       
-00008d50: 2073 656c 662e 6164 6174 612e 756e 735b   self.adata.uns[
-00008d60: 2268 6973 746f 7279 225d 5b64 6174 6574  "history"][datet
-00008d70: 696d 652e 7574 636e 6f77 2829 2e69 736f  ime.utcnow().iso
-00008d80: 666f 726d 6174 2829 5d20 3d20 656e 7472  format()] = entr
-00008d90: 790d 0a20 2020 2020 2020 200d 0a20 2020  y..        ..   
-00008da0: 2064 6566 2067 6574 5f68 6973 746f 7279   def get_history
-00008db0: 2873 656c 6629 3a0d 0a20 2020 2020 2020  (self):..       
-00008dc0: 2022 2222 5265 7475 726e 7320 7469 6d65   """Returns time
-00008dd0: 7374 616d 7065 6420 6869 7374 6f72 7920  stamped history 
-00008de0: 6f66 2044 6174 6173 6574 206f 626a 6563  of Dataset objec
-00008df0: 742e 0d0a 0d0a 2020 2020 2020 2020 3a72  t.....        :r
-00008e00: 6574 7572 6e3a 2068 6973 746f 7279 0d0a  eturn: history..
-00008e10: 2020 2020 2020 2020 3a72 7479 7065 3a20          :rtype: 
-00008e20: 6469 6374 0d0a 2020 2020 2020 2020 2222  dict..        ""
-00008e30: 220d 0a20 2020 2020 2020 2072 6574 7572  "..        retur
-00008e40: 6e20 7365 6c66 2e61 6461 7461 2e75 6e73  n self.adata.uns
-00008e50: 5b22 6869 7374 6f72 7922 5d              ["history"]
+00008240: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+00008250: 7275 6e63 6174 655f 6e65 6761 7469 7665  runcate_negative
+00008260: 3a20 626f 6f6c 203d 2054 7275 650d 0a20  : bool = True.. 
+00008270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008290: 2020 2020 2020 2029 202d 3e20 7064 2e44         ) -> pd.D
+000082a0: 6174 6146 7261 6d65 3a0d 0a20 2020 2020  ataFrame:..     
+000082b0: 2020 2022 2222 4361 6c63 756c 6174 6520     """Calculate 
+000082c0: 5065 6172 736f 6e20 7265 7369 6475 616c  Pearson residual
+000082d0: 206f 6620 6368 692d 7371 7561 7265 6420   of chi-squared 
+000082e0: 7465 7374 2c20 6173 736f 6369 6174 696e  test, associatin
+000082f0: 6720 4745 5073 2066 6f72 2065 6163 6820  g GEPs for each 
+00008300: 7261 6e6b 2028 6b29 2074 6f20 6361 7465  rank (k) to cate
+00008310: 676f 7269 6573 206f 6620 7361 6d70 6c65  gories of sample
+00008320: 732f 6f62 7365 7276 6174 696f 6e73 2e20  s/observations. 
+00008330: 4279 2064 6566 6175 6c74 2c20 7472 756e  By default, trun
+00008340: 6361 7465 7320 6e65 6761 7469 7665 2076  cates negative v
+00008350: 616c 7565 732e 0d0a 0d0a 2020 2020 2020  alues.....      
+00008360: 2020 3a70 6172 616d 206c 6179 6572 3a20    :param layer: 
+00008370: 6e61 6d65 206f 6620 6361 7465 676f 7269  name of categori
+00008380: 6361 6c20 6461 7461 206c 6179 6572 0d0a  cal data layer..
+00008390: 2020 2020 2020 2020 3a74 7970 6520 6c61          :type la
+000083a0: 7965 723a 2073 7472 0d0a 2020 2020 2020  yer: str..      
+000083b0: 2020 3a70 6172 616d 2074 7275 6e63 6174    :param truncat
+000083c0: 655f 6e65 6761 7469 7665 3a20 5472 756e  e_negative: Trun
+000083d0: 6361 7465 206e 6567 6174 6976 6520 7265  cate negative re
+000083e0: 7369 6475 616c 7320 746f 2030 2c20 6465  siduals to 0, de
+000083f0: 6661 756c 7473 2074 6f20 5472 7565 0d0a  faults to True..
+00008400: 2020 2020 2020 2020 3a74 7970 6520 7472          :type tr
+00008410: 756e 6361 7465 5f6e 6567 6174 6976 653a  uncate_negative:
+00008420: 2062 6f6f 6c2c 206f 7074 696f 6e61 6c0d   bool, optional.
+00008430: 0a20 2020 2020 2020 203a 7265 7475 726e  .        :return
+00008440: 3a20 6361 7465 676f 7279 20c3 9720 4745  : category .. GE
+00008450: 5020 6d61 7472 6978 206f 6620 6f76 6572  P matrix of over
+00008460: 7265 7072 6573 656e 7461 7469 6f6e 2076  representation v
+00008470: 616c 7565 730d 0a20 2020 2020 2020 203a  alues..        :
+00008480: 7274 7970 653a 2070 642e 4461 7461 4672  rtype: pd.DataFr
+00008490: 616d 650d 0a20 2020 2020 2020 2022 2222  ame..        """
+000084a0: 0d0a 2020 2020 2020 2020 7573 6167 6520  ..        usage 
+000084b0: 3d20 7365 6c66 2e67 6574 5f75 7361 6765  = self.get_usage
+000084c0: 7328 6e6f 726d 616c 697a 653d 5472 7565  s(normalize=True
+000084d0: 292e 636f 7079 2829 0d0a 2020 2020 2020  ).copy()..      
+000084e0: 2020 7361 6d70 6c65 5f74 6f5f 636c 6173    sample_to_clas
+000084f0: 7320 3d20 7365 6c66 2e67 6574 5f6d 6574  s = self.get_met
+00008500: 6164 6174 615f 6466 2829 5b6c 6179 6572  adata_df()[layer
+00008510: 5d0d 0a20 2020 2020 2020 2075 7361 6765  ]..        usage
+00008520: 2e69 6e64 6578 203d 2075 7361 6765 2e69  .index = usage.i
+00008530: 6e64 6578 2e6d 6170 2873 616d 706c 655f  ndex.map(sample_
+00008540: 746f 5f63 6c61 7373 290d 0a20 2020 2020  to_class)..     
+00008550: 2020 206f 6273 6572 7665 6420 3d20 7573     observed = us
+00008560: 6167 652e 6772 6f75 7062 7928 6178 6973  age.groupby(axis
+00008570: 3d30 2c20 6c65 7665 6c3d 3029 2e73 756d  =0, level=0).sum
+00008580: 2829 0d0a 2020 2020 2020 2020 6f62 7365  ()..        obse
+00008590: 7276 6564 203d 206f 6273 6572 7665 645b  rved = observed[
+000085a0: 6f62 7365 7276 6564 2e73 756d 2861 7869  observed.sum(axi
+000085b0: 733d 3129 203e 2030 5d0d 0a0d 0a20 2020  s=1) > 0]....   
+000085c0: 2020 2020 206e 5f63 6174 6567 6f72 6965       n_categorie
+000085d0: 7320 3d20 6f62 7365 7276 6564 2e73 6861  s = observed.sha
+000085e0: 7065 5b30 5d0d 0a20 2020 2020 2020 2069  pe[0]..        i
+000085f0: 6620 6e5f 6361 7465 676f 7269 6573 203c  f n_categories <
+00008600: 2032 3a0d 0a20 2020 2020 2020 2020 2020   2:..           
+00008610: 206c 6f67 6769 6e67 2e77 6172 6e69 6e67   logging.warning
+00008620: 2866 224f 7665 7272 6570 7265 7365 6e74  (f"Overrepresent
+00008630: 6174 696f 6e20 636f 756c 6420 6e6f 7420  ation could not 
+00008640: 6265 2063 616c 6375 6c61 7465 6420 666f  be calculated fo
+00008650: 7220 6c61 7965 7220 277b 6c61 7965 727d  r layer '{layer}
+00008660: 272c 2061 7320 6f6e 6c79 207b 6e5f 6361  ', as only {n_ca
+00008670: 7465 676f 7269 6573 7d20 6361 7465 676f  tegories} catego
+00008680: 7269 6573 2077 6572 6520 666f 756e 6420  ries were found 
+00008690: 696e 2074 6865 2064 6174 612e 2022 0d0a  in the data. "..
+000086a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000086b0: 2020 2020 2020 2020 2020 2020 6622 4e6f              f"No
+000086c0: 7465 2074 6861 7420 656d 7074 7920 7661  te that empty va
+000086d0: 6c75 6573 2069 6e20 7468 6520 6d65 7461  lues in the meta
+000086e0: 6461 7461 2061 7265 206e 6f74 2063 6f6e  data are not con
+000086f0: 7369 6465 7265 6420 6120 6361 7465 676f  sidered a catego
+00008700: 7279 2e20 220d 0a20 2020 2020 2020 2020  ry. "..         
+00008710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008720: 2020 2066 224f 7665 7272 6570 7265 7365     f"Overreprese
+00008730: 6e74 6174 696f 6e20 6361 6e6e 6f74 2062  ntation cannot b
+00008740: 6520 6361 6c63 756c 6174 6564 2077 6974  e calculated wit
+00008750: 6820 6665 7765 7220 7468 616e 2032 2063  h fewer than 2 c
+00008760: 6174 6567 6f72 6965 7320 666f 7220 6561  ategories for ea
+00008770: 6368 206c 6179 6572 2e20 2229 0d0a 2020  ch layer. ")..  
+00008780: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00008790: 2070 642e 4461 7461 4672 616d 6528 6e70   pd.DataFrame(np
+000087a0: 2e4e 614e 2c20 696e 6465 7820 3d20 6f62  .NaN, index = ob
+000087b0: 7365 7276 6564 2e69 6e64 6578 2c20 636f  served.index, co
+000087c0: 6c75 6d6e 733d 6f62 7365 7276 6564 2e63  lumns=observed.c
+000087d0: 6f6c 756d 6e73 290d 0a20 2020 2020 2020  olumns)..       
+000087e0: 2065 7870 6563 7465 6420 3d20 5b5d 0d0a   expected = []..
+000087f0: 2020 2020 2020 2020 666f 7220 6b2c 206f          for k, o
+00008800: 6273 5f6b 2069 6e20 6f62 7365 7276 6564  bs_k in observed
+00008810: 2e67 726f 7570 6279 2861 7869 733d 312c  .groupby(axis=1,
+00008820: 206c 6576 656c 3d31 293a 0d0a 2020 2020   level=1):..    
+00008830: 2020 2020 2020 2020 6578 705f 6b20 3d20          exp_k = 
+00008840: 7064 2e44 6174 6146 7261 6d65 286f 6273  pd.DataFrame(obs
+00008850: 5f6b 2e73 756d 2861 7869 733d 3129 2920  _k.sum(axis=1)) 
+00008860: 4020 7064 2e44 6174 6146 7261 6d65 286f  @ pd.DataFrame(o
+00008870: 6273 5f6b 2e73 756d 2861 7869 733d 3029  bs_k.sum(axis=0)
+00008880: 292e 5420 2f20 6f62 735f 6b2e 7375 6d28  ).T / obs_k.sum(
+00008890: 292e 7375 6d28 290d 0a20 2020 2020 2020  ).sum()..       
+000088a0: 2020 2020 2065 7870 6563 7465 642e 6170       expected.ap
+000088b0: 7065 6e64 2865 7870 5f6b 290d 0a20 2020  pend(exp_k)..   
+000088c0: 2020 2020 2065 7870 6563 7465 6420 3d20       expected = 
+000088d0: 7064 2e63 6f6e 6361 7428 6578 7065 6374  pd.concat(expect
+000088e0: 6564 2c20 6178 6973 3d31 290d 0a20 2020  ed, axis=1)..   
+000088f0: 2020 2020 2063 6869 7371 5f72 6573 6964       chisq_resid
+00008900: 203d 2028 6f62 7365 7276 6564 202d 2065   = (observed - e
+00008910: 7870 6563 7465 6429 202f 206e 702e 7371  xpected) / np.sq
+00008920: 7274 2865 7870 6563 7465 6429 2020 2320  rt(expected)  # 
+00008930: 7065 6172 736f 6e20 7265 7369 6475 616c  pearson residual
+00008940: 206f 6620 6368 692d 7371 7561 7265 6420   of chi-squared 
+00008950: 7465 7374 206f 6620 636f 6e74 696e 6765  test of continge
+00008960: 6e63 7920 7461 626c 650d 0a20 2020 2020  ncy table..     
+00008970: 2020 2069 6620 7472 756e 6361 7465 5f6e     if truncate_n
+00008980: 6567 6174 6976 653a 0d0a 2020 2020 2020  egative:..      
+00008990: 2020 2020 2020 6368 6973 715f 7265 7369        chisq_resi
+000089a0: 6420 3d20 6368 6973 715f 7265 7369 642e  d = chisq_resid.
+000089b0: 636c 6970 286c 6f77 6572 3d30 290d 0a20  clip(lower=0).. 
+000089c0: 2020 2020 2020 2072 6574 7572 6e20 6368         return ch
+000089d0: 6973 715f 7265 7369 640d 0a20 2020 200d  isq_resid..    .
+000089e0: 0a20 2020 2020 2020 200d 0a20 2020 2064  .        ..    d
+000089f0: 6566 2067 6574 5f6d 6574 6164 6174 615f  ef get_metadata_
+00008a00: 636f 7272 656c 6174 696f 6e28 7365 6c66  correlation(self
+00008a10: 2c20 0d0a 2020 2020 2020 2020 2020 2020  , ..            
+00008a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008a30: 2020 2020 206c 6179 6572 3a20 7374 722c       layer: str,
+00008a40: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00008a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008a60: 2020 206d 6574 686f 643a 2073 7472 203d     method: str =
+00008a70: 2022 7065 6172 736f 6e22 0d0a 2020 2020   "pearson"..    
+00008a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008a90: 2020 2020 2020 2020 2020 2020 2029 202d               ) -
+00008aa0: 3e20 7064 2e53 6572 6965 733a 0d0a 2020  > pd.Series:..  
+00008ab0: 2020 2020 2020 2222 2243 616c 6375 6c61        """Calcula
+00008ac0: 7465 2050 6561 7273 6f6e 2063 6f72 7265  te Pearson corre
+00008ad0: 6c61 7469 6f6e 206f 6620 4745 5020 7573  lation of GEP us
+00008ae0: 6167 6520 746f 206e 756d 6572 6963 616c  age to numerical
+00008af0: 206d 6574 6164 6174 6120 6163 726f 7373   metadata across
+00008b00: 2073 616d 706c 6573 2f6f 6273 6572 7661   samples/observa
+00008b10: 7469 6f6e 732e 0d0a 0d0a 2020 2020 2020  tions.....      
+00008b20: 2020 3a70 6172 616d 206c 6179 6572 3a20    :param layer: 
+00008b30: 6e61 6d65 206f 6620 6e75 6d65 7269 6361  name of numerica
+00008b40: 6c20 6461 7461 206c 6179 6572 0d0a 2020  l data layer..  
+00008b50: 2020 2020 2020 3a74 7970 6520 6c61 7965        :type laye
+00008b60: 723a 2073 7472 0d0a 2020 2020 2020 2020  r: str..        
+00008b70: 3a70 6172 616d 206d 6574 686f 643a 2043  :param method: C
+00008b80: 6f72 7265 6c61 7469 6f6e 206d 6574 686f  orrelation metho
+00008b90: 643a 2022 7065 6172 736f 6e22 2c20 2273  d: "pearson", "s
+00008ba0: 7065 6172 6d61 6e22 2c20 6f72 2022 6b65  pearman", or "ke
+00008bb0: 6e64 616c 6c22 2e20 4465 6661 756c 7473  ndall". Defaults
+00008bc0: 2074 6f20 2270 6561 7273 6f6e 220d 0a20   to "pearson".. 
+00008bd0: 2020 2020 2020 203a 7479 7065 206d 6574         :type met
+00008be0: 686f 643a 2073 7472 2c20 6f70 7469 6f6e  hod: str, option
+00008bf0: 616c 0d0a 2020 2020 2020 2020 3a72 6574  al..        :ret
+00008c00: 7572 6e3a 2063 6f72 7265 6c61 7469 6f6e  urn: correlation
+00008c10: 206f 6620 4745 5020 746f 206d 6574 6164   of GEP to metad
+00008c20: 6174 610d 0a20 2020 2020 2020 203a 7274  ata..        :rt
+00008c30: 7970 653a 2070 642e 5365 7269 6573 0d0a  ype: pd.Series..
+00008c40: 2020 2020 2020 2020 2222 220d 0a20 2020          """..   
+00008c50: 2020 2020 2075 7361 6765 203d 2073 656c       usage = sel
+00008c60: 662e 6765 745f 7573 6167 6573 2829 2e63  f.get_usages().c
+00008c70: 6f70 7928 290d 0a20 2020 2020 2020 206d  opy()..        m
+00008c80: 6574 6164 6174 6120 3d20 7365 6c66 2e67  etadata = self.g
+00008c90: 6574 5f6d 6574 6164 6174 615f 6466 2829  et_metadata_df()
+00008ca0: 5b6c 6179 6572 5d0d 0a20 2020 2020 2020  [layer]..       
+00008cb0: 206d 645f 636f 7272 203d 2075 7361 6765   md_corr = usage
+00008cc0: 2e63 6f72 7277 6974 6828 6d65 7461 6461  .corrwith(metada
+00008cd0: 7461 2c20 6d65 7468 6f64 3d6d 6574 686f  ta, method=metho
+00008ce0: 6429 0d0a 2020 2020 2020 2020 7265 7475  d)..        retu
+00008cf0: 726e 206d 645f 636f 7272 0d0a 2020 2020  rn md_corr..    
+00008d00: 2020 2020 0d0a 2020 2020 6465 6620 6170      ..    def ap
+00008d10: 7065 6e64 5f74 6f5f 6869 7374 6f72 7928  pend_to_history(
+00008d20: 7365 6c66 2c20 656e 7472 7929 3a0d 0a20  self, entry):.. 
+00008d30: 2020 2020 2020 2022 2222 4164 6420 656e         """Add en
+00008d40: 7472 7920 746f 2044 6174 6173 6574 2068  try to Dataset h
+00008d50: 6973 746f 7279 2e0d 0a0d 0a20 2020 2020  istory.....     
+00008d60: 2020 203a 7061 7261 6d20 656e 7472 793a     :param entry:
+00008d70: 2044 6573 6372 6970 7469 6f6e 206f 6620   Description of 
+00008d80: 6576 656e 7420 746f 2072 6563 6f72 6420  event to record 
+00008d90: 696e 2074 6865 2068 6973 746f 7279 2e0d  in the history..
+00008da0: 0a20 2020 2020 2020 203a 7479 7065 2065  .        :type e
+00008db0: 6e74 7279 3a20 7374 720d 0a20 2020 2020  ntry: str..     
+00008dc0: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
+00008dd0: 7365 6c66 2e61 6461 7461 2e75 6e73 5b22  self.adata.uns["
+00008de0: 6869 7374 6f72 7922 5d5b 6461 7465 7469  history"][dateti
+00008df0: 6d65 2e75 7463 6e6f 7728 292e 6973 6f66  me.utcnow().isof
+00008e00: 6f72 6d61 7428 295d 203d 2065 6e74 7279  ormat()] = entry
+00008e10: 0d0a 2020 2020 2020 2020 0d0a 2020 2020  ..        ..    
+00008e20: 6465 6620 6765 745f 6869 7374 6f72 7928  def get_history(
+00008e30: 7365 6c66 293a 0d0a 2020 2020 2020 2020  self):..        
+00008e40: 2222 2252 6574 7572 6e73 2074 696d 6573  """Returns times
+00008e50: 7461 6d70 6564 2068 6973 746f 7279 206f  tamped history o
+00008e60: 6620 4461 7461 7365 7420 6f62 6a65 6374  f Dataset object
+00008e70: 2e0d 0a0d 0a20 2020 2020 2020 203a 7265  .....        :re
+00008e80: 7475 726e 3a20 6869 7374 6f72 790d 0a20  turn: history.. 
+00008e90: 2020 2020 2020 203a 7274 7970 653a 2064         :rtype: d
+00008ea0: 6963 740d 0a20 2020 2020 2020 2022 2222  ict..        """
+00008eb0: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+00008ec0: 2073 656c 662e 6164 6174 612e 756e 735b   self.adata.uns[
+00008ed0: 2268 6973 746f 7279 225d                 "history"]
```

### Comparing `cnmfsns-1.7.0/src/cnmfsns/integration.py` & `cnmfsns-1.7.1/src/cnmfsns/integration.py`

 * *Files identical despite different names*

### Comparing `cnmfsns-1.7.0/src/cnmfsns/plots.py` & `cnmfsns-1.7.1/src/cnmfsns/plots.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 import pandas as pd
 import numpy as np
 import seaborn as sns
 import matplotlib as mpl
 from matplotlib.figure import Figure
 from matplotlib.axes import Axes
 from matplotlib.lines import Line2D
-from matplotlib.patches import Polygon, Rectangle, Patch
+from matplotlib.patches import Polygon, Rectangle, Patch, Arc
 import matplotlib.pyplot as plt
 import upsetplot
 from scipy.cluster.hierarchy import linkage, dendrogram
 import networkx as nx
 
 
 #########################
@@ -341,16 +341,15 @@
                     min_corr = integration.pairwise_thresholds.loc[(dataset_row, dataset_col)]
                     hist_kwargs = {
                         "hue":[("Included" if c else "Excluded") for c in (corr > min_corr)],
                         "palette": {"Included": "red", "Excluded": "gray"},
                         "hue_order": ["Excluded", "Included"]
                     }
                     included_fraction = (corr > min_corr).sum() / corr.shape[0]
-                    ax.text(x=0.01, y=1.08, s=f"AUC = {included_fraction:.3f}", size=8, ha='left', va='bottom', transform=ax.transAxes, color="black")
-                    ax.text(x=0.01, y=1.01, s=f"range = {min_corr:.3f}-{max_corr:.3f}", size=8, ha='left', va='bottom', transform=ax.transAxes, color="red")
+                    ax.text(x=0.01, y=1.01, s=f"AUC = {included_fraction:.3f}\nrange = {min_corr:.3f}-{max_corr:.3f}", size=8, ha='left', va='bottom', transform=ax.transAxes, color="black")
                 else:
                     hist_kwargs = {"color": "gray"}
                 sns.histplot(x=corr, ax=ax,legend=False, bins=bins, linewidth=0, multiple="stack", **hist_kwargs)
 
                 ax.set_ylabel(dataset_row)
                 ax.set_xlabel(dataset_col)
                 ax.set_xlim(-1 - inside_padding, 1 + inside_padding)
@@ -393,16 +392,15 @@
                 sns.histplot(data=corr, x="abscorr", hue="sign", palette= {"Positive": "red", "Negative": "blue"}, bins=bins, alpha=0.4, linewidth=0,
                              hue_order= ["Negative", "Positive"], ax=ax,legend=False)
 
 
                 # show min_corr as text in top left of plot and vertical line
                 min_corr = integration.pairwise_thresholds.loc[(dataset_row, dataset_col)]
                 included_fraction = (corr["corr"] > min_corr).sum() / corr.shape[0]  # could also show the quantile of the min_corr threshold
-                ax.text(x=0.01, y=1.01, s=f"AUC = {included_fraction:.3f}\nrange = {min_corr:.3f}-{max_corr:.3f}",
-                        size=8, ha='left', va='bottom', transform=ax.transAxes, color="black")
+                ax.text(x=0.01, y=1.01, s=f"AUC = {included_fraction:.3f}\nrange = {min_corr:.3f}-{max_corr:.3f}", size=8, ha='left', va='bottom', transform=ax.transAxes, color="black")
                 ax.axvline(min_corr, color="black")
                 ax.set_ylabel(dataset_row)
                 ax.set_xlabel(dataset_col)
                 ax.set_xlim(0 - inside_padding, 1 + inside_padding)
 
     ymax = max([ax.get_ylim()[1] for row in axes for ax in row])
     for row in axes:
@@ -410,43 +408,43 @@
             ax.set_ylim((
                 - ymax * inside_padding,
                 ymax + ymax * inside_padding
             ))
 
     return fig
 
-def plot_overdispersed_features_upset(integration: Integration, figsize: Collection = (6, 4)) -> Figure:
+def plot_overdispersed_features_upset(integration: Integration, figsize: Collection = (6, 4), show_counts: bool = False) -> Figure:
     """Plot overlaps of overdispersed features between datasets
 
     :param integration: integration object
     :type integration: Integration
     :param figsize: width and height of figure, defaults to [6, 4]
     :type figsize: Collection, optional
     :return: figure
     :rtype: Figure
     """
     overdispersed_feature_lists = {dataset_name: dataset.overdispersed_genes for dataset_name, dataset in integration.datasets.items()}
     fig = Figure(figsize=figsize)
-    upsetplot.UpSet(upsetplot.from_contents(overdispersed_feature_lists)).plot(fig=fig)
+    upsetplot.UpSet(upsetplot.from_contents(overdispersed_feature_lists), show_counts=show_counts).plot(fig=fig)
     fig.suptitle("Overdispersed features")
     return fig
 
-def plot_features_upset(integration: Integration, figsize=[6, 4]):
+def plot_features_upset(integration: Integration, figsize=[6, 4], show_counts: bool = False):
     """Plot overlaps of features between datasets
 
     :param integration: integration object
     :type integration: Integration
     :param figsize: width and height of figure, defaults to [6, 4]
     :type figsize: Collection, optional
     :return: figure
     :rtype: Figure
     """
     feature_lists = {dataset_name: list(dataset.adata.var.index) for dataset_name, dataset in integration.datasets.items()}
     fig = Figure(figsize=figsize)
-    upsetplot.UpSet(upsetplot.from_contents(feature_lists)).plot(fig=fig)
+    upsetplot.UpSet(upsetplot.from_contents(feature_lists), show_counts=show_counts).plot(fig=fig)
     fig.suptitle("Features")
     return fig
 
 #####################
 # SNS-related plots #
 #####################
 
@@ -624,20 +622,25 @@
             if draw_labels:
                 a = (previous - np.pi / len(enrichments))
                 x_offset = (size * 1.1) * np.cos(a)
                 y_offset = (size * 1.1) * np.sin(a)
                 ax.text(x+x_offset, y+y_offset, label, rotation=np.rad2deg(a), ha="left", va="center", rotation_mode='anchor', fontsize=label_font_size)
         previous = this
 
-def draw_circle_bar_scale(position, size, ax, scale_factor, label_font_size = 6, linewidth=0.8, rings=[0.2, 0.5, 1]):
+def draw_circle_bar_scale(position, size, ax, scale_factor, label_font_size = 8, linewidth=0.8, rings=[0.2, 0.5, 1]):
     x, y = position
+    max_ring_radius = np.sqrt(np.max(rings)) * size
+    ax.add_line(Line2D([x, x], [y, y+max_ring_radius], color="k", linewidth=linewidth))
+    ax.add_line(Line2D([x, x - 0.5 * max_ring_radius],
+                       [y, y + max_ring_radius * np.cos(np.deg2rad(30))], color="k", linewidth=linewidth))
+
     for ring in rings:
-        ax.add_patch(plt.Circle(position, np.sqrt(ring) * size, color="black", fill=False, linewidth=linewidth))
-    ax.add_patch(Rectangle(position, size * 1.01, size * 1.01, color="#FFFFFF"))
-    ax.scatter(position[0], position[1], s=linewidth*2, color="black", marker=".")
+        arc_diameter = 2 * (np.sqrt(ring) * size)
+        ax.add_patch(Arc(position, width=arc_diameter, height=arc_diameter, angle=0, theta1 = 90, theta2 = 120, linewidth=linewidth))
+    # ax.scatter(position[0], position[1], s=linewidth*2, color="black", marker=".")  # dot at centre of arc
     for ring in rings:
         value = ring/scale_factor
         ax.text(
             x + size * 0.05,
             y + np.sqrt(ring) * size,
             f"{value:.2f}",
             fontsize=label_font_size,
@@ -654,15 +657,14 @@
                                         layer: str,
                                         subset_datasets: Optional[Union[str, Collection[str]]] = None,
                                         ax: Optional[Axes] = None,
                                         pie_size: float = 0.3,
                                         figsize: Collection = (9, 6),
                                         edge_weights: Optional[str] = None,
                                         edge_color: str = "#AAAAAA88",
-                                        metric: str = "pearson_residual",
                                         legend_pie_size: float = 0.1,
                                         show_legend: bool = True) -> Optional[Figure]:
     
     if show_legend:
         assert ax is None
     
     if ax is None:
@@ -682,50 +684,48 @@
     else:
         width = np.array(list(nx.get_edge_attributes(snsmap.gep_graph, edge_weights).values()))
         width = width / np.max(width)
 
     nx.draw_networkx_edges(snsmap.gep_graph, pos=snsmap.layout, edge_color=edge_color, ax=ax_plot, width=width)
     overrepresentation = snsmap.integration.get_category_overrepresentation(subset_datasets=subset_datasets, layer=layer)
     overrepresentation = overrepresentation.fillna(0)
-
     max_or = np.max(overrepresentation.values.flatten())
     if max_or == 0:
         scale_factor = 1
     else:
         scale_factor = 1 / max_or
     
-    
+    color_list = overrepresentation.index.map(colors.get_metadata_colors(layer))
     for gep, gep_or in overrepresentation.items():
         node = "|".join((str(p) for p in gep))
 
         if node in snsmap.gep_graph and gep_or.any():
-            color_list = gep_or.index.map(colors.get_metadata_colors(layer))
             draw_circle_bar_plot(position=snsmap.layout[node],
                                  enrichments=gep_or,
                                  scale_factor=scale_factor,
                                  colors=color_list,
                                  size=pie_size, ax=ax_plot)
 
     if show_legend:
         # Add legends
         draw_circle_bar_plot(
             position=(0, 0.5),
-            enrichments=pd.Series(max_or, index=gep_or.index.sort_values().unique()),
-            colors=overrepresentation.index.map(colors.get_metadata_colors(layer)),
+            enrichments=pd.Series(max_or, index=overrepresentation.index),
+            colors=color_list,
             scale_factor=scale_factor,
             size=legend_pie_size,
             draw_labels=True,
             label_font_size=6, ax=ax_legend)
         draw_circle_bar_scale(
             position=(0, -0.75),
             scale_factor=scale_factor,
             size=pie_size,
-            label_font_size=5, ax=ax_legend)
+            label_font_size=8, ax=ax_legend)
         ax_legend.set_title(f"{layer}")
-        ax_legend.text(0, -0.25, "overrepresentation", ha="center", va="center", )
+        ax_legend.text(0, -1, "overrepresentation", ha="center", va="top", fontsize=10, fontweight="regular")
     
     # assert ax_plot.get_xlim() == ax_plot.get_ylim()
     # assert ax_plot.get_ylim() == ax_legend.get_ylim()
     
     if ax is None:
         return fig
 
@@ -1135,17 +1135,18 @@
             size=legend_pie_size,
             draw_labels=True,
             label_font_size=6, ax=ax_legend)
         draw_circle_bar_scale(
             position=(0, -0.75),
             scale_factor=scale_factor,
             size=pie_size,
-            label_font_size=5, ax=ax_legend)
+            label_font_size=8, ax=ax_legend)
         ax_legend.set_title(f"{layer}")
-        ax_legend.text(0, 0 , "overrepresentation", ha="center", va="center", )
+        ax_legend.text(0, -1, "overrepresentation", ha="center", va="top", fontsize=10, fontweight="regular")
+
     
     # assert ax_plot.get_xlim() == ax_plot.get_ylim()
     # assert ax_plot.get_ylim() == ax_legend.get_ylim()
     
     if ax is None:
         return fig
 
@@ -1310,18 +1311,19 @@
 
 
 def plot_overrepresentation_community_bar(snsmap: SNS,
                                       colors: Colors,
                                       layer: str,
                                       subset_datasets: Optional[Union[str, Collection[str]]] = None,
                                       figsize: Optional[Collection] = None,
+                                      truncate_negative = True,
                                       ax = None
                                       ) -> Figure:
     
-    df = snsmap.get_community_category_overrepresentation(subset_datasets=subset_datasets, layer=layer).fillna(0)
+    df = snsmap.get_community_category_overrepresentation(subset_datasets=subset_datasets, layer=layer, truncate_negative=truncate_negative).fillna(0)
     # if existing axes object is provided, plots with legend on that axes. Otherwise, creates a new figure with a separate plot and legend Axes.
     if ax is None:
         if figsize is None:
             figsize = [0.1 * df.shape[1] + 4, 4]
         fig, (ax_plot, ax_legend) = plt.subplots(1, 2, figsize=figsize, sharey=True, gridspec_kw={"width_ratios": [4, 1]}, layout="tight")
         ax_legend.set_axis_off()
     else:
@@ -1365,14 +1367,44 @@
     ax_plot.set_ylabel(f"Median {method.capitalize()} Correlation")
     ax_plot.set_xlabel("Community")
     
     if ax is None:
         return fig
 
 
+
+def plot_overrepresentation_community_heatmap(snsmap: SNS,
+                                      layer: str,
+                                      subset_datasets: Optional[Union[str, Collection[str]]] = None,
+                                      figsize: Optional[Collection] = None,
+                                      truncate_negative = False,
+                                      ax = None
+                                      ) -> Figure:
+    
+    df = snsmap.get_community_category_overrepresentation(subset_datasets=subset_datasets, layer=layer, truncate_negative=truncate_negative).fillna(0)
+    # if existing axes object is provided, plots with legend on that axes. Otherwise, creates a new figure with a separate plot and legend Axes.
+    if ax is None:
+        if figsize is None:
+            figsize = [0.2 * df.shape[1] + 4, 0.2 * df.shape[0] + 2]
+        fig, ax_plot = plt.subplots(figsize=figsize, layout="constrained")
+    else:
+        ax_plot = ax
+        
+    # Overrepresentation plot
+    sns.heatmap(data=df, ax=ax_plot, xticklabels = True, yticklabels=True, 
+                center = 0, cmap="RdBu_r")
+    
+    ax_plot.set_xticklabels(ax_plot.get_xticklabels(), rotation=0)
+    ax_plot.set_ylabel("Median overrepresentation")
+    ax_plot.set_xlabel("Community")
+    
+    if ax is None:
+        return fig
+
+
 #################################
 # Community-usage Entropy plots #
 #################################
 
 
 def plot_sample_entropy(snsmap: SNS,
                      colors: Colors,
```

### Comparing `cnmfsns-1.7.0/src/cnmfsns/sns.py` & `cnmfsns-1.7.1/src/cnmfsns/sns.py`

 * *Files identical despite different names*

### Comparing `cnmfsns-1.7.0/src/cnmfsns/utils.py` & `cnmfsns-1.7.1/src/cnmfsns/utils.py`

 * *Files identical despite different names*

### Comparing `cnmfsns-1.7.0/src/cnmfsns.egg-info/PKG-INFO` & `cnmfsns-1.7.1/src/cnmfsns.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cnmfsns
-Version: 1.7.0
+Version: 1.7.1
 Summary: cNMF Solution Network Space
 Home-page: https://github.com/MorrissyLab/cNMF-SNS
 Author: Ted Verhey
 Author-email: tbverhey@ucalgary.ca
 Project-URL: Bug Tracker, https://github.com/MorrissyLab/cNMF-SNS/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -16,15 +16,15 @@
 
 ![cNMF-SNS logo](logo.png)
 
 -----------------
 
 # cNMF-SNS: powerful factorization-based multi-omics integration toolkit
 
-![version badge](https://img.shields.io/badge/version-1.7.0-blue)
+![version badge](https://img.shields.io/badge/version-1.7.1-blue)
 [![PyPI Latest Release](https://img.shields.io/pypi/v/cnmfsns.svg)](https://pypi.org/project/cnmfsns/)
 [![Conda Latest Release](https://img.shields.io/conda/vn/conda-forge/cnmfsns)](https://anaconda.org/conda-forge/cnmfsns/)
 [![Documentation status](https://readthedocs.org/projects/cnmf-sns/badge/?version=latest&style=flat)]()
 [![Downloads](https://static.pepy.tech/badge/cnmfsns)](https://pepy.tech/project/cnmfsns)
 [![License](https://img.shields.io/pypi/l/cnmfsns.svg)](https://github.com/MorrissyLab/cNMF-SNS/blob/main/LICENSE)
 
 Authors: [Ted Verhey](https://github.com/verheytb), [Heewon Seo](https://github.com/lootpiz), [Sorana Morrissy](https://github.com/ancasorana)
```

