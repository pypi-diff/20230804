# Comparing `tmp/jupyterlab_vim-4.0.1.tar.gz` & `tmp/jupyterlab_vim-4.0.2.tar.gz`

## Comparing `jupyterlab_vim-4.0.1.tar` & `jupyterlab_vim-4.0.2.tar`

### file list

```diff
@@ -1,36 +1,35 @@
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.1/.eslintignore
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.1/.prettierignore
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.1/.prettierrc
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.1/.yarnrc.yml
--rw-r--r--   0        0        0     7179 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.1/CHANGELOG.md
--rw-r--r--   0        0        0     3923 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.1/RELEASE.md
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.1/install.json
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.1/installing.md
--rw-r--r--   0        0        0     2584 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.1/modify-keybinds.md
--rw-r--r--   0        0        0     6647 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.1/package.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.1/setup.py
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.1/tsconfig.json
--rw-r--r--   0        0        0   212877 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.1/yarn.lock
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.1/jupyterlab_vim/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.1/jupyterlab_vim/_version.py
--rw-r--r--   0        0        0     5921 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.1/jupyterlab_vim/labextension/package.json
--rw-r--r--   0        0        0     6647 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.1/jupyterlab_vim/labextension/schemas/@axlair/jupyterlab_vim/package.json.orig
--rw-r--r--   0        0        0    10856 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.1/jupyterlab_vim/labextension/schemas/@axlair/jupyterlab_vim/plugin.json
--rw-r--r--   0        0        0   130333 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.1/jupyterlab_vim/labextension/static/252.e0500116419ca3a355d1.js
--rw-r--r--   0        0        0    10218 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.1/jupyterlab_vim/labextension/static/353.9c6b79c5ee878d215a0a.js
--rw-r--r--   0        0        0     4399 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.1/jupyterlab_vim/labextension/static/747.a573445024188eae7034.js
--rw-r--r--   0        0        0     7577 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.1/jupyterlab_vim/labextension/static/remoteEntry.ddb05f98b2e0f61dea44.js
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.1/jupyterlab_vim/labextension/static/style.js
--rw-r--r--   0        0        0     7505 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.1/jupyterlab_vim/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0    10856 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.1/schema/plugin.json
--rw-r--r--   0        0        0    11871 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.1/src/codemirrorCommands.ts
--rw-r--r--   0        0        0     6297 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.1/src/index.ts
--rw-r--r--   0        0        0     8187 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.1/src/labCommands.ts
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.1/style/base.css
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.1/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.1/style/index.js
--rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.1/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.1/LICENSE
--rw-r--r--   0        0        0     6383 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.1/README.md
--rw-r--r--   0        0        0     2321 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.1/pyproject.toml
--rw-r--r--   0        0        0     8705 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.1/PKG-INFO
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.2/.eslintignore
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.2/.prettierignore
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.2/.yarnrc.yml
+-rw-r--r--   0        0        0     9051 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.2/CHANGELOG.md
+-rw-r--r--   0        0        0     3923 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.2/RELEASE.md
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.2/install.json
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.2/installing.md
+-rw-r--r--   0        0        0     2584 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.2/modify-keybinds.md
+-rw-r--r--   0        0        0     6831 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.2/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.2/setup.py
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.2/tsconfig.json
+-rw-r--r--   0        0        0   212877 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.2/yarn.lock
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.2/jupyterlab_vim/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.2/jupyterlab_vim/_version.py
+-rw-r--r--   0        0        0     6051 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.2/jupyterlab_vim/labextension/package.json
+-rw-r--r--   0        0        0     6831 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.2/jupyterlab_vim/labextension/schemas/@axlair/jupyterlab_vim/package.json.orig
+-rw-r--r--   0        0        0    10974 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.2/jupyterlab_vim/labextension/schemas/@axlair/jupyterlab_vim/plugin.json
+-rw-r--r--   0        0        0   130333 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.2/jupyterlab_vim/labextension/static/252.e0500116419ca3a355d1.js
+-rw-r--r--   0        0        0    10310 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.2/jupyterlab_vim/labextension/static/353.23043df9052364040d09.js
+-rw-r--r--   0        0        0     4399 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.2/jupyterlab_vim/labextension/static/747.a573445024188eae7034.js
+-rw-r--r--   0        0        0     7575 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.2/jupyterlab_vim/labextension/static/remoteEntry.63ac9819dfe44854c8f6.js
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.2/jupyterlab_vim/labextension/static/style.js
+-rw-r--r--   0        0        0     7505 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.2/jupyterlab_vim/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0    10974 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.2/schema/plugin.json
+-rw-r--r--   0        0        0    11871 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.2/src/codemirrorCommands.ts
+-rw-r--r--   0        0        0     6297 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.2/src/index.ts
+-rw-r--r--   0        0        0     8382 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.2/src/labCommands.ts
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.2/style/base.css
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.2/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.2/style/index.js
+-rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.2/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.2/LICENSE
+-rw-r--r--   0        0        0     6383 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.2/README.md
+-rw-r--r--   0        0        0     2321 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.2/pyproject.toml
+-rw-r--r--   0        0        0     8705 2020-02-02 00:00:00.000000 jupyterlab_vim-4.0.2/PKG-INFO
```

### Comparing `jupyterlab_vim-4.0.1/CHANGELOG.md` & `jupyterlab_vim-4.0.2/CHANGELOG.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,37 @@
 # Changelog
 
 <!-- <START NEW CHANGELOG ENTRY> -->
 
+## 4.0.2
+
+([Full Changelog](https://github.com/jupyterlab-contrib/jupyterlab-vim/compare/v4.0.1...929b801ab0e3df63d24f277630c2d3ab6d3be146))
+
+### Enhancements made
+
+- Clear input state if applicable before hopping out of normal mode to jupyter command mode [#82](https://github.com/jupyterlab-contrib/jupyterlab-vim/pull/82) ([@ryantam626](https://github.com/ryantam626))
+
+### Bugs fixed
+
+- fix: override browser shift-esc in command mode [#100](https://github.com/jupyterlab-contrib/jupyterlab-vim/pull/100) ([@ianhi](https://github.com/ianhi))
+  - Additional thanks to [@petergthatsme](https://github.com/petergthatsme) [@firai](https://github.com/firai) [@lukashergt](https://github.com/lukashergt) for reporting, debugging and testing
+- Fix __init__.py for wheel [#99](https://github.com/jupyterlab-contrib/jupyterlab-vim/pull/99) ([@fcollonval](https://github.com/fcollonval))
+
+### Maintenance and upkeep improvements
+
+- fix: dev install + lint issues [#97](https://github.com/jupyterlab-contrib/jupyterlab-vim/pull/97) ([@ianhi](https://github.com/ianhi))
+
+### Contributors to this release
+
+([GitHub contributors page for this release](https://github.com/jupyterlab-contrib/jupyterlab-vim/graphs/contributors?from=2023-08-01&to=2023-08-03&type=c))
+
+[@fcollonval](https://github.com/search?q=repo%3Ajupyterlab-contrib%2Fjupyterlab-vim+involves%3Afcollonval+updated%3A2023-08-01..2023-08-03&type=Issues) | [@github-actions](https://github.com/search?q=repo%3Ajupyterlab-contrib%2Fjupyterlab-vim+involves%3Agithub-actions+updated%3A2023-08-01..2023-08-03&type=Issues) | [@ianhi](https://github.com/search?q=repo%3Ajupyterlab-contrib%2Fjupyterlab-vim+involves%3Aianhi+updated%3A2023-08-01..2023-08-03&type=Issues) | [@ryantam626](https://github.com/search?q=repo%3Ajupyterlab-contrib%2Fjupyterlab-vim+involves%3Aryantam626+updated%3A2023-08-01..2023-08-03&type=Issues)
+
+<!-- <END NEW CHANGELOG ENTRY> -->
+
 ## 4.0.1
 
 ([Full Changelog](https://github.com/jupyterlab-contrib/jupyterlab-vim/compare/v4.0.0...9aa55aad927c578d91e51f351bb5bcf987d03c46))
 
 ### Enhancements made
 
 - build: don't require package.json for python import [#93](https://github.com/jupyterlab-contrib/jupyterlab-vim/pull/93) ([@ianhi](https://github.com/ianhi))
@@ -21,16 +47,14 @@
 
 ### Contributors to this release
 
 ([GitHub contributors page for this release](https://github.com/jupyterlab-contrib/jupyterlab-vim/graphs/contributors?from=2023-07-31&to=2023-08-01&type=c))
 
 [@github-actions](https://github.com/search?q=repo%3Ajupyterlab-contrib%2Fjupyterlab-vim+involves%3Agithub-actions+updated%3A2023-07-31..2023-08-01&type=Issues) | [@ianhi](https://github.com/search?q=repo%3Ajupyterlab-contrib%2Fjupyterlab-vim+involves%3Aianhi+updated%3A2023-07-31..2023-08-01&type=Issues) | [@krassowski](https://github.com/search?q=repo%3Ajupyterlab-contrib%2Fjupyterlab-vim+involves%3Akrassowski+updated%3A2023-07-31..2023-08-01&type=Issues)
 
-<!-- <END NEW CHANGELOG ENTRY> -->
-
 ## 4.0.0
 
 ([Full Changelog](https://github.com/jupyterlab-contrib/jupyterlab-vim/compare/1.1.0...718d294cbbab1010ffaf35c79773e3abc5d98a6c))
 
 ### Enhancements made
 
 - Add support for vim mode in Text Editor [#90](https://github.com/jupyterlab-contrib/jupyterlab-vim/pull/90) ([@krassowski](https://github.com/krassowski))
```

### Comparing `jupyterlab_vim-4.0.1/RELEASE.md` & `jupyterlab_vim-4.0.2/RELEASE.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_vim-4.0.1/modify-keybinds.md` & `jupyterlab_vim-4.0.2/modify-keybinds.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_vim-4.0.1/package.json` & `jupyterlab_vim-4.0.2/package.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.975%*

 * *Differences: {"'prettier'": "{'overrides': [OrderedDict([('files', 'package.json'), ('options', "*

 * *               "OrderedDict([('tabWidth', 4)]))])]}",*

 * * "'version'": "'4.0.2'"}*

```diff
@@ -131,14 +131,22 @@
     ],
     "license": "MIT",
     "main": "lib/index.js",
     "name": "@axlair/jupyterlab_vim",
     "prettier": {
         "arrowParens": "avoid",
         "endOfLine": "auto",
+        "overrides": [
+            {
+                "files": "package.json",
+                "options": {
+                    "tabWidth": 4
+                }
+            }
+        ],
         "singleQuote": true,
         "trailingComma": "none"
     },
     "publishConfig": {
         "access": "public"
     },
     "repository": {
@@ -187,9 +195,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "4.0.1"
+    "version": "4.0.2"
 }
```

### Comparing `jupyterlab_vim-4.0.1/tsconfig.json` & `jupyterlab_vim-4.0.2/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_vim-4.0.1/yarn.lock` & `jupyterlab_vim-4.0.2/yarn.lock`

 * *Files identical despite different names*

### Comparing `jupyterlab_vim-4.0.1/jupyterlab_vim/labextension/package.json` & `jupyterlab_vim-4.0.2/jupyterlab_vim/labextension/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9745659722222221%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.63ac9819dfe44854c8f6.js'}}",*

 * * "'prettier'": "{'overrides': [OrderedDict([('files', 'package.json'), ('options', "*

 * *               "OrderedDict([('tabWidth', 4)]))])]}",*

 * * "'version'": "'4.0.2'"}*

```diff
@@ -117,15 +117,15 @@
         "schema/**/*.{json,}",
         "style/index.js"
     ],
     "homepage": "https://github.com/jupyterlab-contrib/jupyterlab-vim",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.ddb05f98b2e0f61dea44.js",
+            "load": "static/remoteEntry.63ac9819dfe44854c8f6.js",
             "style": "./style"
         },
         "extension": true,
         "outputDir": "jupyterlab_vim/labextension",
         "schemaDir": "schema"
     },
     "keywords": [
@@ -136,14 +136,22 @@
     ],
     "license": "MIT",
     "main": "lib/index.js",
     "name": "@axlair/jupyterlab_vim",
     "prettier": {
         "arrowParens": "avoid",
         "endOfLine": "auto",
+        "overrides": [
+            {
+                "files": "package.json",
+                "options": {
+                    "tabWidth": 4
+                }
+            }
+        ],
         "singleQuote": true,
         "trailingComma": "none"
     },
     "publishConfig": {
         "access": "public"
     },
     "repository": {
@@ -192,9 +200,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "4.0.1"
+    "version": "4.0.2"
 }
```

### Comparing `jupyterlab_vim-4.0.1/jupyterlab_vim/labextension/schemas/@axlair/jupyterlab_vim/package.json.orig` & `jupyterlab_vim-4.0.2/jupyterlab_vim/labextension/schemas/@axlair/jupyterlab_vim/package.json.orig`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.975%*

 * *Differences: {"'prettier'": "{'overrides': [OrderedDict([('files', 'package.json'), ('options', "*

 * *               "OrderedDict([('tabWidth', 4)]))])]}",*

 * * "'version'": "'4.0.2'"}*

```diff
@@ -131,14 +131,22 @@
     ],
     "license": "MIT",
     "main": "lib/index.js",
     "name": "@axlair/jupyterlab_vim",
     "prettier": {
         "arrowParens": "avoid",
         "endOfLine": "auto",
+        "overrides": [
+            {
+                "files": "package.json",
+                "options": {
+                    "tabWidth": 4
+                }
+            }
+        ],
         "singleQuote": true,
         "trailingComma": "none"
     },
     "publishConfig": {
         "access": "public"
     },
     "repository": {
@@ -187,9 +195,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "4.0.1"
+    "version": "4.0.2"
 }
```

### Comparing `jupyterlab_vim-4.0.1/jupyterlab_vim/labextension/schemas/@axlair/jupyterlab_vim/plugin.json` & `jupyterlab_vim-4.0.2/jupyterlab_vim/labextension/schemas/@axlair/jupyterlab_vim/plugin.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9987745098039216%*

 * *Differences: {"'jupyter.lab.shortcuts'": "{insert: [(26, OrderedDict([('selector', "*

 * *                            "'.jp-Notebook.jp-mod-commandMode'), ('keys', ['Shift Escape']), "*

 * *                            "('command', '')]))]}"}*

```diff
@@ -256,14 +256,21 @@
             "command": "notebook:enter-command-mode",
             "keys": [
                 "Shift Escape"
             ],
             "selector": ".jp-NotebookPanel[data-jp-vim-mode='true'] .jp-Notebook.jp-mod-editMode"
         },
         {
+            "command": "",
+            "keys": [
+                "Shift Escape"
+            ],
+            "selector": ".jp-Notebook.jp-mod-commandMode"
+        },
+        {
             "command": "vim:merge-and-edit",
             "keys": [
                 "Shift M"
             ],
             "selector": ".jp-NotebookPanel[data-jp-vim-mode='true'] .jp-Notebook:focus"
         },
         {
```

### Comparing `jupyterlab_vim-4.0.1/jupyterlab_vim/labextension/static/252.e0500116419ca3a355d1.js` & `jupyterlab_vim-4.0.2/jupyterlab_vim/labextension/static/252.e0500116419ca3a355d1.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_vim-4.0.1/jupyterlab_vim/labextension/static/353.9c6b79c5ee878d215a0a.js` & `jupyterlab_vim-4.0.2/jupyterlab_vim/labextension/static/353.23043df9052364040d09.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,18 +1,18 @@
 "use strict";
 (self.webpackChunk_axlair_jupyterlab_vim = self.webpackChunk_axlair_jupyterlab_vim || []).push([
     [353], {
         353: (e, t, o) => {
             o.r(t), o.d(t, {
                 default: () => p
             });
-            var n = o(861),
-                i = o(785),
-                l = o(408),
-                d = o(663),
+            var n = o(543),
+                i = o(41),
+                l = o(745),
+                d = o(200),
                 a = o(829),
                 c = o(211),
                 s = o(204);
             class r {
                 constructor({
                     enabled: e,
                     userKeybindings: t
@@ -358,15 +358,15 @@
                                             content: e
                                         } = t;
                                         if (null !== e.activeCell) {
                                             const t = e.activeCell.editor,
                                                 n = (0, a.getCM)(t.editor);
                                             if (!n) return void console.error("CodeMirror vim wrapper not found");
                                             const i = n.state.vim;
-                                            i.insertMode || i.visualMode ? a.Vim.handleKey(n, "<Esc>") : o.execute("notebook:enter-command-mode")
+                                            i.insertMode || i.visualMode || null !== i.inputState.operator || null !== i.inputState.motion || 0 !== i.inputState.keyBuffer.length ? a.Vim.handleKey(n, "<Esc>") : o.execute("notebook:enter-command-mode")
                                         }
                                     }
                                 },
                                 isEnabled: d
                             }), o.addCommand("vim:select-below-execute-markdown", {
                                 label: "Execute Markdown and Select Cell Below",
                                 execute: e => {
```

### Comparing `jupyterlab_vim-4.0.1/jupyterlab_vim/labextension/static/747.a573445024188eae7034.js` & `jupyterlab_vim-4.0.2/jupyterlab_vim/labextension/static/747.a573445024188eae7034.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_vim-4.0.1/jupyterlab_vim/labextension/static/remoteEntry.ddb05f98b2e0f61dea44.js` & `jupyterlab_vim-4.0.2/jupyterlab_vim/labextension/static/remoteEntry.63ac9819dfe44854c8f6.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,12 +1,12 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
     var e, r, t, a, o, n, i, l, u, d, f, s, c, p, h, v, m, b, g, y = {
-            130: (e, r, t) => {
+            678: (e, r, t) => {
                 var a = {
                         "./index": () => Promise.all([t.e(598), t.e(353)]).then((() => () => t(353))),
                         "./extension": () => Promise.all([t.e(598), t.e(353)]).then((() => () => t(353))),
                         "./style": () => t.e(747).then((() => () => t(747)))
                     },
                     o = (e, r) => (t.R = r, r = t.o(a, e) ? a[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
@@ -44,21 +44,21 @@
     }, j.d = (e, r) => {
         for (var t in r) j.o(r, t) && !j.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, j.f = {}, j.e = e => Promise.all(Object.keys(j.f).reduce(((r, t) => (j.f[t](e, r), r)), [])), j.u = e => e + "." + {
         252: "e0500116419ca3a355d1",
-        353: "9c6b79c5ee878d215a0a",
+        353: "23043df9052364040d09",
         598: "ad606b2bbb9816d73182",
         747: "a573445024188eae7034",
         818: "53acaa7ded124a9243cd"
     } [e] + ".js?v=" + {
         252: "e0500116419ca3a355d1",
-        353: "9c6b79c5ee878d215a0a",
+        353: "23043df9052364040d09",
         598: "ad606b2bbb9816d73182",
         747: "a573445024188eae7034",
         818: "53acaa7ded124a9243cd"
     } [e], j.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
@@ -113,15 +113,15 @@
                         (!l || !l.loaded && (!a != !l.eager ? a : i > l.from)) && (o[r] = {
                             get: t,
                             from: i,
                             eager: !!a
                         })
                     },
                     u = [];
-                return "default" === t && (l("@axlair/jupyterlab_vim", "4.0.1", (() => Promise.all([j.e(598), j.e(353)]).then((() => () => j(353))))), l("@replit/codemirror-vim", "6.0.14", (() => Promise.all([j.e(252), j.e(598), j.e(818)]).then((() => () => j(252)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                return "default" === t && (l("@axlair/jupyterlab_vim", "4.0.2", (() => Promise.all([j.e(598), j.e(353)]).then((() => () => j(353))))), l("@replit/codemirror-vim", "6.0.14", (() => Promise.all([j.e(252), j.e(598), j.e(818)]).then((() => () => j(252)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         j.g.importScripts && (e = j.g.location + "");
         var r = j.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -223,24 +223,24 @@
         return n && n.then ? n.then(e.bind(e, r, j.S[r], t, a, o)) : e(r, j.S[r], t, a, o)
     })(((e, r, t, a) => (i(e, t), d(r, 0, t, a)))), v = p(((e, r, t, a, o) => {
         var n = r && j.o(r, t) && f(r, t, a);
         return n ? c(n) : o()
     })), m = {}, b = {
         204: () => h("default", "@codemirror/state", [1, 6, 2, 0]),
         211: () => h("default", "@codemirror/view", [1, 6, 9, 6]),
-        408: () => h("default", "@jupyterlab/codemirror", [1, 4, 0, 3]),
+        41: () => h("default", "@jupyterlab/fileeditor", [1, 4, 0, 4]),
+        200: () => h("default", "@jupyterlab/settingregistry", [1, 4, 0, 4]),
+        543: () => h("default", "@jupyterlab/notebook", [1, 4, 0, 4]),
         593: () => h("default", "@lumino/domutils", [1, 2, 0, 0]),
-        663: () => h("default", "@jupyterlab/settingregistry", [1, 4, 0, 3]),
-        785: () => h("default", "@jupyterlab/fileeditor", [1, 4, 0, 3]),
+        745: () => h("default", "@jupyterlab/codemirror", [1, 4, 0, 4]),
         829: () => v("default", "@replit/codemirror-vim", [1, 6, 0, 14], (() => Promise.all([j.e(252), j.e(818)]).then((() => () => j(252))))),
-        861: () => h("default", "@jupyterlab/notebook", [1, 4, 0, 3]),
         373: () => h("default", "@codemirror/language", [1, 6, 0, 0]),
         851: () => h("default", "@lezer/common", [1, 1, 0, 0])
     }, g = {
-        353: [408, 593, 663, 785, 829, 861],
+        353: [41, 200, 543, 593, 745, 829],
         598: [204, 211],
         818: [373, 851]
     }, j.f.consumes = (e, r) => {
         j.o(g, e) && g[e].forEach((e => {
             if (j.o(m, e)) return r.push(m[e]);
             var t = r => {
                     m[e] = 0, j.m[e] = t => {
@@ -290,10 +290,10 @@
                     l && l(j)
                 }
                 for (r && r(t); u < n.length; u++) o = n[u], j.o(e, o) && e[o] && e[o][0](), e[o] = 0
             },
             t = self.webpackChunk_axlair_jupyterlab_vim = self.webpackChunk_axlair_jupyterlab_vim || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
     })(), j.nc = void 0;
-    var S = j(130);
+    var S = j(678);
     (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB)["@axlair/jupyterlab_vim"] = S
 })();
```

### Comparing `jupyterlab_vim-4.0.1/jupyterlab_vim/labextension/static/third-party-licenses.json` & `jupyterlab_vim-4.0.2/jupyterlab_vim/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_vim-4.0.1/schema/plugin.json` & `jupyterlab_vim-4.0.2/schema/plugin.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9987745098039216%*

 * *Differences: {"'jupyter.lab.shortcuts'": "{insert: [(26, OrderedDict([('selector', "*

 * *                            "'.jp-Notebook.jp-mod-commandMode'), ('keys', ['Shift Escape']), "*

 * *                            "('command', '')]))]}"}*

```diff
@@ -256,14 +256,21 @@
             "command": "notebook:enter-command-mode",
             "keys": [
                 "Shift Escape"
             ],
             "selector": ".jp-NotebookPanel[data-jp-vim-mode='true'] .jp-Notebook.jp-mod-editMode"
         },
         {
+            "command": "",
+            "keys": [
+                "Shift Escape"
+            ],
+            "selector": ".jp-Notebook.jp-mod-commandMode"
+        },
+        {
             "command": "vim:merge-and-edit",
             "keys": [
                 "Shift M"
             ],
             "selector": ".jp-NotebookPanel[data-jp-vim-mode='true'] .jp-Notebook:focus"
         },
         {
```

### Comparing `jupyterlab_vim-4.0.1/src/codemirrorCommands.ts` & `jupyterlab_vim-4.0.2/src/codemirrorCommands.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_vim-4.0.1/src/index.ts` & `jupyterlab_vim-4.0.2/src/index.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_vim-4.0.1/src/labCommands.ts` & `jupyterlab_vim-4.0.2/src/labCommands.ts`

 * *Files 8% similar despite different names*

```diff
@@ -171,15 +171,21 @@
             if (!cm) {
               console.error('CodeMirror vim wrapper not found');
               return;
             }
             const vim = cm.state.vim;
 
             // Get the current editor state
-            if (vim.insertMode || vim.visualMode) {
+            if (
+              vim.insertMode ||
+              vim.visualMode ||
+              vim.inputState.operator !== null ||
+              vim.inputState.motion !== null ||
+              vim.inputState.keyBuffer.length !== 0
+            ) {
               Vim.handleKey(cm, '<Esc>');
             } else {
               commands.execute('notebook:enter-command-mode');
             }
           }
         }
       },
```

### Comparing `jupyterlab_vim-4.0.1/.gitignore` & `jupyterlab_vim-4.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyterlab_vim-4.0.1/LICENSE` & `jupyterlab_vim-4.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_vim-4.0.1/README.md` & `jupyterlab_vim-4.0.2/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_vim-4.0.1/pyproject.toml` & `jupyterlab_vim-4.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyterlab_vim-4.0.1/PKG-INFO` & `jupyterlab_vim-4.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyterlab_vim
-Version: 4.0.1
+Version: 4.0.2
 Summary: Code cell vim bindings
 Project-URL: Homepage, https://github.com/jupyterlab-contrib/jupyterlab-vim
 Project-URL: Bug Tracker, https://github.com/jupyterlab-contrib/jupyterlab-vim/issues
 Project-URL: Repository, https://github.com/jupyterlab-contrib/jupyterlab-vim.git
 Author: Axel Fahy
 License: MIT License
```

