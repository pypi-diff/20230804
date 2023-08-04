# Comparing `tmp/pam_tester-0.0.2.tar.gz` & `tmp/pam_tester-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pam_tester-0.0.2.tar", max compression
+gzip compressed data, was "pam_tester-0.0.3.tar", max compression
```

## Comparing `pam_tester-0.0.2.tar` & `pam_tester-0.0.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     2479 2023-08-01 16:04:09.646705 pam_tester-0.0.2/README.md
--rw-r--r--   0        0        0        0 2023-08-01 16:04:09.646705 pam_tester-0.0.2/pam_tester/__init__.py
--rw-r--r--   0        0        0     1221 2023-08-01 16:04:09.646705 pam_tester-0.0.2/pam_tester/pam_tester.py
--rw-r--r--   0        0        0      854 2023-08-01 16:04:09.646705 pam_tester-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     3534 1970-01-01 00:00:00.000000 pam_tester-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     2479 2023-08-04 14:42:32.261146 pam_tester-0.0.3/README.md
+-rw-r--r--   0        0        0        0 2023-08-04 14:42:32.261146 pam_tester-0.0.3/pam_tester/__init__.py
+-rw-r--r--   0        0        0     1264 2023-08-04 14:42:32.261146 pam_tester-0.0.3/pam_tester/pam_tester.py
+-rw-r--r--   0        0        0      854 2023-08-04 14:42:32.261146 pam_tester-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     3534 1970-01-01 00:00:00.000000 pam_tester-0.0.3/PKG-INFO
```

### Comparing `pam_tester-0.0.2/README.md` & `pam_tester-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pam_tester-0.0.2/pam_tester/pam_tester.py` & `pam_tester-0.0.3/pam_tester/pam_tester.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,7 +31,10 @@
     # no error (false) and it errors (true) -> not false and true -> true
     # no error (false) and it does not error (false) -> not false and false -> false
     # an error (true) and it errors (true) -> not true and true -> false
     # an error (true) and it does not error (false) -> not true and false -> false
     if (not expectfail and failed) or (expectfail and not failed):
         sys.exit(1)
     sys.exit(0)
+
+if __name__ == "__main__":
+    pam_auth()
```

### Comparing `pam_tester-0.0.2/pyproject.toml` & `pam_tester-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pam-tester"
-version = "0.0.2"
+version = "0.0.3"
 description = "Tool for testing PAM configurations"
 readme = "README.md"
 authors = ["Martin Schurz <Martin.Schurz@telekom.de>"]
 license = "GPL-3.0-only"
 homepage = "https://github.com/dev-sec/pam-tester"
 repository = "https://github.com/dev-sec/pam-tester"
 documentation = "https://github.com/dev-sec/pam-tester"
```

### Comparing `pam_tester-0.0.2/PKG-INFO` & `pam_tester-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pam-tester
-Version: 0.0.2
+Version: 0.0.3
 Summary: Tool for testing PAM configurations
 Home-page: https://github.com/dev-sec/pam-tester
 License: GPL-3.0-only
 Author: Martin Schurz
 Author-email: Martin.Schurz@telekom.de
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

