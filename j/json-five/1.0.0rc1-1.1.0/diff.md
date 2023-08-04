# Comparing `tmp/json-five-1.0.0rc1.tar.gz` & `tmp/json-five-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "json-five-1.0.0rc1.tar", last modified: Tue Aug  1 04:50:10 2023, max compression
+gzip compressed data, was "json-five-1.1.0.tar", last modified: Fri Aug  4 06:19:41 2023, max compression
```

## Comparing `json-five-1.0.0rc1.tar` & `json-five-1.1.0.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 04:50:10.111713 json-five-1.0.0rc1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-01 04:49:59.000000 json-five-1.0.0rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-01 04:49:59.000000 json-five-1.0.0rc1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-08-01 04:50:10.111713 json-five-1.0.0rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-08-01 04:49:59.000000 json-five-1.0.0rc1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 04:50:10.111713 json-five-1.0.0rc1/json5/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-08-01 04:49:59.000000 json-five-1.0.0rc1/json5/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11263 2023-08-01 04:49:59.000000 json-five-1.0.0rc1/json5/dumper.py
--rw-r--r--   0 runner    (1001) docker     (123)     9195 2023-08-01 04:49:59.000000 json-five-1.0.0rc1/json5/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     7768 2023-08-01 04:49:59.000000 json-five-1.0.0rc1/json5/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    21269 2023-08-01 04:49:59.000000 json-five-1.0.0rc1/json5/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 04:49:59.000000 json-five-1.0.0rc1/json5/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-08-01 04:49:59.000000 json-five-1.0.0rc1/json5/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-08-01 04:49:59.000000 json-five-1.0.0rc1/json5/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 04:50:10.111713 json-five-1.0.0rc1/json_five.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-08-01 04:50:10.000000 json-five-1.0.0rc1/json_five.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-08-01 04:50:10.000000 json-five-1.0.0rc1/json_five.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 04:50:10.000000 json-five-1.0.0rc1/json_five.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-01 04:50:10.000000 json-five-1.0.0rc1/json_five.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-01 04:50:10.000000 json-five-1.0.0rc1/json_five.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-08-01 04:50:10.111713 json-five-1.0.0rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 04:49:59.000000 json-five-1.0.0rc1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 04:50:10.111713 json-five-1.0.0rc1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     7360 2023-08-01 04:49:59.000000 json-five-1.0.0rc1/tests/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-08-01 04:49:59.000000 json-five-1.0.0rc1/tests/test_json5_dump.py
--rw-r--r--   0 runner    (1001) docker     (123)     8082 2023-08-01 04:49:59.000000 json-five-1.0.0rc1/tests/test_json5_load.py
--rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-08-01 04:49:59.000000 json-five-1.0.0rc1/tests/test_json5_official_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-08-01 04:49:59.000000 json-five-1.0.0rc1/tests/test_json_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-08-01 04:49:59.000000 json-five-1.0.0rc1/tests/test_loads_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-08-01 04:49:59.000000 json-five-1.0.0rc1/tests/test_model_loader_dumper.py
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-08-01 04:49:59.000000 json-five-1.0.0rc1/tests/test_modelizer.py
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-08-01 04:49:59.000000 json-five-1.0.0rc1/tests/test_regressions.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-08-01 04:49:59.000000 json-five-1.0.0rc1/tests/test_roundtrip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 06:19:41.355108 json-five-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-04 06:19:30.000000 json-five-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-04 06:19:30.000000 json-five-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5177 2023-08-04 06:19:41.355108 json-five-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4480 2023-08-04 06:19:30.000000 json-five-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 06:19:41.351108 json-five-1.1.0/json5/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-08-04 06:19:30.000000 json-five-1.1.0/json5/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11895 2023-08-04 06:19:30.000000 json-five-1.1.0/json5/dumper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9108 2023-08-04 06:19:30.000000 json-five-1.1.0/json5/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10276 2023-08-04 06:19:30.000000 json-five-1.1.0/json5/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22611 2023-08-04 06:19:30.000000 json-five-1.1.0/json5/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 06:19:30.000000 json-five-1.1.0/json5/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-08-04 06:19:30.000000 json-five-1.1.0/json5/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-08-04 06:19:30.000000 json-five-1.1.0/json5/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 06:19:41.351108 json-five-1.1.0/json_five.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5177 2023-08-04 06:19:41.000000 json-five-1.1.0/json_five.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-08-04 06:19:41.000000 json-five-1.1.0/json_five.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 06:19:41.000000 json-five-1.1.0/json_five.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-04 06:19:41.000000 json-five-1.1.0/json_five.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-04 06:19:41.000000 json-five-1.1.0/json_five.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-08-04 06:19:41.355108 json-five-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 06:19:30.000000 json-five-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 06:19:41.355108 json-five-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7360 2023-08-04 06:19:30.000000 json-five-1.1.0/tests/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-08-04 06:19:30.000000 json-five-1.1.0/tests/test_json5_dump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8082 2023-08-04 06:19:30.000000 json-five-1.1.0/tests/test_json5_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-08-04 06:19:30.000000 json-five-1.1.0/tests/test_json5_official_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-08-04 06:19:30.000000 json-five-1.1.0/tests/test_json_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-08-04 06:19:30.000000 json-five-1.1.0/tests/test_loads_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-08-04 06:19:30.000000 json-five-1.1.0/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-08-04 06:19:30.000000 json-five-1.1.0/tests/test_model_loader_dumper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-08-04 06:19:30.000000 json-five-1.1.0/tests/test_modelizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-08-04 06:19:30.000000 json-five-1.1.0/tests/test_regressions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-08-04 06:19:30.000000 json-five-1.1.0/tests/test_roundtrip.py
```

### Comparing `json-five-1.0.0rc1/LICENSE` & `json-five-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `json-five-1.0.0rc1/json5/dumper.py` & `json-five-1.1.0/json5/dumper.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,39 @@
 from __future__ import annotations
 
 import io
 import json
 import math
 import typing
 from abc import abstractmethod
+from functools import singledispatchmethod
 from typing import Any
 
 from .loader import JsonIdentifier
-from .utils import singledispatchmethod
-from json5.model import *
+from .model import BlockComment
+from .model import BooleanLiteral
+from .model import Comment
+from .model import DoubleQuotedString
+from .model import Float
+from .model import Identifier
+from .model import Infinity
+from .model import Integer
+from .model import JSONArray
+from .model import JSONObject
+from .model import JSONText
+from .model import KeyValuePair
+from .model import LineComment
+from .model import NaN
+from .model import Node
+from .model import NullLiteral
+from .model import SingleQuotedString
+from .model import String
+from .model import TrailingComma
+from .model import UnaryOp
+from .model import Value
 
 
 class Environment:
     def __init__(self) -> None:
         self.outfile: typing.TextIO = io.StringIO()
         self.indent_level: int = 0
         self.indent: int = 0
@@ -196,16 +216,17 @@
 
     @to_json(JSONObject)
     def json_object_to_json(self, node: JSONObject) -> Any:
         self.process_wsc_before(node)
         self.env.write('{')
         if node.leading_wsc:
             self.process_leading_wsc(node)
-        num_pairs = len(node.key_value_pairs)
-        for index, kvp in enumerate(node.key_value_pairs, start=1):
+        key_value_pairs = node.key_value_pairs
+        num_pairs = len(key_value_pairs)
+        for index, kvp in enumerate(key_value_pairs, start=1):
             self.dump(kvp.key)
             self.env.write(':')
             self.dump(kvp.value)
             if index != num_pairs:
                 self.env.write(',')
         if node.trailing_comma:
             self.dump(node.trailing_comma)
```

### Comparing `json-five-1.0.0rc1/json5/loader.py` & `json-five-1.1.0/json5/loader.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 from __future__ import annotations
 
 import logging
 import typing
 from abc import abstractmethod
+from functools import singledispatchmethod
 from typing import Callable
 from typing import Literal
 
-from json5.model import BooleanLiteral
-from json5.model import Comment
-from json5.model import DoubleQuotedString
-from json5.model import Float
-from json5.model import Identifier
-from json5.model import Infinity
-from json5.model import Integer
-from json5.model import JSONArray
-from json5.model import JSONObject
-from json5.model import JSONText
-from json5.model import NaN
-from json5.model import Node
-from json5.model import NullLiteral
-from json5.model import SingleQuotedString
-from json5.model import String
-from json5.model import UnaryOp
-from json5.parser import parse_source
-from json5.utils import singledispatchmethod
+from .model import BooleanLiteral
+from .model import Comment
+from .model import DoubleQuotedString
+from .model import Float
+from .model import Identifier
+from .model import Infinity
+from .model import Integer
+from .model import JSONArray
+from .model import JSONObject
+from .model import JSONText
+from .model import NaN
+from .model import Node
+from .model import NullLiteral
+from .model import SingleQuotedString
+from .model import String
+from .model import UnaryOp
+from .parser import parse_source
 
 logger = logging.getLogger(__name__)
 # logger.setLevel(level=logging.DEBUG)
 # logger.addHandler(logging.StreamHandler(stream=sys.stderr))
 
 
 class Environment:
```

### Comparing `json-five-1.0.0rc1/json5/parser.py` & `json-five-1.1.0/json5/parser.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,19 +8,38 @@
 from typing import Literal
 from typing import Protocol
 
 import regex as re
 from sly import Parser  # type: ignore
 from sly.yacc import SlyLogger  # type: ignore
 
-from json5.model import *
-from json5.tokenizer import JSON5Token
-from json5.tokenizer import JSONLexer
-from json5.tokenizer import tokenize
-from json5.utils import JSON5DecodeError
+from .model import BlockComment
+from .model import BooleanLiteral
+from .model import Comment
+from .model import DoubleQuotedString
+from .model import Float
+from .model import Identifier
+from .model import Infinity
+from .model import Integer
+from .model import JSONArray
+from .model import JSONObject
+from .model import JSONText
+from .model import Key
+from .model import KeyValuePair
+from .model import LineComment
+from .model import NaN
+from .model import NullLiteral
+from .model import SingleQuotedString
+from .model import TrailingComma
+from .model import UnaryOp
+from .model import Value
+from .tokenizer import JSON5Token
+from .tokenizer import JSONLexer
+from .tokenizer import tokenize
+from .utils import JSON5DecodeError
 
 
 class QuietSlyLogger(SlyLogger):  # type: ignore[misc]
     def warning(self, *args: Any, **kwargs: Any) -> None:
         return
 
     debug = warning
@@ -73,132 +92,151 @@
 
 
 def unicode_escape_replace(matchobj: re.Match[str]) -> str:
     s = matchobj.group(0)
     return _unicode_escape_replace(s)
 
 
+class T_TokenSlice(Protocol):
+    def __getitem__(self, item: int) -> JSON5Token:
+        ...
+
+
+class T_AnyProduction(Protocol):
+    _slice: T_TokenSlice
+
+
 class T_TextProduction(Protocol):
     wsc0: list[Comment | str]
     wsc1: list[Comment | str]
+    value: Value
 
     def __getitem__(self, i: Literal[1]) -> Value:
         ...
 
 
-class T_TokenSlice(Protocol):
-    def __getitem__(self, item: int) -> JSON5Token:
-        ...
-
-
 class T_FirstKeyValuePairProduction(Protocol):
     wsc0: list[Comment | str]
     wsc1: list[Comment | str]
     wsc2: list[Comment | str]
     key: Key
     value: Value
+    _slice: T_TokenSlice
 
     def __getitem__(self, item: int) -> Key | Value:
         ...
 
 
 class T_WSCProduction(Protocol):
+    _slice: T_TokenSlice
+
     def __getitem__(self, item: Literal[0]) -> str | Comment:
         ...
 
 
 class T_CommentProduction(Protocol):
+    _slice: T_TokenSlice
+
     def __getitem__(self, item: Literal[0]) -> str:
         ...
 
-    _slice: T_TokenSlice
-
 
 class T_KeyValuePairsProduction(Protocol):
+    _slice: T_TokenSlice
     first_key_value_pair: KeyValuePair
     subsequent_key_value_pair: list[KeyValuePair]
 
 
 class T_JsonObjectProduction(Protocol):
-    key_value_pairs: tuple[list[KeyValuePair], TrailingComma | None] | None
     _slice: T_TokenSlice
+    key_value_pairs: tuple[list[KeyValuePair], TrailingComma | None] | None
     wsc: list[Comment | str]
 
 
 class SubsequentKeyValuePairProduction(Protocol):
+    _slice: T_TokenSlice
     wsc: list[Comment | str]
     first_key_value_pair: KeyValuePair | None
-    _slice: T_TokenSlice
 
 
 class T_FirstArrayValueProduction(Protocol):
+    _slice: T_TokenSlice
+
     def __getitem__(self, item: Literal[1]) -> Value:
         ...
 
     wsc: list[Comment | str]
 
 
 class T_SubsequentArrayValueProduction(Protocol):
+    _slice: T_TokenSlice
     first_array_value: Value | None
     wsc: list[Comment | str]
-    _slice: T_TokenSlice
 
 
 class T_ArrayValuesProduction(Protocol):
+    _slice: T_TokenSlice
     first_array_value: Value
     subsequent_array_value: list[Value]
 
 
 class T_JsonArrayProduction(Protocol):
-    array_values: tuple[list[Value], TrailingComma | None] | None
     _slice: T_TokenSlice
+    array_values: tuple[list[Value], TrailingComma | None] | None
     wsc: list[Comment | str]
 
 
 class T_IdentifierProduction(Protocol):
+    _slice: T_TokenSlice
+
     def __getitem__(self, item: Literal[0]) -> str:
         ...
 
-    _slice: T_TokenSlice
-
 
 class T_KeyProduction(Protocol):
     def __getitem__(self, item: Literal[1]) -> Identifier | DoubleQuotedString | SingleQuotedString:
         ...
 
 
 class T_NumberProduction(Protocol):
+    _slice: T_TokenSlice
+
     def __getitem__(self, item: Literal[0]) -> str:
         ...
 
-    _slice: T_TokenSlice
-
 
 class T_ValueNumberProduction(Protocol):
+    _slice: T_TokenSlice
     number: Infinity | NaN | Float | Integer
 
 
 class T_ExponentNotationProduction(Protocol):
+    _slice: T_TokenSlice
+
     def __getitem__(self, item: int) -> str:
         ...
 
 
 class T_StringTokenProduction(Protocol):
+    _slice: T_TokenSlice
+
     def __getitem__(self, item: Literal[0]) -> str:
         ...
 
-    _slice: T_TokenSlice
-
 
 class T_StringProduction(Protocol):
+    _slice: T_TokenSlice
+
     def __getitem__(self, item: Literal[0]) -> DoubleQuotedString | SingleQuotedString:
         ...
 
 
 class T_ValueProduction(Protocol):
+    _slice: T_TokenSlice
+
     def __getitem__(
         self, item: Literal[0]
     ) -> (
         DoubleQuotedString
         | SingleQuotedString
         | JSONObject
         | JSONArray
@@ -226,15 +264,15 @@
         self.errors: list[JSON5DecodeError] = []
         self.last_token: JSON5Token | None = None
         self.seen_tokens: list[JSON5Token] = []
         self.expecting: list[list[str]] = []
 
     @_('{ wsc } value { wsc }')
     def text(self, p: T_TextProduction) -> JSONText:
-        node = JSONText(value=p[1])
+        node = JSONText(value=p[1], tok=p.value._tok)
         for wsc in p.wsc0:
             node.wsc_before.append(wsc)
         for wsc in p.wsc1:
             node.wsc_after.append(wsc)
         return node
 
     @_('key { wsc } seen_colon COLON { wsc } object_value_seen value { wsc }')
@@ -243,15 +281,15 @@
         for wsc in p.wsc0:
             key.wsc_after.append(wsc)
         value = p[6]
         for wsc in p.wsc1:
             value.wsc_before.append(wsc)
         for wsc in p.wsc2:
             value.wsc_after.append(wsc)
-        return KeyValuePair(key=p.key, value=p.value, tok=getattr(key, 'tok'))
+        return KeyValuePair(key=p.key, value=p.value)
 
     @_('object_delimiter_seen COMMA { wsc } [ first_key_value_pair ]')
     def subsequent_key_value_pair(self, p: SubsequentKeyValuePairProduction) -> KeyValuePair | TrailingComma:
         node: KeyValuePair | TrailingComma
         if p.first_key_value_pair:
             node = p.first_key_value_pair
             for wsc in p.wsc:
@@ -279,15 +317,15 @@
         ret = [
             p.first_key_value_pair,
         ]
         num_sqvp = len(p.subsequent_key_value_pair)
         for index, value in enumerate(p.subsequent_key_value_pair):
             if isinstance(value, TrailingComma):
                 if index + 1 != num_sqvp:
-                    offending_token = value.tok
+                    offending_token = value._tok
                     self.errors.append(JSON5DecodeError("Syntax Error: multiple trailing commas", offending_token))
                 return ret, value
             else:
                 ret.append(value)
         return ret, None
 
     @_('')
@@ -317,18 +355,24 @@
     @_('')
     def seen_RBRACE(self, p: Any) -> None:
         self.expecting.pop()
 
     @_('seen_LBRACE LBRACE { wsc } [ key_value_pairs ] seen_RBRACE RBRACE')
     def json_object(self, p: T_JsonObjectProduction) -> JSONObject:
         if not p.key_value_pairs:
-            node = JSONObject(leading_wsc=list(p.wsc or []), tok=p._slice[0])
+            node = JSONObject(leading_wsc=list(p.wsc or []), tok=p._slice[1], end_tok=p._slice[5])
         else:
             kvps, trailing_comma = p.key_value_pairs
-            node = JSONObject(*kvps, trailing_comma=trailing_comma, leading_wsc=list(p.wsc or []), tok=p._slice[0])
+            node = JSONObject(
+                *kvps,
+                trailing_comma=trailing_comma,
+                leading_wsc=list(p.wsc or []),
+                tok=p._slice[1],
+                end_tok=p._slice[5],
+            )
 
         return node
 
     @_('array_value_seen value { wsc }')
     def first_array_value(self, p: T_FirstArrayValueProduction) -> Value:
         node = p[1]
         for wsc in p.wsc:
@@ -353,28 +397,28 @@
         ret = [
             p.first_array_value,
         ]
         num_values = len(p.subsequent_array_value)
         for index, value in enumerate(p.subsequent_array_value):
             if isinstance(value, TrailingComma):
                 if index + 1 != num_values:
-                    self.errors.append(JSON5DecodeError("Syntax Error: multiple trailing commas", value.tok))
+                    self.errors.append(JSON5DecodeError("Syntax Error: multiple trailing commas", value._tok))
                     return ret, value
                 return ret, value
             else:
                 ret.append(value)
         return ret, None
 
     @_('seen_LBRACKET LBRACKET { wsc } [ array_values ] seen_RBRACKET RBRACKET')
     def json_array(self, p: T_JsonArrayProduction) -> JSONArray:
         if not p.array_values:
-            node = JSONArray(tok=p._slice[1])
+            node = JSONArray(tok=p._slice[1], end_tok=p._slice[5])
         else:
             values, trailing_comma = p.array_values
-            node = JSONArray(*values, trailing_comma=trailing_comma, tok=p._slice[1])
+            node = JSONArray(*values, trailing_comma=trailing_comma, tok=p._slice[1], end_tok=p._slice[5])
 
         for wsc in p.wsc:
             node.leading_wsc.append(wsc)
 
         return node
 
     @_('')
@@ -426,41 +470,41 @@
         raw_value = p[0]
         if re.search(r'[89]+', raw_value):
             self.errors.append(JSON5DecodeError("Invalid octal format. Octal digits must be in range 0-7", p._slice[0]))
             return Integer(raw_value=oct(0), is_octal=True, tok=p._slice[0])
         return Integer(raw_value, is_octal=True, tok=p._slice[0])
 
     @_('INFINITY')  # type: ignore[no-redef]
-    def number(self, p: Any) -> Infinity:
-        return Infinity()
+    def number(self, p: T_AnyProduction) -> Infinity:
+        return Infinity(tok=p._slice[0])
 
     @_('NAN')  # type: ignore[no-redef]
-    def number(self, p: Any) -> NaN:
-        return NaN()
+    def number(self, p: T_AnyProduction) -> NaN:
+        return NaN(tok=p._slice[0])
 
     @_('MINUS number')
     def value(self, p: T_ValueNumberProduction) -> UnaryOp:
         if isinstance(p.number, Infinity):
             p.number.negative = True
-        node = UnaryOp(op='-', value=p.number)
+        node = UnaryOp(op='-', value=p.number, tok=p._slice[0], end_tok=p.number._end_tok)
         return node
 
     @_('PLUS number')  # type: ignore[no-redef]
     def value(self, p: T_ValueNumberProduction):
-        node = UnaryOp(op='+', value=p.number)
+        node = UnaryOp(op='+', value=p.number, tok=p._slice[0], end_tok=p.number._end_tok)
         return node
 
     @_('INTEGER EXPONENT', 'FLOAT EXPONENT')  # type: ignore[no-redef]
     def number(self, p: T_ExponentNotationProduction) -> Float:
         exp_notation = p[1][0]  # e or E
-        return Float(p[0] + p[1], exp_notation=exp_notation)
+        return Float(p[0] + p[1], exp_notation=exp_notation, tok=p._slice[0], end_tok=p._slice[1])
 
     @_('HEXADECIMAL')  # type: ignore[no-redef]
     def number(self, p: T_NumberProduction) -> Integer:
-        return Integer(p[0], is_hex=True)
+        return Integer(p[0], is_hex=True, tok=p._slice[0])
 
     @_('DOUBLE_QUOTE_STRING')
     def double_quoted_string(self, p: T_StringTokenProduction) -> DoubleQuotedString:
         raw_value = p[0]
         contents = raw_value[1:-1]
         terminator_in_string = re.search(r'(?<!\\)([\u000D\u2028\u2029]|(?<!\r)\n)', contents)
         if terminator_in_string:
@@ -513,24 +557,24 @@
         return SingleQuotedString(contents, raw_value=raw_value, tok=p._slice[0])
 
     @_('double_quoted_string', 'single_quoted_string')
     def string(self, p: T_StringProduction) -> SingleQuotedString | DoubleQuotedString:
         return p[0]
 
     @_('TRUE')
-    def boolean(self, p: Any) -> BooleanLiteral:
-        return BooleanLiteral(True)
+    def boolean(self, p: T_AnyProduction) -> BooleanLiteral:
+        return BooleanLiteral(True, tok=p._slice[0])
 
     @_('FALSE')  # type: ignore[no-redef]
-    def boolean(self, p: Any) -> BooleanLiteral:
-        return BooleanLiteral(False)
+    def boolean(self, p: T_AnyProduction) -> BooleanLiteral:
+        return BooleanLiteral(False, tok=p._slice[0])
 
     @_('NULL')
-    def null(self, p: Any) -> NullLiteral:
-        return NullLiteral()
+    def null(self, p: T_AnyProduction) -> NullLiteral:
+        return NullLiteral(tok=p._slice[0])
 
     @_(  # type: ignore[no-redef]
         'string',
         'json_object',
         'json_array',
         'boolean',
         'null',
@@ -554,16 +598,16 @@
         return node
 
     @_('UNTERMINATED_SINGLE_QUOTE_STRING', 'UNTERMINATED_DOUBLE_QUOTE_STRING')  # type: ignore[no-redef]
     def string(self, p: T_StringTokenProduction) -> SingleQuotedString | DoubleQuotedString:
         self.error(p._slice[0])
         raw = p[0]
         if raw.startswith('"'):
-            return DoubleQuotedString(raw[1:], raw_value=raw)
-        return SingleQuotedString(raw[1:], raw_value=raw)
+            return DoubleQuotedString(raw[1:], raw_value=raw, tok=p._slice[0])
+        return SingleQuotedString(raw[1:], raw_value=raw, tok=p._slice[0])
 
     def error(self, token: JSON5Token | None) -> JSON5Token | None:
         if token:
             if self.expecting:
                 expected = self.expecting[-1]
 
                 message = f"Syntax Error. Was expecting {' or '.join(expected)}"
```

### Comparing `json-five-1.0.0rc1/json5/tokenizer.py` & `json-five-1.1.0/json5/tokenizer.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,36 +5,55 @@
 from typing import Generator
 from typing import NoReturn
 
 import regex as re
 from sly import Lexer  # type: ignore
 from sly.lex import Token  # type: ignore
 
-from json5.utils import JSON5DecodeError
+from .utils import JSON5DecodeError
 
 logger = logging.getLogger(__name__)
 # logger.addHandler(logging.StreamHandler(stream=sys.stderr))
 # logger.setLevel(level=logging.DEBUG)
 
 
 class JSON5Token(Token):  # type: ignore[misc]
     '''
     Representation of a single token.
     '''
 
     def __init__(self, tok: Token, doc: str):
-        self.type = tok.type
-        self.value = tok.value
-        self.lineno = tok.lineno
-        self.index = tok.index
-        self.doc = doc
-        self.end = getattr(tok, 'end', None)
+        self.type: str | None = tok.type
+        self.value: str = tok.value
+        self.lineno: int = tok.lineno
+        self.index: int = tok.index
+        self.doc: str = doc
+        self.end: int = tok.end
+
+    @property
+    def colno(self) -> int:
+        line_start_index = self.doc.rfind('\n', 0, self.index) + 1
+        return self.index - line_start_index
+
+    @property
+    def end_colno(self) -> int:
+        return self.colno + self.end - self.index
+
+    @property
+    def end_lineno(self) -> int:
+        return self.lineno + self.value.count('\n')
 
     __slots__ = ('type', 'value', 'lineno', 'index', 'doc', 'end')
 
+    def __str__(self) -> str:
+        if self.value:
+            return self.value
+        else:
+            return ''
+
     def __repr__(self) -> str:
         return f'JSON5Token(type={self.type!r}, value={self.value!r}, lineno={self.lineno}, index={self.index}, end={self.end})'
 
 
 T_CallArg = typing.TypeVar('T_CallArg')
 _: typing.Callable[[str], typing.Callable[[T_CallArg], T_CallArg]]
 
@@ -80,16 +99,23 @@
     LBRACE = r'{'
     RBRACE = r'}'
     LBRACKET = r'\['
     RBRACKET = r'\]'
     COLON = r"\:"
     COMMA = r"\,"
 
-    DOUBLE_QUOTE_STRING = r'"(?:[^"\\]|\\.)*"'
-    SINGLE_QUOTE_STRING = r"'(?:[^'\\]|\\.)*'"
+    @_(r'"(?:[^"\\]|\\.)*"')
+    def DOUBLE_QUOTE_STRING(self, tok: JSON5Token) -> JSON5Token:
+        self.lineno += tok.value.count('\n')
+        return tok
+
+    @_(r"'(?:[^'\\]|\\.)*'")
+    def SINGLE_QUOTE_STRING(self, tok: JSON5Token) -> JSON5Token:
+        self.lineno += tok.value.count('\n')
+        return tok
 
     LINE_COMMENT = r"//[^\n]*"
 
     @_(r'/\*((.|\n))*?\*/')
     def BLOCK_COMMENT(self, tok: JSON5Token) -> JSON5Token:
         self.lineno += tok.value.count('\n')
         return tok
@@ -121,7 +147,13 @@
         raise JSON5DecodeError(f'Illegal character {t.value[0]!r} at index {self.index}', None)
 
 
 def tokenize(text: str) -> Generator[JSON5Token, None, None]:
     lexer = JSONLexer()
     tokens = lexer.tokenize(text)
     return tokens
+
+
+def reversed_enumerate(tokens: typing.Sequence[JSON5Token]) -> typing.Generator[tuple[int, JSON5Token], None, None]:
+    for i in reversed(range(len(tokens))):
+        tok = tokens[i]
+        yield i, tok
```

### Comparing `json-five-1.0.0rc1/json_five.egg-info/SOURCES.txt` & `json-five-1.1.0/json_five.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -18,11 +18,12 @@
 json_five.egg-info/top_level.txt
 tests/test_errors.py
 tests/test_json5_dump.py
 tests/test_json5_load.py
 tests/test_json5_official_tests.py
 tests/test_json_helpers.py
 tests/test_loads_options.py
+tests/test_model.py
 tests/test_model_loader_dumper.py
 tests/test_modelizer.py
 tests/test_regressions.py
 tests/test_roundtrip.py
```

### Comparing `json-five-1.0.0rc1/setup.cfg` & `json-five-1.1.0/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = json-five
-version = 1.0.0rc1
+version = 1.1.0
 url = https://github.com/spyoungtech/json-five
 license = Apache
 author = Spencer Phillip Young
 author_email = spencer.young@spyoung.com
 description = A JSON5 parser that, among other features, supports round-trip preservation of comments
 long_description = file: README.md
 long_description_content_type = text/markdown
@@ -17,15 +17,15 @@
 	Programming Language :: Python :: 3.11
 license_files = LICENSE
 
 [options]
 packages = json5
 python_requires = >=3.8.0
 install_requires = 
-	sly
+	sly>=0.5
 	regex
 
 [options.package_data]
 json5 = 
 	py.typed
 
 [egg_info]
```

### Comparing `json-five-1.0.0rc1/tests/test_errors.py` & `json-five-1.1.0/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `json-five-1.0.0rc1/tests/test_json5_dump.py` & `json-five-1.1.0/tests/test_json5_dump.py`

 * *Files identical despite different names*

### Comparing `json-five-1.0.0rc1/tests/test_json5_load.py` & `json-five-1.1.0/tests/test_json5_load.py`

 * *Files identical despite different names*

### Comparing `json-five-1.0.0rc1/tests/test_json5_official_tests.py` & `json-five-1.1.0/tests/test_json5_official_tests.py`

 * *Files identical despite different names*

### Comparing `json-five-1.0.0rc1/tests/test_json_helpers.py` & `json-five-1.1.0/tests/test_json_helpers.py`

 * *Files identical despite different names*

### Comparing `json-five-1.0.0rc1/tests/test_loads_options.py` & `json-five-1.1.0/tests/test_loads_options.py`

 * *Files identical despite different names*

### Comparing `json-five-1.0.0rc1/tests/test_model_loader_dumper.py` & `json-five-1.1.0/tests/test_model_loader_dumper.py`

 * *Files identical despite different names*

### Comparing `json-five-1.0.0rc1/tests/test_modelizer.py` & `json-five-1.1.0/tests/test_modelizer.py`

 * *Files identical despite different names*

### Comparing `json-five-1.0.0rc1/tests/test_regressions.py` & `json-five-1.1.0/tests/test_regressions.py`

 * *Files identical despite different names*

### Comparing `json-five-1.0.0rc1/tests/test_roundtrip.py` & `json-five-1.1.0/tests/test_roundtrip.py`

 * *Files identical despite different names*

