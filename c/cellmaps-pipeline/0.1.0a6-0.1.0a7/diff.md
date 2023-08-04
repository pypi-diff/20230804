# Comparing `tmp/cellmaps_pipeline-0.1.0a6.tar.gz` & `tmp/cellmaps_pipeline-0.1.0a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cellmaps_pipeline-0.1.0a6.tar", last modified: Tue Aug  1 22:27:37 2023, max compression
+gzip compressed data, was "dist/cellmaps_pipeline-0.1.0a7.tar", last modified: Fri Aug  4 00:18:41 2023, max compression
```

## Comparing `cellmaps_pipeline-0.1.0a6.tar` & `cellmaps_pipeline-0.1.0a7.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-08-01 22:27:37.890920 cellmaps_pipeline-0.1.0a6/
--rw-r--r--   0 churas     (504) staff       (20)      266 2023-06-08 20:06:13.000000 cellmaps_pipeline-0.1.0a6/AUTHORS.rst
--rw-r--r--   0 churas     (504) staff       (20)     3641 2023-03-29 16:39:59.000000 cellmaps_pipeline-0.1.0a6/CONTRIBUTING.rst
--rw-r--r--   0 churas     (504) staff       (20)       89 2023-05-22 23:49:21.000000 cellmaps_pipeline-0.1.0a6/HISTORY.rst
--rw-r--r--   0 churas     (504) staff       (20)     1102 2023-03-29 16:39:59.000000 cellmaps_pipeline-0.1.0a6/LICENSE
--rw-r--r--   0 churas     (504) staff       (20)      262 2023-03-29 16:39:59.000000 cellmaps_pipeline-0.1.0a6/MANIFEST.in
--rw-r--r--   0 churas     (504) staff       (20)     6081 2023-08-01 22:27:37.891053 cellmaps_pipeline-0.1.0a6/PKG-INFO
--rw-r--r--   0 churas     (504) staff       (20)     4079 2023-08-01 00:51:41.000000 cellmaps_pipeline-0.1.0a6/README.rst
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-08-01 22:27:37.881792 cellmaps_pipeline-0.1.0a6/cellmaps_pipeline/
--rw-r--r--   0 churas     (504) staff       (20)      279 2023-08-01 22:27:17.000000 cellmaps_pipeline-0.1.0a6/cellmaps_pipeline/__init__.py
--rw-r--r--   0 churas     (504) staff       (20)     8923 2023-07-17 20:25:30.000000 cellmaps_pipeline-0.1.0a6/cellmaps_pipeline/cellmaps_pipelinecmd.py
--rw-r--r--   0 churas     (504) staff       (20)      132 2023-04-04 23:01:54.000000 cellmaps_pipeline-0.1.0a6/cellmaps_pipeline/exceptions.py
--rw-r--r--   0 churas     (504) staff       (20)    12687 2023-07-17 20:25:30.000000 cellmaps_pipeline-0.1.0a6/cellmaps_pipeline/runner.py
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-08-01 22:27:37.883806 cellmaps_pipeline-0.1.0a6/cellmaps_pipeline.egg-info/
--rw-r--r--   0 churas     (504) staff       (20)     6081 2023-08-01 22:27:37.000000 cellmaps_pipeline-0.1.0a6/cellmaps_pipeline.egg-info/PKG-INFO
--rw-r--r--   0 churas     (504) staff       (20)     1105 2023-08-01 22:27:37.000000 cellmaps_pipeline-0.1.0a6/cellmaps_pipeline.egg-info/SOURCES.txt
--rw-r--r--   0 churas     (504) staff       (20)        1 2023-08-01 22:27:37.000000 cellmaps_pipeline-0.1.0a6/cellmaps_pipeline.egg-info/dependency_links.txt
--rw-r--r--   0 churas     (504) staff       (20)        1 2023-08-01 22:27:37.000000 cellmaps_pipeline-0.1.0a6/cellmaps_pipeline.egg-info/not-zip-safe
--rw-r--r--   0 churas     (504) staff       (20)      243 2023-08-01 22:27:37.000000 cellmaps_pipeline-0.1.0a6/cellmaps_pipeline.egg-info/requires.txt
--rw-r--r--   0 churas     (504) staff       (20)       18 2023-08-01 22:27:37.000000 cellmaps_pipeline-0.1.0a6/cellmaps_pipeline.egg-info/top_level.txt
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-08-01 22:27:37.888386 cellmaps_pipeline-0.1.0a6/docs/
--rw-r--r--   0 churas     (504) staff       (20)      618 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a6/docs/Makefile
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-08-01 22:27:37.878167 cellmaps_pipeline-0.1.0a6/docs/_build/
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-08-01 22:27:37.878352 cellmaps_pipeline-0.1.0a6/docs/_build/html/
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-08-01 22:27:37.888658 cellmaps_pipeline-0.1.0a6/docs/_build/html/_images/
--rw-r--r--   0 churas     (504) staff       (20)    29975 2023-07-18 21:25:06.000000 cellmaps_pipeline-0.1.0a6/docs/_build/html/_images/pipeline_overview.png
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-08-01 22:27:37.889481 cellmaps_pipeline-0.1.0a6/docs/_build/html/_static/
--rw-r--r--   0 churas     (504) staff       (20)      286 2023-05-02 22:49:28.000000 cellmaps_pipeline-0.1.0a6/docs/_build/html/_static/file.png
--rw-r--r--   0 churas     (504) staff       (20)       90 2023-05-02 22:49:28.000000 cellmaps_pipeline-0.1.0a6/docs/_build/html/_static/minus.png
--rw-r--r--   0 churas     (504) staff       (20)       90 2023-05-02 22:49:28.000000 cellmaps_pipeline-0.1.0a6/docs/_build/html/_static/plus.png
--rw-r--r--   0 churas     (504) staff       (20)       28 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a6/docs/authors.rst
--rw-r--r--   0 churas     (504) staff       (20)      744 2023-05-22 23:59:43.000000 cellmaps_pipeline-0.1.0a6/docs/cellmaps_pipeline.rst
--rwxr-xr-x   0 churas     (504) staff       (20)     6035 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a6/docs/conf.py
--rw-r--r--   0 churas     (504) staff       (20)       33 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a6/docs/contributing.rst
--rw-r--r--   0 churas     (504) staff       (20)      174 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a6/docs/devbranches.rst
--rw-r--r--   0 churas     (504) staff       (20)      285 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a6/docs/developer.rst
--rw-r--r--   0 churas     (504) staff       (20)       28 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a6/docs/history.rst
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-08-01 22:27:37.889760 cellmaps_pipeline-0.1.0a6/docs/images/
--rw-r--r--   0 churas     (504) staff       (20)    29975 2023-08-01 00:51:42.000000 cellmaps_pipeline-0.1.0a6/docs/images/pipeline_overview.png
--rw-r--r--   0 churas     (504) staff       (20)     1783 2023-08-01 00:51:42.000000 cellmaps_pipeline-0.1.0a6/docs/index.rst
--rw-r--r--   0 churas     (504) staff       (20)     1189 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a6/docs/installation.rst
--rw-r--r--   0 churas     (504) staff       (20)      451 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a6/docs/integrationtesting.rst
--rw-r--r--   0 churas     (504) staff       (20)      815 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a6/docs/make.bat
--rw-r--r--   0 churas     (504) staff       (20)       76 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a6/docs/modules.rst
--rw-r--r--   0 churas     (504) staff       (20)     4340 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a6/docs/newrelease.rst
--rw-r--r--   0 churas     (504) staff       (20)      787 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a6/docs/pypircfile.rst
--rw-r--r--   0 churas     (504) staff       (20)      884 2023-08-01 00:51:42.000000 cellmaps_pipeline-0.1.0a6/docs/usage.rst
--rw-r--r--   0 churas     (504) staff       (20)      817 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a6/docs/versioningscheme.rst
--rw-r--r--   0 churas     (504) staff       (20)      400 2023-08-01 22:27:37.892075 cellmaps_pipeline-0.1.0a6/setup.cfg
--rw-r--r--   0 churas     (504) staff       (20)     2460 2023-08-01 22:27:17.000000 cellmaps_pipeline-0.1.0a6/setup.py
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-08-01 22:27:37.890695 cellmaps_pipeline-0.1.0a6/tests/
--rw-r--r--   0 churas     (504) staff       (20)       72 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a6/tests/__init__.py
--rw-r--r--   0 churas     (504) staff       (20)     1296 2023-06-07 18:25:27.000000 cellmaps_pipeline-0.1.0a6/tests/test_cellmaps_pipelinecmd.py
--rw-r--r--   0 churas     (504) staff       (20)      896 2023-06-07 18:25:27.000000 cellmaps_pipeline-0.1.0a6/tests/test_cellmapspipeline.py
--rw-r--r--   0 churas     (504) staff       (20)      772 2023-03-29 16:39:59.000000 cellmaps_pipeline-0.1.0a6/tests/test_integration_cellmaps_pipeline.py
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-08-04 00:18:41.882454 cellmaps_pipeline-0.1.0a7/
+-rw-r--r--   0 churas     (504) staff       (20)      266 2023-06-08 20:06:13.000000 cellmaps_pipeline-0.1.0a7/AUTHORS.rst
+-rw-r--r--   0 churas     (504) staff       (20)     3641 2023-03-29 16:39:59.000000 cellmaps_pipeline-0.1.0a7/CONTRIBUTING.rst
+-rw-r--r--   0 churas     (504) staff       (20)       89 2023-05-22 23:49:21.000000 cellmaps_pipeline-0.1.0a7/HISTORY.rst
+-rw-r--r--   0 churas     (504) staff       (20)     1102 2023-03-29 16:39:59.000000 cellmaps_pipeline-0.1.0a7/LICENSE
+-rw-r--r--   0 churas     (504) staff       (20)      262 2023-03-29 16:39:59.000000 cellmaps_pipeline-0.1.0a7/MANIFEST.in
+-rw-r--r--   0 churas     (504) staff       (20)     6081 2023-08-04 00:18:41.882636 cellmaps_pipeline-0.1.0a7/PKG-INFO
+-rw-r--r--   0 churas     (504) staff       (20)     4079 2023-08-01 00:51:41.000000 cellmaps_pipeline-0.1.0a7/README.rst
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-08-04 00:18:41.871960 cellmaps_pipeline-0.1.0a7/cellmaps_pipeline/
+-rw-r--r--   0 churas     (504) staff       (20)      279 2023-08-04 00:18:26.000000 cellmaps_pipeline-0.1.0a7/cellmaps_pipeline/__init__.py
+-rw-r--r--   0 churas     (504) staff       (20)    10519 2023-08-04 00:18:26.000000 cellmaps_pipeline-0.1.0a7/cellmaps_pipeline/cellmaps_pipelinecmd.py
+-rw-r--r--   0 churas     (504) staff       (20)      132 2023-04-04 23:01:54.000000 cellmaps_pipeline-0.1.0a7/cellmaps_pipeline/exceptions.py
+-rw-r--r--   0 churas     (504) staff       (20)    16229 2023-08-04 00:18:26.000000 cellmaps_pipeline-0.1.0a7/cellmaps_pipeline/runner.py
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-08-04 00:18:41.874288 cellmaps_pipeline-0.1.0a7/cellmaps_pipeline.egg-info/
+-rw-r--r--   0 churas     (504) staff       (20)     6081 2023-08-04 00:18:41.000000 cellmaps_pipeline-0.1.0a7/cellmaps_pipeline.egg-info/PKG-INFO
+-rw-r--r--   0 churas     (504) staff       (20)     1105 2023-08-04 00:18:41.000000 cellmaps_pipeline-0.1.0a7/cellmaps_pipeline.egg-info/SOURCES.txt
+-rw-r--r--   0 churas     (504) staff       (20)        1 2023-08-04 00:18:41.000000 cellmaps_pipeline-0.1.0a7/cellmaps_pipeline.egg-info/dependency_links.txt
+-rw-r--r--   0 churas     (504) staff       (20)        1 2023-08-04 00:18:41.000000 cellmaps_pipeline-0.1.0a7/cellmaps_pipeline.egg-info/not-zip-safe
+-rw-r--r--   0 churas     (504) staff       (20)      248 2023-08-04 00:18:41.000000 cellmaps_pipeline-0.1.0a7/cellmaps_pipeline.egg-info/requires.txt
+-rw-r--r--   0 churas     (504) staff       (20)       18 2023-08-04 00:18:41.000000 cellmaps_pipeline-0.1.0a7/cellmaps_pipeline.egg-info/top_level.txt
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-08-04 00:18:41.879121 cellmaps_pipeline-0.1.0a7/docs/
+-rw-r--r--   0 churas     (504) staff       (20)      618 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a7/docs/Makefile
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-08-04 00:18:41.867979 cellmaps_pipeline-0.1.0a7/docs/_build/
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-08-04 00:18:41.868361 cellmaps_pipeline-0.1.0a7/docs/_build/html/
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-08-04 00:18:41.879377 cellmaps_pipeline-0.1.0a7/docs/_build/html/_images/
+-rw-r--r--   0 churas     (504) staff       (20)    31213 2023-08-02 20:18:42.000000 cellmaps_pipeline-0.1.0a7/docs/_build/html/_images/pipeline_overview.png
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-08-04 00:18:41.880296 cellmaps_pipeline-0.1.0a7/docs/_build/html/_static/
+-rw-r--r--   0 churas     (504) staff       (20)      286 2023-05-02 22:49:28.000000 cellmaps_pipeline-0.1.0a7/docs/_build/html/_static/file.png
+-rw-r--r--   0 churas     (504) staff       (20)       90 2023-05-02 22:49:28.000000 cellmaps_pipeline-0.1.0a7/docs/_build/html/_static/minus.png
+-rw-r--r--   0 churas     (504) staff       (20)       90 2023-05-02 22:49:28.000000 cellmaps_pipeline-0.1.0a7/docs/_build/html/_static/plus.png
+-rw-r--r--   0 churas     (504) staff       (20)       28 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a7/docs/authors.rst
+-rw-r--r--   0 churas     (504) staff       (20)      744 2023-05-22 23:59:43.000000 cellmaps_pipeline-0.1.0a7/docs/cellmaps_pipeline.rst
+-rwxr-xr-x   0 churas     (504) staff       (20)     6035 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a7/docs/conf.py
+-rw-r--r--   0 churas     (504) staff       (20)       33 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a7/docs/contributing.rst
+-rw-r--r--   0 churas     (504) staff       (20)      174 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a7/docs/devbranches.rst
+-rw-r--r--   0 churas     (504) staff       (20)      285 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a7/docs/developer.rst
+-rw-r--r--   0 churas     (504) staff       (20)       28 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a7/docs/history.rst
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-08-04 00:18:41.880696 cellmaps_pipeline-0.1.0a7/docs/images/
+-rw-r--r--   0 churas     (504) staff       (20)    31213 2023-08-02 22:59:40.000000 cellmaps_pipeline-0.1.0a7/docs/images/pipeline_overview.png
+-rw-r--r--   0 churas     (504) staff       (20)     1925 2023-08-02 22:59:40.000000 cellmaps_pipeline-0.1.0a7/docs/index.rst
+-rw-r--r--   0 churas     (504) staff       (20)     1189 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a7/docs/installation.rst
+-rw-r--r--   0 churas     (504) staff       (20)      451 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a7/docs/integrationtesting.rst
+-rw-r--r--   0 churas     (504) staff       (20)      815 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a7/docs/make.bat
+-rw-r--r--   0 churas     (504) staff       (20)       76 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a7/docs/modules.rst
+-rw-r--r--   0 churas     (504) staff       (20)     4340 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a7/docs/newrelease.rst
+-rw-r--r--   0 churas     (504) staff       (20)      787 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a7/docs/pypircfile.rst
+-rw-r--r--   0 churas     (504) staff       (20)      884 2023-08-01 00:51:42.000000 cellmaps_pipeline-0.1.0a7/docs/usage.rst
+-rw-r--r--   0 churas     (504) staff       (20)      817 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a7/docs/versioningscheme.rst
+-rw-r--r--   0 churas     (504) staff       (20)      400 2023-08-04 00:18:41.883390 cellmaps_pipeline-0.1.0a7/setup.cfg
+-rw-r--r--   0 churas     (504) staff       (20)     2484 2023-08-04 00:18:26.000000 cellmaps_pipeline-0.1.0a7/setup.py
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-08-04 00:18:41.882041 cellmaps_pipeline-0.1.0a7/tests/
+-rw-r--r--   0 churas     (504) staff       (20)       72 2023-03-29 16:40:00.000000 cellmaps_pipeline-0.1.0a7/tests/__init__.py
+-rw-r--r--   0 churas     (504) staff       (20)     1296 2023-06-07 18:25:27.000000 cellmaps_pipeline-0.1.0a7/tests/test_cellmaps_pipelinecmd.py
+-rw-r--r--   0 churas     (504) staff       (20)      896 2023-06-07 18:25:27.000000 cellmaps_pipeline-0.1.0a7/tests/test_cellmapspipeline.py
+-rw-r--r--   0 churas     (504) staff       (20)      772 2023-03-29 16:39:59.000000 cellmaps_pipeline-0.1.0a7/tests/test_integration_cellmaps_pipeline.py
```

### Comparing `cellmaps_pipeline-0.1.0a6/CONTRIBUTING.rst` & `cellmaps_pipeline-0.1.0a7/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_pipeline-0.1.0a6/LICENSE` & `cellmaps_pipeline-0.1.0a7/LICENSE`

 * *Files identical despite different names*

### Comparing `cellmaps_pipeline-0.1.0a6/PKG-INFO` & `cellmaps_pipeline-0.1.0a7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellmaps_pipeline
-Version: 0.1.0a6
+Version: 0.1.0a7
 Summary: Runs full Cellmaps CM4AI pipeline
 Home-page: https://github.com/idekerlab/cellmaps_pipeline
 Author: Ideker Lab CM4AI team
 Author-email: tools@cm4ai.org
 License: MIT license
 Description: ===================
         Cell Maps Pipeline
```

### Comparing `cellmaps_pipeline-0.1.0a6/README.rst` & `cellmaps_pipeline-0.1.0a7/README.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_pipeline-0.1.0a6/cellmaps_pipeline/cellmaps_pipelinecmd.py` & `cellmaps_pipeline-0.1.0a7/cellmaps_pipeline/cellmaps_pipelinecmd.py`

 * *Files 16% similar despite different names*

```diff
@@ -49,22 +49,22 @@
                              'GeneID1\tSymbol1\tGeneID2\tSymbol2\n'
                              '10159\tATP6AP2\t2\tA2M')
     parser.add_argument('--baitlist',
                         help='baitlist TSV file in format of:\n'
                              'GeneSymbol\tGeneID\t# Interactors\n'
                              '"ADA"\t"100"\t1.')
     parser.add_argument('--model_path', type=str,
-                        help='Path to model file. A model file to download '
-                             'is here: '
-                             'https://github.com/'
-                             'CellProfiling/densenet/releases/download/'
-                             'v0.1.0/external_crop512_focal_slov_hardlog'
-                             '_class_densenet121_dropout_i768_aug2_5folds'
-                             '_fold0_final.pth')
-    parser.add_argument('--fold', default=1, type=int, help='Image node attribute file fold to use')
+                        default='https://github.com/CellProfiling/densenet/releases/download/v0.1.0/external_crop512_focal_slov_hardlog_class_densenet121_dropout_i768_aug2_5folds_fold0_final.pth',
+                        help='URL or path to model file for image embedding')
+    parser.add_argument('--fold', default=[1], nargs='+', type=int,
+                        help='Image node attribute file fold(s) to use. '
+                             'Each additional fold specified will create '
+                             'additional 2.image_embedding_fold# and'
+                             '3.coembedding_fold# directories that will be'
+                             'fed into hierarchy step. Valid values are 1 or 2 or 1 2')
     parser.add_argument('--proteinatlasxml',
                         default='https://www.proteinatlas.org/download/proteinatlas.xml.gz',
                         help='URL or path to proteinatlas.xml or proteinatlas.xml.gz file '
                              'used to look for images not found in the standard location '
                              'on HPA')
     parser.add_argument('--ppi_cutoffs', nargs='+', type=float,
                         default=[0.001, 0.002, 0.003, 0.004, 0.005, 0.006,
@@ -120,15 +120,59 @@
 
     withguids_json = json.dumps(withguid, indent=2)
     register_json = json.dumps(register, indent=2)
 
     desc = """
 Version {version}
 
-Runs the full cellmaps pipeline
+The Cell Maps Pipeline takes ImmunoFluorescent images from the Human Protein 
+Atlas along with Affinity Purification Mass Spectrometry data from one or 
+more sources, converts them into embeddings that are then co-embedded and 
+converted into an integrated interaction network from which a hierarchical 
+model is derived.
+
+The pipeline invokes six tools that each create an output directory where 
+results are stored and registered within Research Object Crates (RO-Crate) 
+using the FAIRSCAPE-cli.
+
+For more information visit https://cellmaps-pipeline.readthedocs.io
+
+                 ppi_download  image_download
+                       ||            ||
+                       \/            \/
+              ppi_embedding  image_embedding_fold#
+                        \\\\      //
+                         \\\\    //
+                    co_embedding_fold#
+                           ||
+                           \/
+                        hierarchy
+              
+In default mode this will create the following directories under <outdir> specified
+on the commandline:
+
+  1.image_download
+  1.ppi_download
+  1.ppi_embedding
+  2.image_embedding_fold1
+  3.coembedding_fold1
+  4.hierarchy
+  
+If --fold 1 2 is passed in on the command line the directories would look like this:
+
+  1.image_download
+  1.ppi_download
+  1.ppi_embedding
+  2.image_embedding_fold1
+  2.image_embedding_fold2
+  3.coembedding_fold1
+  3.coembedding_fold2
+  4.hierarchy
+
+
 
 In addition, the --provenance flag is required and must be set to a path 
 to a JSON file. 
 
 If datasets are already registered with FAIRSCAPE then the following is sufficient:
 
 {withguids}
```

### Comparing `cellmaps_pipeline-0.1.0a6/cellmaps_pipeline/runner.py` & `cellmaps_pipeline-0.1.0a7/cellmaps_pipeline/runner.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 #! /usr/bin/env python
 
 import os
 import warnings
 import logging
 import time
+import requests
 import networkx as nx
+from tqdm import tqdm
 from cellmaps_utils import logutils
 from cellmaps_utils import constants
 from cellmaps_utils.provenance import ProvenanceUtil
 
 from cellmaps_imagedownloader.runner import MultiProcessImageDownloader
 from cellmaps_imagedownloader.runner import FakeImageDownloader
 from cellmaps_imagedownloader.runner import CellmapsImageDownloader
@@ -69,43 +71,40 @@
                  baitlist=None,
                  model_path=None,
                  proteinatlasxml=None,
                  ppi_cutoffs=None,
                  fake=None,
                  provenance=None,
                  provenance_utils=ProvenanceUtil(),
-                 fold=1,
+                 fold=[1],
                  input_data_dict=None):
         """
         Constructor
         """
         super().__init__()
         self._outdir = os.path.abspath(outdir)
         self._samples = samples
         self._unique = unique
         self._edgelist = edgelist
         self._baitlist = baitlist
-        self._model_path = model_path
+        self._model_path = self._download_model(model_path)
         self._fake = fake
         self._provenance = provenance
         self._provenance_utils = provenance_utils
-        self._fold = fold
         self._proteinatlasxml = proteinatlasxml
         self._ppi_cutoffs = ppi_cutoffs
         self._input_data_dict = input_data_dict
         self._image_dir = os.path.join(self._outdir,
                                        constants.IMAGE_DOWNLOAD_STEP_DIR)
         self._ppi_dir = os.path.join(self._outdir,
                                      constants.PPI_DOWNLOAD_STEP_DIR)
         self._ppi_embed_dir = os.path.join(self._outdir,
                                            constants.PPI_EMBEDDING_STEP_DIR)
-        self._image_embed_dir = os.path.join(self._outdir,
-                                             constants.IMAGE_EMBEDDING_STEP_DIR)
-        self._coembed_dir = os.path.join(self._outdir,
-                                         constants.COEMBEDDING_STEP_DIR)
+
+        self._image_coembed_tuples = self._get_image_coembed_tuples(fold)
 
         self._hierarchy_dir = os.path.join(self._outdir,
                                            constants.HIERARCHY_STEP_DIR)
 
     def run(self):
         """
         Runs pipeline programmatically in serial steps. This would
@@ -130,78 +129,161 @@
             raise CellmapsPipelineError('Coembed failed')
 
         if self._hierarchy() != 0:
             raise CellmapsPipelineError('Hierarchy failed')
 
         return 0
 
+    def _download_model(self, model_path):
+        """
+        If model_path is a URL attempt to download it
+        to pipeline directory, otherwise return as is
+
+        :param model_path: URL or file path to model file needed
+                           for image embedding
+        :type model_path: str
+        :return: path to model file
+        :rtype: str
+        """
+        if os.path.isfile(model_path):
+            return model_path
+        dest_file = os.path.join(self._outdir, 'model.pth')
+        with requests.get(model_path,
+                          stream=True) as r:
+            content_size = int(r.headers.get('content-length', 0))
+            tqdm_bar = tqdm(desc='Downloading ' + os.path.basename(model_path),
+                            total=content_size,
+                            unit='B', unit_scale=True,
+                            unit_divisor=1024)
+            logger.debug('Downloading ' + str(model_path) +
+                         ' of size ' + str(content_size) +
+                         'b to ' + dest_file)
+            try:
+                r.raise_for_status()
+                with open(dest_file, 'wb') as f:
+                    for chunk in r.iter_content(chunk_size=8192):
+                        f.write(chunk)
+                        tqdm_bar.update(len(chunk))
+            finally:
+                tqdm_bar.close()
+        return dest_file
+
+    def _get_image_coembed_tuples(self, fold):
+        """
+
+        :param fold:
+        :return:
+        """
+        if fold is None:
+            raise CellmapsPipelineError('Fold cannot be None')
+
+        image_coembed_tuples = []
+        logger.debug('Fold values: ' + str(fold))
+        for fold_val in fold:
+            image_embed_dir = os.path.join(self._outdir,
+                                     constants.IMAGE_EMBEDDING_STEP_DIR +
+                                           str(fold_val))
+            co_embed_dir = os.path.join(self._outdir,
+                                        constants.COEMBEDDING_STEP_DIR +
+                                        str(fold_val))
+
+            image_coembed_tuples.append((fold_val, image_embed_dir,
+                                         co_embed_dir))
+        logger.debug('Value of image_coembed_tuples: ' + str(image_coembed_tuples))
+        return image_coembed_tuples
+
     def _hierarchy(self):
         """
 
         :return:
         """
         if os.path.isdir(self._hierarchy_dir):
             warnings.warn('Found hierarchy dir, assuming we are good. skipping')
             return 0
 
-        ppigen = CosineSimilarityPPIGenerator(embeddingdir=self._coembed_dir,
+        coembed_dirs = []
+        for image_coembed_tuple in self._image_coembed_tuples:
+            coembed_dirs.append(image_coembed_tuple[2])
+
+        logger.debug('Coembedding directories: ' + str(coembed_dirs))
+
+        ppigen = CosineSimilarityPPIGenerator(embeddingdir=coembed_dirs,
                                               cutoffs=self._ppi_cutoffs)
 
         refiner = HiDeFHierarchyRefiner(provenance_utils=self._provenance_utils)
 
         hiergen = CDAPSHiDeFHierarchyGenerator(refiner=refiner,
                                                provenance_utils=self._provenance_utils)
         return CellmapsGenerateHierarchy(outdir=self._hierarchy_dir,
-                                         inputdir=self._coembed_dir,
+                                         inputdir=coembed_dirs,
                                          ppigen=ppigen,
                                          hiergen=hiergen,
                                          input_data_dict=self._input_data_dict,
                                          provenance_utils=self._provenance_utils).run()
 
     def _coembed(self):
         """
 
         :return:
         """
-        if os.path.isdir(self._coembed_dir):
-            warnings.warn('Found coembedding dir, assuming we are good. skipping')
-            return 0
-
-        if self._fake:
-            gen = FakeCoEmbeddingGenerator(ppi_embeddingdir=self._ppi_embed_dir,
-                                           image_embeddingdir=self._image_embed_dir)
-        else:
-            gen = MuseCoEmbeddingGenerator(outdir=self._coembed_dir,
-                                           ppi_embeddingdir=self._ppi_embed_dir,
-                                           image_embeddingdir=self._image_embed_dir)
-        return CellmapsCoEmbedder(outdir=self._coembed_dir,
-                                  inputdirs=[self._image_embed_dir, self._ppi_embed_dir],
-                                  embedding_generator=gen,
-                                  input_data_dict=self._input_data_dict).run()
+        for image_coembed_tuple in self._image_coembed_tuples:
+            if os.path.isdir(image_coembed_tuple[2]):
+                warnings.warn('Found coembedding dir' +
+                              str(image_coembed_tuple[2]) +
+                              ', assuming we are good. skipping')
+                continue
+            if self._fake:
+                gen = FakeCoEmbeddingGenerator(ppi_embeddingdir=self._ppi_embed_dir,
+                                               image_embeddingdir=image_coembed_tuple[1])
+            else:
+                gen = MuseCoEmbeddingGenerator(outdir=image_coembed_tuple[2],
+                                               ppi_embeddingdir=self._ppi_embed_dir,
+                                               image_embeddingdir=image_coembed_tuple[1])
+            retval = CellmapsCoEmbedder(outdir=image_coembed_tuple[2],
+                                        inputdirs=[image_coembed_tuple[1],
+                                                   self._ppi_embed_dir],
+                                        embedding_generator=gen,
+                                        input_data_dict=self._input_data_dict).run()
+            if retval != 0:
+                logger.error('Coembedding ' + image_coembed_tuple[2] +
+                             'using ' + image_coembed_tuple[1] +
+                             ' had non zero exit code of: ' +
+                             str(retval))
+                return retval
+        return 0
 
     def _embed_image(self):
         """
 
         :return:
         """
-        if os.path.isdir(self._image_embed_dir):
-            warnings.warn('Found image embedding dir, assuming we are good. skipping')
-            return 0
-
-        if self._fake is True:
-            gen = FakeEmbeddingGenerator(self._image_dir)
-        else:
-            gen = DensenetEmbeddingGenerator(self._image_dir,
-                                             outdir=self._image_embed_dir,
-                                             model_path=self._model_path,
-                                             fold=self._fold)
-        return CellmapsImageEmbedder(outdir=self._image_embed_dir,
-                                     inputdir=self._image_dir,
-                                     embedding_generator=gen,
-                                     input_data_dict=self._input_data_dict).run()
+        for image_coembed_tuple in self._image_coembed_tuples:
+            if os.path.isdir(image_coembed_tuple[1]):
+                warnings.warn('Found image_embedding dir' +
+                              str(image_coembed_tuple[1]) +
+                              ', assuming we are good. skipping')
+                continue
+            if self._fake is True:
+                gen = FakeEmbeddingGenerator(self._image_dir)
+            else:
+                gen = DensenetEmbeddingGenerator(self._image_dir,
+                                                 outdir=image_coembed_tuple[1],
+                                                 model_path=self._model_path,
+                                                 fold=int(image_coembed_tuple[0]))
+            retval = CellmapsImageEmbedder(outdir=image_coembed_tuple[1],
+                                           inputdir=self._image_dir,
+                                           embedding_generator=gen,
+                                           input_data_dict=self._input_data_dict).run()
+            if retval != 0:
+                logger.error('image embedding ' + image_coembed_tuple[1] +
+                             'using fold' + str(image_coembed_tuple[0] +
+                             ' had non zero exit code of: ' +
+                             str(retval)))
+                return retval
+        return 0
 
     def _embed_ppi(self):
         """
 
         :return:
         """
         if os.path.isdir(self._ppi_embed_dir):
```

### Comparing `cellmaps_pipeline-0.1.0a6/cellmaps_pipeline.egg-info/PKG-INFO` & `cellmaps_pipeline-0.1.0a7/cellmaps_pipeline.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellmaps-pipeline
-Version: 0.1.0a6
+Version: 0.1.0a7
 Summary: Runs full Cellmaps CM4AI pipeline
 Home-page: https://github.com/idekerlab/cellmaps_pipeline
 Author: Ideker Lab CM4AI team
 Author-email: tools@cm4ai.org
 License: MIT license
 Description: ===================
         Cell Maps Pipeline
```

### Comparing `cellmaps_pipeline-0.1.0a6/cellmaps_pipeline.egg-info/SOURCES.txt` & `cellmaps_pipeline-0.1.0a7/cellmaps_pipeline.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cellmaps_pipeline-0.1.0a6/docs/Makefile` & `cellmaps_pipeline-0.1.0a7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cellmaps_pipeline-0.1.0a6/docs/cellmaps_pipeline.rst` & `cellmaps_pipeline-0.1.0a7/docs/cellmaps_pipeline.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_pipeline-0.1.0a6/docs/conf.py` & `cellmaps_pipeline-0.1.0a7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `cellmaps_pipeline-0.1.0a6/docs/index.rst` & `cellmaps_pipeline-0.1.0a7/docs/index.rst`

 * *Files 6% similar despite different names*

```diff
@@ -11,26 +11,28 @@
 
 Cell Maps Pipeline for `Cell Maps for AI (CM4AI) <https://cm4ai.org>`__
 
 The Cell Maps Pipeline takes `ImmunoFluorescent <https://en.wikipedia.org/wiki/Immunofluorescence>`__ images from
 the `Human Protein Atlas <https://www.proteinatlas.org>`__ along with
 `Affinity Purification Mass Spectrometry <https://www.thermofisher.com/us/en/home/industrial/mass-spectrometry/proteomics-protein-mass-spectrometry/proteomics-protein-mass-spectrometry-workflows/protein-structure-analysis-mass-spectrometry/affinity-mass-spectrometry.html>`__
 data from one or more sources, converts them into embeddings that
-are then coembedded and converted into a Protein to Protein Interaction network from which a hierarchical
+are then coembedded and converted into an integrated interaction network from which a hierarchical
 model is derived.
 
 The pipeline invokes six tools that each create an output directory where results are
 stored and registered within `Research Object Crates (RO-Crate) <https://www.researchobject.org/ro-crate>`__ using
 the `FAIRSCAPE-cli <https://pypi.org/project/fairscape-cli>`__.
 
 Overview of Cell Maps Pipeline
 
 .. image:: images/pipeline_overview.png
   :alt: Overview of Cell Maps Pipeline which shows PPI and image download followed by embedding, coembedding, and finally hierarchy generation
 
+..
+    The pipeline_overview.png image is from this google doc: https://docs.google.com/drawings/d/1pAqQkmg8hRh7ySkgu5PVY7Hu4pwMyejAzAYzGge0ilU/edit
 
 
 * Free software: MIT license
 
 .. toctree::
    :maxdepth: 2
    :caption: Contents:
```

### Comparing `cellmaps_pipeline-0.1.0a6/docs/installation.rst` & `cellmaps_pipeline-0.1.0a7/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_pipeline-0.1.0a6/docs/make.bat` & `cellmaps_pipeline-0.1.0a7/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cellmaps_pipeline-0.1.0a6/docs/newrelease.rst` & `cellmaps_pipeline-0.1.0a7/docs/newrelease.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_pipeline-0.1.0a6/docs/pypircfile.rst` & `cellmaps_pipeline-0.1.0a7/docs/pypircfile.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_pipeline-0.1.0a6/docs/usage.rst` & `cellmaps_pipeline-0.1.0a7/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_pipeline-0.1.0a6/docs/versioningscheme.rst` & `cellmaps_pipeline-0.1.0a7/docs/versioningscheme.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_pipeline-0.1.0a6/setup.py` & `cellmaps_pipeline-0.1.0a7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,22 +23,23 @@
 
 with open('README.rst') as readme_file:
     readme = readme_file.read()
 
 with open('HISTORY.rst') as history_file:
     history = history_file.read()
 
-requirements = ['cellmaps_utils==0.1.0a14',
+requirements = ['cellmaps_utils==0.1.0a15',
                 'cellmaps_imagedownloader==0.1.0a7',
                 'cellmaps_ppidownloader==0.1.0a3',
-                'cellmaps_image_embedding==0.1.0a7',
-                'cellmaps_ppi_embedding==0.1.0a4',
-                'cellmaps_coembedding==0.1.0a4',
-                'cellmaps_generate_hierarchy==0.1.0a6',
-                'networkx>=2.8,<2.9']
+                'cellmaps_image_embedding==0.1.0a8',
+                'cellmaps_ppi_embedding==0.1.0a5',
+                'cellmaps_coembedding==0.1.0a5',
+                'cellmaps_generate_hierarchy==0.1.0a7',
+                'networkx>=2.8,<2.9',
+                'tqdm']
 
 setup_requirements = [ ]
 
 test_requirements = [ ]
 
 setup(
     author=author,
```

### Comparing `cellmaps_pipeline-0.1.0a6/tests/test_cellmaps_pipelinecmd.py` & `cellmaps_pipeline-0.1.0a7/tests/test_cellmaps_pipelinecmd.py`

 * *Files identical despite different names*

### Comparing `cellmaps_pipeline-0.1.0a6/tests/test_cellmapspipeline.py` & `cellmaps_pipeline-0.1.0a7/tests/test_cellmapspipeline.py`

 * *Files identical despite different names*

### Comparing `cellmaps_pipeline-0.1.0a6/tests/test_integration_cellmaps_pipeline.py` & `cellmaps_pipeline-0.1.0a7/tests/test_integration_cellmaps_pipeline.py`

 * *Files identical despite different names*

