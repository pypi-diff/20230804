# Comparing `tmp/numbers_parser-4.3.0.tar.gz` & `tmp/numbers_parser-4.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "numbers_parser-4.3.0.tar", max compression
+gzip compressed data, was "numbers_parser-4.4.0.tar", max compression
```

## Comparing `numbers_parser-4.3.0.tar` & `numbers_parser-4.4.0.tar`

### file list

```diff
@@ -1,57 +1,57 @@
--rw-r--r--   0        0        0     1050 2022-06-23 17:13:17.000000 numbers_parser-4.3.0/LICENSE.rst
--rw-r--r--   0        0        0    23133 2023-08-02 18:06:36.519270 numbers_parser-4.3.0/README.md
--rw-r--r--   0        0        0     2130 2023-08-02 18:04:07.008254 numbers_parser-4.3.0/pyproject.toml
--rw-r--r--   0        0        0     2081 2023-07-23 15:54:51.138965 numbers_parser-4.3.0/src/numbers_parser/__init__.py
--rw-r--r--   0        0        0     4336 2023-08-02 13:30:28.000000 numbers_parser-4.3.0/src/numbers_parser/_cat_numbers.py
--rw-r--r--   0        0        0     5784 2023-07-23 15:54:51.177251 numbers_parser-4.3.0/src/numbers_parser/_unpack_numbers.py
--rw-r--r--   0        0        0     2616 2023-05-20 02:42:59.000000 numbers_parser-4.3.0/src/numbers_parser/bullets.py
--rw-r--r--   0        0        0    24971 2023-08-02 17:34:50.770915 numbers_parser-4.3.0/src/numbers_parser/cell.py
--rw-r--r--   0        0        0    28441 2023-08-02 17:30:54.921525 numbers_parser-4.3.0/src/numbers_parser/cell_storage.py
--rw-r--r--   0        0        0     1875 2023-08-02 06:59:20.616439 numbers_parser-4.3.0/src/numbers_parser/constants.py
--rw-r--r--   0        0        0     4239 2023-07-14 19:05:10.687308 numbers_parser-4.3.0/src/numbers_parser/containers.py
--rwxr-xr-x   0        0        0    90316 2023-07-31 12:19:08.304273 numbers_parser-4.3.0/src/numbers_parser/data/empty.numbers
--rw-r--r--   0        0        0    20435 2023-08-02 13:27:23.000000 numbers_parser-4.3.0/src/numbers_parser/document.py
--rw-r--r--   0        0        0      663 2022-10-17 17:39:14.019486 numbers_parser-4.3.0/src/numbers_parser/exceptions.py
--rw-r--r--   0        0        0      374 2023-07-16 14:30:53.391296 numbers_parser-4.3.0/src/numbers_parser/experimental.py
--rw-r--r--   0        0        0     3683 2023-07-23 15:54:51.189959 numbers_parser-4.3.0/src/numbers_parser/file.py
--rw-r--r--   0        0        0    10665 2023-07-14 19:05:10.689467 numbers_parser-4.3.0/src/numbers_parser/formula.py
--rw-r--r--   0        0        0    16007 2023-07-23 16:06:40.954866 numbers_parser-4.3.0/src/numbers_parser/generated/TNArchives_pb2.py
--rw-r--r--   0        0        0     1215 2023-07-23 16:06:40.955183 numbers_parser-4.3.0/src/numbers_parser/generated/TNArchives_sos_pb2.py
--rw-r--r--   0        0        0    18271 2023-07-23 16:06:40.955417 numbers_parser-4.3.0/src/numbers_parser/generated/TNCommandArchives_pb2.py
--rw-r--r--   0        0        0     1857 2023-07-23 16:06:40.955655 numbers_parser-4.3.0/src/numbers_parser/generated/TNCommandArchives_sos_pb2.py
--rw-r--r--   0        0        0    17361 2023-07-23 16:06:40.955915 numbers_parser-4.3.0/src/numbers_parser/generated/TSAArchives_pb2.py
--rw-r--r--   0        0        0     2033 2023-07-23 16:06:40.956132 numbers_parser-4.3.0/src/numbers_parser/generated/TSAArchives_sos_pb2.py
--rw-r--r--   0        0        0     3907 2023-07-23 16:06:40.956319 numbers_parser-4.3.0/src/numbers_parser/generated/TSACommandArchives_sos_pb2.py
--rw-r--r--   0        0        0    64955 2023-07-23 16:06:40.956672 numbers_parser-4.3.0/src/numbers_parser/generated/TSCEArchives_pb2.py
--rw-r--r--   0        0        0    11162 2023-07-23 16:06:40.957188 numbers_parser-4.3.0/src/numbers_parser/generated/TSCH3DArchives_pb2.py
--rw-r--r--   0        0        0     8655 2023-07-23 16:06:40.957541 numbers_parser-4.3.0/src/numbers_parser/generated/TSCHArchives_Common_pb2.py
--rw-r--r--   0        0        0    46323 2023-07-23 16:06:40.957794 numbers_parser-4.3.0/src/numbers_parser/generated/TSCHArchives_GEN_pb2.py
--rw-r--r--   0        0        0    22717 2023-07-23 16:06:40.958066 numbers_parser-4.3.0/src/numbers_parser/generated/TSCHArchives_pb2.py
--rw-r--r--   0        0        0    63730 2023-07-23 16:06:40.958325 numbers_parser-4.3.0/src/numbers_parser/generated/TSCHArchives_sos_pb2.py
--rw-r--r--   0        0        0    27446 2023-07-23 16:06:40.958670 numbers_parser-4.3.0/src/numbers_parser/generated/TSCHCommandArchives_pb2.py
--rw-r--r--   0        0        0    30051 2023-07-23 16:06:40.959087 numbers_parser-4.3.0/src/numbers_parser/generated/TSCHPreUFFArchives_pb2.py
--rw-r--r--   0        0        0    40151 2023-07-23 16:06:40.959435 numbers_parser-4.3.0/src/numbers_parser/generated/TSDArchives_pb2.py
--rw-r--r--   0        0        0     6022 2023-07-23 16:06:40.959684 numbers_parser-4.3.0/src/numbers_parser/generated/TSDArchives_sos_pb2.py
--rw-r--r--   0        0        0    29192 2023-07-23 16:06:40.959950 numbers_parser-4.3.0/src/numbers_parser/generated/TSDCommandArchives_pb2.py
--rw-r--r--   0        0        0    53520 2023-07-23 16:06:40.960332 numbers_parser-4.3.0/src/numbers_parser/generated/TSKArchives_pb2.py
--rw-r--r--   0        0        0     1941 2023-07-23 16:06:40.960544 numbers_parser-4.3.0/src/numbers_parser/generated/TSKArchives_sos_pb2.py
--rw-r--r--   0        0        0    18142 2023-07-23 16:06:40.960804 numbers_parser-4.3.0/src/numbers_parser/generated/TSPArchiveMessages_pb2.py
--rw-r--r--   0        0        0     2024 2023-07-23 16:06:40.961046 numbers_parser-4.3.0/src/numbers_parser/generated/TSPDatabaseMessages_pb2.py
--rw-r--r--   0        0        0    12611 2023-07-23 16:06:40.961302 numbers_parser-4.3.0/src/numbers_parser/generated/TSPMessages_pb2.py
--rw-r--r--   0        0        0     9717 2023-07-23 16:06:40.961563 numbers_parser-4.3.0/src/numbers_parser/generated/TSSArchives_pb2.py
--rw-r--r--   0        0        0     2842 2023-07-23 16:06:40.961856 numbers_parser-4.3.0/src/numbers_parser/generated/TSSArchives_sos_pb2.py
--rw-r--r--   0        0        0    88532 2023-07-23 16:06:40.962320 numbers_parser-4.3.0/src/numbers_parser/generated/TSTArchives_pb2.py
--rw-r--r--   0        0        0    12597 2023-07-23 16:06:40.962544 numbers_parser-4.3.0/src/numbers_parser/generated/TSTArchives_sos_pb2.py
--rw-r--r--   0        0        0    59523 2023-07-23 16:06:40.963108 numbers_parser-4.3.0/src/numbers_parser/generated/TSTCommandArchives_pb2.py
--rw-r--r--   0        0        0    12644 2023-07-23 16:06:40.963347 numbers_parser-4.3.0/src/numbers_parser/generated/TSTStylePropertyArchiving_pb2.py
--rw-r--r--   0        0        0    58663 2023-07-23 16:06:40.963755 numbers_parser-4.3.0/src/numbers_parser/generated/TSWPArchives_pb2.py
--rw-r--r--   0        0        0    28840 2023-07-23 16:06:40.964041 numbers_parser-4.3.0/src/numbers_parser/generated/TSWPArchives_sos_pb2.py
--rw-r--r--   0        0        0    25441 2023-07-23 16:06:40.964356 numbers_parser-4.3.0/src/numbers_parser/generated/TSWPCommandArchives_pb2.py
--rw-r--r--   0        0        0        0 2023-07-23 16:06:40.970289 numbers_parser-4.3.0/src/numbers_parser/generated/__init__.py
--rw-r--r--   0        0        0    22604 2023-07-23 16:06:33.784957 numbers_parser-4.3.0/src/numbers_parser/generated/fontmap.py
--rw-r--r--   0        0        0     6082 2023-07-23 16:06:33.032684 numbers_parser-4.3.0/src/numbers_parser/generated/functionmap.py
--rw-r--r--   0        0        0    11868 2023-07-23 15:54:51.253681 numbers_parser-4.3.0/src/numbers_parser/iwafile.py
--rw-r--r--   0        0        0    32117 2023-07-23 16:07:16.807745 numbers_parser-4.3.0/src/numbers_parser/mapping.py
--rw-r--r--   0        0        0    90563 2023-08-02 13:27:31.000000 numbers_parser-4.3.0/src/numbers_parser/model.py
--rw-r--r--   0        0        0     2642 2023-07-23 15:54:51.198744 numbers_parser-4.3.0/src/numbers_parser/numbers_uuid.py
--rw-r--r--   0        0        0    24349 1970-01-01 00:00:00.000000 numbers_parser-4.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1050 2022-06-23 17:13:17.000000 numbers_parser-4.4.0/LICENSE.rst
+-rw-r--r--   0        0        0    23217 2023-08-04 06:26:31.735290 numbers_parser-4.4.0/README.md
+-rw-r--r--   0        0        0     2130 2023-08-04 06:48:45.358692 numbers_parser-4.4.0/pyproject.toml
+-rw-r--r--   0        0        0     2081 2023-07-23 15:54:51.138965 numbers_parser-4.4.0/src/numbers_parser/__init__.py
+-rw-r--r--   0        0        0     4336 2023-08-02 13:30:28.000000 numbers_parser-4.4.0/src/numbers_parser/_cat_numbers.py
+-rw-r--r--   0        0        0     5784 2023-07-23 15:54:51.177251 numbers_parser-4.4.0/src/numbers_parser/_unpack_numbers.py
+-rw-r--r--   0        0        0     2616 2023-05-20 02:42:59.000000 numbers_parser-4.4.0/src/numbers_parser/bullets.py
+-rw-r--r--   0        0        0    25629 2023-08-04 06:45:07.855203 numbers_parser-4.4.0/src/numbers_parser/cell.py
+-rw-r--r--   0        0        0    28815 2023-08-04 06:26:26.428210 numbers_parser-4.4.0/src/numbers_parser/cell_storage.py
+-rw-r--r--   0        0        0     1900 2023-08-04 06:22:03.075998 numbers_parser-4.4.0/src/numbers_parser/constants.py
+-rw-r--r--   0        0        0     4239 2023-07-14 19:05:10.687308 numbers_parser-4.4.0/src/numbers_parser/containers.py
+-rwxr-xr-x   0        0        0    90316 2023-07-31 12:19:08.304273 numbers_parser-4.4.0/src/numbers_parser/data/empty.numbers
+-rw-r--r--   0        0        0    20435 2023-08-02 13:27:23.000000 numbers_parser-4.4.0/src/numbers_parser/document.py
+-rw-r--r--   0        0        0      663 2022-10-17 17:39:14.019486 numbers_parser-4.4.0/src/numbers_parser/exceptions.py
+-rw-r--r--   0        0        0      374 2023-07-16 14:30:53.391296 numbers_parser-4.4.0/src/numbers_parser/experimental.py
+-rw-r--r--   0        0        0     3683 2023-07-23 15:54:51.189959 numbers_parser-4.4.0/src/numbers_parser/file.py
+-rw-r--r--   0        0        0    10665 2023-07-14 19:05:10.689467 numbers_parser-4.4.0/src/numbers_parser/formula.py
+-rw-r--r--   0        0        0    16007 2023-07-23 16:06:40.954866 numbers_parser-4.4.0/src/numbers_parser/generated/TNArchives_pb2.py
+-rw-r--r--   0        0        0     1215 2023-07-23 16:06:40.955183 numbers_parser-4.4.0/src/numbers_parser/generated/TNArchives_sos_pb2.py
+-rw-r--r--   0        0        0    18271 2023-07-23 16:06:40.955417 numbers_parser-4.4.0/src/numbers_parser/generated/TNCommandArchives_pb2.py
+-rw-r--r--   0        0        0     1857 2023-07-23 16:06:40.955655 numbers_parser-4.4.0/src/numbers_parser/generated/TNCommandArchives_sos_pb2.py
+-rw-r--r--   0        0        0    17361 2023-07-23 16:06:40.955915 numbers_parser-4.4.0/src/numbers_parser/generated/TSAArchives_pb2.py
+-rw-r--r--   0        0        0     2033 2023-07-23 16:06:40.956132 numbers_parser-4.4.0/src/numbers_parser/generated/TSAArchives_sos_pb2.py
+-rw-r--r--   0        0        0     3907 2023-07-23 16:06:40.956319 numbers_parser-4.4.0/src/numbers_parser/generated/TSACommandArchives_sos_pb2.py
+-rw-r--r--   0        0        0    64955 2023-07-23 16:06:40.956672 numbers_parser-4.4.0/src/numbers_parser/generated/TSCEArchives_pb2.py
+-rw-r--r--   0        0        0    11162 2023-07-23 16:06:40.957188 numbers_parser-4.4.0/src/numbers_parser/generated/TSCH3DArchives_pb2.py
+-rw-r--r--   0        0        0     8655 2023-07-23 16:06:40.957541 numbers_parser-4.4.0/src/numbers_parser/generated/TSCHArchives_Common_pb2.py
+-rw-r--r--   0        0        0    46323 2023-07-23 16:06:40.957794 numbers_parser-4.4.0/src/numbers_parser/generated/TSCHArchives_GEN_pb2.py
+-rw-r--r--   0        0        0    22717 2023-07-23 16:06:40.958066 numbers_parser-4.4.0/src/numbers_parser/generated/TSCHArchives_pb2.py
+-rw-r--r--   0        0        0    63730 2023-07-23 16:06:40.958325 numbers_parser-4.4.0/src/numbers_parser/generated/TSCHArchives_sos_pb2.py
+-rw-r--r--   0        0        0    27446 2023-07-23 16:06:40.958670 numbers_parser-4.4.0/src/numbers_parser/generated/TSCHCommandArchives_pb2.py
+-rw-r--r--   0        0        0    30051 2023-07-23 16:06:40.959087 numbers_parser-4.4.0/src/numbers_parser/generated/TSCHPreUFFArchives_pb2.py
+-rw-r--r--   0        0        0    40151 2023-07-23 16:06:40.959435 numbers_parser-4.4.0/src/numbers_parser/generated/TSDArchives_pb2.py
+-rw-r--r--   0        0        0     6022 2023-07-23 16:06:40.959684 numbers_parser-4.4.0/src/numbers_parser/generated/TSDArchives_sos_pb2.py
+-rw-r--r--   0        0        0    29192 2023-07-23 16:06:40.959950 numbers_parser-4.4.0/src/numbers_parser/generated/TSDCommandArchives_pb2.py
+-rw-r--r--   0        0        0    53520 2023-07-23 16:06:40.960332 numbers_parser-4.4.0/src/numbers_parser/generated/TSKArchives_pb2.py
+-rw-r--r--   0        0        0     1941 2023-07-23 16:06:40.960544 numbers_parser-4.4.0/src/numbers_parser/generated/TSKArchives_sos_pb2.py
+-rw-r--r--   0        0        0    18142 2023-07-23 16:06:40.960804 numbers_parser-4.4.0/src/numbers_parser/generated/TSPArchiveMessages_pb2.py
+-rw-r--r--   0        0        0     2024 2023-07-23 16:06:40.961046 numbers_parser-4.4.0/src/numbers_parser/generated/TSPDatabaseMessages_pb2.py
+-rw-r--r--   0        0        0    12611 2023-07-23 16:06:40.961302 numbers_parser-4.4.0/src/numbers_parser/generated/TSPMessages_pb2.py
+-rw-r--r--   0        0        0     9717 2023-07-23 16:06:40.961563 numbers_parser-4.4.0/src/numbers_parser/generated/TSSArchives_pb2.py
+-rw-r--r--   0        0        0     2842 2023-07-23 16:06:40.961856 numbers_parser-4.4.0/src/numbers_parser/generated/TSSArchives_sos_pb2.py
+-rw-r--r--   0        0        0    88532 2023-07-23 16:06:40.962320 numbers_parser-4.4.0/src/numbers_parser/generated/TSTArchives_pb2.py
+-rw-r--r--   0        0        0    12597 2023-07-23 16:06:40.962544 numbers_parser-4.4.0/src/numbers_parser/generated/TSTArchives_sos_pb2.py
+-rw-r--r--   0        0        0    59523 2023-07-23 16:06:40.963108 numbers_parser-4.4.0/src/numbers_parser/generated/TSTCommandArchives_pb2.py
+-rw-r--r--   0        0        0    12644 2023-07-23 16:06:40.963347 numbers_parser-4.4.0/src/numbers_parser/generated/TSTStylePropertyArchiving_pb2.py
+-rw-r--r--   0        0        0    58663 2023-07-23 16:06:40.963755 numbers_parser-4.4.0/src/numbers_parser/generated/TSWPArchives_pb2.py
+-rw-r--r--   0        0        0    28840 2023-07-23 16:06:40.964041 numbers_parser-4.4.0/src/numbers_parser/generated/TSWPArchives_sos_pb2.py
+-rw-r--r--   0        0        0    25441 2023-07-23 16:06:40.964356 numbers_parser-4.4.0/src/numbers_parser/generated/TSWPCommandArchives_pb2.py
+-rw-r--r--   0        0        0        0 2023-07-23 16:06:40.970289 numbers_parser-4.4.0/src/numbers_parser/generated/__init__.py
+-rw-r--r--   0        0        0    22604 2023-07-23 16:06:33.784957 numbers_parser-4.4.0/src/numbers_parser/generated/fontmap.py
+-rw-r--r--   0        0        0     6082 2023-07-23 16:06:33.032684 numbers_parser-4.4.0/src/numbers_parser/generated/functionmap.py
+-rw-r--r--   0        0        0    11868 2023-07-23 15:54:51.253681 numbers_parser-4.4.0/src/numbers_parser/iwafile.py
+-rw-r--r--   0        0        0    32117 2023-07-23 16:07:16.807745 numbers_parser-4.4.0/src/numbers_parser/mapping.py
+-rw-r--r--   0        0        0    91156 2023-08-04 06:41:22.104247 numbers_parser-4.4.0/src/numbers_parser/model.py
+-rw-r--r--   0        0        0     2642 2023-07-23 15:54:51.198744 numbers_parser-4.4.0/src/numbers_parser/numbers_uuid.py
+-rw-r--r--   0        0        0    24433 1970-01-01 00:00:00.000000 numbers_parser-4.4.0/PKG-INFO
```

### Comparing `numbers_parser-4.3.0/LICENSE.rst` & `numbers_parser-4.4.0/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.3.0/README.md` & `numbers_parser-4.4.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -203,15 +203,15 @@
 * `Cell.style.name`: cell style (`str`)
 * `Cell.style.underline`: `True` if the cell font is underline
 * `Cell.style.strikethrough`: `True` if the cell font is strikethrough
 * `Cell.style.first_indent`: first line indent in points (`float`)
 * `Cell.style.left_indent`: left indent in points (`float`)
 * `Cell.style.right_indent`: right indent in points (`float`)
 * `Cell.style.text_inset`: text inset in points (`float`)
-
+* `Cell.style.text_wrap`: `True` if text wrapping is enabled (default for new cells)
 
 #### Cell images
 
 The methods `style.bg_image.filename` and `style.bg_image.data` return data about the image used for a cell's background, where set. If a cell has no background image, `style.bg_image`  is `None`.
 
 ``` python
 cell = table.cell("B1")
```

### Comparing `numbers_parser-4.3.0/pyproject.toml` & `numbers_parser-4.4.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 description = "Read and write Apple Numbers spreadsheets"
 documentation = "https://github.com/masaccio/numbers-parser/blob/main/README.md"
 license = "MIT"
 name = "numbers-parser"
 packages = [{include = "numbers_parser", from = "src"}]
 readme = "README.md"
 repository = "https://github.com/masaccio/numbers-parser"
-version = "4.3.0"
+version = "4.4.0"
 
 [tool.poetry.scripts]
 cat-numbers = "numbers_parser._cat_numbers:main"
 unpack-numbers = "numbers_parser._unpack_numbers:main"
 
 [tool.poetry.dependencies]
 compact-json = "^1.1.3"
```

### Comparing `numbers_parser-4.3.0/src/numbers_parser/__init__.py` & `numbers_parser-4.4.0/src/numbers_parser/__init__.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.3.0/src/numbers_parser/_cat_numbers.py` & `numbers_parser-4.4.0/src/numbers_parser/_cat_numbers.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.3.0/src/numbers_parser/_unpack_numbers.py` & `numbers_parser-4.4.0/src/numbers_parser/_unpack_numbers.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.3.0/src/numbers_parser/bullets.py` & `numbers_parser-4.4.0/src/numbers_parser/bullets.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.3.0/src/numbers_parser/cell.py` & `numbers_parser-4.4.0/src/numbers_parser/cell.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from numbers_parser.cell_storage import CellType, CellStorage
 from numbers_parser.constants import (
     EMPTY_STORAGE_BUFFER,
     DEFAULT_FONT,
     DEFAULT_FONT_SIZE,
     DEFAULT_ALIGNMENT,
     DEFAULT_TEXT_INSET,
+    DEFAULT_TEXT_WRAP,
     DEFAULT_BORDER_WIDTH,
     DEFAULT_BORDER_COLOR,
     DEFAULT_BORDER_STYLE,
     MAX_SIGNIFICANT_DIGITS,
 )
 
 from collections import namedtuple
@@ -24,14 +25,43 @@
 from datetime import datetime as builtin_datetime, timedelta as builtin_timedelta
 from enum import IntEnum
 from functools import lru_cache
 from pendulum import duration, Duration, DateTime, instance as pendulum_instance
 from typing import Any, List, Tuple, Union
 from warnings import warn
 
+__all__ = [
+    "Alignment",
+    "BackgroundImage",
+    "BoolCell",
+    "Border",
+    "BorderType",
+    "BulletedTextCell",
+    "Cell",
+    "CellBorder",
+    "DateCell",
+    "DurationCell",
+    "EmptyCell",
+    "ErrorCell",
+    "HorizontalJustification",
+    "MergeAnchor",
+    "MergeReference",
+    "MergedCell",
+    "NumberCell",
+    "RichTextCell",
+    "RGB",
+    "Style",
+    "TextCell",
+    "VerticalJustification",
+    "xl_cell_to_rowcol",
+    "xl_col_to_name",
+    "xl_range",
+    "xl_rowcol_to_cell",
+]
+
 
 class BackgroundImage:
     def __init__(self, image_data: bytes = None, filename: str = None):
         self._data = image_data
         self._filename = filename
 
     @property
@@ -111,14 +141,15 @@
     italic: bool = False
     strikethrough: bool = False
     underline: bool = False
     first_indent: float = 0
     left_indent: float = 0
     right_indent: float = 0
     text_inset: float = DEFAULT_TEXT_INSET
+    text_wrap: bool = DEFAULT_TEXT_WRAP
     name: str = None
     _text_style_obj_id: int = None
     _cell_style_obj_id: int = None
     _update_cell_style: bool = False
     _update_text_style: bool = False
 
     @staticmethod
@@ -143,14 +174,15 @@
         return [
             "alignment",
             "bg_color",
             "first_indent",
             "left_indent",
             "right_indent",
             "text_inset",
+            "text_wrap",
         ]
 
     @classmethod
     def from_storage(cls, cell_storage: object, model: object):
         style = Style()
 
         if cell_storage.image_data is not None:
@@ -169,14 +201,15 @@
             strikethrough=model.cell_is_strikethrough(cell_storage),
             underline=model.cell_is_underline(cell_storage),
             name=model.cell_style_name(cell_storage),
             first_indent=model.cell_first_indent(cell_storage),
             left_indent=model.cell_left_indent(cell_storage),
             right_indent=model.cell_right_indent(cell_storage),
             text_inset=model.cell_text_inset(cell_storage),
+            text_wrap=model.cell_text_wrap(cell_storage),
             _text_style_obj_id=model.text_style_object_id(cell_storage),
             _cell_style_obj_id=model.cell_style_object_id(cell_storage),
         )
         return style
 
     def __post_init__(self):
         self.bg_color = rgb_color(self.bg_color)
```

### Comparing `numbers_parser-4.3.0/src/numbers_parser/cell_storage.py` & `numbers_parser-4.4.0/src/numbers_parser/cell_storage.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,15 +94,15 @@
         "cell_style_id",
         "text_style_id",
         # "cond_style_id",
         # "cond_rule_style_id",
         "formula_id",
         # "control_id",
         "formula_error_id",
-        # "suggest_id",
+        "suggest_id",
         "num_format_id",
         "currency_format_id",
         "date_format_id",
         "duration_format_id",
         "text_format_id",
         "bool_format_id",
         # "comment_id",
@@ -125,15 +125,15 @@
         self.cell_style_id = None
         self.text_style_id = None
         # self.cond_style_id = None
         # self.cond_rule_style_id = None
         self.formula_id = None
         # self.control_id = None
         self.formula_error_id = None
-        # self.suggest_id = None
+        self.suggest_id = None
         self.num_format_id = None
         self.currency_format_id = None
         self.date_format_id = None
         self.duration_format_id = None
         self.text_format_id = None
         self.bool_format_id = None
         # self.comment_id = None
@@ -181,19 +181,19 @@
             offset += 4
         # if flags & 0x400:
         #     self.control_id = unpack("<i", buffer[offset : offset + 4])[0]
         #     offset += 4
         # if flags & 0x800:
         #     self.formula_error_id = unpack("<i", buffer[offset : offset + 4])[0]
         #     offset += 4
-        # if flags & 0x1000:
-        #     self.suggest_id = unpack("<i", buffer[offset : offset + 4])[0]
-        #     offset += 4
+        if flags & 0x1000:
+            self.suggest_id = unpack("<i", buffer[offset : offset + 4])[0]
+            offset += 4
         # Skip unused flags
-        offset += 4 * bin(flags & 0x1D00).count("1")
+        offset += 4 * bin(flags & 0xD00).count("1")
         #
         if flags & 0x2000:
             self.num_format_id = unpack("<i", buffer[offset : offset + 4])[0]
             offset += 4
         if flags & 0x4000:
             self.currency_format_id = unpack("<i", buffer[offset : offset + 4])[0]
             offset += 4
@@ -525,16 +525,20 @@
                 index += 1
         else:
             formatted_value += current_char
             index += 1
     return formatted_value
 
 
+# import inspect
+
+
 def decode_number_format(format, value, name):  # noqa: C901
     """Parse a custom date format string and return a formatted number value"""
+    # cell = inspect.currentframe().f_back.f_back.f_back.f_locals["self"]
     custom_format_string = format.custom_format_string
     value *= format.scale_factor
     if "%" in custom_format_string and format.scale_factor == 1.0:
         # Per cent scale has 100x but % does not
         value *= 100.0
 
     if format.currency_code != "":
@@ -606,14 +610,17 @@
         else:
             int_pad = CellPadding.SPACE
             int_width = len(int_part)
     else:
         int_pad = None
         int_width = num_integers
 
+    # if num_integers == 0 and dec_pad == CellPadding.SPACE:
+    #     dec_pad = CellPadding.ZERO
+
     # Formatting integer zero:
     #   Blank (padded if needed) if int_pad is SPACE and no decimals
     #   No leading zero if:
     #     int_pad is NONE, dec_pad is SPACE
     #     int_pad is SPACE, dec_pad is SPACE
     #     int_pad is SPACE, dec_pad is ZERO
     #     int_pad is SPACE, dec_pad is NONE if num decimals < decimals length
@@ -643,16 +650,18 @@
     else:
         if format.show_thousands_separator:
             formatted_value = f"{integer:,}"
         else:
             formatted_value = str(integer)
 
     if num_decimals:
-        if dec_pad == CellPadding.ZERO:
+        if dec_pad == CellPadding.ZERO or (dec_pad == CellPadding.SPACE and num_integers == 0):
             formatted_value += "." + f"{decimal:,.{dec_width}f}"[2:]
+        elif dec_pad == CellPadding.SPACE and decimal == 0 and num_integers > 0:
+            formatted_value += ".".ljust(dec_width + 1)
         elif dec_pad == CellPadding.SPACE:
             decimal_str = str(decimal)[2:]
             formatted_value += "." + decimal_str.ljust(dec_width)
         elif decimal or num_integers == 0:
             formatted_value += "." + str(decimal)[2:]
 
     formatted_value = custom_format_string.replace(format_spec, formatted_value)
```

### Comparing `numbers_parser-4.3.0/src/numbers_parser/constants.py` & `numbers_parser-4.4.0/src/numbers_parser/constants.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 DEFAULT_ALIGNMENT = ("auto", "top")
 DEFAULT_BORDER_WIDTH = 0.35
 DEFAULT_BORDER_COLOR = (0, 0, 0)
 DEFAULT_BORDER_STYLE = "solid"
 DEFAULT_FONT = "Helvetica Neue"
 DEFAULT_FONT_SIZE = 11.0
 DEFAULT_TEXT_INSET = 4.0
+DEFAULT_TEXT_WRAP = True
 EMPTY_STORAGE_BUFFER = b"\x05\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00"
 
 # Numbers limits
 MAX_TILE_SIZE = 256
 MAX_ROW_COUNT = 1000000
 MAX_COL_COUNT = 1000
 MAX_HEADER_COUNT = 5
```

### Comparing `numbers_parser-4.3.0/src/numbers_parser/containers.py` & `numbers_parser-4.4.0/src/numbers_parser/containers.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.3.0/src/numbers_parser/data/empty.numbers` & `numbers_parser-4.4.0/src/numbers_parser/data/empty.numbers`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.3.0/src/numbers_parser/document.py` & `numbers_parser-4.4.0/src/numbers_parser/document.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.3.0/src/numbers_parser/exceptions.py` & `numbers_parser-4.4.0/src/numbers_parser/exceptions.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.3.0/src/numbers_parser/file.py` & `numbers_parser-4.4.0/src/numbers_parser/file.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.3.0/src/numbers_parser/formula.py` & `numbers_parser-4.4.0/src/numbers_parser/formula.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.3.0/src/numbers_parser/generated/TNArchives_pb2.py` & `numbers_parser-4.4.0/src/numbers_parser/generated/TNArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.3.0/src/numbers_parser/generated/TNArchives_sos_pb2.py` & `numbers_parser-4.4.0/src/numbers_parser/generated/TNArchives_sos_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.3.0/src/numbers_parser/generated/TNCommandArchives_pb2.py` & `numbers_parser-4.4.0/src/numbers_parser/generated/TNCommandArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.3.0/src/numbers_parser/generated/TNCommandArchives_sos_pb2.py` & `numbers_parser-4.4.0/src/numbers_parser/generated/TNCommandArchives_sos_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.3.0/src/numbers_parser/generated/TSAArchives_pb2.py` & `numbers_parser-4.4.0/src/numbers_parser/generated/TSAArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.3.0/src/numbers_parser/generated/TSAArchives_sos_pb2.py` & `numbers_parser-4.4.0/src/numbers_parser/generated/TSAArchives_sos_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.3.0/src/numbers_parser/generated/TSACommandArchives_sos_pb2.py` & `numbers_parser-4.4.0/src/numbers_parser/generated/TSACommandArchives_sos_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.3.0/src/numbers_parser/generated/TSCEArchives_pb2.py` & `numbers_parser-4.4.0/src/numbers_parser/generated/TSCEArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.3.0/src/numbers_parser/generated/TSCH3DArchives_pb2.py` & `numbers_parser-4.4.0/src/numbers_parser/generated/TSCH3DArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.3.0/src/numbers_parser/generated/TSCHArchives_Common_pb2.py` & `numbers_parser-4.4.0/src/numbers_parser/generated/TSCHArchives_Common_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.3.0/src/numbers_parser/generated/TSCHArchives_GEN_pb2.py` & `numbers_parser-4.4.0/src/numbers_parser/generated/TSCHArchives_GEN_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.3.0/src/numbers_parser/generated/TSCHArchives_pb2.py` & `numbers_parser-4.4.0/src/numbers_parser/generated/TSCHArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.3.0/src/numbers_parser/generated/TSCHArchives_sos_pb2.py` & `numbers_parser-4.4.0/src/numbers_parser/generated/TSCHArchives_sos_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.3.0/src/numbers_parser/generated/TSCHCommandArchives_pb2.py` & `numbers_parser-4.4.0/src/numbers_parser/generated/TSCHCommandArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.3.0/src/numbers_parser/generated/TSCHPreUFFArchives_pb2.py` & `numbers_parser-4.4.0/src/numbers_parser/generated/TSCHPreUFFArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.3.0/src/numbers_parser/generated/TSDArchives_pb2.py` & `numbers_parser-4.4.0/src/numbers_parser/generated/TSDArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.3.0/src/numbers_parser/generated/TSDArchives_sos_pb2.py` & `numbers_parser-4.4.0/src/numbers_parser/generated/TSDArchives_sos_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.3.0/src/numbers_parser/generated/TSDCommandArchives_pb2.py` & `numbers_parser-4.4.0/src/numbers_parser/generated/TSDCommandArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.3.0/src/numbers_parser/generated/TSKArchives_pb2.py` & `numbers_parser-4.4.0/src/numbers_parser/generated/TSKArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.3.0/src/numbers_parser/generated/TSKArchives_sos_pb2.py` & `numbers_parser-4.4.0/src/numbers_parser/generated/TSKArchives_sos_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.3.0/src/numbers_parser/generated/TSPArchiveMessages_pb2.py` & `numbers_parser-4.4.0/src/numbers_parser/generated/TSPArchiveMessages_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.3.0/src/numbers_parser/generated/TSPDatabaseMessages_pb2.py` & `numbers_parser-4.4.0/src/numbers_parser/generated/TSPDatabaseMessages_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.3.0/src/numbers_parser/generated/TSPMessages_pb2.py` & `numbers_parser-4.4.0/src/numbers_parser/generated/TSPMessages_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.3.0/src/numbers_parser/generated/TSSArchives_pb2.py` & `numbers_parser-4.4.0/src/numbers_parser/generated/TSSArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.3.0/src/numbers_parser/generated/TSSArchives_sos_pb2.py` & `numbers_parser-4.4.0/src/numbers_parser/generated/TSSArchives_sos_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.3.0/src/numbers_parser/generated/TSTArchives_pb2.py` & `numbers_parser-4.4.0/src/numbers_parser/generated/TSTArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.3.0/src/numbers_parser/generated/TSTArchives_sos_pb2.py` & `numbers_parser-4.4.0/src/numbers_parser/generated/TSTArchives_sos_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.3.0/src/numbers_parser/generated/TSTCommandArchives_pb2.py` & `numbers_parser-4.4.0/src/numbers_parser/generated/TSTCommandArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.3.0/src/numbers_parser/generated/TSTStylePropertyArchiving_pb2.py` & `numbers_parser-4.4.0/src/numbers_parser/generated/TSTStylePropertyArchiving_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.3.0/src/numbers_parser/generated/TSWPArchives_pb2.py` & `numbers_parser-4.4.0/src/numbers_parser/generated/TSWPArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.3.0/src/numbers_parser/generated/TSWPArchives_sos_pb2.py` & `numbers_parser-4.4.0/src/numbers_parser/generated/TSWPArchives_sos_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.3.0/src/numbers_parser/generated/TSWPCommandArchives_pb2.py` & `numbers_parser-4.4.0/src/numbers_parser/generated/TSWPCommandArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.3.0/src/numbers_parser/generated/fontmap.py` & `numbers_parser-4.4.0/src/numbers_parser/generated/fontmap.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.3.0/src/numbers_parser/generated/functionmap.py` & `numbers_parser-4.4.0/src/numbers_parser/generated/functionmap.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.3.0/src/numbers_parser/iwafile.py` & `numbers_parser-4.4.0/src/numbers_parser/iwafile.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.3.0/src/numbers_parser/mapping.py` & `numbers_parser-4.4.0/src/numbers_parser/mapping.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.3.0/src/numbers_parser/model.py` & `numbers_parser-4.4.0/src/numbers_parser/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     DEFAULT_COLUMN_WIDTH,
     DEFAULT_DOCUMENT,
     DEFAULT_PRE_BNC_BYTES,
     DEFAULT_ROW_HEIGHT,
     DEFAULT_TABLE_OFFSET,
     DEFAULT_TILE_SIZE,
     DEFAULT_TEXT_INSET,
+    DEFAULT_TEXT_WRAP,
     DOCUMENT_ID,
     PACKAGE_ID,
     MAX_TILE_SIZE,
 )
 from numbers_parser.cell import (
     xl_rowcol_to_cell,
     xl_col_to_name,
@@ -1331,14 +1332,15 @@
                 if cell._style is not None and cell._style._update_cell_style:
                     fingerprint = (
                         str(cell.style.alignment.vertical)
                         + str(cell.style.first_indent)
                         + str(cell.style.left_indent)
                         + str(cell.style.right_indent)
                         + str(cell.style.text_inset)
+                        + str(cell.style.text_wrap)
                     )
                     if cell._style.bg_color is not None:
                         fingerprint = fingerprint + (
                             str(cell.style.bg_color.r)
                             + str(cell.style.bg_color.g)
                             + str(cell.style.bg_color.b)
                         )
@@ -1374,14 +1376,15 @@
                     **color_attrs,
                     "padding": {
                         "left": style.text_inset,
                         "top": style.text_inset,
                         "right": style.text_inset,
                         "bottom": style.text_inset,
                     },
+                    "text_wrap": style.text_wrap,
                     "vertical_alignment": style.alignment.vertical,
                 },
             },
             TSTArchives.CellStyleArchive,
         )
         style_id_name = f"numbers-parser-custom-{cell_style_id}"
         cell_style.super.style_identifier = style_id_name
@@ -1425,21 +1428,15 @@
             offset = len("Custom Style ")
             custom_style_ids = [int(x[offset:]) for x in custom_styles]
             return "Custom Style " + str(custom_style_ids[-1] + 1)
         else:
             return "Custom Style 1"
 
     def pack_cell_storage(  # noqa: C901
-        self,
-        table_id: int,
-        data: List,
-        row_num: int,
-        col_num: int,
-        formula_id=None,
-        num_format_id=None,
+        self, table_id: int, data: List, row_num: int, col_num: int
     ) -> bytearray:
         """Create a storage buffer for a cell using v5 (modern) layout"""
         cell = data[row_num][col_num]
         if cell._style is not None:
             if cell._style._text_style_obj_id is not None:
                 cell._storage.text_style_id = self._table_styles.lookup_key(
                     cell._table_id,
@@ -1518,18 +1515,24 @@
             flags |= 0x40
             length += 4
             storage += pack("<i", cell._storage.text_style_id)
         if cell._storage.formula_id is not None:
             flags |= 0x200
             length += 4
             storage += pack("<i", cell._storage.formula_id)
+        if cell._storage.suggest_id is not None:
+            flags |= 0x1000
+            length += 4
+            storage += pack("<i", cell._storage.suggest_id)
         if cell._storage.num_format_id is not None:
             flags |= 0x2000
             length += 4
             storage += pack("<i", cell._storage.num_format_id)
+            storage[4:6] = pack("<h", 2)
+            storage[6:8] = pack("<h", 1)
         if cell._storage.currency_format_id is not None:
             flags |= 0x4000
             length += 4
             storage += pack("<i", cell._storage.currency_format_id)
         if cell._storage.date_format_id is not None:
             flags |= 0x8000
             length += 4
@@ -1787,14 +1790,21 @@
         else:
             style = self.table_style(cell_storage.table_id, cell_storage.cell_style_id)
             padding = self.cell_property(style, "padding")
             # Padding is always identical (only one UI setting)
             text_inset = padding.left
             return text_inset
 
+    def cell_text_wrap(self, cell_storage: CellStorage) -> float:
+        if cell_storage.cell_style_id is None:
+            return DEFAULT_TEXT_WRAP
+        else:
+            style = self.table_style(cell_storage.table_id, cell_storage.cell_style_id)
+            return self.cell_property(style, "text_wrap")
+
     def stroke_type(self, stroke_run: object) -> str:
         """Return the stroke type for a stroke run"""
         stroke_type = stroke_run.stroke.pattern.type
         if stroke_type == StrokePattern.StrokePatternType.TSDSolidPattern:
             return "solid"
         elif stroke_type == StrokePattern.StrokePatternType.TSDPattern:
             if stroke_run.stroke.pattern.pattern[0] < 1.0:
```

### Comparing `numbers_parser-4.3.0/src/numbers_parser/numbers_uuid.py` & `numbers_parser-4.4.0/src/numbers_parser/numbers_uuid.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.3.0/PKG-INFO` & `numbers_parser-4.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: numbers-parser
-Version: 4.3.0
+Version: 4.4.0
 Summary: Read and write Apple Numbers spreadsheets
 Home-page: https://github.com/masaccio/numbers-parser
 License: MIT
 Author: Jon Connell
 Author-email: python@figsandfudge.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -232,15 +232,15 @@
 * `Cell.style.name`: cell style (`str`)
 * `Cell.style.underline`: `True` if the cell font is underline
 * `Cell.style.strikethrough`: `True` if the cell font is strikethrough
 * `Cell.style.first_indent`: first line indent in points (`float`)
 * `Cell.style.left_indent`: left indent in points (`float`)
 * `Cell.style.right_indent`: right indent in points (`float`)
 * `Cell.style.text_inset`: text inset in points (`float`)
-
+* `Cell.style.text_wrap`: `True` if text wrapping is enabled (default for new cells)
 
 #### Cell images
 
 The methods `style.bg_image.filename` and `style.bg_image.data` return data about the image used for a cell's background, where set. If a cell has no background image, `style.bg_image`  is `None`.
 
 ``` python
 cell = table.cell("B1")
```

