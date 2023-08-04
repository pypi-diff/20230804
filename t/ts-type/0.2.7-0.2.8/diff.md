# Comparing `tmp/ts_type-0.2.7.tar.gz` & `tmp/ts_type-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ts_type-0.2.7.tar", last modified: Fri Apr 28 12:37:56 2023, max compression
+gzip compressed data, was "ts_type-0.2.8.tar", last modified: Fri Aug  4 08:04:12 2023, max compression
```

## Comparing `ts_type-0.2.7.tar` & `ts_type-0.2.8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:37:56.391476 ts_type-0.2.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-28 12:37:47.000000 ts_type-0.2.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7233 2023-04-28 12:37:56.387476 ts_type-0.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6718 2023-04-28 12:37:47.000000 ts_type-0.2.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-28 12:37:47.000000 ts_type-0.2.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 12:37:56.391476 ts_type-0.2.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-04-28 12:37:47.000000 ts_type-0.2.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:37:56.387476 ts_type-0.2.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    13146 2023-04-28 12:37:47.000000 ts_type-0.2.7/tests/test_ts_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:37:56.387476 ts_type-0.2.7/ts_type/
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-04-28 12:37:47.000000 ts_type-0.2.7/ts_type/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8684 2023-04-28 12:37:47.000000 ts_type-0.2.7/ts_type/builders.py
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-28 12:37:47.000000 ts_type-0.2.7/ts_type/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-04-28 12:37:47.000000 ts_type-0.2.7/ts_type/generators.py
--rw-r--r--   0 runner    (1001) docker     (123)    11084 2023-04-28 12:37:47.000000 ts_type-0.2.7/ts_type/nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 12:37:47.000000 ts_type-0.2.7/ts_type/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-04-28 12:37:47.000000 ts_type-0.2.7/ts_type/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-28 12:37:47.000000 ts_type-0.2.7/ts_type/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:37:56.387476 ts_type-0.2.7/ts_type.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7233 2023-04-28 12:37:56.000000 ts_type-0.2.7/ts_type.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-04-28 12:37:56.000000 ts_type-0.2.7/ts_type.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 12:37:56.000000 ts_type-0.2.7/ts_type.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-28 12:37:56.000000 ts_type-0.2.7/ts_type.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 08:04:12.296545 ts_type-0.2.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-08-04 08:03:59.000000 ts_type-0.2.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7233 2023-08-04 08:04:12.296545 ts_type-0.2.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6718 2023-08-04 08:03:59.000000 ts_type-0.2.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-08-04 08:03:59.000000 ts_type-0.2.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 08:04:12.296545 ts_type-0.2.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-08-04 08:03:59.000000 ts_type-0.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 08:04:12.296545 ts_type-0.2.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    13146 2023-08-04 08:03:59.000000 ts_type-0.2.8/tests/test_ts_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 08:04:12.296545 ts_type-0.2.8/ts_type/
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-08-04 08:03:59.000000 ts_type-0.2.8/ts_type/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8899 2023-08-04 08:03:59.000000 ts_type-0.2.8/ts_type/builders.py
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-08-04 08:03:59.000000 ts_type-0.2.8/ts_type/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-08-04 08:03:59.000000 ts_type-0.2.8/ts_type/generators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15174 2023-08-04 08:03:59.000000 ts_type-0.2.8/ts_type/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 08:03:59.000000 ts_type-0.2.8/ts_type/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-08-04 08:03:59.000000 ts_type-0.2.8/ts_type/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-04 08:03:59.000000 ts_type-0.2.8/ts_type/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 08:04:12.296545 ts_type-0.2.8/ts_type.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7233 2023-08-04 08:04:12.000000 ts_type-0.2.8/ts_type.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-08-04 08:04:12.000000 ts_type-0.2.8/ts_type.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 08:04:12.000000 ts_type-0.2.8/ts_type.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-04 08:04:12.000000 ts_type-0.2.8/ts_type.egg-info/top_level.txt
```

### Comparing `ts_type-0.2.7/LICENSE` & `ts_type-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ts_type-0.2.7/PKG-INFO` & `ts_type-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ts_type
-Version: 0.2.7
+Version: 0.2.8
 Summary: ts_type generates typescript's type from python code
 Home-page: https://github.com/saryou/ts_type
 Author: Ryosuke Sasaki
 Author-email: saryou.ssk@gmail.com
 Project-URL: Bug Tracker, https://github.com/saryou/ts_type/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ts_type-0.2.7/README.md` & `ts_type-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `ts_type-0.2.7/setup.py` & `ts_type-0.2.8/setup.py`

 * *Files identical despite different names*

### Comparing `ts_type-0.2.7/tests/test_ts_type.py` & `ts_type-0.2.8/tests/test_ts_type.py`

 * *Files identical despite different names*

### Comparing `ts_type-0.2.7/ts_type/__init__.py` & `ts_type-0.2.8/ts_type/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,23 +3,26 @@
 from .builders import NodeCompatible as NodeCompatible  # noqa
 from .exceptions import UnknownTypeError as UnknownTypeError  # noqa
 from .generators import TypeDefinitionGenerator as TypeDefinitionGenerator  # noqa
 from .generators import generator as generator  # noqa
 from .generators import gen_type as gen_type  # noqa
 from .nodes import Array as Array  # noqa
 from .nodes import Boolean as Boolean  # noqa
+from .nodes import Conditional as Conditional  # noqa
 from .nodes import Dict as Dict  # noqa
 from .nodes import DictKeyType as DictKeyType  # noqa
 from .nodes import Exclude as Exclude  # noqa
 from .nodes import Extract as Extract  # noqa
 from .nodes import GlobalTypeNode as GlobalTypeNode  # noqa
+from .nodes import Infer as Infer  # noqa
 from .nodes import Intersection as Intersection  # noqa
 from .nodes import Keyof as Keyof  # noqa
 from .nodes import Literal as Literal  # noqa
 from .nodes import Lookup as Lookup  # noqa
+from .nodes import Never as Never  # noqa
 from .nodes import NonNullable as NonNullable  # noqa
 from .nodes import Null as Null  # noqa
 from .nodes import Number as Number  # noqa
 from .nodes import Object as Object  # noqa
 from .nodes import Omit as Omit  # noqa
 from .nodes import Partial as Partial  # noqa
 from .nodes import Pick as Pick  # noqa
```

### Comparing `ts_type-0.2.7/ts_type/builders.py` & `ts_type-0.2.8/ts_type/builders.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import re
 from datetime import datetime, date, time
 from enum import Enum
 from contextlib import contextmanager
 from dataclasses import fields as dc_fields, is_dataclass
 from importlib import import_module
 from typing import Optional, Any, Type, Callable, Union, ForwardRef, TypeVar,\
-    Literal, List, Dict, Set, Tuple, cast, Generic
+    Literal, List, Dict, Set, Tuple, cast, Generic, Sequence
 
 from .exceptions import UnknownTypeError
 from .utils import resolve_typevar
 from . import nodes
 
 
 T = TypeVar('T')
@@ -46,17 +46,19 @@
 
         to_export = refs_to_export or set(self.definitions.keys())
         ref_names = [k for k in self.definitions if k in to_export]\
             + [k for k in self.definitions if k not in to_export]
 
         def render(k: str) -> str:
             export = 'export ' if k in to_export else ''
+
             ref = nodes.Reference(k)
             node = ctx.definitions[k]
-            lhs = f'{export}type {ref.render(ctx)}'
+            with ctx.enable_typevar_definition():
+                lhs = f'{export}type {ref.render(ctx)}'
             rhs = f'{node.render(ctx)};'
             return f'{lhs} = {rhs}'
 
         return '\n\n'.join([render(k) for k in ref_names])
 
     def type_to_node(self, t: Any) -> nodes.TypeNode:
         if t in [None, type(None)]:
@@ -148,15 +150,16 @@
         def from_identifier(cls, t: str) -> 'NodeBuilder.RefSource':
             return cls(type=None, identifier=t)
 
     def define_ref_node(
             self,
             source: Union[RefSource, type, str],
             define: Callable[[], nodes.TypeNode],
-            generic_params: Optional[List[TypeVar]] = None,
+            generic_params: Optional[Sequence[
+                Union[TypeVar, nodes.TypeVariable]]] = None,
             ref_typevars: List[nodes.TypeNode] = []) -> nodes.Reference:
         if isinstance(source, str):
             source = self.RefSource.from_identifier(source)
         elif isinstance(source, type):
             source = self.RefSource.from_type(source)
 
         t = source.type
@@ -167,15 +170,17 @@
             defs[_id] = nodes.TypeNode()
 
             try:
                 with self._begin_module_context(t):
                     type_node = define()
                     if generic_params is not None:
                         type_node.add_generic_params(
-                            [nodes.TypeVariable(p) for p in generic_params])
+                            [p if isinstance(p, nodes.TypeVariable)
+                             else nodes.TypeVariable(p)
+                             for p in generic_params])
                     elif (params := getattr(t, '__parameters__', None)):
                         type_node.add_generic_params(
                             [nodes.TypeVariable(p) for p in params])
                 defs[_id] = type_node
             except Exception:
                 del defs[_id]
                 raise
```

### Comparing `ts_type-0.2.7/ts_type/generators.py` & `ts_type-0.2.8/ts_type/generators.py`

 * *Files identical despite different names*

### Comparing `ts_type-0.2.7/ts_type/nodes.py` & `ts_type-0.2.8/ts_type/nodes.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 import typing
+import contextlib
 
 
 class RenderContext:
     def __init__(self,
                  definitions: typing.Dict[str, 'TypeNode'],
                  indent_level: int = 0,
                  indent_unit: str = ' ' * 4,):
         self.definitions = definitions
         self.indent_level = indent_level
         self.indent_unit = indent_unit
+        self.typevar_definition_enabled = False
 
     def clone(self, **override) -> 'RenderContext':
         kwargs: typing.Dict[str, typing.Any] = dict(
             definitions=self.definitions,
             indent_level=self.indent_level,
             indent_unit=self.indent_unit)
         kwargs.update(override)
@@ -23,23 +25,64 @@
         return self.indent_unit * self.indent_level
 
     def resolve_ref(self, node: 'TypeNode') -> 'TypeNode':
         if isinstance(node, Reference):
             return self.resolve_ref(self.definitions[node.identifier])
         return node
 
+    def resolve_typevars(self, node: 'TypeNode')\
+            -> typing.List['TypeVariable']:
+        if isinstance(node, Reference):
+            return self.resolve_typevars(self.resolve_ref(node))
+        elif node is (proxy := node.get_proxy_for_generic_params()):
+            return node.get_generic_params()
+        else:
+            return self.resolve_typevars(proxy)
+
+    def render_typevars(
+            self,
+            typevars: typing.Union[
+                'TypeNode',
+                typing.Sequence[typing.Union['TypeVariable', 'TypeNode']],
+            ],
+            brackets: bool = True) -> str:
+        if isinstance(typevars, TypeNode):
+            typevars = self.resolve_typevars(typevars)
+        defs = ', '.join([n.render(self) for n in typevars])
+        if not brackets:
+            return defs
+        return ''.join(['<', defs, '>']) if typevars else ''
+
+    @contextlib.contextmanager
+    def enable_typevar_definition(self):
+        self.typevar_definition_enabled = True
+        yield
+        self.typevar_definition_enabled = False
+
 
 class TypeNode:
     def get_generic_params(self) -> typing.List['TypeVariable']:
+        proxy = self.get_proxy_for_generic_params()
+        if proxy is not self:
+            return proxy.get_generic_params()
+
         return getattr(self, '__params__', [])
 
     def add_generic_params(self, variables: typing.List['TypeVariable']):
+        proxy = self.get_proxy_for_generic_params()
+        if proxy is not self:
+            proxy.add_generic_params(variables)
+            return
+
         self.__params__ = self.get_generic_params()
         self.__params__.extend(variables)
 
+    def get_proxy_for_generic_params(self) -> 'TypeNode':
+        return self
+
     def render(self, context: RenderContext) -> str:
         raise NotImplementedError()
 
 
 class DictKeyType(TypeNode):
     def render_dict_key(self, context: RenderContext) -> str:
         return f'[K in {self.render(context)}]'
@@ -82,55 +125,65 @@
 
 
 class Unknown(GlobalTypeNode):
     def render(self, context: RenderContext) -> str:
         return 'unknown'
 
 
+class Never(GlobalTypeNode):
+    def render(self, context: RenderContext) -> str:
+        return 'never'
+
+
 class Literal(GlobalTypeNode):
     def __init__(self, literal: str):
         self.literal = literal
 
     def render(self, context: RenderContext) -> str:
         return self.literal
 
     def __eq__(self, other):
         return super().__eq__(other)\
             and self.literal == other.literal
 
 
 class TypeVariable(GlobalTypeNode):
-    def __init__(self, typevar: typing.TypeVar):
+    def __init__(self,
+                 typevar: typing.TypeVar,
+                 condition: typing.Optional[TypeNode] = None,
+                 default: typing.Optional[TypeNode] = None):
         self.typevar = typevar
+        self.condition = condition
+        self.default = default
 
     def render(self, context: RenderContext) -> str:
-        return self.typevar.__name__
+        ret = self.typevar.__name__
+        if context.typevar_definition_enabled:
+            if self.condition is not None:
+                ret = f'{ret} extends {self.condition.render(context)}'
+            if self.default is not None:
+                ret = f'{ret} = {self.default.render(context)}'
+        return ret
 
     def __eq__(self, other):
         return super().__eq__(other)\
             and self.typevar == other.typevar
 
 
 class Reference(DictKeyType):
     def __init__(self,
                  identifier: str,
                  typevars: typing.List[TypeNode] = []):
         self.identifier = identifier
         self.typevars = typevars
 
     def render(self, context: RenderContext) -> str:
-        ref_typevars = context.resolve_ref(self).get_generic_params()
+        ref_typevars = context.resolve_typevars(self)
         typevars = [*self.typevars, *ref_typevars[len(self.typevars):]]
-        return self.identifier + self.__render_typevars(context, typevars)
-
-    def __render_typevars(self,
-                          context: RenderContext,
-                          typevars: typing.Sequence[TypeNode]) -> str:
-        defs = [n.render(context) for n in typevars]
-        return ''.join(['<', ', '.join(defs), '>']) if typevars else ''
+        return self.identifier + context.render_typevars(typevars)
 
     def __eq__(self, other):
         return isinstance(other, Reference)\
             and self.identifier == other.identifier\
             and self.typevars == other.typevars
 
 
@@ -180,14 +233,17 @@
     def render(self, context: RenderContext):
         return _render_with_parenthesis(self.of, context) + '[]'
 
     def __eq__(self, other):
         return isinstance(other, Array)\
             and self.of == other.of
 
+    def get_proxy_for_generic_params(self) -> 'TypeNode':
+        return self.of
+
 
 class Dict(TypeNode):
     def __init__(self,
                  key: DictKeyType,
                  value: TypeNode):
         self.key = key
         self.value = value
@@ -202,14 +258,17 @@
         ])
 
     def __eq__(self, other):
         return isinstance(other, Dict)\
             and self.key == other.key\
             and self.value == other.value
 
+    def get_proxy_for_generic_params(self) -> 'TypeNode':
+        return self.value
+
 
 class Union(DictKeyType):
     def __init__(self, of: typing.List[TypeNode]):
         self.of = self._unique(self._flatten(of))
         assert self.of
 
     def _flatten(self, of: typing.List[TypeNode]) -> typing.Iterable[TypeNode]:
@@ -272,14 +331,17 @@
     def render(self, context: RenderContext):
         return 'keyof ' + _render_with_parenthesis(self.of, context)
 
     def __eq__(self, other):
         return isinstance(other, Tuple)\
             and self.of == other.of
 
+    def get_proxy_for_generic_params(self) -> 'TypeNode':
+        return self.of
+
 
 class Lookup(DictKeyType):
     def __init__(self, node: TypeNode, lookup: TypeNode):
         self.node = node
         self.lookup = lookup
 
     def render(self, context: RenderContext) -> str:
@@ -287,14 +349,17 @@
             + f'[{self.lookup.render(context)}]'
 
     def __eq__(self, other):
         return isinstance(other, Lookup)\
             and self.node == other.node\
             and self.lookup == other.lookup
 
+    def get_proxy_for_generic_params(self) -> 'TypeNode':
+        return self.node
+
 
 class UtilityNode(TypeNode):
     def __init__(self, name: str, parameters: typing.List[TypeNode]):
         self.name = name
         self.parameters = parameters
 
     def render(self, context: RenderContext):
@@ -306,56 +371,122 @@
         return isinstance(other, self.__class__)\
             and self.name == other.name\
             and self.parameters == other.parameters
 
 
 class Partial(UtilityNode):
     def __init__(self, type: TypeNode):
+        self.type = type
         super().__init__('Partial', [type])
 
+    def get_proxy_for_generic_params(self) -> 'TypeNode':
+        return self.type
+
 
 class Required(UtilityNode):
     def __init__(self, type: TypeNode):
+        self.type = type
         super().__init__('Required', [type])
 
+    def get_proxy_for_generic_params(self) -> 'TypeNode':
+        return self.type
+
 
 class Readonly(UtilityNode):
     def __init__(self, type: TypeNode):
+        self.type = type
         super().__init__('Readonly', [type])
 
+    def get_proxy_for_generic_params(self) -> 'TypeNode':
+        return self.type
+
 
 class Record(UtilityNode):
     def __init__(self, keys: TypeNode, type: TypeNode):
         super().__init__('Record', [keys, type])
 
 
 class Pick(UtilityNode):
     def __init__(self, type: TypeNode, keys: TypeNode):
+        self.type = type
         super().__init__('Pick', [type, keys])
 
+    def get_proxy_for_generic_params(self) -> 'TypeNode':
+        return self.type
+
 
 class Omit(UtilityNode):
     def __init__(self, type: TypeNode, keys: TypeNode):
+        self.type = type
         super().__init__('Omit', [type, keys])
 
+    def get_proxy_for_generic_params(self) -> 'TypeNode':
+        return self.type
+
 
 class Exclude(UtilityNode):
     def __init__(self, type: TypeNode, excluded_union: TypeNode):
+        self.type = type
         super().__init__('Exclude', [type, excluded_union])
 
+    def get_proxy_for_generic_params(self) -> 'TypeNode':
+        return self.type
+
 
 class Extract(UtilityNode):
     def __init__(self, type: TypeNode, union: TypeNode):
+        self.type = type
         super().__init__('Extract', [type, union])
 
+    def get_proxy_for_generic_params(self) -> 'TypeNode':
+        return self.type
+
 
 class NonNullable(UtilityNode):
     def __init__(self, type: TypeNode):
+        self.type = type
         super().__init__('NonNullable', [type])
 
+    def get_proxy_for_generic_params(self) -> 'TypeNode':
+        return self.type
+
+
+class Infer(TypeNode):
+    def __init__(self, typevar: typing.TypeVar):
+        self.typevar = typevar
+
+    def render(self, context: RenderContext) -> str:
+        return f'infer {self.typevar.__name__}'
+
+
+class Conditional(TypeNode):
+    def __init__(self,
+                 type: TypeNode,
+                 condition: TypeNode,
+                 true: TypeNode,
+                 false: TypeNode):
+        self.type = type
+        self.condition = condition
+        self.true = true
+        self.false = false
+
+    def render(self, context: RenderContext):
+        type = self.type.render(context)
+        condition = self.condition.render(context)
+        true = self.true.render(context)
+        false = self.false.render(context)
+        return f'{type} extends {condition} ? {true} : {false}'
+
+    def __eq__(self, other):
+        return isinstance(other, self.__class__)\
+            and self.type == other.type\
+            and self.condition == other.condition\
+            and self.true == other.true\
+            and self.false == other.false
+
 
 def _render_with_parenthesis(node: TypeNode, context: RenderContext) -> str:
     expr = node.render(context)
 
     if isinstance(node, (Union, Intersection)):
         if len(node.of) == 1:
             return expr
@@ -366,23 +497,26 @@
 
     return expr
 
 
 __all__ = [
     'Array',
     'Boolean',
+    'Conditional',
     'Dict',
     'DictKeyType',
     'Exclude',
     'Extract',
     'GlobalTypeNode',
+    'Infer',
     'Intersection',
     'Keyof',
     'Literal',
     'Lookup',
+    'Never',
     'NonNullable',
     'Null',
     'Number',
     'Object',
     'Omit',
     'Partial',
     'Pick',
```

### Comparing `ts_type-0.2.7/ts_type/utils.py` & `ts_type-0.2.8/ts_type/utils.py`

 * *Files identical despite different names*

### Comparing `ts_type-0.2.7/ts_type.egg-info/PKG-INFO` & `ts_type-0.2.8/ts_type.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ts-type
-Version: 0.2.7
+Version: 0.2.8
 Summary: ts_type generates typescript's type from python code
 Home-page: https://github.com/saryou/ts_type
 Author: Ryosuke Sasaki
 Author-email: saryou.ssk@gmail.com
 Project-URL: Bug Tracker, https://github.com/saryou/ts_type/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

