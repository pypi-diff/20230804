# Comparing `tmp/totolo-1.0.tar.gz` & `tmp/totolo-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "totolo-1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "totolo-1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `totolo-1.0.tar` & `totolo-1.1.tar`

### file list

```diff
@@ -1,47 +1,48 @@
--rw-r--r--   0        0        0     1096 2023-07-30 09:27:45.183451 totolo-1.0/.github/workflows/coverage-branch.yaml
--rw-r--r--   0        0        0     1143 2023-07-30 09:27:45.183451 totolo-1.0/.github/workflows/coverage.yaml
--rw-r--r--   0        0        0     1300 2023-07-30 09:27:45.183451 totolo-1.0/.github/workflows/publish.yaml
--rw-r--r--   0        0        0      854 2023-07-30 09:27:45.183451 totolo-1.0/.github/workflows/test.yaml
--rw-r--r--   0        0        0     3081 2023-07-30 09:27:45.183451 totolo-1.0/.gitignore
--rw-r--r--   0        0        0      892 2023-07-30 09:27:45.183451 totolo-1.0/.vscode/launch.json
--rw-r--r--   0        0        0      277 2023-07-30 09:27:45.183451 totolo-1.0/.vscode/settings.json
--rw-r--r--   0        0        0     1071 2023-07-30 09:27:45.183451 totolo-1.0/LICENSE
--rw-r--r--   0        0        0      729 2023-07-30 09:27:45.183451 totolo-1.0/README.md
--rw-r--r--   0        0        0     1259 2023-07-30 09:27:45.183451 totolo-1.0/pyproject.toml
--rw-r--r--   0        0        0       38 2023-07-30 09:27:45.183451 totolo-1.0/requirements-dev.txt
--rw-r--r--   0        0        0        0 2023-07-30 09:27:45.183451 totolo-1.0/tests/__init__.py
--rw-r--r--   0        0        0       24 2023-07-30 09:27:45.183451 totolo-1.0/tests/data/cycles1.th.txt
--rw-r--r--   0        0        0       47 2023-07-30 09:27:45.183451 totolo-1.0/tests/data/cycles2.th.txt
--rw-r--r--   0        0        0       71 2023-07-30 09:27:45.183451 totolo-1.0/tests/data/cycles3.th.txt
--rw-r--r--   0        0        0   173716 2023-07-30 09:27:45.183451 totolo-1.0/tests/data/film-timeout-top100.st.txt
--rw-r--r--   0        0        0   332534 2023-07-30 09:27:45.187451 totolo-1.0/tests/data/flat.tar.gz
--rw-r--r--   0        0        0      166 2023-07-30 09:27:45.187451 totolo-1.0/tests/data/messy.st.txt
--rw-r--r--   0        0        0   332557 2023-07-30 09:27:45.187451 totolo-1.0/tests/data/sample-2023.07.23.tar.gz
--rw-r--r--   0        0        0    34632 2023-07-30 09:27:45.187451 totolo-1.0/tests/data/sample-2023.07.23/notes/collections/scifi-collections.st.txt
--rw-r--r--   0        0        0    28050 2023-07-30 09:27:45.187451 totolo-1.0/tests/data/sample-2023.07.23/notes/stories/film/film-scifi-1920s.st.txt
--rw-r--r--   0        0        0    48760 2023-07-30 09:27:45.187451 totolo-1.0/tests/data/sample-2023.07.23/notes/stories/film/film-scifi-1930s.st.txt
--rw-r--r--   0        0        0  1011578 2023-07-30 09:27:45.195451 totolo-1.0/tests/data/sample-2023.07.23/notes/themes/primary.th.txt
--rw-r--r--   0        0        0    14882 2023-07-30 09:27:45.195451 totolo-1.0/tests/data/sample-2023.07.23/notes/themes/timeperiod.th.txt
--rw-r--r--   0        0        0      428 2023-07-30 09:27:45.195451 totolo-1.0/tests/data/storytree.st.txt
--rw-r--r--   0        0        0  1011579 2023-07-30 09:27:45.203451 totolo-1.0/tests/data/to-2023.07.09.th.txt
--rw-r--r--   0        0        0     2365 2023-07-30 09:27:45.203451 totolo-1.0/tests/data/to-sample-2023.07.09-copy.st.txt
--rw-r--r--   0        0        0     2365 2023-07-30 09:27:45.203451 totolo-1.0/tests/data/to-sample-2023.07.09.st.txt
--rw-r--r--   0        0        0     6150 2023-07-30 09:27:45.203451 totolo-1.0/tests/test_entries.py
--rw-r--r--   0        0        0     5692 2023-07-30 09:27:45.203451 totolo-1.0/tests/test_impl.py
--rw-r--r--   0        0        0     2219 2023-07-30 09:27:45.203451 totolo-1.0/tests/test_lib.py
--rw-r--r--   0        0        0    10843 2023-07-30 09:27:45.203451 totolo-1.0/tests/test_totolo.py
--rw-r--r--   0        0        0      189 2023-07-30 09:27:45.203451 totolo-1.0/totolo/__init__.py
--rw-r--r--   0        0        0     1201 2023-07-30 09:27:45.203451 totolo-1.0/totolo/api.py
--rw-r--r--   0        0        0        0 2023-07-30 09:27:45.203451 totolo-1.0/totolo/impl/__init__.py
--rw-r--r--   0        0        0     2953 2023-07-30 09:27:45.203451 totolo-1.0/totolo/impl/core.py
--rw-r--r--   0        0        0     5245 2023-07-30 09:27:45.203451 totolo-1.0/totolo/impl/entry.py
--rw-r--r--   0        0        0     3160 2023-07-30 09:27:45.203451 totolo-1.0/totolo/impl/field.py
--rw-r--r--   0        0        0      424 2023-07-30 09:27:45.203451 totolo-1.0/totolo/impl/keyword.py
--rw-r--r--   0        0        0     7567 2023-07-30 09:27:45.203451 totolo-1.0/totolo/impl/parser.py
--rw-r--r--   0        0        0        0 2023-07-30 09:27:45.203451 totolo-1.0/totolo/lib/__init__.py
--rw-r--r--   0        0        0     1134 2023-07-30 09:27:45.203451 totolo-1.0/totolo/lib/files.py
--rw-r--r--   0        0        0     1283 2023-07-30 09:27:45.203451 totolo-1.0/totolo/lib/textformat.py
--rw-r--r--   0        0        0     3456 2023-07-30 09:27:45.203451 totolo-1.0/totolo/story.py
--rw-r--r--   0        0        0     2209 2023-07-30 09:27:45.203451 totolo-1.0/totolo/theme.py
--rw-r--r--   0        0        0     6687 2023-07-30 09:27:45.203451 totolo-1.0/totolo/themeontology.py
--rw-r--r--   0        0        0     1161 1970-01-01 00:00:00.000000 totolo-1.0/PKG-INFO
+-rw-r--r--   0        0        0     1096 2023-08-04 12:18:30.557114 totolo-1.1/.github/workflows/coverage-branch.yaml
+-rw-r--r--   0        0        0     1143 2023-08-04 12:18:30.557114 totolo-1.1/.github/workflows/coverage.yaml
+-rw-r--r--   0        0        0     1300 2023-08-04 12:18:30.557114 totolo-1.1/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0      854 2023-08-04 12:18:30.557114 totolo-1.1/.github/workflows/test.yaml
+-rw-r--r--   0        0        0     3081 2023-08-04 12:18:30.557114 totolo-1.1/.gitignore
+-rw-r--r--   0        0        0     1468 2023-08-04 12:18:30.557114 totolo-1.1/.vscode/launch.json
+-rw-r--r--   0        0        0      277 2023-08-04 12:18:30.557114 totolo-1.1/.vscode/settings.json
+-rw-r--r--   0        0        0     1071 2023-08-04 12:18:30.557114 totolo-1.1/LICENSE
+-rw-r--r--   0        0        0      729 2023-08-04 12:18:30.557114 totolo-1.1/README.md
+-rw-r--r--   0        0        0      977 2023-08-04 12:18:30.557114 totolo-1.1/examples/basics.py
+-rw-r--r--   0        0        0     1387 2023-08-04 12:18:30.557114 totolo-1.1/pyproject.toml
+-rw-r--r--   0        0        0       46 2023-08-04 12:18:30.557114 totolo-1.1/requirements-dev.txt
+-rw-r--r--   0        0        0        0 2023-08-04 12:18:30.557114 totolo-1.1/tests/__init__.py
+-rw-r--r--   0        0        0       24 2023-08-04 12:18:30.557114 totolo-1.1/tests/data/cycles1.th.txt
+-rw-r--r--   0        0        0       47 2023-08-04 12:18:30.557114 totolo-1.1/tests/data/cycles2.th.txt
+-rw-r--r--   0        0        0       71 2023-08-04 12:18:30.557114 totolo-1.1/tests/data/cycles3.th.txt
+-rw-r--r--   0        0        0   173716 2023-08-04 12:18:30.557114 totolo-1.1/tests/data/film-timeout-top100.st.txt
+-rw-r--r--   0        0        0   332534 2023-08-04 12:18:30.561114 totolo-1.1/tests/data/flat.tar.gz
+-rw-r--r--   0        0        0      166 2023-08-04 12:18:30.561114 totolo-1.1/tests/data/messy.st.txt
+-rw-r--r--   0        0        0   332557 2023-08-04 12:18:30.561114 totolo-1.1/tests/data/sample-2023.07.23.tar.gz
+-rw-r--r--   0        0        0    34632 2023-08-04 12:18:30.561114 totolo-1.1/tests/data/sample-2023.07.23/notes/collections/scifi-collections.st.txt
+-rw-r--r--   0        0        0    28050 2023-08-04 12:18:30.561114 totolo-1.1/tests/data/sample-2023.07.23/notes/stories/film/film-scifi-1920s.st.txt
+-rw-r--r--   0        0        0    48760 2023-08-04 12:18:30.561114 totolo-1.1/tests/data/sample-2023.07.23/notes/stories/film/film-scifi-1930s.st.txt
+-rw-r--r--   0        0        0  1011578 2023-08-04 12:18:30.569115 totolo-1.1/tests/data/sample-2023.07.23/notes/themes/primary.th.txt
+-rw-r--r--   0        0        0    14882 2023-08-04 12:18:30.569115 totolo-1.1/tests/data/sample-2023.07.23/notes/themes/timeperiod.th.txt
+-rw-r--r--   0        0        0      428 2023-08-04 12:18:30.569115 totolo-1.1/tests/data/storytree.st.txt
+-rw-r--r--   0        0        0  1011579 2023-08-04 12:18:30.573115 totolo-1.1/tests/data/to-2023.07.09.th.txt
+-rw-r--r--   0        0        0     2365 2023-08-04 12:18:30.577116 totolo-1.1/tests/data/to-sample-2023.07.09-copy.st.txt
+-rw-r--r--   0        0        0     2365 2023-08-04 12:18:30.577116 totolo-1.1/tests/data/to-sample-2023.07.09.st.txt
+-rw-r--r--   0        0        0     6150 2023-08-04 12:18:30.577116 totolo-1.1/tests/test_entries.py
+-rw-r--r--   0        0        0     5663 2023-08-04 12:18:30.577116 totolo-1.1/tests/test_impl.py
+-rw-r--r--   0        0        0     2219 2023-08-04 12:18:30.577116 totolo-1.1/tests/test_lib.py
+-rw-r--r--   0        0        0    10837 2023-08-04 12:18:30.577116 totolo-1.1/tests/test_totolo.py
+-rw-r--r--   0        0        0      189 2023-08-04 12:18:30.577116 totolo-1.1/totolo/__init__.py
+-rw-r--r--   0        0        0     1201 2023-08-04 12:18:30.577116 totolo-1.1/totolo/api.py
+-rw-r--r--   0        0        0        0 2023-08-04 12:18:30.577116 totolo-1.1/totolo/impl/__init__.py
+-rw-r--r--   0        0        0     3014 2023-08-04 12:18:30.577116 totolo-1.1/totolo/impl/core.py
+-rw-r--r--   0        0        0     5913 2023-08-04 12:18:30.577116 totolo-1.1/totolo/impl/entry.py
+-rw-r--r--   0        0        0     3300 2023-08-04 12:18:30.577116 totolo-1.1/totolo/impl/field.py
+-rw-r--r--   0        0        0      666 2023-08-04 12:18:30.577116 totolo-1.1/totolo/impl/keyword.py
+-rw-r--r--   0        0        0     8129 2023-08-04 12:18:30.577116 totolo-1.1/totolo/impl/parser.py
+-rw-r--r--   0        0        0        0 2023-08-04 12:18:30.577116 totolo-1.1/totolo/lib/__init__.py
+-rw-r--r--   0        0        0     1134 2023-08-04 12:18:30.577116 totolo-1.1/totolo/lib/files.py
+-rw-r--r--   0        0        0     1283 2023-08-04 12:18:30.577116 totolo-1.1/totolo/lib/textformat.py
+-rw-r--r--   0        0        0     3419 2023-08-04 12:18:30.577116 totolo-1.1/totolo/story.py
+-rw-r--r--   0        0        0     2209 2023-08-04 12:18:30.577116 totolo-1.1/totolo/theme.py
+-rw-r--r--   0        0        0     6698 2023-08-04 12:18:30.577116 totolo-1.1/totolo/themeontology.py
+-rw-r--r--   0        0        0     1161 1970-01-01 00:00:00.000000 totolo-1.1/PKG-INFO
```

### Comparing `totolo-1.0/.github/workflows/coverage-branch.yaml` & `totolo-1.1/.github/workflows/coverage-branch.yaml`

 * *Files identical despite different names*

### Comparing `totolo-1.0/.github/workflows/coverage.yaml` & `totolo-1.1/.github/workflows/coverage.yaml`

 * *Files identical despite different names*

### Comparing `totolo-1.0/.github/workflows/publish.yaml` & `totolo-1.1/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `totolo-1.0/.github/workflows/test.yaml` & `totolo-1.1/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `totolo-1.0/.gitignore` & `totolo-1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `totolo-1.0/.vscode/launch.json` & `totolo-1.1/.vscode/launch.json`

 * *Files 27% similar despite different names*

```diff
@@ -7,14 +7,33 @@
         {
             "name": "Python: Current File",
             "type": "python",
             "request": "launch",
             "program": "${file}",
             "console": "integratedTerminal",
             "justMyCode": true,
+            "cwd": "${workspaceFolder}",
+            "env": {
+                "PYTHONPATH": "$PYTHONPATH:${workspaceFolder}",
+            }
+        },
+        {
+            "name": "Python: Profile Current File",
+            "type": "python",
+            "request": "launch",
+            "module": "cProfile",
+            "args": [
+                "-o",
+                "profiler-results.prof",
+                "${file}"
+            ],
+            "cwd": "${workspaceFolder}",
+            "env": {
+                "PYTHONPATH": "$PYTHONPATH:${workspaceFolder}",
+            }
         },
         {
             "name": "Python: Debug Tests",
             "type": "python",
             "request": "launch",
             "program": "${file}",
             "purpose": [
```

### Comparing `totolo-1.0/LICENSE` & `totolo-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `totolo-1.0/README.md` & `totolo-1.1/README.md`

 * *Files identical despite different names*

### Comparing `totolo-1.0/pyproject.toml` & `totolo-1.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -21,14 +21,16 @@
 [tool.pylint."MESSAGES CONTROL"]
 disable = [
     "missing-module-docstring",         # don't want it
     "missing-class-docstring",          # don't want it
     "missing-function-docstring",       # don't want it
     "too-few-public-methods",           # don't want it
     "too-many-arguments",               # borderline acceptable
+    "super-init-not-called",            # borderline acceptable
+    "import-outside-toplevel",          # borderline acceptable
     "no-member",                        # pylint gets it wrong
     "unsupported-membership-test",      # pylint gets it wrong
     "not-callable",                     # pylint gets it wrong
     "unsubscriptable-object",           # pylint gets it wrong
     "unsupported-assignment-operation", # pylint gets it wrong
     "unsupported-delete-operation",     # pylint gets it wrong
 ]
```

### Comparing `totolo-1.0/tests/data/film-timeout-top100.st.txt` & `totolo-1.1/tests/data/film-timeout-top100.st.txt`

 * *Files identical despite different names*

### Comparing `totolo-1.0/tests/data/flat.tar.gz` & `totolo-1.1/tests/data/flat.tar.gz`

 * *Files identical despite different names*

### Comparing `totolo-1.0/tests/data/sample-2023.07.23.tar.gz` & `totolo-1.1/tests/data/sample-2023.07.23.tar.gz`

 * *Files identical despite different names*

### Comparing `totolo-1.0/tests/data/sample-2023.07.23/notes/collections/scifi-collections.st.txt` & `totolo-1.1/tests/data/sample-2023.07.23/notes/collections/scifi-collections.st.txt`

 * *Files identical despite different names*

### Comparing `totolo-1.0/tests/data/sample-2023.07.23/notes/stories/film/film-scifi-1920s.st.txt` & `totolo-1.1/tests/data/sample-2023.07.23/notes/stories/film/film-scifi-1920s.st.txt`

 * *Files identical despite different names*

### Comparing `totolo-1.0/tests/data/sample-2023.07.23/notes/stories/film/film-scifi-1930s.st.txt` & `totolo-1.1/tests/data/sample-2023.07.23/notes/stories/film/film-scifi-1930s.st.txt`

 * *Files identical despite different names*

### Comparing `totolo-1.0/tests/data/sample-2023.07.23/notes/themes/primary.th.txt` & `totolo-1.1/tests/data/sample-2023.07.23/notes/themes/primary.th.txt`

 * *Files identical despite different names*

### Comparing `totolo-1.0/tests/data/sample-2023.07.23/notes/themes/timeperiod.th.txt` & `totolo-1.1/tests/data/sample-2023.07.23/notes/themes/timeperiod.th.txt`

 * *Files identical despite different names*

### Comparing `totolo-1.0/tests/data/to-2023.07.09.th.txt` & `totolo-1.1/tests/data/to-2023.07.09.th.txt`

 * *Files identical despite different names*

### Comparing `totolo-1.0/tests/data/to-sample-2023.07.09-copy.st.txt` & `totolo-1.1/tests/data/to-sample-2023.07.09-copy.st.txt`

 * *Files identical despite different names*

### Comparing `totolo-1.0/tests/data/to-sample-2023.07.09.st.txt` & `totolo-1.1/tests/data/to-sample-2023.07.09.st.txt`

 * *Files identical despite different names*

### Comparing `totolo-1.0/tests/test_entries.py` & `totolo-1.1/tests/test_entries.py`

 * *Files identical despite different names*

### Comparing `totolo-1.0/tests/test_impl.py` & `totolo-1.1/tests/test_impl.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,18 +14,17 @@
     bb = sa("txt", default="baz: b", required=True)
     cc = sa("txt", default="baz: c")
     aa = sa("txt", default="baz: a")
 
 
 class TestTOObject:
     def test_object_attributes(self):
-        a = TOTest1(qq=2, bb="monkey", a2="fox")
+        a = TOTest1(a2="fox")
         assert a.a1 == "foo"
         assert a.a2 == "fox"
-        assert a.bb == "monkey"
         attrs = [k for k, _ in a.iter_attrs()]
         sattrs = [k for k, _ in a.iter_stored()]
         assert attrs == ["a1", "a2", "a3", "bb", "cc", "aa"]
         assert sattrs == ["bb", "cc", "aa"]
         assert not hasattr(a, "aa")
         assert not hasattr(a, "cc")
         assert not hasattr(a, "a3")
@@ -54,17 +53,15 @@
         for strobj in strs:
             assert isinstance(strobj, str)
             assert len(strobj) > 5
 
 
 class TestField:
     def make_field(self, fieldtype="text"):
-        field = TOField(name="foo", fieldtype=fieldtype)
-        field.data.append("data line")
-        field.source.append("source line")
+        field = TOField(name="foo", fieldtype=fieldtype, source=["source line"]).setup()
         if fieldtype == "kwlist":
             field.insert_kw(
                 keyword="foo",
                 motivation="bar",
                 capacity="baz",
                 notes="widget",
             )
@@ -149,25 +146,25 @@
             "",
             "",
         ])
         assert story.source[-1] == ""
         assert story.source[-2] == ""
         assert story.source[-3] == "1789"
 
-    def test_oddities(self):
+    def test_bad_url(self):
         ontology = totolo.empty()
-
         with pytest.raises(ValueError):
             TOParser.add_url(ontology, "gobbledygook")
 
+    def test_bad_kwfield(self):
         with pytest.raises(AssertionError):
-            list(TOParser.iter_kwitems(["malformed ] field"]))
+            list(TOParser.iter_kwitems_strict(["malformed ] field"]))
         with pytest.raises(AssertionError):
-            list(TOParser.iter_kwitems(["malformed <[]} field"]))
+            list(TOParser.iter_kwitems_strict(["malformed <[]} field"]))
         with pytest.raises(AssertionError):
-            list(TOParser.iter_kwitems(["malformed {}> field"]))
+            list(TOParser.iter_kwitems_strict(["malformed {}> field"]))
         with pytest.raises(AssertionError):
-            list(TOParser.iter_kwitems(["malformed <<>> field"]))
+            list(TOParser.iter_kwitems_strict(["malformed <<>> field"]))
         with pytest.raises(AssertionError):
-            list(TOParser.iter_kwitems(["malformed {{}} field"]))
+            list(TOParser.iter_kwitems_strict(["malformed {{}} field"]))
         with pytest.raises(AssertionError):
-            list(TOParser.iter_kwitems(["malformed [[]] field"]))
+            list(TOParser.iter_kwitems_strict(["malformed [[]] field"]))
```

### Comparing `totolo-1.0/tests/test_lib.py` & `totolo-1.1/tests/test_lib.py`

 * *Files identical despite different names*

### Comparing `totolo-1.0/tests/test_totolo.py` & `totolo-1.1/tests/test_totolo.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,40 +65,40 @@
     def test_theme_attributes(self):
         ontology = totolo.files("tests/data/to-2023.07.09.th.txt")
         t = ontology.theme["coping with senility"]
         t.print()
         assert t.name == "coping with senility"
         assert t["Description"].str().startswith(
             "A character copes with a loss of their mental faculties")
-        assert t["Parents"].list() == ["human health condition"]
+        assert list(t["Parents"]) == ["human health condition"]
         assert t["Notes"].str().startswith(
             "This theme is used for example when")
         assert t["Examples"].str().startswith(
             'In tng3x23 "Sarek", Sarek coped')
-        assert t["References"].list() == ["https://en.wikipedia.org/wiki/Dementia"]
-        assert t["Aliases"].list() == ["coping with dementia"]
+        assert list(t["References"]) == ["https://en.wikipedia.org/wiki/Dementia"]
+        assert list(t["Aliases"]) == ["coping with dementia"]
 
     def test_story_attributes(self):
         name = "play: The Taming of the Shrew (1592)"
         ontology = totolo.files("tests/data/to-sample-2023.07.09.st.txt")
         s = ontology.story[name]
         s.print()
         assert s.name == name
         assert s.sid == name
         assert s["Title"].str() == "The Taming of the Shrew"
         assert s["Date"].str() == "1592"
         assert s.date == "1592"
         assert s.year == 1592
         assert "a drunken tinker named Christopher Sly" in s["Description"].str()
         assert s["Authors"].str() == "William Shakespeare"
-        assert s["References"].list() == [
+        assert list(s["References"]) == [
             "https://en.wikipedia.org/wiki/The_Taming_of_the_Shrew"
         ]
-        assert s["Ratings"].list() == ["4 <mikael>"]
-        assert s["Collections"].list() == []
+        assert list(s["Ratings"]) == ["4 <mikael>"]
+        assert list(s["Collections"]) == []
 
     def test_fetch_and_write(self):
         print("Downloading master...")
         with open("tests/data/sample-2023.07.23.tar.gz", "rb+") as fh:
             with patch.object(urllib.request, 'urlopen', return_value=fh):
                 to1 = totolo.remote()
         with tempfile.TemporaryDirectory() as prefix:
```

### Comparing `totolo-1.0/totolo/api.py` & `totolo-1.1/totolo/api.py`

 * *Files identical despite different names*

### Comparing `totolo-1.0/totolo/impl/core.py` & `totolo-1.1/totolo/impl/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from collections import OrderedDict
-from copy import deepcopy
 
 
 class TOAttr:
     def __init__(self, default="", private=False):
         self.default = default
         self.private = private
 
@@ -11,15 +10,15 @@
         tname = self.__class__.__name__
         return f"{tname}({self.default})"
 
 
 class TOStoredAttr(TOAttr):
     def __init__(self, datatype="blob", default=None, required=False):
         if default is None:
-            default = [] if "list" in datatype else ""
+            default = list if "list" in datatype else ""
         super().__init__(default, True)
         self.datatype = datatype
         self.required = required
 
     def __str__(self):
         tname = self.__class__.__name__
         return f"{tname}<{self.datatype}>({self.default})"
@@ -37,21 +36,26 @@
                 nkey = key.replace("_", " ")
                 to_attrs[nkey] = value
                 del attr[key]
             elif isinstance(value, TOAttr):
                 to_attrs[key] = value
                 del attr[key]
         attr["_to_attrs"] = to_attrs
+        attr["_to_attrs_public"] = {k: v for k, v in to_attrs.items() if not v.private}
         return super().__new__(mcs, name, bases, attr)
 
     def __call__(cls, *args, **kwargs):
         self = super().__call__(*args, **kwargs)
-        for key, value in self._to_attrs.items():
-            if not value.private and not hasattr(self, key):
-                setattr(self, key, deepcopy(value.default))
+        target = self.__dict__
+        for key, value in self._to_attrs_public.items():
+            if not key in target:
+                if callable(value.default):
+                    target[key] = value.default()
+                else:
+                    target[key] = value.default
         return self
 
     @classmethod
     def __prepare__(mcs, _cls, _bases):
         return OrderedDict()
 
 
@@ -60,21 +64,20 @@
 
 
 def sa(*args, **kwargs):
     return TOStoredAttr(*args, **kwargs)
 
 
 class TOObject(metaclass=TOObjectMeta):
-    def __init__(self, *args, **kwargs):
+    def __init__(self, **kwargs):
         super().__init__()
-        for arg, key in zip(args, self._to_attrs.keys()):
-            setattr(self, key, arg)
-        for key, value in kwargs.items():
-            setattr(self, key, value)
-        self.get_attr = self._to_attrs.get
+        self.__dict__.update(kwargs)
+
+    def get_attr(self, key):
+        return self._to_attrs.get(key)
 
     def iter_attrs(self):
         for key, value in self._to_attrs.items():
             yield key, value
 
     def iter_stored(self):
         for key, value in self.iter_attrs():
```

### Comparing `totolo-1.0/totolo/impl/entry.py` & `totolo-1.1/totolo/impl/entry.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 
 from .core import TOObject, a
 from .field import TOField
 
 
 class TOEntry(TOObject):
     name = a("")
-    fields = a(OrderedDict())
-    parents = a(set())
-    children = a(set())
-    source = a([])
+    fields = a(OrderedDict)
+    parents = a(set)
+    children = a(set)
+    source = a(list)
     source_location = a("<api>)")
-    ontology = a(lambda: None)
+    ontology = a(lambda: (lambda: None))
 
     def __lt__(self, other):
         return str(self) < str(other)
 
     def __hash__(self):
         return hash(self.name)
 
@@ -24,30 +24,31 @@
         return f"{name}[{len(self.fields)}]"
 
     def __getitem__(self, key):
         return self.get(key)
 
     def __setitem__(self, key, value):
         if isinstance(value, list):
-            value = TOField(
+            field = TOField(
                 name=key,
                 fieldtype="list",
                 source=value,
-                data=value,
                 parts=value
             )
-        elif not isinstance(value, TOField):
+        elif isinstance(value, TOField):
+            field = value
+        else:
             data = str(value)
-            value = TOField(
+            field = TOField(
                 name=key,
                 fieldtype="blob",
                 source=[data],
-                data=[data],
-                parts=[data])
-        self.fields[key] = value
+                parts=[data],
+            )
+        self.fields[key] = field.setup()
 
     def __delitem__(self, key):
         del self.fields[key]
 
     def iter_fields(self, reorder=False, skipunknown=False):
         if reorder:
             order = [fn for fn, _ in self.iter_stored()]
@@ -63,30 +64,47 @@
     def ancestors(self):
         yield from self._dfs("parents", self._lookup())
 
     def descendants(self):
         yield from self._dfs("children", self._lookup())
 
     def validate(self):
+        yield from self.validate_junklines()
+        yield from self.validate_fields()
+        yield from self.validate_keywords()
+
+    def validate_junklines(self):
         junklines = []
         for idx, line in enumerate(self.source):
             if idx > 1:
                 if line.startswith("::"):
                     break
                 if line.strip():
                     junklines.append(line)
         if junklines:
             junkmsg = '/'.join(junklines)
             if len(junkmsg) > 13:
                 junkmsg = junkmsg[:10] + "..."
             yield f"{self.name}: junk in entry header: {junkmsg}"
+
+    def validate_fields(self):
         for field in self.fields.values():
             if self.field_type(field.name) == "unknown":
                 yield f"{self.name}: unknown field '{field.name}'"
 
+    def validate_keywords(self):
+        from .parser import TOParser  # pylint: disable=cyclic-import
+        for field in self.fields.values():
+            if field.fieldtype == "kwlist":
+                data_iter = filter(None, (x.strip() for x in field.source[1:]))
+                try:
+                    list(TOParser.iter_kwitems_strict(data_iter))
+                except AssertionError as exc:
+                    yield f"In {self.name}: {exc.args[0]}"
+
     def text_canonical(self):
         lines = [self.name, "=" * len(self.name), ""]
         for field in self.iter_fields(reorder=True, skipunknown=True):
             if self.field_required(field.name) or not field.empty():
                 lines.append(field.text_canonical())
                 lines.append("")
         return "\n".join(lines)
```

### Comparing `totolo-1.0/totolo/impl/field.py` & `totolo-1.1/totolo/impl/field.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,109 +1,108 @@
+import totolo.lib.textformat
+
 from .core import TOObject, a
 from .keyword import TOKeyword
 
 
 class TOField(TOObject):
     name = a("")
     fieldtype = a("")
-    source = a([])
-    data = a([])
-    parts = a([])
+    source = a(list)
+    parts = a(list)
     frozen = a(False)
 
     def __setattr__(self, name, value):
         if name != "frozen":
-            self.assert_mutable()
+            self.mutable()
         super().__setattr__(name, value)
 
     def __repr__(self):
+        self.setup()
         tname = type(self).__name__
         name = self.name.encode("ascii", "ignore")
-        ndata = len(self.data)
+        ndata = len(self.parts)
         return f"{tname}<{name}>[{ndata}]"
 
     def __str__(self):
         return self.text_canonical_contents()
 
     def __iter__(self):
-        for part in self.iter_parts():
-            yield part
+        yield from self.setup().parts
 
     def freeze(self):
         if not self.frozen:
+            self.setup()
             self.source = tuple(self.source)
-            self.data = tuple(self.data)
             self.parts = tuple(self.parts)
             self.frozen = True
         return self
 
-    def assert_mutable(self):
+    def mutable(self):
         if getattr(self, "frozen", False):
             raise AttributeError(
                 "Object is frozen, indicating it is detached from an ontology.")
-        return True
+        return self
 
     def str(self):
         return str(self)
 
-    def list(self):
-        return list(self.parts)
-
     def empty(self):
-        return not any(self.parts)
-
-    def iter_parts(self):
-        for part in self.parts:
-            yield part
+        return not any(self.setup().parts)
 
     def text_canonical_contents(self):
-        parts = [str(x) for x in self.iter_parts()]
-        return "\n".join(parts)
+        text = "\n".join(str(x) for x in self)
+        if self.fieldtype == "text":
+            text = totolo.lib.textformat.add_wordwrap(text).strip()
+        return text
 
     def text_canonical(self):
         parts = [f":: {self.name}"]
-        parts.extend(str(x) for x in self.iter_parts())
+        parts.extend(str(x) for x in self)
         return "\n".join(parts)
 
     def text_original(self):
         return "\n".join(self.source)
 
     def delete_kw(self, keyword):
-        self.assert_mutable()
-        fieldtype = self.fieldtype
+        assert self.mutable().setup().fieldtype == "kwlist"
         todelete = set()
-        if fieldtype == "kwlist":
-            for idx, part in enumerate(self.parts):
-                if part.keyword == keyword:
-                    todelete.add(idx)
+        for idx, part in enumerate(self.parts):
+            if part.keyword == keyword:
+                todelete.add(idx)
         self.parts = [p for idx, p in enumerate(self.parts) if idx not in todelete]
         return len(todelete)
 
     def update_kw(self, match_keyword, keyword=None,
                   motivation=None, capacity=None, notes=None):
-        self.assert_mutable()
-        assert self.fieldtype == "kwlist"
+        assert self.mutable().setup().fieldtype == "kwlist"
         for part in self.parts:
             if part.keyword == match_keyword:
                 if keyword is not None:
                     part.keyword = keyword
                 if motivation is not None:
                     part.motivation = motivation
                 if capacity is not None:
                     part.capacity = capacity
                 if notes is not None:
                     part.notes = notes
 
     def insert_kw(self, idx=None, keyword="", motivation="", capacity="", notes=""):
-        self.assert_mutable()
-        assert self.fieldtype == "kwlist"
+        assert self.mutable().setup().fieldtype == "kwlist"
         if idx is None:
             idx = len(self.parts)
         self.parts.insert(
             idx,
             TOKeyword(
                 keyword,
                 capacity=capacity,
                 motivation=motivation,
                 notes=notes
             )
         )
+
+    def setup(self):
+        if not self.parts and not self.frozen:
+            # this used to be done immediately but is now defered for efficiency
+            from .parser import TOParser  # pylint: disable=cyclic-import
+            TOParser.init_field(self)
+        return self
```

### Comparing `totolo-1.0/totolo/impl/parser.py` & `totolo-1.1/totolo/impl/parser.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 import os
 import re
 import weakref
+from itertools import islice
 from typing import Generator, Iterable, List, Tuple
 
 import totolo.lib.files
 import totolo.lib.textformat
 
 from ..story import TOStory
 from ..theme import TOTheme
 from .field import TOField
 from .keyword import TOKeyword
 
+G = r"[^\(\)\{\}\[\]]"
+KW_PATTERN = re.compile("([\\[\\]\\{\\}\\<\\>\\n])")
+KW_PATTERN2 = re.compile(f"(^{G}*|\\<{G}*\\>|\\[{G}*\\]|{{{G}*\\}})")
+
 
 class TOParser:
     @staticmethod
     def iter_entries(lines: Iterable[str]) -> Generator[str, None, None]:
         """
         Iterate through the "entries" in a text file. An entry is a block of lines
         that starts with a title line, followed by a line starting with "===".
@@ -44,97 +49,109 @@
                 linebuffer = [line]
             elif linebuffer:
                 linebuffer.append(line)
         if linebuffer:
             yield linebuffer
 
     @staticmethod
-    def iter_listitems(lines: Iterable[str]) -> str:
+    def iter_kwitems(
+        lines: Iterable[str]
+    ) -> Generator[Tuple[str, str, str, str], None, None]:
         """
-        Turn a list of strings into items. Items may be newline or comma separated.
+        Turn a list of strings into kewyword items.
+        Items are un-enclosed newline character separated.
+        Items may contain data in () [] {} parentheses.
+        Parantheses may not contain newline characters (once they might).
+
+        This is one of the most time consuming passages in parsing a large ontology.
         """
+        brackets = "<[{"
         for line in lines:
-            # note: once upon a time we used to have multiple items separated by commas
-            # on a single line but that is no longer permitted.
-            item = line.strip()
-            if item:
-                yield item
+            row = ["", "", "", ""]
+            parts = KW_PATTERN2.findall(line)
+            for part in parts:
+                if part:
+                    try:
+                        idx = brackets.index(part[0])
+                        row[idx + 1] = part[1:-1].strip()
+                    except ValueError:
+                        row[0] = part.strip()
+            if row[0]:
+                yield row
 
     @staticmethod
-    def iter_kwitems(
+    def iter_kwitems_strict(
         lines: Iterable[str]
     ) -> Generator[Tuple[str, str, str, str], None, None]:
         """
-        Turn a list of strings into kewyword items. Items may be newline or comma
-        separated. Items may contain data in () [] {} parentheses.
+        Turn a list of strings into kewyword items.
+        Items are un-enclosed newline character separated.
+        Items may contain data in () [] {} parentheses.
+        Parantheses may contain newline characters.
+
+        This is one of the most time consuming passages in parsing a large ontology.
         """
-        def dict2row(tokendict):
-            tkw = tokendict.get("", "").strip()
-            tmotivation = tokendict.get("[", "").strip()
-            tcapacity = tokendict.get("<", "").strip()
-            tnotes = tokendict.get("{", "").strip()
-            return tkw, tcapacity, tmotivation, tnotes
-
-        field = "\n".join(lines)
-        token = {}
-        delcorr = {"[": "]", "{": "}", "<": ">"}
-        farr = re.split("([\\[\\]\\{\\}\\<\\>,\\n])", field)
-        state = ""
-        splitters = ",\n"
-
-        for part in farr:
-            if part in delcorr:
-                state = part
-            elif part in delcorr.values():
-                if delcorr.get(state, None) == part:
-                    state = ""
-                else:
-                    raise AssertionError(
-                        f"Malformed field (bracket mismatch):\n {field}"
-                    )
-            elif part in splitters and not state:
-                tokrow = dict2row(token)
-                if not tokrow[0].strip():
-                    pass  # we allow splitting by both newline and comma
+        ramp = " <[{>]}"
+        for line in lines:
+            field_array = KW_PATTERN.split(line)
+            state_idx = 0
+            close_bracket = ""
+            acc = []
+            row = ["", "", "", ""]
+
+            for part in field_array:
+                if len(part) == 1 and part in ramp:
+                    row[state_idx] += "".join(acc)
+                    acc = []
+                    if part == close_bracket:
+                        state_idx = 0
+                        close_bracket = ""
+                    elif close_bracket:
+                        raise AssertionError(f"Missing '{close_bracket}' in: {row}")
+                    else:
+                        state_idx = ramp.index(part)
+                        if state_idx > 3:
+                            raise AssertionError(f"Unexpected {part} in: {row}")
+                        close_bracket = ramp[state_idx + 3]
                 else:
-                    yield tokrow
-                token = {}
-            else:
-                token[state] = token.get(state, "") + part
+                    acc.append(part)
+
+            row[state_idx] += "".join(acc)
+            if row[0]:
+                yield tuple(x.strip() for x in row)
 
     @classmethod
     def make_field(cls, lines, fieldtype):
-        field = TOField(
+        return TOField(
             fieldtype=fieldtype,
             name=lines[0].strip(": "),
-            data=[line.strip() for line in lines[1:] if line.strip()],
             source=list(lines),
         )
+
+    @classmethod
+    def init_field(cls, field):
+        fieldtype = field.fieldtype
         if fieldtype == "kwlist":
-            for kwtuple in TOParser.iter_kwitems(field.data):
+            data_iter = islice(field.source, 1, 1000)
+            for kwtuple in TOParser.iter_kwitems(data_iter):
                 field.parts.append(TOKeyword(*kwtuple))
         elif fieldtype == "list":
-            for item in TOParser.iter_listitems(field.data):
-                field.parts.append(item)
+            data_iter = filter(None, islice(field.source, 1, 1000))
+            field.parts.extend(data_iter)
         elif fieldtype == "text":
-            field.parts.append(
-                totolo.lib.textformat.add_wordwrap(
-                    "\n".join(field.data)).strip()
-            )
-        else:  # date/ blob
-            field.parts.append('\n'.join(field.data))
+            field.parts.append("\n".join(field.source[1:]).strip())
+        else:  # for datatype "date" and  "blob"
+            field.parts.append('\n'.join(field.source[1:]).strip())
         return field
 
     @classmethod
     def populate_entry(cls, entry, lines):
         entry.source.extend(lines)
-        cleaned = [line.strip() for line in lines]
-        assert len(cleaned) > 1 and cleaned[1].startswith("==="), "missing name"
-        entry.name = cleaned[0]
-        for fieldlines in cls.iter_fields(cleaned):
+        entry.name = lines[0]
+        for fieldlines in cls.iter_fields(lines):
             name = fieldlines[0].strip(": ")
             fieldtype = entry.field_type(name)
             field = cls.make_field(fieldlines, fieldtype)
             entry[field.name] = field
         return entry
 
     @classmethod
```

### Comparing `totolo-1.0/totolo/lib/files.py` & `totolo-1.1/totolo/lib/files.py`

 * *Files identical despite different names*

### Comparing `totolo-1.0/totolo/lib/textformat.py` & `totolo-1.1/totolo/lib/textformat.py`

 * *Files identical despite different names*

### Comparing `totolo-1.0/totolo/story.py` & `totolo-1.1/totolo/story.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,17 +25,16 @@
     def iter_theme_entries(self):
         """
         Yield (weight, TOKeyword) pairs. TOKeyword contains the comment and other
         metadata associated with a theme entry in a story.
         """
         for weight in ["Choice Themes", "Major Themes", "Minor Themes", "Not Themes"]:
             field = self.get(weight)
-            if field:
-                for part in field.iter_parts():
-                    yield weight, part
+            for part in field or ():
+                yield weight, part
 
     def iter_themes(self):
         """
         Iterate over the theme objects associated with this story object.
         """
         ontology = self.ontology()
         if ontology is None:
```

### Comparing `totolo-1.0/totolo/theme.py` & `totolo-1.1/totolo/theme.py`

 * *Files identical despite different names*

### Comparing `totolo-1.0/totolo/themeontology.py` & `totolo-1.1/totolo/themeontology.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,18 +7,18 @@
 
 
 class TODict(dict):
     pass
 
 
 class ThemeOntology(TOObject):
-    theme = a(TODict())
-    story = a(TODict())
-    entries = a({})
-    basepaths = a(set())
+    theme = a(TODict)
+    story = a(TODict)
+    entries = a(dict)
+    basepaths = a(set)
 
     def __len__(self):
         return sum(len(v) for v in self.entries.values())
 
     def __str__(self):
         return f"<{len(self.theme)} themes, {len(self.story)} stories>"
 
@@ -33,15 +33,15 @@
     def astory(self):
         return random.sample(list(self.story.values()), 1)[0]
 
     def atheme(self):
         return random.sample(list(self.theme.values()), 1)[0]
 
     def dataframe(self, implied_themes=True):
-        import pandas as pd  # pylint: disable=C0415
+        import pandas as pd
         data = []
         for story in self.stories():
             for weight, part in story.iter_theme_entries():
                 themes = [part.keyword]
                 if implied_themes and part.keyword in self.theme:
                     theme = self.theme[part.keyword]
                     themes.extend(theme.ancestors())
@@ -163,16 +163,17 @@
         if not os.path.exists(dirname):
             os.makedirs(dirname)
         with open(path, "w", encoding='utf-8') as fhandle:
             sids = set(e.name for e in entries)
             for idx, entry in enumerate(entries):
                 if idx == 0 and entry.name in entry["Collections"]:
                     field = entry.get(cskey)
-                    parts = [x for x in field.parts if x not in sids]
-                    if parts != field.parts:
+                    all_parts = list(field)
+                    parts = [x for x in all_parts if x not in sids]
+                    if parts != all_parts:
                         entry = copy.deepcopy(entry)
                         if parts:
                             field = entry.setdefault(cskey)
                             field.parts = parts
                         else:
                             entry.delete(cskey)
                 lines = entry.text_canonical() if cleaned else entry.text_original()
```

### Comparing `totolo-1.0/PKG-INFO` & `totolo-1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: totolo
-Version: 1.0
+Version: 1.1
 Summary: The Python interface to themeontology.org.
 Author-email: Mikael Onsjö <mikael@odinlake.net>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Project-URL: Documentation, https://github.com/theme-ontology/theming
 Project-URL: Home, https://www.themeontology.org/
 Project-URL: Source, https://github.com/theme-ontology/python-totolo
```

