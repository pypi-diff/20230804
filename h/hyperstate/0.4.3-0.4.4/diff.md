# Comparing `tmp/hyperstate-0.4.3.tar.gz` & `tmp/hyperstate-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyperstate-0.4.3.tar", max compression
+gzip compressed data, was "hyperstate-0.4.4.tar", max compression
```

## Comparing `hyperstate-0.4.3.tar` & `hyperstate-0.4.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     9693 2023-03-14 16:09:48.389060 hyperstate-0.4.3/LICENSE-APACHE
--rw-r--r--   0        0        0     1071 2023-03-14 16:09:48.389060 hyperstate-0.4.3/LICENSE-MIT
--rw-r--r--   0        0        0    13965 2023-03-14 16:09:48.389060 hyperstate-0.4.3/README.md
--rw-r--r--   0        0        0     1101 2023-03-14 16:09:48.389060 hyperstate-0.4.3/hyperstate/__init__.py
--rw-r--r--   0        0        0     5062 2023-03-14 16:09:48.389060 hyperstate-0.4.3/hyperstate/command.py
--rw-r--r--   0        0        0    18625 2023-03-14 16:09:48.389060 hyperstate-0.4.3/hyperstate/hyperstate.py
--rw-r--r--   0        0        0     4557 2023-03-14 16:09:48.389060 hyperstate-0.4.3/hyperstate/lazy.py
--rw-r--r--   0        0        0     1245 2023-03-14 16:09:48.389060 hyperstate-0.4.3/hyperstate/msgpack_torch.py
--rw-r--r--   0        0        0        0 2023-03-14 16:09:48.389060 hyperstate-0.4.3/hyperstate/py.typed
--rw-r--r--   0        0        0     2383 2023-03-14 16:09:48.389060 hyperstate-0.4.3/hyperstate/schedule.py
--rw-r--r--   0        0        0        0 2023-03-14 16:09:48.389060 hyperstate-0.4.3/hyperstate/schema/__init__.py
--rw-r--r--   0        0        0     3843 2023-03-14 16:09:48.389060 hyperstate-0.4.3/hyperstate/schema/help.py
--rw-r--r--   0        0        0      290 2023-03-14 16:09:48.393060 hyperstate-0.4.3/hyperstate/schema/namedtuple_utils.py
--rw-r--r--   0        0        0     8520 2023-03-14 16:09:48.393060 hyperstate-0.4.3/hyperstate/schema/rewrite_rule.py
--rw-r--r--   0        0        0     7352 2023-03-14 16:09:48.393060 hyperstate-0.4.3/hyperstate/schema/schema_change.py
--rw-r--r--   0        0        0    17281 2023-03-14 16:09:48.393060 hyperstate-0.4.3/hyperstate/schema/schema_checker.py
--rw-r--r--   0        0        0      536 2023-03-14 16:09:48.393060 hyperstate-0.4.3/hyperstate/schema/test_dump_schema.py
--rw-r--r--   0        0        0     2740 2023-03-14 16:09:48.393060 hyperstate-0.4.3/hyperstate/schema/test_help.py
--rw-r--r--   0        0        0    17173 2023-03-14 16:09:48.393060 hyperstate-0.4.3/hyperstate/schema/test_schema_evolution.py
--rw-r--r--   0        0        0     9788 2023-03-14 16:09:48.393060 hyperstate-0.4.3/hyperstate/schema/types.py
--rw-r--r--   0        0        0     3218 2023-03-14 16:09:48.393060 hyperstate-0.4.3/hyperstate/schema/versioned.py
--rw-r--r--   0        0        0    12851 2023-03-14 16:09:48.393060 hyperstate-0.4.3/hyperstate/serde.py
--rw-r--r--   0        0        0     4097 2023-03-14 16:09:48.393060 hyperstate-0.4.3/hyperstate/test_checkpoint.py
--rw-r--r--   0        0        0      861 2023-03-14 16:09:48.393060 hyperstate-0.4.3/hyperstate/test_override.py
--rw-r--r--   0        0        0      900 2023-03-14 16:09:48.393060 hyperstate-0.4.3/pyproject.toml
--rw-r--r--   0        0        0    14945 1970-01-01 00:00:00.000000 hyperstate-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0     9693 2023-08-04 16:24:00.565780 hyperstate-0.4.4/LICENSE-APACHE
+-rw-r--r--   0        0        0     1071 2023-08-04 16:24:00.565780 hyperstate-0.4.4/LICENSE-MIT
+-rw-r--r--   0        0        0    13965 2023-08-04 16:24:00.565780 hyperstate-0.4.4/README.md
+-rw-r--r--   0        0        0     1101 2023-08-04 16:24:00.565780 hyperstate-0.4.4/hyperstate/__init__.py
+-rw-r--r--   0        0        0     5062 2023-08-04 16:24:00.565780 hyperstate-0.4.4/hyperstate/command.py
+-rw-r--r--   0        0        0    18625 2023-08-04 16:24:00.565780 hyperstate-0.4.4/hyperstate/hyperstate.py
+-rw-r--r--   0        0        0     4557 2023-08-04 16:24:00.565780 hyperstate-0.4.4/hyperstate/lazy.py
+-rw-r--r--   0        0        0     1245 2023-08-04 16:24:00.565780 hyperstate-0.4.4/hyperstate/msgpack_torch.py
+-rw-r--r--   0        0        0        0 2023-08-04 16:24:00.565780 hyperstate-0.4.4/hyperstate/py.typed
+-rw-r--r--   0        0        0     2383 2023-08-04 16:24:00.565780 hyperstate-0.4.4/hyperstate/schedule.py
+-rw-r--r--   0        0        0        0 2023-08-04 16:24:00.565780 hyperstate-0.4.4/hyperstate/schema/__init__.py
+-rw-r--r--   0        0        0     3843 2023-08-04 16:24:00.565780 hyperstate-0.4.4/hyperstate/schema/help.py
+-rw-r--r--   0        0        0      290 2023-08-04 16:24:00.565780 hyperstate-0.4.4/hyperstate/schema/namedtuple_utils.py
+-rw-r--r--   0        0        0     8520 2023-08-04 16:24:00.565780 hyperstate-0.4.4/hyperstate/schema/rewrite_rule.py
+-rw-r--r--   0        0        0     7352 2023-08-04 16:24:00.565780 hyperstate-0.4.4/hyperstate/schema/schema_change.py
+-rw-r--r--   0        0        0    17281 2023-08-04 16:24:00.565780 hyperstate-0.4.4/hyperstate/schema/schema_checker.py
+-rw-r--r--   0        0        0      536 2023-08-04 16:24:00.565780 hyperstate-0.4.4/hyperstate/schema/test_dump_schema.py
+-rw-r--r--   0        0        0     2740 2023-08-04 16:24:00.565780 hyperstate-0.4.4/hyperstate/schema/test_help.py
+-rw-r--r--   0        0        0    17173 2023-08-04 16:24:00.565780 hyperstate-0.4.4/hyperstate/schema/test_schema_evolution.py
+-rw-r--r--   0        0        0    10490 2023-08-04 16:24:00.565780 hyperstate-0.4.4/hyperstate/schema/types.py
+-rw-r--r--   0        0        0     3218 2023-08-04 16:24:00.565780 hyperstate-0.4.4/hyperstate/schema/versioned.py
+-rw-r--r--   0        0        0    13912 2023-08-04 16:24:00.565780 hyperstate-0.4.4/hyperstate/serde.py
+-rw-r--r--   0        0        0     4149 2023-08-04 16:24:00.565780 hyperstate-0.4.4/hyperstate/test_checkpoint.py
+-rw-r--r--   0        0        0      861 2023-08-04 16:24:00.565780 hyperstate-0.4.4/hyperstate/test_override.py
+-rw-r--r--   0        0        0      900 2023-08-04 16:24:00.565780 hyperstate-0.4.4/pyproject.toml
+-rw-r--r--   0        0        0    14945 1970-01-01 00:00:00.000000 hyperstate-0.4.4/PKG-INFO
```

### Comparing `hyperstate-0.4.3/LICENSE-APACHE` & `hyperstate-0.4.4/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `hyperstate-0.4.3/LICENSE-MIT` & `hyperstate-0.4.4/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `hyperstate-0.4.3/README.md` & `hyperstate-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `hyperstate-0.4.3/hyperstate/__init__.py` & `hyperstate-0.4.4/hyperstate/__init__.py`

 * *Files identical despite different names*

### Comparing `hyperstate-0.4.3/hyperstate/command.py` & `hyperstate-0.4.4/hyperstate/command.py`

 * *Files identical despite different names*

### Comparing `hyperstate-0.4.3/hyperstate/hyperstate.py` & `hyperstate-0.4.4/hyperstate/hyperstate.py`

 * *Files identical despite different names*

### Comparing `hyperstate-0.4.3/hyperstate/lazy.py` & `hyperstate-0.4.4/hyperstate/lazy.py`

 * *Files identical despite different names*

### Comparing `hyperstate-0.4.3/hyperstate/msgpack_torch.py` & `hyperstate-0.4.4/hyperstate/msgpack_torch.py`

 * *Files identical despite different names*

### Comparing `hyperstate-0.4.3/hyperstate/schedule.py` & `hyperstate-0.4.4/hyperstate/schedule.py`

 * *Files identical despite different names*

### Comparing `hyperstate-0.4.3/hyperstate/schema/help.py` & `hyperstate-0.4.4/hyperstate/schema/help.py`

 * *Files identical despite different names*

### Comparing `hyperstate-0.4.3/hyperstate/schema/rewrite_rule.py` & `hyperstate-0.4.4/hyperstate/schema/rewrite_rule.py`

 * *Files identical despite different names*

### Comparing `hyperstate-0.4.3/hyperstate/schema/schema_change.py` & `hyperstate-0.4.4/hyperstate/schema/schema_change.py`

 * *Files identical despite different names*

### Comparing `hyperstate-0.4.3/hyperstate/schema/schema_checker.py` & `hyperstate-0.4.4/hyperstate/schema/schema_checker.py`

 * *Files identical despite different names*

### Comparing `hyperstate-0.4.3/hyperstate/schema/test_dump_schema.py` & `hyperstate-0.4.4/hyperstate/schema/test_dump_schema.py`

 * *Files identical despite different names*

### Comparing `hyperstate-0.4.3/hyperstate/schema/test_help.py` & `hyperstate-0.4.4/hyperstate/schema/test_help.py`

 * *Files identical despite different names*

### Comparing `hyperstate-0.4.3/hyperstate/schema/test_schema_evolution.py` & `hyperstate-0.4.4/hyperstate/schema/test_schema_evolution.py`

 * *Files identical despite different names*

### Comparing `hyperstate-0.4.3/hyperstate/schema/types.py` & `hyperstate-0.4.4/hyperstate/schema/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 
 T = TypeVar("T")
 
 
 Type = typing.Union[
     "Primitive",
     "List",
+    "Tuple",
     "Dict",
     "Union",
     "Struct",
     "Option",
     "Enum",
     "Literal",
     "Nothing",
@@ -57,14 +58,33 @@
             self == other
             or (isinstance(other, List) and self.inner.is_subtype(other.inner))
             or (isinstance(other, Option) and self.is_subtype(other.type))
         )
 
 
 @dataclass(eq=True, frozen=True)
+class Tuple:
+    inner: typing.List[Type]
+
+    def __repr__(self) -> str:
+        return f"Tuple[{self.inner}]"
+
+    def is_subtype(self, other: Type) -> bool:
+        return (
+            self == other
+            or (
+                isinstance(other, Tuple)
+                and all(t.is_subtype(o) for t, o in zip(self.inner, other.inner))
+                and len(self.inner) == len(other.inner)
+            )
+            or (isinstance(other, Option) and self.is_subtype(other.type))
+        )
+
+
+@dataclass(eq=True, frozen=True)
 class Dict:
     key: Type
     val: Type
 
     def __repr__(self) -> str:
         return f"Dict[{self.key}, {self.val}]"
 
@@ -219,14 +239,16 @@
         return Primitive(type="str")
     elif clz == bool:
         return Primitive(type="bool")
     elif clz == float:
         return Primitive(type="float")
     elif hasattr(clz, "__origin__") and clz.__origin__ == list:
         return List(materialize_type(clz.__args__[0]))
+    elif hasattr(clz, "__origin__") and clz.__origin__ == tuple:
+        return Tuple([materialize_type(arg) for arg in clz.__args__])
     elif hasattr(clz, "__origin__") and clz.__origin__ == dict:
         return Dict(
             materialize_type(clz.__args__[0]), materialize_type(clz.__args__[1])
         )
     elif is_optional(clz):
         return Option(materialize_type(clz.__args__[0]))
     elif hasattr(clz, "__origin__") and clz.__origin__ == typing.Union:
@@ -264,14 +286,15 @@
         variants = {}
         for name, value in clz.__members__.items():
             variants[name] = value.value
         return Enum(clz.__name__, variants)
     elif typing.get_origin(clz) == typing.Literal:
         return Literal(list(typing.get_args(clz)))
     else:
+        breakpoint()
         raise ValueError(f"Unsupported type: {clz}")
 
 
 def is_optional(clz: Any) -> bool:
     return (
         hasattr(clz, "__origin__")
         and clz.__origin__ is typing.Union
```

### Comparing `hyperstate-0.4.3/hyperstate/schema/versioned.py` & `hyperstate-0.4.4/hyperstate/schema/versioned.py`

 * *Files identical despite different names*

### Comparing `hyperstate-0.4.3/hyperstate/serde.py` & `hyperstate-0.4.4/hyperstate/serde.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,17 +87,44 @@
         }
         for serializer in serializers:
             serializer.modify_dataclass_attrs(value, attrs, file)
         if named_tuples:
             return namedtuple(value.__class__.__name__, attrs.keys())(**attrs)
         else:
             return attrs
-    elif isinstance(value, dict) or isinstance(value, list):
-        # TODO: recurse
-        return value
+    elif isinstance(value, dict):
+        return {
+            k: asdict(
+                value=v,
+                named_tuples=named_tuples,
+                serializers=serializers,
+                file=k if file == "" else f"{file}.{k}",
+            )
+            for k, v in value.items()
+        }
+    elif isinstance(value, list):
+        return [
+            asdict(
+                v,
+                named_tuples,
+                serializers,
+                file=str(i) if file == "" else f"{file}.{i}",
+            )
+            for i, v in enumerate(value)
+        ]
+    elif isinstance(value, tuple):
+        return tuple(
+            asdict(
+                v,
+                named_tuples,
+                serializers,
+                file=str(i) if file == "" else f"{file}.{i}",
+            )
+            for i, v in enumerate(value)
+        )
     elif isinstance(value, Enum):
         return value.name
     elif (
         isinstance(value, int)
         or isinstance(value, float)
         or isinstance(value, str)
         or isinstance(value, bool)
@@ -192,14 +219,23 @@
         and len(clz.__args__) == 1  # type: ignore
         and clz == List[clz.__args__]  # type: ignore
         and isinstance(value, list)
     ):
         return [from_dict(clz.__args__[0], v, deserializers, fpath + f"[{i}]") for i, v in enumerate(value)]  # type: ignore
     elif (
         hasattr(clz, "__args__")
+        and clz == Tuple[clz.__args__]  # type: ignore
+        and isinstance(value, tuple)
+    ):
+        return tuple(
+            from_dict(clz.__args__[i], v, deserializers, fpath + f"[{i}]")  # type: ignore
+            for i, v in enumerate(value)
+        )
+    elif (
+        hasattr(clz, "__args__")
         and len(clz.__args__) == 2  # type: ignore
         and clz == Dict[clz.__args__]  # type: ignore
         and isinstance(value, dict)
     ):
         return {
             k: from_dict(clz.__args__[1], v, deserializers, fpath=f"{fpath}.{k}")  # type: ignore
             for k, v in value.items()
```

### Comparing `hyperstate-0.4.3/hyperstate/test_checkpoint.py` & `hyperstate-0.4.4/hyperstate/test_checkpoint.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 from dataclasses import dataclass
 import tempfile
 import textwrap
 import os
-from typing import Any, Dict, List, Union
+from typing import Any, Dict, List, Tuple, Union
 
 import numpy as np
 
 from hyperstate.hyperstate import StateManager
 from hyperstate.lazy import Lazy, Serializable
 
 
 @dataclass(eq=True)
 class PPO:
     cliprange: float = 0.2
     gamma: float = 0.99
     lambd: float = 0.95
     entcoeff: float = 0.01
     value_loss_coeff: float = 1
+    betas: Tuple[float, float] = (0.9, 0.98)
 
 
 @dataclass(eq=True)
 class Entity:
     features: List[str]
```

### Comparing `hyperstate-0.4.3/hyperstate/test_override.py` & `hyperstate-0.4.4/hyperstate/test_override.py`

 * *Files identical despite different names*

### Comparing `hyperstate-0.4.3/pyproject.toml` & `hyperstate-0.4.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hyperstate"
-version = "0.4.3"
+version = "0.4.4"
 description = "Library for managing hyperparameters and mutable state of machine learning training systems."
 authors = ["Clemens Winter <clemenswinter1@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 classifiers = [
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
     "License :: OSI Approved :: Apache Software License",
```

### Comparing `hyperstate-0.4.3/PKG-INFO` & `hyperstate-0.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyperstate
-Version: 0.4.3
+Version: 0.4.4
 Summary: Library for managing hyperparameters and mutable state of machine learning training systems.
 License: MIT
 Author: Clemens Winter
 Author-email: clemenswinter1@gmail.com
 Requires-Python: >=3.7.1,<3.11.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: License :: OSI Approved :: MIT License
```

