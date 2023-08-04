# Comparing `tmp/pycln-2.2.0.tar.gz` & `tmp/pycln-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycln-2.2.0.tar", max compression
+gzip compressed data, was "pycln-2.2.1.tar", max compression
```

## Comparing `pycln-2.2.0.tar` & `pycln-2.2.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1099 2023-01-16 09:14:47.289812 pycln-2.2.0/LICENSE
--rw-r--r--   0        0        0     7370 2023-05-31 14:51:44.454169 pycln-2.2.0/README.md
--rw-r--r--   0        0        0     1160 2023-01-16 09:14:47.309812 pycln-2.2.0/pycln/__init__.py
--rw-r--r--   0        0        0      113 2023-01-16 09:14:47.309812 pycln-2.2.0/pycln/__main__.py
--rw-r--r--   0        0        0     6828 2023-01-16 09:14:47.309812 pycln-2.2.0/pycln/cli.py
--rw-r--r--   0        0        0       26 2023-01-16 09:14:47.309812 pycln-2.2.0/pycln/utils/__init__.py
--rw-r--r--   0        0        0     3192 2023-01-16 09:14:47.309812 pycln-2.2.0/pycln/utils/_exceptions.py
--rw-r--r--   0        0        0     1813 2023-01-16 09:14:47.309812 pycln-2.2.0/pycln/utils/_nodes.py
--rw-r--r--   0        0        0     7477 2023-05-26 13:19:42.548063 pycln-2.2.0/pycln/utils/config.py
--rw-r--r--   0        0        0     3908 2023-05-31 14:51:44.464169 pycln-2.2.0/pycln/utils/iou.py
--rw-r--r--   0        0        0    12640 2023-05-31 14:51:44.464169 pycln-2.2.0/pycln/utils/pathu.py
--rw-r--r--   0        0        0    21013 2023-07-19 15:43:44.529950 pycln-2.2.0/pycln/utils/refactor.py
--rw-r--r--   0        0        0     4138 2023-01-16 09:14:47.309812 pycln-2.2.0/pycln/utils/regexu.py
--rw-r--r--   0        0        0    18739 2023-01-16 09:14:47.309812 pycln-2.2.0/pycln/utils/report.py
--rw-r--r--   0        0        0    35157 2023-07-27 12:47:16.416601 pycln-2.2.0/pycln/utils/scan.py
--rw-r--r--   0        0        0     8055 2023-01-16 13:00:31.890686 pycln-2.2.0/pycln/utils/transform.py
--rw-r--r--   0        0        0     1776 2023-07-31 15:33:30.490746 pycln-2.2.0/pyproject.toml
--rw-r--r--   0        0        0       66 2023-01-16 09:14:47.329812 pycln-2.2.0/vendor/custom/__init__.py
--rw-r--r--   0        0        0     2018 2023-01-16 09:14:47.329812 pycln-2.2.0/vendor/custom/_site.py
--rw-r--r--   0        0        0     8599 1970-01-01 00:00:00.000000 pycln-2.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1099 2023-01-16 09:14:47.289812 pycln-2.2.1/LICENSE
+-rw-r--r--   0        0        0     7370 2023-05-31 14:51:44.454169 pycln-2.2.1/README.md
+-rw-r--r--   0        0        0     1160 2023-01-16 09:14:47.309812 pycln-2.2.1/pycln/__init__.py
+-rw-r--r--   0        0        0      113 2023-01-16 09:14:47.309812 pycln-2.2.1/pycln/__main__.py
+-rw-r--r--   0        0        0     6828 2023-08-04 09:55:30.838772 pycln-2.2.1/pycln/cli.py
+-rw-r--r--   0        0        0       26 2023-01-16 09:14:47.309812 pycln-2.2.1/pycln/utils/__init__.py
+-rw-r--r--   0        0        0     3330 2023-08-04 19:30:57.841191 pycln-2.2.1/pycln/utils/_exceptions.py
+-rw-r--r--   0        0        0     1813 2023-01-16 09:14:47.309812 pycln-2.2.1/pycln/utils/_nodes.py
+-rw-r--r--   0        0        0     7477 2023-05-26 13:19:42.548063 pycln-2.2.1/pycln/utils/config.py
+-rw-r--r--   0        0        0     4290 2023-08-04 19:30:57.841191 pycln-2.2.1/pycln/utils/iou.py
+-rw-r--r--   0        0        0    12640 2023-05-31 14:51:44.464169 pycln-2.2.1/pycln/utils/pathu.py
+-rw-r--r--   0        0        0    21103 2023-08-04 19:30:57.841191 pycln-2.2.1/pycln/utils/refactor.py
+-rw-r--r--   0        0        0     4138 2023-01-16 09:14:47.309812 pycln-2.2.1/pycln/utils/regexu.py
+-rw-r--r--   0        0        0    18739 2023-01-16 09:14:47.309812 pycln-2.2.1/pycln/utils/report.py
+-rw-r--r--   0        0        0    35157 2023-07-27 12:47:16.416601 pycln-2.2.1/pycln/utils/scan.py
+-rw-r--r--   0        0        0     8055 2023-01-16 13:00:31.890686 pycln-2.2.1/pycln/utils/transform.py
+-rw-r--r--   0        0        0     1776 2023-08-04 19:30:57.841191 pycln-2.2.1/pyproject.toml
+-rw-r--r--   0        0        0       66 2023-01-16 09:14:47.329812 pycln-2.2.1/vendor/custom/__init__.py
+-rw-r--r--   0        0        0     2018 2023-01-16 09:14:47.329812 pycln-2.2.1/vendor/custom/_site.py
+-rw-r--r--   0        0        0     8599 1970-01-01 00:00:00.000000 pycln-2.2.1/PKG-INFO
```

### Comparing `pycln-2.2.0/LICENSE` & `pycln-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pycln-2.2.0/README.md` & `pycln-2.2.1/README.md`

 * *Files identical despite different names*

### Comparing `pycln-2.2.0/pycln/__init__.py` & `pycln-2.2.1/pycln/__init__.py`

 * *Files identical despite different names*

### Comparing `pycln-2.2.0/pycln/cli.py` & `pycln-2.2.1/pycln/cli.py`

 * *Files identical despite different names*

### Comparing `pycln-2.2.0/pycln/utils/_exceptions.py` & `pycln-2.2.1/pycln/utils/_exceptions.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,14 +20,20 @@
 
 
 class WritePermissionError(BaseOSError):
 
     """Raises when the file does not have write permission."""
 
 
+class InitFileDoesNotExistError(BaseOSError):
+
+    """Raises when an `__init__.py` file path encountered of a non-existing
+    path."""
+
+
 class UnexpandableImportStar(Exception):
 
     """Raises when the import `*` statement unexpandable."""
 
     def __init__(self, path: Path, location: NodeLocation, msg: str):
         line, col = location.start.line, location.start.col
         message = f"{path}:{line}:{col} {self.__class__.__name__}: {msg}"
```

### Comparing `pycln-2.2.0/pycln/utils/_nodes.py` & `pycln-2.2.1/pycln/utils/_nodes.py`

 * *Files identical despite different names*

### Comparing `pycln-2.2.0/pycln/utils/config.py` & `pycln-2.2.1/pycln/utils/config.py`

 * *Files identical despite different names*

### Comparing `pycln-2.2.0/pycln/utils/iou.py` & `pycln-2.2.1/pycln/utils/iou.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,22 +2,28 @@
 import io
 import os
 import sys
 import tokenize
 from pathlib import Path
 from typing import List, Tuple
 
-from ._exceptions import ReadPermissionError, UnparsableFile, WritePermissionError
+from ._exceptions import (
+    InitFileDoesNotExistError,
+    ReadPermissionError,
+    UnparsableFile,
+    WritePermissionError,
+)
 
 # Constants.
 STDIN_FILE = Path("STDIN")
 STDIN_NOTATION = Path("-")
 FORM_FEED_CHAR = "\x0c"
 CRLF = "\r\n"
 LF = "\n"
+__INIT__ = "__init__.py"
 
 # Types
 FileContent = str
 Encoding = str
 NewLine = str
 
 
@@ -57,15 +63,21 @@
     :returns: decoded source code, file encoding, and a newline.
     :raises ReadPermissionError: when `os.R_OK` in permissions
         and the source does not have read permission.
     :raises WritePermissionError: when `os.W_OK` in permissions
         and the source does not have write permission.
     :raises UnparsableFile: If both a BOM and a cookie are present, but disagree.
         or some rare characters presented.
+    :raises InitFileDoesNotExistError: when `path` is a path to a non-existing
+        `__init__.py` file.
     """
+    # Check for a non-existing `__init__.py` file case.
+    if str(path).endswith(__INIT__) and not path.exists():
+        raise InitFileDoesNotExistError(2, "`__init__.py` file does not exist", path)
+
     # Check these permissions before openinig the file.
     for permission in permissions:
         if not os.access(path, permission):
             if permission is os.R_OK:
                 raise ReadPermissionError(13, "Permission denied [READ]", path)
             elif permission is os.W_OK:
                 raise WritePermissionError(13, "Permission denied [WRITE]", path)
```

### Comparing `pycln-2.2.0/pycln/utils/pathu.py` & `pycln-2.2.1/pycln/utils/pathu.py`

 * *Files identical despite different names*

### Comparing `pycln-2.2.0/pycln/utils/refactor.py` & `pycln-2.2.1/pycln/utils/refactor.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from importlib import import_module
 from pathlib import Path, _posix_flavour, _windows_flavour  # type: ignore
 from typing import Iterable, List, Optional, Set, Tuple, Union, cast
 
 from .. import ISWIN
 from . import iou, pathu, regexu, scan
 from ._exceptions import (
+    InitFileDoesNotExistError,
     ReadPermissionError,
     UnexpandableImportStar,
     UnparsableFile,
     UnsupportedCase,
     WritePermissionError,
     libcst_parser_syntax_error_message,
 )
@@ -171,14 +172,16 @@
             self._output(fixed_lines, content.splitlines(True), encoding, newline)
         except (
             ReadPermissionError,
             WritePermissionError,
             UnparsableFile,
         ) as err:
             self.reporter.failure(str(err))
+        except InitFileDoesNotExistError:
+            pass
         finally:
             self._reset()
 
     def _code_session(self, source_code: str) -> str:
         """Refactor the given `source_code`.
 
         :param source_code: python source code.
```

### Comparing `pycln-2.2.0/pycln/utils/regexu.py` & `pycln-2.2.1/pycln/utils/regexu.py`

 * *Files identical despite different names*

### Comparing `pycln-2.2.0/pycln/utils/report.py` & `pycln-2.2.1/pycln/utils/report.py`

 * *Files identical despite different names*

### Comparing `pycln-2.2.0/pycln/utils/scan.py` & `pycln-2.2.1/pycln/utils/scan.py`

 * *Files identical despite different names*

### Comparing `pycln-2.2.0/pycln/utils/transform.py` & `pycln-2.2.1/pycln/utils/transform.py`

 * *Files identical despite different names*

### Comparing `pycln-2.2.0/pyproject.toml` & `pycln-2.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pycln"
-version = "2.2.0"
+version = "2.2.1"
 description = "A formatter for finding and removing unused import statements."
 authors = ["Hadi Alqattan <alqattanhadizaki@gmail.com>"]
 homepage = "https://hadialqattan.github.io/pycln"
 repository = "https://github.com/hadialqattan/pycln"
 keywords = ["formatter", "linter", "quality-assurance", "tools", "cli"]
 classifiers = [
     "License :: OSI Approved :: MIT License",
```

### Comparing `pycln-2.2.0/vendor/custom/_site.py` & `pycln-2.2.1/vendor/custom/_site.py`

 * *Files identical despite different names*

### Comparing `pycln-2.2.0/PKG-INFO` & `pycln-2.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycln
-Version: 2.2.0
+Version: 2.2.1
 Summary: A formatter for finding and removing unused import statements.
 Home-page: https://hadialqattan.github.io/pycln
 License: MIT
 Keywords: formatter,linter,quality-assurance,tools,cli
 Author: Hadi Alqattan
 Author-email: alqattanhadizaki@gmail.com
 Requires-Python: >=3.6.2,<4
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pycln Version: 2.2.0 Summary: A formatter for
+Metadata-Version: 2.1 Name: pycln Version: 2.2.1 Summary: A formatter for
 finding and removing unused import statements. Home-page: https://
 hadialqattan.github.io/pycln License: MIT Keywords: formatter,linter,quality-
 assurance,tools,cli Author: Hadi Alqattan Author-email:
 alqattanhadizaki@gmail.com Requires-Python: >=3.6.2,<4 Classifier: License ::
 OSI Approved :: MIT License Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
```

