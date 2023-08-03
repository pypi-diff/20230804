# Comparing `tmp/repo_review-0.9.1.tar.gz` & `tmp/repo_review-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Thu Aug  3 21:37:06 2023, max compression
+gzip compressed data, last modified: Thu Aug  3 23:40:09 2023, max compression
```

## Comparing `repo_review-0.9.1.tar` & `repo_review-0.9.2.tar`

### file list

```diff
@@ -1,58 +1,58 @@
--rw-r--r--   0        0        0      125 2023-08-03 21:37:06.000000 repo_review-0.9.1/.git_archival.txt
--rw-r--r--   0        0        0       32 2023-08-03 21:37:06.000000 repo_review-0.9.1/.gitattributes
--rw-r--r--   0        0        0     2045 2023-08-03 21:37:06.000000 repo_review-0.9.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      187 2023-08-03 21:37:06.000000 repo_review-0.9.1/.pre-commit-hooks.yaml
--rw-r--r--   0        0        0      400 2023-08-03 21:37:06.000000 repo_review-0.9.1/.readthedocs.yaml
--rw-r--r--   0        0        0     1216 2023-08-03 21:37:06.000000 repo_review-0.9.1/action.yml
--rw-r--r--   0        0        0     3219 2023-08-03 21:37:06.000000 repo_review-0.9.1/noxfile.py
--rw-r--r--   0        0        0      359 2023-08-03 21:37:06.000000 repo_review-0.9.1/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0     2527 2023-08-03 21:37:06.000000 repo_review-0.9.1/.github/CONTRIBUTING.md
--rw-r--r--   0        0        0      162 2023-08-03 21:37:06.000000 repo_review-0.9.1/.github/dependabot.yml
--rw-r--r--   0        0        0      668 2023-08-03 21:37:06.000000 repo_review-0.9.1/.github/matchers/pylint.json
--rw-r--r--   0        0        0      669 2023-08-03 21:37:06.000000 repo_review-0.9.1/.github/workflows/cd.yml
--rw-r--r--   0        0        0     2356 2023-08-03 21:37:06.000000 repo_review-0.9.1/.github/workflows/ci.yml
--rw-r--r--   0        0        0        0 2023-08-03 21:37:06.000000 repo_review-0.9.1/docs/.nojekyll
--rw-r--r--   0        0        0      217 2023-08-03 21:37:06.000000 repo_review-0.9.1/docs/changelog.md
--rw-r--r--   0        0        0     6083 2023-08-03 21:37:06.000000 repo_review-0.9.1/docs/checks.md
--rw-r--r--   0        0        0      990 2023-08-03 21:37:06.000000 repo_review-0.9.1/docs/cli.md
--rw-r--r--   0        0        0     2295 2023-08-03 21:37:06.000000 repo_review-0.9.1/docs/conf.py
--rw-r--r--   0        0        0     1445 2023-08-03 21:37:06.000000 repo_review-0.9.1/docs/families.md
--rw-r--r--   0        0        0     2474 2023-08-03 21:37:06.000000 repo_review-0.9.1/docs/fixtures.md
--rw-r--r--   0        0        0     1915 2023-08-03 21:37:06.000000 repo_review-0.9.1/docs/index.html
--rw-r--r--   0        0        0      253 2023-08-03 21:37:06.000000 repo_review-0.9.1/docs/index.md
--rw-r--r--   0        0        0     2248 2023-08-03 21:37:06.000000 repo_review-0.9.1/docs/intro.md
--rw-r--r--   0        0        0     2746 2023-08-03 21:37:06.000000 repo_review-0.9.1/docs/plugins.md
--rw-r--r--   0        0        0     2821 2023-08-03 21:37:06.000000 repo_review-0.9.1/docs/programmatic.md
--rw-r--r--   0        0        0    11110 2023-08-03 21:37:06.000000 repo_review-0.9.1/docs/webapp.js
--rw-r--r--   0        0        0     1770 2023-08-03 21:37:06.000000 repo_review-0.9.1/docs/webapp.md
--rw-r--r--   0        0        0     1033 2023-08-03 21:37:06.000000 repo_review-0.9.1/docs/api/repo_review.rst
--rw-r--r--   0        0        0      230 2023-08-03 21:37:06.000000 repo_review-0.9.1/src/repo_review/__init__.py
--rw-r--r--   0        0        0     8157 2023-08-03 21:37:06.000000 repo_review-0.9.1/src/repo_review/__main__.py
--rw-r--r--   0        0        0      160 2023-08-03 21:37:06.000000 repo_review-0.9.1/src/repo_review/_version.py
--rw-r--r--   0        0        0      118 2023-08-03 21:37:06.000000 repo_review-0.9.1/src/repo_review/_version.pyi
--rw-r--r--   0        0        0     3625 2023-08-03 21:37:06.000000 repo_review-0.9.1/src/repo_review/checks.py
--rw-r--r--   0        0        0     2389 2023-08-03 21:37:06.000000 repo_review-0.9.1/src/repo_review/families.py
--rw-r--r--   0        0        0     3607 2023-08-03 21:37:06.000000 repo_review-0.9.1/src/repo_review/fixtures.py
--rw-r--r--   0        0        0     6010 2023-08-03 21:37:06.000000 repo_review-0.9.1/src/repo_review/ghpath.py
--rw-r--r--   0        0        0     2449 2023-08-03 21:37:06.000000 repo_review-0.9.1/src/repo_review/html.py
--rw-r--r--   0        0        0     7826 2023-08-03 21:37:06.000000 repo_review-0.9.1/src/repo_review/processor.py
--rw-r--r--   0        0        0        0 2023-08-03 21:37:06.000000 repo_review-0.9.1/src/repo_review/py.typed
--rw-r--r--   0        0        0        0 2023-08-03 21:37:06.000000 repo_review-0.9.1/src/repo_review/_compat/__init__.py
--rw-r--r--   0        0        0      233 2023-08-03 21:37:06.000000 repo_review-0.9.1/src/repo_review/_compat/tomllib.py
--rw-r--r--   0        0        0      246 2023-08-03 21:37:06.000000 repo_review-0.9.1/src/repo_review/_compat/typing.py
--rw-r--r--   0        0        0        0 2023-08-03 21:37:06.000000 repo_review-0.9.1/src/repo_review/_compat/importlib/__init__.py
--rw-r--r--   0        0        0        0 2023-08-03 21:37:06.000000 repo_review-0.9.1/src/repo_review/_compat/importlib/resources/__init__.py
--rw-r--r--   0        0        0      256 2023-08-03 21:37:06.000000 repo_review-0.9.1/src/repo_review/_compat/importlib/resources/abc.py
--rw-r--r--   0        0        0     4400 2023-08-03 21:37:06.000000 repo_review-0.9.1/tests/test_checks.py
--rw-r--r--   0        0        0      904 2023-08-03 21:37:06.000000 repo_review-0.9.1/tests/test_cmd.py
--rw-r--r--   0        0        0      452 2023-08-03 21:37:06.000000 repo_review-0.9.1/tests/test_families.py
--rw-r--r--   0        0        0     2408 2023-08-03 21:37:06.000000 repo_review-0.9.1/tests/test_fixtures.py
--rw-r--r--   0        0        0      598 2023-08-03 21:37:06.000000 repo_review-0.9.1/tests/test_package.py
--rw-r--r--   0        0        0     2712 2023-08-03 21:37:06.000000 repo_review-0.9.1/tests/test_self.py
--rw-r--r--   0        0        0     4309 2023-08-03 21:37:06.000000 repo_review-0.9.1/tests/test_utilities/pyproject.py
--rw-r--r--   0        0        0      424 2023-08-03 21:37:06.000000 repo_review-0.9.1/tests/test_utilities/pyproject.toml
--rw-r--r--   0        0        0     2095 2023-08-03 21:37:06.000000 repo_review-0.9.1/.gitignore
--rw-r--r--   0        0        0     1525 2023-08-03 21:37:06.000000 repo_review-0.9.1/LICENSE
--rw-r--r--   0        0        0     6123 2023-08-03 21:37:06.000000 repo_review-0.9.1/README.md
--rw-r--r--   0        0        0     5137 2023-08-03 21:37:06.000000 repo_review-0.9.1/pyproject.toml
--rw-r--r--   0        0        0     8397 2023-08-03 21:37:06.000000 repo_review-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0      125 2023-08-03 23:40:09.000000 repo_review-0.9.2/.git_archival.txt
+-rw-r--r--   0        0        0       32 2023-08-03 23:40:09.000000 repo_review-0.9.2/.gitattributes
+-rw-r--r--   0        0        0     2045 2023-08-03 23:40:09.000000 repo_review-0.9.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      187 2023-08-03 23:40:09.000000 repo_review-0.9.2/.pre-commit-hooks.yaml
+-rw-r--r--   0        0        0      400 2023-08-03 23:40:09.000000 repo_review-0.9.2/.readthedocs.yaml
+-rw-r--r--   0        0        0     1216 2023-08-03 23:40:09.000000 repo_review-0.9.2/action.yml
+-rw-r--r--   0        0        0     3219 2023-08-03 23:40:09.000000 repo_review-0.9.2/noxfile.py
+-rw-r--r--   0        0        0      359 2023-08-03 23:40:09.000000 repo_review-0.9.2/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0     2527 2023-08-03 23:40:09.000000 repo_review-0.9.2/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0      162 2023-08-03 23:40:09.000000 repo_review-0.9.2/.github/dependabot.yml
+-rw-r--r--   0        0        0      668 2023-08-03 23:40:09.000000 repo_review-0.9.2/.github/matchers/pylint.json
+-rw-r--r--   0        0        0      669 2023-08-03 23:40:09.000000 repo_review-0.9.2/.github/workflows/cd.yml
+-rw-r--r--   0        0        0     2356 2023-08-03 23:40:09.000000 repo_review-0.9.2/.github/workflows/ci.yml
+-rw-r--r--   0        0        0        0 2023-08-03 23:40:09.000000 repo_review-0.9.2/docs/.nojekyll
+-rw-r--r--   0        0        0      217 2023-08-03 23:40:09.000000 repo_review-0.9.2/docs/changelog.md
+-rw-r--r--   0        0        0     6083 2023-08-03 23:40:09.000000 repo_review-0.9.2/docs/checks.md
+-rw-r--r--   0        0        0      990 2023-08-03 23:40:09.000000 repo_review-0.9.2/docs/cli.md
+-rw-r--r--   0        0        0     2295 2023-08-03 23:40:09.000000 repo_review-0.9.2/docs/conf.py
+-rw-r--r--   0        0        0     1445 2023-08-03 23:40:09.000000 repo_review-0.9.2/docs/families.md
+-rw-r--r--   0        0        0     2474 2023-08-03 23:40:09.000000 repo_review-0.9.2/docs/fixtures.md
+-rw-r--r--   0        0        0     1915 2023-08-03 23:40:09.000000 repo_review-0.9.2/docs/index.html
+-rw-r--r--   0        0        0      253 2023-08-03 23:40:09.000000 repo_review-0.9.2/docs/index.md
+-rw-r--r--   0        0        0     2248 2023-08-03 23:40:09.000000 repo_review-0.9.2/docs/intro.md
+-rw-r--r--   0        0        0     2746 2023-08-03 23:40:09.000000 repo_review-0.9.2/docs/plugins.md
+-rw-r--r--   0        0        0     2821 2023-08-03 23:40:09.000000 repo_review-0.9.2/docs/programmatic.md
+-rw-r--r--   0        0        0    11187 2023-08-03 23:40:09.000000 repo_review-0.9.2/docs/webapp.js
+-rw-r--r--   0        0        0     1770 2023-08-03 23:40:09.000000 repo_review-0.9.2/docs/webapp.md
+-rw-r--r--   0        0        0     1033 2023-08-03 23:40:09.000000 repo_review-0.9.2/docs/api/repo_review.rst
+-rw-r--r--   0        0        0      230 2023-08-03 23:40:09.000000 repo_review-0.9.2/src/repo_review/__init__.py
+-rw-r--r--   0        0        0     8157 2023-08-03 23:40:09.000000 repo_review-0.9.2/src/repo_review/__main__.py
+-rw-r--r--   0        0        0      160 2023-08-03 23:40:09.000000 repo_review-0.9.2/src/repo_review/_version.py
+-rw-r--r--   0        0        0      118 2023-08-03 23:40:09.000000 repo_review-0.9.2/src/repo_review/_version.pyi
+-rw-r--r--   0        0        0     3625 2023-08-03 23:40:09.000000 repo_review-0.9.2/src/repo_review/checks.py
+-rw-r--r--   0        0        0     2389 2023-08-03 23:40:09.000000 repo_review-0.9.2/src/repo_review/families.py
+-rw-r--r--   0        0        0     3607 2023-08-03 23:40:09.000000 repo_review-0.9.2/src/repo_review/fixtures.py
+-rw-r--r--   0        0        0     6010 2023-08-03 23:40:09.000000 repo_review-0.9.2/src/repo_review/ghpath.py
+-rw-r--r--   0        0        0     2449 2023-08-03 23:40:09.000000 repo_review-0.9.2/src/repo_review/html.py
+-rw-r--r--   0        0        0     7820 2023-08-03 23:40:09.000000 repo_review-0.9.2/src/repo_review/processor.py
+-rw-r--r--   0        0        0        0 2023-08-03 23:40:09.000000 repo_review-0.9.2/src/repo_review/py.typed
+-rw-r--r--   0        0        0        0 2023-08-03 23:40:09.000000 repo_review-0.9.2/src/repo_review/_compat/__init__.py
+-rw-r--r--   0        0        0      233 2023-08-03 23:40:09.000000 repo_review-0.9.2/src/repo_review/_compat/tomllib.py
+-rw-r--r--   0        0        0      246 2023-08-03 23:40:09.000000 repo_review-0.9.2/src/repo_review/_compat/typing.py
+-rw-r--r--   0        0        0        0 2023-08-03 23:40:09.000000 repo_review-0.9.2/src/repo_review/_compat/importlib/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-03 23:40:09.000000 repo_review-0.9.2/src/repo_review/_compat/importlib/resources/__init__.py
+-rw-r--r--   0        0        0      256 2023-08-03 23:40:09.000000 repo_review-0.9.2/src/repo_review/_compat/importlib/resources/abc.py
+-rw-r--r--   0        0        0     4400 2023-08-03 23:40:09.000000 repo_review-0.9.2/tests/test_checks.py
+-rw-r--r--   0        0        0      904 2023-08-03 23:40:09.000000 repo_review-0.9.2/tests/test_cmd.py
+-rw-r--r--   0        0        0      452 2023-08-03 23:40:09.000000 repo_review-0.9.2/tests/test_families.py
+-rw-r--r--   0        0        0     2408 2023-08-03 23:40:09.000000 repo_review-0.9.2/tests/test_fixtures.py
+-rw-r--r--   0        0        0      598 2023-08-03 23:40:09.000000 repo_review-0.9.2/tests/test_package.py
+-rw-r--r--   0        0        0     2712 2023-08-03 23:40:09.000000 repo_review-0.9.2/tests/test_self.py
+-rw-r--r--   0        0        0     4309 2023-08-03 23:40:09.000000 repo_review-0.9.2/tests/test_utilities/pyproject.py
+-rw-r--r--   0        0        0      424 2023-08-03 23:40:09.000000 repo_review-0.9.2/tests/test_utilities/pyproject.toml
+-rw-r--r--   0        0        0     2095 2023-08-03 23:40:09.000000 repo_review-0.9.2/.gitignore
+-rw-r--r--   0        0        0     1525 2023-08-03 23:40:09.000000 repo_review-0.9.2/LICENSE
+-rw-r--r--   0        0        0     6123 2023-08-03 23:40:09.000000 repo_review-0.9.2/README.md
+-rw-r--r--   0        0        0     5137 2023-08-03 23:40:09.000000 repo_review-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0     8397 2023-08-03 23:40:09.000000 repo_review-0.9.2/PKG-INFO
```

### Comparing `repo_review-0.9.1/.pre-commit-config.yaml` & `repo_review-0.9.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `repo_review-0.9.1/action.yml` & `repo_review-0.9.2/action.yml`

 * *Files identical despite different names*

### Comparing `repo_review-0.9.1/noxfile.py` & `repo_review-0.9.2/noxfile.py`

 * *Files identical despite different names*

### Comparing `repo_review-0.9.1/.github/CONTRIBUTING.md` & `repo_review-0.9.2/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `repo_review-0.9.1/.github/matchers/pylint.json` & `repo_review-0.9.2/.github/matchers/pylint.json`

 * *Files identical despite different names*

### Comparing `repo_review-0.9.1/.github/workflows/cd.yml` & `repo_review-0.9.2/.github/workflows/cd.yml`

 * *Files identical despite different names*

### Comparing `repo_review-0.9.1/.github/workflows/ci.yml` & `repo_review-0.9.2/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `repo_review-0.9.1/docs/checks.md` & `repo_review-0.9.2/docs/checks.md`

 * *Files identical despite different names*

### Comparing `repo_review-0.9.1/docs/cli.md` & `repo_review-0.9.2/docs/cli.md`

 * *Files identical despite different names*

### Comparing `repo_review-0.9.1/docs/conf.py` & `repo_review-0.9.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `repo_review-0.9.1/docs/families.md` & `repo_review-0.9.2/docs/families.md`

 * *Files identical despite different names*

### Comparing `repo_review-0.9.1/docs/fixtures.md` & `repo_review-0.9.2/docs/fixtures.md`

 * *Files identical despite different names*

### Comparing `repo_review-0.9.1/docs/index.html` & `repo_review-0.9.2/docs/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -59,13 +59,13 @@
   <body>
     <div id="root">Loading...</div>
     <script type="text/babel">
       const root = ReactDOM.createRoot(document.getElementById("root"));
       root.render(
         <App
           header={true}
-          deps={["sp-repo-review==2023.08.03", "repo-review==0.9.0"]}
+          deps={["sp-repo-review==2023.08.03", "repo-review==0.9.2"]}
         />,
       );
     </script>
   </body>
 </html>
```

### Comparing `repo_review-0.9.1/docs/intro.md` & `repo_review-0.9.2/docs/intro.md`

 * *Files identical despite different names*

### Comparing `repo_review-0.9.1/docs/plugins.md` & `repo_review-0.9.2/docs/plugins.md`

 * *Files identical despite different names*

### Comparing `repo_review-0.9.1/docs/programmatic.md` & `repo_review-0.9.2/docs/programmatic.md`

 * *Files identical despite different names*

### Comparing `repo_review-0.9.1/docs/webapp.js` & `repo_review-0.9.2/docs/webapp.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -211,15 +211,17 @@
                 props.families[key].name
             } <
             /MaterialUI.ListSubheader> {
                 props.families[key].description && ( <
                     MaterialUI.ListItem >
                     <
                     span dangerouslySetInnerHTML = {
-                        props.families[key].description
+                        {
+                            __html: props.families[key].description,
+                        }
                     }
                     /> <
                     /MaterialUI.ListItem>
                 )
             } {
                 results_components
             } <
```

### Comparing `repo_review-0.9.1/docs/webapp.md` & `repo_review-0.9.2/docs/webapp.md`

 * *Files identical despite different names*

### Comparing `repo_review-0.9.1/docs/api/repo_review.rst` & `repo_review-0.9.2/docs/api/repo_review.rst`

 * *Files identical despite different names*

### Comparing `repo_review-0.9.1/src/repo_review/__main__.py` & `repo_review-0.9.2/src/repo_review/__main__.py`

 * *Files identical despite different names*

### Comparing `repo_review-0.9.1/src/repo_review/checks.py` & `repo_review-0.9.2/src/repo_review/checks.py`

 * *Files identical despite different names*

### Comparing `repo_review-0.9.1/src/repo_review/families.py` & `repo_review-0.9.2/src/repo_review/families.py`

 * *Files identical despite different names*

### Comparing `repo_review-0.9.1/src/repo_review/fixtures.py` & `repo_review-0.9.2/src/repo_review/fixtures.py`

 * *Files identical despite different names*

### Comparing `repo_review-0.9.1/src/repo_review/ghpath.py` & `repo_review-0.9.2/src/repo_review/ghpath.py`

 * *Files identical despite different names*

### Comparing `repo_review-0.9.1/src/repo_review/html.py` & `repo_review-0.9.2/src/repo_review/html.py`

 * *Files identical despite different names*

### Comparing `repo_review-0.9.1/src/repo_review/processor.py` & `repo_review-0.9.2/src/repo_review/processor.py`

 * *Files 0% similar despite different names*

```diff
@@ -206,15 +206,15 @@
         if all(completed.get(n, "") == "" for n in graph[name]):
             result = apply_fixtures({"name": name, **fixtures}, tasks[name].check)
             if isinstance(result, bool):
                 completed[name] = (
                     ""
                     if result
                     else (tasks[name].check.__doc__ or "Check failed").format(
-                        name=name, self=tasks[name].check
+                        name=name, self=tasks[name]
                     )
                 )
             else:
                 completed[name] = result
         else:
             completed[name] = None
```

### Comparing `repo_review-0.9.1/tests/test_checks.py` & `repo_review-0.9.2/tests/test_checks.py`

 * *Files identical despite different names*

### Comparing `repo_review-0.9.1/tests/test_cmd.py` & `repo_review-0.9.2/tests/test_cmd.py`

 * *Files identical despite different names*

### Comparing `repo_review-0.9.1/tests/test_fixtures.py` & `repo_review-0.9.2/tests/test_fixtures.py`

 * *Files identical despite different names*

### Comparing `repo_review-0.9.1/tests/test_package.py` & `repo_review-0.9.2/tests/test_package.py`

 * *Files identical despite different names*

### Comparing `repo_review-0.9.1/tests/test_self.py` & `repo_review-0.9.2/tests/test_self.py`

 * *Files identical despite different names*

### Comparing `repo_review-0.9.1/tests/test_utilities/pyproject.py` & `repo_review-0.9.2/tests/test_utilities/pyproject.py`

 * *Files identical despite different names*

### Comparing `repo_review-0.9.1/.gitignore` & `repo_review-0.9.2/.gitignore`

 * *Files identical despite different names*

### Comparing `repo_review-0.9.1/LICENSE` & `repo_review-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `repo_review-0.9.1/README.md` & `repo_review-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `repo_review-0.9.1/pyproject.toml` & `repo_review-0.9.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `repo_review-0.9.1/PKG-INFO` & `repo_review-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: repo_review
-Version: 0.9.1
+Version: 0.9.2
 Summary: Framework that can run checks on repos
 Project-URL: Changelog, https://github.com/scientific-python/repo-review/releases
 Project-URL: Demo, https://scientific-python.github.io/repo-review
 Project-URL: Documentation, https://repo-review.readthedocs.io
 Project-URL: Homepage, https://repo-review.readthedocs.io
 Project-URL: Source, https://github.com/scientific-python/repo-review
 Author-email: Henry Schreiner <henryfs@princeton.edu>
```

