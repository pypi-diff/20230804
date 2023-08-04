# Comparing `tmp/dask_labextension-6.2.0.tar.gz` & `tmp/dask_labextension-7.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dask_labextension-6.2.0.tar", last modified: Tue Aug  1 20:27:26 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `dask_labextension-6.2.0.tar` & `dask_labextension-7.0.0.tar`

### file list

```diff
@@ -1,62 +1,49 @@
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-08-01 20:27:26.726349 dask_labextension-6.2.0/
--rw-r--r--   0 james      (501) staff       (20)     1532 2023-08-01 20:08:53.000000 dask_labextension-6.2.0/LICENSE
--rw-r--r--   0 james      (501) staff       (20)      625 2023-08-01 20:23:30.000000 dask_labextension-6.2.0/MANIFEST.in
--rw-r--r--   0 james      (501) staff       (20)     8480 2023-08-01 20:27:26.726416 dask_labextension-6.2.0/PKG-INFO
--rw-r--r--   0 james      (501) staff       (20)     7744 2023-08-01 20:23:30.000000 dask_labextension-6.2.0/README.md
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-08-01 20:27:26.726832 dask_labextension-6.2.0/dask_labextension/
--rw-r--r--   0 james      (501) staff       (20)     1581 2023-08-01 20:09:43.000000 dask_labextension-6.2.0/dask_labextension/__init__.py
--rw-r--r--   0 james      (501) staff       (20)      536 2023-08-01 20:27:26.726869 dask_labextension-6.2.0/dask_labextension/_version.py
--rw-r--r--   0 james      (501) staff       (20)     2893 2023-08-01 20:09:43.000000 dask_labextension-6.2.0/dask_labextension/clusterhandler.py
--rw-r--r--   0 james      (501) staff       (20)      297 2023-08-01 20:08:53.000000 dask_labextension-6.2.0/dask_labextension/config.py
--rw-r--r--   0 james      (501) staff       (20)     7539 2023-08-01 20:09:43.000000 dask_labextension-6.2.0/dask_labextension/dashboardhandler.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-08-01 20:27:26.722708 dask_labextension-6.2.0/dask_labextension/labextension/
--rw-r--r--   0 james      (501) staff       (20)     3639 2023-08-01 20:27:26.000000 dask_labextension-6.2.0/dask_labextension/labextension/package.json
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-08-01 20:27:26.717866 dask_labextension-6.2.0/dask_labextension/labextension/schemas/
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-08-01 20:27:26.722957 dask_labextension-6.2.0/dask_labextension/labextension/schemas/dask-labextension/
--rw-r--r--   0 james      (501) staff       (20)     3523 2023-08-01 20:27:25.000000 dask_labextension-6.2.0/dask_labextension/labextension/schemas/dask-labextension/package.json.orig
--rw-r--r--   0 james      (501) staff       (20)     2822 2023-08-01 20:27:25.000000 dask_labextension-6.2.0/dask_labextension/labextension/schemas/dask-labextension/plugin.json
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-08-01 20:27:26.723598 dask_labextension-6.2.0/dask_labextension/labextension/static/
--rw-r--r--   0 james      (501) staff       (20)     8783 2023-08-01 20:27:26.000000 dask_labextension-6.2.0/dask_labextension/labextension/static/114.f9e3bc980911cf750147.js
--rw-r--r--   0 james      (501) staff       (20)    43202 2023-08-01 20:27:26.000000 dask_labextension-6.2.0/dask_labextension/labextension/static/224.86c44b816becca807a99.js
--rw-r--r--   0 james      (501) staff       (20)     7818 2023-08-01 20:27:26.000000 dask_labextension-6.2.0/dask_labextension/labextension/static/remoteEntry.48341a7428463ba2c6bb.js
--rw-r--r--   0 james      (501) staff       (20)      118 2023-08-01 20:27:25.000000 dask_labextension-6.2.0/dask_labextension/labextension/static/style.js
--rw-r--r--   0 james      (501) staff       (20)     2590 2023-08-01 20:27:26.000000 dask_labextension-6.2.0/dask_labextension/labextension/static/third-party-licenses.json
--rw-r--r--   0 james      (501) staff       (20)      361 2023-08-01 20:09:43.000000 dask_labextension-6.2.0/dask_labextension/labextension.yaml
--rw-r--r--   0 james      (501) staff       (20)     9359 2023-08-01 20:09:43.000000 dask_labextension-6.2.0/dask_labextension/manager.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-08-01 20:27:26.723714 dask_labextension-6.2.0/dask_labextension/tests/
--rw-r--r--   0 james      (501) staff       (20)     5094 2023-08-01 20:09:43.000000 dask_labextension-6.2.0/dask_labextension/tests/test_manager.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-08-01 20:27:26.722579 dask_labextension-6.2.0/dask_labextension.egg-info/
--rw-r--r--   0 james      (501) staff       (20)     8480 2023-08-01 20:27:26.000000 dask_labextension-6.2.0/dask_labextension.egg-info/PKG-INFO
--rw-r--r--   0 james      (501) staff       (20)     1473 2023-08-01 20:27:26.000000 dask_labextension-6.2.0/dask_labextension.egg-info/SOURCES.txt
--rw-r--r--   0 james      (501) staff       (20)        1 2023-08-01 20:27:26.000000 dask_labextension-6.2.0/dask_labextension.egg-info/dependency_links.txt
--rw-r--r--   0 james      (501) staff       (20)        1 2023-08-01 20:27:00.000000 dask_labextension-6.2.0/dask_labextension.egg-info/not-zip-safe
--rw-r--r--   0 james      (501) staff       (20)       90 2023-08-01 20:27:26.000000 dask_labextension-6.2.0/dask_labextension.egg-info/requires.txt
--rw-r--r--   0 james      (501) staff       (20)       18 2023-08-01 20:27:26.000000 dask_labextension-6.2.0/dask_labextension.egg-info/top_level.txt
--rw-r--r--   0 james      (501) staff       (20)      195 2023-08-01 20:09:43.000000 dask_labextension-6.2.0/install.json
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-08-01 20:27:26.718234 dask_labextension-6.2.0/jupyter-config/
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-08-01 20:27:26.723840 dask_labextension-6.2.0/jupyter-config/jupyter_notebook_config.d/
--rw-r--r--   0 james      (501) staff       (20)       94 2023-08-01 20:08:53.000000 dask_labextension-6.2.0/jupyter-config/jupyter_notebook_config.d/dask_labextension.json
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-08-01 20:27:26.724831 dask_labextension-6.2.0/jupyter-config/jupyter_server_config.d/
--rw-r--r--   0 james      (501) staff       (20)       92 2023-08-01 20:09:43.000000 dask_labextension-6.2.0/jupyter-config/jupyter_server_config.d/dask_labextension.json
--rw-r--r--   0 james      (501) staff       (20)     3523 2023-08-01 20:25:35.000000 dask_labextension-6.2.0/package.json
--rw-r--r--   0 james      (501) staff       (20)      157 2023-08-01 20:09:43.000000 dask_labextension-6.2.0/pyproject.toml
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-08-01 20:27:26.725031 dask_labextension-6.2.0/schema/
--rw-r--r--   0 james      (501) staff       (20)     2822 2023-08-01 20:09:43.000000 dask_labextension-6.2.0/schema/plugin.json
--rw-r--r--   0 james      (501) staff       (20)      738 2023-08-01 20:27:26.726709 dask_labextension-6.2.0/setup.cfg
--rw-r--r--   0 james      (501) staff       (20)     2861 2023-08-01 20:23:30.000000 dask_labextension-6.2.0/setup.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-08-01 20:27:26.725773 dask_labextension-6.2.0/src/
--rw-r--r--   0 james      (501) staff       (20)    23013 2023-08-01 20:09:43.000000 dask_labextension-6.2.0/src/clusters.tsx
--rw-r--r--   0 james      (501) staff       (20)    17355 2023-08-01 20:09:43.000000 dask_labextension-6.2.0/src/dashboard.tsx
--rw-r--r--   0 james      (501) staff       (20)    25542 2023-08-01 20:09:43.000000 dask_labextension-6.2.0/src/index.ts
--rw-r--r--   0 james      (501) staff       (20)     7137 2023-08-01 20:08:53.000000 dask_labextension-6.2.0/src/scaling.tsx
--rw-r--r--   0 james      (501) staff       (20)     2657 2023-08-01 20:08:53.000000 dask_labextension-6.2.0/src/sidebar.ts
--rw-r--r--   0 james      (501) staff       (20)       74 2023-08-01 20:09:43.000000 dask_labextension-6.2.0/src/svg.d.ts
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-08-01 20:27:26.726227 dask_labextension-6.2.0/style/
--rw-r--r--   0 james      (501) staff       (20)      246 2023-08-01 20:08:53.000000 dask_labextension-6.2.0/style/code-dark.svg
--rw-r--r--   0 james      (501) staff       (20)      246 2023-08-01 20:08:53.000000 dask_labextension-6.2.0/style/code-light.svg
--rw-r--r--   0 james      (501) staff       (20)     1607 2023-08-01 20:09:43.000000 dask_labextension-6.2.0/style/dask.svg
--rw-r--r--   0 james      (501) staff       (20)     6941 2023-08-01 20:09:43.000000 dask_labextension-6.2.0/style/index.css
--rw-r--r--   0 james      (501) staff       (20)       75 2023-08-01 20:09:43.000000 dask_labextension-6.2.0/tsconfig.eslint.json
--rw-r--r--   0 james      (501) staff       (20)      555 2023-08-01 20:09:43.000000 dask_labextension-6.2.0/tsconfig.json
--rw-r--r--   0 james      (501) staff       (20)    69015 2023-08-01 20:09:43.000000 dask_labextension-6.2.0/versioneer.py
--rw-r--r--   0 james      (501) staff       (20)   214431 2023-08-01 20:23:30.000000 dask_labextension-6.2.0/yarn.lock
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 dask_labextension-7.0.0/.eslintignore
+-rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 dask_labextension-7.0.0/.eslintrc.js
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 dask_labextension-7.0.0/.flake8
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 dask_labextension-7.0.0/.gitattributes
+-rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 dask_labextension-7.0.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 dask_labextension-7.0.0/.prettierignore
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 dask_labextension-7.0.0/.prettierrc
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 dask_labextension-7.0.0/.yarnrc.yml
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 dask_labextension-7.0.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0  1626828 2020-02-02 00:00:00.000000 dask_labextension-7.0.0/dask.png
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 dask_labextension-7.0.0/install.json
+-rw-r--r--   0        0        0     3742 2020-02-02 00:00:00.000000 dask_labextension-7.0.0/package.json
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 dask_labextension-7.0.0/tsconfig.eslint.json
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 dask_labextension-7.0.0/tsconfig.json
+-rw-r--r--   0        0        0   216494 2020-02-02 00:00:00.000000 dask_labextension-7.0.0/yarn.lock
+-rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 dask_labextension-7.0.0/dask_labextension/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 dask_labextension-7.0.0/dask_labextension/_version.py
+-rw-r--r--   0        0        0     2893 2020-02-02 00:00:00.000000 dask_labextension-7.0.0/dask_labextension/clusterhandler.py
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 dask_labextension-7.0.0/dask_labextension/config.py
+-rw-r--r--   0        0        0     7539 2020-02-02 00:00:00.000000 dask_labextension-7.0.0/dask_labextension/dashboardhandler.py
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 dask_labextension-7.0.0/dask_labextension/labextension.yaml
+-rw-r--r--   0        0        0     9359 2020-02-02 00:00:00.000000 dask_labextension-7.0.0/dask_labextension/manager.py
+-rw-r--r--   0        0        0     3524 2020-02-02 00:00:00.000000 dask_labextension-7.0.0/dask_labextension/labextension/package.json
+-rw-r--r--   0        0        0     3742 2020-02-02 00:00:00.000000 dask_labextension-7.0.0/dask_labextension/labextension/schemas/dask-labextension/package.json.orig
+-rw-r--r--   0        0        0     2822 2020-02-02 00:00:00.000000 dask_labextension-7.0.0/dask_labextension/labextension/schemas/dask-labextension/plugin.json
+-rw-r--r--   0        0        0    43845 2020-02-02 00:00:00.000000 dask_labextension-7.0.0/dask_labextension/labextension/static/11.92ba9866db6ad7a7f70f.js
+-rw-r--r--   0        0        0     7301 2020-02-02 00:00:00.000000 dask_labextension-7.0.0/dask_labextension/labextension/static/remoteEntry.55eb452b48896f869659.js
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 dask_labextension-7.0.0/dask_labextension/labextension/static/style.js
+-rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 dask_labextension-7.0.0/dask_labextension/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 dask_labextension-7.0.0/dask_labextension/tests/__init__.py
+-rw-r--r--   0        0        0     5094 2020-02-02 00:00:00.000000 dask_labextension-7.0.0/dask_labextension/tests/test_manager.py
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 dask_labextension-7.0.0/jupyter-config/jupyter_notebook_config.d/dask_labextension.json
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 dask_labextension-7.0.0/jupyter-config/jupyter_server_config.d/dask_labextension.json
+-rw-r--r--   0        0        0     2822 2020-02-02 00:00:00.000000 dask_labextension-7.0.0/schema/plugin.json
+-rw-r--r--   0        0        0    23025 2020-02-02 00:00:00.000000 dask_labextension-7.0.0/src/clusters.tsx
+-rw-r--r--   0        0        0    17355 2020-02-02 00:00:00.000000 dask_labextension-7.0.0/src/dashboard.tsx
+-rw-r--r--   0        0        0    25676 2020-02-02 00:00:00.000000 dask_labextension-7.0.0/src/index.ts
+-rw-r--r--   0        0        0     7137 2020-02-02 00:00:00.000000 dask_labextension-7.0.0/src/scaling.tsx
+-rw-r--r--   0        0        0     2657 2020-02-02 00:00:00.000000 dask_labextension-7.0.0/src/sidebar.ts
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 dask_labextension-7.0.0/src/svg.d.ts
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 dask_labextension-7.0.0/style/code-dark.svg
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 dask_labextension-7.0.0/style/code-light.svg
+-rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 dask_labextension-7.0.0/style/dask.svg
+-rw-r--r--   0        0        0     6941 2020-02-02 00:00:00.000000 dask_labextension-7.0.0/style/index.css
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 dask_labextension-7.0.0/.gitignore
+-rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 dask_labextension-7.0.0/LICENSE
+-rw-r--r--   0        0        0     8390 2020-02-02 00:00:00.000000 dask_labextension-7.0.0/README.md
+-rw-r--r--   0        0        0     3009 2020-02-02 00:00:00.000000 dask_labextension-7.0.0/pyproject.toml
+-rw-r--r--   0        0        0    11334 2020-02-02 00:00:00.000000 dask_labextension-7.0.0/PKG-INFO
```

### Comparing `dask_labextension-6.2.0/LICENSE` & `dask_labextension-7.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dask_labextension-6.2.0/PKG-INFO` & `dask_labextension-7.0.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,10 @@
-Metadata-Version: 2.1
-Name: dask_labextension
-Version: 6.2.0
-Summary: A JupyterLab extension for Dask.
-Home-page: https://github.com/dask/dask-labextension
-Author: Ian Rose, Matt Rocklin, Jacob Tomlinson
-License: BSD-3-Clause
-Keywords: dask,Jupyter,JupyterLab,JupyterLab3
-Platform: Linux
-Platform: Mac OS X
-Platform: Windows
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Framework :: Jupyter
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Dask JupyterLab Extension
 
-[![Build Status](https://travis-ci.org/dask/dask-labextension.svg?branch=main)](https://travis-ci.org/dask/dask-labextension) [![Version](https://img.shields.io/npm/v/dask-labextension.svg)](https://www.npmjs.com/package/dask-labextension) [![Downloads](https://img.shields.io/npm/dm/dask-labextension.svg)](https://www.npmjs.com/package/dask-labextension) [![Dependencies](https://img.shields.io/librariesio/release/npm/dask-labextension.svg)](https://libraries.io/npm/dask-labextension)
+[![Build Status](https://github.com/dask/dask-labextension/actions/workflows/python.yaml/badge.svg)](https://github.com/dask/dask-labextension/actions/workflows/python.yaml) [![Version](https://img.shields.io/npm/v/dask-labextension.svg)](https://www.npmjs.com/package/dask-labextension) [![Downloads](https://img.shields.io/npm/dm/dask-labextension.svg)](https://www.npmjs.com/package/dask-labextension) [![Dependencies](https://img.shields.io/librariesio/release/npm/dask-labextension.svg)](https://libraries.io/npm/dask-labextension)
 
 This package provides a JupyterLab extension to manage Dask clusters,
 as well as embed Dask's dashboard plots directly into JupyterLab panes.
 
 ![Dask Extension](./dask.png)
 
 ## Explanatory Video (5 minutes)
@@ -50,37 +28,45 @@
 One source common to Python users is the conda package manager.
 
 ```bash
 conda install jupyterlab
 conda install -c conda-forge nodejs
 ```
 
-### JupyterLab 3.0 or greater
+### JupyterLab 4.x
 
-You should be able to install this extension with pip or conda,
+Install the latest version of the extension for the JupyterLab 4
+support. You should be able to install this extension with pip or conda,
 and start using it immediately, e.g.
 
 ```bash
 pip install dask-labextension
 ```
 
 ### JupyterLab 3.x
 
-This extension includes both client-side and server-side components.
-Prior to JupyterLab 3.0 these needed to be installed separately,
-with node available on the machine.
+For JupyterLab 3.x, use lastest supported version `6.2.0`.
+
+```bash
+pip install dask-labextension==6.2.0
+```
+
+### JupyterLab 2.x
+
+Prior to JupyterLab 3.0 client-side and server-side components needed
+to be installed separately, with node available on the machine.
 
 The server-side component can be installed via pip or conda-forge:
 
 ```bash
-pip install dask_labextension
+pip install 'dask_labextension<5'
 ```
 
 ```bash
-conda install -c conda-forge dask-labextension
+conda install -c conda-forge 'dask-labextension<5'
 ```
 
 You then build the client-side extension into JupyterLab with:
 
 ```bash
 jupyter labextension install dask-labextension
 ```
@@ -236,26 +222,39 @@
 ## Publishing
 
 This extension contains a front-end component written in TypeScript
 and a back-end component written in Python.
 The front-end is compiled to Javascript during the build process
 and is distributed as static assets along with the Python package.
 
-_Note: Package versions are not prefixed with the letter `v`. You will need to disable this._
-
-```console
-$ jlpm config set version-tag-prefix ""
-```
-
 ### Release process
 
-This requires `node`, `build`, and `twine` to be installed.
+This requires `node`, `build`, `hatch` and `twine` to be installed.
 
 ```bash
-jlpm version [--major|--minor|--patch]  # updates package.json and creates git commit and tag
+# To set version (e.g. 7.0.0). hatch will update version string in package.json
+hatch version "7.0.0"
+
+# Examples of bumping version
+# minor bump
+hatch version minor  # Bumps to 7.1.0
+# beta pre-release bump
+# If published to pypi this can be installed with the --pre flag to pip
+hatch version b  # Bumps to 7.1.0b0
+# bump minor and beta
+hatch version minor,b  # Bumps to 7.2.0b0
+# release all of the --pre-release flags such as alpha beta rc
+hatch release  # Bumps to 7.2.0
+
+# git commit after bumping version
+git add package.json && git commit -m "Bump version: {version}"
+# Tag this version
+git tag {version}
+
+# Finally push to main, build and upload package to PyPI
 git push upstream main && git push upstream main --tags  # pushes to GitHub
 python -m build .  # Build the package
 twine upload dist/*  # Upload the package to PyPI
 ```
 
 ### Handling Javascript package version conflicts
```

#### html2text {}

```diff
@@ -1,74 +1,67 @@
-Metadata-Version: 2.1 Name: dask_labextension Version: 6.2.0 Summary: A
-JupyterLab extension for Dask. Home-page: https://github.com/dask/dask-
-labextension Author: Ian Rose, Matt Rocklin, Jacob Tomlinson License: BSD-3-
-Clause Keywords: dask,Jupyter,JupyterLab,JupyterLab3 Platform: Linux Platform:
-Mac OS X Platform: Windows Classifier: License :: OSI Approved :: BSD License
-Classifier: Programming Language :: Python Classifier: Programming Language ::
-Python :: 3 Classifier: Programming Language :: Python :: 3.6 Classifier:
-Programming Language :: Python :: 3.7 Classifier: Programming Language ::
-Python :: 3.8 Classifier: Framework :: Jupyter Requires-Python: >=3.6
-Description-Content-Type: text/markdown License-File: LICENSE # Dask JupyterLab
-Extension [![Build Status](https://travis-ci.org/dask/dask-
-labextension.svg?branch=main)](https://travis-ci.org/dask/dask-labextension) [!
-[Version](https://img.shields.io/npm/v/dask-labextension.svg)](https://
-www.npmjs.com/package/dask-labextension) [![Downloads](https://img.shields.io/
-npm/dm/dask-labextension.svg)](https://www.npmjs.com/package/dask-labextension)
-[![Dependencies](https://img.shields.io/librariesio/release/npm/dask-
+# Dask JupyterLab Extension [![Build Status](https://github.com/dask/dask-
+labextension/actions/workflows/python.yaml/badge.svg)](https://github.com/dask/
+dask-labextension/actions/workflows/python.yaml) [![Version](https://
+img.shields.io/npm/v/dask-labextension.svg)](https://www.npmjs.com/package/
+dask-labextension) [![Downloads](https://img.shields.io/npm/dm/dask-
+labextension.svg)](https://www.npmjs.com/package/dask-labextension) [!
+[Dependencies](https://img.shields.io/librariesio/release/npm/dask-
 labextension.svg)](https://libraries.io/npm/dask-labextension) This package
 provides a JupyterLab extension to manage Dask clusters, as well as embed
 Dask's dashboard plots directly into JupyterLab panes. ![Dask Extension](./
 dask.png) ## Explanatory Video (5 minutes) [Dask_+_JupyterLab_Screencast] ##
 Requirements JupyterLab >= 1.0 distributed >= 1.24.1 ## Installation To install
 the Dask JupyterLab extension you will need to have JupyterLab installed. For
 JupyterLab < 3.0, you will also need [Node.js](https://nodejs.org/) version >=
 12. These are available through a variety of sources. One source common to
 Python users is the conda package manager. ```bash conda install jupyterlab
-conda install -c conda-forge nodejs ``` ### JupyterLab 3.0 or greater You
-should be able to install this extension with pip or conda, and start using it
-immediately, e.g. ```bash pip install dask-labextension ``` ### JupyterLab 3.x
-This extension includes both client-side and server-side components. Prior to
-JupyterLab 3.0 these needed to be installed separately, with node available on
-the machine. The server-side component can be installed via pip or conda-forge:
-```bash pip install dask_labextension ``` ```bash conda install -c conda-forge
-dask-labextension ``` You then build the client-side extension into JupyterLab
-with: ```bash jupyter labextension install dask-labextension ``` If you are
-running Notebook 5.2 or earlier, enable the server extension by running ```bash
-jupyter serverextension enable --py --sys-prefix dask_labextension ``` ##
-Configuration of Dask cluster management This extension has the ability to
-launch and manage several kinds of Dask clusters, including local clusters and
-kubernetes clusters. Options for how to launch these clusters are set via the
-[dask configuration system](http://docs.dask.org/en/latest/
-configuration.html#configuration), typically a `.yml` file on disk. By default
-the extension launches a `LocalCluster`, for which the configuration is:
-```yaml labextension: factory: module: 'dask.distributed' class: 'LocalCluster'
-args: [] kwargs: {} default: workers: null adapt: null # minimum: 0 # maximum:
-10 initial: [] # - name: "My Big Cluster" # workers: 100 # - name: "Adaptive
-Cluster" # adapt: # minimum: 0 # maximum: 50 ``` In this configuration,
-`factory` gives the module, class name, and arguments needed to create the
-cluster. The `default` key describes the initial number of workers for the
-cluster, as well as whether it is adaptive. The `initial` key gives a list of
-initial clusters to start upon launch of the notebook server. In addition to
-`LocalCluster`, this extension has been used to launch several other Dask
-cluster objects, a few examples of which are: - A SLURM cluster, using ```yaml
-labextension: factory: module: 'dask_jobqueue' class: 'SLURMCluster' args: []
-kwargs: {} ``` - A PBS cluster, using ```yaml labextension: factory: module:
-'dask_jobqueue' class: 'PBSCluster' args: [] kwargs: {} ``` - A [Kubernetes
-cluster](https://github.com/pangeo-data/pangeo-cloud-federation/blob/
-8f7f4bf9963ef1ed180dd20c952ff1aa8df54ca2/deployments/ocean/image/binder/
-dask_config.yaml#L37-L42), using ```yaml labextension: factory: module:
-dask_kubernetes class: KubeCluster args: [] kwargs: {} ``` ## Configuring a
-default layout This extension can store a default layout for the Dask dashboard
-panes, which is useful if you find yourself reaching for the same dashboard
-charts over and over. You can launch the default layout via the command
-palette, or by going to the File menu and choosing "Launch Dask Dashboard
-Layout". Default layouts can be configured via the JupyterLab config system
-(either using the JSON editor or the user interface). Specify a layout by
-writing a JSON object keyed by the [individual charts](https://github.com/dask/
-distributed/blob/f31fbde748294065ed70dd5c4399821fa664a9f1/distributed/
+conda install -c conda-forge nodejs ``` ### JupyterLab 4.x Install the latest
+version of the extension for the JupyterLab 4 support. You should be able to
+install this extension with pip or conda, and start using it immediately, e.g.
+```bash pip install dask-labextension ``` ### JupyterLab 3.x For JupyterLab
+3.x, use lastest supported version `6.2.0`. ```bash pip install dask-
+labextension==6.2.0 ``` ### JupyterLab 2.x Prior to JupyterLab 3.0 client-side
+and server-side components needed to be installed separately, with node
+available on the machine. The server-side component can be installed via pip or
+conda-forge: ```bash pip install 'dask_labextension<5' ``` ```bash conda
+install -c conda-forge 'dask-labextension<5' ``` You then build the client-side
+extension into JupyterLab with: ```bash jupyter labextension install dask-
+labextension ``` If you are running Notebook 5.2 or earlier, enable the server
+extension by running ```bash jupyter serverextension enable --py --sys-prefix
+dask_labextension ``` ## Configuration of Dask cluster management This
+extension has the ability to launch and manage several kinds of Dask clusters,
+including local clusters and kubernetes clusters. Options for how to launch
+these clusters are set via the [dask configuration system](http://
+docs.dask.org/en/latest/configuration.html#configuration), typically a `.yml`
+file on disk. By default the extension launches a `LocalCluster`, for which the
+configuration is: ```yaml labextension: factory: module: 'dask.distributed'
+class: 'LocalCluster' args: [] kwargs: {} default: workers: null adapt: null #
+minimum: 0 # maximum: 10 initial: [] # - name: "My Big Cluster" # workers: 100
+# - name: "Adaptive Cluster" # adapt: # minimum: 0 # maximum: 50 ``` In this
+configuration, `factory` gives the module, class name, and arguments needed to
+create the cluster. The `default` key describes the initial number of workers
+for the cluster, as well as whether it is adaptive. The `initial` key gives a
+list of initial clusters to start upon launch of the notebook server. In
+addition to `LocalCluster`, this extension has been used to launch several
+other Dask cluster objects, a few examples of which are: - A SLURM cluster,
+using ```yaml labextension: factory: module: 'dask_jobqueue' class:
+'SLURMCluster' args: [] kwargs: {} ``` - A PBS cluster, using ```yaml
+labextension: factory: module: 'dask_jobqueue' class: 'PBSCluster' args: []
+kwargs: {} ``` - A [Kubernetes cluster](https://github.com/pangeo-data/pangeo-
+cloud-federation/blob/8f7f4bf9963ef1ed180dd20c952ff1aa8df54ca2/deployments/
+ocean/image/binder/dask_config.yaml#L37-L42), using ```yaml labextension:
+factory: module: dask_kubernetes class: KubeCluster args: [] kwargs: {} ``` ##
+Configuring a default layout This extension can store a default layout for the
+Dask dashboard panes, which is useful if you find yourself reaching for the
+same dashboard charts over and over. You can launch the default layout via the
+command palette, or by going to the File menu and choosing "Launch Dask
+Dashboard Layout". Default layouts can be configured via the JupyterLab config
+system (either using the JSON editor or the user interface). Specify a layout
+by writing a JSON object keyed by the [individual charts](https://github.com/
+dask/distributed/blob/f31fbde748294065ed70dd5c4399821fa664a9f1/distributed/
 dashboard/scheduler.py#L72-L117) you would like to open. Each chart is opened
 with a `mode`, and a `ref`. `mode` refers to how the chart is to be added to
 the workspace. For example, if you want to split a panel and add the new one to
 the right, choose `split-right`. Other options are `split-top`, `split-bottom`,
 `split-left`, `tab-after`, and `tab-before`. `ref` refers to the panel to which
 `mode` is applied, and might be the names of other dashboard panels. If `ref`
 is `null`, the panel in question is added at the top of the layout hierarchy. A
@@ -87,19 +80,25 @@
 directory as an extension ``` To rebuild the extension: ```bash jlpm build ```
 You should then be able to refresh the JupyterLab page and it will pick up the
 changes to the extension. To run an editable install of the server extension,
 run ```bash pip install -e . jupyter serverextension enable --sys-prefix
 dask_labextension ``` ## Publishing This extension contains a front-end
 component written in TypeScript and a back-end component written in Python. The
 front-end is compiled to Javascript during the build process and is distributed
-as static assets along with the Python package. _Note: Package versions are not
-prefixed with the letter `v`. You will need to disable this._ ```console $ jlpm
-config set version-tag-prefix "" ``` ### Release process This requires `node`,
-`build`, and `twine` to be installed. ```bash jlpm version [--major|--minor|--
-patch] # updates package.json and creates git commit and tag git push upstream
-main && git push upstream main --tags # pushes to GitHub python -m build . #
-Build the package twine upload dist/* # Upload the package to PyPI ``` ###
-Handling Javascript package version conflicts Unlike Python, Javascript
-packages can include more than one version of the same dependency. Usually the
-`yarn` package manager handles this okay, but occasionally you might end up
-with conflicting versions, or with unexpected package bloat. You can try to fix
-this by deduplicating dependencies: ```bash jlpm yarn-deduplicate -s fewer ```
+as static assets along with the Python package. ### Release process This
+requires `node`, `build`, `hatch` and `twine` to be installed. ```bash # To set
+version (e.g. 7.0.0). hatch will update version string in package.json hatch
+version "7.0.0" # Examples of bumping version # minor bump hatch version minor
+# Bumps to 7.1.0 # beta pre-release bump # If published to pypi this can be
+installed with the --pre flag to pip hatch version b # Bumps to 7.1.0b0 # bump
+minor and beta hatch version minor,b # Bumps to 7.2.0b0 # release all of the --
+pre-release flags such as alpha beta rc hatch release # Bumps to 7.2.0 # git
+commit after bumping version git add package.json && git commit -m "Bump
+version: {version}" # Tag this version git tag {version} # Finally push to
+main, build and upload package to PyPI git push upstream main && git push
+upstream main --tags # pushes to GitHub python -m build . # Build the package
+twine upload dist/* # Upload the package to PyPI ``` ### Handling Javascript
+package version conflicts Unlike Python, Javascript packages can include more
+than one version of the same dependency. Usually the `yarn` package manager
+handles this okay, but occasionally you might end up with conflicting versions,
+or with unexpected package bloat. You can try to fix this by deduplicating
+dependencies: ```bash jlpm yarn-deduplicate -s fewer ```
```

### Comparing `dask_labextension-6.2.0/dask_labextension/__init__.py` & `dask_labextension-7.0.0/dask_labextension/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,18 +3,15 @@
 from jupyter_server.utils import url_path_join
 
 from . import config
 from .clusterhandler import DaskClusterHandler
 from .dashboardhandler import DaskDashboardCheckHandler, DaskDashboardHandler
 
 
-from ._version import get_versions
-
-__version__ = get_versions()["version"]
-del get_versions
+from ._version import __version__
 
 
 def _jupyter_labextension_paths():
     return [
         {
             "src": "labextension",
             "dest": "dask-labextension",
```

### Comparing `dask_labextension-6.2.0/dask_labextension/clusterhandler.py` & `dask_labextension-7.0.0/dask_labextension/clusterhandler.py`

 * *Files identical despite different names*

### Comparing `dask_labextension-6.2.0/dask_labextension/dashboardhandler.py` & `dask_labextension-7.0.0/dask_labextension/dashboardhandler.py`

 * *Files identical despite different names*

### Comparing `dask_labextension-6.2.0/dask_labextension/labextension/package.json` & `dask_labextension-7.0.0/dask_labextension/labextension/package.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8063214869281046%*

 * *Differences: {"'author'": "{replace: OrderedDict([('name', 'Ian Rose, Matt Rocklin, Jacob Tomlinson')])}",*

 * * "'dependencies'": "{'@jupyterlab/application': '^4.0.0', '@jupyterlab/apputils': '^4.0.0', "*

 * *                   "'@jupyterlab/codeeditor': '^4.0.0', '@jupyterlab/console': '^4.0.0', "*

 * *                   "'@jupyterlab/coreutils': '^6.0.0', '@jupyterlab/docregistry': '^4.0.0', "*

 * *                   "'@jupyterlab/mainmenu': '^4.0.0', '@jupyterlab/nbformat': '^4.0.0', "*

 * *                   "'@jupyterlab/notebook': '^4.0 […]*

```diff
@@ -1,89 +1,85 @@
 {
-    "author": "Ian Rose, Matt Rocklin, Jacob Tomlinson",
+    "author": {
+        "name": "Ian Rose, Matt Rocklin, Jacob Tomlinson"
+    },
     "bugs": {
         "url": "https://github.com/dask/dask-labextension/issues"
     },
     "dependencies": {
-        "@jupyterlab/application": "^3.0.0",
-        "@jupyterlab/apputils": "^3.0.0",
-        "@jupyterlab/codeeditor": "^3.0.0",
-        "@jupyterlab/console": "^3.0.0",
-        "@jupyterlab/coreutils": "^5.0.0",
-        "@jupyterlab/docregistry": "^3.4.3",
-        "@jupyterlab/mainmenu": "^3.0.0",
-        "@jupyterlab/nbformat": "^3.0.0",
-        "@jupyterlab/notebook": "^3.0.0",
-        "@jupyterlab/services": "^6.0.0",
-        "@jupyterlab/settingregistry": "^3.0.0",
-        "@jupyterlab/statedb": "^3.0.0",
-        "@jupyterlab/ui-components": "^3.0.0",
-        "@lumino/algorithm": "^1.3.3",
-        "@lumino/coreutils": "^1.5.3",
-        "@lumino/domutils": "^1.2.3",
-        "@lumino/dragdrop": "^1.7.1",
-        "@lumino/messaging": "^1.4.3",
-        "@lumino/polling": "^1.0.4",
-        "@lumino/signaling": "^1.4.3",
-        "@lumino/widgets": "^1.17.0",
-        "react": "^17.0.1",
-        "react-dom": "^17.0.1"
+        "@jupyterlab/application": "^4.0.0",
+        "@jupyterlab/apputils": "^4.0.0",
+        "@jupyterlab/codeeditor": "^4.0.0",
+        "@jupyterlab/console": "^4.0.0",
+        "@jupyterlab/coreutils": "^6.0.0",
+        "@jupyterlab/docregistry": "^4.0.0",
+        "@jupyterlab/mainmenu": "^4.0.0",
+        "@jupyterlab/nbformat": "^4.0.0",
+        "@jupyterlab/notebook": "^4.0.0",
+        "@jupyterlab/services": "^7.0.0",
+        "@jupyterlab/settingregistry": "^4.0.0",
+        "@jupyterlab/statedb": "^4.0.0",
+        "@jupyterlab/ui-components": "^4.0.0",
+        "@lumino/algorithm": "^2.0.0",
+        "@lumino/coreutils": "^2.0.0",
+        "@lumino/domutils": "^2.0.0",
+        "@lumino/dragdrop": "^2.0.0",
+        "@lumino/messaging": "^2.0.0",
+        "@lumino/polling": "^2.0.0",
+        "@lumino/signaling": "^2.0.0",
+        "@lumino/widgets": "^2.0.0",
+        "react": "^18.0.0",
+        "react-dom": "^18.0.0"
     },
     "description": "A JupyterLab extension for Dask.",
     "devDependencies": {
-        "@jupyterlab/builder": "^3.0.0",
-        "@types/react": "^17.0.0",
-        "@types/react-dom": "^17.0.0",
-        "@typescript-eslint/eslint-plugin": "^4.18.0",
-        "@typescript-eslint/parser": "^4.18.0",
-        "eslint": "^7.14.0",
-        "eslint-config-prettier": "^6.10.1",
-        "eslint-plugin-prettier": "^3.1.4",
+        "@jupyterlab/builder": "^4.0.0",
+        "@types/react": "^18.0.0",
+        "@types/react-dom": "^18.0.0",
+        "@typescript-eslint/eslint-plugin": "^5.59.0",
+        "@typescript-eslint/parser": "^5.59.0",
+        "eslint": "^8.4.0",
+        "eslint-config-prettier": "^8.8.0",
+        "eslint-plugin-prettier": "^4.2.1",
         "eslint-plugin-react": "^7.21.5",
         "mkdirp": "^1.0.3",
         "mocha": "^6.2.0",
         "npm-run-all": "^4.1.5",
-        "prettier": "^2.1.1",
-        "rimraf": "^3.0.2",
-        "typescript": "~4.1.3",
-        "yarn": "1.22.0",
-        "yarn-deduplicate": "^5.0.0"
+        "prettier": "^3.0.1",
+        "rimraf": "^5.0.0",
+        "typescript": "^5.1.3"
     },
     "files": [
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "schema/*.json",
         "style/**/*.{css,eot,gif,html,jpg,json,png,svg,woff2,ttf}"
     ],
     "homepage": "https://github.com/dask/dask-labextension",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.48341a7428463ba2c6bb.js"
+            "load": "static/remoteEntry.55eb452b48896f869659.js"
         },
         "extension": true,
         "outputDir": "dask_labextension/labextension",
         "schemaDir": "schema"
     },
     "keywords": [
         "dask",
         "jupyter",
         "jupyterlab",
         "jupyterlab-extension"
     ],
     "license": "BSD-3-Clause",
     "main": "lib/index.js",
     "name": "dask-labextension",
-    "private": false,
     "repository": {
         "type": "git",
         "url": "https://github.com/dask/dask-labextension"
     },
-    "resolutions": {
-        "@types/react": "~17.0.0"
-    },
     "scripts": {
         "build": "jlpm run build:lib && jlpm run build:labextension:dev",
         "build:labextension": "jupyter labextension build .",
         "build:labextension:dev": "jupyter labextension build --development True .",
         "build:lib": "tsc",
         "build:prod": "jlpm run build:lib && jlpm run build:labextension",
         "clean": "jlpm run clean:lib",
@@ -98,9 +94,9 @@
         "prettier:check": "prettier --list-different '**/*{.ts,.tsx,.js,.jsx,.css,.json,.md}'",
         "test": "mocha",
         "watch": "run-p watch:src watch:labextension",
         "watch:labextension": "jupyter labextension watch .",
         "watch:src": "tsc -w"
     },
     "types": "lib/index.d.ts",
-    "version": "6.2.0"
+    "version": "7.0.0"
 }
```

### Comparing `dask_labextension-6.2.0/dask_labextension/labextension/schemas/dask-labextension/package.json.orig` & `dask_labextension-7.0.0/package.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8071895424836601%*

 * *Differences: {"'author'": "{replace: OrderedDict([('name', 'Ian Rose, Matt Rocklin, Jacob Tomlinson')])}",*

 * * "'dependencies'": "{'@jupyterlab/application': '^4.0.0', '@jupyterlab/apputils': '^4.0.0', "*

 * *                   "'@jupyterlab/codeeditor': '^4.0.0', '@jupyterlab/console': '^4.0.0', "*

 * *                   "'@jupyterlab/coreutils': '^6.0.0', '@jupyterlab/docregistry': '^4.0.0', "*

 * *                   "'@jupyterlab/mainmenu': '^4.0.0', '@jupyterlab/nbformat': '^4.0.0', "*

 * *                   "'@jupyterlab/notebook': '^4.0 […]*

```diff
@@ -1,56 +1,56 @@
 {
-    "author": "Ian Rose, Matt Rocklin, Jacob Tomlinson",
+    "author": {
+        "name": "Ian Rose, Matt Rocklin, Jacob Tomlinson"
+    },
     "bugs": {
         "url": "https://github.com/dask/dask-labextension/issues"
     },
     "dependencies": {
-        "@jupyterlab/application": "^3.0.0",
-        "@jupyterlab/apputils": "^3.0.0",
-        "@jupyterlab/codeeditor": "^3.0.0",
-        "@jupyterlab/console": "^3.0.0",
-        "@jupyterlab/coreutils": "^5.0.0",
-        "@jupyterlab/docregistry": "^3.4.3",
-        "@jupyterlab/mainmenu": "^3.0.0",
-        "@jupyterlab/nbformat": "^3.0.0",
-        "@jupyterlab/notebook": "^3.0.0",
-        "@jupyterlab/services": "^6.0.0",
-        "@jupyterlab/settingregistry": "^3.0.0",
-        "@jupyterlab/statedb": "^3.0.0",
-        "@jupyterlab/ui-components": "^3.0.0",
-        "@lumino/algorithm": "^1.3.3",
-        "@lumino/coreutils": "^1.5.3",
-        "@lumino/domutils": "^1.2.3",
-        "@lumino/dragdrop": "^1.7.1",
-        "@lumino/messaging": "^1.4.3",
-        "@lumino/polling": "^1.0.4",
-        "@lumino/signaling": "^1.4.3",
-        "@lumino/widgets": "^1.17.0",
-        "react": "^17.0.1",
-        "react-dom": "^17.0.1"
+        "@jupyterlab/application": "^4.0.0",
+        "@jupyterlab/apputils": "^4.0.0",
+        "@jupyterlab/codeeditor": "^4.0.0",
+        "@jupyterlab/console": "^4.0.0",
+        "@jupyterlab/coreutils": "^6.0.0",
+        "@jupyterlab/docregistry": "^4.0.0",
+        "@jupyterlab/mainmenu": "^4.0.0",
+        "@jupyterlab/nbformat": "^4.0.0",
+        "@jupyterlab/notebook": "^4.0.0",
+        "@jupyterlab/services": "^7.0.0",
+        "@jupyterlab/settingregistry": "^4.0.0",
+        "@jupyterlab/statedb": "^4.0.0",
+        "@jupyterlab/ui-components": "^4.0.0",
+        "@lumino/algorithm": "^2.0.0",
+        "@lumino/coreutils": "^2.0.0",
+        "@lumino/domutils": "^2.0.0",
+        "@lumino/dragdrop": "^2.0.0",
+        "@lumino/messaging": "^2.0.0",
+        "@lumino/polling": "^2.0.0",
+        "@lumino/signaling": "^2.0.0",
+        "@lumino/widgets": "^2.0.0",
+        "react": "^18.0.0",
+        "react-dom": "^18.0.0"
     },
     "description": "A JupyterLab extension for Dask.",
     "devDependencies": {
-        "@jupyterlab/builder": "^3.0.0",
-        "@types/react": "^17.0.0",
-        "@types/react-dom": "^17.0.0",
-        "@typescript-eslint/eslint-plugin": "^4.18.0",
-        "@typescript-eslint/parser": "^4.18.0",
-        "eslint": "^7.14.0",
-        "eslint-config-prettier": "^6.10.1",
-        "eslint-plugin-prettier": "^3.1.4",
+        "@jupyterlab/builder": "^4.0.0",
+        "@types/react": "^18.0.0",
+        "@types/react-dom": "^18.0.0",
+        "@typescript-eslint/eslint-plugin": "^5.59.0",
+        "@typescript-eslint/parser": "^5.59.0",
+        "eslint": "^8.4.0",
+        "eslint-config-prettier": "^8.8.0",
+        "eslint-plugin-prettier": "^4.2.1",
         "eslint-plugin-react": "^7.21.5",
         "mkdirp": "^1.0.3",
         "mocha": "^6.2.0",
         "npm-run-all": "^4.1.5",
-        "prettier": "^2.1.1",
-        "rimraf": "^3.0.2",
-        "typescript": "~4.1.3",
-        "yarn": "1.22.0",
-        "yarn-deduplicate": "^5.0.0"
+        "prettier": "^3.0.1",
+        "rimraf": "^5.0.0",
+        "typescript": "^5.1.3"
     },
     "files": [
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "schema/*.json",
         "style/**/*.{css,eot,gif,html,jpg,json,png,svg,woff2,ttf}"
     ],
     "homepage": "https://github.com/dask/dask-labextension",
@@ -64,22 +64,18 @@
         "jupyter",
         "jupyterlab",
         "jupyterlab-extension"
     ],
     "license": "BSD-3-Clause",
     "main": "lib/index.js",
     "name": "dask-labextension",
-    "private": false,
     "repository": {
         "type": "git",
         "url": "https://github.com/dask/dask-labextension"
     },
-    "resolutions": {
-        "@types/react": "~17.0.0"
-    },
     "scripts": {
         "build": "jlpm run build:lib && jlpm run build:labextension:dev",
         "build:labextension": "jupyter labextension build .",
         "build:labextension:dev": "jupyter labextension build --development True .",
         "build:lib": "tsc",
         "build:prod": "jlpm run build:lib && jlpm run build:labextension",
         "clean": "jlpm run clean:lib",
@@ -94,9 +90,9 @@
         "prettier:check": "prettier --list-different '**/*{.ts,.tsx,.js,.jsx,.css,.json,.md}'",
         "test": "mocha",
         "watch": "run-p watch:src watch:labextension",
         "watch:labextension": "jupyter labextension watch .",
         "watch:src": "tsc -w"
     },
     "types": "lib/index.d.ts",
-    "version": "6.2.0"
+    "version": "7.0.0"
 }
```

### Comparing `dask_labextension-6.2.0/dask_labextension/labextension/schemas/dask-labextension/plugin.json` & `dask_labextension-7.0.0/dask_labextension/labextension/schemas/dask-labextension/plugin.json`

 * *Files identical despite different names*

### Comparing `dask_labextension-6.2.0/dask_labextension/labextension/static/224.86c44b816becca807a99.js` & `dask_labextension-7.0.0/dask_labextension/labextension/static/11.92ba9866db6ad7a7f70f.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,36 +1,36 @@
+"use strict";
 (self.webpackChunkdask_labextension = self.webpackChunkdask_labextension || []).push([
-    [224], {
-        224: (e, t, n) => {
-            "use strict";
+    [11], {
+        11: (e, t, n) => {
             n.r(t), n.d(t, {
-                DaskIcon: () => F,
-                default: () => z
+                DaskIcon: () => K,
+                default: () => J
             });
-            var s, a = n(638),
-                i = n(303),
-                r = n(745),
-                o = n(543),
-                l = n(535),
-                d = n(299),
-                c = n(548),
-                u = n(127),
-                h = n(918),
-                m = n(840),
-                p = n(344),
-                g = n(139),
-                v = n(526),
-                C = n(358),
-                f = n(832),
-                b = n(271),
-                k = n(456);
-            class w extends i.MainAreaWidget {
+            var s, a = n(220),
+                r = n(833),
+                i = n(35),
+                o = n(656),
+                l = n(664),
+                c = n(200),
+                d = n(731),
+                u = n(543),
+                h = n(697),
+                p = n(901),
+                m = n(151),
+                g = n(255),
+                v = n(930),
+                b = n(797),
+                f = n(778),
+                k = n(29),
+                C = n(704);
+            class y extends r.MainAreaWidget {
                 constructor() {
                     super({
-                        content: new i.IFrame({
+                        content: new r.IFrame({
                             sandbox: ["allow-scripts", "allow-same-origin"]
                         })
                     }), this._item = null, this._dashboardUrl = "", this._active = !1, this._inactivePanel = s.createInactivePanel(), this.content.node.appendChild(this._inactivePanel), this.addClass("dask-DaskDashboard-widget"), this.update()
                 }
                 get item() {
                     return this._item
                 }
@@ -47,18 +47,18 @@
                     return this._active
                 }
                 set active(e) {
                     e !== this._active && (this._active = e, this.update())
                 }
                 onUpdateRequest() {
                     if (!this.item || !this.dashboardUrl || !this.active) return this.content.url = "", void(this._inactivePanel.style.display = "");
-                    this._inactivePanel.style.display = "none", this.content.url = p.URLExt.join(this.dashboardUrl, this.item.route)
+                    this._inactivePanel.style.display = "none", this.content.url = m.URLExt.join(this.dashboardUrl, this.item.route)
                 }
             }
-            class y extends f.Widget {
+            class w extends f.Widget {
                 constructor(e) {
                     super();
                     let t = this.layout = new f.PanelLayout;
                     this._dashboard = new f.Widget, this._serverSettings = g.ServerConnection.makeSettings(), this._input = new _(this._serverSettings, e.linkFinder), t.addWidget(this._input), t.addWidget(this._dashboard), this.addClass("dask-DaskDashboardLauncher"), this._items = e.items || [], this._launchItem = e.launchItem, this._input.urlInfoChanged.connect(this._updateLinks, this)
                 }
                 _updateLinks(e, t) {
                     if (!t.newValue.isActive) return void this.update();
@@ -68,36 +68,36 @@
                 get items() {
                     return this._items
                 }
                 get input() {
                     return this._input
                 }
                 onUpdateRequest() {
-                    this.isVisible && k.render(b.createElement(x, {
+                    this.isVisible && C.render(k.createElement(x, {
                         launchItem: this._launchItem,
                         isEnabled: this.input.urlInfo.isActive,
                         items: this._items
                     }), this._dashboard.node)
                 }
                 onAfterShow() {
                     this.update()
                 }
             }
             class _ extends f.Widget {
                 constructor(e, t) {
-                    super(), this._urlChanged = new m.Signal(this), this._urlInfo = {
+                    super(), this._urlChanged = new p.Signal(this), this._urlInfo = {
                         isActive: !1,
                         url: "",
                         plots: {}
                     }, this._browserDashboardCheck = !1, this.addClass("dask-URLInput");
                     const n = this.layout = new f.PanelLayout,
                         s = new f.Widget;
                     if (s.addClass("dask-URLInput-wrapper"), this._input = document.createElement("input"), this._input.placeholder = "DASK DASHBOARD URL", s.node.appendChild(this._input), n.addWidget(s), this._serverSettings = e, t) {
-                        const e = new i.ToolbarButton({
-                            icon: r.searchIcon,
+                        const e = new r.ToolbarButton({
+                            icon: i.searchIcon,
                             onClick: async () => {
                                 let e = await t();
                                 e && (this.url = e)
                             },
                             tooltip: "Auto-detect dashboard URL"
                         });
                         n.addWidget(e)
@@ -138,15 +138,15 @@
                 onAfterAttach() {
                     this._input.addEventListener("keydown", this, !0)
                 }
                 onBeforeDetach() {
                     this._input.removeEventListener("keydown", this, !0)
                 }
                 _startUrlCheckTimer() {
-                    this._poll = new C.Poll({
+                    this._poll = new b.Poll({
                         factory: async () => {
                             const e = this._urlInfo;
                             if (!e.url) return;
                             const t = await s.testDaskDashboard(e.url, this._serverSettings, this._browserDashboardCheck);
                             if (!t.isActive && e.isActive && console.warn(`The connection to dask dashboard ${e.url} has been lost`), v.JSONExt.deepEqual(t, e) || (this._urlInfo = t, this._urlChanged.emit({
                                     oldValue: e,
                                     newValue: t
@@ -159,47 +159,47 @@
                         },
                         standby: "when-hidden"
                     }), this._urlChanged.connect((() => this._poll.refresh()), this)
                 }
             }
 
             function x(e) {
-                if (!e.isEnabled) return b.createElement("div", {
+                if (!e.isEnabled) return k.createElement("div", {
                     className: "dask-DashboardListing-inactive"
-                }, b.createElement("span", {
+                }, k.createElement("span", {
                     className: "dask-DashboardListing-inactive-title"
-                }, "Dashboard not connected"), b.createElement("span", {
+                }, "Dashboard not connected"), k.createElement("span", {
                     className: "dask-DashboardListing-inactive-detail"
                 }, "To connect, paste a dashboard URL in the box above, or create a new Dask cluster with the cluster manager below. If you are still unable to connect, check your network setup."));
-                const t = [...e.items].sort(((e, t) => e.label <= t.label ? -1 : 1)).map((t => b.createElement("li", {
+                const t = [...e.items].sort(((e, t) => e.label <= t.label ? -1 : 1)).map((t => k.createElement("li", {
                     className: "dask-DashboardListing-item",
                     key: t.route
-                }, b.createElement("button", {
+                }, k.createElement("button", {
                     className: "jp-mod-styled jp-mod-accept",
                     value: t.label,
                     disabled: !e.isEnabled,
                     onClick: () => e.launchItem(t)
                 }, t.label))));
-                return b.createElement("div", null, b.createElement("ul", {
+                return k.createElement("div", null, k.createElement("ul", {
                     className: "dask-DashboardListing-list"
                 }, t))
             }! function(e) {
                 function t(e, t = "") {
                     if (n(e)) {
-                        t || (t = p.PageConfig.getBaseUrl());
+                        t || (t = m.PageConfig.getBaseUrl());
                         const n = new URL(t);
                         e.startsWith(n.pathname) && (e = e.slice(n.pathname.length)), e = t + e
                     }
                     return e.endsWith("status") ? e = e.slice(0, -6) : e.endsWith("status/") && (e = e.slice(0, -7)), e
                 }
 
                 function n(e) {
                     const {
                         protocol: t
-                    } = p.URLExt.parse(e);
+                    } = m.URLExt.parse(e);
                     return 0 !== e.toLowerCase().indexOf(t) && 0 !== e.indexOf("//")
                 }
                 e.normalizeDashboardUrl = t, e.getDashboardPlots = function(e) {
                     const t = [];
                     for (let n in e.plots) {
                         const s = n.replace("Individual ", ""),
                             a = {
@@ -207,15 +207,15 @@
                                 label: s,
                                 key: s
                             };
                         t.push(a)
                     }
                     return t
                 }, e.testDaskDashboard = async function(e, n, s = !1) {
-                    if (0 === (e = t(e, n.baseUrl)).indexOf(n.baseUrl)) return g.ServerConnection.makeRequest(p.URLExt.join(e, "individual-plots.json"), {}, n).then((async t => {
+                    if (0 === (e = t(e, n.baseUrl)).indexOf(n.baseUrl)) return g.ServerConnection.makeRequest(m.URLExt.join(e, "individual-plots.json"), {}, n).then((async t => {
                         if (200 === t.status) {
                             const n = await t.json();
                             return {
                                 url: e,
                                 isActive: !0,
                                 plots: n
                             }
@@ -226,15 +226,15 @@
                             plots: {}
                         }
                     })).catch((() => ({
                         url: e,
                         isActive: !1,
                         plots: {}
                     })));
-                    if (s) return fetch(p.URLExt.join(e, "individual-plots.json")).then((async t => {
+                    if (s) return fetch(m.URLExt.join(e, "individual-plots.json")).then((async t => {
                         if (200 === t.status) {
                             const n = await t.json();
                             return {
                                 url: e,
                                 isActive: !0,
                                 plots: n
                             }
@@ -245,24 +245,24 @@
                             plots: {}
                         }
                     })).catch((() => ({
                         url: e,
                         isActive: !1,
                         plots: {}
                     })));
-                    const a = await g.ServerConnection.makeRequest(p.URLExt.join(n.baseUrl, "dask", "dashboard-check", encodeURIComponent(e)), {}, n);
+                    const a = await g.ServerConnection.makeRequest(m.URLExt.join(n.baseUrl, "dask", "dashboard-check", encodeURIComponent(e)), {}, n);
                     return await a.json()
                 }, e.createInactivePanel = function() {
                     const e = document.createElement("div");
                     return e.className = "dask-DaskDashboard-inactive", e
                 }, e.isLocal = n
             }(s || (s = {}));
-            var L, I = n(520),
-                E = n(694);
-            class D extends b.Component {
+            var L, I = n(593),
+                S = n(359);
+            class E extends k.Component {
                 constructor(e) {
                     let t;
                     super(e);
                     const n = !!e.initialModel.adapt;
                     t = n ? e.initialModel : {
                         ...e.initialModel,
                         adapt: {
@@ -324,99 +324,99 @@
                     })
                 }
                 render() {
                     const e = this.state.model,
                         t = e.adapt,
                         n = this.state.adaptive,
                         s = "dask-mod-disabled";
-                    return b.createElement("div", null, b.createElement("span", {
+                    return k.createElement("div", null, k.createElement("span", {
                         className: "dask-ScalingHeader"
-                    }, "Manual Scaling"), b.createElement("div", {
+                    }, "Manual Scaling"), k.createElement("div", {
                         className: "dask-ScalingSection"
-                    }, b.createElement("div", {
+                    }, k.createElement("div", {
                         className: "dask-ScalingSection-item"
-                    }, b.createElement("span", {
+                    }, k.createElement("span", {
                         className: `dask-ScalingSection-label ${n?s:""}`
-                    }, "Workers"), b.createElement("input", {
+                    }, "Workers"), k.createElement("input", {
                         className: "dask-ScalingInput",
                         disabled: n,
                         value: e.workers,
                         type: "number",
                         step: "1",
                         onChange: e => {
                             this.onScaleChanged(e)
                         }
-                    }))), b.createElement("div", {
+                    }))), k.createElement("div", {
                         className: "dask-ScalingHeader"
-                    }, "Adaptive Scaling", b.createElement("input", {
+                    }, "Adaptive Scaling", k.createElement("input", {
                         className: "dask-ScalingCheckbox",
                         type: "checkbox",
                         checked: n,
                         onChange: e => {
                             this.onScalingChanged(e)
                         }
-                    })), b.createElement("div", {
+                    })), k.createElement("div", {
                         className: "dask-ScalingSection"
-                    }, b.createElement("div", {
+                    }, k.createElement("div", {
                         className: "dask-ScalingSection-item"
-                    }, b.createElement("span", {
+                    }, k.createElement("span", {
                         className: `dask-ScalingSection-label ${n?"":s}`
-                    }, "Minimum workers"), b.createElement("input", {
+                    }, "Minimum workers"), k.createElement("input", {
                         className: "dask-ScalingInput",
                         disabled: !n,
                         type: "number",
                         value: t.minimum,
                         step: "1",
                         onChange: e => {
                             this.onMinimumChanged(e)
                         }
-                    }))), b.createElement("div", {
+                    }))), k.createElement("div", {
                         className: "dask-ScalingSection"
-                    }, b.createElement("div", {
+                    }, k.createElement("div", {
                         className: "dask-ScalingSection-item"
-                    }, b.createElement("span", {
+                    }, k.createElement("span", {
                         className: `dask-ScalingSection-label ${n?"":s}`
-                    }, "Maximum workers"), b.createElement("input", {
+                    }, "Maximum workers"), k.createElement("input", {
                         className: "dask-ScalingInput",
                         disabled: !n,
                         type: "number",
                         value: t.maximum,
                         step: "1",
                         onChange: e => {
                             this.onMaximumChanged(e)
                         }
                     }))))
                 }
             }
-            class S extends f.Widget {
+            class D extends f.Widget {
                 constructor(e) {
-                    super(), this._dragData = null, this._clusters = [], this._activeClusterChanged = new m.Signal(this), this._failedServerChecks = 0, this._hasServer = !1, this._isReady = !0, this.addClass("dask-DaskClusterManager"), this._serverSettings = g.ServerConnection.makeSettings(), this._injectClientCodeForCluster = e.injectClientCodeForCluster, this._getClientCodeForCluster = e.getClientCodeForCluster, this._registry = e.registry, this._launchClusterId = e.launchClusterId, this._setActiveById = t => {
+                    super(), this._dragData = null, this._clusters = [], this._activeClusterChanged = new p.Signal(this), this._failedServerChecks = 0, this._hasServer = !1, this._isReady = !0, this.addClass("dask-DaskClusterManager"), this._serverSettings = g.ServerConnection.makeSettings(), this._injectClientCodeForCluster = e.injectClientCodeForCluster, this._getClientCodeForCluster = e.getClientCodeForCluster, this._registry = e.registry, this._launchClusterId = e.launchClusterId, this._setActiveById = t => {
                         const n = this._clusters.find((e => e.id === t));
                         if (!n) return;
-                        const s = p.URLExt.join(this._serverSettings.baseUrl, "proxy"),
+                        const s = m.URLExt.join(this._serverSettings.baseUrl, "proxy"),
                             a = new URL(s).pathname; - 1 !== n.dashboard_link.indexOf(a) ? e.setDashboardUrl(n.dashboard_link) : e.setDashboardUrl(`dask/dashboard/${n.id}`);
-                        const i = this._activeCluster;
-                        i && i.id === n.id || (this._activeCluster = n, this._activeClusterChanged.emit({
+                        const r = this._activeCluster;
+                        r && r.id === n.id || (this._activeCluster = n, this._activeClusterChanged.emit({
                             name: "cluster",
-                            oldValue: i,
+                            oldValue: r,
                             newValue: n
                         }), this.update())
                     };
                     const t = this.layout = new f.PanelLayout;
                     this._clusterListing = new f.Widget, this._clusterListing.addClass("dask-ClusterListing");
-                    const n = new i.Toolbar,
+                    const n = new r.Toolbar,
                         s = new f.Widget;
-                    s.node.textContent = "CLUSTERS", s.addClass("dask-DaskClusterManager-label"), n.addItem("label", s), n.addItem("refresh", new i.ToolbarButton({
-                        icon: r.refreshIcon,
+                    s.node.textContent = "CLUSTERS", s.addClass("dask-DaskClusterManager-label"), n.addItem("label", s), n.addItem("refresh", new r.ToolbarButton({
+                        icon: i.refreshIcon,
                         onClick: async () => this._updateClusterList(),
                         tooltip: "Refresh Cluster List"
-                    })), n.addItem(this._launchClusterId, new i.CommandToolbarButton({
+                    })), n.addItem(this._launchClusterId, new r.CommandToolbarButton({
                         commands: this._registry,
                         id: this._launchClusterId
-                    })), t.addWidget(n), t.addWidget(this._clusterListing), this._updateClusterList(), this._poll = new C.Poll({
+                    })), t.addWidget(n), t.addWidget(this._clusterListing), this._updateClusterList(), this._poll = new b.Poll({
                         factory: async () => {
                             await this._updateClusterList()
                         },
                         frequency: {
                             interval: 5e3,
                             backoff: !0,
                             max: 6e4
@@ -453,15 +453,15 @@
                     if (!this._clusters.find((t => t.id === e))) throw Error(`Cannot find cluster ${e}`);
                     return await this._scaleById(e)
                 }
                 dispose() {
                     this.isDisposed || (this._poll.dispose(), super.dispose())
                 }
                 onUpdateRequest(e) {
-                    this.isVisible && k.render(b.createElement(j, {
+                    this.isVisible && C.render(k.createElement(j, {
                         clusters: this._clusters,
                         activeClusterId: this._activeCluster && this._activeCluster.id || "",
                         scaleById: e => this._scaleById(e),
                         stopById: e => this._stopById(e),
                         setActiveById: this._setActiveById,
                         injectClientCodeForCluster: this._injectClientCodeForCluster
                     }), this._clusterListing.node)
@@ -512,27 +512,27 @@
                     let n = Math.abs(e.clientX - t.pressX),
                         s = Math.abs(e.clientY - t.pressY);
                     (n >= 5 || s >= 5) && (e.preventDefault(), e.stopPropagation(), this._startDrag(t.index, e.clientX, e.clientY))
                 }
                 async _startDrag(e, t, n) {
                     const s = this._clusters[e],
                         a = this._clusterListing.node.querySelector(`li.dask-ClusterListingItem[data-cluster-id="${s.id}"]`),
-                        i = L.createDragImage(a);
-                    this._drag = new E.Drag({
+                        r = L.createDragImage(a);
+                    this._drag = new S.Drag({
                         mimeData: new v.MimeData,
-                        dragImage: i,
+                        dragImage: r,
                         supportedActions: "copy",
                         proposedAction: "copy",
                         source: this
                     });
-                    const r = this._getClientCodeForCluster(s);
-                    this._drag.mimeData.setData("text/plain", r);
+                    const i = this._getClientCodeForCluster(s);
+                    this._drag.mimeData.setData("text/plain", i);
                     const o = [{
                         cell_type: "code",
-                        source: r,
+                        source: i,
                         outputs: [],
                         execution_count: null,
                         metadata: {}
                     }];
                     return this._drag.mimeData.setData("application/vnd.jupyter.cells", o), document.removeEventListener("mousemove", this, !0), document.removeEventListener("mouseup", this, !0), this._drag.start(t, n).then((e => {
                         this.isDisposed || (this._drag = null, this._dragData = null)
                     }))
@@ -540,25 +540,25 @@
                 async _launchCluster() {
                     this._isReady = !1, this._registry.notifyCommandChanged(this._launchClusterId);
                     const e = await g.ServerConnection.makeRequest(`${this._serverSettings.baseUrl}dask/clusters`, {
                         method: "PUT"
                     }, this._serverSettings);
                     if (200 !== e.status) {
                         const t = await e.json();
-                        throw (0, i.showErrorMessage)("Cluster Start Error", t), this._isReady = !0, this._registry.notifyCommandChanged(this._launchClusterId), t
+                        throw (0, r.showErrorMessage)("Cluster Start Error", t), this._isReady = !0, this._registry.notifyCommandChanged(this._launchClusterId), t
                     }
                     const t = await e.json();
                     return await this._updateClusterList(), this._isReady = !0, this._registry.notifyCommandChanged(this._launchClusterId), t
                 }
                 async _updateClusterList() {
                     const e = await g.ServerConnection.makeRequest(`${this._serverSettings.baseUrl}dask/clusters`, {}, this._serverSettings);
                     if (200 !== e.status) {
                         this._failedServerChecks++;
                         const e = new Error("Failed to list Dask clusters: might the server extension not be installed/enabled?");
-                        throw this._hasServer || 5 != this._failedServerChecks || (0, i.showErrorMessage)("Dask Server Error", e), e
+                        throw this._hasServer || 5 != this._failedServerChecks || (0, r.showErrorMessage)("Dask Server Error", e), e
                     }
                     this._hasServer = !0;
                     const t = await e.json();
                     if (this._clusters = t, !this._clusters.find((e => e.id === (this._activeCluster && this._activeCluster.id)))) {
                         const e = this._clusters[0] && this._clusters[0].id || "";
                         this._setActiveById(e)
                     }
@@ -566,147 +566,147 @@
                 }
                 async _stopById(e) {
                     const t = await g.ServerConnection.makeRequest(`${this._serverSettings.baseUrl}dask/clusters/${e}`, {
                         method: "DELETE"
                     }, this._serverSettings);
                     if (204 !== t.status) {
                         const e = await t.json();
-                        throw (0, i.showErrorMessage)("Failed to close cluster", e), e
+                        throw (0, r.showErrorMessage)("Failed to close cluster", e), e
                     }
                     await this._updateClusterList()
                 }
                 async _scaleById(e) {
                     const t = this._clusters.find((t => t.id === e));
                     if (!t) throw Error(`Failed to find cluster ${e} to scale`);
                     const n = await
                     function(e) {
                         let t = {
                             ...e
                         };
-                        return (0, i.showDialog)({
+                        return (0, r.showDialog)({
                             title: `Scale ${e.name}`,
-                            body: b.createElement(D, {
+                            body: k.createElement(E, {
                                 initialModel: e,
                                 stateEscapeHatch: e => {
                                     t = e
                                 }
                             }),
-                            buttons: [i.Dialog.cancelButton(), i.Dialog.okButton({
+                            buttons: [r.Dialog.cancelButton(), r.Dialog.okButton({
                                 label: "SCALE"
                             })]
                         }).then((n => n.button.accept ? t : e))
                     }(t);
                     if (v.JSONExt.deepEqual(n, t)) return Promise.resolve(t);
                     const s = await g.ServerConnection.makeRequest(`${this._serverSettings.baseUrl}dask/clusters/${e}`, {
                         method: "PATCH",
                         body: JSON.stringify(n)
                     }, this._serverSettings);
                     if (200 !== s.status) {
                         const e = await s.json();
-                        throw (0, i.showErrorMessage)("Failed to scale cluster", e), e
+                        throw (0, r.showErrorMessage)("Failed to scale cluster", e), e
                     }
                     const a = await s.json();
                     return await this._updateClusterList(), a
                 }
                 _findCluster(e) {
                     const t = Array.from(this.node.querySelectorAll("li.dask-ClusterListingItem"));
                     return h.ArrayExt.findFirstIndex(t, (t => I.ElementExt.hitTest(t, e.clientX, e.clientY)))
                 }
             }
 
             function j(e) {
-                let t = e.clusters.map((t => b.createElement(M, {
+                let t = e.clusters.map((t => k.createElement(M, {
                     isActive: t.id === e.activeClusterId,
                     key: t.id,
                     cluster: t,
                     scale: () => e.scaleById(t.id),
                     stop: () => e.stopById(t.id),
                     setActive: () => e.setActiveById(t.id),
                     injectClientCode: () => e.injectClientCodeForCluster(t)
                 })));
-                return b.createElement("div", null, b.createElement("ul", {
+                return k.createElement("div", null, k.createElement("ul", {
                     className: "dask-ClusterListing-list"
                 }, t))
             }
 
             function M(e) {
                 const {
                     cluster: t,
                     isActive: n,
                     setActive: s,
                     scale: a,
-                    stop: i,
-                    injectClientCode: r
+                    stop: r,
+                    injectClientCode: i
                 } = e;
                 let o = "dask-ClusterListingItem";
                 o = n ? `${o} jp-mod-active` : o;
                 let l = null,
-                    d = null;
-                return t.adapt && (l = b.createElement("div", {
+                    c = null;
+                return t.adapt && (l = k.createElement("div", {
                     className: "dask-ClusterListingItem-stats"
-                }, "Minimum Workers: ", t.adapt.minimum), d = b.createElement("div", {
+                }, "Minimum Workers: ", t.adapt.minimum), c = k.createElement("div", {
                     className: "dask-ClusterListingItem-stats"
-                }, "Maximum Workers: ", t.adapt.maximum)), b.createElement("li", {
+                }, "Maximum Workers: ", t.adapt.maximum)), k.createElement("li", {
                     className: o,
                     "data-cluster-id": t.id,
                     onClick: e => {
                         s(), e.stopPropagation()
                     }
-                }, b.createElement("div", {
+                }, k.createElement("div", {
                     className: "dask-ClusterListingItem-title"
-                }, t.name), b.createElement("div", {
+                }, t.name), k.createElement("div", {
                     className: "dask-ClusterListingItem-link",
                     title: t.scheduler_address
-                }, "Scheduler Address: ", t.scheduler_address), b.createElement("div", {
+                }, "Scheduler Address: ", t.scheduler_address), k.createElement("div", {
                     className: "dask-ClusterListingItem-link"
-                }, "Dashboard URL:", " ", b.createElement("a", {
+                }, "Dashboard URL:", " ", k.createElement("a", {
                     target: "_blank",
                     rel: "noreferrer",
                     href: t.dashboard_link,
                     title: t.dashboard_link
-                }, t.dashboard_link)), b.createElement("div", {
+                }, t.dashboard_link)), k.createElement("div", {
                     className: "dask-ClusterListingItem-stats"
-                }, "Number of Cores: ", t.cores), b.createElement("div", {
+                }, "Number of Cores: ", t.cores), k.createElement("div", {
                     className: "dask-ClusterListingItem-stats"
-                }, "Memory: ", t.memory), b.createElement("div", {
+                }, "Memory: ", t.memory), k.createElement("div", {
                     className: "dask-ClusterListingItem-stats"
-                }, "Number of Workers: ", t.workers), l, d, b.createElement("div", {
+                }, "Number of Workers: ", t.workers), l, c, k.createElement("div", {
                     className: "dask-ClusterListingItem-button-panel"
-                }, b.createElement("button", {
+                }, k.createElement("button", {
                     className: "dask-ClusterListingItem-button dask-ClusterListingItem-code dask-CodeIcon jp-mod-styled",
                     onClick: e => {
-                        r(), e.stopPropagation()
+                        i(), e.stopPropagation()
                     },
                     title: `Inject client code for ${t.name}`
-                }), b.createElement("button", {
+                }), k.createElement("button", {
                     className: "dask-ClusterListingItem-button dask-ClusterListingItem-scale jp-mod-styled",
                     onClick: async e => (e.stopPropagation(), a()),
                     title: `Rescale ${t.name}`
-                }, "SCALE"), b.createElement("button", {
+                }, "SCALE"), k.createElement("button", {
                     className: "dask-ClusterListingItem-button dask-ClusterListingItem-stop jp-mod-styled",
-                    onClick: async e => (e.stopPropagation(), i()),
+                    onClick: async e => (e.stopPropagation(), r()),
                     title: `Shutdown ${t.name}`
                 }, "SHUTDOWN")))
             }! function(e) {
                 e.createDragImage = function(e) {
                     const t = e.cloneNode(!0);
                     return t.classList.add("dask-ClusterListingItem-drag"), t
                 }
             }(L || (L = {}));
             class U extends f.Widget {
                 constructor(e) {
                     super(), this.addClass("dask-DaskSidebar");
                     let t = this.layout = new f.PanelLayout;
-                    this._dashboard = new y({
+                    this._dashboard = new w({
                         launchItem: e.launchDashboardItem,
                         linkFinder: e.linkFinder
                     });
                     const n = e.clientCodeInjector,
                         s = e.clientCodeGetter;
-                    this._clusters = new S({
+                    this._clusters = new D({
                         registry: e.registry,
                         launchClusterId: e.launchClusterId,
                         setDashboardUrl: e => {
                             this._dashboard.input.url = e
                         },
                         injectClientCodeForCluster: n,
                         getClientCodeForCluster: s
@@ -716,260 +716,271 @@
                     return this._dashboard
                 }
                 get clusterManager() {
                     return this._clusters
                 }
             }
             var A = n(379),
-                N = n.n(A),
-                R = n(760);
-            N()(R.Z, {
-                insert: "head",
-                singleton: !1
-            }), R.Z.locals;
-            const F = new r.LabIcon({
+                R = n.n(A),
+                N = n(795),
+                P = n.n(N),
+                F = n(569),
+                $ = n.n(F),
+                W = n(565),
+                B = n.n(W),
+                z = n(216),
+                T = n.n(z),
+                q = n(589),
+                V = n.n(q),
+                H = n(760),
+                O = {};
+            O.styleTagTransform = V(), O.setAttributes = B(), O.insert = $().bind(null, "head"), O.domAPI = P(), O.insertStyleElement = T(), R()(H.Z, O), H.Z && H.Z.locals && H.Z.locals;
+            const K = new i.LabIcon({
                 name: "dask:icon",
                 svgstr: '<?xml version="1.0" encoding="utf-8"?>\n\x3c!-- Generator: Adobe Illustrator 26.0.3, SVG Export Plug-In . SVG Version: 6.00 Build 0)  --\x3e\n<svg version="1.1" id="Layer_1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" x="0px" y="0px"\n\t viewBox="0 0 512 512" style="enable-background:new 0 0 512 512;" xml:space="preserve">\n<style type="text/css">\n\t.st0{fill:#FFC11E;}\n\t.st1{fill:#04255C;}\n\t.st2{fill:#FC6E6B;}\n\t.st3{fill:#FFFFFF;}\n\t.st4{fill:#EF1161;}\n</style>\n<g>\n\t<path class="st0" d="M143.71,157.61l126.5-72.99c1.25-0.72,2.02-2.05,2.02-3.5l0.01-43.77c0-6.48-2.66-12.9-7.83-16.81\n\t\tc-6.69-5.06-15.28-5.56-22.33-1.48L65.13,121.17c-6.22,3.59-10.06,10.23-10.06,17.41L55,369.18c0,6.47,2.65,12.89,7.81,16.81\n\t\tc6.68,5.07,15.29,5.57,22.35,1.49l37.48-21.62c1.25-0.72,2.02-2.05,2.02-3.5l0.05-171.85C124.71,176.93,131.95,164.4,143.71,157.61\n\t\tz"/>\n\t<path class="st4" d="M446.95,124.53c-3.15-1.82-6.61-2.73-10.06-2.73c-3.45,0-6.9,0.91-10.05,2.73l-176.96,102.1\n\t\tc-6.2,3.58-10.06,10.25-10.06,17.41l-0.07,231.47c0,7.27,3.76,13.78,10.05,17.42c6.3,3.64,13.81,3.64,20.11,0l176.95-102.11\n\t\tc6.2-3.58,10.06-10.25,10.06-17.41L457,141.95C457,134.68,453.24,128.16,446.95,124.53z"/>\n\t<path class="st2" d="M240.95,211.14l116.78-67.38c1.25-0.72,2.02-2.05,2.02-3.5l0.02-50.98c0-6.48-2.66-12.9-7.83-16.81\n\t\tc-6.69-5.06-15.27-5.55-22.33-1.48l-48.43,27.95L152.64,173.1c-6.22,3.59-10.06,10.23-10.06,17.41l-0.05,174.18l-0.02,56.41\n\t\tc0,6.48,2.65,12.89,7.81,16.81c6.69,5.07,15.29,5.57,22.35,1.49l47.2-27.24c1.25-0.72,2.02-2.05,2.02-3.5l0.05-164.64\n\t\tC221.95,230.46,229.19,217.92,240.95,211.14z"/>\n</g>\n</svg>\n'
             });
-            var B;
+            var G;
             ! function(e) {
                 e.launchPanel = "dask:launch-dashboard", e.launchLayout = "dask:launch-layout", e.populateDashboardUrl = "dask:populate-dashboard-url", e.populateAndLaunchLayout = "dask:populate-and-launch-layout", e.injectClientCode = "dask:inject-client-code", e.launchCluster = "dask:launch-cluster", e.stopCluster = "dask:stop-cluster", e.scaleCluster = "dask:scale-cluster", e.toggleAutoStartClient = "dask:toggle-auto-start-client"
-            }(B || (B = {}));
-            const P = "dask-labextension:plugin",
-                W = {
-                    activate: async function(e, t, n, s, a, r, o, l, d) {
-                        const c = "dask-dashboard-launcher",
+            }(G || (G = {}));
+            const X = "dask-labextension:plugin",
+                Y = {
+                    activate: async function(e, t, n, s, a, i, o, l, c) {
+                        const d = "dask-dashboard-launcher",
                             u = async () => {
-                                const e = $.getCurrentKernel(s, o, n);
-                                return await $.shouldUseKernel(e) ? await $.checkKernel(e) : ""
-                            }, p = t => {
-                                const s = $.getCurrentEditor(e, o, n);
-                                s && $.injectClientCode(t, s)
+                                const e = Z.getCurrentKernel(s, o, n);
+                                return await Z.shouldUseKernel(e) ? await Z.checkKernel(e) : ""
+                            }, m = async t => {
+                                const s = await Z.getCurrentEditor(e, o, n);
+                                s && Z.injectClientCode(t, s)
                             }, g = new U({
                                 launchDashboardItem: t => {
-                                    e.commands.execute(B.launchPanel, {
+                                    e.commands.execute(G.launchPanel, {
                                         item: t
                                     })
                                 },
                                 linkFinder: u,
-                                clientCodeInjector: p,
-                                clientCodeGetter: $.getClientCode,
+                                clientCodeInjector: m,
+                                clientCodeGetter: Z.getClientCode,
                                 registry: e.commands,
-                                launchClusterId: B.launchCluster
+                                launchClusterId: G.launchCluster
                             });
-                        g.id = c, g.title.icon = F, g.title.iconClass = "jp-SideBar-tabIcon", g.title.caption = "Dask";
-                        const v = new i.WidgetTracker({
+                        g.id = d, g.title.icon = K, g.title.iconClass = "jp-SideBar-tabIcon", g.title.caption = "Dask";
+                        const v = new r.WidgetTracker({
                             namespace: "dask-dashboard-launcher"
                         });
-                        a.add(g, c), a.restore(v, {
-                            command: B.launchPanel,
+                        a.add(g, d), a.restore(v, {
+                            command: G.launchPanel,
                             args: e => ({
                                 item: e.item
                             } || {}),
                             name: e => e.item && e.item.route || ""
                         }), s.add(g, "left", {
                             rank: 200
                         });
-                        const C = () => {
+                        const b = () => {
                             const e = g.dashboardLauncher.input,
                                 t = g.dashboardLauncher.items;
                             v.forEach((n => {
                                 const s = t.find((e => {
                                     var t;
                                     return (null === (t = n.item) || void 0 === t ? void 0 : t.route) === e.route
                                 }));
                                 if (!s || !e.urlInfo.isActive) return n.active = !1, void(n.dashboardUrl = "");
                                 `${s.label}` !== n.title.label && (n.title.label = `${s.label}`), n.dashboardUrl = e.urlInfo.effectiveUrl || e.urlInfo.url, n.active = !0
                             }))
                         };
                         g.dashboardLauncher.input.urlInfoChanged.connect((async (e, t) => {
-                            C();
+                            b();
                             const n = g.clusterManager.activeCluster;
-                            return d.save(c, {
+                            return c.save(d, {
                                 url: t.newValue.url,
                                 cluster: n ? n.id : ""
                             })
                         })), g.clusterManager.activeClusterChanged.connect((async () => {
                             const e = g.clusterManager.activeCluster;
-                            return d.save(c, {
+                            return c.save(d, {
                                 url: g.dashboardLauncher.input.urlInfo.url,
                                 cluster: e ? e.id : ""
                             })
-                        })), C();
+                        })), b();
                         const f = async e => {
                             if (!e) return;
                             const t = g.clusterManager.activeCluster;
-                            return t && await $.shouldUseKernel(e.kernel) ? $.createClientForKernel(t, e.kernel) : void 0
-                        }, b = [o, n], k = async e => {
+                            return t && await Z.shouldUseKernel(e.kernel) ? Z.createClientForKernel(t, e.kernel) : void 0
+                        }, k = [o, n], C = async e => {
                             if (e.session && e.session.kernel && "restarting" === e.session.kernel.status) return f(e.session)
-                        }, y = (e, t) => {
-                            t.sessionContext.statusChanged.connect(k)
+                        }, w = (e, t) => {
+                            t.sessionContext.statusChanged.connect(C)
                         }, _ = () => {
-                            b.forEach((e => {
+                            k.forEach((e => {
                                 e.forEach((async e => {
                                     const t = e.sessionContext.session;
-                                    if (t && await $.shouldUseKernel(t.kernel)) return f(t)
+                                    if (t && await Z.shouldUseKernel(t.kernel)) return f(t)
                                 }))
                             }))
                         };
                         let x, L = !1,
                             I = !1,
-                            E = !1;
-                        Promise.all([l.load(P), d.fetch(c)]).then((async e => {
+                            S = !1;
+                        Promise.all([l.load(X), c.fetch(d)]).then((async e => {
                             const t = e[0];
                             if (!t) return void console.warn("Unable to retrieve dask-labextension settings");
                             const n = e[1],
                                 s = n ? n.url : "",
                                 a = n ? n.cluster : "",
-                                i = g.dashboardLauncher.input.urlInfo.effectiveUrl || g.dashboardLauncher.input.urlInfo.url;
-                            g.dashboardLauncher.input.url = s && !i ? s : t.get("defaultURL").composite;
-                            const r = () => {
-                                L = t.get("autoStartClient").composite, m.Signal.clearData(y), m.Signal.clearData(k), m.Signal.clearData(_), L && (b.forEach((e => {
-                                    e.widgetAdded.connect(y)
-                                })), b.forEach((e => {
+                                r = g.dashboardLauncher.input.urlInfo.effectiveUrl || g.dashboardLauncher.input.urlInfo.url;
+                            g.dashboardLauncher.input.url = s && !r ? s : t.get("defaultURL").composite;
+                            const i = () => {
+                                L = t.get("autoStartClient").composite, p.Signal.clearData(w), p.Signal.clearData(C), p.Signal.clearData(_), L && (k.forEach((e => {
+                                    e.widgetAdded.connect(w)
+                                })), k.forEach((e => {
                                     e.forEach((async e => {
-                                        await f(e.sessionContext.session), e.sessionContext.statusChanged.connect(k)
+                                        await f(e.sessionContext.session), e.sessionContext.statusChanged.connect(C)
                                     }))
-                                })), g.clusterManager.activeClusterChanged.connect(_)), E = t.get("browserDashboardCheck").composite, g.dashboardLauncher.input.browserDashboardCheck = E, I = t.get("hideClusterManager").composite, g.clusterManager.setHidden(I), x = t.get("defaultLayout").composite
+                                })), g.clusterManager.activeClusterChanged.connect(_)), S = t.get("browserDashboardCheck").composite, g.dashboardLauncher.input.browserDashboardCheck = S, I = t.get("hideClusterManager").composite, g.clusterManager.setHidden(I), x = t.get("defaultLayout").composite
                             };
-                            r(), t.changed.connect(r), a && (await g.clusterManager.refresh(), g.clusterManager.setActiveCluster(a))
-                        })), e.commands.addCommand(B.launchPanel, {
+                            i(), t.changed.connect(i), a && (await g.clusterManager.refresh(), g.clusterManager.setActiveCluster(a))
+                        })), e.commands.addCommand(G.launchPanel, {
                             label: e => `Launch Dask ${e.item.label||""} Dashboard`,
                             caption: "Launch a Dask dashboard",
                             execute: e => {
                                 const t = g.dashboardLauncher.input.urlInfo,
                                     n = t.effectiveUrl || t.url,
                                     a = t.isActive,
-                                    i = e.item,
-                                    r = null == e ? void 0 : e.options,
-                                    o = v.find((e => !(!e || !e.item || e.item.route !== i.route)));
-                                if (o) return o.isAttached || s.add(o, "main", r), void s.activateById(o.id);
-                                const l = new w;
-                                return l.dashboardUrl = n, l.item = i, l.active = a, l.id = "dask-dashboard-" + $.id++, l.title.label = `${i.label}`, l.title.icon = F, s.add(l, "main", r), v.add(l), l
+                                    r = e.item,
+                                    i = null == e ? void 0 : e.options,
+                                    o = v.find((e => !(!e || !e.item || e.item.route !== r.route)));
+                                if (o) return o.isAttached || s.add(o, "main", i), void s.activateById(o.id);
+                                const l = new y;
+                                return l.dashboardUrl = n, l.item = r, l.active = a, l.id = "dask-dashboard-" + Z.id++, l.title.label = `${r.label}`, l.title.icon = K, s.add(l, "main", i), v.add(l), l
                             }
                         });
-                        const D = e => (e.startsWith("/") && (e = e.slice(1)), e.startsWith("individual-") || (e = "individual-" + e), e);
-                        e.commands.addCommand(B.launchLayout, {
+                        const E = e => (e.startsWith("/") && (e = e.slice(1)), e.startsWith("individual-") || (e = "individual-" + e), e);
+                        e.commands.addCommand(G.launchLayout, {
                             label: "Launch Dask Dashboard Layout",
                             caption: "Launch a pre-configured Dask Dashboard Layout",
                             isEnabled: () => g.dashboardLauncher.input.urlInfo.isActive,
                             execute: async () => {
                                 const t = g.dashboardLauncher.items,
                                     n = [];
                                 for (let e of Object.keys(x)) n.push([x[e].ref || null, e]);
                                 const s = (0, h.topologicSort)(n).filter((e => e)),
                                     a = e.shell.currentWidget;
                                 for (let n of s) {
                                     const s = x[n],
-                                        a = t.find((e => D(e.route) === D(n)));
+                                        a = t.find((e => E(e.route) === E(n)));
                                     if (!a) {
                                         console.warn(`Non-existent dashboard found in Dask layout spec ${n}`);
                                         continue
                                     }
-                                    const i = {
+                                    const r = {
                                         mode: s.mode
                                     };
                                     if (s.ref) {
-                                        const e = v.find((e => !(!e || !e.item || D(e.item.route) !== D(s.ref))));
-                                        e ? i.ref = e.id : (console.warn(`Non-existent dashboard found in Dask layout spec ${s.ref}`), i.ref = null)
-                                    } else i.ref = null;
-                                    await e.commands.execute(B.launchPanel, {
+                                        const e = v.find((e => !(!e || !e.item || E(e.item.route) !== E(s.ref))));
+                                        e ? r.ref = e.id : (console.warn(`Non-existent dashboard found in Dask layout spec ${s.ref}`), r.ref = null)
+                                    } else r.ref = null;
+                                    await e.commands.execute(G.launchPanel, {
                                         item: a,
-                                        options: i
+                                        options: r
                                     })
                                 }
                                 e.shell.activateById(a.id)
                             }
-                        }), e.commands.addCommand(B.populateDashboardUrl, {
+                        }), e.commands.addCommand(G.populateDashboardUrl, {
                             label: "Populate Dask Dashboard URL",
                             caption: "Attempt to populate the URL for an active Dask cluster",
                             execute: async e => {
                                 let t = e.url || await u();
                                 return t && (g.dashboardLauncher.input.url = t), t
                             }
-                        }), e.commands.addCommand(B.populateAndLaunchLayout, {
+                        }), e.commands.addCommand(G.populateAndLaunchLayout, {
                             label: "Populate Dask Dashboard URL and launch the default layout",
                             caption: "Attempt to populate the URL for an active Dask cluster and then launch the default layout",
                             execute: async t => {
-                                await e.commands.execute(B.populateDashboardUrl, t) && await e.commands.execute(B.launchLayout)
+                                await e.commands.execute(G.populateDashboardUrl, t) && await e.commands.execute(G.launchLayout)
                             }
-                        }), e.commands.addCommand(B.injectClientCode, {
+                        }), e.commands.addCommand(G.injectClientCode, {
                             label: "Inject Dask Client Connection Code",
-                            execute: () => {
-                                const t = $.clusterFromClick(e, g.clusterManager);
-                                t && p(t)
+                            execute: async () => {
+                                const t = Z.clusterFromClick(e, g.clusterManager);
+                                t && await m(t)
                             }
-                        }), e.commands.addCommand(B.launchCluster, {
+                        }), e.commands.addCommand(G.launchCluster, {
                             label: e => e.isPalette ? "Launch New Cluster" : "NEW",
                             execute: () => g.clusterManager.start(),
                             iconClass: e => e.isPalette ? "" : "jp-AddIcon jp-Icon jp-Icon-16",
                             isEnabled: () => g.clusterManager.isReady,
                             caption: () => g.clusterManager.isReady ? "Start New Dask Cluster" : "Cluster starting..."
-                        }), e.commands.addCommand(B.stopCluster, {
+                        }), e.commands.addCommand(G.stopCluster, {
                             label: "Shutdown Cluster",
                             execute: () => {
-                                const t = $.clusterFromClick(e, g.clusterManager);
+                                const t = Z.clusterFromClick(e, g.clusterManager);
                                 if (t) return g.clusterManager.stop(t.id)
                             }
-                        }), e.commands.addCommand(B.scaleCluster, {
+                        }), e.commands.addCommand(G.scaleCluster, {
                             label: "Scale Cluster…",
                             execute: () => {
-                                const t = $.clusterFromClick(e, g.clusterManager);
+                                const t = Z.clusterFromClick(e, g.clusterManager);
                                 if (t) return g.clusterManager.scale(t.id)
                             }
-                        }), e.commands.addCommand(B.toggleAutoStartClient, {
+                        }), e.commands.addCommand(G.toggleAutoStartClient, {
                             label: "Auto-Start Dask",
                             isToggled: () => L,
                             execute: async () => {
                                 const e = !L,
                                     t = "autoStartClient";
-                                return l.set(P, t, e).catch((e => {
-                                    console.error(`Failed to set ${P}:${t} - ${e.message}`)
+                                return l.set(X, t, e).catch((e => {
+                                    console.error(`Failed to set ${X}:${t} - ${e.message}`)
                                 }))
                             }
-                        }), r.fileMenu.addGroup([{
-                            command: B.launchLayout
-                        }], 50), r.settingsMenu.addGroup([{
-                            command: B.toggleAutoStartClient
-                        }]), [B.launchCluster, B.launchLayout, B.toggleAutoStartClient].forEach((e => {
+                        }), i.fileMenu.addGroup([{
+                            command: G.launchLayout
+                        }], 50), i.settingsMenu.addGroup([{
+                            command: G.toggleAutoStartClient
+                        }]), [G.launchCluster, G.launchLayout, G.toggleAutoStartClient].forEach((e => {
                             t.addItem({
                                 category: "Dask",
                                 command: e,
                                 args: {
                                     isPalette: !0
                                 }
                             })
                         })), e.contextMenu.addItem({
-                            command: B.injectClientCode,
+                            command: G.injectClientCode,
                             selector: ".dask-ClusterListingItem",
                             rank: 10
                         }), e.contextMenu.addItem({
-                            command: B.stopCluster,
+                            command: G.stopCluster,
                             selector: ".dask-ClusterListingItem",
                             rank: 3
                         }), e.contextMenu.addItem({
-                            command: B.scaleCluster,
+                            command: G.scaleCluster,
                             selector: ".dask-ClusterListingItem",
                             rank: 2
                         }), e.contextMenu.addItem({
-                            command: B.launchCluster,
+                            command: G.launchCluster,
                             selector: ".dask-ClusterListing-list",
                             rank: 1
                         })
                     },
-                    id: P,
-                    requires: [i.ICommandPalette, o.IConsoleTracker, a.ILabShell, a.ILayoutRestorer, l.IMainMenu, u.INotebookTracker, d.ISettingRegistry, c.IStateDB],
+                    id: X,
+                    requires: [r.ICommandPalette, o.IConsoleTracker, a.ILabShell, a.ILayoutRestorer, l.IMainMenu, u.INotebookTracker, c.ISettingRegistry, d.IStateDB],
                     autoStart: !0
                 },
-                z = W;
-            var $;
+                J = Y;
+            var Z;
             ! function(e) {
                 function t(e) {
                     return `from dask.distributed import Client\n\nclient = Client("${e.scheduler_address}")\nclient`
                 }
+                async function n(e) {
+                    return await e.ready, e && e.editor
+                }
                 e.id = 0, e.shouldUseKernel = async function(e) {
                     if (!e) return !1;
                     const t = await e.spec;
                     return !!t && -1 !== t.language.toLowerCase().indexOf("python")
                 }, e.checkKernel = function(e) {
                     const t = {
                         store_history: !1,
@@ -989,238 +1000,230 @@
                     };
                     return new Promise(((e, s) => {
                         t.requestExecute(n).onIOPub = t => {
                             "display_data" === t.header.msg_type && e(void 0)
                         }
                     }))
                 }, e.injectClientCode = function(e, n) {
-                    const s = n.getCursorPosition(),
-                        a = n.getOffsetAt(s),
-                        i = t(e);
-                    n.model.value.insert(a, i)
+                    const s = t(e);
+                    n.model.sharedModel.setSource(s)
                 }, e.getClientCode = t, e.getCurrentKernel = function(e, t, n) {
-                    var s, a, i, r;
+                    var s, a, r, i;
                     let o, l = e.currentWidget;
-                    return l && t.has(l) ? o = null === (s = l.sessionContext.session) || void 0 === s ? void 0 : s.kernel : l && n.has(l) ? o = null === (a = l.sessionContext.session) || void 0 === a ? void 0 : a.kernel : t.currentWidget ? o = null === (i = t.currentWidget.sessionContext.session) || void 0 === i ? void 0 : i.kernel : n.currentWidget && (o = null === (r = n.currentWidget.sessionContext.session) || void 0 === r ? void 0 : r.kernel), o
-                }, e.getCurrentEditor = function(e, t, n) {
-                    let s, a = e.shell.currentWidget;
-                    if (a && t.has(a)) {
-                        u.NotebookActions.insertAbove(a.content);
-                        const e = a.content.activeCell;
-                        s = e && e.editor
-                    } else if (a && n.has(a)) {
-                        const e = a.console.promptCell;
-                        s = e && e.editor
-                    } else if (t.currentWidget) {
+                    return l && t.has(l) ? o = null === (s = l.sessionContext.session) || void 0 === s ? void 0 : s.kernel : l && n.has(l) ? o = null === (a = l.sessionContext.session) || void 0 === a ? void 0 : a.kernel : t.currentWidget ? o = null === (r = t.currentWidget.sessionContext.session) || void 0 === r ? void 0 : r.kernel : n.currentWidget && (o = null === (i = n.currentWidget.sessionContext.session) || void 0 === i ? void 0 : i.kernel), o
+                }, e.getEditor = n, e.getCurrentEditor = async function(e, t, s) {
+                    let a = e.shell.currentWidget;
+                    if (a && t.has(a)) return u.NotebookActions.insertAbove(a.content), n(a.content.activeCell);
+                    if (a && s.has(a)) return n(a.console.promptCell);
+                    if (t.currentWidget) {
                         const e = t.currentWidget;
-                        u.NotebookActions.insertAbove(e.content);
-                        const n = e.content.activeCell;
-                        s = n && n.editor
-                    } else if (n.currentWidget) {
-                        const e = n.currentWidget.console.promptCell;
-                        s = e && e.editor
+                        return u.NotebookActions.insertAbove(e.content), n(e.content.activeCell)
                     }
-                    return s
+                    return s.currentWidget ? n(s.currentWidget.console.promptCell) : void 0
                 }, e.clusterFromClick = function(e, t) {
                     const n = e.contextMenuHitTest((e => !!e.dataset.clusterId));
                     if (!n) return;
                     const s = n.dataset.clusterId;
                     return t.clusters.find((e => e.id === s))
                 }
-            }($ || ($ = {}))
+            }(Z || (Z = {}))
         },
         760: (e, t, n) => {
-            "use strict";
             n.d(t, {
-                Z: () => C
+                Z: () => v
             });
-            var s = n(645),
+            var s = n(81),
                 a = n.n(s),
-                i = n(667),
-                r = n.n(i),
-                o = n(637),
+                r = n(645),
+                i = n.n(r),
+                o = n(667),
                 l = n.n(o),
-                d = n(490),
-                c = n.n(d),
-                u = n(935),
-                h = n.n(u),
-                m = a()((function(e) {
-                    return e[1]
-                })),
-                p = r()(l()),
-                g = r()(c()),
-                v = r()(h());
-            m.push([e.id, ":root {\n  --dask-launch-button-height: 24px;\n}\n\n/**\n * Rules related to the overall sidebar panel.\n */\n\n.dask-DaskSidebar {\n  background: var(--jp-layout-color1);\n  color: var(--jp-ui-font-color1);\n  font-size: var(--jp-ui-font-size1);\n  overflow: auto;\n}\n\n/**\n * Rules related to the dashboard launcher.\n */\n\n.dask-DashboardListing-inactive {\n  display: flex;\n  flex-direction: column;\n  justify-content: center;\n  align-items: center;\n  margin: 0;\n  padding: 0;\n  width: 100%;\n  height: 600px;\n  color: var(--jp-ui-font-color3);\n}\n\n.dask-DashboardListing-inactive-title {\n  font-size: var(--jp-ui-font-size3);\n  padding: 24px;\n  text-align: center;\n}\n\n.dask-DashboardListing-inactive-detail {\n  font-size: var(--jp-ui-font-size4);\n  padding: 24px;\n}\n\n.dask-DashboardListing-inactive:before {\n  content: '';\n  position: absolute;\n  top: 0;\n  left: 0;\n  width: 80%;\n  height: 80%;\n  background-image: url(" + p + ");\n  background-repeat: no-repeat;\n  background-position: center;\n  opacity: 0.1;\n}\n\n.dask-DashboardListing-list {\n  margin: 8px;\n  padding: 0;\n  list-style-type: none;\n}\n\n.dask-DashboardListing-item {\n  margin-top: 4px;\n  margin-bottom: 4px;\n  margin-left: 12px;\n  margin-right: 12px;\n  white-space: nowrap;\n}\n\n.dask-DashboardListing-item button {\n  font-size: var(--jp-ui-font-size0);\n  border-radius: 2px;\n  line-height: 1em;\n  padding: 0px 8px;\n  width: 100%;\n}\n\n.dask-DashboardListing-item button.jp-mod-styled.jp-mod-accept {\n  height: var(--dask-launch-button-height);\n  color: #262326;\n  background-color: #ffc11e;\n  border: 1px solid #ffc11e;\n  text-transform: uppercase;\n}\n\n.dask-URLInput {\n  padding: 8px;\n  display: flex;\n  align-items: center;\n  background-color: var(--jp-layout-color1);\n  border-bottom: 1px solid var(--jp-border-color2);\n  box-shadow: var(--jp-toolbar-box-shadow);\n  z-index: 2;\n}\n\n.dask-URLInput-wrapper {\n  background-color: var(--jp-input-active-background);\n  border: var(--jp-border-width) solid var(--jp-border-color2);\n  flex: 1 1 auto;\n  height: 30px;\n  padding: 0px 12px;\n  margin: 0 4px 0 0;\n}\n\n.dask-URLInput-wrapper:focus-within {\n  border: var(--jp-border-width) solid var(--md-blue-500);\n  box-shadow: inset 0 0 4px var(--md-blue-300);\n}\n\n.dask-URLInput-wrapper input {\n  background: transparent;\n  float: left;\n  border: none;\n  outline: none;\n  font-size: var(--jp-ui-font-size1);\n  color: var(--jp-ui-font-color0);\n  width: calc(100% - 18px);\n  line-height: 28px;\n}\n\n.dask-URLInput-wrapper::placeholder {\n  color: var(--jp-ui-font-color3);\n  font-size: var(--jp-ui-font-size1);\n}\n\n.dask-UrlInput .jp-ToolbarButton {\n  flex: 0 0 auto;\n  margin: 0 0 0 4px;\n  background-color: var(--jp-layout-color2);\n  min-width: 16px;\n}\n\n/**\n * Rules for the dashboard panels.\n */\n.dask-DaskDashboard-widget {\n  background-color: white;\n}\n\n.dask-DaskDashboard-inactive {\n  position: absolute;\n  top: 0;\n  left: 0;\n  width: 100%;\n  height: 100%;\n  display: flex;\n  align-items: center;\n  justify-content: center;\n  color: var(--jp-ui-font-color3);\n  font-size: var(--jp-ui-font-size3);\n  background-color: var(--jp-layout-color0);\n  z-index: 10;\n}\n\n.dask-DaskDashboard-inactive:before {\n  content: '';\n  position: absolute;\n  top: 0;\n  left: 0;\n  width: 100%;\n  height: 100%;\n  background-image: url(" + p + ");\n  background-repeat: no-repeat;\n  background-position: center;\n  opacity: 0.1;\n}\n\n/**\n * Rules related to the cluster manager.\n */\n\n.dask-DaskClusterManager {\n  border-top: 6px solid var(--jp-toolbar-border-color);\n}\n\n.dask-DaskClusterManager .jp-Toolbar {\n  align-items: center;\n}\n\n.dask-DaskClusterManager .jp-Toolbar .dask-DaskClusterManager-label {\n  flex: 0 0 auto;\n  font-weight: 600;\n  text-transform: uppercase;\n  letter-spacing: 1px;\n  font-size: var(--jp-ui-font-size0);\n  padding: 8px 8px 8px 12px;\n  margin: 0px;\n}\n\n.dask-DaskClusterManager button.jp-Button > span {\n  display: flex;\n  flex-direction: row;\n  align-items: center;\n}\n\n.dask-ClusterListing ul.dask-ClusterListing-list {\n  list-style-type: none;\n  padding: 0;\n  margin: 0;\n}\n\n.dask-ClusterListingItem {\n  display: inline-block;\n  list-style-type: none;\n  padding: 8px;\n  width: 100%;\n  white-space: nowrap;\n  overflow: hidden;\n  text-overflow: ellipsis;\n  cursor: grab;\n}\n\n.dask-ClusterListingItem-drag {\n  opacity: 0.7;\n  color: var(--jp-ui-font-color1);\n  cursor: grabbing;\n  max-width: 260px;\n  transform: translateX(-50%) translateY(-50%);\n}\n\n.dask-ClusterListingItem-title {\n  margin: 0px;\n  font-size: var(--jp-ui-font-size2);\n}\n\n.dask-ClusterListingItem-link a {\n  text-decoration: none;\n  color: var(--jp-content-link-color);\n}\n\n.dask-ClusterListingItem-link a:hover {\n  text-decoration: underline;\n}\n\n.dask-ClusterListingItem-link a:visited {\n  color: var(--jp-content-link-color);\n}\n\n.dask-ClusterListingItem:hover {\n  background: var(--jp-layout-color2);\n}\n\n.dask-ClusterListingItem.jp-mod-active {\n  color: white;\n  background: var(--jp-brand-color0);\n}\n\n.dask-ClusterListingItem.jp-mod-active a,\n.dask-ClusterListingItem.jp-mod-active a:visited {\n  color: white;\n}\n\n.dask-ClusterListingItem button.jp-mod-styled {\n  background-color: transparent;\n}\n\n.dask-ClusterListingItem button.jp-mod-styled:hover {\n  background-color: var(--jp-layout-color3);\n}\n\n.dask-ClusterListingItem.jp-mod-active button.jp-mod-styled:hover {\n  background-color: var(--jp-brand-color1);\n}\n\n.dask-ClusterListingItem-button-panel {\n  display: flex;\n  align-content: center;\n}\n\nbutton.dask-ClusterListingItem-stop {\n  color: var(--jp-warn-color1);\n  font-weight: 600;\n}\n\nbutton.dask-ClusterListingItem-scale {\n  color: var(--jp-accent-color1);\n  font-weight: 600;\n}\n\n.dask-ClusterListingItem button.dask-ClusterListingItem-code.jp-mod-styled {\n  margin: 0 4px 0 4px;\n  background-repeat: no-repeat;\n  background-position: center;\n}\n\n/**\n * Rules for the scaling dialog.\n */\n\n.dask-ScalingHeader {\n  font-size: var(--jp-ui-font-size2);\n}\n\n.dask-ScalingSection {\n  margin-left: 24px;\n}\n\n.dask-ScalingSection-item {\n  display: flex;\n  align-items: center;\n  justify-content: space-around;\n  margin: 12px 0 12px 0;\n}\n\n.dask-ScalingHeader input[type='checkbox'] {\n  position: relative;\n  top: 4px;\n  left: 4px;\n  margin: 0 0 0 8px;\n}\n\n.dask-ScalingSection input[type='number'] {\n  width: 72px;\n}\n\n.dask-ScalingSection-label.dask-mod-disabled {\n  color: var(--jp-ui-font-color3);\n}\n\n.dask-ScalingSection input[type='number']:disabled {\n  color: var(--jp-ui-font-color3);\n}\n\n/**\n * Rules for the logos.\n */\n\n.dask-SearchIcon {\n  background-image: var(--jp-icon-search);\n}\n\n[data-jp-theme-light='true'] .dask-CodeIcon {\n  background-image: url(" + g + ");\n}\n\n[data-jp-theme-light='false'] .dask-CodeIcon {\n  background-image: url(" + v + ");\n}\n\n.dask-ClusterListingItem.jp-mod-active .dask-CodeIcon {\n  background-image: url(" + v + ");\n}\n\n.dask-DaskLogo {\n  background-image: url(" + p + ");\n}\n\n#setting-editor .dask-DaskLogo {\n  background-repeat: no-repeat;\n  background-size: 85%;\n  background-position: center;\n}\n", ""]);
-            const C = m
+                c = new URL(n(39), n.b),
+                d = new URL(n(810), n.b),
+                u = new URL(n(520), n.b),
+                h = i()(a()),
+                p = l()(c),
+                m = l()(d),
+                g = l()(u);
+            h.push([e.id, `:root {\n  --dask-launch-button-height: 24px;\n}\n\n/**\n * Rules related to the overall sidebar panel.\n */\n\n.dask-DaskSidebar {\n  background: var(--jp-layout-color1);\n  color: var(--jp-ui-font-color1);\n  font-size: var(--jp-ui-font-size1);\n  overflow: auto;\n}\n\n/**\n * Rules related to the dashboard launcher.\n */\n\n.dask-DashboardListing-inactive {\n  display: flex;\n  flex-direction: column;\n  justify-content: center;\n  align-items: center;\n  margin: 0;\n  padding: 0;\n  width: 100%;\n  height: 600px;\n  color: var(--jp-ui-font-color3);\n}\n\n.dask-DashboardListing-inactive-title {\n  font-size: var(--jp-ui-font-size3);\n  padding: 24px;\n  text-align: center;\n}\n\n.dask-DashboardListing-inactive-detail {\n  font-size: var(--jp-ui-font-size4);\n  padding: 24px;\n}\n\n.dask-DashboardListing-inactive:before {\n  content: '';\n  position: absolute;\n  top: 0;\n  left: 0;\n  width: 80%;\n  height: 80%;\n  background-image: url(${p});\n  background-repeat: no-repeat;\n  background-position: center;\n  opacity: 0.1;\n}\n\n.dask-DashboardListing-list {\n  margin: 8px;\n  padding: 0;\n  list-style-type: none;\n}\n\n.dask-DashboardListing-item {\n  margin-top: 4px;\n  margin-bottom: 4px;\n  margin-left: 12px;\n  margin-right: 12px;\n  white-space: nowrap;\n}\n\n.dask-DashboardListing-item button {\n  font-size: var(--jp-ui-font-size0);\n  border-radius: 2px;\n  line-height: 1em;\n  padding: 0px 8px;\n  width: 100%;\n}\n\n.dask-DashboardListing-item button.jp-mod-styled.jp-mod-accept {\n  height: var(--dask-launch-button-height);\n  color: #262326;\n  background-color: #ffc11e;\n  border: 1px solid #ffc11e;\n  text-transform: uppercase;\n}\n\n.dask-URLInput {\n  padding: 8px;\n  display: flex;\n  align-items: center;\n  background-color: var(--jp-layout-color1);\n  border-bottom: 1px solid var(--jp-border-color2);\n  box-shadow: var(--jp-toolbar-box-shadow);\n  z-index: 2;\n}\n\n.dask-URLInput-wrapper {\n  background-color: var(--jp-input-active-background);\n  border: var(--jp-border-width) solid var(--jp-border-color2);\n  flex: 1 1 auto;\n  height: 30px;\n  padding: 0px 12px;\n  margin: 0 4px 0 0;\n}\n\n.dask-URLInput-wrapper:focus-within {\n  border: var(--jp-border-width) solid var(--md-blue-500);\n  box-shadow: inset 0 0 4px var(--md-blue-300);\n}\n\n.dask-URLInput-wrapper input {\n  background: transparent;\n  float: left;\n  border: none;\n  outline: none;\n  font-size: var(--jp-ui-font-size1);\n  color: var(--jp-ui-font-color0);\n  width: calc(100% - 18px);\n  line-height: 28px;\n}\n\n.dask-URLInput-wrapper::placeholder {\n  color: var(--jp-ui-font-color3);\n  font-size: var(--jp-ui-font-size1);\n}\n\n.dask-UrlInput .jp-ToolbarButton {\n  flex: 0 0 auto;\n  margin: 0 0 0 4px;\n  background-color: var(--jp-layout-color2);\n  min-width: 16px;\n}\n\n/**\n * Rules for the dashboard panels.\n */\n.dask-DaskDashboard-widget {\n  background-color: white;\n}\n\n.dask-DaskDashboard-inactive {\n  position: absolute;\n  top: 0;\n  left: 0;\n  width: 100%;\n  height: 100%;\n  display: flex;\n  align-items: center;\n  justify-content: center;\n  color: var(--jp-ui-font-color3);\n  font-size: var(--jp-ui-font-size3);\n  background-color: var(--jp-layout-color0);\n  z-index: 10;\n}\n\n.dask-DaskDashboard-inactive:before {\n  content: '';\n  position: absolute;\n  top: 0;\n  left: 0;\n  width: 100%;\n  height: 100%;\n  background-image: url(${p});\n  background-repeat: no-repeat;\n  background-position: center;\n  opacity: 0.1;\n}\n\n/**\n * Rules related to the cluster manager.\n */\n\n.dask-DaskClusterManager {\n  border-top: 6px solid var(--jp-toolbar-border-color);\n}\n\n.dask-DaskClusterManager .jp-Toolbar {\n  align-items: center;\n}\n\n.dask-DaskClusterManager .jp-Toolbar .dask-DaskClusterManager-label {\n  flex: 0 0 auto;\n  font-weight: 600;\n  text-transform: uppercase;\n  letter-spacing: 1px;\n  font-size: var(--jp-ui-font-size0);\n  padding: 8px 8px 8px 12px;\n  margin: 0px;\n}\n\n.dask-DaskClusterManager button.jp-Button > span {\n  display: flex;\n  flex-direction: row;\n  align-items: center;\n}\n\n.dask-ClusterListing ul.dask-ClusterListing-list {\n  list-style-type: none;\n  padding: 0;\n  margin: 0;\n}\n\n.dask-ClusterListingItem {\n  display: inline-block;\n  list-style-type: none;\n  padding: 8px;\n  width: 100%;\n  white-space: nowrap;\n  overflow: hidden;\n  text-overflow: ellipsis;\n  cursor: grab;\n}\n\n.dask-ClusterListingItem-drag {\n  opacity: 0.7;\n  color: var(--jp-ui-font-color1);\n  cursor: grabbing;\n  max-width: 260px;\n  transform: translateX(-50%) translateY(-50%);\n}\n\n.dask-ClusterListingItem-title {\n  margin: 0px;\n  font-size: var(--jp-ui-font-size2);\n}\n\n.dask-ClusterListingItem-link a {\n  text-decoration: none;\n  color: var(--jp-content-link-color);\n}\n\n.dask-ClusterListingItem-link a:hover {\n  text-decoration: underline;\n}\n\n.dask-ClusterListingItem-link a:visited {\n  color: var(--jp-content-link-color);\n}\n\n.dask-ClusterListingItem:hover {\n  background: var(--jp-layout-color2);\n}\n\n.dask-ClusterListingItem.jp-mod-active {\n  color: white;\n  background: var(--jp-brand-color0);\n}\n\n.dask-ClusterListingItem.jp-mod-active a,\n.dask-ClusterListingItem.jp-mod-active a:visited {\n  color: white;\n}\n\n.dask-ClusterListingItem button.jp-mod-styled {\n  background-color: transparent;\n}\n\n.dask-ClusterListingItem button.jp-mod-styled:hover {\n  background-color: var(--jp-layout-color3);\n}\n\n.dask-ClusterListingItem.jp-mod-active button.jp-mod-styled:hover {\n  background-color: var(--jp-brand-color1);\n}\n\n.dask-ClusterListingItem-button-panel {\n  display: flex;\n  align-content: center;\n}\n\nbutton.dask-ClusterListingItem-stop {\n  color: var(--jp-warn-color1);\n  font-weight: 600;\n}\n\nbutton.dask-ClusterListingItem-scale {\n  color: var(--jp-accent-color1);\n  font-weight: 600;\n}\n\n.dask-ClusterListingItem button.dask-ClusterListingItem-code.jp-mod-styled {\n  margin: 0 4px 0 4px;\n  background-repeat: no-repeat;\n  background-position: center;\n}\n\n/**\n * Rules for the scaling dialog.\n */\n\n.dask-ScalingHeader {\n  font-size: var(--jp-ui-font-size2);\n}\n\n.dask-ScalingSection {\n  margin-left: 24px;\n}\n\n.dask-ScalingSection-item {\n  display: flex;\n  align-items: center;\n  justify-content: space-around;\n  margin: 12px 0 12px 0;\n}\n\n.dask-ScalingHeader input[type='checkbox'] {\n  position: relative;\n  top: 4px;\n  left: 4px;\n  margin: 0 0 0 8px;\n}\n\n.dask-ScalingSection input[type='number'] {\n  width: 72px;\n}\n\n.dask-ScalingSection-label.dask-mod-disabled {\n  color: var(--jp-ui-font-color3);\n}\n\n.dask-ScalingSection input[type='number']:disabled {\n  color: var(--jp-ui-font-color3);\n}\n\n/**\n * Rules for the logos.\n */\n\n.dask-SearchIcon {\n  background-image: var(--jp-icon-search);\n}\n\n[data-jp-theme-light='true'] .dask-CodeIcon {\n  background-image: url(${m});\n}\n\n[data-jp-theme-light='false'] .dask-CodeIcon {\n  background-image: url(${g});\n}\n\n.dask-ClusterListingItem.jp-mod-active .dask-CodeIcon {\n  background-image: url(${g});\n}\n\n.dask-DaskLogo {\n  background-image: url(${p});\n}\n\n#setting-editor .dask-DaskLogo {\n  background-repeat: no-repeat;\n  background-size: 85%;\n  background-position: center;\n}\n`, ""]);
+            const v = h
         },
         645: e => {
-            "use strict";
             e.exports = function(e) {
                 var t = [];
                 return t.toString = function() {
                     return this.map((function(t) {
-                        var n = e(t);
-                        return t[2] ? "@media ".concat(t[2], " {").concat(n, "}") : n
+                        var n = "",
+                            s = void 0 !== t[5];
+                        return t[4] && (n += "@supports (".concat(t[4], ") {")), t[2] && (n += "@media ".concat(t[2], " {")), s && (n += "@layer".concat(t[5].length > 0 ? " ".concat(t[5]) : "", " {")), n += e(t), s && (n += "}"), t[2] && (n += "}"), t[4] && (n += "}"), n
                     })).join("")
-                }, t.i = function(e, n, s) {
+                }, t.i = function(e, n, s, a, r) {
                     "string" == typeof e && (e = [
-                        [null, e, ""]
+                        [null, e, void 0]
                     ]);
-                    var a = {};
+                    var i = {};
                     if (s)
-                        for (var i = 0; i < this.length; i++) {
-                            var r = this[i][0];
-                            null != r && (a[r] = !0)
+                        for (var o = 0; o < this.length; o++) {
+                            var l = this[o][0];
+                            null != l && (i[l] = !0)
                         }
-                    for (var o = 0; o < e.length; o++) {
-                        var l = [].concat(e[o]);
-                        s && a[l[0]] || (n && (l[2] ? l[2] = "".concat(n, " and ").concat(l[2]) : l[2] = n), t.push(l))
+                    for (var c = 0; c < e.length; c++) {
+                        var d = [].concat(e[c]);
+                        s && i[d[0]] || (void 0 !== r && (void 0 === d[5] || (d[1] = "@layer".concat(d[5].length > 0 ? " ".concat(d[5]) : "", " {").concat(d[1], "}")), d[5] = r), n && (d[2] ? (d[1] = "@media ".concat(d[2], " {").concat(d[1], "}"), d[2] = n) : d[2] = n), a && (d[4] ? (d[1] = "@supports (".concat(d[4], ") {").concat(d[1], "}"), d[4] = a) : d[4] = "".concat(a)), t.push(d))
                     }
                 }, t
             }
         },
         667: e => {
-            "use strict";
             e.exports = function(e, t) {
-                return t || (t = {}), "string" != typeof(e = e && e.__esModule ? e.default : e) ? e : (/^['"].*['"]$/.test(e) && (e = e.slice(1, -1)), t.hash && (e += t.hash), /["'() \t\n]/.test(e) || t.needQuotes ? '"'.concat(e.replace(/"/g, '\\"').replace(/\n/g, "\\n"), '"') : e)
+                return t || (t = {}), e ? (e = String(e.__esModule ? e.default : e), /^['"].*['"]$/.test(e) && (e = e.slice(1, -1)), t.hash && (e += t.hash), /["'() \t\n]|(%20)/.test(e) || t.needQuotes ? '"'.concat(e.replace(/"/g, '\\"').replace(/\n/g, "\\n"), '"') : e) : e
             }
         },
-        379: (e, t, n) => {
-            "use strict";
-            var s, a = function() {
-                    var e = {};
-                    return function(t) {
-                        if (void 0 === e[t]) {
-                            var n = document.querySelector(t);
-                            if (window.HTMLIFrameElement && n instanceof window.HTMLIFrameElement) try {
-                                n = n.contentDocument.head
-                            } catch (e) {
-                                n = null
-                            }
-                            e[t] = n
-                        }
-                        return e[t]
-                    }
-                }(),
-                i = [];
+        81: e => {
+            e.exports = function(e) {
+                return e[1]
+            }
+        },
+        379: e => {
+            var t = [];
 
-            function r(e) {
-                for (var t = -1, n = 0; n < i.length; n++)
-                    if (i[n].identifier === e) {
-                        t = n;
+            function n(e) {
+                for (var n = -1, s = 0; s < t.length; s++)
+                    if (t[s].identifier === e) {
+                        n = s;
                         break
-                    } return t
+                    } return n
             }
 
-            function o(e, t) {
-                for (var n = {}, s = [], a = 0; a < e.length; a++) {
-                    var o = e[a],
-                        l = t.base ? o[0] + t.base : o[0],
-                        d = n[l] || 0,
-                        c = "".concat(l, " ").concat(d);
-                    n[l] = d + 1;
-                    var u = r(c),
-                        h = {
-                            css: o[1],
-                            media: o[2],
-                            sourceMap: o[3]
-                        }; - 1 !== u ? (i[u].references++, i[u].updater(h)) : i.push({
-                        identifier: c,
-                        updater: g(h, t),
-                        references: 1
-                    }), s.push(c)
+            function s(e, s) {
+                for (var r = {}, i = [], o = 0; o < e.length; o++) {
+                    var l = e[o],
+                        c = s.base ? l[0] + s.base : l[0],
+                        d = r[c] || 0,
+                        u = "".concat(c, " ").concat(d);
+                    r[c] = d + 1;
+                    var h = n(u),
+                        p = {
+                            css: l[1],
+                            media: l[2],
+                            sourceMap: l[3],
+                            supports: l[4],
+                            layer: l[5]
+                        };
+                    if (-1 !== h) t[h].references++, t[h].updater(p);
+                    else {
+                        var m = a(p, s);
+                        s.byIndex = o, t.splice(o, 0, {
+                            identifier: u,
+                            updater: m,
+                            references: 1
+                        })
+                    }
+                    i.push(u)
                 }
-                return s
+                return i
             }
 
-            function l(e) {
-                var t = document.createElement("style"),
-                    s = e.attributes || {};
-                if (void 0 === s.nonce) {
-                    var i = n.nc;
-                    i && (s.nonce = i)
-                }
-                if (Object.keys(s).forEach((function(e) {
-                        t.setAttribute(e, s[e])
-                    })), "function" == typeof e.insert) e.insert(t);
-                else {
-                    var r = a(e.insert || "head");
-                    if (!r) throw new Error("Couldn't find a style target. This probably means that the value for the 'insert' parameter is invalid.");
-                    r.appendChild(t)
-                }
-                return t
+            function a(e, t) {
+                var n = t.domAPI(t);
+                return n.update(e),
+                    function(t) {
+                        if (t) {
+                            if (t.css === e.css && t.media === e.media && t.sourceMap === e.sourceMap && t.supports === e.supports && t.layer === e.layer) return;
+                            n.update(e = t)
+                        } else n.remove()
+                    }
             }
-            var d, c = (d = [], function(e, t) {
-                return d[e] = t, d.filter(Boolean).join("\n")
-            });
-
-            function u(e, t, n, s) {
-                var a = n ? "" : s.media ? "@media ".concat(s.media, " {").concat(s.css, "}") : s.css;
-                if (e.styleSheet) e.styleSheet.cssText = c(t, a);
-                else {
-                    var i = document.createTextNode(a),
-                        r = e.childNodes;
-                    r[t] && e.removeChild(r[t]), r.length ? e.insertBefore(i, r[t]) : e.appendChild(i)
+            e.exports = function(e, a) {
+                var r = s(e = e || [], a = a || {});
+                return function(e) {
+                    e = e || [];
+                    for (var i = 0; i < r.length; i++) {
+                        var o = n(r[i]);
+                        t[o].references--
+                    }
+                    for (var l = s(e, a), c = 0; c < r.length; c++) {
+                        var d = n(r[c]);
+                        0 === t[d].references && (t[d].updater(), t.splice(d, 1))
+                    }
+                    r = l
                 }
             }
-
-            function h(e, t, n) {
-                var s = n.css,
-                    a = n.media,
-                    i = n.sourceMap;
-                if (a ? e.setAttribute("media", a) : e.removeAttribute("media"), i && "undefined" != typeof btoa && (s += "\n/*# sourceMappingURL=data:application/json;base64,".concat(btoa(unescape(encodeURIComponent(JSON.stringify(i)))), " */")), e.styleSheet) e.styleSheet.cssText = s;
-                else {
-                    for (; e.firstChild;) e.removeChild(e.firstChild);
-                    e.appendChild(document.createTextNode(s))
-                }
+        },
+        569: e => {
+            var t = {};
+            e.exports = function(e, n) {
+                var s = function(e) {
+                    if (void 0 === t[e]) {
+                        var n = document.querySelector(e);
+                        if (window.HTMLIFrameElement && n instanceof window.HTMLIFrameElement) try {
+                            n = n.contentDocument.head
+                        } catch (e) {
+                            n = null
+                        }
+                        t[e] = n
+                    }
+                    return t[e]
+                }(e);
+                if (!s) throw new Error("Couldn't find a style target. This probably means that the value for the 'insert' parameter is invalid.");
+                s.appendChild(n)
             }
-            var m = null,
-                p = 0;
-
-            function g(e, t) {
-                var n, s, a;
-                if (t.singleton) {
-                    var i = p++;
-                    n = m || (m = l(t)), s = u.bind(null, n, i, !1), a = u.bind(null, n, i, !0)
-                } else n = l(t), s = h.bind(null, n, t), a = function() {
-                    ! function(e) {
-                        if (null === e.parentNode) return !1;
-                        e.parentNode.removeChild(e)
-                    }(n)
+        },
+        216: e => {
+            e.exports = function(e) {
+                var t = document.createElement("style");
+                return e.setAttributes(t, e.attributes), e.insert(t, e.options), t
+            }
+        },
+        565: (e, t, n) => {
+            e.exports = function(e) {
+                var t = n.nc;
+                t && e.setAttribute("nonce", t)
+            }
+        },
+        795: e => {
+            e.exports = function(e) {
+                if ("undefined" == typeof document) return {
+                    update: function() {},
+                    remove: function() {}
                 };
-                return s(e),
-                    function(t) {
-                        if (t) {
-                            if (t.css === e.css && t.media === e.media && t.sourceMap === e.sourceMap) return;
-                            s(e = t)
-                        } else a()
+                var t = e.insertStyleElement(e);
+                return {
+                    update: function(n) {
+                        ! function(e, t, n) {
+                            var s = "";
+                            n.supports && (s += "@supports (".concat(n.supports, ") {")), n.media && (s += "@media ".concat(n.media, " {"));
+                            var a = void 0 !== n.layer;
+                            a && (s += "@layer".concat(n.layer.length > 0 ? " ".concat(n.layer) : "", " {")), s += n.css, a && (s += "}"), n.media && (s += "}"), n.supports && (s += "}");
+                            var r = n.sourceMap;
+                            r && "undefined" != typeof btoa && (s += "\n/*# sourceMappingURL=data:application/json;base64,".concat(btoa(unescape(encodeURIComponent(JSON.stringify(r)))), " */")), t.styleTagTransform(s, e, t.options)
+                        }(t, e, n)
+                    },
+                    remove: function() {
+                        ! function(e) {
+                            if (null === e.parentNode) return !1;
+                            e.parentNode.removeChild(e)
+                        }(t)
                     }
+                }
             }
+        },
+        589: e => {
             e.exports = function(e, t) {
-                (t = t || {}).singleton || "boolean" == typeof t.singleton || (t.singleton = (void 0 === s && (s = Boolean(window && document && document.all && !window.atob)), s));
-                var n = o(e = e || [], t);
-                return function(e) {
-                    if (e = e || [], "[object Array]" === Object.prototype.toString.call(e)) {
-                        for (var s = 0; s < n.length; s++) {
-                            var a = r(n[s]);
-                            i[a].references--
-                        }
-                        for (var l = o(e, t), d = 0; d < n.length; d++) {
-                            var c = r(n[d]);
-                            0 === i[c].references && (i[c].updater(), i.splice(c, 1))
-                        }
-                        n = l
-                    }
+                if (t.styleSheet) t.styleSheet.cssText = e;
+                else {
+                    for (; t.firstChild;) t.removeChild(t.firstChild);
+                    t.appendChild(document.createTextNode(e))
                 }
             }
         },
-        935: e => {
-            e.exports = "data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' fill='%23E0E0E0' width='24' height='24' viewBox='0 0 24 24'%3E%3Cpath fill='none' d='M0 0h24v24H0V0z'/%3E%3Cpath d='M9.4 16.6L4.8 12l4.6-4.6L8 6l-6 6 6 6 1.4-1.4zm5.2 0l4.6-4.6-4.6-4.6L16 6l6 6-6 6-1.4-1.4z'/%3E%3C/svg%3E"
+        520: e => {
+            e.exports = "data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' fill='%23E0E0E0' width='24' height='24' viewBox='0 0 24 24'%3e%3cpath fill='none' d='M0 0h24v24H0V0z'/%3e%3cpath d='M9.4 16.6L4.8 12l4.6-4.6L8 6l-6 6 6 6 1.4-1.4zm5.2 0l4.6-4.6-4.6-4.6L16 6l6 6-6 6-1.4-1.4z'/%3e%3c/svg%3e"
         },
-        490: e => {
-            e.exports = "data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' fill='%23616161' width='24' height='24' viewBox='0 0 24 24'%3E%3Cpath fill='none' d='M0 0h24v24H0V0z'/%3E%3Cpath d='M9.4 16.6L4.8 12l4.6-4.6L8 6l-6 6 6 6 1.4-1.4zm5.2 0l4.6-4.6-4.6-4.6L16 6l6 6-6 6-1.4-1.4z'/%3E%3C/svg%3E"
+        810: e => {
+            e.exports = "data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' fill='%23616161' width='24' height='24' viewBox='0 0 24 24'%3e%3cpath fill='none' d='M0 0h24v24H0V0z'/%3e%3cpath d='M9.4 16.6L4.8 12l4.6-4.6L8 6l-6 6 6 6 1.4-1.4zm5.2 0l4.6-4.6-4.6-4.6L16 6l6 6-6 6-1.4-1.4z'/%3e%3c/svg%3e"
         },
-        637: e => {
-            e.exports = "data:image/svg+xml,%3C!-- Generator: Adobe Illustrator 26.0.3, SVG Export Plug-In . SVG Version: 6.00 Build 0) --%3E %3Csvg version='1.1' id='Layer_1' xmlns='http://www.w3.org/2000/svg' xmlns:xlink='http://www.w3.org/1999/xlink' x='0px' y='0px' viewBox='0 0 512 512' style='enable-background:new 0 0 512 512;' xml:space='preserve'%3E %3Cstyle type='text/css'%3E .st0%7Bfill:%23FFC11E;%7D .st1%7Bfill:%2304255C;%7D .st2%7Bfill:%23FC6E6B;%7D .st3%7Bfill:%23FFFFFF;%7D .st4%7Bfill:%23EF1161;%7D %3C/style%3E %3Cg%3E %3Cpath class='st0' d='M143.71,157.61l126.5-72.99c1.25-0.72,2.02-2.05,2.02-3.5l0.01-43.77c0-6.48-2.66-12.9-7.83-16.81 c-6.69-5.06-15.28-5.56-22.33-1.48L65.13,121.17c-6.22,3.59-10.06,10.23-10.06,17.41L55,369.18c0,6.47,2.65,12.89,7.81,16.81 c6.68,5.07,15.29,5.57,22.35,1.49l37.48-21.62c1.25-0.72,2.02-2.05,2.02-3.5l0.05-171.85C124.71,176.93,131.95,164.4,143.71,157.61 z'/%3E %3Cpath class='st4' d='M446.95,124.53c-3.15-1.82-6.61-2.73-10.06-2.73c-3.45,0-6.9,0.91-10.05,2.73l-176.96,102.1 c-6.2,3.58-10.06,10.25-10.06,17.41l-0.07,231.47c0,7.27,3.76,13.78,10.05,17.42c6.3,3.64,13.81,3.64,20.11,0l176.95-102.11 c6.2-3.58,10.06-10.25,10.06-17.41L457,141.95C457,134.68,453.24,128.16,446.95,124.53z'/%3E %3Cpath class='st2' d='M240.95,211.14l116.78-67.38c1.25-0.72,2.02-2.05,2.02-3.5l0.02-50.98c0-6.48-2.66-12.9-7.83-16.81 c-6.69-5.06-15.27-5.55-22.33-1.48l-48.43,27.95L152.64,173.1c-6.22,3.59-10.06,10.23-10.06,17.41l-0.05,174.18l-0.02,56.41 c0,6.48,2.65,12.89,7.81,16.81c6.69,5.07,15.29,5.57,22.35,1.49l47.2-27.24c1.25-0.72,2.02-2.05,2.02-3.5l0.05-164.64 C221.95,230.46,229.19,217.92,240.95,211.14z'/%3E %3C/g%3E %3C/svg%3E"
+        39: e => {
+            e.exports = "data:image/svg+xml,%3c%3fxml version='1.0' encoding='utf-8'%3f%3e %3c!-- Generator: Adobe Illustrator 26.0.3%2c SVG Export Plug-In . SVG Version: 6.00 Build 0) --%3e %3csvg version='1.1' id='Layer_1' xmlns='http://www.w3.org/2000/svg' xmlns:xlink='http://www.w3.org/1999/xlink' x='0px' y='0px' viewBox='0 0 512 512' style='enable-background:new 0 0 512 512%3b' xml:space='preserve'%3e %3cstyle type='text/css'%3e .st0%7bfill:%23FFC11E%3b%7d .st1%7bfill:%2304255C%3b%7d .st2%7bfill:%23FC6E6B%3b%7d .st3%7bfill:white%3b%7d .st4%7bfill:%23EF1161%3b%7d %3c/style%3e %3cg%3e %3cpath class='st0' d='M143.71%2c157.61l126.5-72.99c1.25-0.72%2c2.02-2.05%2c2.02-3.5l0.01-43.77c0-6.48-2.66-12.9-7.83-16.81 c-6.69-5.06-15.28-5.56-22.33-1.48L65.13%2c121.17c-6.22%2c3.59-10.06%2c10.23-10.06%2c17.41L55%2c369.18c0%2c6.47%2c2.65%2c12.89%2c7.81%2c16.81 c6.68%2c5.07%2c15.29%2c5.57%2c22.35%2c1.49l37.48-21.62c1.25-0.72%2c2.02-2.05%2c2.02-3.5l0.05-171.85C124.71%2c176.93%2c131.95%2c164.4%2c143.71%2c157.61 z'/%3e %3cpath class='st4' d='M446.95%2c124.53c-3.15-1.82-6.61-2.73-10.06-2.73c-3.45%2c0-6.9%2c0.91-10.05%2c2.73l-176.96%2c102.1 c-6.2%2c3.58-10.06%2c10.25-10.06%2c17.41l-0.07%2c231.47c0%2c7.27%2c3.76%2c13.78%2c10.05%2c17.42c6.3%2c3.64%2c13.81%2c3.64%2c20.11%2c0l176.95-102.11 c6.2-3.58%2c10.06-10.25%2c10.06-17.41L457%2c141.95C457%2c134.68%2c453.24%2c128.16%2c446.95%2c124.53z'/%3e %3cpath class='st2' d='M240.95%2c211.14l116.78-67.38c1.25-0.72%2c2.02-2.05%2c2.02-3.5l0.02-50.98c0-6.48-2.66-12.9-7.83-16.81 c-6.69-5.06-15.27-5.55-22.33-1.48l-48.43%2c27.95L152.64%2c173.1c-6.22%2c3.59-10.06%2c10.23-10.06%2c17.41l-0.05%2c174.18l-0.02%2c56.41 c0%2c6.48%2c2.65%2c12.89%2c7.81%2c16.81c6.69%2c5.07%2c15.29%2c5.57%2c22.35%2c1.49l47.2-27.24c1.25-0.72%2c2.02-2.05%2c2.02-3.5l0.05-164.64 C221.95%2c230.46%2c229.19%2c217.92%2c240.95%2c211.14z'/%3e %3c/g%3e %3c/svg%3e"
         }
     }
 ]);
```

### Comparing `dask_labextension-6.2.0/dask_labextension/labextension/static/remoteEntry.48341a7428463ba2c6bb.js` & `dask_labextension-7.0.0/dask_labextension/labextension/static/remoteEntry.55eb452b48896f869659.js`

 * *Files 15% similar despite different names*

#### js-beautify {}

```diff
@@ -1,15 +1,15 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, o, a, i, l, u, s, d, f, c, p, h, b, v, m, g, y = {
-            391: (e, r, t) => {
+    var e, r, t, n, o, a, i, l, u, s, d, f, p, c, h, v, b = {
+            803: (e, r, t) => {
                 var n = {
-                        "./index": () => Promise.all([t.e(60), t.e(224)]).then((() => () => t(224))),
-                        "./extension": () => Promise.all([t.e(60), t.e(224)]).then((() => () => t(224)))
+                        "./index": () => t.e(11).then((() => () => t(11))),
+                        "./extension": () => t.e(11).then((() => () => t(11)))
                     },
                     o = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
                     })), t.R = void 0, r),
                     a = (e, r) => {
                         if (t.S) {
                             var n = "default",
@@ -20,116 +20,107 @@
                     };
                 t.d(r, {
                     get: () => o,
                     init: () => a
                 })
             }
         },
-        w = {};
+        m = {};
 
-    function j(e) {
-        var r = w[e];
+    function g(e) {
+        var r = m[e];
         if (void 0 !== r) return r.exports;
-        var t = w[e] = {
+        var t = m[e] = {
             id: e,
             exports: {}
         };
-        return y[e](t, t.exports, j), t.exports
+        return b[e](t, t.exports, g), t.exports
     }
-    j.m = y, j.c = w, j.n = e => {
+    g.m = b, g.c = m, g.n = e => {
         var r = e && e.__esModule ? () => e.default : () => e;
-        return j.d(r, {
+        return g.d(r, {
             a: r
         }), r
-    }, j.d = (e, r) => {
-        for (var t in r) j.o(r, t) && !j.o(e, t) && Object.defineProperty(e, t, {
+    }, g.d = (e, r) => {
+        for (var t in r) g.o(r, t) && !g.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
-    }, j.f = {}, j.e = e => Promise.all(Object.keys(j.f).reduce(((r, t) => (j.f[t](e, r), r)), [])), j.u = e => e + "." + {
-        60: "6b27874877fba88bc953",
-        114: "f9e3bc980911cf750147",
-        224: "86c44b816becca807a99"
-    } [e] + ".js?v=" + {
-        60: "6b27874877fba88bc953",
-        114: "f9e3bc980911cf750147",
-        224: "86c44b816becca807a99"
-    } [e], j.g = function() {
+    }, g.f = {}, g.e = e => Promise.all(Object.keys(g.f).reduce(((r, t) => (g.f[t](e, r), r)), [])), g.u = e => e + ".92ba9866db6ad7a7f70f.js?v=92ba9866db6ad7a7f70f", g.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
-    }(), j.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "dask-labextension:", j.l = (t, n, o, a) => {
+    }(), g.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "dask-labextension:", g.l = (t, n, o, a) => {
         if (e[t]) e[t].push(n);
         else {
             var i, l;
             if (void 0 !== o)
                 for (var u = document.getElementsByTagName("script"), s = 0; s < u.length; s++) {
                     var d = u[s];
                     if (d.getAttribute("src") == t || d.getAttribute("data-webpack") == r + o) {
                         i = d;
                         break
                     }
                 }
-            i || (l = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, j.nc && i.setAttribute("nonce", j.nc), i.setAttribute("data-webpack", r + o), i.src = t), e[t] = [n];
+            i || (l = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, g.nc && i.setAttribute("nonce", g.nc), i.setAttribute("data-webpack", r + o), i.src = t), e[t] = [n];
             var f = (r, n) => {
-                    i.onerror = i.onload = null, clearTimeout(c);
+                    i.onerror = i.onload = null, clearTimeout(p);
                     var o = e[t];
                     if (delete e[t], i.parentNode && i.parentNode.removeChild(i), o && o.forEach((e => e(n))), r) return r(n)
                 },
-                c = setTimeout(f.bind(null, void 0, {
+                p = setTimeout(f.bind(null, void 0, {
                     type: "timeout",
                     target: i
                 }), 12e4);
             i.onerror = f.bind(null, i.onerror), i.onload = f.bind(null, i.onload), l && document.head.appendChild(i)
         }
-    }, j.r = e => {
+    }, g.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
     }, (() => {
-        j.S = {};
+        g.S = {};
         var e = {},
             r = {};
-        j.I = (t, n) => {
+        g.I = (t, n) => {
             n || (n = []);
             var o = r[t];
             if (o || (o = r[t] = {}), !(n.indexOf(o) >= 0)) {
                 if (n.push(o), e[t]) return e[t];
-                j.o(j.S, t) || (j.S[t] = {});
-                var a = j.S[t],
+                g.o(g.S, t) || (g.S[t] = {});
+                var a = g.S[t],
                     i = "dask-labextension",
-                    l = (e, r, t, n) => {
-                        var o = a[e] = a[e] || {},
-                            l = o[r];
-                        (!l || !l.loaded && (!n != !l.eager ? n : i > l.from)) && (o[r] = {
-                            get: t,
-                            from: i,
-                            eager: !!n
-                        })
-                    },
-                    u = [];
-                return "default" === t && (l("@lumino/polling", "1.11.4", (() => Promise.all([j.e(114), j.e(60)]).then((() => () => j(114))))), l("dask-labextension", "6.2.0", (() => Promise.all([j.e(60), j.e(224)]).then((() => () => j(224)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                    l = [];
+                return "default" === t && ((e, r, t, n) => {
+                    var o = a[e] = a[e] || {},
+                        l = o[r];
+                    (!l || !l.loaded && (1 != !l.eager ? n : i > l.from)) && (o[r] = {
+                        get: () => g.e(11).then((() => () => g(11))),
+                        from: i,
+                        eager: !1
+                    })
+                })("dask-labextension", "7.0.0"), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
-        j.g.importScripts && (e = j.g.location + "");
-        var r = j.g.document;
+        g.g.importScripts && (e = g.g.location + "");
+        var r = g.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
             var t = r.getElementsByTagName("script");
             if (t.length)
                 for (var n = t.length - 1; n > -1 && !e;) e = t[n--].src
         }
         if (!e) throw new Error("Automatic publicPath is not supported in this browser");
-        e = e.replace(/#.*$/, "").replace(/\?.*$/, "").replace(/\/[^\/]+$/, "/"), j.p = e
+        e = e.replace(/#.*$/, "").replace(/\?.*$/, "").replace(/\/[^\/]+$/, "/"), g.p = e
     })(), t = e => {
         var r = e => e.split(".").map((e => +e == e ? +e : e)),
             t = /^([^-+]+)?(?:-([^+]+))?(?:\+(.+))?$/.exec(e),
             n = t[1] ? r(t[1]) : [];
         return t[2] && (n.length++, n.push.apply(n, r(t[2]))), t[3] && (n.push([]), n.push.apply(n, r(t[3]))), n
     }, n = (e, r) => {
         e = t(e), r = t(r);
@@ -187,115 +178,109 @@
                     u = !1, l--
                 } else {
                     if (l <= n || d < f != o) return !1;
                     u = !1
                 } else "s" != f && "n" != f && (u = !1, l--)
             }
         }
-        var c = [],
-            p = c.pop.bind(c);
+        var p = [],
+            c = p.pop.bind(p);
         for (i = 1; i < e.length; i++) {
             var h = e[i];
-            c.push(1 == h ? p() | p() : 2 == h ? p() & p() : h ? a(h, r) : !p())
+            p.push(1 == h ? c() | c() : 2 == h ? c() & c() : h ? a(h, r) : !c())
         }
-        return !!p()
+        return !!c()
     }, i = (e, r) => {
-        var t = j.S[e];
-        if (!t || !j.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
+        var t = g.S[e];
+        if (!t || !g.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, l = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
     }, u = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(n) + ")", s = (e, r, t, n) => {
         var o = l(e, t);
-        return a(n, o) || f(u(e, t, o, n)), c(e[t][o])
-    }, d = (e, r, t) => {
-        var o = e[r];
-        return (r = Object.keys(o).reduce(((e, r) => !a(t, r) || e && !n(e, r) ? e : r), 0)) && o[r]
-    }, f = e => {
+        return a(n, o) || d(u(e, t, o, n)), f(e[t][o])
+    }, d = e => {
         "undefined" != typeof console && console.warn && console.warn(e)
-    }, c = e => (e.loaded = 1, e.get()), h = (p = e => function(r, t, n, o) {
-        var a = j.I(r);
-        return a && a.then ? a.then(e.bind(e, r, j.S[r], t, n, o)) : e(r, j.S[r], t, n, o)
-    })(((e, r, t, n) => (i(e, t), s(r, 0, t, n)))), b = p(((e, r, t, n, o) => {
-        var a = r && j.o(r, t) && d(r, t, n);
-        return a ? c(a) : o()
-    })), v = {}, m = {
-        526: () => h("default", "@lumino/coreutils", [1, 1, 11, 0]),
-        840: () => h("default", "@lumino/signaling", [1, 1, 10, 0]),
-        127: () => h("default", "@jupyterlab/notebook", [1, 3, 6, 5]),
-        139: () => h("default", "@jupyterlab/services", [1, 6, 6, 5]),
-        271: () => h("default", "react", [1, 17, 0, 1]),
-        299: () => h("default", "@jupyterlab/settingregistry", [1, 3, 6, 5]),
-        303: () => h("default", "@jupyterlab/apputils", [1, 3, 6, 5]),
-        344: () => h("default", "@jupyterlab/coreutils", [1, 5, 6, 5]),
-        358: () => b("default", "@lumino/polling", [1, 1, 0, 4], (() => j.e(114).then((() => () => j(114))))),
-        456: () => h("default", "react-dom", [1, 17, 0, 1]),
-        520: () => h("default", "@lumino/domutils", [1, 1, 8, 0]),
-        535: () => h("default", "@jupyterlab/mainmenu", [1, 3, 6, 5]),
-        543: () => h("default", "@jupyterlab/console", [1, 3, 6, 5]),
-        548: () => h("default", "@jupyterlab/statedb", [1, 3, 6, 5]),
-        638: () => h("default", "@jupyterlab/application", [1, 3, 6, 5]),
-        694: () => h("default", "@lumino/dragdrop", [1, 1, 13, 0]),
-        745: () => h("default", "@jupyterlab/ui-components", [1, 3, 6, 5]),
-        832: () => h("default", "@lumino/widgets", [1, 1, 37, 2]),
-        918: () => h("default", "@lumino/algorithm", [1, 1, 9, 0])
-    }, g = {
-        60: [526, 840],
-        224: [127, 139, 271, 299, 303, 344, 358, 456, 520, 535, 543, 548, 638, 694, 745, 832, 918]
-    }, j.f.consumes = (e, r) => {
-        j.o(g, e) && g[e].forEach((e => {
-            if (j.o(v, e)) return r.push(v[e]);
+    }, f = e => (e.loaded = 1, e.get()), p = (e => function(r, t, n, o) {
+        var a = g.I(r);
+        return a && a.then ? a.then(e.bind(e, r, g.S[r], t, n, o)) : e(r, g.S[r], t, n)
+    })(((e, r, t, n) => (i(e, t), s(r, 0, t, n)))), c = {}, h = {
+        220: () => p("default", "@jupyterlab/application", [1, 4, 0, 4]),
+        833: () => p("default", "@jupyterlab/apputils", [1, 4, 1, 4]),
+        35: () => p("default", "@jupyterlab/ui-components", [1, 4, 0, 4]),
+        656: () => p("default", "@jupyterlab/console", [1, 4, 0, 4]),
+        664: () => p("default", "@jupyterlab/mainmenu", [1, 4, 0, 4]),
+        200: () => p("default", "@jupyterlab/settingregistry", [1, 4, 0, 4]),
+        731: () => p("default", "@jupyterlab/statedb", [1, 4, 0, 4]),
+        543: () => p("default", "@jupyterlab/notebook", [1, 4, 0, 4]),
+        697: () => p("default", "@lumino/algorithm", [1, 2, 0, 0]),
+        901: () => p("default", "@lumino/signaling", [1, 2, 0, 0]),
+        151: () => p("default", "@jupyterlab/coreutils", [1, 6, 0, 4]),
+        255: () => p("default", "@jupyterlab/services", [1, 7, 0, 4]),
+        930: () => p("default", "@lumino/coreutils", [1, 2, 0, 0]),
+        797: () => p("default", "@lumino/polling", [1, 2, 0, 0]),
+        778: () => p("default", "@lumino/widgets", [1, 2, 0, 1]),
+        29: () => p("default", "react", [1, 18, 2, 0]),
+        704: () => p("default", "react-dom", [1, 18, 2, 0]),
+        593: () => p("default", "@lumino/domutils", [1, 2, 0, 0]),
+        359: () => p("default", "@lumino/dragdrop", [1, 2, 0, 0])
+    }, v = {
+        11: [220, 833, 35, 656, 664, 200, 731, 543, 697, 901, 151, 255, 930, 797, 778, 29, 704, 593, 359]
+    }, g.f.consumes = (e, r) => {
+        g.o(v, e) && v[e].forEach((e => {
+            if (g.o(c, e)) return r.push(c[e]);
             var t = r => {
-                    v[e] = 0, j.m[e] = t => {
-                        delete j.c[e], t.exports = r()
+                    c[e] = 0, g.m[e] = t => {
+                        delete g.c[e], t.exports = r()
                     }
                 },
                 n = r => {
-                    delete v[e], j.m[e] = t => {
-                        throw delete j.c[e], r
+                    delete c[e], g.m[e] = t => {
+                        throw delete g.c[e], r
                     }
                 };
             try {
-                var o = m[e]();
-                o.then ? r.push(v[e] = o.then(t).catch(n)) : t(o)
+                var o = h[e]();
+                o.then ? r.push(c[e] = o.then(t).catch(n)) : t(o)
             } catch (e) {
                 n(e)
             }
         }))
     }, (() => {
+        g.b = document.baseURI || self.location.href;
         var e = {
             754: 0
         };
-        j.f.j = (r, t) => {
-            var n = j.o(e, r) ? e[r] : void 0;
+        g.f.j = (r, t) => {
+            var n = g.o(e, r) ? e[r] : void 0;
             if (0 !== n)
                 if (n) t.push(n[2]);
-                else if (60 != r) {
-                var o = new Promise(((t, o) => n = e[r] = [t, o]));
-                t.push(n[2] = o);
-                var a = j.p + j.u(r),
-                    i = new Error;
-                j.l(a, (t => {
-                    if (j.o(e, r) && (0 !== (n = e[r]) && (e[r] = void 0), n)) {
-                        var o = t && ("load" === t.type ? "missing" : t.type),
-                            a = t && t.target && t.target.src;
-                        i.message = "Loading chunk " + r + " failed.\n(" + o + ": " + a + ")", i.name = "ChunkLoadError", i.type = o, i.request = a, n[1](i)
-                    }
-                }), "chunk-" + r, r)
-            } else e[r] = 0
+                else {
+                    var o = new Promise(((t, o) => n = e[r] = [t, o]));
+                    t.push(n[2] = o);
+                    var a = g.p + g.u(r),
+                        i = new Error;
+                    g.l(a, (t => {
+                        if (g.o(e, r) && (0 !== (n = e[r]) && (e[r] = void 0), n)) {
+                            var o = t && ("load" === t.type ? "missing" : t.type),
+                                a = t && t.target && t.target.src;
+                            i.message = "Loading chunk " + r + " failed.\n(" + o + ": " + a + ")", i.name = "ChunkLoadError", i.type = o, i.request = a, n[1](i)
+                        }
+                    }), "chunk-" + r, r)
+                }
         };
         var r = (r, t) => {
                 var n, o, [a, i, l] = t,
                     u = 0;
                 if (a.some((r => 0 !== e[r]))) {
-                    for (n in i) j.o(i, n) && (j.m[n] = i[n]);
-                    l && l(j)
+                    for (n in i) g.o(i, n) && (g.m[n] = i[n]);
+                    l && l(g)
                 }
-                for (r && r(t); u < a.length; u++) o = a[u], j.o(e, o) && e[o] && e[o][0](), e[o] = 0
+                for (r && r(t); u < a.length; u++) o = a[u], g.o(e, o) && e[o] && e[o][0](), e[o] = 0
             },
             t = self.webpackChunkdask_labextension = self.webpackChunkdask_labextension || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
-    })(), j.nc = void 0;
-    var k = j(391);
-    (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB)["dask-labextension"] = k
+    })(), g.nc = void 0;
+    var y = g(803);
+    (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB)["dask-labextension"] = y
 })();
```

### Comparing `dask_labextension-6.2.0/dask_labextension/labextension/static/third-party-licenses.json` & `dask_labextension-7.0.0/dask_labextension/labextension/static/third-party-licenses.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7916666666666667%*

 * *Differences: {"'packages'": "{0: {'versionInfo': '6.8.1'}, 1: {'versionInfo': '3.3.3'}, delete: [0]}"}*

```diff
@@ -1,22 +1,16 @@
 {
     "packages": [
         {
-            "extractedText": "",
-            "licenseId": "BSD-3-Clause",
-            "name": "@lumino/polling",
-            "versionInfo": "1.11.4"
-        },
-        {
             "extractedText": "Copyright JS Foundation and other contributors\n\nPermission is hereby granted, free of charge, to any person obtaining\na copy of this software and associated documentation files (the\n'Software'), to deal in the Software without restriction, including\nwithout limitation the rights to use, copy, modify, merge, publish,\ndistribute, sublicense, and/or sell copies of the Software, and to\npermit persons to whom the Software is furnished to do so, subject to\nthe following conditions:\n\nThe above copyright notice and this permission notice shall be\nincluded in all copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED 'AS IS', WITHOUT WARRANTY OF ANY KIND,\nEXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF\nMERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.\nIN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY\nCLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,\nTORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE\nSOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.\n",
             "licenseId": "MIT",
             "name": "css-loader",
-            "versionInfo": "5.2.7"
+            "versionInfo": "6.8.1"
         },
         {
             "extractedText": "Copyright JS Foundation and other contributors\n\nPermission is hereby granted, free of charge, to any person obtaining\na copy of this software and associated documentation files (the\n'Software'), to deal in the Software without restriction, including\nwithout limitation the rights to use, copy, modify, merge, publish,\ndistribute, sublicense, and/or sell copies of the Software, and to\npermit persons to whom the Software is furnished to do so, subject to\nthe following conditions:\n\nThe above copyright notice and this permission notice shall be\nincluded in all copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED 'AS IS', WITHOUT WARRANTY OF ANY KIND,\nEXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF\nMERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.\nIN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY\nCLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,\nTORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE\nSOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.\n",
             "licenseId": "MIT",
             "name": "style-loader",
-            "versionInfo": "2.0.0"
+            "versionInfo": "3.3.3"
         }
     ]
 }
```

### Comparing `dask_labextension-6.2.0/dask_labextension/manager.py` & `dask_labextension-7.0.0/dask_labextension/manager.py`

 * *Files identical despite different names*

### Comparing `dask_labextension-6.2.0/dask_labextension/tests/test_manager.py` & `dask_labextension-7.0.0/dask_labextension/tests/test_manager.py`

 * *Files identical despite different names*

### Comparing `dask_labextension-6.2.0/dask_labextension.egg-info/PKG-INFO` & `dask_labextension-7.0.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,32 +1,67 @@
 Metadata-Version: 2.1
-Name: dask-labextension
-Version: 6.2.0
+Name: dask_labextension
+Version: 7.0.0
 Summary: A JupyterLab extension for Dask.
-Home-page: https://github.com/dask/dask-labextension
+Project-URL: Homepage, https://github.com/dask/dask-labextension
+Project-URL: Bug Tracker, https://github.com/dask/dask-labextension/issues
+Project-URL: Repository, https://github.com/dask/dask-labextension
 Author: Ian Rose, Matt Rocklin, Jacob Tomlinson
-License: BSD-3-Clause
-Keywords: dask,Jupyter,JupyterLab,JupyterLab3
-Platform: Linux
-Platform: Mac OS X
-Platform: Windows
+License: Copyright (c) 2016, Project Jupyter Contributors and Anaconda Inc.
+        All rights reserved.
+        
+        Redistribution and use in source and binary forms, with or without
+        modification, are permitted provided that the following conditions are met:
+        
+        1. Redistributions of source code must retain the above copyright notice, this
+           list of conditions and the following disclaimer.
+        
+        2. Redistributions in binary form must reproduce the above copyright notice,
+           this list of conditions and the following disclaimer in the documentation
+           and/or other materials provided with the distribution.
+        
+        3. Neither the name of the copyright holder nor the names of its
+           contributors may be used to endorse or promote products derived from
+           this software without specific prior written permission.
+        
+        THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+        AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+        IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+        DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
+        FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
+        DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
+        SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
+        CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
+        OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
+        OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+License-File: LICENSE
+Classifier: Framework :: Jupyter
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Classifier: Framework :: Jupyter
-Requires-Python: >=3.6
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
+Requires-Dist: bokeh!=2.0.0,>=1.0.0
+Requires-Dist: distributed>=1.24.1
+Requires-Dist: jupyter-server-proxy>=1.3.2
+Requires-Dist: jupyterlab<5,>=4.0.0
+Provides-Extra: test
+Requires-Dist: black; extra == 'test'
+Requires-Dist: flake8; extra == 'test'
+Requires-Dist: pytest; extra == 'test'
+Requires-Dist: pytest-cov; extra == 'test'
+Requires-Dist: pytest-html; extra == 'test'
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 # Dask JupyterLab Extension
 
-[![Build Status](https://travis-ci.org/dask/dask-labextension.svg?branch=main)](https://travis-ci.org/dask/dask-labextension) [![Version](https://img.shields.io/npm/v/dask-labextension.svg)](https://www.npmjs.com/package/dask-labextension) [![Downloads](https://img.shields.io/npm/dm/dask-labextension.svg)](https://www.npmjs.com/package/dask-labextension) [![Dependencies](https://img.shields.io/librariesio/release/npm/dask-labextension.svg)](https://libraries.io/npm/dask-labextension)
+[![Build Status](https://github.com/dask/dask-labextension/actions/workflows/python.yaml/badge.svg)](https://github.com/dask/dask-labextension/actions/workflows/python.yaml) [![Version](https://img.shields.io/npm/v/dask-labextension.svg)](https://www.npmjs.com/package/dask-labextension) [![Downloads](https://img.shields.io/npm/dm/dask-labextension.svg)](https://www.npmjs.com/package/dask-labextension) [![Dependencies](https://img.shields.io/librariesio/release/npm/dask-labextension.svg)](https://libraries.io/npm/dask-labextension)
 
 This package provides a JupyterLab extension to manage Dask clusters,
 as well as embed Dask's dashboard plots directly into JupyterLab panes.
 
 ![Dask Extension](./dask.png)
 
 ## Explanatory Video (5 minutes)
@@ -50,37 +85,45 @@
 One source common to Python users is the conda package manager.
 
 ```bash
 conda install jupyterlab
 conda install -c conda-forge nodejs
 ```
 
-### JupyterLab 3.0 or greater
+### JupyterLab 4.x
 
-You should be able to install this extension with pip or conda,
+Install the latest version of the extension for the JupyterLab 4
+support. You should be able to install this extension with pip or conda,
 and start using it immediately, e.g.
 
 ```bash
 pip install dask-labextension
 ```
 
 ### JupyterLab 3.x
 
-This extension includes both client-side and server-side components.
-Prior to JupyterLab 3.0 these needed to be installed separately,
-with node available on the machine.
+For JupyterLab 3.x, use lastest supported version `6.2.0`.
+
+```bash
+pip install dask-labextension==6.2.0
+```
+
+### JupyterLab 2.x
+
+Prior to JupyterLab 3.0 client-side and server-side components needed
+to be installed separately, with node available on the machine.
 
 The server-side component can be installed via pip or conda-forge:
 
 ```bash
-pip install dask_labextension
+pip install 'dask_labextension<5'
 ```
 
 ```bash
-conda install -c conda-forge dask-labextension
+conda install -c conda-forge 'dask-labextension<5'
 ```
 
 You then build the client-side extension into JupyterLab with:
 
 ```bash
 jupyter labextension install dask-labextension
 ```
@@ -236,26 +279,39 @@
 ## Publishing
 
 This extension contains a front-end component written in TypeScript
 and a back-end component written in Python.
 The front-end is compiled to Javascript during the build process
 and is distributed as static assets along with the Python package.
 
-_Note: Package versions are not prefixed with the letter `v`. You will need to disable this._
-
-```console
-$ jlpm config set version-tag-prefix ""
-```
-
 ### Release process
 
-This requires `node`, `build`, and `twine` to be installed.
+This requires `node`, `build`, `hatch` and `twine` to be installed.
 
 ```bash
-jlpm version [--major|--minor|--patch]  # updates package.json and creates git commit and tag
+# To set version (e.g. 7.0.0). hatch will update version string in package.json
+hatch version "7.0.0"
+
+# Examples of bumping version
+# minor bump
+hatch version minor  # Bumps to 7.1.0
+# beta pre-release bump
+# If published to pypi this can be installed with the --pre flag to pip
+hatch version b  # Bumps to 7.1.0b0
+# bump minor and beta
+hatch version minor,b  # Bumps to 7.2.0b0
+# release all of the --pre-release flags such as alpha beta rc
+hatch release  # Bumps to 7.2.0
+
+# git commit after bumping version
+git add package.json && git commit -m "Bump version: {version}"
+# Tag this version
+git tag {version}
+
+# Finally push to main, build and upload package to PyPI
 git push upstream main && git push upstream main --tags  # pushes to GitHub
 python -m build .  # Build the package
 twine upload dist/*  # Upload the package to PyPI
 ```
 
 ### Handling Javascript package version conflicts
```

#### html2text {}

```diff
@@ -1,44 +1,73 @@
-Metadata-Version: 2.1 Name: dask-labextension Version: 6.2.0 Summary: A
-JupyterLab extension for Dask. Home-page: https://github.com/dask/dask-
-labextension Author: Ian Rose, Matt Rocklin, Jacob Tomlinson License: BSD-3-
-Clause Keywords: dask,Jupyter,JupyterLab,JupyterLab3 Platform: Linux Platform:
-Mac OS X Platform: Windows Classifier: License :: OSI Approved :: BSD License
+Metadata-Version: 2.1 Name: dask_labextension Version: 7.0.0 Summary: A
+JupyterLab extension for Dask. Project-URL: Homepage, https://github.com/dask/
+dask-labextension Project-URL: Bug Tracker, https://github.com/dask/dask-
+labextension/issues Project-URL: Repository, https://github.com/dask/dask-
+labextension Author: Ian Rose, Matt Rocklin, Jacob Tomlinson License: Copyright
+(c) 2016, Project Jupyter Contributors and Anaconda Inc. All rights reserved.
+Redistribution and use in source and binary forms, with or without
+modification, are permitted provided that the following conditions are met: 1.
+Redistributions of source code must retain the above copyright notice, this
+list of conditions and the following disclaimer. 2. Redistributions in binary
+form must reproduce the above copyright notice, this list of conditions and the
+following disclaimer in the documentation and/or other materials provided with
+the distribution. 3. Neither the name of the copyright holder nor the names of
+its contributors may be used to endorse or promote products derived from this
+software without specific prior written permission. THIS SOFTWARE IS PROVIDED
+BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED
+WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF
+MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO
+EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT,
+INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING,
+BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE,
+DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
+LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE
+OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
+ADVISED OF THE POSSIBILITY OF SUCH DAMAGE. License-File: LICENSE Classifier:
+Framework :: Jupyter Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python Classifier: Programming Language ::
-Python :: 3 Classifier: Programming Language :: Python :: 3.6 Classifier:
-Programming Language :: Python :: 3.7 Classifier: Programming Language ::
-Python :: 3.8 Classifier: Framework :: Jupyter Requires-Python: >=3.6
-Description-Content-Type: text/markdown License-File: LICENSE # Dask JupyterLab
-Extension [![Build Status](https://travis-ci.org/dask/dask-
-labextension.svg?branch=main)](https://travis-ci.org/dask/dask-labextension) [!
-[Version](https://img.shields.io/npm/v/dask-labextension.svg)](https://
-www.npmjs.com/package/dask-labextension) [![Downloads](https://img.shields.io/
-npm/dm/dask-labextension.svg)](https://www.npmjs.com/package/dask-labextension)
-[![Dependencies](https://img.shields.io/librariesio/release/npm/dask-
-labextension.svg)](https://libraries.io/npm/dask-labextension) This package
-provides a JupyterLab extension to manage Dask clusters, as well as embed
-Dask's dashboard plots directly into JupyterLab panes. ![Dask Extension](./
-dask.png) ## Explanatory Video (5 minutes) [Dask_+_JupyterLab_Screencast] ##
-Requirements JupyterLab >= 1.0 distributed >= 1.24.1 ## Installation To install
-the Dask JupyterLab extension you will need to have JupyterLab installed. For
-JupyterLab < 3.0, you will also need [Node.js](https://nodejs.org/) version >=
-12. These are available through a variety of sources. One source common to
-Python users is the conda package manager. ```bash conda install jupyterlab
-conda install -c conda-forge nodejs ``` ### JupyterLab 3.0 or greater You
-should be able to install this extension with pip or conda, and start using it
-immediately, e.g. ```bash pip install dask-labextension ``` ### JupyterLab 3.x
-This extension includes both client-side and server-side components. Prior to
-JupyterLab 3.0 these needed to be installed separately, with node available on
-the machine. The server-side component can be installed via pip or conda-forge:
-```bash pip install dask_labextension ``` ```bash conda install -c conda-forge
-dask-labextension ``` You then build the client-side extension into JupyterLab
-with: ```bash jupyter labextension install dask-labextension ``` If you are
-running Notebook 5.2 or earlier, enable the server extension by running ```bash
-jupyter serverextension enable --py --sys-prefix dask_labextension ``` ##
-Configuration of Dask cluster management This extension has the ability to
+Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-
+Python: >=3.8 Requires-Dist: bokeh!=2.0.0,>=1.0.0 Requires-Dist:
+distributed>=1.24.1 Requires-Dist: jupyter-server-proxy>=1.3.2 Requires-Dist:
+jupyterlab<5,>=4.0.0 Provides-Extra: test Requires-Dist: black; extra == 'test'
+Requires-Dist: flake8; extra == 'test' Requires-Dist: pytest; extra == 'test'
+Requires-Dist: pytest-cov; extra == 'test' Requires-Dist: pytest-html; extra ==
+'test' Description-Content-Type: text/markdown # Dask JupyterLab Extension [!
+[Build Status](https://github.com/dask/dask-labextension/actions/workflows/
+python.yaml/badge.svg)](https://github.com/dask/dask-labextension/actions/
+workflows/python.yaml) [![Version](https://img.shields.io/npm/v/dask-
+labextension.svg)](https://www.npmjs.com/package/dask-labextension) [!
+[Downloads](https://img.shields.io/npm/dm/dask-labextension.svg)](https://
+www.npmjs.com/package/dask-labextension) [![Dependencies](https://
+img.shields.io/librariesio/release/npm/dask-labextension.svg)](https://
+libraries.io/npm/dask-labextension) This package provides a JupyterLab
+extension to manage Dask clusters, as well as embed Dask's dashboard plots
+directly into JupyterLab panes. ![Dask Extension](./dask.png) ## Explanatory
+Video (5 minutes) [Dask_+_JupyterLab_Screencast] ## Requirements JupyterLab >=
+1.0 distributed >= 1.24.1 ## Installation To install the Dask JupyterLab
+extension you will need to have JupyterLab installed. For JupyterLab < 3.0, you
+will also need [Node.js](https://nodejs.org/) version >= 12. These are
+available through a variety of sources. One source common to Python users is
+the conda package manager. ```bash conda install jupyterlab conda install -
+c conda-forge nodejs ``` ### JupyterLab 4.x Install the latest version of the
+extension for the JupyterLab 4 support. You should be able to install this
+extension with pip or conda, and start using it immediately, e.g. ```bash pip
+install dask-labextension ``` ### JupyterLab 3.x For JupyterLab 3.x, use
+lastest supported version `6.2.0`. ```bash pip install dask-labextension==6.2.0
+``` ### JupyterLab 2.x Prior to JupyterLab 3.0 client-side and server-side
+components needed to be installed separately, with node available on the
+machine. The server-side component can be installed via pip or conda-forge:
+```bash pip install 'dask_labextension<5' ``` ```bash conda install -c conda-
+forge 'dask-labextension<5' ``` You then build the client-side extension into
+JupyterLab with: ```bash jupyter labextension install dask-labextension ``` If
+you are running Notebook 5.2 or earlier, enable the server extension by running
+```bash jupyter serverextension enable --py --sys-prefix dask_labextension ```
+## Configuration of Dask cluster management This extension has the ability to
 launch and manage several kinds of Dask clusters, including local clusters and
 kubernetes clusters. Options for how to launch these clusters are set via the
 [dask configuration system](http://docs.dask.org/en/latest/
 configuration.html#configuration), typically a `.yml` file on disk. By default
 the extension launches a `LocalCluster`, for which the configuration is:
 ```yaml labextension: factory: module: 'dask.distributed' class: 'LocalCluster'
 args: [] kwargs: {} default: workers: null adapt: null # minimum: 0 # maximum:
@@ -87,19 +116,25 @@
 directory as an extension ``` To rebuild the extension: ```bash jlpm build ```
 You should then be able to refresh the JupyterLab page and it will pick up the
 changes to the extension. To run an editable install of the server extension,
 run ```bash pip install -e . jupyter serverextension enable --sys-prefix
 dask_labextension ``` ## Publishing This extension contains a front-end
 component written in TypeScript and a back-end component written in Python. The
 front-end is compiled to Javascript during the build process and is distributed
-as static assets along with the Python package. _Note: Package versions are not
-prefixed with the letter `v`. You will need to disable this._ ```console $ jlpm
-config set version-tag-prefix "" ``` ### Release process This requires `node`,
-`build`, and `twine` to be installed. ```bash jlpm version [--major|--minor|--
-patch] # updates package.json and creates git commit and tag git push upstream
-main && git push upstream main --tags # pushes to GitHub python -m build . #
-Build the package twine upload dist/* # Upload the package to PyPI ``` ###
-Handling Javascript package version conflicts Unlike Python, Javascript
-packages can include more than one version of the same dependency. Usually the
-`yarn` package manager handles this okay, but occasionally you might end up
-with conflicting versions, or with unexpected package bloat. You can try to fix
-this by deduplicating dependencies: ```bash jlpm yarn-deduplicate -s fewer ```
+as static assets along with the Python package. ### Release process This
+requires `node`, `build`, `hatch` and `twine` to be installed. ```bash # To set
+version (e.g. 7.0.0). hatch will update version string in package.json hatch
+version "7.0.0" # Examples of bumping version # minor bump hatch version minor
+# Bumps to 7.1.0 # beta pre-release bump # If published to pypi this can be
+installed with the --pre flag to pip hatch version b # Bumps to 7.1.0b0 # bump
+minor and beta hatch version minor,b # Bumps to 7.2.0b0 # release all of the --
+pre-release flags such as alpha beta rc hatch release # Bumps to 7.2.0 # git
+commit after bumping version git add package.json && git commit -m "Bump
+version: {version}" # Tag this version git tag {version} # Finally push to
+main, build and upload package to PyPI git push upstream main && git push
+upstream main --tags # pushes to GitHub python -m build . # Build the package
+twine upload dist/* # Upload the package to PyPI ``` ### Handling Javascript
+package version conflicts Unlike Python, Javascript packages can include more
+than one version of the same dependency. Usually the `yarn` package manager
+handles this okay, but occasionally you might end up with conflicting versions,
+or with unexpected package bloat. You can try to fix this by deduplicating
+dependencies: ```bash jlpm yarn-deduplicate -s fewer ```
```

### Comparing `dask_labextension-6.2.0/package.json` & `dask_labextension-7.0.0/dask_labextension/labextension/schemas/dask-labextension/package.json.orig`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8071895424836601%*

 * *Differences: {"'author'": "{replace: OrderedDict([('name', 'Ian Rose, Matt Rocklin, Jacob Tomlinson')])}",*

 * * "'dependencies'": "{'@jupyterlab/application': '^4.0.0', '@jupyterlab/apputils': '^4.0.0', "*

 * *                   "'@jupyterlab/codeeditor': '^4.0.0', '@jupyterlab/console': '^4.0.0', "*

 * *                   "'@jupyterlab/coreutils': '^6.0.0', '@jupyterlab/docregistry': '^4.0.0', "*

 * *                   "'@jupyterlab/mainmenu': '^4.0.0', '@jupyterlab/nbformat': '^4.0.0', "*

 * *                   "'@jupyterlab/notebook': '^4.0 […]*

```diff
@@ -1,56 +1,56 @@
 {
-    "author": "Ian Rose, Matt Rocklin, Jacob Tomlinson",
+    "author": {
+        "name": "Ian Rose, Matt Rocklin, Jacob Tomlinson"
+    },
     "bugs": {
         "url": "https://github.com/dask/dask-labextension/issues"
     },
     "dependencies": {
-        "@jupyterlab/application": "^3.0.0",
-        "@jupyterlab/apputils": "^3.0.0",
-        "@jupyterlab/codeeditor": "^3.0.0",
-        "@jupyterlab/console": "^3.0.0",
-        "@jupyterlab/coreutils": "^5.0.0",
-        "@jupyterlab/docregistry": "^3.4.3",
-        "@jupyterlab/mainmenu": "^3.0.0",
-        "@jupyterlab/nbformat": "^3.0.0",
-        "@jupyterlab/notebook": "^3.0.0",
-        "@jupyterlab/services": "^6.0.0",
-        "@jupyterlab/settingregistry": "^3.0.0",
-        "@jupyterlab/statedb": "^3.0.0",
-        "@jupyterlab/ui-components": "^3.0.0",
-        "@lumino/algorithm": "^1.3.3",
-        "@lumino/coreutils": "^1.5.3",
-        "@lumino/domutils": "^1.2.3",
-        "@lumino/dragdrop": "^1.7.1",
-        "@lumino/messaging": "^1.4.3",
-        "@lumino/polling": "^1.0.4",
-        "@lumino/signaling": "^1.4.3",
-        "@lumino/widgets": "^1.17.0",
-        "react": "^17.0.1",
-        "react-dom": "^17.0.1"
+        "@jupyterlab/application": "^4.0.0",
+        "@jupyterlab/apputils": "^4.0.0",
+        "@jupyterlab/codeeditor": "^4.0.0",
+        "@jupyterlab/console": "^4.0.0",
+        "@jupyterlab/coreutils": "^6.0.0",
+        "@jupyterlab/docregistry": "^4.0.0",
+        "@jupyterlab/mainmenu": "^4.0.0",
+        "@jupyterlab/nbformat": "^4.0.0",
+        "@jupyterlab/notebook": "^4.0.0",
+        "@jupyterlab/services": "^7.0.0",
+        "@jupyterlab/settingregistry": "^4.0.0",
+        "@jupyterlab/statedb": "^4.0.0",
+        "@jupyterlab/ui-components": "^4.0.0",
+        "@lumino/algorithm": "^2.0.0",
+        "@lumino/coreutils": "^2.0.0",
+        "@lumino/domutils": "^2.0.0",
+        "@lumino/dragdrop": "^2.0.0",
+        "@lumino/messaging": "^2.0.0",
+        "@lumino/polling": "^2.0.0",
+        "@lumino/signaling": "^2.0.0",
+        "@lumino/widgets": "^2.0.0",
+        "react": "^18.0.0",
+        "react-dom": "^18.0.0"
     },
     "description": "A JupyterLab extension for Dask.",
     "devDependencies": {
-        "@jupyterlab/builder": "^3.0.0",
-        "@types/react": "^17.0.0",
-        "@types/react-dom": "^17.0.0",
-        "@typescript-eslint/eslint-plugin": "^4.18.0",
-        "@typescript-eslint/parser": "^4.18.0",
-        "eslint": "^7.14.0",
-        "eslint-config-prettier": "^6.10.1",
-        "eslint-plugin-prettier": "^3.1.4",
+        "@jupyterlab/builder": "^4.0.0",
+        "@types/react": "^18.0.0",
+        "@types/react-dom": "^18.0.0",
+        "@typescript-eslint/eslint-plugin": "^5.59.0",
+        "@typescript-eslint/parser": "^5.59.0",
+        "eslint": "^8.4.0",
+        "eslint-config-prettier": "^8.8.0",
+        "eslint-plugin-prettier": "^4.2.1",
         "eslint-plugin-react": "^7.21.5",
         "mkdirp": "^1.0.3",
         "mocha": "^6.2.0",
         "npm-run-all": "^4.1.5",
-        "prettier": "^2.1.1",
-        "rimraf": "^3.0.2",
-        "typescript": "~4.1.3",
-        "yarn": "1.22.0",
-        "yarn-deduplicate": "^5.0.0"
+        "prettier": "^3.0.1",
+        "rimraf": "^5.0.0",
+        "typescript": "^5.1.3"
     },
     "files": [
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "schema/*.json",
         "style/**/*.{css,eot,gif,html,jpg,json,png,svg,woff2,ttf}"
     ],
     "homepage": "https://github.com/dask/dask-labextension",
@@ -64,22 +64,18 @@
         "jupyter",
         "jupyterlab",
         "jupyterlab-extension"
     ],
     "license": "BSD-3-Clause",
     "main": "lib/index.js",
     "name": "dask-labextension",
-    "private": false,
     "repository": {
         "type": "git",
         "url": "https://github.com/dask/dask-labextension"
     },
-    "resolutions": {
-        "@types/react": "~17.0.0"
-    },
     "scripts": {
         "build": "jlpm run build:lib && jlpm run build:labextension:dev",
         "build:labextension": "jupyter labextension build .",
         "build:labextension:dev": "jupyter labextension build --development True .",
         "build:lib": "tsc",
         "build:prod": "jlpm run build:lib && jlpm run build:labextension",
         "clean": "jlpm run clean:lib",
@@ -94,9 +90,9 @@
         "prettier:check": "prettier --list-different '**/*{.ts,.tsx,.js,.jsx,.css,.json,.md}'",
         "test": "mocha",
         "watch": "run-p watch:src watch:labextension",
         "watch:labextension": "jupyter labextension watch .",
         "watch:src": "tsc -w"
     },
     "types": "lib/index.d.ts",
-    "version": "6.2.0"
+    "version": "7.0.0"
 }
```

### Comparing `dask_labextension-6.2.0/schema/plugin.json` & `dask_labextension-7.0.0/schema/plugin.json`

 * *Files identical despite different names*

### Comparing `dask_labextension-6.2.0/src/clusters.tsx` & `dask_labextension-7.0.0/src/clusters.tsx`

 * *Files 0% similar despite different names*

```diff
@@ -682,16 +682,16 @@
  * A TSX functional component for rendering a single running cluster.
  */
 function ClusterListingItem(props: IClusterListingItemProps) {
   const { cluster, isActive, setActive, scale, stop, injectClientCode } = props;
   let itemClass = 'dask-ClusterListingItem';
   itemClass = isActive ? `${itemClass} jp-mod-active` : itemClass;
 
-  let minimum: JSX.Element | null = null;
-  let maximum: JSX.Element | null = null;
+  let minimum: React.JSX.Element | null = null;
+  let maximum: React.JSX.Element | null = null;
   if (cluster.adapt) {
     minimum = (
       <div className="dask-ClusterListingItem-stats">
         Minimum Workers: {cluster.adapt.minimum}
       </div>
     );
     maximum = (
```

### Comparing `dask_labextension-6.2.0/src/dashboard.tsx` & `dask_labextension-7.0.0/src/dashboard.tsx`

 * *Files identical despite different names*

### Comparing `dask_labextension-6.2.0/src/index.ts` & `dask_labextension-7.0.0/src/index.ts`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 import {
   ICommandPalette,
   ISessionContext,
   IWidgetTracker,
   WidgetTracker
 } from '@jupyterlab/apputils';
 
+import { Cell } from '@jupyterlab/cells';
+
 import { CodeEditor } from '@jupyterlab/codeeditor';
 
 import { LabIcon } from '@jupyterlab/ui-components';
 
 import { ConsolePanel, IConsoleTracker } from '@jupyterlab/console';
 
 import { DocumentRegistry } from '@jupyterlab/docregistry';
@@ -156,16 +158,16 @@
       return '';
     }
     // If so, find the link if we can.
     const link = await Private.checkKernel(kernel!);
     return link;
   };
 
-  const clientCodeInjector = (model: IClusterModel) => {
-    const editor = Private.getCurrentEditor(
+  const clientCodeInjector = async (model: IClusterModel) => {
+    const editor = await Private.getCurrentEditor(
       app,
       notebookTracker,
       consoleTracker
     );
     if (!editor) {
       return;
     }
@@ -193,15 +195,15 @@
     namespace: 'dask-dashboard-launcher'
   });
 
   // Add state restoration for the dashboard items.
   restorer.add(sidebar, id);
   void restorer.restore(tracker, {
     command: CommandIDs.launchPanel,
-    args: widget => ({ item: widget.item } || {}),
+    args: widget => ({ item: widget.item }) || {},
     name: widget => (widget.item && widget.item.route) || ''
   });
 
   labShell.add(sidebar, 'left', { rank: 200 });
 
   const updateDashboards = () => {
     const input = sidebar.dashboardLauncher.input;
@@ -378,15 +380,16 @@
         // Determine whether to use the auto-starting client.
         autoStartClient = settings.get('autoStartClient').composite as boolean;
         updateTrackers();
 
         // Determine whether to validate dashboards via browser check.
         browserDashboardCheck = settings.get('browserDashboardCheck')
           .composite as boolean;
-        sidebar.dashboardLauncher.input.browserDashboardCheck = browserDashboardCheck;
+        sidebar.dashboardLauncher.input.browserDashboardCheck =
+          browserDashboardCheck;
 
         //Determine whether to hide the cluster manager
         hideClusterManager = settings.get('hideClusterManager')
           .composite as boolean;
         sidebar.clusterManager.setHidden(hideClusterManager);
 
         // Get the default layout
@@ -544,20 +547,20 @@
 
   // Add a command to inject client connection code for a given cluster model.
   // This looks for a cluster model in the application context menu,
   // and looks for an editor among the currently active notebooks and consoles.
   // If either is not found, it bails.
   app.commands.addCommand(CommandIDs.injectClientCode, {
     label: 'Inject Dask Client Connection Code',
-    execute: () => {
+    execute: async () => {
       const cluster = Private.clusterFromClick(app, sidebar.clusterManager);
       if (!cluster) {
         return;
       }
-      clientCodeInjector(cluster);
+      await clientCodeInjector(cluster);
     }
   });
 
   // Add a command to launch a new cluster.
   app.commands.addCommand(CommandIDs.launchCluster, {
     label: args => (args['isPalette'] ? 'Launch New Cluster' : 'NEW'),
     execute: () => sidebar.clusterManager.start(),
@@ -726,18 +729,16 @@
   /**
    * Insert code to connect to a given cluster.
    */
   export function injectClientCode(
     cluster: IClusterModel,
     editor: CodeEditor.IEditor
   ): void {
-    const cursor = editor.getCursorPosition();
-    const offset = editor.getOffsetAt(cursor);
     const code = getClientCode(cluster);
-    editor.model.value.insert(offset, code);
+    editor.model.sharedModel.setSource(code);
   }
 
   /**
    * Get code to connect to a given cluster.
    */
   export function getClientCode(cluster: IClusterModel): string {
     return `from dask.distributed import Client
@@ -770,44 +771,51 @@
       const current = consoleTracker.currentWidget;
       kernel = current.sessionContext.session?.kernel;
     }
     return kernel;
   }
 
   /**
+   * Wait until the cell is ready and return a promise
+   * that fullfils to editor
+   */
+  export async function getEditor(
+    cell: Cell
+  ): Promise<CodeEditor.IEditor | null | undefined> {
+    await cell.ready;
+    return cell && cell.editor;
+  }
+
+  /**
    * Get the currently focused editor in the application,
    * checking both notebooks and consoles.
    * In the case of a notebook, it creates a new cell above the currently
    * active cell and then returns that.
    */
-  export function getCurrentEditor(
+  export async function getCurrentEditor(
     app: JupyterFrontEnd,
     notebookTracker: INotebookTracker,
     consoleTracker: IConsoleTracker
-  ): CodeEditor.IEditor | null | undefined {
+  ): Promise<CodeEditor.IEditor | null | undefined> {
     // Get a handle on the most relevant kernel,
     // whether it is attached to a notebook or a console.
     let current = app.shell.currentWidget;
     let editor: CodeEditor.IEditor | null | undefined;
     if (current && notebookTracker.has(current)) {
       NotebookActions.insertAbove((current as NotebookPanel).content);
-      const cell = (current as NotebookPanel).content.activeCell;
-      editor = cell && cell.editor;
+      return getEditor((current as NotebookPanel).content.activeCell);
     } else if (current && consoleTracker.has(current)) {
-      const cell = (current as ConsolePanel).console.promptCell;
-      editor = cell && cell.editor;
+      return getEditor((current as ConsolePanel).console.promptCell);
     } else if (notebookTracker.currentWidget) {
       const current = notebookTracker.currentWidget;
       NotebookActions.insertAbove(current.content);
-      const cell = current.content.activeCell;
-      editor = cell && cell.editor;
+      return getEditor(current.content.activeCell);
     } else if (consoleTracker.currentWidget) {
       const current = consoleTracker.currentWidget;
-      const cell = current.console.promptCell;
-      editor = cell && cell.editor;
+      return getEditor(current.console.promptCell);
     }
     return editor;
   }
 
   /**
    * Get a cluster model based on the application context menu click node.
    */
```

### Comparing `dask_labextension-6.2.0/src/scaling.tsx` & `dask_labextension-7.0.0/src/scaling.tsx`

 * *Files identical despite different names*

### Comparing `dask_labextension-6.2.0/src/sidebar.ts` & `dask_labextension-7.0.0/src/sidebar.ts`

 * *Files identical despite different names*

### Comparing `dask_labextension-6.2.0/style/dask.svg` & `dask_labextension-7.0.0/style/dask.svg`

 * *Files identical despite different names*

### Comparing `dask_labextension-6.2.0/style/index.css` & `dask_labextension-7.0.0/style/index.css`

 * *Files identical despite different names*

### Comparing `dask_labextension-6.2.0/tsconfig.json` & `dask_labextension-7.0.0/tsconfig.json`

 * *Files identical despite different names*

