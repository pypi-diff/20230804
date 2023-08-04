# Comparing `tmp/pygenomeviz-0.3.2.tar.gz` & `tmp/pygenomeviz-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygenomeviz-0.3.2.tar", max compression
+gzip compressed data, was "pygenomeviz-0.4.0.tar", max compression
```

## Comparing `pygenomeviz-0.3.2.tar` & `pygenomeviz-0.4.0.tar`

### file list

```diff
@@ -1,53 +1,59 @@
--rw-r--r--   0        0        0     1062 2023-01-31 14:56:08.035411 pygenomeviz-0.3.2/LICENSE
--rw-r--r--   0        0        0    15681 2023-01-31 14:56:08.035411 pygenomeviz-0.3.2/README.md
--rw-r--r--   0        0        0     1480 2023-01-31 14:56:08.155411 pygenomeviz-0.3.2/pyproject.toml
--rw-r--r--   0        0        0      883 2023-01-31 14:56:08.155411 pygenomeviz-0.3.2/src/pygenomeviz/__init__.py
--rw-r--r--   0        0        0    22619 2023-01-31 14:56:08.155411 pygenomeviz-0.3.2/src/pygenomeviz/align.py
--rw-r--r--   0        0        0     2411 2023-01-31 14:56:08.155411 pygenomeviz-0.3.2/src/pygenomeviz/config.py
--rw-r--r--   0        0        0    19158 2023-01-31 14:56:08.155411 pygenomeviz-0.3.2/src/pygenomeviz/feature.py
--rw-r--r--   0        0        0    26053 2023-01-31 14:56:08.155411 pygenomeviz-0.3.2/src/pygenomeviz/genomeviz.py
--rw-r--r--   0        0        0     6762 2023-01-31 14:56:08.155411 pygenomeviz-0.3.2/src/pygenomeviz/link.py
--rw-r--r--   0        0        0      127 2023-01-31 14:56:08.155411 pygenomeviz-0.3.2/src/pygenomeviz/parser/__init__.py
--rw-r--r--   0        0        0    14433 2023-01-31 14:56:08.155411 pygenomeviz-0.3.2/src/pygenomeviz/parser/genbank.py
--rw-r--r--   0        0        0    13398 2023-01-31 14:56:08.155411 pygenomeviz-0.3.2/src/pygenomeviz/parser/gff.py
--rw-r--r--   0        0        0     2991 2023-01-31 14:56:08.155411 pygenomeviz-0.3.2/src/pygenomeviz/scripts/__init__.py
--rw-r--r--   0        0        0     1687 2023-01-31 14:56:08.155411 pygenomeviz-0.3.2/src/pygenomeviz/scripts/download_dataset.py
--rw-r--r--   0        0        0    14718 2023-01-31 14:56:08.155411 pygenomeviz-0.3.2/src/pygenomeviz/scripts/mmseqs.py
--rw-r--r--   0        0        0    16243 2023-01-31 14:56:08.155411 pygenomeviz-0.3.2/src/pygenomeviz/scripts/mummer.py
--rw-r--r--   0        0        0    13002 2023-01-31 14:56:08.155411 pygenomeviz-0.3.2/src/pygenomeviz/scripts/pmauve.py
--rw-r--r--   0        0        0     9598 2023-01-31 14:56:08.155411 pygenomeviz-0.3.2/src/pygenomeviz/scripts/simpleplot.py
--rw-r--r--   0        0        0    33043 2023-01-31 14:56:08.155411 pygenomeviz-0.3.2/src/pygenomeviz/track.py
--rw-r--r--   0        0        0     8206 2023-01-31 14:56:08.155411 pygenomeviz-0.3.2/src/pygenomeviz/utils.py
--rw-r--r--   0        0        0     7090 2023-01-31 14:56:08.155411 pygenomeviz-0.3.2/src/pygenomeviz/viewer/assets/lib/images/ui-icons_444444_256x240.png
--rw-r--r--   0        0        0     7074 2023-01-31 14:56:08.155411 pygenomeviz-0.3.2/src/pygenomeviz/viewer/assets/lib/images/ui-icons_555555_256x240.png
--rw-r--r--   0        0        0     4618 2023-01-31 14:56:08.155411 pygenomeviz-0.3.2/src/pygenomeviz/viewer/assets/lib/images/ui-icons_777620_256x240.png
--rw-r--r--   0        0        0     7111 2023-01-31 14:56:08.155411 pygenomeviz-0.3.2/src/pygenomeviz/viewer/assets/lib/images/ui-icons_777777_256x240.png
--rw-r--r--   0        0        0     4618 2023-01-31 14:56:08.155411 pygenomeviz-0.3.2/src/pygenomeviz/viewer/assets/lib/images/ui-icons_cc0000_256x240.png
--rw-r--r--   0        0        0     6487 2023-01-31 14:56:08.155411 pygenomeviz-0.3.2/src/pygenomeviz/viewer/assets/lib/images/ui-icons_ffffff_256x240.png
--rw-r--r--   0        0        0    30801 2023-01-31 14:56:08.155411 pygenomeviz-0.3.2/src/pygenomeviz/viewer/assets/lib/jquery-ui.min.css
--rw-r--r--   0        0        0   255079 2023-01-31 14:56:08.159411 pygenomeviz-0.3.2/src/pygenomeviz/viewer/assets/lib/jquery-ui.min.js
--rw-r--r--   0        0        0    89664 2023-01-31 14:56:08.159411 pygenomeviz-0.3.2/src/pygenomeviz/viewer/assets/lib/jquery.min.js
--rw-r--r--   0        0        0    10026 2023-01-31 14:56:08.159411 pygenomeviz-0.3.2/src/pygenomeviz/viewer/assets/lib/panzoom.min.js
--rw-r--r--   0        0        0    10465 2023-01-31 14:56:08.159411 pygenomeviz-0.3.2/src/pygenomeviz/viewer/assets/lib/spectrum.min.css
--rw-r--r--   0        0        0    27904 2023-01-31 14:56:08.159411 pygenomeviz-0.3.2/src/pygenomeviz/viewer/assets/lib/spectrum.min.js
--rw-r--r--   0        0        0     8060 2023-01-31 14:56:08.159411 pygenomeviz-0.3.2/src/pygenomeviz/viewer/assets/pgv-viewer.js
--rw-r--r--   0        0        0    10132 2023-01-31 14:56:08.159411 pygenomeviz-0.3.2/src/pygenomeviz/viewer/pgv-viewer-template.html
--rw-r--r--   0        0        0     1740 2023-01-31 14:56:08.159411 pygenomeviz-0.3.2/tests/conftest.py
--rw-r--r--   0        0        0     3958 2023-01-31 14:56:08.159411 pygenomeviz-0.3.2/tests/parser/test_genbank.py
--rw-r--r--   0        0        0     6439 2023-01-31 14:56:08.159411 pygenomeviz-0.3.2/tests/parser/test_gff.py
--rw-r--r--   0        0        0     3070 2023-01-31 14:56:08.159411 pygenomeviz-0.3.2/tests/test_feature.py
--rw-r--r--   0        0        0    11221 2023-01-31 14:56:08.159411 pygenomeviz-0.3.2/tests/test_genomeviz.py
--rw-r--r--   0        0        0     2544 2023-01-31 14:56:08.159411 pygenomeviz-0.3.2/tests/test_link.py
--rw-r--r--   0        0        0     2803 2023-01-31 14:56:08.159411 pygenomeviz-0.3.2/tests/test_scripts.py
--rw-r--r--   0        0        0     4448 2023-01-31 14:56:08.159411 pygenomeviz-0.3.2/tests/test_track.py
--rw-r--r--   0        0        0     1834 2023-01-31 14:56:08.159411 pygenomeviz-0.3.2/tests/test_utils.py
--rw-r--r--   0        0        0   115113 2023-01-31 14:56:08.159411 pygenomeviz-0.3.2/tests/testdata/genbank/test.gbff
--rw-r--r--   0        0        0    28102 2023-01-31 14:56:08.159411 pygenomeviz-0.3.2/tests/testdata/genbank/test.gbff.bz2
--rw-r--r--   0        0        0    34564 2023-01-31 14:56:08.159411 pygenomeviz-0.3.2/tests/testdata/genbank/test.gbff.gz
--rw-r--r--   0        0        0    33773 2023-01-31 14:56:08.159411 pygenomeviz-0.3.2/tests/testdata/genbank/test.zip
--rw-r--r--   0        0        0    36204 2023-01-31 14:56:08.159411 pygenomeviz-0.3.2/tests/testdata/gff/test.gff
--rw-r--r--   0        0        0     4409 2023-01-31 14:56:08.159411 pygenomeviz-0.3.2/tests/testdata/gff/test.gff.bz2
--rw-r--r--   0        0        0     5632 2023-01-31 14:56:08.159411 pygenomeviz-0.3.2/tests/testdata/gff/test.gff.gz
--rw-r--r--   0        0        0     5799 2023-01-31 14:56:08.159411 pygenomeviz-0.3.2/tests/testdata/gff/test.zip
--rw-r--r--   0        0        0    17527 1970-01-01 00:00:00.000000 pygenomeviz-0.3.2/setup.py
--rw-r--r--   0        0        0    16666 1970-01-01 00:00:00.000000 pygenomeviz-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-08-04 13:38:05.989622 pygenomeviz-0.4.0/LICENSE
+-rw-r--r--   0        0        0    16885 2023-08-04 13:38:05.989622 pygenomeviz-0.4.0/README.md
+-rw-r--r--   0        0        0     1972 2023-08-04 13:38:06.101624 pygenomeviz-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      883 2023-08-04 13:38:06.101624 pygenomeviz-0.4.0/src/pygenomeviz/__init__.py
+-rw-r--r--   0        0        0    23011 2023-08-04 13:38:06.101624 pygenomeviz-0.4.0/src/pygenomeviz/align.py
+-rw-r--r--   0        0        0     2411 2023-08-04 13:38:06.101624 pygenomeviz-0.4.0/src/pygenomeviz/config.py
+-rw-r--r--   0        0        0    20442 2023-08-04 13:38:06.101624 pygenomeviz-0.4.0/src/pygenomeviz/feature.py
+-rw-r--r--   0        0        0    27801 2023-08-04 13:38:06.101624 pygenomeviz-0.4.0/src/pygenomeviz/genomeviz.py
+-rw-r--r--   0        0        0        0 2023-08-04 13:38:06.101624 pygenomeviz-0.4.0/src/pygenomeviz/gui/__init__.py
+-rw-r--r--   0        0        0    12319 2023-08-04 13:38:06.101624 pygenomeviz-0.4.0/src/pygenomeviz/gui/app.py
+-rw-r--r--   0        0        0  1753383 2023-08-04 13:38:06.109624 pygenomeviz-0.4.0/src/pygenomeviz/gui/assets/pgv_demo.gif
+-rw-r--r--   0        0        0     1465 2023-08-04 13:38:06.109624 pygenomeviz-0.4.0/src/pygenomeviz/gui/config.py
+-rw-r--r--   0        0        0     4777 2023-08-04 13:38:06.109624 pygenomeviz-0.4.0/src/pygenomeviz/gui/plot.py
+-rw-r--r--   0        0        0     1202 2023-08-04 13:38:06.109624 pygenomeviz-0.4.0/src/pygenomeviz/gui/utils.py
+-rw-r--r--   0        0        0     7349 2023-08-04 13:38:06.109624 pygenomeviz-0.4.0/src/pygenomeviz/link.py
+-rw-r--r--   0        0        0      127 2023-08-04 13:38:06.109624 pygenomeviz-0.4.0/src/pygenomeviz/parser/__init__.py
+-rw-r--r--   0        0        0    18102 2023-08-04 13:38:06.109624 pygenomeviz-0.4.0/src/pygenomeviz/parser/genbank.py
+-rw-r--r--   0        0        0    17331 2023-08-04 13:38:06.109624 pygenomeviz-0.4.0/src/pygenomeviz/parser/gff.py
+-rw-r--r--   0        0        0     2991 2023-08-04 13:38:06.109624 pygenomeviz-0.4.0/src/pygenomeviz/scripts/__init__.py
+-rw-r--r--   0        0        0     1687 2023-08-04 13:38:06.109624 pygenomeviz-0.4.0/src/pygenomeviz/scripts/download_dataset.py
+-rw-r--r--   0        0        0     2081 2023-08-04 13:38:06.109624 pygenomeviz-0.4.0/src/pygenomeviz/scripts/gui.py
+-rw-r--r--   0        0        0    14780 2023-08-04 13:38:06.109624 pygenomeviz-0.4.0/src/pygenomeviz/scripts/mmseqs.py
+-rw-r--r--   0        0        0    16305 2023-08-04 13:38:06.109624 pygenomeviz-0.4.0/src/pygenomeviz/scripts/mummer.py
+-rw-r--r--   0        0        0    13064 2023-08-04 13:38:06.109624 pygenomeviz-0.4.0/src/pygenomeviz/scripts/pmauve.py
+-rw-r--r--   0        0        0     9598 2023-08-04 13:38:06.109624 pygenomeviz-0.4.0/src/pygenomeviz/scripts/simpleplot.py
+-rw-r--r--   0        0        0    33004 2023-08-04 13:38:06.109624 pygenomeviz-0.4.0/src/pygenomeviz/track.py
+-rw-r--r--   0        0        0     8206 2023-08-04 13:38:06.109624 pygenomeviz-0.4.0/src/pygenomeviz/utils.py
+-rw-r--r--   0        0        0     7090 2023-08-04 13:38:06.109624 pygenomeviz-0.4.0/src/pygenomeviz/viewer/assets/lib/images/ui-icons_444444_256x240.png
+-rw-r--r--   0        0        0     7074 2023-08-04 13:38:06.109624 pygenomeviz-0.4.0/src/pygenomeviz/viewer/assets/lib/images/ui-icons_555555_256x240.png
+-rw-r--r--   0        0        0     4618 2023-08-04 13:38:06.109624 pygenomeviz-0.4.0/src/pygenomeviz/viewer/assets/lib/images/ui-icons_777620_256x240.png
+-rw-r--r--   0        0        0     7111 2023-08-04 13:38:06.109624 pygenomeviz-0.4.0/src/pygenomeviz/viewer/assets/lib/images/ui-icons_777777_256x240.png
+-rw-r--r--   0        0        0     4618 2023-08-04 13:38:06.109624 pygenomeviz-0.4.0/src/pygenomeviz/viewer/assets/lib/images/ui-icons_cc0000_256x240.png
+-rw-r--r--   0        0        0     6487 2023-08-04 13:38:06.109624 pygenomeviz-0.4.0/src/pygenomeviz/viewer/assets/lib/images/ui-icons_ffffff_256x240.png
+-rw-r--r--   0        0        0    30801 2023-08-04 13:38:06.109624 pygenomeviz-0.4.0/src/pygenomeviz/viewer/assets/lib/jquery-ui.min.css
+-rw-r--r--   0        0        0   255079 2023-08-04 13:38:06.109624 pygenomeviz-0.4.0/src/pygenomeviz/viewer/assets/lib/jquery-ui.min.js
+-rw-r--r--   0        0        0    89664 2023-08-04 13:38:06.113624 pygenomeviz-0.4.0/src/pygenomeviz/viewer/assets/lib/jquery.min.js
+-rw-r--r--   0        0        0    10026 2023-08-04 13:38:06.113624 pygenomeviz-0.4.0/src/pygenomeviz/viewer/assets/lib/panzoom.min.js
+-rw-r--r--   0        0        0    10465 2023-08-04 13:38:06.113624 pygenomeviz-0.4.0/src/pygenomeviz/viewer/assets/lib/spectrum.min.css
+-rw-r--r--   0        0        0    27904 2023-08-04 13:38:06.113624 pygenomeviz-0.4.0/src/pygenomeviz/viewer/assets/lib/spectrum.min.js
+-rw-r--r--   0        0        0     6583 2023-08-04 13:38:06.113624 pygenomeviz-0.4.0/src/pygenomeviz/viewer/assets/pgv-viewer.js
+-rw-r--r--   0        0        0    10132 2023-08-04 13:38:06.113624 pygenomeviz-0.4.0/src/pygenomeviz/viewer/pgv-viewer-template.html
+-rw-r--r--   0        0        0     1740 2023-08-04 13:38:06.113624 pygenomeviz-0.4.0/tests/conftest.py
+-rw-r--r--   0        0        0     3959 2023-08-04 13:38:06.113624 pygenomeviz-0.4.0/tests/parser/test_genbank.py
+-rw-r--r--   0        0        0     6440 2023-08-04 13:38:06.113624 pygenomeviz-0.4.0/tests/parser/test_gff.py
+-rw-r--r--   0        0        0     3071 2023-08-04 13:38:06.113624 pygenomeviz-0.4.0/tests/test_feature.py
+-rw-r--r--   0        0        0    11268 2023-08-04 13:38:06.113624 pygenomeviz-0.4.0/tests/test_genomeviz.py
+-rw-r--r--   0        0        0     2545 2023-08-04 13:38:06.113624 pygenomeviz-0.4.0/tests/test_link.py
+-rw-r--r--   0        0        0     2804 2023-08-04 13:38:06.113624 pygenomeviz-0.4.0/tests/test_scripts.py
+-rw-r--r--   0        0        0     4450 2023-08-04 13:38:06.113624 pygenomeviz-0.4.0/tests/test_track.py
+-rw-r--r--   0        0        0     1835 2023-08-04 13:38:06.113624 pygenomeviz-0.4.0/tests/test_utils.py
+-rw-r--r--   0        0        0   115113 2023-08-04 13:38:06.113624 pygenomeviz-0.4.0/tests/testdata/genbank/test.gbff
+-rw-r--r--   0        0        0    28102 2023-08-04 13:38:06.113624 pygenomeviz-0.4.0/tests/testdata/genbank/test.gbff.bz2
+-rw-r--r--   0        0        0    34564 2023-08-04 13:38:06.113624 pygenomeviz-0.4.0/tests/testdata/genbank/test.gbff.gz
+-rw-r--r--   0        0        0    33773 2023-08-04 13:38:06.113624 pygenomeviz-0.4.0/tests/testdata/genbank/test.zip
+-rw-r--r--   0        0        0    36204 2023-08-04 13:38:06.113624 pygenomeviz-0.4.0/tests/testdata/gff/test.gff
+-rw-r--r--   0        0        0     4409 2023-08-04 13:38:06.113624 pygenomeviz-0.4.0/tests/testdata/gff/test.gff.bz2
+-rw-r--r--   0        0        0     5632 2023-08-04 13:38:06.113624 pygenomeviz-0.4.0/tests/testdata/gff/test.gff.gz
+-rw-r--r--   0        0        0     5799 2023-08-04 13:38:06.113624 pygenomeviz-0.4.0/tests/testdata/gff/test.zip
+-rw-r--r--   0        0        0    18020 1970-01-01 00:00:00.000000 pygenomeviz-0.4.0/PKG-INFO
```

### Comparing `pygenomeviz-0.3.2/LICENSE` & `pygenomeviz-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pygenomeviz-0.3.2/README.md` & `pygenomeviz-0.4.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -9,16 +9,18 @@
 
 ## Table of contents
 
 - [Overview](#overview)
 - [Installation](#installation)
 - [API Examples](#api-examples)
 - [CLI Examples](#cli-examples)
+- [GUI (Web browser)](#gui-web-browser)
 - [Interactive HTML Viewer](#interactive-html-viewer)
 - [Inspiration](#inspiration)
+- [Circular Genome Visualization](#circular-genome-visualization)
 
 ## Overview
 
 pyGenomeViz is a genome visualization python package for comparative genomics implemented based on matplotlib.
 This package is developed for the purpose of easily and beautifully plotting genomic
 features and sequence similarity comparison links between multiple genomes.
 It supports genome visualization of Genbank/GFF format file and can be saved figure in various formats (JPG/PNG/SVG/PDF/HTML).
@@ -26,30 +28,34 @@
 or automatic genome visualization figure plotting in genome analysis scripts/pipelines.
 
 For more information, please see full documentation [here](https://moshi4.github.io/pyGenomeViz/).
 
 ![pygenomeviz_gallery.png](https://raw.githubusercontent.com/moshi4/pyGenomeViz/main/docs/images/pygenomeviz_gallery.png)  
 **Fig.1 pyGenomeViz example plot gallery**
 
+:sparkles: GUI (Web browser) functionality is newly added from v0.4.0
+
+![pygenomeviz_gui.gif](https://raw.githubusercontent.com/moshi4/pyGenomeViz/main/src/pygenomeviz/gui/assets/pgv_demo.gif)
+**Fig.2 pyGenomeViz GUI (Web browser) version example**
+
 ## Installation
 
 `Python 3.8 or later` is required for installation.
 
 **Install PyPI package:**
 
     pip install pygenomeviz
 
 **Install bioconda package:**
 
     conda install -c conda-forge -c bioconda pygenomeviz
 
 **Use Docker ([Image Registry](https://github.com/moshi4/pyGenomeViz/pkgs/container/pygenomeviz)):**
 
-    docker pull ghcr.io/moshi4/pygenomeviz:latest
-    docker run -it --rm ghcr.io/moshi4/pygenomeviz:latest pgv-pmauve -h
+    docker run --rm -p 8501:8501 ghcr.io/moshi4/pygenomeviz:latest pgv-gui
 
 ## API Examples
 
 Jupyter notebooks containing code examples below is available [here](https://moshi4.github.io/pyGenomeViz/getting_started/).
 
 ### Basic Example
 
@@ -383,14 +389,22 @@
 > :warning: progressiveMauve must be installed in advance to run
 
     pgv-pmauve --seq_files NC_000913.gbk NC_002695.gbk NC_011751.gbk NC_011750.gbk \
                -o pmauve_example --tick_style bar
 
 ![pmauve_example.png](https://raw.githubusercontent.com/moshi4/pyGenomeViz/main/docs/images/pmauve_example1.png)  
 
+## GUI (Web browser)
+
+pyGenomeViz implements GUI (Web browser) functionality using [Streamlit](https://github.com/streamlit/streamlit) as an option.
+Users can easily perform data visualization of Genbank files and genome comparison
+results using MUMmer or MMseqs. See [pgv-gui document](https://moshi4.github.io/pyGenomeViz/gui-docs/pgv-gui/) for details.
+
+![pygenomeviz_gui.gif](https://raw.githubusercontent.com/moshi4/pyGenomeViz/main/src/pygenomeviz/gui/assets/pgv_demo.gif)
+
 ## Interactive HTML Viewer
 
 pyGenomeViz implements HTML file output functionality for interactive data visualization.
 In API, HTML file can be output using `savefig_html` method. In CLI, user can select HTML file output option.
 As shown below, data tooltip display, pan/zoom, object color change, text change, etc are available in HTML viewer
 ([Demo Page](https://moshi4.github.io/pyGenomeViz/images/pgv-viewer-demo.html)).
 
@@ -400,7 +414,15 @@
 
 pyGenomeViz was inspired by
 
 - [GenomeDiagram (BioPython)](https://github.com/biopython/biopython)
 - [Easyfig](http://mjsull.github.io/Easyfig/)
 - [genoplotR](https://genoplotr.r-forge.r-project.org/)
 - [gggenomes](https://github.com/thackl/gggenomes)
+
+## Circular Genome Visualization
+
+pyGenomeViz is a python package designed for linear genome visualization.
+If you are interested in circular genome visualization, check out my other python package [pyCirclize](https://github.com/moshi4/pyCirclize).
+
+![pycirclize_example.png](https://raw.githubusercontent.com/moshi4/pyGenomeViz/main/docs/images/pycirclize_example.png)  
+**Fig. pyCirclize example plot gallery**
```

### Comparing `pygenomeviz-0.3.2/src/pygenomeviz/__init__.py` & `pygenomeviz-0.4.0/src/pygenomeviz/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from pygenomeviz.genomeviz import GenomeViz
 from pygenomeviz.parser import Genbank, Gff
 from pygenomeviz.utils import load_dataset, load_example_gff
 
 warnings.filterwarnings("ignore")
 
-__version__ = "0.3.2"
+__version__ = "0.4.0"
 
 __all__ = [
     "GenomeViz",
     "Genbank",
     "Gff",
     "load_dataset",
     "load_example_gff",
```

### Comparing `pygenomeviz-0.3.2/src/pygenomeviz/align.py` & `pygenomeviz-0.4.0/src/pygenomeviz/align.py`

 * *Files 1% similar despite different names*

```diff
@@ -155,16 +155,21 @@
         mp_data_list: list[tuple[Path, Path, int]] = []
         for idx in range(0, self.genome_num - 1):
             fa_file1 = self._genome_fasta_files[idx]
             fa_file2 = self._genome_fasta_files[idx + 1]
             mp_data_list.append((fa_file1, fa_file2, idx))
 
         # Run MUMmer with multiprocessing
-        with mp.Pool(processes=self.process_num) as p:
-            results = p.starmap(self._run_mummer, mp_data_list)
+        if self.process_num > 1:
+            with mp.Pool(processes=self.process_num) as p:
+                results = p.starmap(self._run_mummer, mp_data_list)
+        else:
+            results = []
+            for fa_file1, fa_file2, idx in mp_data_list:
+                results.append(self._run_mummer(fa_file1, fa_file2, idx))
 
         align_coords = list(itertools.chain.from_iterable(results))
 
         # Add min_range to start, end coordinates
         gbk_name2min_range = {gbk.name: gbk.min_range for gbk in self.gbk_resources}
         for ac in align_coords:
             ac.ref_start = ac.ref_start + gbk_name2min_range[ac.ref_name]
@@ -209,15 +214,15 @@
         cmd = f"show-coords -H -T -r -k {filter_delta_file} > {coords_file}"
         _ = sp.run(cmd, shell=True, capture_output=True, text=True)
 
         align_coords = self.parse_coords_file(coords_file, self.seqtype)
 
         # Delete work files
         for work_file in (delta_file, filter_delta_file, coords_file):
-            os.unlink(work_file)
+            work_file.unlink(missing_ok=True)
 
         return align_coords
 
     @staticmethod
     def parse_coords_file(
         coords_tsv_file: str | Path,
         seqtype,
@@ -275,41 +280,45 @@
     def __init__(
         self,
         gbk_resources: list[str | Path] | list[Genbank],
         outdir: str | Path,
         identity: float = 0,
         evalue: float = 1e-3,
         process_num: int | None = None,
+        quiet: bool = False,
     ):
         """
         Parameters
         ----------
         gbk_resources : list[str | Path] | list[Genbank]
             Genome sequence genbank files or Genbank objects
         outdir : str | Path
             Output directory
         identity : float, optional
             Identity threshold
         evalue : float, optional
             E-value threshold
         process_num : int | None, optional
             Use processor number (Default: `'Max Processor' - 1`)
+        quiet : bool, optional
+            If True, do not print message
         """
         self.check_installation()
 
         self.gbk_list: list[Genbank] = []
         for gr in gbk_resources:
             if isinstance(gr, Genbank):
                 self.gbk_list.append(gr)
             else:
                 self.gbk_list.append(Genbank(gr))
         self.outdir = Path(outdir)
         self.identity = identity
         self.evalue = evalue
         self.process_num = self.max_process_num if process_num is None else process_num
+        self.quiet = quiet
 
         os.makedirs(self.outdir, exist_ok=True)
 
     def run(self) -> list[AlignCoord]:
         """Run genome alignment
 
         Returns
@@ -330,15 +339,16 @@
 
             with tempfile.TemporaryDirectory() as tmpdir:
                 name1 = fa_file1.with_suffix("").name
                 name2 = fa_file2.with_suffix("").name
                 rbh_result_file = self.outdir / f"{idx+1:02d}_{name1}-{name2}_rbh.tsv"
                 cmd = f"mmseqs easy-rbh {fa_file1} {fa_file2} {rbh_result_file} "
                 cmd += f"{tmpdir} --threads {self.process_num} -e {self.evalue} -v 0"
-                print(f"# {idx+1:02d}: {name1}-{name2} RBH search\n$ {cmd}\n")
+                if not self.quiet:
+                    print(f"# {idx+1:02d}: {name1}-{name2} RBH search\n$ {cmd}\n")
                 sp.run(cmd, shell=True)
 
                 align_coords.extend(
                     self.parse_rbh_result(rbh_result_file, name1, name2)
                 )
 
         return align_coords
```

### Comparing `pygenomeviz-0.3.2/src/pygenomeviz/config.py` & `pygenomeviz-0.4.0/src/pygenomeviz/config.py`

 * *Files identical despite different names*

### Comparing `pygenomeviz-0.3.2/src/pygenomeviz/feature.py` & `pygenomeviz-0.4.0/src/pygenomeviz/feature.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from __future__ import annotations
 
+import textwrap
+import uuid
 from copy import deepcopy
 from dataclasses import dataclass
 from typing import Any, get_args
 
 from Bio.SeqFeature import SeqFeature
 from matplotlib.axes import Axes
 from matplotlib.patches import FancyArrow, PathPatch, Rectangle
@@ -30,16 +32,18 @@
     labelvpos: LiteralTypes.LABELVPOS = "strand"
     labelhpos: LiteralTypes.LABELHPOS = "center"
     labelha: LiteralTypes.LABELHA = "left"
     arrow_shaft_ratio: float = 0.5
     size_ratio: float = 0.9
     patch_kws: dict[str, Any] | None = None
     seq_feature: SeqFeature | None = None
+    tooltip: str | None = None
 
     def __post_init__(self):
+        self._uuid = uuid.uuid4()
         # start-end value for HTML display
         self._display_start = self.start
         self._display_end = self.end
         # Change unknown strand value to 1
         if self.strand not in (1, -1):
             self.strand = 1
         # Check start, end postion
@@ -67,14 +71,39 @@
             err_msg += f"({self.arrow_shaft_ratio=})"
             raise ValueError(err_msg)
         # Check size ratio
         if not 0 <= self.size_ratio <= 1:
             err_msg = f"'size_ratio' must be '0 <= value <= 1' ({self.size_ratio=})"
             raise ValueError(err_msg)
 
+        self._set_tooltip()
+
+    ############################################################
+    # Property
+    ############################################################
+
+    @property
+    def gid(self) -> str:
+        """Group ID"""
+        return "Feature-" + str(self._uuid)
+
+    @property
+    def length(self) -> int:
+        """Feature length"""
+        return self.end - self.start
+
+    @property
+    def is_bigstyle(self) -> bool:
+        """Check plotstyle is 'big~~~' or not"""
+        return self.plotstyle.startswith("big")
+
+    ############################################################
+    # Public Method
+    ############################################################
+
     def plot_feature(
         self, ax: Axes, max_track_size: int, ylim: tuple[float, float]
     ) -> None:
         """Plot feature
 
         Parameters
         ----------
@@ -109,48 +138,51 @@
         ylim : tuple[float, float]
             Y-axis limit
         """
         if self.label != "" and self.labelsize != 0:
             start, end = self.start, self.end
             ax.text(**self._label_kwargs(start, end, self.label, ylim))
 
-    @property
-    def length(self) -> int:
-        """Feature length"""
-        return self.end - self.start
-
-    @property
-    def is_bigstyle(self) -> bool:
-        """Check plotstyle is 'big~~~' or not"""
-        return self.plotstyle.startswith("big")
-
-    @property
-    def gid(self) -> str:
-        """Group ID"""
-        start, end = self._display_start, self._display_end
-        type, gene, protein_id, product = "na", "na", "na", "na"
-        if self.seq_feature is not None:
+    ############################################################
+    # Private Method
+    ############################################################
+
+    def _set_tooltip(self) -> None:
+        """Set tooltip"""
+        # Skip if tooltip already exists
+        if self.tooltip is not None:
+            return
+        strand = "-" if self.strand == -1 else "+"
+        if self.seq_feature is None:
+            # Set basic tooltip
+            self.tooltip = textwrap.dedent(
+                f"""
+                location: {self._display_start:,} - {self._display_end:,} ({strand})
+                length: {self.length:,}
+                """
+            )[1:-1]
+        else:
+            # Set detail tooltip from SeqFeature info
             type = self.seq_feature.type
             qualifiers = self.seq_feature.qualifiers
             gene = qualifiers.get("gene", ["na"])[0]
-            protein_id = qualifiers.get("protein_id", ["na"])[0].split(".")[0]
+            protein_id = qualifiers.get("protein_id", ["na"])[0]
             product = qualifiers.get("product", ["na"])[0]
             if product == "na":
                 product = qualifiers.get("Name", ["na"])[0]
-            # Replace special characters to underscore (For html ID tag selection)
-            trans_dict = {e: "_" for e in list(" /:;()+.,'`\"\\!|^~[]{}<>#$%&@?=")}
-            trans_table = str.maketrans(trans_dict)
-            gene = gene.translate(trans_table)
-            protein_id = protein_id.translate(trans_table)
-            product = product.translate(trans_table)
-
-        return (
-            f"Feature_{start}_{end}_{self.strand}_"
-            + f"type_{type}_gene_{gene}_protein_id_{protein_id}_product_{product}"
-        )
+            self.tooltip = textwrap.dedent(
+                f"""
+                location: {self._display_start:,} - {self._display_end:,} ({strand})
+                length: {self.length:,}
+                type: {type}
+                gene: {gene}
+                protein_id: {protein_id}
+                product: {product}
+                """
+            )[1:-1]
 
     def _box_patch(self, start: int, end: int, ylim: tuple[float, float]) -> Rectangle:
         """Box patch
 
         Parameters
         ----------
         start : int
@@ -302,23 +334,24 @@
 
         Returns
         -------
         patch_kwargs : dict[str, Any]
             Patch keyword arguments dict
         """
         patch_kws = {} if self.patch_kws is None else self.patch_kws
-        return {
-            "fc": self.facecolor,
-            "ec": self.edgecolor,
-            "lw": self.linewidth,
-            "clip_on": False,
-            "zorder": 5 if self.is_bigstyle else -5,
-            "gid": self.gid,
-            **patch_kws,
-        }
+        zorder = 5 if self.is_bigstyle else -5
+        default_kwargs = dict(
+            fc=self.facecolor,
+            ec=self.edgecolor,
+            lw=self.linewidth,
+            clip_on=False,
+            zorder=zorder,
+            gid=self.gid,
+        )
+        return {**default_kwargs, **patch_kws}
 
     def _label_kwargs(
         self, start: int, end: int, label: str, ylim: tuple[float, float]
     ) -> dict[str, Any]:
         """Label keyword arguments dict
 
         Parameters
@@ -370,26 +403,26 @@
                 y = 0
             else:
                 y = (abs(ylim[0]) / 2) * self.strand
 
         # labelrotation=90, labelha="center", rotation_mode="default" is best
         rotation_mode = "default" if self.labelrotation == 90 else "anchor"
 
-        return {
-            "x": x,
-            "y": y,
-            "s": label,
-            "color": self.labelcolor,
-            "fontsize": self.labelsize,
-            "rotation": labelrotation,
-            "ha": self.labelha,
-            "va": labelva,
-            "zorder": 10,
-            "rotation_mode": rotation_mode,
-        }
+        return dict(
+            x=x,
+            y=y,
+            s=label,
+            color=self.labelcolor,
+            fontsize=self.labelsize,
+            rotation=labelrotation,
+            ha=self.labelha,
+            va=labelva,
+            zorder=10,
+            rotation_mode=rotation_mode,
+        )
 
     def __add__(self, offset: int):
         feature = deepcopy(self)
         feature.start += offset
         feature.end += offset
         return feature
 
@@ -446,14 +479,35 @@
             seq_feature,
         )
 
         if exon_labels is not None and len(exon_regions) != len(exon_labels):
             err_msg = "'exon_regions' & 'exon_labels' length is diffrent."
             raise ValueError(err_msg)
 
+    ############################################################
+    # Property
+    ############################################################
+
+    @property
+    def intron_regions(self) -> list[tuple[int, int]]:
+        """Intron regions"""
+        intron_regions = []
+        if len(self.exon_regions) > 1:
+            for i in range(0, len(self.exon_regions) - 1):
+                intron_start = self.exon_regions[i][1]
+                intron_end = self.exon_regions[i + 1][0]
+                if intron_end < intron_start:
+                    continue
+                intron_regions.append((intron_start, intron_end))
+        return intron_regions
+
+    ############################################################
+    # Public Method
+    ############################################################
+
     def plot_feature(
         self, ax: Axes, max_track_size: int, ylim: tuple[float, float]
     ) -> None:
         """Plot feature
 
         Parameters
         ----------
@@ -463,15 +517,15 @@
             Max track size
         ylim : tuple[float, float]
             Y-axis limit
         """
         ylim = (ylim[0] * self.size_ratio, ylim[1] * self.size_ratio)
 
         # Plot intron feature
-        for (start, end) in self.intron_regions:
+        for start, end in self.intron_regions:
             p = self._intron_patch(start, end, ylim)
             ax.add_patch(p)
 
         # Plot exon feature
         exon_regions = self.exon_regions[:: self.strand]
         for idx, (start, end) in enumerate(exon_regions, 1):
             if self.plotstyle in ("bigbox", "box"):
@@ -499,31 +553,22 @@
         if self.exon_labels is not None:
             for (start, end), label in zip(self.exon_regions, self.exon_labels):
                 if label != "" and self.labelsize != 0:
                     label_kwargs = self._label_kwargs(start, end, label, ylim)
                     label_kwargs.update(self.exon_label_kws)
                     ax.text(**label_kwargs)
 
-    @property
-    def intron_regions(self) -> list[tuple[int, int]]:
-        """Intron regions"""
-        intron_regions = []
-        if len(self.exon_regions) > 1:
-            for i in range(0, len(self.exon_regions) - 1):
-                intron_start = self.exon_regions[i][1]
-                intron_end = self.exon_regions[i + 1][0]
-                if intron_end < intron_start:
-                    continue
-                intron_regions.append((intron_start, intron_end))
-        return intron_regions
+    ############################################################
+    # Private Method
+    ############################################################
 
     def _check_exon_regions(self) -> None:
         """Check exon_regions values are properly set"""
         max_pos_record = None
-        for (exon_start, exon_end) in self.exon_regions:
+        for exon_start, exon_end in self.exon_regions:
             if exon_start >= exon_end:
                 err_msg = "Exon start-end value must be 'start < end'."
                 raise ValueError(err_msg)
             if max_pos_record is not None and exon_start < max_pos_record:
                 err_msg = "Set exon regions in ascending order of genomic position."
                 raise ValueError(err_msg)
             max_pos_record = exon_end
@@ -569,26 +614,22 @@
         """Intron patch keyword arguments dict
 
         Returns
         -------
         intron_patch_kwargs : dict[str, Any]
             Intron patch keyword arguments dict
         """
-        return {
-            "lw": 1,
-            "fill": False,
-            "clip_on": False,
-            "zorder": 5 if self.is_bigstyle else -5,
-            **self.intron_patch_kws,
-        }
+        zorder = 5 if self.is_bigstyle else -5
+        default_kwargs = dict(lw=1, fill=False, clip_on=False, zorder=zorder)
+        return {**default_kwargs, **self.intron_patch_kws}
 
     def __add__(self, offset: int):
         feature = deepcopy(self)
         # Add offset to start & end
         feature.start += offset
         feature.end += offset
         # Add offset to exon regions
         exon_regions = []
-        for (exon_start, exon_end) in feature.exon_regions:
+        for exon_start, exon_end in feature.exon_regions:
             exon_regions.append((exon_start + offset, exon_end + offset))
         feature.exon_regions = exon_regions
         return feature
```

### Comparing `pygenomeviz-0.3.2/src/pygenomeviz/genomeviz.py` & `pygenomeviz-0.4.0/src/pygenomeviz/genomeviz.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 import datetime
 import io
-from abc import ABCMeta, abstractmethod
+import json
 from pathlib import Path
 from typing import Any, get_args
 
 import matplotlib.pyplot as plt
 from matplotlib import colors, gridspec
 from matplotlib.axes import Axes
 from matplotlib.colorbar import Colorbar
@@ -15,16 +15,16 @@
 
 import pygenomeviz
 from pygenomeviz.config import ASSETS_FILES, TEMPLATE_HTML_FILE, LiteralTypes
 from pygenomeviz.link import Link
 from pygenomeviz.track import FeatureSubTrack, FeatureTrack, LinkTrack, TickTrack, Track
 
 
-class GenomeVizBase(metaclass=ABCMeta):
-    """GenomeViz Abstract Base Class"""
+class GenomeViz:
+    """GenomeViz Class"""
 
     def __init__(
         self,
         fig_width: float = 15,
         fig_track_height: float = 1.0,
         align_type: LiteralTypes.ALIGN_TYPE = "left",
         feature_track_ratio: float = 1.0,
@@ -72,152 +72,17 @@
         self.tick_style = tick_style
         self.plot_size_thr = plot_size_thr
         self.tick_labelsize = tick_labelsize
         self._tracks: list[Track] = []
 
         self._check_init_values()
 
-    def _check_init_values(self) -> None:
-        """Check initial values"""
-        if self.align_type not in get_args(LiteralTypes.ALIGN_TYPE):
-            err_msg = f"{self.align_type=} is invalid."
-            raise ValueError(err_msg)
-
-        if self.tick_style not in get_args(LiteralTypes.TICK_STYLE):
-            err_msg = f"{self.tick_style=} is invalid."
-            raise ValueError(err_msg)
-
-    def _get_track_offset(self, track: Track) -> int:
-        """Get track offset
-
-        Parameters
-        ----------
-        track : Track
-            Target track offset for alignment
-
-        Returns
-        -------
-        track_offset : int
-            Track offset
-        """
-        if self.align_type == "left":
-            return 0
-        elif self.align_type == "center":
-            return int((self.max_track_size - track.size) / 2)
-        elif self.align_type == "right":
-            return self.max_track_size - track.size
-        else:
-            raise NotImplementedError
-
-    @property
-    def _track_name2link_offset(self) -> dict[str, int]:
-        """Track name & link offset dict"""
-        track_name2offset = {}
-        for track in self.get_feature_tracks():
-            track_name2offset[track.name] = self._get_track_offset(track) - track.start
-        return track_name2offset
-
-    def _get_link_track(
-        self, feature_track_name1: str, feature_track_name2: str
-    ) -> LinkTrack:
-        """Get link track from two adjacent feature track names
-
-        Parameters
-        ----------
-        feature_track_name1 : str
-            Feature track name1
-        feature_track_name2 : str
-            Feature track name2
-
-        Returns
-        -------
-        link_track : LinkTrack
-            Target link track
-        """
-        track_names = [t.name for t in self.get_tracks()]
-        feature_track_idx1 = track_names.index(feature_track_name1)
-        feature_track_idx2 = track_names.index(feature_track_name2)
-        if abs(feature_track_idx1 - feature_track_idx2) == 2:
-            link_track_idx = int((feature_track_idx1 + feature_track_idx2) / 2)
-            target_link_track = self.get_tracks()[link_track_idx]
-            if isinstance(target_link_track, LinkTrack):
-                return target_link_track
-            else:
-                err_msg = "LinkTrack is not found between target feature tracks "
-                err_msg += f"({feature_track_name1=}, {feature_track_name2=})"
-                raise ValueError(err_msg)
-        else:
-            err_msg = f"{feature_track_name1=} and {feature_track_name2=} "
-            err_msg += "are not adjacent feature tracks."
-            raise ValueError(err_msg)
-
-    @abstractmethod
-    def add_feature_track():
-        """Add feature track"""
-        raise NotImplementedError
-
-    @abstractmethod
-    def add_link():
-        """Add link track"""
-        raise NotImplementedError
-
-    def get_track(self, track_name: str) -> Track:
-        """Get track by name
-
-        Parameters
-        ----------
-        track_name : str
-            Target track name
-
-        Returns
-        -------
-        track : Track
-            Target track
-        """
-        name2track = {t.name: t for t in self.get_tracks()}
-        track_names = name2track.keys()
-        if track_name not in track_names:
-            err_msg = f"{track_name=} is not found ({track_names=})."
-            raise ValueError(err_msg)
-        return name2track[track_name]
-
-    def get_tracks(self, subtrack: bool = False) -> list[Track]:
-        """Get tracks
-
-        Parameters
-        ----------
-        subtrack : bool, optional
-            If True, include feature subtracks
-
-        Returns
-        -------
-        tracks : list[Track]
-            Track list
-        """
-        tracks = []
-        for track in self._tracks:
-            if isinstance(track, FeatureTrack):
-                if subtrack:
-                    tracks.extend([t for t in track.subtracks if t.position == "above"])
-                tracks.append(track)
-                if subtrack:
-                    tracks.extend([t for t in track.subtracks if t.position == "below"])
-            else:
-                tracks.append(track)
-        return tracks
-
-    def get_feature_tracks(self) -> list[FeatureTrack]:
-        """Get feature tracks
-
-        Returns
-        -------
-        feature_tracks : list[FeatureTrack]
-            Feature track list
-        """
-        return [t for t in self.get_tracks() if isinstance(t, FeatureTrack)]
+    ############################################################
+    # Property
+    ############################################################
 
     @property
     def top_track(self) -> FeatureTrack:
         """Top feature track"""
         feature_tracks = self.get_feature_tracks()
         if len(feature_tracks) == 0:
             err_msg = "No track found. Can't access 'top_track' property."
@@ -237,149 +102,43 @@
     def max_track_size(self) -> int:
         """Max track size"""
         if len(self.get_tracks()) == 0:
             err_msg = "No track found. Can't access 'max_track_size' property."
             raise ValueError(err_msg)
         return max([track.size for track in self.get_tracks()])
 
-    @abstractmethod
-    def plotfig(self, dpi: int = 100) -> Figure:
-        """Plot figure"""
-        raise NotImplementedError
-
-    def savefig(
-        self,
-        savefile: str | Path,
-        dpi: int = 100,
-        pad_inches: float = 0.5,
-    ) -> None:
-        """Save figure to file
-
-        Parameters
-        ----------
-        savefile : str | Path
-            Save file
-        dpi : int, optional
-            DPI
-        pad_inches : float, optional
-            Padding inches
-        """
-        figure = self.plotfig(dpi=dpi)
-        figure.savefig(
-            fname=savefile,
-            dpi=dpi,
-            pad_inches=pad_inches,
-            bbox_inches="tight",
-        )
-
-    def print_tracks_info(self, detail=False) -> None:
-        """Print tracks info (Mainly for debugging work)
-
-        Parameters
-        ----------
-        detail : bool, optional
-            If True, also output feature and link details
-        """
-        for idx, track in enumerate(self.get_tracks(subtrack=True), 1):
-            # Print track common info
-            class_name = track.__class__.__name__
-            print(f"\n# Track{idx:02d}: Name='{track.name}' ({class_name})")
-            size, ratio, zorder = track.size, track.ratio, track.zorder
-            print(f"# Size={size}, Ratio={ratio}, Zorder={zorder}", end="")
-
-            # Print each track specific info
-            if isinstance(track, FeatureTrack):
-                print(f", FeatureNumber={len(track.features)}")
-                if detail:
-                    for feature in track.features:
-                        print(feature)
-            elif isinstance(track, FeatureSubTrack):
-                print()
-            elif isinstance(track, LinkTrack):
-                print(f", LinkNumber={len(track.links)}")
-                if detail:
-                    for link in track.links:
-                        print(link)
-            elif isinstance(track, TickTrack):
-                print()
-
-    def set_colorbar(
-        self,
-        figure: Figure,
-        bar_colors: list[str] = ["grey", "red"],
-        alpha: float = 0.8,
-        vmin: float = 0,
-        vmax: float = 100,
-        bar_height: float = 0.2,
-        bar_width: float = 0.01,
-        bar_left: float = 1.02,
-        bar_bottom: float = 0,
-        bar_label: str = "",
-        bar_labelsize: float = 15,
-        tick_labelsize: float = 10,
-    ) -> None:
-        """Set colorbars to figure
-
-        Set colorbars for similarity links between genome tracks
-
-        Parameters
-        ----------
-        figure : Figure
-            Matplotlib figure
-        bar_colors : list[str], optional
-            Bar color list
-        alpha : float, optional
-            Color transparency
-        vmin : float, optional
-            Colorbar min value
-        vmax : float, optional
-            Colorbar max value
-        bar_height : float, optional
-            Colorbar height
-        bar_width : float, optional
-            Colorbar width
-        bar_left : float, optional
-            Colorbar left position
-        bar_bottom : float, optional
-            Colorbar bottom position
-        bar_label : str, optional
-            Colorbar label name
-        bar_labelsize : float, optional
-            Colorbar label size
-        tick_labelsize : float, optional
-            Colorbar tick label size
-        """
-        if bar_height == 0 or bar_width == 0:
-            return
-        bar_colors = list(dict.fromkeys([colors.to_hex(c) for c in bar_colors]))
-        for cnt, color in enumerate(bar_colors):
-            left = bar_left + bar_width * cnt
-            cbar_ax = figure.add_axes([left, bar_bottom, bar_width, bar_height])
-
-            def to_nearly_white(color: str, nearly_value: float = 0.1) -> str:
-                """Convert target color to nearly white"""
-                cmap = colors.LinearSegmentedColormap.from_list("m", ("white", color))
-                return colors.to_hex(cmap(nearly_value))
-
-            nearly_white = to_nearly_white(color)
-            cmap = colors.LinearSegmentedColormap.from_list("m", (nearly_white, color))
-            norm = colors.Normalize(vmin=vmin, vmax=vmax)
-            cb_kws = {"orientation": "vertical", "ticks": []}
-            cb = Colorbar(cbar_ax, cmap=cmap, norm=norm, alpha=alpha, **cb_kws)
-            if cnt == len(bar_colors) - 1:
-                ticks = [vmin, vmax]
-                labels = [f"{t}%" for t in ticks]
-                cb.set_ticks(ticks, labels=labels, fontsize=tick_labelsize)
-                x, y = 2.0, (vmin + vmax) / 2
-                text_kws = {"rotation": 90, "ha": "left", "va": "center"}
-                cbar_ax.text(x, y, bar_label, size=bar_labelsize, **text_kws)
+    @property
+    def track_name2link_offset(self) -> dict[str, int]:
+        """Track name & link offset dict"""
+        track_name2offset = {}
+        for track in self.get_feature_tracks():
+            track_name2offset[track.name] = self._get_track_offset(track) - track.start
+        return track_name2offset
 
+    @property
+    def gid2feature_tooltip(self) -> dict[str, str]:
+        """Group ID & feature tooltip dict"""
+        gid2feature_tooltip = {}
+        for track in self.get_feature_tracks():
+            for feature in track.features:
+                gid2feature_tooltip[feature.gid] = feature.tooltip
+        return gid2feature_tooltip
 
-class GenomeViz(GenomeVizBase):
-    """GenomeViz Class"""
+    @property
+    def gid2link_tooltip(self) -> dict[str, str]:
+        """Group ID & link tooltip dict"""
+        gid2link_tooltip = {}
+        for track in self.get_link_tracks():
+            for link in track.links:
+                gid2link_tooltip[link.gid] = link.tooltip
+        return gid2link_tooltip
+
+    ############################################################
+    # Public Method
+    ############################################################
 
     def add_feature_track(
         self,
         name: str,
         size: int,
         start_pos: int = 0,
         labelsize: int = 20,
@@ -536,14 +295,151 @@
                 vmax,
                 curve,
                 size_ratio,
                 patch_kws,
             )
         )
 
+    def get_track(self, track_name: str) -> Track:
+        """Get track by name
+
+        Parameters
+        ----------
+        track_name : str
+            Target track name
+
+        Returns
+        -------
+        track : Track
+            Target track
+        """
+        name2track = {t.name: t for t in self.get_tracks()}
+        track_names = name2track.keys()
+        if track_name not in track_names:
+            err_msg = f"{track_name=} is not found ({track_names=})."
+            raise ValueError(err_msg)
+        return name2track[track_name]
+
+    def get_tracks(self, subtrack: bool = False) -> list[Track]:
+        """Get tracks
+
+        Parameters
+        ----------
+        subtrack : bool, optional
+            If True, include feature subtracks
+
+        Returns
+        -------
+        tracks : list[Track]
+            Track list
+        """
+        tracks = []
+        for track in self._tracks:
+            if isinstance(track, FeatureTrack):
+                if subtrack:
+                    tracks.extend([t for t in track.subtracks if t.position == "above"])
+                tracks.append(track)
+                if subtrack:
+                    tracks.extend([t for t in track.subtracks if t.position == "below"])
+            else:
+                tracks.append(track)
+        return tracks
+
+    def get_feature_tracks(self) -> list[FeatureTrack]:
+        """Get feature tracks
+
+        Returns
+        -------
+        feature_tracks : list[FeatureTrack]
+            Feature track list
+        """
+        return [t for t in self.get_tracks() if isinstance(t, FeatureTrack)]
+
+    def get_link_tracks(self) -> list[LinkTrack]:
+        """Get link tracks
+
+        Returns
+        -------
+        link_tracks : list[LinkTrack]
+            Link track list
+        """
+        return [t for t in self.get_tracks() if isinstance(t, LinkTrack)]
+
+    def set_colorbar(
+        self,
+        figure: Figure,
+        bar_colors: list[str] | None = None,
+        alpha: float = 0.8,
+        vmin: float = 0,
+        vmax: float = 100,
+        bar_height: float = 0.2,
+        bar_width: float = 0.01,
+        bar_left: float = 1.02,
+        bar_bottom: float = 0,
+        bar_label: str = "",
+        bar_labelsize: float = 15,
+        tick_labelsize: float = 10,
+    ) -> None:
+        """Set colorbars to figure
+
+        Set colorbars for similarity links between genome tracks
+
+        Parameters
+        ----------
+        figure : Figure
+            Matplotlib figure
+        bar_colors : list[str] | None, optional
+            Bar color list
+        alpha : float, optional
+            Color transparency
+        vmin : float, optional
+            Colorbar min value
+        vmax : float, optional
+            Colorbar max value
+        bar_height : float, optional
+            Colorbar height
+        bar_width : float, optional
+            Colorbar width
+        bar_left : float, optional
+            Colorbar left position
+        bar_bottom : float, optional
+            Colorbar bottom position
+        bar_label : str, optional
+            Colorbar label name
+        bar_labelsize : float, optional
+            Colorbar label size
+        tick_labelsize : float, optional
+            Colorbar tick label size
+        """
+        if bar_height == 0 or bar_width == 0:
+            return
+        bar_colors = ["grey", "red"] if bar_colors is None else bar_colors
+        bar_colors = list(dict.fromkeys([colors.to_hex(c) for c in bar_colors]))
+        for cnt, color in enumerate(bar_colors):
+            left = bar_left + bar_width * cnt
+            cbar_ax = figure.add_axes([left, bar_bottom, bar_width, bar_height])
+
+            def to_nearly_white(color: str, nearly_value: float = 0.1) -> str:
+                """Convert target color to nearly white"""
+                cmap = colors.LinearSegmentedColormap.from_list("m", ("white", color))
+                return colors.to_hex(cmap(nearly_value))
+
+            nearly_white = to_nearly_white(color)
+            cmap = colors.LinearSegmentedColormap.from_list("m", (nearly_white, color))
+            norm = colors.Normalize(vmin=vmin, vmax=vmax)
+            cb_kws = {"orientation": "vertical", "ticks": []}
+            cb = Colorbar(cbar_ax, cmap=cmap, norm=norm, alpha=alpha, **cb_kws)
+            if cnt == len(bar_colors) - 1:
+                ticks = [vmin, vmax]
+                labels = [f"{t}%" for t in ticks]
+                cb.set_ticks(ticks, labels=labels, fontsize=tick_labelsize)
+                x, y = 2.0, (vmin + vmax) / 2
+                text_kws = {"rotation": 90, "ha": "left", "va": "center"}
+                cbar_ax.text(x, y, bar_label, size=bar_labelsize, **text_kws)
+
     def plotfig(self, dpi: int = 100) -> Figure:
         """Plot figure
 
         Parameters
         ----------
         dpi : int, optional
             DPI
@@ -570,15 +466,15 @@
                 )
             )
 
         # Set figure
         track_num = len(self.get_tracks(subtrack=True))
         figsize = (self.fig_width, self.fig_track_height * track_num)
         tight_layout = False if track_num < 3 else True
-        figure: Figure = plt.figure(
+        figure: Figure = plt.figure(  # type: ignore
             figsize=figsize, facecolor="white", dpi=dpi, tight_layout=tight_layout
         )
 
         # Set gridspec
         height_ratios = [t.ratio for t in self.get_tracks(subtrack=True)]
         gs = gridspec.GridSpec(nrows=track_num, ncols=1, height_ratios=height_ratios)
         gs.update(left=0, right=1, bottom=0, top=1, hspace=0, wspace=0)
@@ -595,15 +491,15 @@
                 raise TypeError("Error: Not matplotlib Axes class instance.")
             ax.set_gid(f"{track.__class__.__name__}{idx:02d}")
             track_offset = self._get_track_offset(track)
             track._ax, track._offset = ax, track_offset
             # Set 'spines' and 'ticks' visibility
             for spine, display in track.spines_params.items():
                 ax.spines[spine].set_visible(display)
-            ax.tick_params(**track.tick_params)
+            ax.tick_params(**track.tick_params)  # type: ignore
 
             if isinstance(track, FeatureTrack):
                 ax.set_gid(str(ax.get_gid()) + f" {track})")
                 # Plot track scale line
                 xmin, xmax = track_offset, track.size + track_offset
                 ax.hlines(0, xmin, xmax, track.linecolor, linewidth=track.linewidth)
                 # Plot track label
@@ -631,15 +527,15 @@
 
             elif isinstance(track, LinkTrack):
                 for link in track.links:
                     # Don't plot too small link (To reduce drawing time)
                     length1, length2 = link.track_length1, link.track_length2
                     if 0 < length1 < plot_length_thr or 0 < length2 < plot_length_thr:
                         continue
-                    link = link.add_offset(self._track_name2link_offset)
+                    link = link.add_offset(self.track_name2link_offset)
                     link.plot_link(ax, ylim)
 
             elif isinstance(track, TickTrack):
                 if self.tick_style == "axis":
                     ax.xaxis.set_major_locator(MaxNLocator(10, steps=[1, 2, 5, 10]))
                     ax.xaxis.set_major_formatter(track.tick_formatter)
                 elif self.tick_style == "bar":
@@ -653,24 +549,49 @@
                     ax.text(**track.scalebar_text_params)
 
             else:
                 raise NotImplementedError()
 
         return figure
 
+    def savefig(
+        self,
+        savefile: str | Path,
+        dpi: int = 100,
+        pad_inches: float = 0.5,
+    ) -> None:
+        """Save figure to file
+
+        Parameters
+        ----------
+        savefile : str | Path
+            Save file
+        dpi : int, optional
+            DPI
+        pad_inches : float, optional
+            Padding inches
+        """
+        figure = self.plotfig(dpi=dpi)
+        figure.savefig(
+            fname=savefile,
+            dpi=dpi,
+            pad_inches=pad_inches,
+            bbox_inches="tight",
+        )
+
     def savefig_html(
         self,
-        html_outfile: str | Path,
+        html_outfile: str | Path | io.StringIO | io.BytesIO,
         fig: Figure | None = None,
     ) -> None:
         """Save figure in html format
 
         Parameters
         ----------
-        html_outfile : str | Path
+        html_outfile : str | Path | StringIO | BytesIO
             Output HTML file (*.html)
         fig : Figure | None, optional
             If Figure set, plot html viewer using user customized fig
         """
         # Load SVG contents
         if fig is None:
             fig = self.plotfig()
@@ -692,17 +613,133 @@
         for file in ASSETS_FILES:
             with open(file) as f:
                 contents = f.read()
             if file.suffix == ".css":
                 style_contents += contents + "\n"
             elif file.suffix == ".js":
                 script_contents += contents + "\n"
+        feature_tooltip_json = json.dumps(self.gid2feature_tooltip, indent=4)
+        script_contents = script_contents.replace(
+            "FEATURE_TOOLTIP_JSON = {}",
+            f"FEATURE_TOOLTIP_JSON = {feature_tooltip_json}",
+        )
+        link_tooltip_json = json.dumps(self.gid2link_tooltip, indent=4)
+        script_contents = script_contents.replace(
+            "LINK_TOOLTIP_JSON = {}",
+            f"LINK_TOOLTIP_JSON = {link_tooltip_json}",
+        )
         viewer_html = viewer_html.replace(
             "<style></style>", f"<style>{style_contents}</style>"
         )
         viewer_html = viewer_html.replace(
             "<script></script>", f"<script>{script_contents}</script>"
         )
 
         # Write viewer html contents
-        with open(html_outfile, "w") as f:
-            f.write(viewer_html)
+        if isinstance(html_outfile, io.StringIO):
+            html_outfile.write(viewer_html)
+        elif isinstance(html_outfile, io.BytesIO):
+            html_outfile.write(bytes(viewer_html, encoding="utf-8"))
+        else:
+            with open(html_outfile, "w") as f:
+                f.write(viewer_html)
+
+    def print_tracks_info(self, detail=False) -> None:
+        """Print tracks info (Mainly for debugging work)
+
+        Parameters
+        ----------
+        detail : bool, optional
+            If True, also output feature and link details
+        """
+        for idx, track in enumerate(self.get_tracks(subtrack=True), 1):
+            # Print track common info
+            class_name = track.__class__.__name__
+            print(f"\n# Track{idx:02d}: Name='{track.name}' ({class_name})")
+            size, ratio, zorder = track.size, track.ratio, track.zorder
+            print(f"# Size={size}, Ratio={ratio}, Zorder={zorder}", end="")
+
+            # Print each track specific info
+            if isinstance(track, FeatureTrack):
+                print(f", FeatureNumber={len(track.features)}")
+                if detail:
+                    for feature in track.features:
+                        print(feature)
+            elif isinstance(track, FeatureSubTrack):
+                print()
+            elif isinstance(track, LinkTrack):
+                print(f", LinkNumber={len(track.links)}")
+                if detail:
+                    for link in track.links:
+                        print(link)
+            elif isinstance(track, TickTrack):
+                print()
+
+    ############################################################
+    # Private Method
+    ############################################################
+
+    def _check_init_values(self) -> None:
+        """Check initial values"""
+        if self.align_type not in get_args(LiteralTypes.ALIGN_TYPE):
+            err_msg = f"{self.align_type=} is invalid."
+            raise ValueError(err_msg)
+
+        if self.tick_style not in get_args(LiteralTypes.TICK_STYLE):
+            err_msg = f"{self.tick_style=} is invalid."
+            raise ValueError(err_msg)
+
+    def _get_track_offset(self, track: Track) -> int:
+        """Get track offset
+
+        Parameters
+        ----------
+        track : Track
+            Target track offset for alignment
+
+        Returns
+        -------
+        track_offset : int
+            Track offset
+        """
+        if self.align_type == "left":
+            return 0
+        elif self.align_type == "center":
+            return int((self.max_track_size - track.size) / 2)
+        elif self.align_type == "right":
+            return self.max_track_size - track.size
+        else:
+            raise NotImplementedError
+
+    def _get_link_track(
+        self, feature_track_name1: str, feature_track_name2: str
+    ) -> LinkTrack:
+        """Get link track from two adjacent feature track names
+
+        Parameters
+        ----------
+        feature_track_name1 : str
+            Feature track name1
+        feature_track_name2 : str
+            Feature track name2
+
+        Returns
+        -------
+        link_track : LinkTrack
+            Target link track
+        """
+        track_names = [t.name for t in self.get_tracks()]
+        feature_track_idx1 = track_names.index(feature_track_name1)
+        feature_track_idx2 = track_names.index(feature_track_name2)
+        if abs(feature_track_idx1 - feature_track_idx2) == 2:
+            link_track_idx = int((feature_track_idx1 + feature_track_idx2) / 2)
+            target_link_track = self.get_tracks()[link_track_idx]
+            if isinstance(target_link_track, LinkTrack):
+                return target_link_track
+            else:
+                err_msg = "LinkTrack is not found between target feature tracks "
+                err_msg += f"({feature_track_name1=}, {feature_track_name2=})"
+                raise ValueError(err_msg)
+        else:
+            err_msg = f"{feature_track_name1=} and {feature_track_name2=} "
+            err_msg += "are not adjacent feature tracks."
+            raise ValueError(err_msg)
```

### Comparing `pygenomeviz-0.3.2/src/pygenomeviz/link.py` & `pygenomeviz-0.4.0/src/pygenomeviz/link.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from __future__ import annotations
 
+import textwrap
+import uuid
 from copy import deepcopy
 from dataclasses import dataclass
 from typing import Any
 
 from matplotlib import colors
 from matplotlib.axes import Axes
 from matplotlib.patches import PathPatch
@@ -25,16 +27,18 @@
     alpha: float = 0.8
     v: float | None = None
     vmin: float = 0
     vmax: float = 100
     curve: bool = False
     size_ratio: float = 1.0
     patch_kws: dict[str, Any] | None = None
+    tooltip: str | None = None
 
     def __post_init__(self):
+        self._uuid = uuid.uuid4()
         # start-end value for HTML display
         self._display_track_start1 = self.track_start1
         self._display_track_end1 = self.track_end1
         self._display_track_start2 = self.track_start2
         self._display_track_end2 = self.track_end2
         # Check color string
         if not colors.is_color_like(self.normal_color):
@@ -52,38 +56,71 @@
         if self.v is not None:
             if not 0 <= self.vmin <= self.v <= self.vmax <= 100:
                 err_msg = "'Interpolation value must be "
                 err_msg += "'0 <= vmin <= value <= vmax <= 100' "
                 err_msg += f" ({self.v=}, {self.vmin=}, {self.vmax=})"
                 raise ValueError(err_msg)
 
+        self._set_tooltip()
+
+    ############################################################
+    # Property
+    ############################################################
+
+    @property
+    def gid(self) -> str:
+        """Group ID"""
+        return "Link-" + str(self._uuid)
+
     @property
     def track_length1(self) -> int:
         """Track length1"""
         return abs(self.track_end1 - self.track_start1)
 
     @property
     def track_length2(self) -> int:
         """Track length2"""
         return abs(self.track_end2 - self.track_start2)
 
     @property
-    def gid(self) -> str:
-        """Group ID"""
-        trans_dict = {e: "_" for e in list(" /:;()+.,'`\"\\!|^~[]{}<>#$%&@?=")}
-        trans_table = str.maketrans(trans_dict)
-        name1 = self.track_name1.translate(trans_table)
-        start1 = self._display_track_start1
-        end1 = self._display_track_end1
-        name2 = self.track_name2.translate(trans_table)
-        start2 = self._display_track_start2
-        end2 = self._display_track_end2
-        track_info = f"{name1}_{start1}_{end1}_{name2}_{start2}_{end2}"
-        identity = "na" if self.v is None else int(self.v)
-        return f"Link_{track_info}_{identity}"
+    def color(self) -> str:
+        """Get conditional hexcolor code"""
+        color = self.inverted_color if self.is_inverted else self.normal_color
+        if self.v is None:
+            rgba = colors.to_rgba(color, alpha=self.alpha)
+            return colors.to_hex(rgba, keep_alpha=True)
+        else:
+
+            def to_nearly_white(color: str, nearly_value: float = 0.1) -> str:
+                """Convert target color to nearly white"""
+                cmap = colors.LinearSegmentedColormap.from_list("m", ("white", color))
+                return colors.to_hex(cmap(nearly_value))
+
+            nearly_white = to_nearly_white(color)
+            cmap = colors.LinearSegmentedColormap.from_list("m", (nearly_white, color))
+            norm = colors.Normalize(vmin=self.vmin, vmax=self.vmax)
+            norm_value = norm(self.v)
+            return colors.to_hex(cmap(norm_value, alpha=self.alpha), keep_alpha=True)
+
+    @property
+    def is_inverted(self) -> bool:
+        """Check inverted link or not
+
+        Returns
+        -------
+        is_inverted : bool
+            Check result
+        """
+        track_link_length1 = self.track_end1 - self.track_start1
+        track_link_length2 = self.track_end2 - self.track_start2
+        return track_link_length1 * track_link_length2 < 0
+
+    ############################################################
+    # Public Method
+    ############################################################
 
     def plot_link(self, ax: Axes, ylim: tuple[float, float] = (-1.0, 1.0)) -> None:
         """Plot link
 
         Parameters
         ----------
         ax : Axes
@@ -114,65 +151,14 @@
                 (Path.LINETO, (end1, ymax)),
                 (Path.LINETO, (start1, ymax)),
                 (Path.LINETO, (start2, ymin)),
             ]
         codes, verts = zip(*path_data)
         ax.add_patch(PathPatch(Path(verts, codes), **self._patch_kwargs()))
 
-    def _patch_kwargs(self) -> dict[str, Any]:
-        """Patch keyword arguments dict
-
-        Returns
-        -------
-        patch_kwargs : dict[str, Any]
-            Patch keyword arguments dict
-        """
-        patch_kws = {} if self.patch_kws is None else self.patch_kws
-        lw = 1 if self.track_length1 == self.track_length2 == 0 else 0
-        return {
-            "fc": self.color,
-            "ec": "grey",
-            "lw": lw,
-            "gid": self.gid,
-            **patch_kws,
-        }
-
-    @property
-    def color(self) -> str:
-        """Get conditional hexcolor code"""
-        color = self.inverted_color if self.is_inverted else self.normal_color
-        if self.v is None:
-            rgba = colors.to_rgba(color, alpha=self.alpha)
-            return colors.to_hex(rgba, keep_alpha=True)
-        else:
-
-            def to_nearly_white(color: str, nearly_value: float = 0.1) -> str:
-                """Convert target color to nearly white"""
-                cmap = colors.LinearSegmentedColormap.from_list("m", ("white", color))
-                return colors.to_hex(cmap(nearly_value))
-
-            nearly_white = to_nearly_white(color)
-            cmap = colors.LinearSegmentedColormap.from_list("m", (nearly_white, color))
-            norm = colors.Normalize(vmin=self.vmin, vmax=self.vmax)
-            norm_value = norm(self.v)
-            return colors.to_hex(cmap(norm_value, alpha=self.alpha), keep_alpha=True)
-
-    @property
-    def is_inverted(self) -> bool:
-        """Check inverted link or not
-
-        Returns
-        -------
-        is_inverted : bool
-            Check result
-        """
-        track_link_length1 = self.track_end1 - self.track_start1
-        track_link_length2 = self.track_end2 - self.track_start2
-        return track_link_length1 * track_link_length2 < 0
-
     def add_offset(self, track_name2offset: dict[str, int]) -> Link:
         """Add offset to each link position
 
         Parameters
         ----------
         track_name2offset : dict[str, int]
             Track name & offset dict
@@ -184,7 +170,38 @@
         """
         link = deepcopy(self)
         link.track_start1 += track_name2offset[self.track_name1]
         link.track_end1 += track_name2offset[self.track_name1]
         link.track_start2 += track_name2offset[self.track_name2]
         link.track_end2 += track_name2offset[self.track_name2]
         return link
+
+    ############################################################
+    # Private Method
+    ############################################################
+
+    def _set_tooltip(self) -> None:
+        """Set tooltip"""
+        if self.tooltip is None:
+            start1, end1 = self._display_track_start1, self._display_track_end1
+            start2, end2 = self._display_track_start2, self._display_track_end2
+            identity = "na" if self.v is None else f"{self.v:.2f}%"
+            self.tooltip = textwrap.dedent(
+                f"""
+                1. {self.track_name1} ({start1:,} - {end1:,} bp)
+                2. {self.track_name2} ({start2:,} - {end2:,} bp)
+                Identity: {identity}
+                """
+            )[1:-1]
+
+    def _patch_kwargs(self) -> dict[str, Any]:
+        """Patch keyword arguments dict
+
+        Returns
+        -------
+        patch_kwargs : dict[str, Any]
+            Patch keyword arguments dict
+        """
+        patch_kws = {} if self.patch_kws is None else self.patch_kws
+        lw = 1 if self.track_length1 == self.track_length2 == 0 else 0
+        default_kwargs = dict(fc=self.color, ec="grey", lw=lw, gid=self.gid)
+        return {**default_kwargs, **patch_kws}
```

### Comparing `pygenomeviz-0.3.2/src/pygenomeviz/parser/genbank.py` & `pygenomeviz-0.4.0/src/pygenomeviz/parser/genbank.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import bz2
 import gzip
 import zipfile
-from functools import lru_cache
+from collections import defaultdict
 from io import TextIOWrapper
 from pathlib import Path
 from typing import Any
 
 import numpy as np
 from Bio import SeqIO, SeqUtils
 from Bio.SeqFeature import FeatureLocation, Seq, SeqFeature
@@ -129,40 +129,48 @@
 
     @property
     def genome_seq(self) -> str:
         """Range genome sequence"""
         seq = "".join(str(r.seq) for r in self.records)
         return seq[self.min_range : self.max_range]
 
-    @lru_cache(maxsize=None)
     def calc_genome_gc_content(self) -> float:
         """Calculate genome GC content"""
-        return SeqUtils.gc_fraction(self.genome_seq) * 100
+        try:
+            gc_content = SeqUtils.gc_fraction(self.genome_seq) * 100
+        except AttributeError:
+            # For backward compatibility, biopython <= 1.79
+            gc_content = SeqUtils.GC(self.genome_seq)
+        return gc_content
 
     def calc_gc_skew(
         self,
         window_size: int | None = None,
         step_size: int | None = None,
+        *,
+        seq: str | None = None,
     ) -> tuple[np.ndarray, np.ndarray]:
         """Calculate GC skew in sliding window
 
         Parameters
         ----------
         window_size : int | None, optional
             Window size (Default: `genome_size / 500`)
         step_size : int | None, optional
             Step size (Default: `genome_size / 1000`)
+        seq : str | None, optional
+            Sequence for GCskew calculation (Default: `self.genome_seq`)
 
         Returns
         -------
         gc_skew_result_tuple : tuple[np.ndarray, np.ndarray]
             Position list & GC skew list
         """
         pos_list, gc_skew_list = [], []
-        seq = self.genome_seq
+        seq = self.genome_seq if seq is None else seq
         if window_size is None:
             window_size = int(len(seq) / 500)
         if step_size is None:
             step_size = int(len(seq) / 1000)
         pos_list = list(range(0, len(seq), step_size)) + [len(seq)]
         for pos in pos_list:
             window_start_pos = pos - int(window_size / 2)
@@ -181,47 +189,132 @@
 
         return (np.array(pos_list), np.array(gc_skew_list))
 
     def calc_gc_content(
         self,
         window_size: int | None = None,
         step_size: int | None = None,
+        *,
+        seq: str | None = None,
     ) -> tuple[np.ndarray, np.ndarray]:
         """Calculate GC content in sliding window
 
         Parameters
         ----------
         window_size : int | None, optional
             Window size (Default: `genome_size / 500`)
         step_size : int | None, optional
             Step size (Default: `genome_size / 1000`)
+        seq : str | None, optional
+            Sequence for GCskew calculation (Default: `self.genome_seq`)
 
         Returns
         -------
         gc_content_result_tuple : tuple[np.ndarray, np.ndarray]
             Position list & GC content list
         """
         pos_list, gc_content_list = [], []
-        seq = self.genome_seq
+        seq = self.genome_seq if seq is None else seq
         if window_size is None:
             window_size = int(len(seq) / 500)
         if step_size is None:
             step_size = int(len(seq) / 1000)
         pos_list = list(range(0, len(seq), step_size)) + [len(seq)]
         for pos in pos_list:
             window_start_pos = pos - int(window_size / 2)
             window_end_pos = pos + int(window_size / 2)
             window_start_pos = 0 if window_start_pos < 0 else window_start_pos
             window_end_pos = len(seq) if window_end_pos > len(seq) else window_end_pos
 
             subseq = seq[window_start_pos:window_end_pos]
-            gc_content_list.append(SeqUtils.gc_fraction(subseq) * 100)
+            try:
+                gc_content = SeqUtils.gc_fraction(subseq) * 100
+            except AttributeError:
+                # For backward compatibility, biopython <= 1.79
+                gc_content = SeqUtils.GC(subseq)
+            gc_content_list.append(gc_content)
 
         return (np.array(pos_list), np.array(gc_content_list))
 
+    def get_seqid2seq(self) -> dict[str, str]:
+        """Get seqid & complete/contig/scaffold genome sequence dict
+
+        Returns
+        -------
+        seqid2seq : dict[str, int]
+            seqid & genome sequence dict
+        """
+        return {rec.id: rec.seq for rec in self.records}
+
+    def get_seqid2size(self) -> dict[str, int]:
+        """Get seqid & complete/contig/scaffold genome size dict
+
+        Returns
+        -------
+        seqid2size : dict[str, int]
+            seqid & genome size dict
+        """
+        return {seqid: len(seq) for seqid, seq in self.get_seqid2seq().items()}
+
+    def get_seqid2features(
+        self,
+        feature_type: str | None = "CDS",
+        target_strand: int | None = None,
+        pseudogene: bool | None = False,
+    ) -> dict[str, list[SeqFeature]]:
+        """Get seqid & features in target seqid genome dict
+
+        Parameters
+        ----------
+        feature_type : str | None, optional
+            Feature type (`CDS`, `gene`, `mRNA`, etc...)
+            If None, extract regardless of feature type.
+        target_strand : int | None, optional
+            Extract target strand. If None, extract regardless of strand.
+        pseudogene : bool | None, optional
+            If True, `pseudo=`, `pseudogene=` tagged record only extract.
+            If False, `pseudo=`, `pseudogene=` not tagged record only extract.
+            If None, extract regardless of pseudogene tag.
+
+        Returns
+        -------
+        seqid2features : dict[str, list[SeqFeature]]
+            seqid & features dict
+        """
+        seqid2features: dict[str, list[SeqFeature]] = defaultdict(list)
+        for rec in self.records:
+            feat: SeqFeature
+            for feat in rec.features:
+                if feature_type is not None and feat.type != feature_type:
+                    continue
+                if target_strand is not None and feat.strand != target_strand:
+                    continue
+                if feat.strand == -1:
+                    start = self._to_int(feat.location.parts[-1].start)
+                    end = self._to_int(feat.location.parts[0].end)
+                else:
+                    start = self._to_int(feat.location.parts[0].start)
+                    end = self._to_int(feat.location.parts[-1].end)
+
+                qual = feat.qualifiers
+                has_pseudo_qual = "pseudo" in qual or "pseudogene" in qual
+                if (
+                    pseudogene is None
+                    or (pseudogene is True and has_pseudo_qual)
+                    or (pseudogene is False and not has_pseudo_qual)
+                ):
+                    seqid2features[rec.id].append(
+                        SeqFeature(
+                            location=FeatureLocation(start, end, feat.strand),
+                            type=feat.type,
+                            qualifiers=feat.qualifiers,
+                        ),
+                    )
+        return seqid2features
+
     def extract_features(
         self,
         feature_type: str = "CDS",
         target_strand: int | None = None,
         fix_position: bool = False,
         allow_partial: bool = False,
         pseudogene: bool = False,
@@ -372,17 +465,16 @@
             Output genome fasta file
         """
         write_seq = self.genome_seq
         with open(outfile, "w") as f:
             f.write(f">{self.name}\n{write_seq}\n")
 
     def _to_int(self, value: Any) -> int:
-        """Convert to int (Required for AbstractPostion|ExactPostion)"""
+        """Convert to int (Required for AbstractPosition|ExactPosition)"""
         return int(str(value).replace("<", "").replace(">", ""))
 
     def __str__(self):
-        name = str(self._gbk_source)
         min_max_range = f"{self.min_range:,} - {self.max_range:,} bp"
         if self.reverse:
-            return f"{name} ({min_max_range}) [Reverse Complement]"
+            return f"{self.name} ({min_max_range}) [Reverse Complement]"
         else:
-            return f"{name} ({min_max_range})"
+            return f"{self.name} ({min_max_range})"
```

### Comparing `pygenomeviz-0.3.2/src/pygenomeviz/parser/gff.py` & `pygenomeviz-0.4.0/src/pygenomeviz/parser/gff.py`

 * *Files 16% similar despite different names*

```diff
@@ -106,43 +106,54 @@
             GFF target seqid
 
         Returns
         -------
         gff_records, start, end : tuple[list[GffRecord], int, int]
             GFF record list, start, end
         """
+        # Parse GFF lines
         gff_all_lines = handle.read().splitlines()
         gff_record_lines = filter(GffRecord.is_gff_line, gff_all_lines)
         gff_records = list(map(GffRecord.parse_gff_line, gff_record_lines))
         if len(gff_records) == 0:
             err_msg = f"Failed to parse '{self._gff_file}' as GFF file "
             raise ValueError(err_msg)
 
+        # Get target seqid & GFF records
         seqid_list = list(dict.fromkeys([rec.seqid for rec in gff_records]))
-        self._seqid_list = seqid_list
         if target_seqid is None:
             target_seqid = seqid_list[0]
-        self._target_seqid = target_seqid
         if target_seqid not in seqid_list:
             err_msg = f"Not found {target_seqid=} in '{self._gff_file}'"
             raise ValueError(err_msg)
-        gff_records = [rec for rec in gff_records if rec.seqid == target_seqid]
+        target_gff_records = [rec for rec in gff_records if rec.seqid == target_seqid]
 
         # Try to get start-end region from '##sequence-region' annotation line
-        start, end = None, None
-        for line in gff_all_lines:
-            if line.startswith("##sequence-region") and target_seqid in line:
-                if len(line.split()) == 4:
-                    start, end = line.split()[2:4]
-                    start, end = int(start) - 1, int(end)
-                    break
-        if start is None or end is None:
-            start, end = 0, max([r.end for r in gff_records])
+        # If not found, (0, max_coordinate) is set as start-end
+        seqid2start_end: dict[str, tuple[int, int]] = {}
+        for seqid in seqid_list:
+            start, end = None, None
+            for line in gff_all_lines:
+                if line.startswith("##sequence-region") and seqid in line:
+                    if len(line.split()) == 4:
+                        start, end = line.split()[2:4]
+                        start, end = int(start) - 1, int(end)
+                        break
+            if start is None or end is None:
+                start, end = 0, max([r.end for r in target_gff_records])
+            seqid2start_end[seqid] = (start, end)
+        seqid2size = {seqid: e - s for seqid, (s, e) in seqid2start_end.items()}
+
+        # Set properties
+        self._target_seqid = target_seqid
+        self._seqid_list = seqid_list
+        self._all_records = gff_records
+        self._seqid2size = seqid2size
 
-        return gff_records, start, end
+        return target_gff_records, *seqid2start_end[target_seqid]
 
     @property
     def name(self) -> str:
         """Name"""
         if self._name is not None:
             return self._name
         if self._gff_file.suffix in (".gz", ".bz2", ".zip"):
@@ -156,18 +167,23 @@
 
         If `##sequence-region` pragma is not found, seq_region=`(0, max_coords_value)`
         """
         return self._seq_region
 
     @property
     def records(self) -> list[GffRecord]:
-        """GFF records"""
+        """GFF records (target seqid only)"""
         return self._records
 
     @property
+    def all_records(self) -> list[GffRecord]:
+        """All GFF records"""
+        return self._all_records
+
+    @property
     def records_within_range(self) -> list[GffRecord]:
         """GFF records within min-max range"""
         target_gff_records: list[GffRecord] = []
         for rec in self.records:
             if rec.is_within_range(self.min_range, self.max_range):
                 target_gff_records.append(rec)
         return target_gff_records
@@ -183,49 +199,94 @@
         return self._target_seqid
 
     @property
     def seqid_list(self) -> list[str]:
         """seqid list"""
         return self._seqid_list
 
+    def get_seqid2size(self) -> dict[str, int]:
+        """Get seqid & complete/contig/scaffold genome size dict
+
+        Returns
+        -------
+        seqid2size : dict[str, int]
+            seqid & genome size dict
+        """
+        return self._seqid2size
+
+    def get_seqid2features(
+        self,
+        feature_type: str | None = "CDS",
+        target_strand: int | None = None,
+        pseudogene: bool | None = False,
+    ) -> dict[str, list[SeqFeature]]:
+        """Get seqid & features in target seqid genome dict
+
+        Parameters
+        ----------
+        feature_type : str | None, optional
+            Feature type (`CDS`, `gene`, `mRNA`, etc...)
+            If None, extract regardless of feature type.
+        target_strand : int | None, optional
+            Extract target strand. If None, extract regardless of strand.
+        pseudogene : bool | None, optional
+            If True, `pseudo=`, `pseudogene=` tagged record only extract.
+            If False, `pseudo=`, `pseudogene=` not tagged record only extract.
+            If None, extract regardless of pseudogene tag.
+
+        Returns
+        -------
+        seqid2features : dict[str, list[SeqFeature]]
+            seqid & features dict
+        """
+        gff_records = GffRecord.filter_records(
+            self.all_records,
+            feature_type=feature_type,
+            target_strand=target_strand,
+            pseudogene=pseudogene,
+        )
+        seqid2features: dict[str, list[SeqFeature]] = {}
+        for seqid in self.seqid_list:
+            seqid2features[seqid] = []
+        for rec in gff_records:
+            seqid2features[rec.seqid].append(rec.to_seq_feature())
+        return seqid2features
+
     def extract_features(
         self,
-        feature_type: str = "CDS",
+        feature_type: str | None = "CDS",
         target_strand: int | None = None,
-        pseudogene: bool = False,
+        pseudogene: bool | None = False,
     ) -> list[SeqFeature]:
         """Extract features within min-max range
 
         Parameters
         ----------
-        feature_type : str, optional
+        feature_type : str | None, optional
             Feature type (`CDS`, `gene`, `mRNA`, etc...)
+            If None, extract regardless of feature type.
         target_strand : int | None, optional
-            Extract target strand
-        pseudogene : bool, optional
-            If True, `pseudo=`, `pseudogne=` tagged record only extract.
+            Extract target strand. If None, extract regardless of strand.
+        pseudogene : bool | None, optional
+            If True, `pseudo=`, `pseudogene=` tagged record only extract.
             If False, `pseudo=`, `pseudogene=` not tagged record only extract.
+            If None, extract all regardless of pseudogene tag.
 
         Returns
         -------
         features : list[SeqFeature]
             Feature list
         """
-        features: list[SeqFeature] = []
-        for rec in self.records_within_range:
-            if rec.type != feature_type:
-                continue
-            if target_strand is not None and rec.strand != target_strand:
-                continue
-            if pseudogene and ("pseudo" in rec.attrs or "pseudogene" in rec.attrs):
-                features.append(rec.to_seq_feature())
-            else:
-                features.append(rec.to_seq_feature())
-
-        return features
+        gff_records = GffRecord.filter_records(
+            self.records_within_range,
+            feature_type=feature_type,
+            target_strand=target_strand,
+            pseudogene=pseudogene,
+        )
+        return [rec.to_seq_feature() for rec in gff_records]
 
     def extract_exon_features(self, feature_type: str = "mRNA") -> list[SeqFeature]:
         """Extract exon structure features within min-max range
 
         Extract exons based on `parent feature` and `exon` ID-Parent relation
 
         Parameters
@@ -410,7 +471,49 @@
         for attr in attrs:
             if attr != "" and "=" in attr:
                 key, value = attr.split("=")
                 attr_dict[key] = value.split(",")
         gff_elms[8] = attr_dict
 
         return GffRecord(*gff_elms)
+
+    @staticmethod
+    def filter_records(
+        gff_records: list[GffRecord],
+        feature_type: str | None = "CDS",
+        target_strand: int | None = None,
+        pseudogene: bool | None = False,
+    ) -> list[GffRecord]:
+        """Filter GFF records (feature_type, strand, pseudogene)
+
+        Parameters
+        ----------
+        gff_records : list[GffRecord]
+            GFF records to be filterd
+        feature_type : str | None, optional
+            Feature type (`CDS`, `gene`, `mRNA`, etc...). If None, no filter.
+        target_strand : int | None, optional
+            Target strand. If None, no filter.
+        pseudogene : bool | None, optional
+            If True, `pseudo=`, `pseudogene=` tagged record only filter.
+            If False, `pseudo=`, `pseudogene=` not tagged record only filter.
+            If None, no filter.
+
+        Returns
+        -------
+        filter_gff_records : list[SeqFeature]
+            Filtered GFF records
+        """
+        filter_gff_records = []
+        for rec in gff_records:
+            if feature_type is not None and rec.type != feature_type:
+                continue
+            if target_strand is not None and rec.strand != target_strand:
+                continue
+            has_pseudo_attr = "pseudo" in rec.attrs or "pseudogene" in rec.attrs
+            if (
+                pseudogene is None
+                or (pseudogene is True and has_pseudo_attr)
+                or (pseudogene is False and not has_pseudo_attr)
+            ):
+                filter_gff_records.append(rec)
+        return filter_gff_records
```

### Comparing `pygenomeviz-0.3.2/src/pygenomeviz/scripts/__init__.py` & `pygenomeviz-0.4.0/src/pygenomeviz/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `pygenomeviz-0.3.2/src/pygenomeviz/scripts/download_dataset.py` & `pygenomeviz-0.4.0/src/pygenomeviz/scripts/download_dataset.py`

 * *Files identical despite different names*

### Comparing `pygenomeviz-0.3.2/src/pygenomeviz/scripts/mmseqs.py` & `pygenomeviz-0.4.0/src/pygenomeviz/scripts/mmseqs.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     run(**args.__dict__)
 
 
 def run(
     # General options
     gbk_resources: list[str | Path] | list[Genbank],
     outdir: str | Path,
-    format: list[str] = ["png", "html"],
+    format: list[str] | None = None,
     reuse: bool = False,
     # MMseqs options
     evalue: float = 1e-3,
     min_identity: float = 0,
     thread_num: int | None = None,
     # Figure appearence options
     fig_width: float = 15,
@@ -54,15 +54,15 @@
 
     Parameters
     ----------
     gbk_resources : list[str | Path] | list[Genbank]
         Input genome genbank files or Genbank objects
     outdir : str | Path
         Output directory
-    format : list[str], optional
+    format : list[str] | None, optional
         Output image format (`png`|`jpg`|`svg`|`pdf`|`html`)
     reuse : bool, optional
         If True, reuse previous result if available
     evalue : float, optional
         MMseqs RBH search E-value parameter
     min_identity : float, optional
         Min-identity threshold to be plotted
@@ -108,14 +108,15 @@
         Figure DPI
 
     Returns
     -------
     gv : GenomeViz
         GenomeViz instance
     """
+    format = ["png", "html"] if format is None else format
     # Check MMseqs installation
     MMseqs.check_installation()
 
     # Setup output contents
     outdir = Path(outdir)
     mmseqs_dir = outdir / "mmseqs_result"
     os.makedirs(mmseqs_dir, exist_ok=True)
```

### Comparing `pygenomeviz-0.3.2/src/pygenomeviz/scripts/mummer.py` & `pygenomeviz-0.4.0/src/pygenomeviz/scripts/mummer.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     run(**args.__dict__)
 
 
 def run(
     # General options
     gbk_resources: list[str | Path] | list[Genbank],
     outdir: str | Path,
-    format: list[str] = ["png", "html"],
+    format: list[str] | None = None,
     reuse: bool = False,
     # MUMmer alignment options
     seqtype: Literal["protein", "nucleotide"] = "protein",
     min_length: int = 0,
     min_identity: float = 0,
     thread_num: int | None = None,
     # Figure appearence options
@@ -59,15 +59,15 @@
 
     Parameters
     ----------
     gbk_resources : list[str | Path] | list[Genbank]
         Input genome genbank files or Genbank objects
     outdir : [str | Path
         Output directory
-    format : list[str], optional
+    format : list[str] | None, optional
         Output image format (`png`|`jpg`|`svg`|`pdf`|`html`)
     reuse : bool, optional
         If True, reuse previous result if available
     seqtype : str, optional
         MUMmer alignment sequence type (`protein`|`nucleotide`)
     min_length : int, optional
         Min-length threshold to be plotted
@@ -119,14 +119,15 @@
         Figure DPI
 
     Returns
     -------
     gv : GenomeViz
         GenomeViz instance
     """
+    format = ["png", "html"] if format is None else format
     # Check MUMmer installation
     MUMmer.check_installation()
 
     # Setup output contents
     outdir = Path(outdir)
     os.makedirs(outdir, exist_ok=True)
     align_coords_file = outdir / "align_coords.tsv"
```

### Comparing `pygenomeviz-0.3.2/src/pygenomeviz/scripts/pmauve.py` & `pygenomeviz-0.4.0/src/pygenomeviz/scripts/pmauve.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 
 def run(
     # General options
     seq_files: list[str | Path],
     outdir: str | Path,
     refid: int = 0,
-    format: list[str] = ["png", "html"],
+    format: list[str] | None = None,
     reuse: bool = False,
     # Figure appearence options
     fig_width: float = 15,
     fig_track_height: float = 1.0,
     feature_track_ratio: float = 1.0,
     link_track_ratio: float = 5.0,
     tick_track_ratio: float = 1.0,
@@ -50,15 +50,15 @@
 
     Parameters
     ----------
     seq_files : list[str | Path]
         Input genome sequence files (Genbank or Fasta format)
     outdir : str | Path
         Output directory
-    format : list[str], optional
+    format : list[str] | None, optional
         Output image format (`png`|`jpg`|`svg`|`pdf`|`html`)
     reuse : bool, optional
         If True, reuse previous result if available
     fig_width : float, optional
         Figure width
     fig_track_height : float, optional
         Figure track height
@@ -90,14 +90,15 @@
         Figure DPI
 
     Returns
     -------
     gv : GenomeViz
         GenomeViz instance
     """
+    format = ["png", "html"] if format is None else format
     # Check progressiveMauve installation
     ProgressiveMauve.check_installation()
 
     # Setup output contents
     outdir = Path(outdir)
     pmauve_dir = outdir / "pmauve_result"
     os.makedirs(pmauve_dir, exist_ok=True)
```

### Comparing `pygenomeviz-0.3.2/src/pygenomeviz/scripts/simpleplot.py` & `pygenomeviz-0.4.0/src/pygenomeviz/scripts/simpleplot.py`

 * *Files identical despite different names*

### Comparing `pygenomeviz-0.3.2/src/pygenomeviz/track.py` & `pygenomeviz-0.4.0/src/pygenomeviz/track.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,30 +54,22 @@
     def ylim(self) -> tuple[float, float]:
         """Track y min-max limit tuple"""
         return (-1.0, 1.0)
 
     @property
     def tick_params(self) -> dict[str, bool]:
         """Track tick parameters dict"""
-        return {
-            "left": False,
-            "labelleft": False,
-            "bottom": False,
-            "labelbottom": False,
-        }
+        return dict(left=False, labelleft=False, bottom=False, labelbottom=False)
 
     @property
     def spines_params(self) -> dict[str, bool]:
         """Spines parameters dict"""
-        return {
-            "left": self.spines,
-            "right": self.spines,
-            "top": self.spines,
-            "bottom": self.spines,
-        }
+        return dict(
+            left=self.spines, right=self.spines, top=self.spines, bottom=self.spines
+        )
 
     @property
     def offset(self) -> int:
         """Track alignment offset"""
         if self._offset is None:
             err_msg = "Can't access offset property before calling 'plotfig' method."
             raise ValueError(err_msg)
@@ -174,36 +166,36 @@
     def zorder(self) -> float:
         """Track zorder"""
         return 10
 
     @property
     def label_params(self) -> dict[str, Any]:
         """Label drawing parameters"""
-        return {
-            "s": self.name,
-            "fontsize": self.labelsize,
-            "color": self.labelcolor,
-            "ha": "right",
-            "va": "center",
-            "gid": f"TrackLabel_{self.name}",
-        }
+        return dict(
+            s=self.name,
+            fontsize=self.labelsize,
+            color=self.labelcolor,
+            ha="right",
+            va="center",
+            gid=f"TrackLabel_{self.name}",
+        )
 
     @property
     def sublabel_params(self) -> dict[str, Any]:
         """Sublabel drawing parameters"""
-        return {
-            "y": self._sublabel_y,
-            "s": self._sublabel_text,
-            "fontsize": self._sublabel_size,
-            "color": self._sublabel_color,
-            "ha": self._sublabel_ha,
-            "va": self._sublabel_va,
-            "zorder": 10,
-            **self._sublabel_kws,
-        }
+        default_kwargs = dict(
+            y=self._sublabel_y,
+            s=self._sublabel_text,
+            fontsize=self._sublabel_size,
+            color=self._sublabel_color,
+            ha=self._sublabel_ha,
+            va=self._sublabel_va,
+            zorder=10,
+        )
+        return {**default_kwargs, **self._sublabel_kws}
 
     def _within_valid_range(
         self, start: int, end: int, raise_error_on_false: bool = False
     ) -> bool:
         """Check if start-end position within valid track range
 
         Parameters
@@ -301,16 +293,16 @@
             Sublabel position (`[top|bottom]-[left|center|right]`)
         ymargin : float, optional
             Sublabel y-margin
         sublabel_kws: dict[str, Any] | None, optional
             Text properties (e.g. `dict(size=12, color="red", ...)`)
             <https://matplotlib.org/stable/api/_as_gen/matplotlib.axes.Axes.text.html>
         """
-        # Sublabel text setting (e.g. '0 - 1000 bp')
-        default_text = f"{self.start} - {self.end} bp"
+        # Sublabel text setting (e.g. '0 - 1,000 bp')
+        default_text = f"{self.start:,} - {self.end:,} bp"
         self._sublabel_text = default_text if text is None else text
         self._sublabel_size = size
         self._sublabel_color = color
         self._sublabel_kws = {} if sublabel_kws is None else sublabel_kws
         # Sublabel position setting
         vpos, hpos = position.split("-")
         vpos_types, hpos_types = ("top", "bottom"), ("left", "center", "right")
@@ -476,15 +468,15 @@
             Exon patch properties (e.g. `dict(fc="red", ec="black", lw=0.5, ...)`)
             <https://matplotlib.org/stable/api/_as_gen/matplotlib.patches.Patch.html>
         intron_patch_kws : dict[str, Any] | None, optional
             Intron patch properties (e.g. `dict(ec="red", lw=2, ...)`)
             <https://matplotlib.org/stable/api/_as_gen/matplotlib.patches.Patch.html>
         """
         # Check if start & end positions are within appropriate track range
-        for (exon_start, exon_end) in exon_regions:
+        for exon_start, exon_end in exon_regions:
             self._within_valid_range(exon_start, exon_end, raise_error_on_false=True)
 
         self.features.append(
             ExonFeature(
                 exon_regions,
                 strand,
                 label,
@@ -740,21 +732,23 @@
                 exon_regions: list[tuple[int, int]] = []
                 for loc in feature.location.parts:
                     start, end = int(str(loc.start)), int(str(loc.end))
                     self._within_valid_range(start, end, raise_error_on_false=True)
                     exon_regions.append((start, end))
                 # Add exon feature
                 feature_kws["intron_patch_kws"] = intron_patch_kws
-                self.features.append(ExonFeature(exon_regions, **feature_kws))
+                exon_feature = ExonFeature(exon_regions, **feature_kws)  # type: ignore
+                self.features.append(exon_feature)
             else:
                 start = int(str(feature.location.start))
                 end = int(str(feature.location.end))
                 self._within_valid_range(start, end, raise_error_on_false=True)
                 # Add feature
-                self.features.append(Feature(start, end, **feature_kws))
+                feature = Feature(start, end, **feature_kws)  # type: ignore
+                self.features.append(feature)
 
     def __str__(self):
         return f"{self.name}:{self.start}-{self.end}"
 
 
 class FeatureSubTrack(Track):
     """FeatureSubTrack Class"""
@@ -841,43 +835,43 @@
         super().__init__("tick", size, labelsize, spines, ratio)
         self.tick_style = tick_style
         self.height_scale = 1.0
 
     @property
     def tick_params(self) -> dict[str, Any]:
         """Track tick parameters dict"""
-        return {
-            "left": False,
-            "labelleft": False,
-            "bottom": self.tick_style == "axis",
-            "labelbottom": self.tick_style == "axis",
-            "labelsize": self.labelsize,
-        }
+        return dict(
+            left=False,
+            labelleft=False,
+            bottom=self.tick_style == "axis",
+            labelbottom=self.tick_style == "axis",
+            labelsize=self.labelsize,
+        )
 
     @property
     def spines_params(self) -> dict[str, bool]:
         """Spines parameters dict"""
-        return {
-            "left": self.spines,
-            "right": self.spines,
-            "top": self.spines,
-            "bottom": self.spines or self.tick_style == "axis",
-        }
+        return dict(
+            left=self.spines,
+            right=self.spines,
+            top=self.spines,
+            bottom=self.spines or self.tick_style == "axis",
+        )
 
     @property
     def scalebar_text_params(self) -> dict[str, Any]:
         """Scalebar text parameters dict"""
-        return {
-            "x": self.xcenter,
-            "y": self.ymin,
-            "s": self.scalebar_label,
-            "fontsize": self.labelsize,
-            "ha": "center",
-            "va": "top",
-        }
+        return dict(
+            x=self.xcenter,
+            y=self.ymin,
+            s=self.scalebar_label,
+            fontsize=self.labelsize,
+            ha="center",
+            va="top",
+        )
 
     @property
     def unit(self) -> str:
         """Unit (bp, Kb, Mb, Gb)"""
         for unit, value in self.unit2base_value.items():
             if self.size >= value:
                 return unit
@@ -895,15 +889,15 @@
     def base_value(self) -> float:
         """Base value"""
         return self.unit2base_value[self.unit]
 
     @property
     def unit2base_value(self) -> dict[str, int]:
         """Unit & base value dict"""
-        return {"Gb": 10**9, "Mb": 10**6, "Kb": 10**3, "bp": 1}
+        return dict(Gb=10**9, Mb=10**6, Kb=10**3, bp=1)
 
     @property
     def scalebar_label(self) -> str:
         """Label"""
         label = f"{self.scalebar_size / self.base_value:{self.format_str}}"
         return f"{label} {self.unit}"
```

### Comparing `pygenomeviz-0.3.2/src/pygenomeviz/utils.py` & `pygenomeviz-0.4.0/src/pygenomeviz/utils.py`

 * *Files identical despite different names*

### Comparing `pygenomeviz-0.3.2/src/pygenomeviz/viewer/assets/lib/images/ui-icons_444444_256x240.png` & `pygenomeviz-0.4.0/src/pygenomeviz/viewer/assets/lib/images/ui-icons_444444_256x240.png`

 * *Files identical despite different names*

### Comparing `pygenomeviz-0.3.2/src/pygenomeviz/viewer/assets/lib/images/ui-icons_555555_256x240.png` & `pygenomeviz-0.4.0/src/pygenomeviz/viewer/assets/lib/images/ui-icons_555555_256x240.png`

 * *Files identical despite different names*

### Comparing `pygenomeviz-0.3.2/src/pygenomeviz/viewer/assets/lib/images/ui-icons_777620_256x240.png` & `pygenomeviz-0.4.0/src/pygenomeviz/viewer/assets/lib/images/ui-icons_777620_256x240.png`

 * *Files identical despite different names*

### Comparing `pygenomeviz-0.3.2/src/pygenomeviz/viewer/assets/lib/images/ui-icons_777777_256x240.png` & `pygenomeviz-0.4.0/src/pygenomeviz/viewer/assets/lib/images/ui-icons_777777_256x240.png`

 * *Files identical despite different names*

### Comparing `pygenomeviz-0.3.2/src/pygenomeviz/viewer/assets/lib/images/ui-icons_cc0000_256x240.png` & `pygenomeviz-0.4.0/src/pygenomeviz/viewer/assets/lib/images/ui-icons_cc0000_256x240.png`

 * *Files identical despite different names*

### Comparing `pygenomeviz-0.3.2/src/pygenomeviz/viewer/assets/lib/images/ui-icons_ffffff_256x240.png` & `pygenomeviz-0.4.0/src/pygenomeviz/viewer/assets/lib/images/ui-icons_ffffff_256x240.png`

 * *Files identical despite different names*

### Comparing `pygenomeviz-0.3.2/src/pygenomeviz/viewer/assets/lib/jquery-ui.min.css` & `pygenomeviz-0.4.0/src/pygenomeviz/viewer/assets/lib/jquery-ui.min.css`

 * *Files identical despite different names*

### Comparing `pygenomeviz-0.3.2/src/pygenomeviz/viewer/assets/lib/jquery-ui.min.js` & `pygenomeviz-0.4.0/src/pygenomeviz/viewer/assets/lib/jquery-ui.min.js`

 * *Files identical despite different names*

### Comparing `pygenomeviz-0.3.2/src/pygenomeviz/viewer/assets/lib/jquery.min.js` & `pygenomeviz-0.4.0/src/pygenomeviz/viewer/assets/lib/jquery.min.js`

 * *Files identical despite different names*

### Comparing `pygenomeviz-0.3.2/src/pygenomeviz/viewer/assets/lib/panzoom.min.js` & `pygenomeviz-0.4.0/src/pygenomeviz/viewer/assets/lib/panzoom.min.js`

 * *Files identical despite different names*

### Comparing `pygenomeviz-0.3.2/src/pygenomeviz/viewer/assets/lib/spectrum.min.css` & `pygenomeviz-0.4.0/src/pygenomeviz/viewer/assets/lib/spectrum.min.css`

 * *Files identical despite different names*

### Comparing `pygenomeviz-0.3.2/src/pygenomeviz/viewer/assets/lib/spectrum.min.js` & `pygenomeviz-0.4.0/src/pygenomeviz/viewer/assets/lib/spectrum.min.js`

 * *Files identical despite different names*

### Comparing `pygenomeviz-0.3.2/src/pygenomeviz/viewer/assets/pgv-viewer.js` & `pygenomeviz-0.4.0/src/pygenomeviz/viewer/assets/pgv-viewer.js`

 * *Files 23% similar despite different names*

#### js-beautify {}

```diff
@@ -1,46 +1,10 @@
-/**
- * Convert feature ID to proper label for tooltip display
- * @param {string} featureId
- * @returns {string} Feature info for tooltip display
- */
-function convertFeatureIdToLabel(featureId) {
-    const matchResult = featureId.match(/Feature_(\d+)_(\d+)_(-*\d+)_type_(.+)_gene_(.+)_protein_id_(.+)_product_(.+)/)
-    let [start, end, strand, type, gene, proteinId, product] = matchResult.slice(1, 8)
-    const locale = "en-US"
-    length = Number(end - start).toLocaleString(locale)
-    start = Number(start).toLocaleString(locale)
-    end = Number(end).toLocaleString(locale)
-    strand = strand === "-1" ? "-" : "+"
-    product = product.replaceAll("_", " ")
-    let label = `location: ${start} - ${end} (${strand})\nlength: ${length} bp`
-    if (type !== "na") {
-        label += `\ntype: ${type}\ngene: ${gene}\nprotein_id: ${proteinId}\nproduct: ${product}`
-    }
-    return label
-}
-/**
- * Convert link ID to proper label for tooltip display
- * @param {string} linkId
- * @returns {string} Link info for tooltip display
- */
-function convertLinkIdToLabel(linkId) {
-    const matchResult = linkId.match(/Link_(.+)_(\d+)_(\d+)_(.+)_(\d+)_(\d+)_(.+)$/)
-    let [n1, s1, e1, n2, s2, e2, ident] = matchResult.slice(1, 8)
-    const locale = "en-US"
-    s1 = Number(s1).toLocaleString(locale)
-    e1 = Number(e1).toLocaleString(locale)
-    s2 = Number(s2).toLocaleString(locale)
-    e2 = Number(e2).toLocaleString(locale)
-    let label = `1. ${n1} (${s1} - ${e1} bp)\n2. ${n2} (${s2} - ${e2} bp)`
-    if (ident !== "na") {
-        label += `\nIdentity: ${ident}%`
-    }
-    return label
-}
+const FEATURE_TOOLTIP_JSON = {}
+const LINK_TOOLTIP_JSON = {}
+
 /**
  * Save as PNG image
  * @param {HTMLElement} svgNode
  * @param {string} fileName
  */
 function saveAsPng(svgNode, fileName = "image.png") {
     const svgData = new XMLSerializer().serializeToString(svgNode)
@@ -122,17 +86,17 @@
             continue
         }
 
         let $pathObj = $("#" + pathId + ">path")
         $pathObj.attr("title", "")
         let tooltipLabel = ""
         if (pathId.startsWith("Feature")) {
-            tooltipLabel = convertFeatureIdToLabel(pathId)
+            tooltipLabel = FEATURE_TOOLTIP_JSON[pathId]
         } else if (pathId.startsWith("Link")) {
-            tooltipLabel = convertLinkIdToLabel(pathId)
+            tooltipLabel = LINK_TOOLTIP_JSON[pathId]
         }
         $pathObj.tooltip({
             content: tooltipLabel,
             show: false,
             hide: false,
             track: true
         })
```

### Comparing `pygenomeviz-0.3.2/src/pygenomeviz/viewer/pgv-viewer-template.html` & `pygenomeviz-0.4.0/src/pygenomeviz/viewer/pgv-viewer-template.html`

 * *Files identical despite different names*

### Comparing `pygenomeviz-0.3.2/tests/conftest.py` & `pygenomeviz-0.4.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pygenomeviz-0.3.2/tests/parser/test_genbank.py` & `pygenomeviz-0.4.0/tests/parser/test_genbank.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import math
 from pathlib import Path
 
 import pytest
 from Bio.Seq import reverse_complement
+
 from pygenomeviz import Genbank
 
 
 def test_default_param(gbk_file: Path):
     """Test default parameter result"""
     gbk = Genbank(gbk_file)
     assert gbk.name == "test"
```

### Comparing `pygenomeviz-0.3.2/tests/parser/test_gff.py` & `pygenomeviz-0.4.0/tests/parser/test_gff.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from pathlib import Path
 
 import pytest
+
 from pygenomeviz import Gff
 from pygenomeviz.parser.gff import GffRecord
 
 ###########################################################
 # Test Gff
 ###########################################################
```

### Comparing `pygenomeviz-0.3.2/tests/test_feature.py` & `pygenomeviz-0.4.0/tests/test_feature.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import pytest
+
 from pygenomeviz.feature import ExonFeature, Feature
 
 ###########################################################
 # Test Feature Class
 ###########################################################
```

### Comparing `pygenomeviz-0.3.2/tests/test_genomeviz.py` & `pygenomeviz-0.4.0/tests/test_genomeviz.py`

 * *Files 2% similar despite different names*

```diff
@@ -225,23 +225,23 @@
     assert str(e.value).startswith("track_name='test' is not found")
 
 
 def test_top_track_error():
     """Test top track property access error"""
     gv = GenomeViz()
     with pytest.raises(ValueError) as e:
-        gv.top_track
+        assert gv.top_track
     assert str(e.value).startswith("No track found.")
 
 
 def test_max_track_size_error():
     """Test max track size property access error"""
     gv = GenomeViz()
     with pytest.raises(ValueError) as e:
-        gv.max_track_size
+        assert gv.max_track_size
     assert str(e.value).startswith("No track found.")
 
 
 def test_track_name_duplication_error():
     """Test track name duplication case"""
     gv = GenomeViz()
     dup_name, size = "duplication track", 1000
@@ -310,23 +310,23 @@
 
 def test_ax_property():
     """Test ax property access"""
     gv = GenomeViz()
     gv.add_feature_track("track01", 1000)
     # Can't access ax property before calling 'plotfig' method
     with pytest.raises(ValueError):
-        gv.top_track.ax
+        assert gv.top_track.ax
     # Propery access ax property after calling 'plotfig' method
     gv.plotfig()
-    gv.top_track.ax
+    assert gv.top_track.ax
 
 
 def test_offset_property():
     """Test offset property access"""
     gv = GenomeViz()
     gv.add_feature_track("track01", 1000)
     # Can't access offset property before calling 'plotfig' method
     with pytest.raises(ValueError):
-        gv.top_track.offset
+        assert gv.top_track.offset
     # Propery access offset property after calling 'plotfig' method
     gv.plotfig()
-    gv.top_track.offset
+    assert gv.top_track.offset == 0
```

### Comparing `pygenomeviz-0.3.2/tests/test_link.py` & `pygenomeviz-0.4.0/tests/test_link.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import pytest
+
 from pygenomeviz.link import Link
 
 
 def test_is_inverted():
     """Test inverted check"""
     # Case1. forward-forward
     ff_link = Link("1", 1, 100, "2", 101, 200)
```

### Comparing `pygenomeviz-0.3.2/tests/test_scripts.py` & `pygenomeviz-0.4.0/tests/test_scripts.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import subprocess as sp
 from pathlib import Path
 
 import pytest
+
 from pygenomeviz.scripts.mmseqs import MMseqs
 from pygenomeviz.scripts.mummer import MUMmer
 from pygenomeviz.scripts.pmauve import ProgressiveMauve
 from pygenomeviz.utils import load_dataset
 
 
 def test_download_dataset_cli(tmp_path: Path):
```

### Comparing `pygenomeviz-0.3.2/tests/test_track.py` & `pygenomeviz-0.4.0/tests/test_track.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import pytest
+
 from pygenomeviz.track import FeatureTrack
 
 
 def test_add_subtrack():
     """Test add subtrack"""
     track_name, track_size = "feature track", 1000
     track = FeatureTrack(track_name, track_size)
@@ -43,15 +44,15 @@
 
 def test_set_sublabel():
     """Test set sublabel"""
     track_name, track_size = "feature track", 1000
     track = FeatureTrack(track_name, track_size)
     # Default text
     track.set_sublabel()
-    assert track._sublabel_text == "0 - 1000 bp"
+    assert track._sublabel_text == "0 - 1,000 bp"
     # User defined text
     sublabel_text = "sublabel"
     track.set_sublabel(text=sublabel_text)
     assert track._sublabel_text == sublabel_text
 
 
 def test_set_sublabel_position_error():
```

### Comparing `pygenomeviz-0.3.2/tests/test_utils.py` & `pygenomeviz-0.4.0/tests/test_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from pathlib import Path
 
 import pytest
+
 from pygenomeviz.utils import ColorCycler, load_dataset, load_example_gff
 
 
 def test_load_dataset(tmp_path: Path):
     """Test load_dataset"""
     gbk_files, links = load_dataset("escherichia_phage", tmp_path)
     for gbk_file in gbk_files:
```

### Comparing `pygenomeviz-0.3.2/tests/testdata/genbank/test.gbff` & `pygenomeviz-0.4.0/tests/testdata/genbank/test.gbff`

 * *Files identical despite different names*

### Comparing `pygenomeviz-0.3.2/tests/testdata/genbank/test.gbff.bz2` & `pygenomeviz-0.4.0/tests/testdata/genbank/test.gbff.bz2`

 * *Files identical despite different names*

### Comparing `pygenomeviz-0.3.2/tests/testdata/genbank/test.gbff.gz` & `pygenomeviz-0.4.0/tests/testdata/genbank/test.gbff.gz`

 * *Files identical despite different names*

### Comparing `pygenomeviz-0.3.2/tests/testdata/genbank/test.zip` & `pygenomeviz-0.4.0/tests/testdata/genbank/test.zip`

 * *Files identical despite different names*

### Comparing `pygenomeviz-0.3.2/tests/testdata/gff/test.gff` & `pygenomeviz-0.4.0/tests/testdata/gff/test.gff`

 * *Files identical despite different names*

### Comparing `pygenomeviz-0.3.2/tests/testdata/gff/test.gff.bz2` & `pygenomeviz-0.4.0/tests/testdata/gff/test.gff.bz2`

 * *Files identical despite different names*

### Comparing `pygenomeviz-0.3.2/tests/testdata/gff/test.gff.gz` & `pygenomeviz-0.4.0/tests/testdata/gff/test.gff.gz`

 * *Files identical despite different names*

### Comparing `pygenomeviz-0.3.2/tests/testdata/gff/test.zip` & `pygenomeviz-0.4.0/tests/testdata/gff/test.zip`

 * *Files identical despite different names*

### Comparing `pygenomeviz-0.3.2/setup.py` & `pygenomeviz-0.4.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,47 +1,455 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: pygenomeviz
+Version: 0.4.0
+Summary: A genome visualization python package for comparative genomics
+Home-page: https://moshi4.github.io/pyGenomeViz/
+License: MIT
+Keywords: bioinformatics,genomics,matplotlib,visualization,comparative-genomics
+Author: moshi4
+Requires-Python: >=3.8,<4.0
+Classifier: Framework :: Matplotlib
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
+Provides-Extra: gui
+Requires-Dist: biopython (>=1.79)
+Requires-Dist: matplotlib (>=3.5.2)
+Requires-Dist: numpy (>=1.21)
+Requires-Dist: streamlit (>=1.25.0) ; (python_version >= "3.8" and python_full_version != "3.9.7" and python_version < "4.0") and (extra == "gui")
+Project-URL: Repository, https://github.com/moshi4/pyGenomeViz/
+Description-Content-Type: text/markdown
 
-package_dir = \
-{'': 'src'}
+# pyGenomeViz
 
-packages = \
-['pygenomeviz', 'pygenomeviz.parser', 'pygenomeviz.scripts']
+![Python3](https://img.shields.io/badge/Language-Python3-steelblue)
+![OS](https://img.shields.io/badge/OS-_Windows_|_Mac_|_Linux-steelblue)
+![License](https://img.shields.io/badge/License-MIT-steelblue)
+[![Latest PyPI version](https://img.shields.io/pypi/v/pygenomeviz.svg)](https://pypi.python.org/pypi/pygenomeviz)
+[![Bioconda](https://img.shields.io/conda/vn/bioconda/pygenomeviz.svg?color=green)](https://anaconda.org/bioconda/pygenomeviz)
+[![CI](https://github.com/moshi4/pyGenomeViz/actions/workflows/ci.yml/badge.svg)](https://github.com/moshi4/pyGenomeViz/actions/workflows/ci.yml)
 
-package_data = \
-{'': ['*'],
- 'pygenomeviz': ['viewer/*',
-                 'viewer/assets/*',
-                 'viewer/assets/lib/*',
-                 'viewer/assets/lib/images/*']}
-
-install_requires = \
-['biopython>=1.79,<2.0', 'matplotlib>=3.5.2,<4.0.0', 'numpy>=1.21,<2.0']
-
-entry_points = \
-{'console_scripts': ['pgv-download-dataset = '
-                     'pygenomeviz.scripts.download_dataset:main',
-                     'pgv-mmseqs = pygenomeviz.scripts.mmseqs:main',
-                     'pgv-mummer = pygenomeviz.scripts.mummer:main',
-                     'pgv-pmauve = pygenomeviz.scripts.pmauve:main',
-                     'pgv-simpleplot = pygenomeviz.scripts.simpleplot:main']}
-
-setup_kwargs = {
-    'name': 'pygenomeviz',
-    'version': '0.3.2',
-    'description': 'A genome visualization python package for comparative genomics',
-    'long_description': '# pyGenomeViz\n\n![Python3](https://img.shields.io/badge/Language-Python3-steelblue)\n![OS](https://img.shields.io/badge/OS-_Windows_|_Mac_|_Linux-steelblue)\n![License](https://img.shields.io/badge/License-MIT-steelblue)\n[![Latest PyPI version](https://img.shields.io/pypi/v/pygenomeviz.svg)](https://pypi.python.org/pypi/pygenomeviz)\n[![Bioconda](https://img.shields.io/conda/vn/bioconda/pygenomeviz.svg?color=green)](https://anaconda.org/bioconda/pygenomeviz)\n[![CI](https://github.com/moshi4/pyGenomeViz/actions/workflows/ci.yml/badge.svg)](https://github.com/moshi4/pyGenomeViz/actions/workflows/ci.yml)\n\n## Table of contents\n\n- [Overview](#overview)\n- [Installation](#installation)\n- [API Examples](#api-examples)\n- [CLI Examples](#cli-examples)\n- [Interactive HTML Viewer](#interactive-html-viewer)\n- [Inspiration](#inspiration)\n\n## Overview\n\npyGenomeViz is a genome visualization python package for comparative genomics implemented based on matplotlib.\nThis package is developed for the purpose of easily and beautifully plotting genomic\nfeatures and sequence similarity comparison links between multiple genomes.\nIt supports genome visualization of Genbank/GFF format file and can be saved figure in various formats (JPG/PNG/SVG/PDF/HTML).\nUser can use pyGenomeViz for interactive genome visualization figure plotting on jupyter notebook,\nor automatic genome visualization figure plotting in genome analysis scripts/pipelines.\n\nFor more information, please see full documentation [here](https://moshi4.github.io/pyGenomeViz/).\n\n![pygenomeviz_gallery.png](https://raw.githubusercontent.com/moshi4/pyGenomeViz/main/docs/images/pygenomeviz_gallery.png)  \n**Fig.1 pyGenomeViz example plot gallery**\n\n## Installation\n\n`Python 3.8 or later` is required for installation.\n\n**Install PyPI package:**\n\n    pip install pygenomeviz\n\n**Install bioconda package:**\n\n    conda install -c conda-forge -c bioconda pygenomeviz\n\n**Use Docker ([Image Registry](https://github.com/moshi4/pyGenomeViz/pkgs/container/pygenomeviz)):**\n\n    docker pull ghcr.io/moshi4/pygenomeviz:latest\n    docker run -it --rm ghcr.io/moshi4/pygenomeviz:latest pgv-pmauve -h\n\n## API Examples\n\nJupyter notebooks containing code examples below is available [here](https://moshi4.github.io/pyGenomeViz/getting_started/).\n\n### Basic Example\n\n#### Single Track\n\n```python\nfrom pygenomeviz import GenomeViz\n\nname, genome_size = "Tutorial 01", 5000\ncds_list = ((100, 900, -1), (1100, 1300, 1), (1350, 1500, 1), (1520, 1700, 1), (1900, 2200, -1), (2500, 2700, 1), (2700, 2800, -1), (2850, 3000, -1), (3100, 3500, 1), (3600, 3800, -1), (3900, 4200, -1), (4300, 4700, -1), (4800, 4850, 1))\n\ngv = GenomeViz()\ntrack = gv.add_feature_track(name, genome_size)\nfor idx, cds in enumerate(cds_list, 1):\n    start, end, strand = cds\n    track.add_feature(start, end, strand, label=f"CDS{idx:02d}")\n\ngv.savefig("example01.png")\n```\n\n![example01.png](https://raw.githubusercontent.com/moshi4/pyGenomeViz/main/docs/images/example01.png)\n\n#### Multiple Tracks & Links\n\n```python\nfrom pygenomeviz import GenomeViz\n\ngenome_list = (\n    {"name": "genome 01", "size": 1000, "cds_list": ((150, 300, 1), (500, 700, -1), (750, 950, 1))},\n    {"name": "genome 02", "size": 1300, "cds_list": ((50, 200, 1), (350, 450, 1), (700, 900, -1), (950, 1150, -1))},\n    {"name": "genome 03", "size": 1200, "cds_list": ((150, 300, 1), (350, 450, -1), (500, 700, -1), (700, 900, -1))},\n)\n\ngv = GenomeViz(tick_style="axis")\nfor genome in genome_list:\n    name, size, cds_list = genome["name"], genome["size"], genome["cds_list"]\n    track = gv.add_feature_track(name, size)\n    for idx, cds in enumerate(cds_list, 1):\n        start, end, strand = cds\n        track.add_feature(start, end, strand, label=f"gene{idx:02d}", linewidth=1, labelrotation=0, labelvpos="top", labelhpos="center", labelha="center")\n\n# Add links between "genome 01" and "genome 02"\ngv.add_link(("genome 01", 150, 300), ("genome 02", 50, 200))\ngv.add_link(("genome 01", 700, 500), ("genome 02", 900, 700))\ngv.add_link(("genome 01", 750, 950), ("genome 02", 1150, 950))\n# Add links between "genome 02" and "genome 03"\ngv.add_link(("genome 02", 50, 200), ("genome 03", 150, 300), normal_color="skyblue", inverted_color="lime", curve=True)\ngv.add_link(("genome 02", 350, 450), ("genome 03", 450, 350), normal_color="skyblue", inverted_color="lime", curve=True)\ngv.add_link(("genome 02", 900, 700), ("genome 03", 700, 500), normal_color="skyblue", inverted_color="lime", curve=True)\ngv.add_link(("genome 03", 900, 700), ("genome 02", 1150, 950), normal_color="skyblue", inverted_color="lime", curve=True)\n\ngv.savefig("example02.png")\n```\n\n![example02.png](https://raw.githubusercontent.com/moshi4/pyGenomeViz/main/docs/images/example02.png)\n\n#### Exon Features\n\n```python\nfrom pygenomeviz import GenomeViz\n\nexon_regions1 = [(0, 210), (300, 480), (590, 800), (850, 1000), (1030, 1300)]\nexon_regions2 = [(1500, 1710), (2000, 2480), (2590, 2800)]\nexon_regions3 = [(3000, 3300), (3400, 3690), (3800, 4100), (4200, 4620)]\n\ngv = GenomeViz()\ntrack = gv.add_feature_track(name=f"Exon Features", size=5000)\ntrack.add_exon_feature(exon_regions1, strand=1, plotstyle="box", label="box", labelrotation=0, labelha="center")\ntrack.add_exon_feature(exon_regions2, strand=-1, plotstyle="arrow", label="arrow", labelrotation=0, labelha="center", facecolor="darkgrey", intron_patch_kws={"ec": "red"})\n\nexon_labels = [f"exon{i+1}" for i in range(len(exon_regions3))]\ntrack.add_exon_feature(exon_regions3, strand=1, plotstyle="bigarrow", label="bigarrow", facecolor="lime", linewidth=1, exon_labels=exon_labels, labelrotation=0, labelha="center", exon_label_kws={"y": 0, "va": "center", "color": "blue"})\n\ngv.savefig("example03.png")\n```\n\n![example03.png](https://raw.githubusercontent.com/moshi4/pyGenomeViz/main/docs/images/example03.png)\n\n### Practical Example\n\n#### Add Features from Genbank file\n\n```python\nfrom pygenomeviz import Genbank, GenomeViz, load_dataset\n\ngbk_files, _ = load_dataset("enterobacteria_phage")\ngbk = Genbank(gbk_files[0])\n\ngv = GenomeViz()\ntrack = gv.add_feature_track(gbk.name, gbk.range_size)\ntrack.add_genbank_features(gbk)\n\ngv.savefig("example04.png")\n```\n\n![example04.png](https://raw.githubusercontent.com/moshi4/pyGenomeViz/main/docs/images/example04.png)\n\n#### Add Features from GFF file\n\n```python\nfrom pygenomeviz import Gff, GenomeViz, load_example_gff\n\ngff_file = load_example_gff("enterobacteria_phage.gff")\ngff = Gff(gff_file, min_range=5000, max_range=25000)\n\ngv = GenomeViz(fig_track_height=0.7, tick_track_ratio=0.5, tick_style="bar")\ntrack = gv.add_feature_track(gff.name, size=gff.range_size, start_pos=gff.min_range)\ntrack.add_gff_features(gff, plotstyle="arrow", facecolor="tomato")\ntrack.set_sublabel()\n\ngv.savefig("example05.png")\n```\n\n![example05.png](https://raw.githubusercontent.com/moshi4/pyGenomeViz/main/docs/images/example05.png)\n\n#### Multiple Tracks & Links from Genbank files\n\n```python\nfrom pygenomeviz import Genbank, GenomeViz, load_dataset\n\ngv = GenomeViz(\n    fig_track_height=0.7,\n    feature_track_ratio=0.2,\n    tick_track_ratio=0.4,\n    tick_style="bar",\n    align_type="center",\n)\n\ngbk_files, links = load_dataset("escherichia_phage")\nfor gbk_file in gbk_files:\n    gbk = Genbank(gbk_file)\n    track = gv.add_feature_track(gbk.name, gbk.range_size)\n    track.add_genbank_features(gbk, facecolor="limegreen", linewidth=0.5, arrow_shaft_ratio=1.0)\n\nfor link in links:\n    link_data1 = (link.ref_name, link.ref_start, link.ref_end)\n    link_data2 = (link.query_name, link.query_start, link.query_end)\n    gv.add_link(link_data1, link_data2, v=link.identity, curve=True)\n\ngv.savefig("example06.png")\n```\n\n![example06.png](https://raw.githubusercontent.com/moshi4/pyGenomeViz/main/docs/images/example06.png)\n\n### Customization Tips\n\nSince pyGenomeViz is implemented based on matplotlib, users can easily customize\nthe figure in the manner of matplotlib. Here are some tips for figure customization.\n\n#### Customization Tips 01\n\n- Add `GC Content` & `GC skew` subtrack\n- Add annotation label & fillbox\n- Add colorbar for links identity\n\n<details>\n<summary>Code</summary>\n\n```python\nfrom pygenomeviz import Genbank, GenomeViz, load_dataset\n\ngv = GenomeViz(\n    fig_width=12,\n    fig_track_height=0.7,\n    feature_track_ratio=0.5,\n    tick_track_ratio=0.3,\n    tick_style="axis",\n    tick_labelsize=10,\n)\n\ngbk_files, links = load_dataset("erwinia_phage")\ngbk_list = [Genbank(gbk_file) for gbk_file in gbk_files]\nfor gbk in gbk_list:\n    track = gv.add_feature_track(gbk.name, gbk.range_size, labelsize=15)\n    track.add_genbank_features(gbk, plotstyle="arrow")\n\nmin_identity = int(min(link.identity for link in links))\nfor link in links:\n    link_data1 = (link.ref_name, link.ref_start, link.ref_end)\n    link_data2 = (link.query_name, link.query_start, link.query_end)\n    gv.add_link(link_data1, link_data2, v=link.identity, vmin=min_identity)\n\n# Add subtracks to top track for plotting \'GC content\' & \'GC skew\'\ngv.top_track.add_subtrack(ratio=0.7, name="gc_content")\ngv.top_track.add_subtrack(ratio=0.7, name="gc_skew")\n\nfig = gv.plotfig()\n\n# Add label annotation to top track\ntop_track = gv.top_track  # or, gv.get_track("MT939486") or gv.get_tracks()[0]\nlabel, start, end = "Inverted", 310000 + top_track.offset, 358000 + top_track.offset\ncenter = int((start + end) / 2)\ntop_track.ax.hlines(1.5, start, end, colors="red", linewidth=1, linestyles="dashed", clip_on=False)\ntop_track.ax.text(center, 2.0, label, fontsize=12, color="red", ha="center", va="bottom")\n\n# Add fillbox to top track\nx, y = (start, start, end, end), (1, -1, -1, 1)\ntop_track.ax.fill(x, y, fc="lime", linewidth=0, alpha=0.1, zorder=-10)\n\n# Plot GC content for top track\npos_list, gc_content_list = gbk_list[0].calc_gc_content()\npos_list += gv.top_track.offset  # Offset is required if align_type is not \'left\'\ngc_content_ax = gv.top_track.subtracks[0].ax\ngc_content_ax.set_ylim(bottom=0, top=max(gc_content_list))\ngc_content_ax.fill_between(pos_list, gc_content_list, alpha=0.2, color="blue")\ngc_content_ax.text(gv.top_track.offset, max(gc_content_list) / 2, "GC(%) ", ha="right", va="center", color="blue")\n\n# Plot GC skew for top track\npos_list, gc_skew_list = gbk_list[0].calc_gc_skew()\npos_list += gv.top_track.offset  # Offset is required if align_type is not \'left\'\ngc_skew_abs_max = max(abs(gc_skew_list))\ngc_skew_ax = gv.top_track.subtracks[1].ax\ngc_skew_ax.set_ylim(bottom=-gc_skew_abs_max, top=gc_skew_abs_max)\ngc_skew_ax.fill_between(pos_list, gc_skew_list, alpha=0.2, color="red")\ngc_skew_ax.text(gv.top_track.offset, 0, "GC skew ", ha="right", va="center", color="red")\n\n# Set coloarbar for link\ngv.set_colorbar(fig, vmin=min_identity)\n\nfig.savefig("example07.png")\n```\n\n</details>\n\n![example07.png](https://raw.githubusercontent.com/moshi4/pyGenomeViz/main/docs/images/example07.png)\n\n#### Customization Tips 02\n\n- Add legends\n- Add colorbar for links identity\n\n<details>\n<summary>Code</summary>\n\n```python\nfrom matplotlib.lines import Line2D\nfrom matplotlib.patches import Patch\n\nfrom pygenomeviz import Genbank, GenomeViz, load_dataset\n\ngv = GenomeViz(\n    fig_width=10,\n    fig_track_height=0.5,\n    feature_track_ratio=0.5,\n    tick_track_ratio=0.3,\n    align_type="center",\n    tick_style="bar",\n    tick_labelsize=10,\n)\n\ngbk_files, links = load_dataset("enterobacteria_phage")\nfor idx, gbk_file in enumerate(gbk_files):\n    gbk = Genbank(gbk_file)\n    track = gv.add_feature_track(gbk.name, gbk.range_size, labelsize=10)\n    track.add_genbank_features(\n        gbk,\n        label_type="product" if idx == 0 else None,  # Labeling only top track\n        label_handle_func=lambda s: "" if s.startswith("hypothetical") else s,  # Ignore \'hypothetical ~~~\' label\n        labelsize=8,\n        labelvpos="top",\n        facecolor="skyblue",\n        linewidth=0.5,\n    )\n\nnormal_color, inverted_color, alpha = "chocolate", "limegreen", 0.5\nmin_identity = int(min(link.identity for link in links))\nfor link in links:\n    link_data1 = (link.ref_name, link.ref_start, link.ref_end)\n    link_data2 = (link.query_name, link.query_start, link.query_end)\n    gv.add_link(link_data1, link_data2, normal_color, inverted_color, alpha, v=link.identity, vmin=min_identity, curve=True)\n\nfig = gv.plotfig()\n\n# Add Legends (Maybe there is a better way)\nhandles = [\n    Line2D([], [], marker=">", color="skyblue", label="CDS", ms=10, ls="none"),\n    Patch(color=normal_color, label="Normal Link"),\n    Patch(color=inverted_color, label="Inverted Link"),\n]\nfig.legend(handles=handles, bbox_to_anchor=(1, 1))\n\n# Set colorbar for link\ngv.set_colorbar(fig, bar_colors=[normal_color, inverted_color], alpha=alpha, vmin=min_identity, bar_label="Identity", bar_labelsize=10)\n\nfig.savefig("example08.png")\n```\n\n</details>\n\n![example08.png](https://raw.githubusercontent.com/moshi4/pyGenomeViz/main/docs/images/example08.png)\n\n## CLI Examples\n\npyGenomeViz provides CLI workflow for visualization of genome alignment or\nreciprocal best-hit CDS search results with `MUMmer` or `MMseqs` or `progressiveMauve`.\nEach CLI workflow requires the installation of additional dependent tools to run.\n\n### MUMmer CLI Workflow Example\n\nSee [pgv-mummer document](https://moshi4.github.io/pyGenomeViz/cli-docs/pgv-mummer/) for details.\n\nDownload example dataset: `pgv-download-dataset -n erwinia_phage`\n\n> :warning: MUMmer must be installed in advance to run\n\n    pgv-mummer --gbk_resources MT939486.gbk MT939487.gbk MT939488.gbk LT960552.gbk \\\n               -o mummer_example --tick_style axis --align_type left --feature_plotstyle arrow\n\n![mummer_example.png](https://raw.githubusercontent.com/moshi4/pyGenomeViz/main/docs/images/mummer_example1.png)  \n\n### MMseqs CLI Workflow Example\n\nSee [pgv-mmseqs document](https://moshi4.github.io/pyGenomeViz/cli-docs/pgv-mmseqs/) for details.\n\nDownload example dataset: `pgv-download-dataset -n enterobacteria_phage`\n\n> :warning: MMseqs must be installed in advance to run\n\n    pgv-mmseqs --gbk_resources NC_019724.gbk NC_024783.gbk NC_016566.gbk NC_013600.gbk NC_031081.gbk NC_028901.gbk \\\n               -o mmseqs_example --fig_track_height 0.7 --feature_linewidth 0.3 --tick_style bar --curve \\\n               --normal_link_color chocolate --inverted_link_color limegreen --feature_color skyblue\n\n![mmseqs_example.png](https://raw.githubusercontent.com/moshi4/pyGenomeViz/main/docs/images/mmseqs_example3.png)  \n\n### progressiveMauve CLI Workflow Example\n\nSee [pgv-pmauve document](https://moshi4.github.io/pyGenomeViz/cli-docs/pgv-pmauve/) for details.\n\nDownload example dataset: `pgv-download-dataset -n escherichia_coli`\n\n> :warning: progressiveMauve must be installed in advance to run\n\n    pgv-pmauve --seq_files NC_000913.gbk NC_002695.gbk NC_011751.gbk NC_011750.gbk \\\n               -o pmauve_example --tick_style bar\n\n![pmauve_example.png](https://raw.githubusercontent.com/moshi4/pyGenomeViz/main/docs/images/pmauve_example1.png)  \n\n## Interactive HTML Viewer\n\npyGenomeViz implements HTML file output functionality for interactive data visualization.\nIn API, HTML file can be output using `savefig_html` method. In CLI, user can select HTML file output option.\nAs shown below, data tooltip display, pan/zoom, object color change, text change, etc are available in HTML viewer\n([Demo Page](https://moshi4.github.io/pyGenomeViz/images/pgv-viewer-demo.html)).\n\n![pgv-viewer-demo.gif](https://raw.githubusercontent.com/moshi4/pyGenomeViz/main/docs/images/pgv-viewer-demo.gif)\n\n## Inspiration\n\npyGenomeViz was inspired by\n\n- [GenomeDiagram (BioPython)](https://github.com/biopython/biopython)\n- [Easyfig](http://mjsull.github.io/Easyfig/)\n- [genoplotR](https://genoplotr.r-forge.r-project.org/)\n- [gggenomes](https://github.com/thackl/gggenomes)\n',
-    'author': 'moshi4',
-    'author_email': 'None',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://moshi4.github.io/pyGenomeViz/',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.8,<4.0',
-}
+## Table of contents
 
+- [Overview](#overview)
+- [Installation](#installation)
+- [API Examples](#api-examples)
+- [CLI Examples](#cli-examples)
+- [GUI (Web browser)](#gui-web-browser)
+- [Interactive HTML Viewer](#interactive-html-viewer)
+- [Inspiration](#inspiration)
+- [Circular Genome Visualization](#circular-genome-visualization)
+
+## Overview
+
+pyGenomeViz is a genome visualization python package for comparative genomics implemented based on matplotlib.
+This package is developed for the purpose of easily and beautifully plotting genomic
+features and sequence similarity comparison links between multiple genomes.
+It supports genome visualization of Genbank/GFF format file and can be saved figure in various formats (JPG/PNG/SVG/PDF/HTML).
+User can use pyGenomeViz for interactive genome visualization figure plotting on jupyter notebook,
+or automatic genome visualization figure plotting in genome analysis scripts/pipelines.
+
+For more information, please see full documentation [here](https://moshi4.github.io/pyGenomeViz/).
+
+![pygenomeviz_gallery.png](https://raw.githubusercontent.com/moshi4/pyGenomeViz/main/docs/images/pygenomeviz_gallery.png)  
+**Fig.1 pyGenomeViz example plot gallery**
+
+:sparkles: GUI (Web browser) functionality is newly added from v0.4.0
+
+![pygenomeviz_gui.gif](https://raw.githubusercontent.com/moshi4/pyGenomeViz/main/src/pygenomeviz/gui/assets/pgv_demo.gif)
+**Fig.2 pyGenomeViz GUI (Web browser) version example**
+
+## Installation
+
+`Python 3.8 or later` is required for installation.
+
+**Install PyPI package:**
+
+    pip install pygenomeviz
+
+**Install bioconda package:**
+
+    conda install -c conda-forge -c bioconda pygenomeviz
+
+**Use Docker ([Image Registry](https://github.com/moshi4/pyGenomeViz/pkgs/container/pygenomeviz)):**
+
+    docker run --rm -p 8501:8501 ghcr.io/moshi4/pygenomeviz:latest pgv-gui
+
+## API Examples
+
+Jupyter notebooks containing code examples below is available [here](https://moshi4.github.io/pyGenomeViz/getting_started/).
+
+### Basic Example
+
+#### Single Track
+
+```python
+from pygenomeviz import GenomeViz
+
+name, genome_size = "Tutorial 01", 5000
+cds_list = ((100, 900, -1), (1100, 1300, 1), (1350, 1500, 1), (1520, 1700, 1), (1900, 2200, -1), (2500, 2700, 1), (2700, 2800, -1), (2850, 3000, -1), (3100, 3500, 1), (3600, 3800, -1), (3900, 4200, -1), (4300, 4700, -1), (4800, 4850, 1))
+
+gv = GenomeViz()
+track = gv.add_feature_track(name, genome_size)
+for idx, cds in enumerate(cds_list, 1):
+    start, end, strand = cds
+    track.add_feature(start, end, strand, label=f"CDS{idx:02d}")
+
+gv.savefig("example01.png")
+```
+
+![example01.png](https://raw.githubusercontent.com/moshi4/pyGenomeViz/main/docs/images/example01.png)
+
+#### Multiple Tracks & Links
+
+```python
+from pygenomeviz import GenomeViz
+
+genome_list = (
+    {"name": "genome 01", "size": 1000, "cds_list": ((150, 300, 1), (500, 700, -1), (750, 950, 1))},
+    {"name": "genome 02", "size": 1300, "cds_list": ((50, 200, 1), (350, 450, 1), (700, 900, -1), (950, 1150, -1))},
+    {"name": "genome 03", "size": 1200, "cds_list": ((150, 300, 1), (350, 450, -1), (500, 700, -1), (700, 900, -1))},
+)
+
+gv = GenomeViz(tick_style="axis")
+for genome in genome_list:
+    name, size, cds_list = genome["name"], genome["size"], genome["cds_list"]
+    track = gv.add_feature_track(name, size)
+    for idx, cds in enumerate(cds_list, 1):
+        start, end, strand = cds
+        track.add_feature(start, end, strand, label=f"gene{idx:02d}", linewidth=1, labelrotation=0, labelvpos="top", labelhpos="center", labelha="center")
+
+# Add links between "genome 01" and "genome 02"
+gv.add_link(("genome 01", 150, 300), ("genome 02", 50, 200))
+gv.add_link(("genome 01", 700, 500), ("genome 02", 900, 700))
+gv.add_link(("genome 01", 750, 950), ("genome 02", 1150, 950))
+# Add links between "genome 02" and "genome 03"
+gv.add_link(("genome 02", 50, 200), ("genome 03", 150, 300), normal_color="skyblue", inverted_color="lime", curve=True)
+gv.add_link(("genome 02", 350, 450), ("genome 03", 450, 350), normal_color="skyblue", inverted_color="lime", curve=True)
+gv.add_link(("genome 02", 900, 700), ("genome 03", 700, 500), normal_color="skyblue", inverted_color="lime", curve=True)
+gv.add_link(("genome 03", 900, 700), ("genome 02", 1150, 950), normal_color="skyblue", inverted_color="lime", curve=True)
+
+gv.savefig("example02.png")
+```
+
+![example02.png](https://raw.githubusercontent.com/moshi4/pyGenomeViz/main/docs/images/example02.png)
+
+#### Exon Features
+
+```python
+from pygenomeviz import GenomeViz
+
+exon_regions1 = [(0, 210), (300, 480), (590, 800), (850, 1000), (1030, 1300)]
+exon_regions2 = [(1500, 1710), (2000, 2480), (2590, 2800)]
+exon_regions3 = [(3000, 3300), (3400, 3690), (3800, 4100), (4200, 4620)]
+
+gv = GenomeViz()
+track = gv.add_feature_track(name=f"Exon Features", size=5000)
+track.add_exon_feature(exon_regions1, strand=1, plotstyle="box", label="box", labelrotation=0, labelha="center")
+track.add_exon_feature(exon_regions2, strand=-1, plotstyle="arrow", label="arrow", labelrotation=0, labelha="center", facecolor="darkgrey", intron_patch_kws={"ec": "red"})
+
+exon_labels = [f"exon{i+1}" for i in range(len(exon_regions3))]
+track.add_exon_feature(exon_regions3, strand=1, plotstyle="bigarrow", label="bigarrow", facecolor="lime", linewidth=1, exon_labels=exon_labels, labelrotation=0, labelha="center", exon_label_kws={"y": 0, "va": "center", "color": "blue"})
+
+gv.savefig("example03.png")
+```
+
+![example03.png](https://raw.githubusercontent.com/moshi4/pyGenomeViz/main/docs/images/example03.png)
+
+### Practical Example
+
+#### Add Features from Genbank file
+
+```python
+from pygenomeviz import Genbank, GenomeViz, load_dataset
+
+gbk_files, _ = load_dataset("enterobacteria_phage")
+gbk = Genbank(gbk_files[0])
+
+gv = GenomeViz()
+track = gv.add_feature_track(gbk.name, gbk.range_size)
+track.add_genbank_features(gbk)
+
+gv.savefig("example04.png")
+```
+
+![example04.png](https://raw.githubusercontent.com/moshi4/pyGenomeViz/main/docs/images/example04.png)
+
+#### Add Features from GFF file
+
+```python
+from pygenomeviz import Gff, GenomeViz, load_example_gff
+
+gff_file = load_example_gff("enterobacteria_phage.gff")
+gff = Gff(gff_file, min_range=5000, max_range=25000)
+
+gv = GenomeViz(fig_track_height=0.7, tick_track_ratio=0.5, tick_style="bar")
+track = gv.add_feature_track(gff.name, size=gff.range_size, start_pos=gff.min_range)
+track.add_gff_features(gff, plotstyle="arrow", facecolor="tomato")
+track.set_sublabel()
+
+gv.savefig("example05.png")
+```
+
+![example05.png](https://raw.githubusercontent.com/moshi4/pyGenomeViz/main/docs/images/example05.png)
+
+#### Multiple Tracks & Links from Genbank files
+
+```python
+from pygenomeviz import Genbank, GenomeViz, load_dataset
+
+gv = GenomeViz(
+    fig_track_height=0.7,
+    feature_track_ratio=0.2,
+    tick_track_ratio=0.4,
+    tick_style="bar",
+    align_type="center",
+)
+
+gbk_files, links = load_dataset("escherichia_phage")
+for gbk_file in gbk_files:
+    gbk = Genbank(gbk_file)
+    track = gv.add_feature_track(gbk.name, gbk.range_size)
+    track.add_genbank_features(gbk, facecolor="limegreen", linewidth=0.5, arrow_shaft_ratio=1.0)
+
+for link in links:
+    link_data1 = (link.ref_name, link.ref_start, link.ref_end)
+    link_data2 = (link.query_name, link.query_start, link.query_end)
+    gv.add_link(link_data1, link_data2, v=link.identity, curve=True)
+
+gv.savefig("example06.png")
+```
+
+![example06.png](https://raw.githubusercontent.com/moshi4/pyGenomeViz/main/docs/images/example06.png)
+
+### Customization Tips
+
+Since pyGenomeViz is implemented based on matplotlib, users can easily customize
+the figure in the manner of matplotlib. Here are some tips for figure customization.
+
+#### Customization Tips 01
+
+- Add `GC Content` & `GC skew` subtrack
+- Add annotation label & fillbox
+- Add colorbar for links identity
+
+<details>
+<summary>Code</summary>
+
+```python
+from pygenomeviz import Genbank, GenomeViz, load_dataset
+
+gv = GenomeViz(
+    fig_width=12,
+    fig_track_height=0.7,
+    feature_track_ratio=0.5,
+    tick_track_ratio=0.3,
+    tick_style="axis",
+    tick_labelsize=10,
+)
+
+gbk_files, links = load_dataset("erwinia_phage")
+gbk_list = [Genbank(gbk_file) for gbk_file in gbk_files]
+for gbk in gbk_list:
+    track = gv.add_feature_track(gbk.name, gbk.range_size, labelsize=15)
+    track.add_genbank_features(gbk, plotstyle="arrow")
+
+min_identity = int(min(link.identity for link in links))
+for link in links:
+    link_data1 = (link.ref_name, link.ref_start, link.ref_end)
+    link_data2 = (link.query_name, link.query_start, link.query_end)
+    gv.add_link(link_data1, link_data2, v=link.identity, vmin=min_identity)
+
+# Add subtracks to top track for plotting 'GC content' & 'GC skew'
+gv.top_track.add_subtrack(ratio=0.7, name="gc_content")
+gv.top_track.add_subtrack(ratio=0.7, name="gc_skew")
+
+fig = gv.plotfig()
+
+# Add label annotation to top track
+top_track = gv.top_track  # or, gv.get_track("MT939486") or gv.get_tracks()[0]
+label, start, end = "Inverted", 310000 + top_track.offset, 358000 + top_track.offset
+center = int((start + end) / 2)
+top_track.ax.hlines(1.5, start, end, colors="red", linewidth=1, linestyles="dashed", clip_on=False)
+top_track.ax.text(center, 2.0, label, fontsize=12, color="red", ha="center", va="bottom")
+
+# Add fillbox to top track
+x, y = (start, start, end, end), (1, -1, -1, 1)
+top_track.ax.fill(x, y, fc="lime", linewidth=0, alpha=0.1, zorder=-10)
+
+# Plot GC content for top track
+pos_list, gc_content_list = gbk_list[0].calc_gc_content()
+pos_list += gv.top_track.offset  # Offset is required if align_type is not 'left'
+gc_content_ax = gv.top_track.subtracks[0].ax
+gc_content_ax.set_ylim(bottom=0, top=max(gc_content_list))
+gc_content_ax.fill_between(pos_list, gc_content_list, alpha=0.2, color="blue")
+gc_content_ax.text(gv.top_track.offset, max(gc_content_list) / 2, "GC(%) ", ha="right", va="center", color="blue")
+
+# Plot GC skew for top track
+pos_list, gc_skew_list = gbk_list[0].calc_gc_skew()
+pos_list += gv.top_track.offset  # Offset is required if align_type is not 'left'
+gc_skew_abs_max = max(abs(gc_skew_list))
+gc_skew_ax = gv.top_track.subtracks[1].ax
+gc_skew_ax.set_ylim(bottom=-gc_skew_abs_max, top=gc_skew_abs_max)
+gc_skew_ax.fill_between(pos_list, gc_skew_list, alpha=0.2, color="red")
+gc_skew_ax.text(gv.top_track.offset, 0, "GC skew ", ha="right", va="center", color="red")
+
+# Set coloarbar for link
+gv.set_colorbar(fig, vmin=min_identity)
+
+fig.savefig("example07.png")
+```
+
+</details>
+
+![example07.png](https://raw.githubusercontent.com/moshi4/pyGenomeViz/main/docs/images/example07.png)
+
+#### Customization Tips 02
+
+- Add legends
+- Add colorbar for links identity
+
+<details>
+<summary>Code</summary>
+
+```python
+from matplotlib.lines import Line2D
+from matplotlib.patches import Patch
+
+from pygenomeviz import Genbank, GenomeViz, load_dataset
+
+gv = GenomeViz(
+    fig_width=10,
+    fig_track_height=0.5,
+    feature_track_ratio=0.5,
+    tick_track_ratio=0.3,
+    align_type="center",
+    tick_style="bar",
+    tick_labelsize=10,
+)
+
+gbk_files, links = load_dataset("enterobacteria_phage")
+for idx, gbk_file in enumerate(gbk_files):
+    gbk = Genbank(gbk_file)
+    track = gv.add_feature_track(gbk.name, gbk.range_size, labelsize=10)
+    track.add_genbank_features(
+        gbk,
+        label_type="product" if idx == 0 else None,  # Labeling only top track
+        label_handle_func=lambda s: "" if s.startswith("hypothetical") else s,  # Ignore 'hypothetical ~~~' label
+        labelsize=8,
+        labelvpos="top",
+        facecolor="skyblue",
+        linewidth=0.5,
+    )
+
+normal_color, inverted_color, alpha = "chocolate", "limegreen", 0.5
+min_identity = int(min(link.identity for link in links))
+for link in links:
+    link_data1 = (link.ref_name, link.ref_start, link.ref_end)
+    link_data2 = (link.query_name, link.query_start, link.query_end)
+    gv.add_link(link_data1, link_data2, normal_color, inverted_color, alpha, v=link.identity, vmin=min_identity, curve=True)
+
+fig = gv.plotfig()
+
+# Add Legends (Maybe there is a better way)
+handles = [
+    Line2D([], [], marker=">", color="skyblue", label="CDS", ms=10, ls="none"),
+    Patch(color=normal_color, label="Normal Link"),
+    Patch(color=inverted_color, label="Inverted Link"),
+]
+fig.legend(handles=handles, bbox_to_anchor=(1, 1))
+
+# Set colorbar for link
+gv.set_colorbar(fig, bar_colors=[normal_color, inverted_color], alpha=alpha, vmin=min_identity, bar_label="Identity", bar_labelsize=10)
+
+fig.savefig("example08.png")
+```
+
+</details>
+
+![example08.png](https://raw.githubusercontent.com/moshi4/pyGenomeViz/main/docs/images/example08.png)
+
+## CLI Examples
+
+pyGenomeViz provides CLI workflow for visualization of genome alignment or
+reciprocal best-hit CDS search results with `MUMmer` or `MMseqs` or `progressiveMauve`.
+Each CLI workflow requires the installation of additional dependent tools to run.
+
+### MUMmer CLI Workflow Example
+
+See [pgv-mummer document](https://moshi4.github.io/pyGenomeViz/cli-docs/pgv-mummer/) for details.
+
+Download example dataset: `pgv-download-dataset -n erwinia_phage`
+
+> :warning: MUMmer must be installed in advance to run
+
+    pgv-mummer --gbk_resources MT939486.gbk MT939487.gbk MT939488.gbk LT960552.gbk \
+               -o mummer_example --tick_style axis --align_type left --feature_plotstyle arrow
+
+![mummer_example.png](https://raw.githubusercontent.com/moshi4/pyGenomeViz/main/docs/images/mummer_example1.png)  
+
+### MMseqs CLI Workflow Example
+
+See [pgv-mmseqs document](https://moshi4.github.io/pyGenomeViz/cli-docs/pgv-mmseqs/) for details.
+
+Download example dataset: `pgv-download-dataset -n enterobacteria_phage`
+
+> :warning: MMseqs must be installed in advance to run
+
+    pgv-mmseqs --gbk_resources NC_019724.gbk NC_024783.gbk NC_016566.gbk NC_013600.gbk NC_031081.gbk NC_028901.gbk \
+               -o mmseqs_example --fig_track_height 0.7 --feature_linewidth 0.3 --tick_style bar --curve \
+               --normal_link_color chocolate --inverted_link_color limegreen --feature_color skyblue
+
+![mmseqs_example.png](https://raw.githubusercontent.com/moshi4/pyGenomeViz/main/docs/images/mmseqs_example3.png)  
+
+### progressiveMauve CLI Workflow Example
+
+See [pgv-pmauve document](https://moshi4.github.io/pyGenomeViz/cli-docs/pgv-pmauve/) for details.
+
+Download example dataset: `pgv-download-dataset -n escherichia_coli`
+
+> :warning: progressiveMauve must be installed in advance to run
+
+    pgv-pmauve --seq_files NC_000913.gbk NC_002695.gbk NC_011751.gbk NC_011750.gbk \
+               -o pmauve_example --tick_style bar
+
+![pmauve_example.png](https://raw.githubusercontent.com/moshi4/pyGenomeViz/main/docs/images/pmauve_example1.png)  
+
+## GUI (Web browser)
+
+pyGenomeViz implements GUI (Web browser) functionality using [Streamlit](https://github.com/streamlit/streamlit) as an option.
+Users can easily perform data visualization of Genbank files and genome comparison
+results using MUMmer or MMseqs. See [pgv-gui document](https://moshi4.github.io/pyGenomeViz/gui-docs/pgv-gui/) for details.
+
+![pygenomeviz_gui.gif](https://raw.githubusercontent.com/moshi4/pyGenomeViz/main/src/pygenomeviz/gui/assets/pgv_demo.gif)
+
+## Interactive HTML Viewer
+
+pyGenomeViz implements HTML file output functionality for interactive data visualization.
+In API, HTML file can be output using `savefig_html` method. In CLI, user can select HTML file output option.
+As shown below, data tooltip display, pan/zoom, object color change, text change, etc are available in HTML viewer
+([Demo Page](https://moshi4.github.io/pyGenomeViz/images/pgv-viewer-demo.html)).
+
+![pgv-viewer-demo.gif](https://raw.githubusercontent.com/moshi4/pyGenomeViz/main/docs/images/pgv-viewer-demo.gif)
+
+## Inspiration
+
+pyGenomeViz was inspired by
+
+- [GenomeDiagram (BioPython)](https://github.com/biopython/biopython)
+- [Easyfig](http://mjsull.github.io/Easyfig/)
+- [genoplotR](https://genoplotr.r-forge.r-project.org/)
+- [gggenomes](https://github.com/thackl/gggenomes)
+
+## Circular Genome Visualization
+
+pyGenomeViz is a python package designed for linear genome visualization.
+If you are interested in circular genome visualization, check out my other python package [pyCirclize](https://github.com/moshi4/pyCirclize).
+
+![pycirclize_example.png](https://raw.githubusercontent.com/moshi4/pyGenomeViz/main/docs/images/pycirclize_example.png)  
+**Fig. pyCirclize example plot gallery**
 
-setup(**setup_kwargs)
```

