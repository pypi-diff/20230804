# Comparing `tmp/pydamage-0.70.tar.gz` & `tmp/pydamage-0.71.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pydamage-0.70.tar", last modified: Thu Mar 10 12:57:25 2022, max compression
+gzip compressed data, was "pydamage-0.71.tar", last modified: Fri Aug  4 13:56:39 2023, max compression
```

## Comparing `pydamage-0.70.tar` & `pydamage-0.71.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-03-10 12:57:25.000000 pydamage-0.70/
--rw-r--r--   0 runner    (1001) docker     (116)     3839 2022-03-10 12:57:25.000000 pydamage-0.70/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     2830 2022-03-10 12:57:16.000000 pydamage-0.70/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-03-10 12:57:25.000000 pydamage-0.70/pydamage/
--rw-r--r--   0 runner    (1001) docker     (116)       64 2022-03-10 12:57:16.000000 pydamage-0.70/pydamage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1045 2022-03-10 12:57:16.000000 pydamage-0.70/pydamage/accuracy_model.py
--rw-r--r--   0 runner    (1001) docker     (116)      625 2022-03-10 12:57:16.000000 pydamage-0.70/pydamage/citation.py
--rw-r--r--   0 runner    (1001) docker     (116)     2996 2022-03-10 12:57:16.000000 pydamage-0.70/pydamage/cli.py
--rw-r--r--   0 runner    (1001) docker     (116)    11706 2022-03-10 12:57:16.000000 pydamage-0.70/pydamage/damage.py
--rw-r--r--   0 runner    (1001) docker     (116)      403 2022-03-10 12:57:16.000000 pydamage-0.70/pydamage/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (116)     2399 2022-03-10 12:57:16.000000 pydamage-0.70/pydamage/filter.py
--rw-r--r--   0 runner    (1001) docker     (116)      674 2022-03-10 12:57:16.000000 pydamage-0.70/pydamage/gc_content.py
--rw-r--r--   0 runner    (1001) docker     (116)      497 2022-03-10 12:57:16.000000 pydamage-0.70/pydamage/likelihood_ratio.py
--rw-r--r--   0 runner    (1001) docker     (116)     3826 2022-03-10 12:57:16.000000 pydamage-0.70/pydamage/main.py
--rw-r--r--   0 runner    (1001) docker     (116)     2959 2022-03-10 12:57:16.000000 pydamage-0.70/pydamage/model_fit.py
--rw-r--r--   0 runner    (1001) docker     (116)     2289 2022-03-10 12:57:16.000000 pydamage-0.70/pydamage/models.py
--rw-r--r--   0 runner    (1001) docker     (116)     1034 2022-03-10 12:57:16.000000 pydamage-0.70/pydamage/optim.py
--rw-r--r--   0 runner    (1001) docker     (116)     2642 2022-03-10 12:57:16.000000 pydamage-0.70/pydamage/parse_damage.py
--rw-r--r--   0 runner    (1001) docker     (116)     4302 2022-03-10 12:57:16.000000 pydamage-0.70/pydamage/plot.py
--rw-r--r--   0 runner    (1001) docker     (116)     7315 2022-03-10 12:57:16.000000 pydamage-0.70/pydamage/utils.py
--rw-r--r--   0 runner    (1001) docker     (116)      596 2022-03-10 12:57:16.000000 pydamage-0.70/pydamage/vuong.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-03-10 12:57:25.000000 pydamage-0.70/pydamage.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     3839 2022-03-10 12:57:24.000000 pydamage-0.70/pydamage.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      564 2022-03-10 12:57:25.000000 pydamage-0.70/pydamage.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-03-10 12:57:24.000000 pydamage-0.70/pydamage.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       47 2022-03-10 12:57:24.000000 pydamage-0.70/pydamage.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (116)       75 2022-03-10 12:57:24.000000 pydamage-0.70/pydamage.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        9 2022-03-10 12:57:24.000000 pydamage-0.70/pydamage.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)       38 2022-03-10 12:57:25.000000 pydamage-0.70/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1192 2022-03-10 12:57:16.000000 pydamage-0.70/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:56:39.626516 pydamage-0.71/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-08-04 13:56:36.000000 pydamage-0.71/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-08-04 13:56:39.626516 pydamage-0.71/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-08-04 13:56:36.000000 pydamage-0.71/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:56:39.626516 pydamage-0.71/pydamage/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-08-04 13:56:36.000000 pydamage-0.71/pydamage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-08-04 13:56:36.000000 pydamage-0.71/pydamage/accuracy_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-08-04 13:56:36.000000 pydamage-0.71/pydamage/citation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-08-04 13:56:36.000000 pydamage-0.71/pydamage/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11706 2023-08-04 13:56:36.000000 pydamage-0.71/pydamage/damage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-08-04 13:56:36.000000 pydamage-0.71/pydamage/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2399 2023-08-04 13:56:36.000000 pydamage-0.71/pydamage/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-08-04 13:56:36.000000 pydamage-0.71/pydamage/gc_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-08-04 13:56:36.000000 pydamage-0.71/pydamage/likelihood_ratio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4079 2023-08-04 13:56:36.000000 pydamage-0.71/pydamage/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-08-04 13:56:36.000000 pydamage-0.71/pydamage/model_fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-08-04 13:56:36.000000 pydamage-0.71/pydamage/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-08-04 13:56:36.000000 pydamage-0.71/pydamage/optim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-08-04 13:56:36.000000 pydamage-0.71/pydamage/parse_damage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-08-04 13:56:36.000000 pydamage-0.71/pydamage/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7465 2023-08-04 13:56:36.000000 pydamage-0.71/pydamage/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-08-04 13:56:36.000000 pydamage-0.71/pydamage/vuong.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:56:39.626516 pydamage-0.71/pydamage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-08-04 13:56:39.000000 pydamage-0.71/pydamage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-08-04 13:56:39.000000 pydamage-0.71/pydamage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 13:56:39.000000 pydamage-0.71/pydamage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-04 13:56:39.000000 pydamage-0.71/pydamage.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-08-04 13:56:39.000000 pydamage-0.71/pydamage.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-04 13:56:39.000000 pydamage-0.71/pydamage.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 13:56:39.626516 pydamage-0.71/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-08-04 13:56:36.000000 pydamage-0.71/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pydamage-0.70/PKG-INFO` & `pydamage-0.71/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,103 +1,94 @@
-Metadata-Version: 2.1
-Name: pydamage
-Version: 0.70
-Summary: Damage parameter estimation for ancient DNA
-Home-page: https://github.com/maxibor/pydamage
-License: GNU-GPLv3
-Description: <p align="center">
-            <a href="https://github.com/maxibor/pydamage"><img src="https://github.com/maxibor/pydamage/raw/master/docs/img/logo.png" alt="PyDamage"></a>
-        </p>
-        
-        <p align="center">
-            <a href="https://github.com/maxibor/pydamage/releases"><img src="https://img.shields.io/github/v/release/maxibor/pydamage?include_prereleases&label=version"/></a>
-            <a href="https://github.com/maxibor/pydamage/actions"><img src="https://github.com/maxibor/pydamage/workflows/pydamage_ci/badge.svg"/></a>
-            <a href="https://pydamage.readthedocs.io"><img src="https://readthedocs.org/projects/pydamage/badge/?version=latest"/></a>
-            <a href="https://pypi.org/project/pydamage/"><img src="https://img.shields.io/badge/install%20with-pip-blue"/></a>
-            <a href="https://anaconda.org/bioconda/pydamage"><img src="https://img.shields.io/badge/install%20with-bioconda-brightgreen.svg?style=flat"/></a>
-        </p>
-        
-        # PyDamage
-        
-        Pydamage, is a Python software to automate the process of contig damage identification and estimation.
-        After modelling the ancient DNA damage using the C to T transitions, Pydamage uses a likelihood ratio test to discriminate between truly ancient, and modern contigs originating from sample contamination.
-        
-        ## Installation
-        
-        ### With [conda](https://docs.conda.io/en/latest/) (recommended)
-        
-        ```bash
-        conda install -c bioconda pydamage
-        ```
-        
-        ### With pip
-        
-        ```bash
-        pip install pydamage
-        ```
-        
-        ### Install from source to use the development version
-        
-        Using pip
-        
-        ```bash
-        pip install git+ssh://git@github.com/maxibor/pydamage.git@dev
-        ```
-        
-        By cloning in a dedicated conda environment
-        
-        ```bash
-        git clone git@github.com:maxibor/pydamage.git
-        cd pydamage
-        git checkout dev
-        conda env create -f environment.yml
-        conda activate pydamage
-        pip install -e .
-        ```
-        
-        
-        ## Quick start
-        
-        ```bash
-        pydamage --outdir result_directory analyze aligned.bam
-        ```
-        
-        > Note that if you specify `--outdir`, it has to be before the PyDamage subcommand, example: `pydamage --outdir test filter pydamage_results.csv`
-        
-        ## CLI help
-        
-        Command line interface help message
-        
-        ```bash
-        pydamage --help
-        ```
-        
-        ## Documentation
-        
-        [pydamage.readthedocs.io](https://pydamage.readthedocs.io)
-        
-        ## Cite
-        
-        PyDamage has been published in PeerJ: [10.7717/peerj.11845](https://doi.org/10.7717/peerj.11845)
-        
-        ```
-        @article{borry_pydamage_2021,
-            author = {Borry, Maxime and Hübner, Alexander and Rohrlach, Adam B. and Warinner, Christina},
-            doi = {10.7717/peerj.11845},
-            issn = {2167-8359},
-            journal = {PeerJ},
-            language = {en},
-            month = {July},
-            note = {Publisher: PeerJ Inc.},
-            pages = {e11845},
-            shorttitle = {PyDamage},
-            title = {PyDamage: automated ancient damage identification and estimation for contigs in ancient DNA de novo assembly},
-            url = {https://peerj.com/articles/11845},
-            urldate = {2021-07-27},
-            volume = {9},
-            year = {2021}
-        }
-        
-        ```
-Platform: UNKNOWN
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
+<p align="center">
+    <a href="https://github.com/maxibor/pydamage"><img src="https://github.com/maxibor/pydamage/raw/master/docs/img/logo.png" alt="PyDamage"></a>
+</p>
+
+<p align="center">
+    <a href="https://github.com/maxibor/pydamage/releases"><img src="https://img.shields.io/github/v/release/maxibor/pydamage?include_prereleases&label=version"/></a>
+    <a href="https://github.com/maxibor/pydamage/actions"><img src="https://github.com/maxibor/pydamage/workflows/pydamage_ci/badge.svg"/></a>
+    <a href="https://pydamage.readthedocs.io"><img src="https://readthedocs.org/projects/pydamage/badge/?version=latest"/></a>
+    <a href="https://pypi.org/project/pydamage/"><img src="https://img.shields.io/badge/install%20with-pip-blue"/></a>
+    <a href="https://anaconda.org/bioconda/pydamage"><img src="https://img.shields.io/badge/install%20with-bioconda-brightgreen.svg?style=flat"/></a>
+</p>
+
+# PyDamage
+
+Pydamage, is a Python software to automate the process of contig damage identification and estimation.
+After modelling the ancient DNA damage using the C to T transitions, Pydamage uses a likelihood ratio test to discriminate between truly ancient, and modern contigs originating from sample contamination.
+
+## Installation
+
+### With [conda](https://docs.conda.io/en/latest/) (recommended)
+
+```bash
+conda install -c bioconda pydamage
+```
+
+### With pip
+
+```bash
+pip install pydamage
+```
+
+### Install from source to use the development version
+
+Using pip
+
+```bash
+pip install git+ssh://git@github.com/maxibor/pydamage.git@dev
+```
+
+By cloning in a dedicated conda environment
+
+```bash
+git clone git@github.com:maxibor/pydamage.git
+cd pydamage
+git checkout dev
+conda env create -f environment.yml
+conda activate pydamage
+pip install -e .
+```
+
+
+## Quick start
+
+```bash
+pydamage --outdir result_directory analyze aligned.bam
+```
+
+> Note that if you specify `--outdir`, it has to be before the PyDamage subcommand, example: `pydamage --outdir test filter pydamage_results.csv`
+
+## CLI help
+
+Command line interface help message
+
+```bash
+pydamage --help
+```
+
+## Documentation
+
+[pydamage.readthedocs.io](https://pydamage.readthedocs.io)
+
+## Cite
+
+PyDamage has been published in PeerJ: [10.7717/peerj.11845](https://doi.org/10.7717/peerj.11845)
+
+```
+@article{borry_pydamage_2021,
+    author = {Borry, Maxime and Hübner, Alexander and Rohrlach, Adam B. and Warinner, Christina},
+    doi = {10.7717/peerj.11845},
+    issn = {2167-8359},
+    journal = {PeerJ},
+    language = {en},
+    month = {July},
+    note = {Publisher: PeerJ Inc.},
+    pages = {e11845},
+    shorttitle = {PyDamage},
+    title = {PyDamage: automated ancient damage identification and estimation for contigs in ancient DNA de novo assembly},
+    url = {https://peerj.com/articles/11845},
+    urldate = {2021-07-27},
+    volume = {9},
+    year = {2021}
+}
+
+```
```

#### html2text {}

```diff
@@ -1,10 +1,7 @@
-Metadata-Version: 2.1 Name: pydamage Version: 0.70 Summary: Damage parameter
-estimation for ancient DNA Home-page: https://github.com/maxibor/pydamage
-License: GNU-GPLv3 Description:
                                   [PyDamage]
                [https://img.shields.io/github/v/release/maxibor/
    pydamage?include_prereleases&label=version] [https://github.com/maxibor/
  pydamage/workflows/pydamage_ci/badge.svg] [https://readthedocs.org/projects/
  pydamage/badge/?version=latest] [https://img.shields.io/badge/install%20with-
        pip-blue] [https://img.shields.io/badge/install%20with-bioconda-
                           brightgreen.svg?style=flat]
@@ -28,9 +25,8 @@
 [10.7717/peerj.11845](https://doi.org/10.7717/peerj.11845) ``` @article
 {borry_pydamage_2021, author = {Borry, Maxime and HÃ¼bner, Alexander and
 Rohrlach, Adam B. and Warinner, Christina}, doi = {10.7717/peerj.11845}, issn =
 {2167-8359}, journal = {PeerJ}, language = {en}, month = {July}, note =
 {Publisher: PeerJ Inc.}, pages = {e11845}, shorttitle = {PyDamage}, title =
 {PyDamage: automated ancient damage identification and estimation for contigs
 in ancient DNA de novo assembly}, url = {https://peerj.com/articles/11845},
-urldate = {2021-07-27}, volume = {9}, year = {2021} } ``` Platform: UNKNOWN
-Requires-Python: >=3.6 Description-Content-Type: text/markdown
+urldate = {2021-07-27}, volume = {9}, year = {2021} } ```
```

### Comparing `pydamage-0.70/README.md` & `pydamage-0.71/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+Metadata-Version: 2.1
+Name: pydamage
+Version: 0.71
+Summary: Damage parameter estimation for ancient DNA
+Home-page: https://github.com/maxibor/pydamage
+License: GNU-GPLv3
+Platform: UNKNOWN
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <p align="center">
     <a href="https://github.com/maxibor/pydamage"><img src="https://github.com/maxibor/pydamage/raw/master/docs/img/logo.png" alt="PyDamage"></a>
 </p>
 
 <p align="center">
     <a href="https://github.com/maxibor/pydamage/releases"><img src="https://img.shields.io/github/v/release/maxibor/pydamage?include_prereleases&label=version"/></a>
     <a href="https://github.com/maxibor/pydamage/actions"><img src="https://github.com/maxibor/pydamage/workflows/pydamage_ci/badge.svg"/></a>
@@ -87,8 +98,9 @@
     title = {PyDamage: automated ancient damage identification and estimation for contigs in ancient DNA de novo assembly},
     url = {https://peerj.com/articles/11845},
     urldate = {2021-07-27},
     volume = {9},
     year = {2021}
 }
 
-```
+```
+
```

#### html2text {}

```diff
@@ -1,7 +1,11 @@
+Metadata-Version: 2.1 Name: pydamage Version: 0.71 Summary: Damage parameter
+estimation for ancient DNA Home-page: https://github.com/maxibor/pydamage
+License: GNU-GPLv3 Platform: UNKNOWN Requires-Python: >=3.6 Description-
+Content-Type: text/markdown License-File: LICENSE
                                   [PyDamage]
                [https://img.shields.io/github/v/release/maxibor/
    pydamage?include_prereleases&label=version] [https://github.com/maxibor/
  pydamage/workflows/pydamage_ci/badge.svg] [https://readthedocs.org/projects/
  pydamage/badge/?version=latest] [https://img.shields.io/badge/install%20with-
        pip-blue] [https://img.shields.io/badge/install%20with-bioconda-
                           brightgreen.svg?style=flat]
```

### Comparing `pydamage-0.70/pydamage/accuracy_model.py` & `pydamage-0.71/pydamage/accuracy_model.py`

 * *Files identical despite different names*

### Comparing `pydamage-0.70/pydamage/citation.py` & `pydamage-0.71/pydamage/citation.py`

 * *Files identical despite different names*

### Comparing `pydamage-0.70/pydamage/cli.py` & `pydamage-0.71/pydamage/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,14 +55,22 @@
     "--wlen",
     default=20,
     type=int,
     show_default=True,
     help="Window length (in bp) for damage modeling",
 )
 @click.option(
+    "-m",
+    "--minlen",
+    default=0,
+    type=int,
+    show_default=True,
+    help="Minimum of length of reference sequence to consider",
+)
+@click.option(
     "-p",
     "--process",
     default=2,
     type=int,
     show_default=True,
     help="Number of processes for parallel computing",
 )
@@ -74,15 +82,15 @@
 @click.option(
     "-f", "--force", is_flag=True, help="Force overwriting of results directory"
 )
 @click.option(
     "-g",
     "--group",
     is_flag=True,
-    help="Use entire BAM file as single reference for analyis "
+    help="Use entire BAM file as single reference for analysis "
     "(ignore reference headers)",
 )
 def analyze(ctx, no_args_is_help=True, **kwargs):
     """\b
     Run the PyDamage analysis
 
     BAM: path to BAM/SAM/CRAM alignment file. MD tags need to be set.
```

### Comparing `pydamage-0.70/pydamage/damage.py` & `pydamage-0.71/pydamage/damage.py`

 * *Files identical despite different names*

### Comparing `pydamage-0.70/pydamage/filter.py` & `pydamage-0.71/pydamage/filter.py`

 * *Files identical despite different names*

### Comparing `pydamage-0.70/pydamage/gc_content.py` & `pydamage-0.71/pydamage/gc_content.py`

 * *Files identical despite different names*

### Comparing `pydamage-0.70/pydamage/main.py` & `pydamage-0.71/pydamage/main.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 import pysam
 from pydamage import utils
 import multiprocessing
 from functools import partial
 from pydamage import damage
 from pydamage.plot import damageplot
-from pydamage.exceptions import PyDamageWarning
+from pydamage.exceptions import PyDamageWarning, AlignmentFileError
 from pydamage.accuracy_model import prepare_data, glm_predict
 from pydamage.models import glm_model_params
 import sys
 from tqdm import tqdm
 import warnings
 from pydamage import __version__
 
@@ -36,43 +36,45 @@
 #             bam, wlen, show_al, process, outdir, plot, verbose, force
 #         )
 
 
 def pydamage_analyze(
     bam,
     wlen=30,
+    minlen=0,
     show_al=False,
     process=1,
     outdir="",
     plot=False,
     verbose=False,
     force=False,
     group=False,
 ):
     """Runs the pydamage analysis for each reference separately
 
     Args:
         bam(str): Path to alignment (sam/bam/cram) file
+        minlen(int): minimum reference sequence length threshold
         wlen(int): window length
         show_al(bool): print alignments representations
         process(int):  Number of  processes for parellel computing
         outdir(str): Path to output directory
         verbose(bool): verbose mode
         force(bool): force overwriting of results directory
     Returns:
         pd.DataFrame: pandas DataFrame containg pydamage results
 
     """
     if verbose:
         print(f"Pydamage version {__version__}\n")
     utils.makedir(outdir, force=force)
 
-    refs, mode = utils.prepare_bam(bam)
+    refs, mode = utils.prepare_bam(bam, minlen=minlen)
 
-    proc = min(len(refs), process)
+    proc = max(1, min(len(refs), process))
 
     ##########################
     # Simple loop for debugging
     ##########################
     # filt_res = []
     # for ref in refs:
     #     res = damage.test_damage(
@@ -109,19 +111,22 @@
                 wlen=wlen,
                 show_al=show_al,
                 process=process,
                 verbose=verbose,
             )
         ]
     else:
-        with multiprocessing.Pool(proc) as p:
-            res = list(tqdm(p.imap(test_damage_partial, refs), total=len(refs)))
-        filt_res = [i for i in res if i]
+        if len(refs) > 0:
+            with multiprocessing.Pool(proc) as p:
+                res = list(tqdm(p.imap(test_damage_partial, refs), total=len(refs)))
+            filt_res = [i for i in res if i]
+        else:
+            raise AlignmentFileError("No reference sequences were found in alignment file")
 
-    print(f"{len(filt_res)} contig(s) successfully analyzed by Pydamage")
+    print(f"{len(filt_res)} contig(s) analyzed by Pydamage")
     if len(filt_res) == 0:
         warnings.warn(
             "No alignments were found, check your alignment file", PyDamageWarning
         )
 
     if plot and len(filt_res) > 0:
         print("\nGenerating Pydamage plots")
```

### Comparing `pydamage-0.70/pydamage/model_fit.py` & `pydamage-0.71/pydamage/model_fit.py`

 * *Files identical despite different names*

### Comparing `pydamage-0.70/pydamage/models.py` & `pydamage-0.71/pydamage/models.py`

 * *Files identical despite different names*

### Comparing `pydamage-0.70/pydamage/optim.py` & `pydamage-0.71/pydamage/optim.py`

 * *Files identical despite different names*

### Comparing `pydamage-0.70/pydamage/parse_damage.py` & `pydamage-0.71/pydamage/parse_damage.py`

 * *Files identical despite different names*

### Comparing `pydamage-0.70/pydamage/plot.py` & `pydamage-0.71/pydamage/plot.py`

 * *Files identical despite different names*

### Comparing `pydamage-0.70/pydamage/utils.py` & `pydamage-0.71/pydamage/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -149,15 +149,15 @@
     Args:
         df(pandas DataFrame): Pydamage results DataFrame
         outdir (str): Path to output directory
     """
     df = df.round(3)
     if not outdir:
         outdir = "."
-    df.to_csv(f"{outdir}/{outfile}")
+    df.to_csv(f"{outdir}/{outfile}", index=False)
 
 
 def sort_dict_by_keys(adict: dict) -> dict:
     """Sort dictonary by keys
 
     Args:
         adict (dict): dictorary to sort
@@ -214,19 +214,20 @@
             if i in non_damage:
                 non_damage_dict[i] = non_damage[i]
             else:
                 non_damage_dict[i] = 0
 
     return (damage_dict, non_damage_dict)
 
-def prepare_bam(bam: str) -> Tuple[Tuple, str]:
-    """Checks for file extension, and returns tuple of mapped refs
+def prepare_bam(bam: str, minlen: int) -> Tuple[Tuple, str]:
+    """Checks for file extension, and returns tuple of mapped refs of minlen
 
     Args:
         bam (str): Path to bam file
+        minlen(int): minimum reference sequence length threshold
 
     Returns:
         Tuple: Tuple of mapped references
         str: bam opening mode
     """
     mode = check_extension(bam)
     alf = AlignmentFile(bam, mode)
@@ -235,15 +236,15 @@
         print(
             f"BAM file {bam} has no index. Sort BAM file and provide index "
             "before running pydamage."
         )
         sys.exit(1)
 
     present_refs = set()
-    for ref_stat in alf.get_index_statistics():
+    for ref_stat,ref_len in zip(alf.get_index_statistics(), alf.lengths):
         refname = ref_stat[0]
         nb_mapped_reads = ref_stat[1]
-        if nb_mapped_reads > 0:
+        if nb_mapped_reads > 0 and ref_len >= minlen:
             present_refs.add(refname)
     alf.close()
     return tuple(present_refs), mode
-    
+
```

### Comparing `pydamage-0.70/pydamage/vuong.py` & `pydamage-0.71/pydamage/vuong.py`

 * *Files identical despite different names*

### Comparing `pydamage-0.70/pydamage.egg-info/PKG-INFO` & `pydamage-0.71/pydamage.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,103 +1,106 @@
 Metadata-Version: 2.1
 Name: pydamage
-Version: 0.70
+Version: 0.71
 Summary: Damage parameter estimation for ancient DNA
 Home-page: https://github.com/maxibor/pydamage
 License: GNU-GPLv3
-Description: <p align="center">
-            <a href="https://github.com/maxibor/pydamage"><img src="https://github.com/maxibor/pydamage/raw/master/docs/img/logo.png" alt="PyDamage"></a>
-        </p>
-        
-        <p align="center">
-            <a href="https://github.com/maxibor/pydamage/releases"><img src="https://img.shields.io/github/v/release/maxibor/pydamage?include_prereleases&label=version"/></a>
-            <a href="https://github.com/maxibor/pydamage/actions"><img src="https://github.com/maxibor/pydamage/workflows/pydamage_ci/badge.svg"/></a>
-            <a href="https://pydamage.readthedocs.io"><img src="https://readthedocs.org/projects/pydamage/badge/?version=latest"/></a>
-            <a href="https://pypi.org/project/pydamage/"><img src="https://img.shields.io/badge/install%20with-pip-blue"/></a>
-            <a href="https://anaconda.org/bioconda/pydamage"><img src="https://img.shields.io/badge/install%20with-bioconda-brightgreen.svg?style=flat"/></a>
-        </p>
-        
-        # PyDamage
-        
-        Pydamage, is a Python software to automate the process of contig damage identification and estimation.
-        After modelling the ancient DNA damage using the C to T transitions, Pydamage uses a likelihood ratio test to discriminate between truly ancient, and modern contigs originating from sample contamination.
-        
-        ## Installation
-        
-        ### With [conda](https://docs.conda.io/en/latest/) (recommended)
-        
-        ```bash
-        conda install -c bioconda pydamage
-        ```
-        
-        ### With pip
-        
-        ```bash
-        pip install pydamage
-        ```
-        
-        ### Install from source to use the development version
-        
-        Using pip
-        
-        ```bash
-        pip install git+ssh://git@github.com/maxibor/pydamage.git@dev
-        ```
-        
-        By cloning in a dedicated conda environment
-        
-        ```bash
-        git clone git@github.com:maxibor/pydamage.git
-        cd pydamage
-        git checkout dev
-        conda env create -f environment.yml
-        conda activate pydamage
-        pip install -e .
-        ```
-        
-        
-        ## Quick start
-        
-        ```bash
-        pydamage --outdir result_directory analyze aligned.bam
-        ```
-        
-        > Note that if you specify `--outdir`, it has to be before the PyDamage subcommand, example: `pydamage --outdir test filter pydamage_results.csv`
-        
-        ## CLI help
-        
-        Command line interface help message
-        
-        ```bash
-        pydamage --help
-        ```
-        
-        ## Documentation
-        
-        [pydamage.readthedocs.io](https://pydamage.readthedocs.io)
-        
-        ## Cite
-        
-        PyDamage has been published in PeerJ: [10.7717/peerj.11845](https://doi.org/10.7717/peerj.11845)
-        
-        ```
-        @article{borry_pydamage_2021,
-            author = {Borry, Maxime and Hübner, Alexander and Rohrlach, Adam B. and Warinner, Christina},
-            doi = {10.7717/peerj.11845},
-            issn = {2167-8359},
-            journal = {PeerJ},
-            language = {en},
-            month = {July},
-            note = {Publisher: PeerJ Inc.},
-            pages = {e11845},
-            shorttitle = {PyDamage},
-            title = {PyDamage: automated ancient damage identification and estimation for contigs in ancient DNA de novo assembly},
-            url = {https://peerj.com/articles/11845},
-            urldate = {2021-07-27},
-            volume = {9},
-            year = {2021}
-        }
-        
-        ```
 Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+<p align="center">
+    <a href="https://github.com/maxibor/pydamage"><img src="https://github.com/maxibor/pydamage/raw/master/docs/img/logo.png" alt="PyDamage"></a>
+</p>
+
+<p align="center">
+    <a href="https://github.com/maxibor/pydamage/releases"><img src="https://img.shields.io/github/v/release/maxibor/pydamage?include_prereleases&label=version"/></a>
+    <a href="https://github.com/maxibor/pydamage/actions"><img src="https://github.com/maxibor/pydamage/workflows/pydamage_ci/badge.svg"/></a>
+    <a href="https://pydamage.readthedocs.io"><img src="https://readthedocs.org/projects/pydamage/badge/?version=latest"/></a>
+    <a href="https://pypi.org/project/pydamage/"><img src="https://img.shields.io/badge/install%20with-pip-blue"/></a>
+    <a href="https://anaconda.org/bioconda/pydamage"><img src="https://img.shields.io/badge/install%20with-bioconda-brightgreen.svg?style=flat"/></a>
+</p>
+
+# PyDamage
+
+Pydamage, is a Python software to automate the process of contig damage identification and estimation.
+After modelling the ancient DNA damage using the C to T transitions, Pydamage uses a likelihood ratio test to discriminate between truly ancient, and modern contigs originating from sample contamination.
+
+## Installation
+
+### With [conda](https://docs.conda.io/en/latest/) (recommended)
+
+```bash
+conda install -c bioconda pydamage
+```
+
+### With pip
+
+```bash
+pip install pydamage
+```
+
+### Install from source to use the development version
+
+Using pip
+
+```bash
+pip install git+ssh://git@github.com/maxibor/pydamage.git@dev
+```
+
+By cloning in a dedicated conda environment
+
+```bash
+git clone git@github.com:maxibor/pydamage.git
+cd pydamage
+git checkout dev
+conda env create -f environment.yml
+conda activate pydamage
+pip install -e .
+```
+
+
+## Quick start
+
+```bash
+pydamage --outdir result_directory analyze aligned.bam
+```
+
+> Note that if you specify `--outdir`, it has to be before the PyDamage subcommand, example: `pydamage --outdir test filter pydamage_results.csv`
+
+## CLI help
+
+Command line interface help message
+
+```bash
+pydamage --help
+```
+
+## Documentation
+
+[pydamage.readthedocs.io](https://pydamage.readthedocs.io)
+
+## Cite
+
+PyDamage has been published in PeerJ: [10.7717/peerj.11845](https://doi.org/10.7717/peerj.11845)
+
+```
+@article{borry_pydamage_2021,
+    author = {Borry, Maxime and Hübner, Alexander and Rohrlach, Adam B. and Warinner, Christina},
+    doi = {10.7717/peerj.11845},
+    issn = {2167-8359},
+    journal = {PeerJ},
+    language = {en},
+    month = {July},
+    note = {Publisher: PeerJ Inc.},
+    pages = {e11845},
+    shorttitle = {PyDamage},
+    title = {PyDamage: automated ancient damage identification and estimation for contigs in ancient DNA de novo assembly},
+    url = {https://peerj.com/articles/11845},
+    urldate = {2021-07-27},
+    volume = {9},
+    year = {2021}
+}
+
+```
+
```

#### html2text {}

```diff
@@ -1,10 +1,11 @@
-Metadata-Version: 2.1 Name: pydamage Version: 0.70 Summary: Damage parameter
+Metadata-Version: 2.1 Name: pydamage Version: 0.71 Summary: Damage parameter
 estimation for ancient DNA Home-page: https://github.com/maxibor/pydamage
-License: GNU-GPLv3 Description:
+License: GNU-GPLv3 Platform: UNKNOWN Requires-Python: >=3.6 Description-
+Content-Type: text/markdown License-File: LICENSE
                                   [PyDamage]
                [https://img.shields.io/github/v/release/maxibor/
    pydamage?include_prereleases&label=version] [https://github.com/maxibor/
  pydamage/workflows/pydamage_ci/badge.svg] [https://readthedocs.org/projects/
  pydamage/badge/?version=latest] [https://img.shields.io/badge/install%20with-
        pip-blue] [https://img.shields.io/badge/install%20with-bioconda-
                           brightgreen.svg?style=flat]
@@ -28,9 +29,8 @@
 [10.7717/peerj.11845](https://doi.org/10.7717/peerj.11845) ``` @article
 {borry_pydamage_2021, author = {Borry, Maxime and HÃ¼bner, Alexander and
 Rohrlach, Adam B. and Warinner, Christina}, doi = {10.7717/peerj.11845}, issn =
 {2167-8359}, journal = {PeerJ}, language = {en}, month = {July}, note =
 {Publisher: PeerJ Inc.}, pages = {e11845}, shorttitle = {PyDamage}, title =
 {PyDamage: automated ancient damage identification and estimation for contigs
 in ancient DNA de novo assembly}, url = {https://peerj.com/articles/11845},
-urldate = {2021-07-27}, volume = {9}, year = {2021} } ``` Platform: UNKNOWN
-Requires-Python: >=3.6 Description-Content-Type: text/markdown
+urldate = {2021-07-27}, volume = {9}, year = {2021} } ```
```

### Comparing `pydamage-0.70/pydamage.egg-info/SOURCES.txt` & `pydamage-0.71/pydamage.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 setup.py
 pydamage/__init__.py
 pydamage/accuracy_model.py
 pydamage/citation.py
 pydamage/cli.py
 pydamage/damage.py
```

### Comparing `pydamage-0.70/setup.py` & `pydamage-0.71/setup.py`

 * *Files identical despite different names*

