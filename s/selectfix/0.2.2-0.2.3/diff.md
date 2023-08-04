# Comparing `tmp/selectfix-0.2.2.tar.gz` & `tmp/selectfix-0.2.3.tar.gz`

## Comparing `selectfix-0.2.2.tar` & `selectfix-0.2.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      438 1970-01-01 00:00:00.000000 selectfix-0.2.2/Cargo.toml
--rw-r--r--   0     1001      123     1272 2023-07-14 06:46:14.000000 selectfix-0.2.2/.github/workflows/CI.yml
--rw-r--r--   0     1001      123     1046 2023-07-14 06:46:14.000000 selectfix-0.2.2/.github/workflows/_workflow.yml
--rw-r--r--   0     1001      123      685 2023-07-14 06:46:14.000000 selectfix-0.2.2/.gitignore
--rw-r--r--   0     1001      123      125 2023-07-14 06:46:14.000000 selectfix-0.2.2/README.md
--rw-r--r--   0     1001      123      313 2023-07-14 06:46:14.000000 selectfix-0.2.2/pyproject.toml
--rw-r--r--   0     1001      123     8854 2023-07-14 06:46:14.000000 selectfix-0.2.2/src/lib.rs
--rw-r--r--   0     1001      123        0 2023-07-14 06:46:14.000000 selectfix-0.2.2/tests/__init__.py
--rw-r--r--   0     1001      123     2893 2023-07-14 06:46:14.000000 selectfix-0.2.2/tests/test_selectfix.py
--rw-r--r--   0     1001      123     8559 2023-07-14 06:46:14.000000 selectfix-0.2.2/Cargo.lock
--rw-r--r--   0        0        0      453 1970-01-01 00:00:00.000000 selectfix-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0      438 1970-01-01 00:00:00.000000 selectfix-0.2.3/Cargo.toml
+-rw-r--r--   0     1001      123     1272 2023-08-04 02:22:20.000000 selectfix-0.2.3/.github/workflows/CI.yml
+-rw-r--r--   0     1001      123     1046 2023-08-04 02:22:20.000000 selectfix-0.2.3/.github/workflows/_workflow.yml
+-rw-r--r--   0     1001      123      685 2023-08-04 02:22:20.000000 selectfix-0.2.3/.gitignore
+-rw-r--r--   0     1001      123      125 2023-08-04 02:22:20.000000 selectfix-0.2.3/README.md
+-rw-r--r--   0     1001      123      313 2023-08-04 02:22:20.000000 selectfix-0.2.3/pyproject.toml
+-rw-r--r--   0     1001      123    12925 2023-08-04 02:22:20.000000 selectfix-0.2.3/src/lib.rs
+-rw-r--r--   0     1001      123        0 2023-08-04 02:22:20.000000 selectfix-0.2.3/tests/__init__.py
+-rw-r--r--   0     1001      123     3281 2023-08-04 02:22:20.000000 selectfix-0.2.3/tests/test_selectfix.py
+-rw-r--r--   0     1001      123     8559 2023-08-04 02:22:20.000000 selectfix-0.2.3/Cargo.lock
+-rw-r--r--   0        0        0      453 1970-01-01 00:00:00.000000 selectfix-0.2.3/PKG-INFO
```

### Comparing `selectfix-0.2.2/.github/workflows/CI.yml` & `selectfix-0.2.3/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `selectfix-0.2.2/.github/workflows/_workflow.yml` & `selectfix-0.2.3/.github/workflows/_workflow.yml`

 * *Files identical despite different names*

### Comparing `selectfix-0.2.2/.gitignore` & `selectfix-0.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `selectfix-0.2.2/tests/test_selectfix.py` & `selectfix-0.2.3/tests/test_selectfix.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,59 +2,64 @@
 
 import numpy as np
 
 import selectfix
 
 class TestSelectfix(unittest.TestCase):
     def test_selectfix_basic(self):
-        sel = selectfix.Selector(2, [], [], 0.0, {}, 0.0)
+        sel = selectfix.Selector(2, [], [], 0.0, {}, None, 0.0)
         val = sel({"x1": 10, "x2": 10, "x3": 0, "x4": 0})
         assert val == 0
         val = sel({"x1": 10, "x2": 10, "x3": 10, "x4": 0})
         assert val == -10
         val = sel({"x1": 10, "x2": 10, "x3": 10, "x4": 10})
         assert val == -20
 
     def test_selectfix_jacobian(self):
-        sel = selectfix.Selector(1, ["x1", "x2", "x3"], [], 0.0, {}, 0.0)
+        sel = selectfix.Selector(1, ["x1", "x2", "x3"], [], 0.0, {}, None, 0.0)
         val = sel({"x1": 10, "x2": 10, "x3": 0, "x4": 0})
         assert val == 0
         val = sel({"x1": 10, "x2": 10, "x3": 10, "x4": 0})
         assert val == -10
         val = sel({"x1": 10, "x2": 10, "x3": 10, "x4": 10})
         assert val == -10
         np.testing.assert_array_equal(sel.jacobian({"x1": 10, "x2": 10, "x3": 10, "x4": 0}), np.array([0, 0, 1, 0]))
         np.testing.assert_array_equal(sel.jacobian({"x1": 10, "x2": 10, "x3": 0, "x4": 0}), np.array([0, 0, 1, 0]))
         np.testing.assert_array_equal(sel.hessian({"x1": 10, "x2": 10, "x3": 0, "x4": 0}), np.zeros((4, 4)))
 
-    def test_selectfix_using_exclude_free(self):
-        sel = selectfix.Selector(1, ["x1", "x2", "x3"], [["x1", "x2"]], 0.0, {}, 0.0)
+    def test_selectfix_using_excluded_unfixed_combinations(self):
+        sel = selectfix.Selector(1, ["x1", "x2", "x3"], [["x1", "x2"]], 0.0, {}, None, 0.0)
         val = sel({"x1": 10, "x2": 10, "x3": 0, "x4": 0})
         assert val == -10
         np.testing.assert_array_equal(sel.jacobian({"x1": 10, "x2": 10, "x3": 0, "x4": 0}), np.array([0, 1, 0, 0]))
         np.testing.assert_array_equal(sel.hessian({"x1": 10, "x2": 10, "x3": 0, "x4": 0}), np.zeros((4, 4)))
 
-        sel = selectfix.Selector(1, ["x1", "x2", "x3"], [["x1", "x2"], ["x2", "x3"]], 0.0, {}, 0.0)
+        sel = selectfix.Selector(1, ["x1", "x2", "x3"], [["x1", "x2"], ["x2", "x3"]], 0.0, {}, None, 0.0)
         val = sel({"x1": 10, "x2": 11, "x3": 12, "x4": 0})
         assert val == -11
         np.testing.assert_array_equal(sel.jacobian({"x1": 10, "x2": 10, "x3": 0, "x4": 0}), np.array([0, 1, 0, 0]))
         np.testing.assert_array_equal(sel.hessian({"x1": 10, "x2": 10, "x3": 0, "x4": 0}), np.zeros((4, 4)))
 
         sel = selectfix.Selector(
-            2, ["x1", "x2", "x3", "x4", "x5"], [["x1", "x2"], ["x1", "x3"], ["x1", "x4"]], 0.0, {}, 0.0
+            2, ["x1", "x2", "x3", "x4", "x5"], [["x1", "x2"], ["x1", "x3"], ["x1", "x4"]], 0.0, {}, None, 0.0
         )
         val = sel({"x1": 14, "x2": 13, "x3": 12, "x4": 11, "x5": 10})
         assert val == -24
         np.testing.assert_array_equal(
             sel.jacobian({"x1": 14, "x2": 13, "x3": 12, "x4": 11, "x5": 10}), np.array([1, 0, 0, 0, 1])
         )
         np.testing.assert_array_equal(sel.hessian({"x1": 14, "x2": 13, "x3": 12, "x4": 11, "x5": 10}), np.zeros((5, 5)))
 
     def test_selectfix_using_range_penalty(self):
-        sel = selectfix.Selector(1, ["x1", "x2", "x3"], [], 0.0, {"x1": (20, 30)}, 0.0)
+        sel = selectfix.Selector(1, ["x1", "x2", "x3"], [], 0.0, {"x1": (20, 30)}, None, 0.0)
         val = sel({"x1": 10, "x2": 10, "x3": 0})
         assert val == -10
         np.testing.assert_array_equal(sel.jacobian({"x1": 10, "x2": 10, "x3": 0}), np.array([1, 0, 1]))
 
+    def test_selectfix_using_range_penalty_and_n_select_max(self):
+        sel = selectfix.Selector(1, ["x1", "x2", "x3"], [], 0.0, {"x1": (20, 30)}, 2, 0.0)
+        val = sel({"x1": 10, "x2": 10, "x3": 0})
+        assert val == 0
+        np.testing.assert_array_equal(sel.jacobian({"x1": 10, "x2": 10, "x3": 0}), np.array([0, 0, 1]))
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `selectfix-0.2.2/Cargo.lock` & `selectfix-0.2.3/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -211,15 +211,15 @@
 name = "scopeguard"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
 
 [[package]]
 name = "selectfix"
-version = "0.2.2"
+version = "0.2.3"
 dependencies = [
  "anyhow",
  "bincode",
  "indexmap",
  "ordered-float",
  "pyo3",
  "serde",
```

