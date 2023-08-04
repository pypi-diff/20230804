# Comparing `tmp/jupyterlab_pyflyby-4.3.0.tar.gz` & `tmp/jupyterlab_pyflyby-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyterlab_pyflyby-4.3.0.tar", last modified: Fri Aug  4 07:17:17 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `jupyterlab_pyflyby-4.3.0.tar` & `jupyterlab_pyflyby-5.0.0.tar`

### file list

```diff
@@ -1,49 +1,46 @@
-drwxrwsr-x   0 choudhdi (20059) choudhdi (20059)        0 2023-08-04 07:17:17.083346 jupyterlab_pyflyby-4.3.0/
--rw-rw-r--   0 choudhdi (20059) choudhdi (20059)     1504 2023-05-24 09:35:51.000000 jupyterlab_pyflyby-4.3.0/LICENSE.txt
--rw-rw-r--   0 choudhdi (20059) choudhdi (20059)      455 2023-05-24 09:35:51.000000 jupyterlab_pyflyby-4.3.0/MANIFEST.in
--rw-rw-r--   0 choudhdi (20059) choudhdi (20059)     4670 2023-08-04 07:17:17.082971 jupyterlab_pyflyby-4.3.0/PKG-INFO
--rw-rw-r--   0 choudhdi (20059) choudhdi (20059)     3943 2023-08-03 07:55:58.000000 jupyterlab_pyflyby-4.3.0/README.md
--rw-rw-r--   0 choudhdi (20059) choudhdi (20059)      197 2023-05-24 09:35:51.000000 jupyterlab_pyflyby-4.3.0/install.json
-drwxrwsr-x   0 choudhdi (20059) choudhdi (20059)        0 2023-08-04 07:17:17.063021 jupyterlab_pyflyby-4.3.0/jupyter-config/
--rw-rw-r--   0 choudhdi (20059) choudhdi (20059)       93 2023-05-24 09:35:51.000000 jupyterlab_pyflyby-4.3.0/jupyter-config/jupyterlab_pyflyby.json
-drwxrwsr-x   0 choudhdi (20059) choudhdi (20059)        0 2023-08-04 07:17:17.065556 jupyterlab_pyflyby-4.3.0/jupyterlab_pyflyby/
--rw-rw-r--   0 choudhdi (20059) choudhdi (20059)      788 2023-08-03 07:55:58.000000 jupyterlab_pyflyby-4.3.0/jupyterlab_pyflyby/__init__.py
--rw-rw-r--   0 choudhdi (20059) choudhdi (20059)      441 2023-08-03 07:55:58.000000 jupyterlab_pyflyby-4.3.0/jupyterlab_pyflyby/_version.py
--rw-rw-r--   0 choudhdi (20059) choudhdi (20059)     3050 2023-08-03 07:55:58.000000 jupyterlab_pyflyby-4.3.0/jupyterlab_pyflyby/handlers.py
-drwxrwsr-x   0 choudhdi (20059) choudhdi (20059)        0 2023-08-04 07:17:17.069563 jupyterlab_pyflyby-4.3.0/jupyterlab_pyflyby/labextension/
--rw-rw-r--   0 choudhdi (20059) choudhdi (20059)     3188 2023-08-04 07:15:37.000000 jupyterlab_pyflyby-4.3.0/jupyterlab_pyflyby/labextension/package.json
-drwxrwsr-x   0 choudhdi (20059) choudhdi (20059)        0 2023-08-04 07:17:17.051388 jupyterlab_pyflyby-4.3.0/jupyterlab_pyflyby/labextension/schemas/
-drwxrwsr-x   0 choudhdi (20059) choudhdi (20059)        0 2023-08-04 07:17:17.051710 jupyterlab_pyflyby-4.3.0/jupyterlab_pyflyby/labextension/schemas/@deshaw/
-drwxrwsr-x   0 choudhdi (20059) choudhdi (20059)        0 2023-08-04 07:17:17.070616 jupyterlab_pyflyby-4.3.0/jupyterlab_pyflyby/labextension/schemas/@deshaw/jupyterlab-pyflyby/
--rw-rw-r--   0 choudhdi (20059) choudhdi (20059)     3045 2023-08-04 07:15:36.000000 jupyterlab_pyflyby-4.3.0/jupyterlab_pyflyby/labextension/schemas/@deshaw/jupyterlab-pyflyby/package.json.orig
--rw-rw-r--   0 choudhdi (20059) choudhdi (20059)      836 2023-08-04 07:15:36.000000 jupyterlab_pyflyby-4.3.0/jupyterlab_pyflyby/labextension/schemas/@deshaw/jupyterlab-pyflyby/plugin.json
-drwxrwsr-x   0 choudhdi (20059) choudhdi (20059)        0 2023-08-04 07:17:17.074441 jupyterlab_pyflyby-4.3.0/jupyterlab_pyflyby/labextension/static/
--rw-rw-r--   0 choudhdi (20059) choudhdi (20059)     7739 2023-08-04 07:15:37.000000 jupyterlab_pyflyby-4.3.0/jupyterlab_pyflyby/labextension/static/227.d0383463ef62876fb46f.js
--rw-rw-r--   0 choudhdi (20059) choudhdi (20059)    11373 2023-08-04 07:15:37.000000 jupyterlab_pyflyby-4.3.0/jupyterlab_pyflyby/labextension/static/586.e31cbc5a08f78b80f8bc.js
--rw-rw-r--   0 choudhdi (20059) choudhdi (20059)     3385 2023-08-04 07:15:37.000000 jupyterlab_pyflyby-4.3.0/jupyterlab_pyflyby/labextension/static/747.895f1f90006f2cd62bc9.js
--rw-rw-r--   0 choudhdi (20059) choudhdi (20059)     7392 2023-08-04 07:15:37.000000 jupyterlab_pyflyby-4.3.0/jupyterlab_pyflyby/labextension/static/remoteEntry.d287a35fa86eaa718ab8.js
--rw-rw-r--   0 choudhdi (20059) choudhdi (20059)      169 2023-08-04 07:15:36.000000 jupyterlab_pyflyby-4.3.0/jupyterlab_pyflyby/labextension/static/style.js
--rw-rw-r--   0 choudhdi (20059) choudhdi (20059)     6188 2023-08-04 07:15:37.000000 jupyterlab_pyflyby-4.3.0/jupyterlab_pyflyby/labextension/static/third-party-licenses.json
-drwxrwsr-x   0 choudhdi (20059) choudhdi (20059)        0 2023-08-04 07:17:17.069188 jupyterlab_pyflyby-4.3.0/jupyterlab_pyflyby.egg-info/
--rw-rw-r--   0 choudhdi (20059) choudhdi (20059)     4670 2023-08-04 07:17:16.000000 jupyterlab_pyflyby-4.3.0/jupyterlab_pyflyby.egg-info/PKG-INFO
--rw-rw-r--   0 choudhdi (20059) choudhdi (20059)     1218 2023-08-04 07:17:16.000000 jupyterlab_pyflyby-4.3.0/jupyterlab_pyflyby.egg-info/SOURCES.txt
--rw-rw-r--   0 choudhdi (20059) choudhdi (20059)        1 2023-08-04 07:17:16.000000 jupyterlab_pyflyby-4.3.0/jupyterlab_pyflyby.egg-info/dependency_links.txt
--rw-rw-r--   0 choudhdi (20059) choudhdi (20059)        1 2023-05-24 09:39:43.000000 jupyterlab_pyflyby-4.3.0/jupyterlab_pyflyby.egg-info/not-zip-safe
--rw-rw-r--   0 choudhdi (20059) choudhdi (20059)       71 2023-08-04 07:17:16.000000 jupyterlab_pyflyby-4.3.0/jupyterlab_pyflyby.egg-info/requires.txt
--rw-rw-r--   0 choudhdi (20059) choudhdi (20059)       19 2023-08-04 07:17:16.000000 jupyterlab_pyflyby-4.3.0/jupyterlab_pyflyby.egg-info/top_level.txt
--rw-rw-r--   0 choudhdi (20059) choudhdi (20059)     3045 2023-08-04 07:14:08.000000 jupyterlab_pyflyby-4.3.0/package.json
--rw-rw-r--   0 choudhdi (20059) choudhdi (20059)      274 2023-08-03 07:55:58.000000 jupyterlab_pyflyby-4.3.0/pyproject.toml
--rw-rw-r--   0 choudhdi (20059) choudhdi (20059)       38 2023-08-04 07:17:17.083413 jupyterlab_pyflyby-4.3.0/setup.cfg
--rw-rw-r--   0 choudhdi (20059) choudhdi (20059)     2286 2023-08-03 07:55:58.000000 jupyterlab_pyflyby-4.3.0/setup.py
-drwxrwsr-x   0 choudhdi (20059) choudhdi (20059)        0 2023-08-04 07:17:17.076334 jupyterlab_pyflyby-4.3.0/src/
--rw-rw-r--   0 choudhdi (20059) choudhdi (20059)     3649 2023-08-04 07:14:08.000000 jupyterlab_pyflyby-4.3.0/src/cellUtils.ts
--rw-rw-r--   0 choudhdi (20059) choudhdi (20059)      401 2023-08-04 07:14:08.000000 jupyterlab_pyflyby-4.3.0/src/constants.ts
--rw-rw-r--   0 choudhdi (20059) choudhdi (20059)     1094 2023-08-03 07:55:58.000000 jupyterlab_pyflyby-4.3.0/src/handler.ts
--rw-rw-r--   0 choudhdi (20059) choudhdi (20059)    20637 2023-08-04 07:14:08.000000 jupyterlab_pyflyby-4.3.0/src/index.tsx
-drwxrwsr-x   0 choudhdi (20059) choudhdi (20059)        0 2023-08-04 07:17:17.082502 jupyterlab_pyflyby-4.3.0/style/
--rw-rw-r--   0 choudhdi (20059) choudhdi (20059)        0 2023-08-03 07:55:58.000000 jupyterlab_pyflyby-4.3.0/style/base.css
--rw-rw-r--   0 choudhdi (20059) choudhdi (20059)       25 2023-08-03 07:55:58.000000 jupyterlab_pyflyby-4.3.0/style/index.css
--rw-rw-r--   0 choudhdi (20059) choudhdi (20059)       21 2023-05-24 09:35:51.000000 jupyterlab_pyflyby-4.3.0/style/index.js
--rw-rw-r--   0 choudhdi (20059) choudhdi (20059)      750 2023-08-04 07:14:08.000000 jupyterlab_pyflyby-4.3.0/style/tidy-import.svg
--rw-rw-r--   0 choudhdi (20059) choudhdi (20059)      555 2023-08-04 07:14:08.000000 jupyterlab_pyflyby-4.3.0/tsconfig.json
--rw-rw-r--   0 choudhdi (20059) choudhdi (20059)   204830 2023-08-04 07:14:08.000000 jupyterlab_pyflyby-4.3.0/yarn.lock
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 jupyterlab_pyflyby-5.0.0/.eslintignore
+-rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 jupyterlab_pyflyby-5.0.0/.eslintrc.js
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 jupyterlab_pyflyby-5.0.0/.gitattributes
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jupyterlab_pyflyby-5.0.0/.prettierignore
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 jupyterlab_pyflyby-5.0.0/.prettierrc
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 jupyterlab_pyflyby-5.0.0/.stylelintrc
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 jupyterlab_pyflyby-5.0.0/.yarnrc.yml
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 jupyterlab_pyflyby-5.0.0/CHANGELOG.md
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 jupyterlab_pyflyby-5.0.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 jupyterlab_pyflyby-5.0.0/MANIFEST.in
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 jupyterlab_pyflyby-5.0.0/install.json
+-rw-r--r--   0        0        0     3753 2020-02-02 00:00:00.000000 jupyterlab_pyflyby-5.0.0/package.json
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 jupyterlab_pyflyby-5.0.0/tsconfig.json
+-rw-r--r--   0        0        0   209252 2020-02-02 00:00:00.000000 jupyterlab_pyflyby-5.0.0/yarn.lock
+-rwxr-xr-x   0        0        0       67 2020-02-02 00:00:00.000000 jupyterlab_pyflyby-5.0.0/.husky/pre-commit
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 jupyterlab_pyflyby-5.0.0/.husky/_/.gitignore
+-rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 jupyterlab_pyflyby-5.0.0/.husky/_/husky.sh
+-rw-r--r--   0        0        0    47943 2020-02-02 00:00:00.000000 jupyterlab_pyflyby-5.0.0/docs/pyflyby.gif
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 jupyterlab_pyflyby-5.0.0/jupyter-config/jupyterlab_pyflyby.json
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 jupyterlab_pyflyby-5.0.0/jupyter-config/nb-config/jupyterlab_pyflyby.json
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 jupyterlab_pyflyby-5.0.0/jupyter-config/server-config/jupyterlab_pyflyby.json
+-rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 jupyterlab_pyflyby-5.0.0/jupyterlab_pyflyby/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_pyflyby-5.0.0/jupyterlab_pyflyby/_version.py
+-rw-r--r--   0        0        0     3087 2020-02-02 00:00:00.000000 jupyterlab_pyflyby-5.0.0/jupyterlab_pyflyby/handlers.py
+-rw-r--r--   0        0        0     3895 2020-02-02 00:00:00.000000 jupyterlab_pyflyby-5.0.0/jupyterlab_pyflyby/labextension/package.json
+-rw-r--r--   0        0        0     3753 2020-02-02 00:00:00.000000 jupyterlab_pyflyby-5.0.0/jupyterlab_pyflyby/labextension/schemas/@deshaw/jupyterlab-pyflyby/package.json.orig
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 jupyterlab_pyflyby-5.0.0/jupyterlab_pyflyby/labextension/schemas/@deshaw/jupyterlab-pyflyby/plugin.json
+-rw-r--r--   0        0        0     7739 2020-02-02 00:00:00.000000 jupyterlab_pyflyby-5.0.0/jupyterlab_pyflyby/labextension/static/227.d0383463ef62876fb46f.js
+-rw-r--r--   0        0        0     8329 2020-02-02 00:00:00.000000 jupyterlab_pyflyby-5.0.0/jupyterlab_pyflyby/labextension/static/36.815b80fd2ca5b739309a.js
+-rw-r--r--   0        0        0     4032 2020-02-02 00:00:00.000000 jupyterlab_pyflyby-5.0.0/jupyterlab_pyflyby/labextension/static/747.642119a933d152ff1ed4.js
+-rw-r--r--   0        0        0     7199 2020-02-02 00:00:00.000000 jupyterlab_pyflyby-5.0.0/jupyterlab_pyflyby/labextension/static/remoteEntry.2f3f2d893fd3c5c9aea1.js
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 jupyterlab_pyflyby-5.0.0/jupyterlab_pyflyby/labextension/static/style.js
+-rw-r--r--   0        0        0     6188 2020-02-02 00:00:00.000000 jupyterlab_pyflyby-5.0.0/jupyterlab_pyflyby/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 jupyterlab_pyflyby-5.0.0/schema/plugin.json
+-rw-r--r--   0        0        0     3650 2020-02-02 00:00:00.000000 jupyterlab_pyflyby-5.0.0/src/cellUtils.ts
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 jupyterlab_pyflyby-5.0.0/src/constants.ts
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 jupyterlab_pyflyby-5.0.0/src/handler.ts
+-rw-r--r--   0        0        0    16167 2020-02-02 00:00:00.000000 jupyterlab_pyflyby-5.0.0/src/index.tsx
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 jupyterlab_pyflyby-5.0.0/style/base.css
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 jupyterlab_pyflyby-5.0.0/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_pyflyby-5.0.0/style/index.js
+-rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 jupyterlab_pyflyby-5.0.0/.gitignore
+-rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 jupyterlab_pyflyby-5.0.0/LICENSE.txt
+-rw-r--r--   0        0        0     4333 2020-02-02 00:00:00.000000 jupyterlab_pyflyby-5.0.0/README.md
+-rw-r--r--   0        0        0     2526 2020-02-02 00:00:00.000000 jupyterlab_pyflyby-5.0.0/pyproject.toml
+-rw-r--r--   0        0        0     7167 2020-02-02 00:00:00.000000 jupyterlab_pyflyby-5.0.0/PKG-INFO
```

### Comparing `jupyterlab_pyflyby-4.3.0/LICENSE.txt` & `jupyterlab_pyflyby-5.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jupyterlab_pyflyby-4.3.0/PKG-INFO` & `jupyterlab_pyflyby-5.0.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,7 @@
-Metadata-Version: 2.1
-Name: jupyterlab_pyflyby
-Version: 4.3.0
-Summary: A labextension to integrate pyflyby with notebooks
-Home-page: https://github.com/deshaw/jupyterlab-pyflyby
-License: BSD-3-Clause
-Keywords: Jupyter,JupyterLab,JupyterLab3,ipython,pyflyby
-Platform: Linux
-Platform: Mac OS X
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Framework :: Jupyter
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE.txt
-
 # @deshaw/jupyterlab_pyflyby
 
 [![PyPI version][pypi-image]][pypi-url] [![PyPI DM][pypi-dm-image]][pypi-url]
 [![Github Actions Status][github-status-image]][github-status-url]
 
 A labextension to integrate pyflyby with notebooks
 
@@ -30,15 +9,15 @@
 
 ![Screenshot](https://github.com/deshaw/jupyterlab-pyflyby/blob/main/docs/pyflyby.gif 'PyFlyBy')
 
 You can decide cell where imports should be added by adding 'pyflyby-cell' cell tag to it.
 
 ## Requirements
 
-- JupyterLab >= 3.0
+- JupyterLab >= 4.0
 
 ## Install
 
 ```bash
 pip install jupyterlab_pyflyby
 ```
 
@@ -92,30 +71,29 @@
 git tag vX.Z.Y
 git push && git push --tags
 ```
 
 3. Create the artifacts
 
 ```
-rm -rf dist
-python setup.py sdist bdist_wheel
+rm -rf dist tsconfig.tsbuildinfo lib jupyterlab_pyflyby/labextension jupyterlab_pyflyby-*.tar.gz jupyterlab_pyflyby-*.whl
+hatch build .
 ```
 
 4. Test this against the test pypi. You can then install from here to test as well:
 
 ```
-twine upload --repository-url https://test.pypi.org/legacy/ dist/*
-# In a new venv
+twine upload --repository-url https://test.pypi.org/legacy/ jupyterlab_pyflyby-*.tar.gz jupyterlab_pyflyby-*.whl# In a new venv
 pip install --index-url https://test.pypi.org/simple/ jupyterlab_pyflyby
 ```
 
 5. Upload this to pypi:
 
 ```
-twine upload dist/*
+twine upload jupyterlab_pyflyby-*.tar.gz jupyterlab_pyflyby-*.whl
 ```
 
 ### Uninstall
 
 ```bash
 pip uninstall jupyterlab_pyflyby
 ```
@@ -130,14 +108,17 @@
     </a>
 </p>
 
 ## License
 
 This project is released under a [BSD-3-Clause license](https://github.com/deshaw/jupyterlab-pyflyby/blob/master/LICENSE.txt).
 
+We love contributions! Before you can contribute, please sign and submit this [Contributor License Agreement (CLA)](https://www.deshaw.com/oss/cla).
+This CLA is in place to protect all users of this project.
+
 "Jupyter" is a trademark of the NumFOCUS foundation, of which Project Jupyter is a part.
 
 [pypi-url]: https://pypi.org/project/jupyterlab-pyflyby
 [pypi-image]: https://img.shields.io/pypi/v/jupyterlab-pyflyby
 [pypi-dm-image]: https://img.shields.io/pypi/dm/jupyterlab-pyflyby
 [github-status-image]: https://github.com/deshaw/jupyterlab-pyflyby/workflows/Build/badge.svg
 [github-status-url]: https://github.com/deshaw/jupyterlab-pyflyby/actions?query=workflow%3ABuild
```

#### html2text {}

```diff
@@ -1,61 +1,56 @@
-Metadata-Version: 2.1 Name: jupyterlab_pyflyby Version: 4.3.0 Summary: A
-labextension to integrate pyflyby with notebooks Home-page: https://github.com/
-deshaw/jupyterlab-pyflyby License: BSD-3-Clause Keywords:
-Jupyter,JupyterLab,JupyterLab3,ipython,pyflyby Platform: Linux Platform: Mac OS
-X Classifier: License :: OSI Approved :: BSD License Classifier: Programming
-Language :: Python Classifier: Programming Language :: Python :: 3 Classifier:
-Programming Language :: Python :: 3.7 Classifier: Programming Language ::
-Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Framework :: Jupyter Requires-Python: >=3.7 Description-Content-Type: text/
-markdown Provides-Extra: dev License-File: LICENSE.txt # @deshaw/
-jupyterlab_pyflyby [![PyPI version][pypi-image]][pypi-url] [![PyPI DM][pypi-dm-
-image]][pypi-url] [![Github Actions Status][github-status-image]][github-
-status-url] A labextension to integrate pyflyby with notebooks [Pyflyby](https:
-//github.com/deshaw/pyflyby) helps you get rid of the tedious task of recalling
-and adding import statements. This labextension takes it further by adding the
-import statements automatically in your notebook. For eg. executing `np.arange
-(10)` ![Screenshot](https://github.com/deshaw/jupyterlab-pyflyby/blob/main/
-docs/pyflyby.gif 'PyFlyBy') You can decide cell where imports should be added
-by adding 'pyflyby-cell' cell tag to it. ## Requirements - JupyterLab >= 3.0 ##
-Install ```bash pip install jupyterlab_pyflyby ``` ## Contributing ###
-Development install Note: You will need NodeJS to build the extension package.
-The `jlpm` command is JupyterLab's pinned version of [yarn](https://
-yarnpkg.com/) that is installed with JupyterLab. You may use `yarn` or `npm` in
-lieu of `jlpm` below. ```bash # Clone the repo to your local environment #
-Change directory to the jupyterlab_pyflyby directory # Install package in
-development mode pip install -e . # Link your development version of the
-extension with JupyterLab jupyter-labextension develop . --overwrite # Rebuild
-extension Typescript source after making changes jlpm run build ``` You can
-watch the source directory and run JupyterLab at the same time in different
+# @deshaw/jupyterlab_pyflyby [![PyPI version][pypi-image]][pypi-url] [![PyPI
+DM][pypi-dm-image]][pypi-url] [![Github Actions Status][github-status-image]]
+[github-status-url] A labextension to integrate pyflyby with notebooks
+[Pyflyby](https://github.com/deshaw/pyflyby) helps you get rid of the tedious
+task of recalling and adding import statements. This labextension takes it
+further by adding the import statements automatically in your notebook. For eg.
+executing `np.arange(10)` ![Screenshot](https://github.com/deshaw/jupyterlab-
+pyflyby/blob/main/docs/pyflyby.gif 'PyFlyBy') You can decide cell where imports
+should be added by adding 'pyflyby-cell' cell tag to it. ## Requirements -
+JupyterLab >= 4.0 ## Install ```bash pip install jupyterlab_pyflyby ``` ##
+Contributing ### Development install Note: You will need NodeJS to build the
+extension package. The `jlpm` command is JupyterLab's pinned version of [yarn]
+(https://yarnpkg.com/) that is installed with JupyterLab. You may use `yarn` or
+`npm` in lieu of `jlpm` below. ```bash # Clone the repo to your local
+environment # Change directory to the jupyterlab_pyflyby directory # Install
+package in development mode pip install -e . # Link your development version of
+the extension with JupyterLab jupyter-labextension develop . --overwrite #
+Rebuild extension Typescript source after making changes jlpm run build ``` You
+can watch the source directory and run JupyterLab at the same time in different
 terminals to watch for changes in the extension's source and automatically
 rebuild the extension. ```bash # Watch the source directory in one terminal,
 automatically rebuilding when needed jlpm run watch # Run JupyterLab in another
 terminal jupyter-lab ``` With the watch command running, every saved change
 will immediately be built locally and available in your running JupyterLab.
 Refresh JupyterLab to load the change in your browser (you may need to wait
 several seconds for the extension to be rebuilt). By default, the `jlpm run
 build` command generates the source maps for this extension to make it easier
 to debug using the browser dev tools. To also generate source maps for the
 JupyterLab core extensions, you can run the following command: ```bash jupyter
 lab build --minimize=False ``` #### Publishing Before starting, you'll need to
 have run: `pip install twine jupyter_packaging` 1. Update the version in
 `package.json` and update the release date in `CHANGELOG.md` 2. Commit the
 change in step 1, tag it, then push it ``` git commit -am  git tag vX.Z.Y git
-push && git push --tags ``` 3. Create the artifacts ``` rm -rf dist python
-setup.py sdist bdist_wheel ``` 4. Test this against the test pypi. You can then
-install from here to test as well: ``` twine upload --repository-url https://
-test.pypi.org/legacy/ dist/* # In a new venv pip install --index-url https://
+push && git push --tags ``` 3. Create the artifacts ``` rm -rf dist
+tsconfig.tsbuildinfo lib jupyterlab_pyflyby/labextension jupyterlab_pyflyby-
+*.tar.gz jupyterlab_pyflyby-*.whl hatch build . ``` 4. Test this against the
+test pypi. You can then install from here to test as well: ``` twine upload --
+repository-url https://test.pypi.org/legacy/ jupyterlab_pyflyby-*.tar.gz
+jupyterlab_pyflyby-*.whl# In a new venv pip install --index-url https://
 test.pypi.org/simple/ jupyterlab_pyflyby ``` 5. Upload this to pypi: ``` twine
-upload dist/* ``` ### Uninstall ```bash pip uninstall jupyterlab_pyflyby ``` ##
-History This plugin was contributed back to the community by the [D. E. Shaw
-group](https://www.deshaw.com/).
+upload jupyterlab_pyflyby-*.tar.gz jupyterlab_pyflyby-*.whl ``` ### Uninstall
+```bash pip uninstall jupyterlab_pyflyby ``` ## History This plugin was
+contributed back to the community by the [D. E. Shaw group](https://
+www.deshaw.com/).
                                [D._E._Shaw_Logo]
 ## License This project is released under a [BSD-3-Clause license](https://
-github.com/deshaw/jupyterlab-pyflyby/blob/master/LICENSE.txt). "Jupyter" is a
-trademark of the NumFOCUS foundation, of which Project Jupyter is a part.
-[pypi-url]: https://pypi.org/project/jupyterlab-pyflyby [pypi-image]: https://
-img.shields.io/pypi/v/jupyterlab-pyflyby [pypi-dm-image]: https://
-img.shields.io/pypi/dm/jupyterlab-pyflyby [github-status-image]: https://
-github.com/deshaw/jupyterlab-pyflyby/workflows/Build/badge.svg [github-status-
-url]: https://github.com/deshaw/jupyterlab-pyflyby/
-actions?query=workflow%3ABuild
+github.com/deshaw/jupyterlab-pyflyby/blob/master/LICENSE.txt). We love
+contributions! Before you can contribute, please sign and submit this
+[Contributor License Agreement (CLA)](https://www.deshaw.com/oss/cla). This CLA
+is in place to protect all users of this project. "Jupyter" is a trademark of
+the NumFOCUS foundation, of which Project Jupyter is a part. [pypi-url]: https:
+//pypi.org/project/jupyterlab-pyflyby [pypi-image]: https://img.shields.io/
+pypi/v/jupyterlab-pyflyby [pypi-dm-image]: https://img.shields.io/pypi/dm/
+jupyterlab-pyflyby [github-status-image]: https://github.com/deshaw/jupyterlab-
+pyflyby/workflows/Build/badge.svg [github-status-url]: https://github.com/
+deshaw/jupyterlab-pyflyby/actions?query=workflow%3ABuild
```

### Comparing `jupyterlab_pyflyby-4.3.0/jupyterlab_pyflyby/handlers.py` & `jupyterlab_pyflyby-5.0.0/jupyterlab_pyflyby/handlers.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,50 +1,50 @@
-from jupyter_server.base.handlers import APIHandler
-from jupyter_server.utils import url_path_join
-import tornado
 import json
-from notebook.base.handlers import IPythonHandler
 import os
 import subprocess
 
+from jupyter_server.base.handlers import APIHandler
+from jupyter_server.utils import url_path_join
+import tornado
+
+
+class Status(APIHandler):
+    """Checks if pyflyby is loaded by default in ipython session
 
-class PyflybyStatus(IPythonHandler):
-    """
-    Checks if pyflyby is loaded by default in ipython session
     Return {"status": "loaded"} if included by default, else {"status": "not-loaded"}
     """
-
+    # Users must be authenticated to make requests to the jupyter server
+    @tornado.web.authenticated
     def get(self):
         from IPython.terminal.ipapp import load_default_config
 
         extensions = load_default_config().InteractiveShellApp.extensions.to_dict()
         if any(["pyflyby" in val for val in extensions.values()]):
             self.finish({"status": "loaded"})
         else:
             self.finish({"status": "not-loaded"})
 
 
-class InstallPyflyby(IPythonHandler):
-    """
-    Adds pyflyby to ipython extensions, to be included default everytime ipython is launched
-    """
+class Install(APIHandler):
+    """Adds pyflyby to ipython extensions.
 
+    Pyflyby will be included by default everytime ipython is launched.
+    """
+    @tornado.web.authenticated
     def post(self):
         try:
             subprocess.run(["py", "pyflyby.install_in_ipython_config_file"])
             self.finish({"result": "Installed pyflyby successfully"})
         except Exception as err:
             self.send_error({"result": "Pyflyby installation failed - {}".format(err)})
 
 
-class DisablePyflybyClient(IPythonHandler):
-    """
-    Disables jupyterlab-pyflyby labextension for user
-    """
-
+class Disable(APIHandler):
+    """Disables jupyterlab-pyflyby labextension for user"""
+    @tornado.web.authenticated
     def post(self):
         try:
             settings_dir = os.environ.get(
                 "JUPYTERLAB_SETTINGS_DIR",
                 os.path.join(os.environ.get("HOME"), ".jupyter/lab/user-settings"),
             )
             pyflyby_settings_file = os.path.join(
@@ -53,15 +53,16 @@
             installDialogDisplayed = (
                 True
                 if self.get_body_argument("installDialogDisplayed") == "true"
                 else False
             )
 
             settings = {"enabled": False}
-            # To remember dialog box to install pyflyby ipython extension was displayed for current user
+            # To remember dialog box to install pyflyby ipython extension was
+            # displayed for current user
             settings["installDialogDisplayed"] = installDialogDisplayed
 
             if os.path.exists(pyflyby_settings_file):
                 with open(pyflyby_settings_file, "r") as f:
                     settings = {**json.load(f), **settings}
 
             with open(pyflyby_settings_file, "w") as f:
@@ -72,16 +73,14 @@
                 {"result": "Could not disable pyflyby extension - {}".format(err)}
             )
 
 
 def setup_handlers(web_app):
     host_pattern = ".*$"
 
-    pyflyby_handlers = [
-        ("/pyflyby/pyflyby-status", PyflybyStatus),
-        ("/pyflyby/install-pyflyby", InstallPyflyby),
-        ("/pyflyby/disable-pyflyby", DisablePyflybyClient),
-    ]
     base_url = web_app.settings["base_url"]
-    pyflyby_handlers = [(url_path_join(base_url, v[0]), v[1]) for v in pyflyby_handlers]
-
-    web_app.add_handlers(host_pattern, pyflyby_handlers)
+    handlers = [
+        (url_path_join(base_url, "pyflyby", "pyflyby-status"), Status),
+        (url_path_join(base_url, "pyflyby", "install-pyflyby"), Install),
+        (url_path_join(base_url, "pyflyby", "disable-pyflyby"), Disable),
+    ]
+    web_app.add_handlers(host_pattern, handlers)
```

### Comparing `jupyterlab_pyflyby-4.3.0/jupyterlab_pyflyby/labextension/package.json` & `jupyterlab_pyflyby-5.0.0/package.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8165639185376028%*

 * *Differences: {"'dependencies'": "{'@jupyterlab/application': '^4.0.0', '@jupyterlab/apputils': '^4.0.0', "*

 * *                   "'@jupyterlab/docregistry': '^4.0.0', '@jupyterlab/nbformat': '^4.0.0', "*

 * *                   "'@jupyterlab/notebook': '^4.0.0', '@jupyterlab/services': '^7.0.0', "*

 * *                   "'@jupyterlab/settingregistry': '^4.0.0', '@lumino/algorithm': '^2.0.0', "*

 * *                   "'@lumino/coreutils': '^2.0.0', '@lumino/widgets': '^2.0.1'}",*

 * * "'devDependencies'": "{'@jupyterlab/builder': '^4.0.0', '@ […]*

```diff
@@ -1,57 +1,59 @@
 {
     "bugs": {
         "url": "https://github.com/deshaw/jupyterlab-pyflyby/issues"
     },
     "dependencies": {
-        "@jupyterlab/application": "^3.0.7",
-        "@jupyterlab/apputils": "^3.0.5",
-        "@jupyterlab/docregistry": "^3.0.7",
-        "@jupyterlab/nbformat": "^3.0.3",
-        "@jupyterlab/notebook": "^3.0.7",
-        "@jupyterlab/services": "^6.0.5",
-        "@jupyterlab/settingregistry": "^3.0.3",
-        "@lumino/algorithm": "^1.3.3",
-        "@lumino/coreutils": "^1.5.3",
-        "@lumino/widgets": "^1.16.1",
+        "@jupyterlab/application": "^4.0.0",
+        "@jupyterlab/apputils": "^4.0.0",
+        "@jupyterlab/docregistry": "^4.0.0",
+        "@jupyterlab/nbformat": "^4.0.0",
+        "@jupyterlab/notebook": "^4.0.0",
+        "@jupyterlab/services": "^7.0.0",
+        "@jupyterlab/settingregistry": "^4.0.0",
+        "@lumino/algorithm": "^2.0.0",
+        "@lumino/coreutils": "^2.0.0",
+        "@lumino/widgets": "^2.0.1",
         "debug": "^4.1.1"
     },
     "description": "A labextension to integrate pyflyby with notebooks",
     "devDependencies": {
-        "@jupyterlab/builder": "^3.0.0",
+        "@jupyterlab/builder": "^4.0.0",
         "@types/debug": "^4.1.5",
-        "@typescript-eslint/eslint-plugin": "^4.8.1",
-        "@typescript-eslint/parser": "^4.8.1",
-        "eslint": "^7.14.0",
-        "eslint-config-prettier": "^8.1.0",
-        "eslint-plugin-prettier": "^3.1.4",
-        "husky": "^4.2.3",
+        "@types/json-schema": "^7.0.11",
+        "@types/react": "^18.0.26",
+        "@typescript-eslint/eslint-plugin": "^5.55.0",
+        "@typescript-eslint/parser": "^5.55.0",
+        "css-loader": "^6.7.1",
+        "eslint": "^8.36.0",
+        "eslint-config-prettier": "^8.7.0",
+        "eslint-plugin-prettier": "^4.2.1",
+        "husky": "^8.0.0",
+        "mkdirp": "^1.0.3",
         "npm-run-all": "^4.1.5",
-        "prettier": "^2.2.1",
-        "rimraf": "^3.0.2",
-        "typescript": "~4.1.3"
+        "prettier": "^2.8.7",
+        "rimraf": "^4.4.1",
+        "source-map-loader": "^1.0.2",
+        "style-loader": "^3.3.1",
+        "stylelint": "^14.9.1",
+        "stylelint-config-prettier": "^9.0.4",
+        "stylelint-config-recommended": "^8.0.0",
+        "stylelint-config-standard": "^26.0.0",
+        "stylelint-prettier": "^2.0.0",
+        "typescript": "~5.0.2",
+        "yjs": "^13.5.40"
     },
     "files": [
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "schema/*",
         "style/index.js"
     ],
     "homepage": "https://github.com/deshaw/jupyterlab-pyflyby",
-    "husky": {
-        "hooks": {
-            "pre-commit": "jlpm run lint"
-        }
-    },
     "jupyterlab": {
-        "_build": {
-            "extension": "./extension",
-            "load": "static/remoteEntry.d287a35fa86eaa718ab8.js",
-            "style": "./style"
-        },
         "extension": true,
         "outputDir": "jupyterlab_pyflyby/labextension",
         "schemaDir": "schema"
     },
     "keywords": [
         "jupyter",
         "jupyterlab",
@@ -63,35 +65,39 @@
     "peerDependencies": {
         "react": "~17.0.1"
     },
     "repository": {
         "type": "git",
         "url": "https://github.com/deshaw/jupyterlab-pyflyby.git"
     },
-    "resolutions": {
-        "@jupyterlab/rendermime-interfaces": "3.6.3"
-    },
     "scripts": {
         "black": "black *.py jupyterlab_pyflyby/**.py",
-        "build": "jlpm run build:lib && jlpm run build:labextension:dev",
-        "build:labextension": "jupyter-labextension build .",
-        "build:labextension:dev": "jupyter-labextension build --development True .",
-        "build:lib": "tsc",
-        "build:prod": "jlpm run clean && jlpm run build:lib && jlpm run build:labextension",
-        "clean": "jlpm run clean:lib",
-        "clean:all": "jlpm run clean:lib && jlpm run clean:labextension",
-        "clean:labextension": "rimraf jupyterlab_pyflyby/labextension",
+        "build": "jlpm build:lib && jlpm build:labextension:dev",
+        "build:labextension": "jupyter labextension build .",
+        "build:labextension:dev": "jupyter labextension build --development True .",
+        "build:lib": "tsc --sourceMap",
+        "build:lib:prod": "tsc",
+        "build:prod": "jlpm clean && jlpm build:lib:prod && jlpm build:labextension",
+        "clean": "jlpm clean:lib",
+        "clean:all": "jlpm clean:lib && jlpm clean:labextension && jlpm clean:lintcache",
+        "clean:labextension": "rimraf jupyterlab_pyflyby/labextension jupyterlab_pyflyby/_version.py",
         "clean:lib": "rimraf lib tsconfig.tsbuildinfo",
-        "eslint": "eslint . --ext .ts,.tsx --fix",
-        "eslint:check": "eslint . --ext .ts,.tsx",
-        "install:extension": "jlpm run build",
-        "lint": "jlpm run black && jlpm run prettier && jlpm run eslint",
-        "prepare": "jlpm run clean && jlpm run build:prod",
-        "prettier": "prettier --write '**/*{.ts,.tsx,.js,.jsx,.css,.json,.md}'",
+        "clean:lintcache": "rimraf .eslintcache .stylelintcache",
+        "eslint": "jlpm eslint:check --fix",
+        "eslint:check": "eslint . --cache --ext .ts,.tsx",
+        "install:extension": "jlpm build",
+        "lint": "jlpm stylelint && jlpm prettier && jlpm eslint",
+        "lint:check": "jlpm stylelint:check && jlpm prettier:check && jlpm eslint:check",
+        "prepare": "jlpm run clean && jlpm run build:prod && husky install",
+        "prettier": "jlpm prettier:base --write --list-different",
+        "prettier:base": "prettier \"**/*{.ts,.tsx,.js,.jsx,.css,.json,.md}\"",
+        "prettier:check": "jlpm prettier:base --check",
+        "stylelint": "jlpm stylelint:check --fix",
+        "stylelint:check": "stylelint --cache \"style/**/*.css\"",
         "watch": "run-p watch:src watch:labextension",
-        "watch:labextension": "jupyter-labextension watch .",
+        "watch:labextension": "jupyter labextension watch .",
         "watch:src": "tsc -w"
     },
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "4.3.0"
+    "version": "5.0.0"
 }
```

### Comparing `jupyterlab_pyflyby-4.3.0/jupyterlab_pyflyby/labextension/schemas/@deshaw/jupyterlab-pyflyby/package.json.orig` & `jupyterlab_pyflyby-5.0.0/jupyterlab_pyflyby/labextension/schemas/@deshaw/jupyterlab-pyflyby/package.json.orig`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8231428659060239%*

 * *Differences: {"'dependencies'": "{'@jupyterlab/application': '^4.0.0', '@jupyterlab/apputils': '^4.0.0', "*

 * *                   "'@jupyterlab/docregistry': '^4.0.0', '@jupyterlab/nbformat': '^4.0.0', "*

 * *                   "'@jupyterlab/notebook': '^4.0.0', '@jupyterlab/services': '^7.0.0', "*

 * *                   "'@jupyterlab/settingregistry': '^4.0.0', '@lumino/algorithm': '^2.0.0', "*

 * *                   "'@lumino/coreutils': '^2.0.0', '@lumino/widgets': '^2.0.1'}",*

 * * "'devDependencies'": "{'@jupyterlab/builder': '^4.0.0', '@ […]*

```diff
@@ -1,51 +1,58 @@
 {
     "bugs": {
         "url": "https://github.com/deshaw/jupyterlab-pyflyby/issues"
     },
     "dependencies": {
-        "@jupyterlab/application": "^3.0.7",
-        "@jupyterlab/apputils": "^3.0.5",
-        "@jupyterlab/docregistry": "^3.0.7",
-        "@jupyterlab/nbformat": "^3.0.3",
-        "@jupyterlab/notebook": "^3.0.7",
-        "@jupyterlab/services": "^6.0.5",
-        "@jupyterlab/settingregistry": "^3.0.3",
-        "@lumino/algorithm": "^1.3.3",
-        "@lumino/coreutils": "^1.5.3",
-        "@lumino/widgets": "^1.16.1",
+        "@jupyterlab/application": "^4.0.0",
+        "@jupyterlab/apputils": "^4.0.0",
+        "@jupyterlab/docregistry": "^4.0.0",
+        "@jupyterlab/nbformat": "^4.0.0",
+        "@jupyterlab/notebook": "^4.0.0",
+        "@jupyterlab/services": "^7.0.0",
+        "@jupyterlab/settingregistry": "^4.0.0",
+        "@lumino/algorithm": "^2.0.0",
+        "@lumino/coreutils": "^2.0.0",
+        "@lumino/widgets": "^2.0.1",
         "debug": "^4.1.1"
     },
     "description": "A labextension to integrate pyflyby with notebooks",
     "devDependencies": {
-        "@jupyterlab/builder": "^3.0.0",
+        "@jupyterlab/builder": "^4.0.0",
         "@types/debug": "^4.1.5",
-        "@typescript-eslint/eslint-plugin": "^4.8.1",
-        "@typescript-eslint/parser": "^4.8.1",
-        "eslint": "^7.14.0",
-        "eslint-config-prettier": "^8.1.0",
-        "eslint-plugin-prettier": "^3.1.4",
-        "husky": "^4.2.3",
+        "@types/json-schema": "^7.0.11",
+        "@types/react": "^18.0.26",
+        "@typescript-eslint/eslint-plugin": "^5.55.0",
+        "@typescript-eslint/parser": "^5.55.0",
+        "css-loader": "^6.7.1",
+        "eslint": "^8.36.0",
+        "eslint-config-prettier": "^8.7.0",
+        "eslint-plugin-prettier": "^4.2.1",
+        "husky": "^8.0.0",
+        "mkdirp": "^1.0.3",
         "npm-run-all": "^4.1.5",
-        "prettier": "^2.2.1",
-        "rimraf": "^3.0.2",
-        "typescript": "~4.1.3"
+        "prettier": "^2.8.7",
+        "rimraf": "^4.4.1",
+        "source-map-loader": "^1.0.2",
+        "style-loader": "^3.3.1",
+        "stylelint": "^14.9.1",
+        "stylelint-config-prettier": "^9.0.4",
+        "stylelint-config-recommended": "^8.0.0",
+        "stylelint-config-standard": "^26.0.0",
+        "stylelint-prettier": "^2.0.0",
+        "typescript": "~5.0.2",
+        "yjs": "^13.5.40"
     },
     "files": [
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "schema/*",
         "style/index.js"
     ],
     "homepage": "https://github.com/deshaw/jupyterlab-pyflyby",
-    "husky": {
-        "hooks": {
-            "pre-commit": "jlpm run lint"
-        }
-    },
     "jupyterlab": {
         "extension": true,
         "outputDir": "jupyterlab_pyflyby/labextension",
         "schemaDir": "schema"
     },
     "keywords": [
         "jupyter",
@@ -58,35 +65,39 @@
     "peerDependencies": {
         "react": "~17.0.1"
     },
     "repository": {
         "type": "git",
         "url": "https://github.com/deshaw/jupyterlab-pyflyby.git"
     },
-    "resolutions": {
-        "@jupyterlab/rendermime-interfaces": "3.6.3"
-    },
     "scripts": {
         "black": "black *.py jupyterlab_pyflyby/**.py",
-        "build": "jlpm run build:lib && jlpm run build:labextension:dev",
-        "build:labextension": "jupyter-labextension build .",
-        "build:labextension:dev": "jupyter-labextension build --development True .",
-        "build:lib": "tsc",
-        "build:prod": "jlpm run clean && jlpm run build:lib && jlpm run build:labextension",
-        "clean": "jlpm run clean:lib",
-        "clean:all": "jlpm run clean:lib && jlpm run clean:labextension",
-        "clean:labextension": "rimraf jupyterlab_pyflyby/labextension",
+        "build": "jlpm build:lib && jlpm build:labextension:dev",
+        "build:labextension": "jupyter labextension build .",
+        "build:labextension:dev": "jupyter labextension build --development True .",
+        "build:lib": "tsc --sourceMap",
+        "build:lib:prod": "tsc",
+        "build:prod": "jlpm clean && jlpm build:lib:prod && jlpm build:labextension",
+        "clean": "jlpm clean:lib",
+        "clean:all": "jlpm clean:lib && jlpm clean:labextension && jlpm clean:lintcache",
+        "clean:labextension": "rimraf jupyterlab_pyflyby/labextension jupyterlab_pyflyby/_version.py",
         "clean:lib": "rimraf lib tsconfig.tsbuildinfo",
-        "eslint": "eslint . --ext .ts,.tsx --fix",
-        "eslint:check": "eslint . --ext .ts,.tsx",
-        "install:extension": "jlpm run build",
-        "lint": "jlpm run black && jlpm run prettier && jlpm run eslint",
-        "prepare": "jlpm run clean && jlpm run build:prod",
-        "prettier": "prettier --write '**/*{.ts,.tsx,.js,.jsx,.css,.json,.md}'",
+        "clean:lintcache": "rimraf .eslintcache .stylelintcache",
+        "eslint": "jlpm eslint:check --fix",
+        "eslint:check": "eslint . --cache --ext .ts,.tsx",
+        "install:extension": "jlpm build",
+        "lint": "jlpm stylelint && jlpm prettier && jlpm eslint",
+        "lint:check": "jlpm stylelint:check && jlpm prettier:check && jlpm eslint:check",
+        "prepare": "jlpm run clean && jlpm run build:prod && husky install",
+        "prettier": "jlpm prettier:base --write --list-different",
+        "prettier:base": "prettier \"**/*{.ts,.tsx,.js,.jsx,.css,.json,.md}\"",
+        "prettier:check": "jlpm prettier:base --check",
+        "stylelint": "jlpm stylelint:check --fix",
+        "stylelint:check": "stylelint --cache \"style/**/*.css\"",
         "watch": "run-p watch:src watch:labextension",
-        "watch:labextension": "jupyter-labextension watch .",
+        "watch:labextension": "jupyter labextension watch .",
         "watch:src": "tsc -w"
     },
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "4.3.0"
+    "version": "5.0.0"
 }
```

### Comparing `jupyterlab_pyflyby-4.3.0/jupyterlab_pyflyby/labextension/schemas/@deshaw/jupyterlab-pyflyby/plugin.json` & `jupyterlab_pyflyby-5.0.0/jupyterlab_pyflyby/labextension/schemas/@deshaw/jupyterlab-pyflyby/plugin.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_pyflyby-4.3.0/jupyterlab_pyflyby/labextension/static/227.d0383463ef62876fb46f.js` & `jupyterlab_pyflyby-5.0.0/jupyterlab_pyflyby/labextension/static/227.d0383463ef62876fb46f.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_pyflyby-4.3.0/jupyterlab_pyflyby/labextension/static/586.e31cbc5a08f78b80f8bc.js` & `jupyterlab_pyflyby-5.0.0/jupyterlab_pyflyby/labextension/static/36.815b80fd2ca5b739309a.js`

 * *Files 26% similar despite different names*

#### js-beautify {}

```diff
@@ -1,429 +1,321 @@
 "use strict";
 (self.webpackChunk_deshaw_jupyterlab_pyflyby = self.webpackChunk_deshaw_jupyterlab_pyflyby || []).push([
-    [586], {
-        586: (t, e, o) => {
-            o.r(e), o.d(e, {
-                default: () => F
+    [36], {
+        36: (e, t, s) => {
+            s.r(t), s.d(t, {
+                default: () => v
             });
-            var s = o(918),
-                n = o(431),
-                i = o(884),
-                r = o(194),
-                l = o(679),
-                a = o(215),
-                c = o(923),
-                d = o(840),
-                h = o(305),
-                m = o(271),
-                u = o.n(m);
-            const y = "pyflyby-cell",
-                g = "# END AUTO-GENERATED BLOCK\n",
-                p = "pyflyby.missing_imports",
-                _ = "pyflyby.format_imports",
-                b = "pyflyby.init_comms",
-                f = "pyflyby.tidy_imports",
-                C = t => "string" == typeof t ? t.split("\n") : t,
-                w = t => !(t.startsWith("#") || t.startsWith('"""') || "" === t.trim() || t.match(/^\s.*$/)) || t.startsWith("%"),
-                x = t => "" === t.trim() || !t.match(/^\s.*$/);
-            var k = o(848),
-                L = o(613);
-            async function S(t = "", e = {}) {
-                const o = L.ServerConnection.makeSettings(),
-                    s = k.URLExt.join(o.baseUrl, "pyflyby", t);
+            var o = s(697),
+                n = s(778),
+                i = s(501),
+                r = s(629),
+                a = s(901),
+                l = s(305),
+                c = s(29),
+                h = s.n(c);
+            const d = "pyflyby-cell",
+                u = "# END AUTO-GENERATED BLOCK\n",
+                m = "pyflyby.missing_imports",
+                y = "pyflyby.format_imports",
+                g = "pyflyby.init_comms",
+                _ = e => "string" == typeof e ? e.split("\n") : e,
+                p = e => !(e.startsWith("#") || e.startsWith('"""') || "" === e.trim() || e.match(/^\s.*$/)) || e.startsWith("%"),
+                f = e => "" === e.trim() || !e.match(/^\s.*$/);
+            var b = s(406),
+                C = s(67);
+            async function w(e = "", t = {}) {
+                const s = C.ServerConnection.makeSettings(),
+                    o = b.URLExt.join(s.baseUrl, "pyflyby", e);
                 let n;
                 try {
-                    n = await L.ServerConnection.makeRequest(s, e, o)
-                } catch (t) {
-                    throw new L.ServerConnection.NetworkError(t)
+                    n = await C.ServerConnection.makeRequest(o, t, s)
+                } catch (e) {
+                    throw new C.ServerConnection.NetworkError(e)
                 }
                 let i = await n.text();
                 if (i.length > 0) try {
                     i = JSON.parse(i)
-                } catch (t) {
+                } catch (e) {
                     console.log("Not a JSON response body.", n)
                 }
-                if (!n.ok) throw new L.ServerConnection.ResponseError(n, i.message || i);
+                if (!n.ok) throw new C.ServerConnection.ResponseError(n, i.message || i);
                 return i
             }
-            const T = (0, h.debug)("PYFLYBY:");
-            class v {
-                constructor(t, e) {
-                    this._lockTimeout = t, this._activeTimeout = null, this.requestedLockCount = 0, this.clearedLockCount = 0, this._releaseLock = {}, this.promise = {
+            const k = (0, l.debug)("PYFLYBY:");
+            class x {
+                constructor(e, t) {
+                    this._recentKernelState = "", this._lockTimeout = e, this._activeTimeout = void 0, this.requestedLockCount = 0, this.clearedLockCount = 0, this._releaseLock = {}, this.promise = {
                         0: Promise.resolve()
-                    }, this._timeoutSignal = new d.Signal(this), this._sessionContext = e, this._sessionContext.statusChanged.connect(this.kernelStateRecorder, this), this._timeoutSignal.connect(this.timeoutExpireHandler, this)
+                    }, this._timeoutSignal = new a.Signal(this), this._sessionContext = t, this._sessionContext.statusChanged.connect(this.kernelStateRecorder, this), this._timeoutSignal.connect(this.timeoutExpireHandler, this)
                 }
-                kernelStateRecorder(t, e) {
-                    this._recentKernelState = e
+                kernelStateRecorder(e, t) {
+                    this._recentKernelState = t
                 }
                 _clearTimeout() {
-                    window.clearTimeout(this._activeTimeout), this._activeTimeout = null
+                    window.clearTimeout(this._activeTimeout), this._activeTimeout = void 0
                 }
-                timeoutExpireHandler(t, e) {
-                    this._clearTimeout(), "busy" === this._recentKernelState ? (console.debug("Extending Timeout For: ", e), this.createTimeout(e)) : this.release(e)
+                timeoutExpireHandler(e, t) {
+                    this._clearTimeout(), "busy" === this._recentKernelState ? (console.debug("Extending Timeout For: ", t), this.createTimeout(t)) : this.release(t)
                 }
                 async acquire() {
-                    const t = this.promise[this.requestedLockCount];
+                    const e = this.promise[this.requestedLockCount];
                     this.requestedLockCount++;
-                    const e = this.requestedLockCount;
-                    return this.promise[e] = new Promise((t => {
-                        this._releaseLock[e] = t
-                    })), await t, new Promise(((t, o) => t(e)))
-                }
-                release(t) {
-                    var e, o;
-                    this.clearedLockCount = t, null === (o = (e = this._releaseLock)[t]) || void 0 === o || o.call(e), delete this._releaseLock[t], this._clearTimeout(), this.clearedLockCount < this.requestedLockCount && this.createTimeout(t + 1)
+                    const t = this.requestedLockCount;
+                    return this.promise[t] = new Promise((e => {
+                        this._releaseLock[t] = e
+                    })), await e, new Promise(((e, s) => e(t)))
+                }
+                release(e) {
+                    var t, s;
+                    this.clearedLockCount = e, null === (s = (t = this._releaseLock)[e]) || void 0 === s || s.call(t), delete this._releaseLock[e], this._clearTimeout(), this.clearedLockCount < this.requestedLockCount && this.createTimeout(e + 1)
                 }
-                createTimeout(t) {
+                createTimeout(e) {
                     this._activeTimeout = setTimeout((() => {
-                        this._timeoutSignal.emit(t)
+                        this._timeoutSignal.emit(e)
                     }), this._lockTimeout)
                 }
             }
-            let Y = !1;
-            class I extends n.Widget {
-                constructor(t, e, o) {
-                    super(), this._context = null, this._sessionContext = null, this._settings = null, this._comms = {}, o.load("@deshaw/jupyterlab-pyflyby:plugin").then((t => {
-                        this._settings = t, (t.get("enabled").user || t.get("enabled").composite) && (this._sessionContext.kernelChanged.connect(this._handleKernelChange, this), this._sessionContext.statusChanged.connect(this._handleKernelStatusChange, this));
-                        const e = 1e3 * (t.get("lockTimeout").user || t.get("lockTimeout").composite);
-                        this._lock = new v(e, this._sessionContext)
-                    }), (t => {
-                        T("PYFLYBY extension has been disabled")
-                    })), this._context = t, this._sessionContext = t.sessionContext
+            let S = !1;
+            class Y extends n.Widget {
+                constructor(e, t, s) {
+                    super(), this._comms = {}, s.load("@deshaw/jupyterlab-pyflyby:plugin").then((e => {
+                        this._settings = e, (e.get("enabled").user || e.get("enabled").composite) && (this._sessionContext.kernelChanged.connect(this._handleKernelChange, this), this._sessionContext.statusChanged.connect(this._handleKernelStatusChange, this));
+                        const t = 1e3 * (e.get("lockTimeout").user || e.get("lockTimeout").composite);
+                        this._lock = new x(t, this._sessionContext)
+                    }), (e => {
+                        k("PYFLYBY extension has been disabled")
+                    })), this._context = e, this._sessionContext = e.sessionContext
                 }
-                async _launchDialog(t) {
-                    const e = new i.Dialog({
+                async _launchDialog(e) {
+                    const t = new i.Dialog({
                         title: "PYFLYBY",
                         body: "PYFLYBY will be adding imports to the first code cell in the notebook.\n            To disable the PYFLYBY extension or to disable this notification in future, go\n            to Settings -> Advanced Settings Editor and choose PYFLYBY preferences tab",
                         buttons: [i.Dialog.okButton()]
                     });
                     try {
-                        return await e.launch(), t
-                    } catch (t) {
-                        console.error(t)
+                        return await t.launch(), e
+                    } catch (e) {
+                        console.error(e)
                     }
                 }
                 _findAndSetImportCoordinates() {
                     const {
-                        model: t
+                        model: e
                     } = this._context;
-                    let e = s.ArrayExt.findFirstIndex((0, s.toArray)(t.cells), ((t, e) => {
-                        const o = t.metadata.get("tags");
-                        return !(!o || -1 === o.indexOf(y))
-                    })); - 1 === e && (e = (t => {
-                        const e = (0, s.toArray)(t);
-                        for (let t = 0; t < e.length; t++) {
-                            const o = e[t];
-                            if ("code" === o.type) {
-                                const e = C(o.toJSON().source);
-                                if (e.length > 0 && !e[0].startsWith("%") && !e[0].startsWith('"""'))
-                                    for (let o = 0; o < e.length; o++)
-                                        if (w(e[o])) return t
+                    let t = o.ArrayExt.findFirstIndex(Array.from(e.cells), ((e, t) => {
+                        const s = e.getMetadata("tags");
+                        return !(!s || -1 === s.indexOf(d))
+                    })); - 1 === t && (t = (e => {
+                        const t = (0, o.toArray)(e);
+                        for (let e = 0; e < t.length; e++) {
+                            const s = t[e];
+                            if ("code" === s.type) {
+                                const t = _(s.toJSON().source);
+                                if (t.length > 0 && !t[0].startsWith("%") && !t[0].startsWith('"""'))
+                                    for (let s = 0; s < t.length; s++)
+                                        if (p(t[s])) return e
                             }
                         }
                         return -1
-                    })((0, s.toArray)(t.cells)));
-                    let o = t.cells.get(e),
-                        n = (t => {
-                            const e = C(t.toJSON().source);
-                            for (let t = e.length - 1; t >= 0; t--)
-                                if (e[t] === g.substr(0, 26)) {
-                                    let o = 0;
-                                    for (let s = 0; s < t - 1; s++) o += e[s].length + 1;
-                                    return o
-                                } for (let t = e.length - 1; t >= 0; t--)
-                                if (o = e[t], w(o) && (o.includes("__future__") || -1 !== o.split(" ").indexOf("import") || o.includes("import_all_names")) && (t === e.length - 1 || x(e[t + 1]))) {
-                                    let o = 0;
-                                    for (let s = 0; s <= t; s++) o += e[s].length + 1;
-                                    return o
-                                } var o;
+                    })(Array.from(e.cells)));
+                    let s = e.cells.get(t).sharedModel,
+                        n = (e => {
+                            const t = _(e.toJSON().source);
+                            for (let e = t.length - 1; e >= 0; e--)
+                                if (t[e] === u.substr(0, 26)) {
+                                    let s = 0;
+                                    for (let o = 0; o < e - 1; o++) s += t[o].length + 1;
+                                    return s
+                                } for (let e = t.length - 1; e >= 0; e--)
+                                if (s = t[e], p(s) && (s.includes("__future__") || -1 !== s.split(" ").indexOf("import") || s.includes("import_all_names")) && (e === t.length - 1 || f(t[e + 1]))) {
+                                    let s = 0;
+                                    for (let o = 0; o <= e; o++) s += t[o].length + 1;
+                                    return s
+                                } var s;
                             return -1
-                        })(t.cells.get(e));
-                    return -1 === n && (o = this._context.model.contentFactory.createCodeCell({
-                        cell: {
-                            source: `# THIS CELL WAS AUTO-GENERATED BY PYFLYBY\n\n\n${g}`,
-                            cell_type: "code",
-                            metadata: {}
-                        }
-                    }), this._context.model.cells.insert(e, o), n = 43), o.metadata.set("tags", [y]), {
-                        cellIndex: e,
+                        })(e.cells.get(t));
+                    return -1 === n && (s = this._context.model.sharedModel.insertCell(0, {
+                        source: `# THIS CELL WAS AUTO-GENERATED BY PYFLYBY\n\n\n${u}`,
+                        cell_type: "code",
+                        metadata: {}
+                    }), n = 43), s.setMetadata("tags", [d]), {
+                        cellIndex: t,
                         position: n
                     }
                 }
-                _insertImport(t) {
-                    let e = null;
-                    return Y || this._settings.get("disableNotification").user ? e = Promise.resolve(t) : (e = this._launchDialog(t), Y = !0), this._findAndSetImportCoordinates(), e
-                }
-                _sendFormatCodeMsg(t, e) {
-                    const o = s.ArrayExt.findFirstIndex((0, s.toArray)(this._context.model.cells), ((t, e) => {
-                        const o = t.metadata.get("tags");
-                        return !(!o || -1 === o.indexOf(y))
+                _insertImport(e) {
+                    let t;
+                    return S || !this._settings || this._settings.get("disableNotification").user ? t = Promise.resolve(e) : (t = this._launchDialog(e), S = !0), this._findAndSetImportCoordinates(), t
+                }
+                _sendFormatCodeMsg(e, t) {
+                    const s = o.ArrayExt.findFirstIndex(Array.from(this._context.model.cells), ((e, t) => {
+                        const s = e.getMetadata("tags");
+                        return !(!s || -1 === s.indexOf(d))
                     }));
-                    if (-1 !== o) {
-                        const s = this._context.model.cells.get(o).toJSON().source,
-                            n = this._comms[_];
+                    if (-1 !== s) {
+                        const o = this._context.model.cells.get(s).toJSON().source,
+                            n = this._comms[y];
                         n && !n.isDisposed && n.send({
-                            msg_id: e,
-                            input_code: s,
-                            imports: t,
-                            type: _
+                            msg_id: t,
+                            input_code: o,
+                            imports: e,
+                            type: y
                         })
                     }
                 }
-                async sendTidyImportRequest() {
-                    const t = this._getCellArray(),
-                        e = this._comms[f];
-                    e && !e.isDisposed && e.send({
-                        type: f,
-                        cellArray: t,
-                        checksum: this._getHashOfCodeInNotebook()
-                    })
-                }
-                _getCellArray() {
-                    const t = this._context.model.cells,
-                        e = [];
-                    for (let o = 0; o < t.length; ++o) e.push({
-                        text: t.get(o).value.text,
-                        type: t.get(o).type
-                    });
-                    return e
-                }
-                restoreNotebookAfterTidyImports(t, e) {
-                    const {
-                        cellIndex: o
-                    } = this._findAndSetImportCoordinates(), s = this._context.model.cells;
-                    for (let e = 0; e < t.length; ++e) {
-                        const o = s.get(e);
-                        o.value.remove(0, o.value.text.length), o.value.insert(0, t[e].text.trim())
-                    }
-                    const n = e.join("\n").trim();
-                    if (0 === s.get(0).value.text.length) s.get(0).value.insert(0, n);
-                    else {
-                        const t = this._context.model.contentFactory.createCodeCell({
-                            cell: {
-                                source: n,
-                                cell_type: "code",
-                                metadata: {
-                                    trusted: !0
-                                }
-                            }
-                        });
-                        s.insert(o, t)
-                    }
-                }
-                _fastStringHash(t) {
-                    let e = 0;
-                    for (let o = 0, s = t.length; o < s; o++) e = (e << 5) - e + t.charCodeAt(o), e |= 0;
-                    return e
-                }
-                _getHashOfCodeInNotebook() {
-                    const t = this._getCellArray();
-                    let e = "";
-                    for (let o = 0; o < t.length; ++o) e += t[o].text;
-                    return this._fastStringHash(e)
-                }
                 _getCommMsgHandler() {
-                    return async t => {
-                        const e = t.content.data;
-                        switch (e.type) {
-                            case p: {
-                                const t = e.missing_imports;
-                                this._insertImport(t).then((async t => {
-                                    const e = await this._lock.acquire();
-                                    this._sendFormatCodeMsg(t, e)
+                    return async e => {
+                        const t = e.content.data;
+                        switch (t.type) {
+                            case m: {
+                                const e = t.missing_imports;
+                                this._insertImport(e).then((async e => {
+                                    if (void 0 !== this._lock) {
+                                        const t = await this._lock.acquire();
+                                        this._sendFormatCodeMsg(e, t)
+                                    }
                                 }));
                                 break
                             }
-                            case _: {
-                                this._formatImports(e);
+                            case y: {
+                                this._formatImports(t);
                                 const {
-                                    msg_id: t
-                                } = e;
-                                this._lock.release(t);
-                                break
-                            }
-                            case b:
-                                this._initializeComms().catch(console.error);
-                                break;
-                            case f: {
-                                const {
-                                    cells: t,
-                                    imports: o,
-                                    checksum: s
-                                } = e;
-                                s === this._getHashOfCodeInNotebook() ? this.restoreNotebookAfterTidyImports(t, o) : await (0, i.showDialog)({
-                                    title: "TidyImports Interrupted",
-                                    body: "TidyImports could not be run because code in the notebook has been changed",
-                                    buttons: [i.Dialog.okButton({
-                                        label: "Ok"
-                                    })],
-                                    defaultButton: 0
-                                });
+                                    msg_id: e
+                                } = t;
+                                void 0 !== this._lock && this._lock.release(e);
                                 break
                             }
+                            case g:
+                                this._initializeComms().catch(console.error)
                         }
                     }
                 }
                 async _initializeComms() {
                     if (!this._sessionContext.session) return;
                     const {
-                        kernel: t
+                        kernel: e
                     } = this._sessionContext.session;
-                    if (!t) return;
-                    const e = p,
-                        o = t.createComm(e);
-                    o.onMsg = this._getCommMsgHandler();
-                    try {
-                        o.open()
-                    } catch (t) {
-                        console.error(`Unable to open PYFLYBY comm - ${t}`)
-                    }
-                    const s = t.createComm(_);
-                    s.onMsg = this._getCommMsgHandler(), s.onClose = t => {
-                        const e = t.content.comm_id;
-                        delete this._comms[e]
-                    }, this._comms[_] = s;
+                    if (!e) return;
+                    const t = m,
+                        s = e.createComm(t);
+                    s.onMsg = this._getCommMsgHandler();
                     try {
                         s.open()
-                    } catch (t) {
-                        console.error(`Unable to open PYFLYBY comm - ${t}`)
+                    } catch (e) {
+                        console.error(`Unable to open PYFLYBY comm - ${e}`)
                     }
-                    const n = t.createComm(f);
-                    n.onMsg = this._getCommMsgHandler(), this._comms[f] = n;
+                    const o = e.createComm(y);
+                    o.onMsg = this._getCommMsgHandler(), o.onClose = e => {
+                        const t = e.content.comm_id;
+                        delete this._comms[t]
+                    }, this._comms[y] = o;
                     try {
-                        n.open()
-                    } catch (t) {
-                        console.error(`Unable to open PYFLYBY comm - ${t}`)
+                        o.open()
+                    } catch (e) {
+                        console.error(`Unable to open PYFLYBY comm - ${e}`)
                     }
-                    return t.registerCommTarget(b, ((t, e) => {
-                        t.onMsg = this._getCommMsgHandler()
+                    return e.registerCommTarget(g, ((e, t) => {
+                        e.onMsg = this._getCommMsgHandler()
                     })), Promise.resolve()
                 }
-                _formatImports(t) {
+                _formatImports(e) {
                     const {
-                        formatted_code: e
-                    } = t, o = s.ArrayExt.findFirstIndex((0, s.toArray)(this._context.model.cells), ((t, e) => {
-                        const o = t.metadata.get("tags");
-                        return !(!o || -1 === o.indexOf(y))
+                        formatted_code: t
+                    } = e, s = o.ArrayExt.findFirstIndex(Array.from(this._context.model.cells), ((e, t) => {
+                        const s = e.getMetadata("tags");
+                        return !(!s || -1 === s.indexOf(d))
                     }));
-                    if (-1 !== o) {
-                        const t = this._context.model.cells.get(o);
-                        t.value.remove(0, t.value.text.length), t.value.insert(0, e)
+                    if (-1 !== s) {
+                        const e = this._context.model.cells.get(s).sharedModel;
+                        e.updateSource(0, e.source.length, t)
                     }
                 }
-                async _handleKernelChange(t, e) {
+                async _handleKernelChange(e, t) {
                     return await this._initializeComms()
                 }
-                _handleKernelStatusChange(t, e) {
-                    return "restarting" === e ? this._initializeComms() : null
+                _handleKernelStatusChange(e, t) {
+                    return "restarting" === t ? this._initializeComms() : null
                 }
             }
             class E {
-                constructor(t) {
-                    this._settingRegistry = null, this._settingRegistry = t, this._loadSettings().catch(console.error)
+                constructor(e) {
+                    this._settingRegistry = e, this._loadSettings().catch(console.error)
                 }
                 async _loadSettings() {
                     try {
-                        await this._settingRegistry.load("@deshaw/jupyterlab-pyflyby:plugin"), T("Successfully loaded PYFLYBY extension settings")
-                    } catch (t) {
+                        await this._settingRegistry.load("@deshaw/jupyterlab-pyflyby:plugin"), k("Successfully loaded PYFLYBY extension settings")
+                    } catch (e) {
                         console.error("Settings could not be loaded")
                     }
                 }
-                createNew(t, e) {
-                    return P = new I(e, t, this._settingRegistry), P
+                createNew(e, t) {
+                    return new Y(t, e, this._settingRegistry)
                 }
             }
-            async function A() {
+            async function T() {
                 try {
-                    await S("install-pyflyby", {
+                    await w("install-pyflyby", {
                         method: "POST"
                     })
-                } catch (t) {
-                    const e = await t.json();
-                    console.error(e.result)
+                } catch (e) {
+                    console.error(e)
                 }
             }
-            const N = u().createElement("div", null, u().createElement("p", null, "To use @deshaw/jupyterlab-pyflyby,", " ", u().createElement("a", {
-                href: "https://github.com/deshaw/pyflyby/blob/master/README.rst",
-                style: {
-                    color: "#0000EE"
-                },
-                target: "_blank",
-                rel: "noopener noreferrer"
-            }, "pyflyby"), " ", "ipython extension needs to be installed."), u().createElement("br", null), u().createElement("p", null, 'Clicking on "Install" will run following command'), u().createElement("div", {
-                style: {
-                    font: "monospace",
-                    color: "#ffffff",
-                    backgroundColor: "#000000",
-                    marginTop: "5px"
-                }
-            }, "$ py pyflyby.install_in_ipython_config_file"), u().createElement("br", null));
-            class D {
-                createNew(t, e) {
-                    const o = new i.ToolbarButton({
-                        className: "tidy-import-button",
-                        tooltip: "Run tidy-imports on this notebook",
-                        icon: B,
-                        onClick: () => P.sendTidyImportRequest()
-                    });
-                    return t.toolbar.insertItem(10, "tidy-imports", o), new c.DisposableDelegate((() => {
-                        o.dispose()
-                    }))
-                }
-            }
-            const B = new a.LabIcon({
-                name: "DJSDocSearch",
-                svgstr: '<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 512 512">\x3c!-- Font Awesome Pro 5.15.4 by @fontawesome - https://fontawesome.com License - https://fontawesome.com/license (Commercial License) --\x3e<path d="M224 96l16-32 32-16-32-16-16-32-16 32-32 16 32 16 16 32zM80 160l26.66-53.33L160 80l-53.34-26.67L80 0 53.34 53.33 0 80l53.34 26.67L80 160zm352 128l-26.66 53.33L352 368l53.34 26.67L432 448l26.66-53.33L512 368l-53.34-26.67L432 288zm70.62-193.77L417.77 9.38C411.53 3.12 403.34 0 395.15 0c-8.19 0-16.38 3.12-22.63 9.38L9.38 372.52c-12.5 12.5-12.5 32.76 0 45.25l84.85 84.85c6.25 6.25 14.44 9.37 22.62 9.37 8.19 0 16.38-3.12 22.63-9.37l363.14-363.15c12.5-12.48 12.5-32.75 0-45.24zM359.45 203.46l-50.91-50.91 86.6-86.6 50.91 50.91-86.6 86.6z"/></svg>'
-            });
-            let P = null;
-            const R = "djs:run-tidy-imports",
-                F = {
+            const L = h().createElement("div", null, h().createElement("p", null, "To use @deshaw/jupyterlab-pyflyby,", " ", h().createElement("a", {
+                    href: "https://github.com/deshaw/pyflyby/blob/master/README.rst",
+                    style: {
+                        color: "#0000EE"
+                    },
+                    target: "_blank",
+                    rel: "noopener noreferrer"
+                }, "pyflyby"), " ", "ipython extension needs to be installed."), h().createElement("br", null), h().createElement("p", null, 'Clicking on "Install" will run following command'), h().createElement("div", {
+                    style: {
+                        font: "monospace",
+                        color: "#ffffff",
+                        backgroundColor: "#000000",
+                        marginTop: "5px"
+                    }
+                }, "$ py pyflyby.install_in_ipython_config_file"), h().createElement("br", null)),
+                v = {
                     id: "@deshaw/jupyterlab-pyflyby:plugin",
                     autoStart: !0,
-                    requires: [r.ISettingRegistry, l.INotebookTracker, i.ICommandPalette],
-                    activate: async function(t, e, o, s) {
-                        console.log("JupyterLab extension @deshaw/jupyterlab-pyflyby is activated!"), t.commands.addCommand(R, {
-                            execute: () => P.sendTidyImportRequest(),
-                            icon: B,
-                            label: "Run tidy-imports on Notebook"
-                        }), s.addItem({
-                            command: R,
-                            category: "Notebook"
-                        });
-                        const n = await e.load("@deshaw/jupyterlab-pyflyby:plugin"),
-                            r = n.get("enabled").user || n.get("enabled").composite,
-                            l = n.get("installDialogDisplayed").user;
-                        r && "loaded" !== await async function() {
-                            return (await S("pyflyby-status")).status
-                        }() && (l || (await (0, i.showDialog)({
+                    requires: [r.ISettingRegistry],
+                    activate: async function(e, t) {
+                        console.log("JupyterLab extension @deshaw/jupyterlab-pyflyby is activated!");
+                        const s = await t.load("@deshaw/jupyterlab-pyflyby:plugin"),
+                            o = s.get("enabled").user || s.get("enabled").composite,
+                            n = s.get("installDialogDisplayed").user;
+                        o && "loaded" !== await async function() {
+                            return (await w("pyflyby-status")).status
+                        }() && (n || (await (0, i.showDialog)({
                             title: "Installation required",
-                            body: N,
+                            body: L,
                             buttons: [i.Dialog.okButton({
                                 label: "Install"
                             }), i.Dialog.cancelButton({
                                 label: "Cancel",
                                 displayType: "default"
                             })],
                             defaultButton: 0
-                        })).button.accept ? await A() : await async function(t) {
+                        })).button.accept ? await T() : await async function(e) {
                             try {
-                                await S("disable-pyflyby", {
+                                await w("disable-pyflyby", {
                                     method: "POST",
                                     mode: "cors",
                                     cache: "no-cache",
                                     credentials: "include",
                                     headers: {
                                         "Content-type": "application/x-www-form-urlencoded"
                                     },
                                     body: new URLSearchParams("installDialogDisplayed=true")
                                 })
-                            } catch (t) {
-                                const e = await t.json();
-                                console.error(e.result)
+                            } catch (e) {
+                                console.error(e)
                             }
-                            await t.reload("@deshaw/jupyterlab-pyflyby:plugin")
-                        }(e)), t.docRegistry.addWidgetExtension("Notebook", new E(e)), t.docRegistry.addWidgetExtension("Notebook", new D)
+                            await e.reload("@deshaw/jupyterlab-pyflyby:plugin")
+                        }(t)), e.docRegistry.addWidgetExtension("Notebook", new E(t))
                     }
                 }
         }
     }
 ]);
```

### Comparing `jupyterlab_pyflyby-4.3.0/jupyterlab_pyflyby/labextension/static/remoteEntry.d287a35fa86eaa718ab8.js` & `jupyterlab_pyflyby-5.0.0/jupyterlab_pyflyby/labextension/static/remoteEntry.2f3f2d893fd3c5c9aea1.js`

 * *Files 12% similar despite different names*

#### js-beautify {}

```diff
@@ -1,15 +1,15 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, a, o, i, u, l, f, s, d, p, c, h, v, y, b, g, m = {
-            603: (e, r, t) => {
+    var e, r, t, n, a, o, i, u, l, d, s, f, p, c, h, v, y, b, g, m = {
+            556: (e, r, t) => {
                 var n = {
-                        "./index": () => t.e(586).then((() => () => t(586))),
-                        "./extension": () => t.e(586).then((() => () => t(586))),
+                        "./index": () => t.e(36).then((() => () => t(36))),
+                        "./extension": () => t.e(36).then((() => () => t(36))),
                         "./style": () => t.e(747).then((() => () => t(747)))
                     },
                     a = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
                     })), t.R = void 0, r),
                     o = (e, r) => {
                         if (t.S) {
@@ -43,51 +43,51 @@
         }), r
     }, j.d = (e, r) => {
         for (var t in r) j.o(r, t) && !j.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, j.f = {}, j.e = e => Promise.all(Object.keys(j.f).reduce(((r, t) => (j.f[t](e, r), r)), [])), j.u = e => e + "." + {
+        36: "815b80fd2ca5b739309a",
         227: "d0383463ef62876fb46f",
-        586: "e31cbc5a08f78b80f8bc",
-        747: "895f1f90006f2cd62bc9"
+        747: "642119a933d152ff1ed4"
     } [e] + ".js?v=" + {
+        36: "815b80fd2ca5b739309a",
         227: "d0383463ef62876fb46f",
-        586: "e31cbc5a08f78b80f8bc",
-        747: "895f1f90006f2cd62bc9"
+        747: "642119a933d152ff1ed4"
     } [e], j.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
     }(), j.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "@deshaw/jupyterlab-pyflyby:", j.l = (t, n, a, o) => {
         if (e[t]) e[t].push(n);
         else {
             var i, u;
             if (void 0 !== a)
-                for (var l = document.getElementsByTagName("script"), f = 0; f < l.length; f++) {
-                    var s = l[f];
+                for (var l = document.getElementsByTagName("script"), d = 0; d < l.length; d++) {
+                    var s = l[d];
                     if (s.getAttribute("src") == t || s.getAttribute("data-webpack") == r + a) {
                         i = s;
                         break
                     }
                 }
             i || (u = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, j.nc && i.setAttribute("nonce", j.nc), i.setAttribute("data-webpack", r + a), i.src = t), e[t] = [n];
-            var d = (r, n) => {
+            var f = (r, n) => {
                     i.onerror = i.onload = null, clearTimeout(p);
                     var a = e[t];
                     if (delete e[t], i.parentNode && i.parentNode.removeChild(i), a && a.forEach((e => e(n))), r) return r(n)
                 },
-                p = setTimeout(d.bind(null, void 0, {
+                p = setTimeout(f.bind(null, void 0, {
                     type: "timeout",
                     target: i
                 }), 12e4);
-            i.onerror = d.bind(null, i.onerror), i.onload = d.bind(null, i.onload), u && document.head.appendChild(i)
+            i.onerror = f.bind(null, i.onerror), i.onload = f.bind(null, i.onload), u && document.head.appendChild(i)
         }
     }, j.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
@@ -109,15 +109,15 @@
                         (!u || !u.loaded && (!n != !u.eager ? n : i > u.from)) && (a[r] = {
                             get: t,
                             from: i,
                             eager: !!n
                         })
                     },
                     l = [];
-                return "default" === t && (u("@deshaw/jupyterlab-pyflyby", "4.3.0", (() => j.e(586).then((() => () => j(586))))), u("debug", "4.3.4", (() => j.e(227).then((() => () => j(227)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
+                return "default" === t && (u("@deshaw/jupyterlab-pyflyby", "5.0.0", (() => j.e(36).then((() => () => j(36))))), u("debug", "4.3.4", (() => j.e(227).then((() => () => j(227)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         j.g.importScripts && (e = j.g.location + "");
         var r = j.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -167,33 +167,33 @@
     }, o = (e, r) => {
         if (0 in e) {
             r = t(r);
             var n = e[0],
                 a = n < 0;
             a && (n = -n - 1);
             for (var i = 0, u = 1, l = !0;; u++, i++) {
-                var f, s, d = u < e.length ? (typeof e[u])[0] : "";
-                if (i >= r.length || "o" == (s = (typeof(f = r[i]))[0])) return !l || ("u" == d ? u > n && !a : "" == d != a);
+                var d, s, f = u < e.length ? (typeof e[u])[0] : "";
+                if (i >= r.length || "o" == (s = (typeof(d = r[i]))[0])) return !l || ("u" == f ? u > n && !a : "" == f != a);
                 if ("u" == s) {
-                    if (!l || "u" != d) return !1
+                    if (!l || "u" != f) return !1
                 } else if (l)
-                    if (d == s)
+                    if (f == s)
                         if (u <= n) {
-                            if (f != e[u]) return !1
+                            if (d != e[u]) return !1
                         } else {
-                            if (a ? f > e[u] : f < e[u]) return !1;
-                            f != e[u] && (l = !1)
+                            if (a ? d > e[u] : d < e[u]) return !1;
+                            d != e[u] && (l = !1)
                         }
-                else if ("s" != d && "n" != d) {
+                else if ("s" != f && "n" != f) {
                     if (a || u <= n) return !1;
                     l = !1, u--
                 } else {
-                    if (u <= n || s < d != a) return !1;
+                    if (u <= n || s < f != a) return !1;
                     l = !1
-                } else "s" != d && "n" != d && (l = !1, u--)
+                } else "s" != f && "n" != f && (l = !1, u--)
             }
         }
         var p = [],
             c = p.pop.bind(p);
         for (i = 1; i < e.length; i++) {
             var h = e[i];
             p.push(1 == h ? c() | c() : 2 == h ? c() & c() : h ? o(h, r) : !c())
@@ -202,43 +202,40 @@
     }, i = (e, r) => {
         var t = j.S[e];
         if (!t || !j.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, u = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
-    }, l = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + a(n) + ")", f = (e, r, t, n) => {
+    }, l = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + a(n) + ")", d = (e, r, t, n) => {
         var a = u(e, t);
-        return o(n, a) || d(l(e, t, a, n)), p(e[t][a])
+        return o(n, a) || f(l(e, t, a, n)), p(e[t][a])
     }, s = (e, r, t) => {
         var a = e[r];
         return (r = Object.keys(a).reduce(((e, r) => !o(t, r) || e && !n(e, r) ? e : r), 0)) && a[r]
-    }, d = e => {
+    }, f = e => {
         "undefined" != typeof console && console.warn && console.warn(e)
     }, p = e => (e.loaded = 1, e.get()), h = (c = e => function(r, t, n, a) {
         var o = j.I(r);
         return o && o.then ? o.then(e.bind(e, r, j.S[r], t, n, a)) : e(r, j.S[r], t, n, a)
-    })(((e, r, t, n) => (i(e, t), f(r, 0, t, n)))), v = c(((e, r, t, n, a) => {
+    })(((e, r, t, n) => (i(e, t), d(r, 0, t, n)))), v = c(((e, r, t, n, a) => {
         var o = r && j.o(r, t) && s(r, t, n);
         return o ? p(o) : a()
     })), y = {}, b = {
-        194: () => h("default", "@jupyterlab/settingregistry", [1, 3, 6, 2]),
-        215: () => h("default", "@jupyterlab/ui-components", [1, 3, 6, 2]),
-        271: () => h("default", "react", [1, 17, 0, 1]),
+        29: () => h("default", "react", [1, 18, 2, 0]),
+        67: () => h("default", "@jupyterlab/services", [1, 7, 0, 0]),
         305: () => v("default", "debug", [1, 4, 1, 1], (() => j.e(227).then((() => () => j(227))))),
-        431: () => h("default", "@lumino/widgets", [1, 1, 37, 1]),
-        613: () => h("default", "@jupyterlab/services", [1, 6, 6, 2]),
-        679: () => h("default", "@jupyterlab/notebook", [1, 3, 6, 2]),
-        840: () => h("default", "@lumino/signaling", [1, 1, 10, 0]),
-        848: () => h("default", "@jupyterlab/coreutils", [1, 5, 6, 2]),
-        884: () => h("default", "@jupyterlab/apputils", [1, 3, 6, 2]),
-        918: () => h("default", "@lumino/algorithm", [1, 1, 9, 0]),
-        923: () => h("default", "@lumino/disposable", [1, 1, 10, 0])
+        406: () => h("default", "@jupyterlab/coreutils", [1, 6, 0, 0]),
+        501: () => h("default", "@jupyterlab/apputils", [1, 4, 0, 0]),
+        629: () => h("default", "@jupyterlab/settingregistry", [1, 4, 0, 0]),
+        697: () => h("default", "@lumino/algorithm", [1, 2, 0, 0]),
+        778: () => h("default", "@lumino/widgets", [1, 2, 0, 1]),
+        901: () => h("default", "@lumino/signaling", [1, 2, 0, 0])
     }, g = {
-        586: [194, 215, 271, 305, 431, 613, 679, 840, 848, 884, 918, 923]
+        36: [29, 67, 305, 406, 501, 629, 697, 778, 901]
     }, j.f.consumes = (e, r) => {
         j.o(g, e) && g[e].forEach((e => {
             if (j.o(y, e)) return r.push(y[e]);
             var t = r => {
                     y[e] = 0, j.m[e] = t => {
                         delete j.c[e], t.exports = r()
                     }
@@ -285,10 +282,10 @@
                     u && u(j)
                 }
                 for (r && r(t); l < o.length; l++) a = o[l], j.o(e, a) && e[a] && e[a][0](), e[a] = 0
             },
             t = self.webpackChunk_deshaw_jupyterlab_pyflyby = self.webpackChunk_deshaw_jupyterlab_pyflyby || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
     })(), j.nc = void 0;
-    var S = j(603);
+    var S = j(556);
     (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB)["@deshaw/jupyterlab-pyflyby"] = S
 })();
```

### Comparing `jupyterlab_pyflyby-4.3.0/jupyterlab_pyflyby/labextension/static/third-party-licenses.json` & `jupyterlab_pyflyby-5.0.0/jupyterlab_pyflyby/labextension/static/third-party-licenses.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.975%*

 * *Differences: {"'packages'": "{0: {'versionInfo': '6.7.4'}, 4: {'versionInfo': '3.3.3'}}"}*

```diff
@@ -1,14 +1,14 @@
 {
     "packages": [
         {
             "extractedText": "Copyright JS Foundation and other contributors\n\nPermission is hereby granted, free of charge, to any person obtaining\na copy of this software and associated documentation files (the\n'Software'), to deal in the Software without restriction, including\nwithout limitation the rights to use, copy, modify, merge, publish,\ndistribute, sublicense, and/or sell copies of the Software, and to\npermit persons to whom the Software is furnished to do so, subject to\nthe following conditions:\n\nThe above copyright notice and this permission notice shall be\nincluded in all copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED 'AS IS', WITHOUT WARRANTY OF ANY KIND,\nEXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF\nMERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.\nIN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY\nCLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,\nTORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE\nSOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.\n",
             "licenseId": "MIT",
             "name": "css-loader",
-            "versionInfo": "5.2.7"
+            "versionInfo": "6.7.4"
         },
         {
             "extractedText": "(The MIT License)\n\nCopyright (c) 2014-2017 TJ Holowaychuk <tj@vision-media.ca>\nCopyright (c) 2018-2021 Josh Junon\n\nPermission is hereby granted, free of charge, to any person obtaining a copy of this software\nand associated documentation files (the 'Software'), to deal in the Software without restriction,\nincluding without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense,\nand/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so,\nsubject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in all copies or substantial\nportions of the Software.\n\nTHE SOFTWARE IS PROVIDED 'AS IS', WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT\nLIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.\nIN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY,\nWHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE\nSOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.\n\n",
             "licenseId": "MIT",
             "name": "debug",
             "versionInfo": "4.3.4"
         },
@@ -24,11 +24,11 @@
             "name": "process",
             "versionInfo": "0.11.10"
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

### Comparing `jupyterlab_pyflyby-4.3.0/package.json` & `jupyterlab_pyflyby-5.0.0/jupyterlab_pyflyby/labextension/package.json`

 * *Files 23% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8165639185376028%*

 * *Differences: {"'dependencies'": "{'@jupyterlab/application': '^4.0.0', '@jupyterlab/apputils': '^4.0.0', "*

 * *                   "'@jupyterlab/docregistry': '^4.0.0', '@jupyterlab/nbformat': '^4.0.0', "*

 * *                   "'@jupyterlab/notebook': '^4.0.0', '@jupyterlab/services': '^7.0.0', "*

 * *                   "'@jupyterlab/settingregistry': '^4.0.0', '@lumino/algorithm': '^2.0.0', "*

 * *                   "'@lumino/coreutils': '^2.0.0', '@lumino/widgets': '^2.0.1'}",*

 * * "'devDependencies'": "{'@jupyterlab/builder': '^4.0.0', '@ […]*

```diff
@@ -1,52 +1,64 @@
 {
     "bugs": {
         "url": "https://github.com/deshaw/jupyterlab-pyflyby/issues"
     },
     "dependencies": {
-        "@jupyterlab/application": "^3.0.7",
-        "@jupyterlab/apputils": "^3.0.5",
-        "@jupyterlab/docregistry": "^3.0.7",
-        "@jupyterlab/nbformat": "^3.0.3",
-        "@jupyterlab/notebook": "^3.0.7",
-        "@jupyterlab/services": "^6.0.5",
-        "@jupyterlab/settingregistry": "^3.0.3",
-        "@lumino/algorithm": "^1.3.3",
-        "@lumino/coreutils": "^1.5.3",
-        "@lumino/widgets": "^1.16.1",
+        "@jupyterlab/application": "^4.0.0",
+        "@jupyterlab/apputils": "^4.0.0",
+        "@jupyterlab/docregistry": "^4.0.0",
+        "@jupyterlab/nbformat": "^4.0.0",
+        "@jupyterlab/notebook": "^4.0.0",
+        "@jupyterlab/services": "^7.0.0",
+        "@jupyterlab/settingregistry": "^4.0.0",
+        "@lumino/algorithm": "^2.0.0",
+        "@lumino/coreutils": "^2.0.0",
+        "@lumino/widgets": "^2.0.1",
         "debug": "^4.1.1"
     },
     "description": "A labextension to integrate pyflyby with notebooks",
     "devDependencies": {
-        "@jupyterlab/builder": "^3.0.0",
+        "@jupyterlab/builder": "^4.0.0",
         "@types/debug": "^4.1.5",
-        "@typescript-eslint/eslint-plugin": "^4.8.1",
-        "@typescript-eslint/parser": "^4.8.1",
-        "eslint": "^7.14.0",
-        "eslint-config-prettier": "^8.1.0",
-        "eslint-plugin-prettier": "^3.1.4",
-        "husky": "^4.2.3",
+        "@types/json-schema": "^7.0.11",
+        "@types/react": "^18.0.26",
+        "@typescript-eslint/eslint-plugin": "^5.55.0",
+        "@typescript-eslint/parser": "^5.55.0",
+        "css-loader": "^6.7.1",
+        "eslint": "^8.36.0",
+        "eslint-config-prettier": "^8.7.0",
+        "eslint-plugin-prettier": "^4.2.1",
+        "husky": "^8.0.0",
+        "mkdirp": "^1.0.3",
         "npm-run-all": "^4.1.5",
-        "prettier": "^2.2.1",
-        "rimraf": "^3.0.2",
-        "typescript": "~4.1.3"
+        "prettier": "^2.8.7",
+        "rimraf": "^4.4.1",
+        "source-map-loader": "^1.0.2",
+        "style-loader": "^3.3.1",
+        "stylelint": "^14.9.1",
+        "stylelint-config-prettier": "^9.0.4",
+        "stylelint-config-recommended": "^8.0.0",
+        "stylelint-config-standard": "^26.0.0",
+        "stylelint-prettier": "^2.0.0",
+        "typescript": "~5.0.2",
+        "yjs": "^13.5.40"
     },
     "files": [
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "schema/*",
         "style/index.js"
     ],
     "homepage": "https://github.com/deshaw/jupyterlab-pyflyby",
-    "husky": {
-        "hooks": {
-            "pre-commit": "jlpm run lint"
-        }
-    },
     "jupyterlab": {
+        "_build": {
+            "extension": "./extension",
+            "load": "static/remoteEntry.2f3f2d893fd3c5c9aea1.js",
+            "style": "./style"
+        },
         "extension": true,
         "outputDir": "jupyterlab_pyflyby/labextension",
         "schemaDir": "schema"
     },
     "keywords": [
         "jupyter",
         "jupyterlab",
@@ -58,35 +70,39 @@
     "peerDependencies": {
         "react": "~17.0.1"
     },
     "repository": {
         "type": "git",
         "url": "https://github.com/deshaw/jupyterlab-pyflyby.git"
     },
-    "resolutions": {
-        "@jupyterlab/rendermime-interfaces": "3.6.3"
-    },
     "scripts": {
         "black": "black *.py jupyterlab_pyflyby/**.py",
-        "build": "jlpm run build:lib && jlpm run build:labextension:dev",
-        "build:labextension": "jupyter-labextension build .",
-        "build:labextension:dev": "jupyter-labextension build --development True .",
-        "build:lib": "tsc",
-        "build:prod": "jlpm run clean && jlpm run build:lib && jlpm run build:labextension",
-        "clean": "jlpm run clean:lib",
-        "clean:all": "jlpm run clean:lib && jlpm run clean:labextension",
-        "clean:labextension": "rimraf jupyterlab_pyflyby/labextension",
+        "build": "jlpm build:lib && jlpm build:labextension:dev",
+        "build:labextension": "jupyter labextension build .",
+        "build:labextension:dev": "jupyter labextension build --development True .",
+        "build:lib": "tsc --sourceMap",
+        "build:lib:prod": "tsc",
+        "build:prod": "jlpm clean && jlpm build:lib:prod && jlpm build:labextension",
+        "clean": "jlpm clean:lib",
+        "clean:all": "jlpm clean:lib && jlpm clean:labextension && jlpm clean:lintcache",
+        "clean:labextension": "rimraf jupyterlab_pyflyby/labextension jupyterlab_pyflyby/_version.py",
         "clean:lib": "rimraf lib tsconfig.tsbuildinfo",
-        "eslint": "eslint . --ext .ts,.tsx --fix",
-        "eslint:check": "eslint . --ext .ts,.tsx",
-        "install:extension": "jlpm run build",
-        "lint": "jlpm run black && jlpm run prettier && jlpm run eslint",
-        "prepare": "jlpm run clean && jlpm run build:prod",
-        "prettier": "prettier --write '**/*{.ts,.tsx,.js,.jsx,.css,.json,.md}'",
+        "clean:lintcache": "rimraf .eslintcache .stylelintcache",
+        "eslint": "jlpm eslint:check --fix",
+        "eslint:check": "eslint . --cache --ext .ts,.tsx",
+        "install:extension": "jlpm build",
+        "lint": "jlpm stylelint && jlpm prettier && jlpm eslint",
+        "lint:check": "jlpm stylelint:check && jlpm prettier:check && jlpm eslint:check",
+        "prepare": "jlpm run clean && jlpm run build:prod && husky install",
+        "prettier": "jlpm prettier:base --write --list-different",
+        "prettier:base": "prettier \"**/*{.ts,.tsx,.js,.jsx,.css,.json,.md}\"",
+        "prettier:check": "jlpm prettier:base --check",
+        "stylelint": "jlpm stylelint:check --fix",
+        "stylelint:check": "stylelint --cache \"style/**/*.css\"",
         "watch": "run-p watch:src watch:labextension",
-        "watch:labextension": "jupyter-labextension watch .",
+        "watch:labextension": "jupyter labextension watch .",
         "watch:src": "tsc -w"
     },
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "4.3.0"
+    "version": "5.0.0"
 }
```

### Comparing `jupyterlab_pyflyby-4.3.0/src/cellUtils.ts` & `jupyterlab_pyflyby-5.0.0/src/cellUtils.ts`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import { toArray } from '@lumino/algorithm';
+
 import { MultilineString } from '@jupyterlab/nbformat';
 import { ICellModel } from '@jupyterlab/cells';
 import { PYFLYBY_END_MSG } from './constants';
 
 // FIXME: There's got to be a better Typescript solution
 // for distinguishing between members of a union type at runtime.
 export const normalizeMultilineString = (source: MultilineString): string[] => {
```

### Comparing `jupyterlab_pyflyby-4.3.0/src/handler.ts` & `jupyterlab_pyflyby-5.0.0/src/handler.ts`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     endPoint
   );
 
   let response: Response;
   try {
     response = await ServerConnection.makeRequest(requestUrl, init, settings);
   } catch (error) {
-    throw new ServerConnection.NetworkError(error);
+    throw new ServerConnection.NetworkError(error as any);
   }
 
   let data: any = await response.text();
 
   if (data.length > 0) {
     try {
       data = JSON.parse(data);
```

### Comparing `jupyterlab_pyflyby-4.3.0/src/index.tsx` & `jupyterlab_pyflyby-5.0.0/src/index.tsx`

 * *Files 14% similar despite different names*

```diff
@@ -14,37 +14,32 @@
  * 1. If PYFLYBY_END_MSG is present, import is added above it.
  * 2. Added import after last import statement in code cell. Identifying import statement is
  *    is done by simple heuristics. This step can be shifted to pyflyby where python parser can be used to
  *    determine it accurately.
  */
 
 // Lumino imports
-import { toArray, ArrayExt } from '@lumino/algorithm';
+import { ArrayExt } from '@lumino/algorithm';
 import { JSONValue, JSONObject } from '@lumino/coreutils';
 import { Widget, Panel } from '@lumino/widgets';
 
 // Jupyterlab imports
-import { JupyterFrontEnd } from '@jupyterlab/application';
+import {
+  JupyterFrontEnd,
+  JupyterFrontEndPlugin
+} from '@jupyterlab/application';
 import { Dialog, ISessionContext, showDialog } from '@jupyterlab/apputils';
 import { ICellModel } from '@jupyterlab/cells';
+import { ISharedCell } from '@jupyter/ydoc';
 import { ISettingRegistry } from '@jupyterlab/settingregistry';
 import { DocumentRegistry } from '@jupyterlab/docregistry';
-import {
-  INotebookModel,
-  INotebookTracker,
-  NotebookPanel
-} from '@jupyterlab/notebook';
-import { LabIcon } from '@jupyterlab/ui-components';
-import { ICommandPalette, ToolbarButton } from '@jupyterlab/apputils';
-import { DisposableDelegate, IDisposable } from '@lumino/disposable';
+import { INotebookModel } from '@jupyterlab/notebook';
 import { Session, Kernel, KernelMessage } from '@jupyterlab/services';
 import { Signal } from '@lumino/signaling';
-// eslint-disable-next-line @typescript-eslint/ban-ts-comment
-// @ts-ignore
-import tidyImportSVG from '../style/tidy-import.svg';
+
 import { debug } from 'debug';
 import React from 'react';
 
 // relative imports
 import { findCell, findLinePos } from './cellUtils';
 import {
   PYFLYBY_CELL_TAG,
@@ -57,47 +52,47 @@
 const log = debug('PYFLYBY:');
 
 class CommLock {
   _releaseLock: any;
   promise: any;
   requestedLockCount: number;
   clearedLockCount: number;
-  _activeTimeout: number;
+  _activeTimeout: number | undefined;
   _lockTimeout: number;
   _timeoutSignal: Signal<CommLock, number>;
-  _recentKernelState: string;
+  _recentKernelState = '';
   _sessionContext: ISessionContext;
 
   constructor(_lockTimeout: number, sessionContext: ISessionContext) {
     this._lockTimeout = _lockTimeout;
-    this._activeTimeout = null;
+    this._activeTimeout = undefined;
     this.requestedLockCount = 0;
     this.clearedLockCount = 0;
     this._releaseLock = {};
     this.promise = { 0: Promise.resolve() };
     this._timeoutSignal = new Signal<CommLock, number>(this);
     this._sessionContext = sessionContext;
     this._sessionContext.statusChanged.connect(this.kernelStateRecorder, this);
     this._timeoutSignal.connect(this.timeoutExpireHandler, this);
   }
 
-  kernelStateRecorder(sender: ISessionContext, args: Kernel.Status) {
+  kernelStateRecorder(_sender: ISessionContext, args: Kernel.Status) {
     this._recentKernelState = args;
   }
 
   _clearTimeout() {
     window.clearTimeout(this._activeTimeout);
-    this._activeTimeout = null;
+    this._activeTimeout = undefined;
   }
 
   /*
-    If the kernel was busy the last time, we assume it was busy executing 
+    If the kernel was busy the last time, we assume it was busy executing
     code and we restart the timeout.
   */
-  timeoutExpireHandler(sender: CommLock, id: number) {
+  timeoutExpireHandler(_sender: CommLock, id: number) {
     this._clearTimeout();
     if (this._recentKernelState === 'busy') {
       console.debug('Extending Timeout For: ', id);
       this.createTimeout(id);
     } else {
       this.release(id);
     }
@@ -107,15 +102,15 @@
     const lastLockPromise = this.promise[this.requestedLockCount];
     this.requestedLockCount++;
     const lockId = this.requestedLockCount;
     this.promise[lockId] = new Promise(resolve => {
       this._releaseLock[lockId] = resolve;
     });
     await lastLockPromise;
-    return new Promise((res, rej) => res(lockId));
+    return new Promise((res, _rej) => res(lockId));
   }
 
   release(lockId: number): void {
     this.clearedLockCount = lockId;
     this._releaseLock[lockId]?.();
     delete this._releaseLock[lockId];
     this._clearTimeout();
@@ -134,18 +129,18 @@
 // We'd like to show the notification only once per session, not for each notebook
 let _userWasNotified = false;
 
 /**
  * An extension that adds pyflyby integration to a single notebook widget
  */
 class PyflyByWidget extends Widget {
-  _lock: CommLock;
+  _lock: CommLock | undefined;
   constructor(
     context: DocumentRegistry.IContext<INotebookModel>,
-    panel: Panel,
+    _panel: Panel,
     settingRegistry: ISettingRegistry
   ) {
     super();
     // get a reference to the settings registry
     settingRegistry.load('@deshaw/jupyterlab-pyflyby:plugin').then(
       (settings: ISettingRegistry.ISettings) => {
         this._settings = settings;
@@ -164,15 +159,15 @@
 
         const _lockTimeout =
           1000 *
           ((settings.get('lockTimeout').user ||
             settings.get('lockTimeout').composite) as number);
         this._lock = new CommLock(_lockTimeout, this._sessionContext);
       },
-      (err: any) => {
+      (_err: any) => {
         log('PYFLYBY extension has been disabled');
       }
     );
     this._context = context;
     this._sessionContext = context.sessionContext;
   }
 
@@ -191,80 +186,79 @@
       await dialog.launch();
       return imports;
     } catch (e) {
       console.error(e);
     }
   }
 
-  /**
-   * All the logic related to finding the right cell
-   */
+  // /**
+  //  * All the logic related to finding the right cell
+  //  */
   _findAndSetImportCoordinates() {
     const { model } = this._context;
     let pyflybyCellIndex = ArrayExt.findFirstIndex(
-      toArray(model.cells),
-      (cell: ICellModel, index: number) => {
-        const tags = cell.metadata.get('tags') as string[];
+      Array.from(model.cells),
+      (cell: ICellModel, _index: number) => {
+        const tags = cell.getMetadata('tags') as string[];
         return !!(tags && tags.indexOf(PYFLYBY_CELL_TAG) !== -1);
       }
     );
 
     /**
      * Since the cell doesn't exist, we make one or, if the first
      * code cell contains an import block, put it below that.
      */
     if (pyflybyCellIndex === -1) {
-      pyflybyCellIndex = findCell(toArray(model.cells));
+      pyflybyCellIndex = findCell(Array.from(model.cells));
     }
 
-    let cell = model.cells.get(pyflybyCellIndex);
-
+    let cell = model.cells.get(pyflybyCellIndex).sharedModel;
     let position = findLinePos(model.cells.get(pyflybyCellIndex));
 
     if (position === -1) {
-      cell = this._context.model.contentFactory.createCodeCell({
-        cell: {
-          source: `${PYFLYBY_START_MSG}\n\n${PYFLYBY_END_MSG}`,
-          cell_type: 'code',
-          metadata: {}
-        }
+      cell = this._context.model.sharedModel.insertCell(0, {
+        source: `${PYFLYBY_START_MSG}\n\n${PYFLYBY_END_MSG}`,
+        cell_type: 'code',
+        metadata: {}
       });
-
-      this._context.model.cells.insert(pyflybyCellIndex, cell);
       position = PYFLYBY_START_MSG.length + 1;
     }
-    cell.metadata.set('tags', [PYFLYBY_CELL_TAG]);
+    cell.setMetadata('tags', [PYFLYBY_CELL_TAG]);
     return { cellIndex: pyflybyCellIndex, position };
   }
 
   /**
    * Adds the import block to the appropriate cell at the appropriate
    * location.
    *
    * @param importBlock - the import statement or block of import statements
    */
   _insertImport(imports: any) {
-    let p: Promise<any> = null;
-    if (!_userWasNotified && !this._settings.get('disableNotification').user) {
+    let p: Promise<any>;
+    if (
+      !_userWasNotified &&
+      this._settings &&
+      !this._settings.get('disableNotification').user
+    ) {
       p = this._launchDialog(imports);
       _userWasNotified = true;
     } else {
       p = Promise.resolve(imports);
     }
 
     // creates the cell for imports
     this._findAndSetImportCoordinates();
     return p;
   }
 
   _sendFormatCodeMsg(imports: any, lockId: number) {
     const pyflybyCellIndex = ArrayExt.findFirstIndex(
-      toArray(this._context.model.cells),
-      (cell: ICellModel, index: number) => {
-        const tags = cell.metadata.get('tags') as string[];
+      Array.from(this._context.model.cells),
+      (cell: ICellModel, _index: number) => {
+        const tags = cell.getMetadata('tags') as string[];
         return !!(tags && tags.indexOf(PYFLYBY_CELL_TAG) !== -1);
       }
     );
     if (pyflybyCellIndex !== -1) {
       const cellSource = this._context.model.cells
         .get(pyflybyCellIndex)
         .toJSON().source;
@@ -276,125 +270,41 @@
           imports: imports,
           type: PYFLYBY_COMMS.FORMAT_IMPORTS
         });
       }
     }
   }
 
-  async sendTidyImportRequest(): Promise<any> {
-    const cellArray = this._getCellArray();
-    const comm = this._comms[PYFLYBY_COMMS.TIDY_IMPORTS];
-    if (comm && !comm.isDisposed) {
-      comm.send({
-        type: PYFLYBY_COMMS.TIDY_IMPORTS,
-        cellArray: cellArray,
-        checksum: this._getHashOfCodeInNotebook()
-      });
-    }
-  }
-
-  _getCellArray() {
-    const cells = this._context.model.cells;
-    const cellArray = [];
-
-    for (let i = 0; i < cells.length; ++i) {
-      cellArray.push({
-        text: cells.get(i).value.text,
-        type: cells.get(i).type
-      });
-    }
-
-    return cellArray;
-  }
-
-  restoreNotebookAfterTidyImports(cellArray: any, imports: any): void {
-    const { cellIndex } = this._findAndSetImportCoordinates();
-    const cells = this._context.model.cells;
-    for (let i = 0; i < cellArray.length; ++i) {
-      const cell = cells.get(i);
-      cell.value.remove(0, cell.value.text.length);
-      cell.value.insert(0, cellArray[i].text.trim());
-    }
-    const joined_imports = imports.join('\n').trim();
-    if (cells.get(0).value.text.length === 0) {
-      cells.get(0).value.insert(0, joined_imports);
-    } else {
-      const cell = this._context.model.contentFactory.createCodeCell({
-        cell: {
-          source: joined_imports,
-          cell_type: 'code',
-          metadata: {
-            trusted: true
-          }
-        }
-      });
-      cells.insert(cellIndex, cell);
-    }
-  }
-
-  _fastStringHash(str: string) {
-    let hash = 0;
-    for (let i = 0, len = str.length; i < len; i++) {
-      const chr = str.charCodeAt(i);
-      hash = (hash << 5) - hash + chr;
-      hash |= 0; // Convert to 32bit integer
-    }
-    return hash;
-  }
-
-  _getHashOfCodeInNotebook() {
-    const cellArray = this._getCellArray();
-    let joinedText = '';
-    for (let i = 0; i < cellArray.length; ++i) {
-      joinedText = joinedText + cellArray[i].text;
-    }
-    return this._fastStringHash(joinedText);
-  }
-
   _getCommMsgHandler() {
     return async (msg: KernelMessage.ICommMsgMsg) => {
       const msgContent: JSONValue = msg.content.data;
       switch ((msgContent as JSONObject).type) {
         case PYFLYBY_COMMS.MISSING_IMPORTS: {
           const itd = msgContent['missing_imports'];
           this._insertImport(itd).then(async imports => {
             // Acquire new lock but wait for previous lock to expire
-            const currentLockId = await this._lock.acquire();
-            this._sendFormatCodeMsg(imports, currentLockId);
+            if (this._lock !== undefined) {
+              const currentLockId = await this._lock.acquire();
+              this._sendFormatCodeMsg(imports, currentLockId);
+            }
           });
           break;
         }
         case PYFLYBY_COMMS.FORMAT_IMPORTS: {
           this._formatImports(msgContent);
           const { msg_id: lockId }: any = msgContent;
-          this._lock.release(lockId);
+          if (this._lock !== undefined) {
+            this._lock.release(lockId);
+          }
           break;
         }
         case PYFLYBY_COMMS.INIT: {
           this._initializeComms().catch(console.error);
           break;
         }
-        case PYFLYBY_COMMS.TIDY_IMPORTS: {
-          const { cells, imports, checksum } = msgContent;
-          if (checksum === this._getHashOfCodeInNotebook()) {
-            this.restoreNotebookAfterTidyImports(cells, imports);
-          } else {
-            await showDialog({
-              title: 'TidyImports Interrupted',
-              body: 'TidyImports could not be run because code in the notebook has been changed',
-              buttons: [
-                Dialog.okButton({
-                  label: 'Ok'
-                })
-              ],
-              defaultButton: 0
-            });
-          }
-          break;
-        }
         default:
           break;
       }
     };
   }
 
   async _initializeComms() {
@@ -424,68 +334,60 @@
     this._comms[PYFLYBY_COMMS.FORMAT_IMPORTS] = formatMsgComm;
     try {
       formatMsgComm.open();
     } catch (e) {
       console.error(`Unable to open PYFLYBY comm - ${e}`);
     }
 
-    const tidyImportsComm = kernel.createComm(PYFLYBY_COMMS.TIDY_IMPORTS);
-    tidyImportsComm.onMsg = this._getCommMsgHandler();
-    this._comms[PYFLYBY_COMMS.TIDY_IMPORTS] = tidyImportsComm;
-    try {
-      tidyImportsComm.open();
-    } catch (e) {
-      console.error(`Unable to open PYFLYBY comm - ${e}`);
-    }
     kernel.registerCommTarget(
       PYFLYBY_COMMS.INIT,
-      (comm, msg: KernelMessage.ICommOpenMsg) => {
+      (comm, _msg: KernelMessage.ICommOpenMsg) => {
         comm.onMsg = this._getCommMsgHandler();
       }
     );
 
     return Promise.resolve();
   }
 
   _formatImports(msgData: any) {
     const { formatted_code: formattedCode } = msgData;
     const pyflybyCellIndex = ArrayExt.findFirstIndex(
-      toArray(this._context.model.cells),
-      (cell: ICellModel, index: number) => {
-        const tags = cell.metadata.get('tags') as string[];
+      Array.from(this._context.model.cells),
+      (cell: ICellModel, _index: number) => {
+        const tags = cell.getMetadata('tags') as string[];
         return !!(tags && tags.indexOf(PYFLYBY_CELL_TAG) !== -1);
       }
     );
     if (pyflybyCellIndex !== -1) {
-      const cell: ICellModel = this._context.model.cells.get(pyflybyCellIndex);
-      cell.value.remove(0, cell.value.text.length);
-      cell.value.insert(0, formattedCode);
+      const cell: ISharedCell =
+        this._context.model.cells.get(pyflybyCellIndex).sharedModel;
+      cell.updateSource(0, cell.source.length, formattedCode);
     }
   }
 
   async _handleKernelChange(
-    sender: ISessionContext,
-    kernelChangedArgs: Session.ISessionConnection.IKernelChangedArgs
+    _sender: ISessionContext,
+    _kernelChangedArgs: Session.ISessionConnection.IKernelChangedArgs
   ): Promise<any> {
     return await this._initializeComms();
   }
 
   _handleKernelStatusChange(
-    sender: ISessionContext,
+    _sender: ISessionContext,
     args: Kernel.Status
   ): Promise<any> | null {
     if (args === 'restarting') {
       return this._initializeComms();
     }
     return null;
   }
 
-  private _context: DocumentRegistry.IContext<INotebookModel> = null;
-  private _sessionContext: ISessionContext = null;
-  private _settings: ISettingRegistry.ISettings = null;
+  private _context: DocumentRegistry.IContext<INotebookModel>;
+  private _sessionContext: ISessionContext;
+  private _settings: ISettingRegistry.ISettings | undefined;
   private _comms: any = {};
 }
 
 /**
  * An extension that adds pyflyby integration to a notebook widget
  */
 class PyflyByWidgetExtension implements DocumentRegistry.WidgetExtension {
@@ -503,48 +405,45 @@
       log('Successfully loaded PYFLYBY extension settings');
     } catch (e) {
       console.error('Settings could not be loaded');
     }
   }
 
   createNew(panel: Panel, context: DocumentRegistry.IContext<INotebookModel>) {
-    pyflybyWidget = new PyflyByWidget(context, panel, this._settingRegistry);
-    return pyflybyWidget;
+    return new PyflyByWidget(context, panel, this._settingRegistry);
   }
 
-  private _settingRegistry: ISettingRegistry = null;
+  private _settingRegistry: ISettingRegistry;
 }
 
 async function isPyflybyInstalled() {
   const pyflybyStatus = await requestAPI<any>('pyflyby-status');
   return pyflybyStatus.status;
 }
 
 async function installPyflyby() {
   try {
     await requestAPI<any>('install-pyflyby', { method: 'POST' });
   } catch (err) {
-    const errMsg = await err.json();
-    console.error(errMsg.result);
+    console.error(err);
   }
 }
 
 async function disableJupyterlabPyflyby(registry: ISettingRegistry) {
   try {
     await requestAPI<any>('disable-pyflyby', {
       method: 'POST',
       mode: 'cors',
       cache: 'no-cache',
       credentials: 'include',
       headers: { 'Content-type': 'application/x-www-form-urlencoded' },
       body: new URLSearchParams('installDialogDisplayed=true')
     });
   } catch (err) {
-    const errMsg = await err.json();
-    console.error(errMsg.result);
+    console.error(err);
   }
   await registry.reload('@deshaw/jupyterlab-pyflyby:plugin');
 }
 
 const installationBody = (
   <div>
     <p>
@@ -571,69 +470,26 @@
     >
       $ py pyflyby.install_in_ipython_config_file
     </div>
     <br />
   </div>
 );
 
-class TidyImportButtonExtension
-  implements DocumentRegistry.IWidgetExtension<NotebookPanel, INotebookModel>
-{
-  createNew(
-    widget: NotebookPanel,
-    context: DocumentRegistry.IContext<INotebookModel>
-  ): IDisposable {
-    const button = new ToolbarButton({
-      className: 'tidy-import-button',
-      tooltip: 'Run tidy-imports on this notebook',
-      icon: TidyImportsIcon,
-      onClick: () => pyflybyWidget.sendTidyImportRequest()
-    });
-
-    widget.toolbar.insertItem(10, 'tidy-imports', button);
-    return new DisposableDelegate(() => {
-      button.dispose();
-    });
-  }
-}
-
-const TidyImportsIcon = new LabIcon({
-  name: 'DJSDocSearch',
-  svgstr: tidyImportSVG
-});
-
-let pyflybyWidget: any = null;
-
-const djsTidyImportsCommand = 'djs:run-tidy-imports';
-
-const extension = {
+const extension: JupyterFrontEndPlugin<void> = {
   id: '@deshaw/jupyterlab-pyflyby:plugin',
   autoStart: true,
-  requires: [ISettingRegistry, INotebookTracker, ICommandPalette],
+  requires: [ISettingRegistry],
   activate: async function (
     app: JupyterFrontEnd,
-    registry: ISettingRegistry,
-    tracker: INotebookTracker,
-    palette: ICommandPalette
+    registry: ISettingRegistry
   ): Promise<void> {
     console.log(
       'JupyterLab extension @deshaw/jupyterlab-pyflyby is activated!'
     );
 
-    app.commands.addCommand(djsTidyImportsCommand, {
-      execute: () => pyflybyWidget.sendTidyImportRequest(),
-      icon: TidyImportsIcon,
-      label: 'Run tidy-imports on Notebook'
-    });
-
-    palette.addItem({
-      command: djsTidyImportsCommand,
-      category: 'Notebook'
-    });
-
     const settings = await registry.load('@deshaw/jupyterlab-pyflyby:plugin');
     const enabled =
       settings.get('enabled').user || settings.get('enabled').composite;
     const dialogDisplayedEarlier = settings.get('installDialogDisplayed').user;
 
     if (enabled) {
       const response = await isPyflybyInstalled();
@@ -662,16 +518,11 @@
       }
     }
 
     app.docRegistry.addWidgetExtension(
       'Notebook',
       new PyflyByWidgetExtension(registry)
     );
-
-    app.docRegistry.addWidgetExtension(
-      'Notebook',
-      new TidyImportButtonExtension()
-    );
   }
 };
 
 export default extension;
```

### Comparing `jupyterlab_pyflyby-4.3.0/tsconfig.json` & `jupyterlab_pyflyby-5.0.0/tsconfig.json`

 * *Files 19% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9868421052631579%*

 * *Differences: {"'compilerOptions'": "{'strictNullChecks': True, 'target': 'ES2018'}"}*

```diff
@@ -12,15 +12,15 @@
         "noImplicitAny": true,
         "noUnusedLocals": true,
         "outDir": "lib",
         "preserveWatchOutput": true,
         "resolveJsonModule": true,
         "rootDir": "src",
         "strict": true,
-        "strictNullChecks": false,
-        "target": "es2018",
+        "strictNullChecks": true,
+        "target": "ES2018",
         "types": []
     },
     "include": [
         "src/*"
     ]
 }
```

