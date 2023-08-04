# Comparing `tmp/dask-expr-0.1.2.tar.gz` & `tmp/dask-expr-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dask-expr-0.1.2.tar", last modified: Fri Jul 28 08:41:23 2023, max compression
+gzip compressed data, was "dask-expr-0.1.3.tar", last modified: Fri Aug  4 12:41:03 2023, max compression
```

## Comparing `dask-expr-0.1.2.tar` & `dask-expr-0.1.3.tar`

### file list

```diff
@@ -1,35 +1,37 @@
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-28 08:41:23.732414 dask-expr-0.1.2/
--rw-r--r--   0 patrick    (501) staff       (20)     1516 2023-07-21 10:19:51.000000 dask-expr-0.1.2/LICENSE.txt
--rw-r--r--   0 patrick    (501) staff       (20)     4558 2023-07-28 08:41:23.732477 dask-expr-0.1.2/PKG-INFO
--rw-r--r--   0 patrick    (501) staff       (20)     3626 2023-07-26 09:32:50.000000 dask-expr-0.1.2/README.md
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-28 08:41:23.732787 dask-expr-0.1.2/dask_expr/
--rw-r--r--   0 patrick    (501) staff       (20)      127 2023-07-21 10:19:51.000000 dask-expr-0.1.2/dask_expr/__init__.py
--rw-r--r--   0 patrick    (501) staff       (20)     2603 2023-07-21 10:19:51.000000 dask-expr-0.1.2/dask_expr/_accessor.py
--rw-r--r--   0 patrick    (501) staff       (20)     1434 2023-07-21 10:19:51.000000 dask-expr-0.1.2/dask_expr/_align.py
--rw-r--r--   0 patrick    (501) staff       (20)     3683 2023-07-21 10:19:51.000000 dask-expr-0.1.2/dask_expr/_categorical.py
--rw-r--r--   0 patrick    (501) staff       (20)    38879 2023-07-28 08:40:24.000000 dask-expr-0.1.2/dask_expr/_collection.py
--rw-r--r--   0 patrick    (501) staff       (20)     6820 2023-07-26 09:32:50.000000 dask-expr-0.1.2/dask_expr/_concat.py
--rw-r--r--   0 patrick    (501) staff       (20)    70009 2023-07-28 08:40:24.000000 dask-expr-0.1.2/dask_expr/_expr.py
--rw-r--r--   0 patrick    (501) staff       (20)    15912 2023-07-21 10:19:51.000000 dask-expr-0.1.2/dask_expr/_groupby.py
--rw-r--r--   0 patrick    (501) staff       (20)     9161 2023-07-21 10:19:51.000000 dask-expr-0.1.2/dask_expr/_merge.py
--rw-r--r--   0 patrick    (501) staff       (20)     2169 2023-07-21 10:19:51.000000 dask-expr-0.1.2/dask_expr/_quantiles.py
--rw-r--r--   0 patrick    (501) staff       (20)    24731 2023-07-27 14:56:31.000000 dask-expr-0.1.2/dask_expr/_reductions.py
--rw-r--r--   0 patrick    (501) staff       (20)    11011 2023-07-27 14:56:31.000000 dask-expr-0.1.2/dask_expr/_repartition.py
--rw-r--r--   0 patrick    (501) staff       (20)    31301 2023-07-26 09:32:50.000000 dask-expr-0.1.2/dask_expr/_shuffle.py
--rw-r--r--   0 patrick    (501) staff       (20)      950 2023-07-26 09:32:50.000000 dask-expr-0.1.2/dask_expr/_util.py
--rw-r--r--   0 patrick    (501) staff       (20)      497 2023-07-28 08:41:23.732828 dask-expr-0.1.2/dask_expr/_version.py
--rw-r--r--   0 patrick    (501) staff       (20)     6228 2023-07-21 10:19:51.000000 dask-expr-0.1.2/dask_expr/datasets.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-28 08:41:23.732221 dask-expr-0.1.2/dask_expr/io/
--rw-r--r--   0 patrick    (501) staff       (20)       96 2023-05-12 07:18:29.000000 dask-expr-0.1.2/dask_expr/io/__init__.py
--rw-r--r--   0 patrick    (501) staff       (20)      980 2023-06-27 13:49:53.000000 dask-expr-0.1.2/dask_expr/io/csv.py
--rw-r--r--   0 patrick    (501) staff       (20)     3068 2023-07-21 10:19:51.000000 dask-expr-0.1.2/dask_expr/io/io.py
--rw-r--r--   0 patrick    (501) staff       (20)    33982 2023-07-26 09:32:50.000000 dask-expr-0.1.2/dask_expr/io/parquet.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-28 08:41:23.730871 dask-expr-0.1.2/dask_expr.egg-info/
--rw-r--r--   0 patrick    (501) staff       (20)     4558 2023-07-28 08:41:23.000000 dask-expr-0.1.2/dask_expr.egg-info/PKG-INFO
--rw-r--r--   0 patrick    (501) staff       (20)      665 2023-07-28 08:41:23.000000 dask-expr-0.1.2/dask_expr.egg-info/SOURCES.txt
--rw-r--r--   0 patrick    (501) staff       (20)        1 2023-07-28 08:41:23.000000 dask-expr-0.1.2/dask_expr.egg-info/dependency_links.txt
--rw-r--r--   0 patrick    (501) staff       (20)       32 2023-07-28 08:41:23.000000 dask-expr-0.1.2/dask_expr.egg-info/requires.txt
--rw-r--r--   0 patrick    (501) staff       (20)       10 2023-07-28 08:41:23.000000 dask-expr-0.1.2/dask_expr.egg-info/top_level.txt
--rw-r--r--   0 patrick    (501) staff       (20)     1615 2023-07-21 10:19:51.000000 dask-expr-0.1.2/pyproject.toml
--rw-r--r--   0 patrick    (501) staff       (20)      230 2023-07-28 08:41:23.732681 dask-expr-0.1.2/setup.cfg
--rwxr-xr-x   0 patrick    (501) staff       (20)      194 2023-07-21 10:19:51.000000 dask-expr-0.1.2/setup.py
+drwxr-xr-x   0 patrick    (502) staff       (20)        0 2023-08-04 12:41:03.364465 dask-expr-0.1.3/
+-rw-r--r--   0 patrick    (502) staff       (20)     1516 2023-08-02 08:54:32.000000 dask-expr-0.1.3/LICENSE.txt
+-rw-r--r--   0 patrick    (502) staff       (20)     4558 2023-08-04 12:41:03.364536 dask-expr-0.1.3/PKG-INFO
+-rw-r--r--   0 patrick    (502) staff       (20)     3626 2023-08-02 08:54:32.000000 dask-expr-0.1.3/README.md
+drwxr-xr-x   0 patrick    (502) staff       (20)        0 2023-08-04 12:41:03.364926 dask-expr-0.1.3/dask_expr/
+-rw-r--r--   0 patrick    (502) staff       (20)      127 2023-08-02 08:54:32.000000 dask-expr-0.1.3/dask_expr/__init__.py
+-rw-r--r--   0 patrick    (502) staff       (20)     2603 2023-08-02 08:54:32.000000 dask-expr-0.1.3/dask_expr/_accessor.py
+-rw-r--r--   0 patrick    (502) staff       (20)     1434 2023-08-02 08:54:32.000000 dask-expr-0.1.3/dask_expr/_align.py
+-rw-r--r--   0 patrick    (502) staff       (20)     3683 2023-08-02 08:54:32.000000 dask-expr-0.1.3/dask_expr/_categorical.py
+-rw-r--r--   0 patrick    (502) staff       (20)    39471 2023-08-04 12:35:03.000000 dask-expr-0.1.3/dask_expr/_collection.py
+-rw-r--r--   0 patrick    (502) staff       (20)     6820 2023-08-02 08:54:32.000000 dask-expr-0.1.3/dask_expr/_concat.py
+-rw-r--r--   0 patrick    (502) staff       (20)    70239 2023-08-04 12:35:03.000000 dask-expr-0.1.3/dask_expr/_expr.py
+-rw-r--r--   0 patrick    (502) staff       (20)    15912 2023-08-02 08:54:32.000000 dask-expr-0.1.3/dask_expr/_groupby.py
+-rw-r--r--   0 patrick    (502) staff       (20)     9161 2023-08-02 08:54:32.000000 dask-expr-0.1.3/dask_expr/_merge.py
+-rw-r--r--   0 patrick    (502) staff       (20)     2456 2023-08-04 12:28:50.000000 dask-expr-0.1.3/dask_expr/_quantiles.py
+-rw-r--r--   0 patrick    (502) staff       (20)    24909 2023-08-04 12:28:50.000000 dask-expr-0.1.3/dask_expr/_reductions.py
+-rw-r--r--   0 patrick    (502) staff       (20)    14364 2023-08-04 12:34:50.000000 dask-expr-0.1.3/dask_expr/_repartition.py
+-rw-r--r--   0 patrick    (502) staff       (20)    31990 2023-08-04 12:34:50.000000 dask-expr-0.1.3/dask_expr/_shuffle.py
+-rw-r--r--   0 patrick    (502) staff       (20)      217 2023-06-27 15:57:00.000000 dask-expr-0.1.3/dask_expr/_typing.py
+-rw-r--r--   0 patrick    (502) staff       (20)     2089 2023-08-04 12:35:17.000000 dask-expr-0.1.3/dask_expr/_util.py
+-rw-r--r--   0 patrick    (502) staff       (20)      497 2023-08-04 12:41:03.364961 dask-expr-0.1.3/dask_expr/_version.py
+-rw-r--r--   0 patrick    (502) staff       (20)     6506 2023-08-04 12:40:43.000000 dask-expr-0.1.3/dask_expr/datasets.py
+drwxr-xr-x   0 patrick    (502) staff       (20)        0 2023-08-04 12:41:03.364249 dask-expr-0.1.3/dask_expr/io/
+-rw-r--r--   0 patrick    (502) staff       (20)       96 2023-05-16 14:29:09.000000 dask-expr-0.1.3/dask_expr/io/__init__.py
+-rw-r--r--   0 patrick    (502) staff       (20)     1759 2023-08-04 12:35:03.000000 dask-expr-0.1.3/dask_expr/io/csv.py
+-rw-r--r--   0 patrick    (502) staff       (20)     7370 2023-08-04 12:35:03.000000 dask-expr-0.1.3/dask_expr/io/io.py
+-rw-r--r--   0 patrick    (502) staff       (20)    32050 2023-08-04 12:35:03.000000 dask-expr-0.1.3/dask_expr/io/parquet.py
+drwxr-xr-x   0 patrick    (502) staff       (20)        0 2023-08-04 12:41:03.363560 dask-expr-0.1.3/dask_expr.egg-info/
+-rw-r--r--   0 patrick    (502) staff       (20)     4558 2023-08-04 12:41:03.000000 dask-expr-0.1.3/dask_expr.egg-info/PKG-INFO
+-rw-r--r--   0 patrick    (502) staff       (20)      700 2023-08-04 12:41:03.000000 dask-expr-0.1.3/dask_expr.egg-info/SOURCES.txt
+-rw-r--r--   0 patrick    (502) staff       (20)        1 2023-08-04 12:41:03.000000 dask-expr-0.1.3/dask_expr.egg-info/dependency_links.txt
+-rw-r--r--   0 patrick    (502) staff       (20)       32 2023-08-04 12:41:03.000000 dask-expr-0.1.3/dask_expr.egg-info/requires.txt
+-rw-r--r--   0 patrick    (502) staff       (20)       10 2023-08-04 12:41:03.000000 dask-expr-0.1.3/dask_expr.egg-info/top_level.txt
+-rw-r--r--   0 patrick    (502) staff       (20)     1615 2023-08-02 08:54:32.000000 dask-expr-0.1.3/pyproject.toml
+-rw-r--r--   0 patrick    (502) staff       (20)      230 2023-08-04 12:41:03.364790 dask-expr-0.1.3/setup.cfg
+-rwxr-xr-x   0 patrick    (502) staff       (20)      194 2023-08-04 10:47:33.000000 dask-expr-0.1.3/setup.py
+-rw-r--r--   0 patrick    (502) staff       (20)    86677 2023-07-12 17:47:49.000000 dask-expr-0.1.3/versioneer.py
```

### Comparing `dask-expr-0.1.2/LICENSE.txt` & `dask-expr-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dask-expr-0.1.2/PKG-INFO` & `dask-expr-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dask-expr
-Version: 0.1.2
+Version: 0.1.3
 Summary: High Level Expressions for Dask 
 Maintainer-email: Matthew Rocklin <mrocklin@gmail.com>
 License: BSD
 Project-URL: Source code, https://github.com/dask-contrib/dask-expr/
 Keywords: dask pandas
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `dask-expr-0.1.2/README.md` & `dask-expr-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `dask-expr-0.1.2/dask_expr/_accessor.py` & `dask-expr-0.1.3/dask_expr/_accessor.py`

 * *Files identical despite different names*

### Comparing `dask-expr-0.1.2/dask_expr/_align.py` & `dask-expr-0.1.3/dask_expr/_align.py`

 * *Files identical despite different names*

### Comparing `dask-expr-0.1.2/dask_expr/_categorical.py` & `dask-expr-0.1.3/dask_expr/_categorical.py`

 * *Files identical despite different names*

### Comparing `dask-expr-0.1.2/dask_expr/_collection.py` & `dask-expr-0.1.3/dask_expr/_collection.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,22 +110,30 @@
     def expr(self) -> expr.Expr:
         return self._expr
 
     @property
     def _meta(self):
         return self.expr._meta
 
+    @functools.cached_property
+    def _meta_nonempty(self):
+        return meta_nonempty(self._meta)
+
     @property
     def size(self):
         return new_collection(self.expr.size)
 
     @property
     def columns(self):
         return self._meta.columns
 
+    @columns.setter
+    def columns(self, columns):
+        self._expr = self.rename(dict(zip(self.columns, columns)))._expr
+
     def __len__(self):
         return new_collection(Len(self.expr)).compute()
 
     @property
     def nbytes(self):
         raise NotImplementedError("nbytes is not implemented on DataFrame")
 
@@ -388,15 +396,17 @@
             transform_divisions,
             clear_divisions,
             kwargs,
             *[arg.expr if isinstance(arg, FrameBase) else arg for arg in args],
         )
         return new_collection(new_expr)
 
-    def repartition(self, npartitions=None, divisions=None, force=False):
+    def repartition(
+        self, npartitions=None, divisions=None, force=False, partition_size=None
+    ):
         """Repartition a collection
 
         Exactly one of `divisions` or `npartitions` should be specified.
         A ``ValueError`` will be raised when that is not the case.
 
         Parameters
         ----------
@@ -411,21 +421,32 @@
             See https://docs.dask.org/en/latest/dataframe-design.html#partitions.
         force : bool, default False
             Allows the expansion of the existing divisions.
             If False then the new divisions' lower and upper bounds must be
             the same as the old divisions'.
         """
 
-        if sum([divisions is not None, npartitions is not None]) != 1:
+        if (
+            sum(
+                [
+                    divisions is not None,
+                    npartitions is not None,
+                    partition_size is not None,
+                ]
+            )
+            != 1
+        ):
             raise ValueError(
                 "Please provide exactly one of the ``npartitions=`` or "
                 "``divisions=`` keyword arguments."
             )
 
-        return new_collection(Repartition(self.expr, npartitions, divisions, force))
+        return new_collection(
+            Repartition(self.expr, npartitions, divisions, force, partition_size)
+        )
 
     def to_dask_dataframe(self, optimize: bool = True, **optimize_kwargs) -> _Frame:
         """Convert to a dask-dataframe collection
 
         Parameters
         ----------
         optimize
@@ -829,14 +850,15 @@
         other,
         drop=True,
         sorted=False,
         npartitions: int | None = None,
         divisions=None,
         sort: bool = True,
         upsample: float = 1.0,
+        partition_size: float = 128e6,
     ):
         if isinstance(other, DataFrame):
             raise TypeError("other can't be of type DataFrame")
         if isinstance(other, Series):
             if other._name == self.index._name:
                 return self
         elif other == self.index.name:
@@ -863,14 +885,15 @@
             SetIndex(
                 self.expr,
                 other,
                 drop,
                 user_divisions=divisions,
                 npartitions=npartitions,
                 upsample=upsample,
+                partition_size=partition_size,
             )
         )
 
     def sort_values(
         self,
         by: str | list[str],
         npartitions: int | None = None,
@@ -1088,20 +1111,20 @@
     """
     graph = ddf.dask
     if optimize:
         graph = ddf.__dask_optimize__(graph, ddf.__dask_keys__())
     return from_graph(graph, ddf._meta, ddf.divisions, ddf._name)
 
 
-def read_csv(path, *args, **kwargs):
+def read_csv(path, *args, usecols=None, **kwargs):
     from dask_expr.io.csv import ReadCSV
 
     if not isinstance(path, str):
         path = stringify_path(path)
-    return new_collection(ReadCSV(path, *args, **kwargs))
+    return new_collection(ReadCSV(path, *args, columns=usecols, **kwargs))
 
 
 def read_parquet(
     path=None,
     columns=None,
     filters=None,
     categories=None,
```

### Comparing `dask-expr-0.1.2/dask_expr/_concat.py` & `dask-expr-0.1.3/dask_expr/_concat.py`

 * *Files identical despite different names*

### Comparing `dask-expr-0.1.2/dask_expr/_expr.py` & `dask-expr-0.1.3/dask_expr/_expr.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     make_meta,
 )
 from dask.dataframe.dispatch import meta_nonempty
 from dask.dataframe.utils import clear_known_categories, drop_by_shallow_copy
 from dask.utils import M, apply, funcname, import_required, is_arraylike
 from tlz import merge_sorted, unique
 
-from dask_expr._util import _tokenize_deterministic
+from dask_expr._util import _tokenize_deterministic, _tokenize_partial
 
 replacement_rules = []
 
 no_default = "__no_default__"
 
 
 class Expr:
@@ -40,14 +40,15 @@
 
     This mostly includes Dask protocols and various Pandas-like method
     definitions to make us look more like a DataFrame.
     """
 
     _parameters = []
     _defaults = {}
+    _is_length_preserving = False
 
     def __init__(self, *args, **kwargs):
         operands = list(args)
         for parameter in type(self)._parameters[len(operands) :]:
             try:
                 operands.append(kwargs.pop(parameter))
             except KeyError:
@@ -764,28 +765,17 @@
         alike = [
             op for op in root.find_operations(type(self)) if op._name != self._name
         ]
         if not alike:
             # No other operations of the same type. Early return
             return []
 
-        def _tokenize(rp):
-            # Helper function to "tokenize" the operands
-            # that are not in the `ignore` list
-            return _tokenize_deterministic(
-                *[
-                    op
-                    for i, op in enumerate(rp.operands)
-                    if i >= len(rp._parameters) or rp._parameters[i] not in ignore
-                ]
-            )
-
         # Return subset of `alike` with the same "token"
-        token = _tokenize(self)
-        return [item for item in alike if _tokenize(item) == token]
+        token = _tokenize_partial(self, ignore)
+        return [item for item in alike if _tokenize_partial(item, ignore) == token]
 
     def _node_label_args(self):
         """Operands to include in the node label by `visualize`"""
         return self.dependencies()
 
     def _to_graphviz(
         self,
@@ -1081,16 +1071,19 @@
                     )
                 ) or common._name == op._name:
                     push_up_op = True
                     break
 
             if push_up_op:
                 # Add operations back in the same order
-                for op in reversed(operations):
+                for i, op in enumerate(reversed(operations)):
                     common = common[op]
+                    if i > 0:
+                        # Combine stacked projections
+                        common = common._simplify_down() or common
                 return common
         return None
 
 
 class MapPartitions(Blockwise):
     _parameters = [
         "frame",
@@ -1252,14 +1245,15 @@
 
 
 class VarColumns(Blockwise):
     _parameters = ["frame", "skipna", "ddof", "numeric_only"]
     _defaults = {"skipna": True, "ddof": 1, "numeric_only": False}
     _keyword_only = ["skipna", "ddof", "numeric_only"]
     operation = M.var
+    _is_length_preserving = True
 
     @functools.cached_property
     def _kwargs(self) -> dict:
         return {"axis": 1, **super()._kwargs}
 
 
 class Sqrt(Blockwise):
@@ -1270,14 +1264,15 @@
 class Elemwise(Blockwise):
     """
     This doesn't really do anything, but we anticipate that future
     optimizations, like `len` will care about which operations preserve length
     """
 
     _filter_passthrough = True
+    _is_length_preserving = True
 
     def _simplify_up(self, parent):
         if self._filter_passthrough and isinstance(parent, Filter):
             return type(self)(
                 self.frame[parent.operand("predicate")], *self.operands[1:]
             )
         return super()._simplify_up(parent)
@@ -1611,14 +1606,17 @@
             return (None, None)
         return super()._divisions()
 
     def _simplify_down(self):
         if (
             str(self.frame.columns) == str(self.columns)
             and self._meta.ndim == self.frame._meta.ndim
+            and not (
+                isinstance(self.frame, BlockwiseIO) and self.frame._absorb_projections
+            )
         ):
             # TODO: we should get more precise around Expr.columns types
             return self.frame
         if isinstance(self.frame, Projection):
             # df[a][b]
             a = self.frame.operand("columns")
             b = self.operand("columns")
@@ -2126,15 +2124,20 @@
             yield e
 
 
 def are_co_aligned(*exprs):
     """Do inputs come from different parents, modulo blockwise?"""
     exprs = [expr for expr in exprs if not is_broadcastable(expr)]
     ancestors = [set(non_blockwise_ancestors(e)) for e in exprs]
-    return len(set(flatten(ancestors, container=set))) == 1
+    unique_ancestors = {
+        # Account for column projection within IO expressions
+        _tokenize_partial(item, ["columns", "_series"])
+        for item in flatten(ancestors, container=set)
+    }
+    return len(unique_ancestors) == 1
 
 
 ## Utilites for Expr fusion
 
 
 def optimize_blockwise_fusion(expr):
     """Traverse the expression graph and apply fusion"""
```

### Comparing `dask-expr-0.1.2/dask_expr/_groupby.py` & `dask-expr-0.1.3/dask_expr/_groupby.py`

 * *Files identical despite different names*

### Comparing `dask-expr-0.1.2/dask_expr/_merge.py` & `dask-expr-0.1.3/dask_expr/_merge.py`

 * *Files identical despite different names*

### Comparing `dask-expr-0.1.2/dask_expr/_quantiles.py` & `dask-expr-0.1.3/dask_expr/_quantiles.py`

 * *Files 17% similar despite different names*

```diff
@@ -55,14 +55,22 @@
             )
             for i, (state, key) in enumerate(zip(state_data, keys))
         }
 
         merge_dsk = create_merge_tree(
             merge_and_compress_summaries, sorted(percentiles_dsk), self._name, 2
         )
+        if not merge_dsk:
+            # Compress the data even if we only have one partition
+            merge_dsk = {
+                (self._name, 2, 0): (
+                    merge_and_compress_summaries,
+                    [list(percentiles_dsk)[0]],
+                )
+            }
 
         merged_key = max(merge_dsk)
         last_dsk = {
             (self._name, 0): (
                 pd.Series,
                 (
                     process_val_weights,
```

### Comparing `dask-expr-0.1.2/dask_expr/_reductions.py` & `dask-expr-0.1.3/dask_expr/_reductions.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,18 +9,19 @@
     idxmaxmin_agg,
     idxmaxmin_chunk,
     idxmaxmin_combine,
     is_dataframe_like,
     is_series_like,
     make_meta,
     meta_nonempty,
+    total_mem_usage,
 )
 from dask.utils import M, apply, funcname
 
-from dask_expr._expr import Blockwise, Elemwise, Expr, Index, Projection
+from dask_expr._expr import Blockwise, Expr, Index, Projection
 from dask_expr._util import is_scalar
 
 
 class ApplyConcatApply(Expr):
     """Perform reduction-like operation on dataframes
 
     This pattern is commonly used for reductions, groupby-aggregations, and
@@ -554,19 +555,19 @@
     reduction_chunk = staticmethod(len)
     reduction_aggregate = sum
 
     def _simplify_down(self):
         from dask_expr.io.io import IO
 
         # We introduce Index nodes sometimes.  We special case around them.
-        if isinstance(self.frame, Index) and isinstance(self.frame.frame, Elemwise):
+        if isinstance(self.frame, Index) and self.frame.frame._is_length_preserving:
             return Len(self.frame.frame)
 
         # Pass through Elemwises, unless we just introduced an Index
-        if isinstance(self.frame, Elemwise) and not isinstance(self.frame, Index):
+        if self.frame._is_length_preserving and not isinstance(self.frame, Index):
             child = max(self.frame.dependencies(), key=lambda expr: expr.npartitions)
             return Len(child)
 
         # Let the child handle it.  They often know best
         if isinstance(self.frame, IO):
             return self
 
@@ -864,7 +865,15 @@
         return {"is_dataframe": is_dataframe_like(self.frame._meta)}
 
     @staticmethod
     def reduction_combine(x, is_dataframe):
         if is_dataframe:
             return x.groupby(x.index).sum()
         return x.sum()
+
+
+class TotalMemoryUsageFrame(MemoryUsageFrame):
+    reduction_chunk = total_mem_usage
+
+    @staticmethod
+    def reduction_combine(x, is_dataframe):
+        return x
```

### Comparing `dask-expr-0.1.2/dask_expr/_repartition.py` & `dask-expr-0.1.3/dask_expr/_repartition.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,44 @@
 import functools
 from operator import getitem
 from pprint import pformat
 
 import numpy as np
 import pandas as pd
+from dask.base import tokenize
 from dask.dataframe import methods
 from dask.dataframe.core import split_evenly
 from dask.dataframe.utils import is_series_like
+from dask.utils import iter_chunks, parse_bytes
 from pandas.api.types import is_datetime64_any_dtype, is_numeric_dtype
 from tlz import unique
 
 from dask_expr._expr import Expr, Projection
+from dask_expr._reductions import TotalMemoryUsageFrame
+from dask_expr._util import LRU
 
 
 class Repartition(Expr):
     """Abstract repartitioning expression"""
 
-    _parameters = ["frame", "n", "new_divisions", "force"]
-    _defaults = {"n": None, "new_divisions": None, "force": False}
+    _parameters = ["frame", "n", "new_divisions", "force", "partition_size"]
+    _defaults = {
+        "n": None,
+        "new_divisions": None,
+        "force": False,
+        "partition_size": None,
+    }
+    _is_length_preserving = True
 
     @property
     def _meta(self):
         return self.frame._meta
 
     def _divisions(self):
-        if self.n is not None:
+        if self.n is not None or self.partition_size is not None:
             x = self.optimize(fuse=False)
             return x._divisions()
         return self.new_divisions
 
     def _lower(self):
         if type(self) != Repartition:
             # This lower logic should not be inherited
@@ -77,14 +87,16 @@
                     return RepartitionDivisions(df, divisions, self.force)
                 else:
                     return RepartitionToMore(self.frame, self.n)
         elif self.new_divisions:
             if tuple(self.new_divisions) == self.frame.divisions:
                 return self.frame
             return RepartitionDivisions(self.frame, self.new_divisions, self.force)
+        elif self.partition_size is not None:
+            return RepartitionSize(self.frame, partition_size=self.partition_size)
         else:
             raise NotImplementedError()
 
     def _simplify_up(self, parent):
         # Reorder with column projection
         if isinstance(parent, Projection):
             return type(self)(self.frame[parent.operand("columns")], *self.operands[1:])
@@ -105,22 +117,17 @@
         assert npartitions_input > self.n
 
         npartitions_ratio = npartitions_input / npartitions
         new_partitions_boundaries = [
             int(new_partition_index * npartitions_ratio)
             for new_partition_index in range(npartitions + 1)
         ]
-
-        if not isinstance(new_partitions_boundaries, list):
-            new_partitions_boundaries = list(new_partitions_boundaries)
-        if new_partitions_boundaries[0] > 0:
-            new_partitions_boundaries.insert(0, 0)
-        if new_partitions_boundaries[-1] < self.frame.npartitions:
-            new_partitions_boundaries.append(self.frame.npartitions)
-        return new_partitions_boundaries
+        return _clean_new_division_boundaries(
+            new_partitions_boundaries, self.frame.npartitions
+        )
 
     def _layer(self):
         new_partitions_boundaries = self._partitions_boundaries
         return {
             (self._name, i): (
                 methods.concat,
                 [(self.frame._name, j) for j in range(start, end)],
@@ -310,7 +317,103 @@
                         "check for duplicate partitions\nold:\n%s\n\n"
                         "new:\n%s\n\ncombined:\n%s"
                         % (pformat(a), pformat(b), pformat(c))
                     )
                 d[(out2, j - 1)] = (methods.concat, tmp)
             j += 1
         return d
+
+
+class RepartitionSize(Repartition):
+    @functools.cached_property
+    def _size(self):
+        size = self.operand("partition_size")
+        if isinstance(size, str):
+            size = parse_bytes(size)
+        return int(size)
+
+    @functools.cached_property
+    def _nsplits(self):
+        return 1 + _get_mem_usages(self.frame) // self._size
+
+    @functools.cached_property
+    def _partition_boundaries(self):
+        nsplits = self._nsplits
+        mem_usages = _get_mem_usages(self.frame)
+
+        if np.any(nsplits > 1):
+            split_mem_usages = []
+            for n, usage in zip(nsplits, mem_usages):
+                split_mem_usages.extend([usage / n] * n)
+            mem_usages = pd.Series(split_mem_usages)
+
+        assert np.all(mem_usages <= self._size)
+        new_npartitions = list(map(len, iter_chunks(mem_usages, self._size)))
+        new_partitions_boundaries = np.cumsum(new_npartitions)
+        return _clean_new_division_boundaries(
+            new_partitions_boundaries, self.frame.npartitions
+        )
+
+    def _divisions(self):
+        if np.any(self._nsplits > 1):
+            return (None,) * len(self._partition_boundaries)
+        return (self.frame.divisions[i] for i in self._partition_boundaries)
+
+    def _layer(self) -> dict:
+        df = self.frame
+        dsk = {}
+
+        if np.any(self._nsplits > 1):
+            split_name = f"split-{tokenize(df, self._nsplits)}"
+            new_name = f"repartition-split-{self._size}-{tokenize(df)}"
+            j = 0
+            for i, k in enumerate(self._nsplits):
+                if k == 1:
+                    dsk[new_name, j] = (df._name, i)
+                    j += 1
+                else:
+                    dsk[split_name, i] = (split_evenly, (df._name, i), k)
+                    for jj in range(k):
+                        dsk[new_name, j] = (getitem, (split_name, i), jj)
+                        j += 1
+        else:
+            new_name = self.frame._name
+
+        dsk.update(
+            {
+                (self._name, i): (
+                    methods.concat,
+                    [(new_name, j) for j in range(start, end)],
+                )
+                for i, (start, end) in enumerate(
+                    zip(self._partition_boundaries, self._partition_boundaries[1:])
+                )
+            }
+        )
+        return dsk
+
+
+def _clean_new_division_boundaries(new_partitions_boundaries, frame_npartitions):
+    if not isinstance(new_partitions_boundaries, list):
+        new_partitions_boundaries = list(new_partitions_boundaries)
+    if new_partitions_boundaries[0] > 0:
+        new_partitions_boundaries.insert(0, 0)
+    if new_partitions_boundaries[-1] < frame_npartitions:
+        new_partitions_boundaries.append(frame_npartitions)
+    return new_partitions_boundaries
+
+
+mem_usages_lru = LRU(10)
+
+
+def _get_mem_usages(frame):
+    if frame._name in mem_usages_lru:
+        return mem_usages_lru[frame._name]
+    result = _compute_mem_usages(frame)
+    mem_usages_lru[frame._name] = result
+    return result
+
+
+def _compute_mem_usages(frame):
+    from dask_expr._collection import new_collection
+
+    return new_collection(TotalMemoryUsageFrame(frame, deep=True)).compute()
```

### Comparing `dask-expr-0.1.2/dask_expr/_shuffle.py` & `dask-expr-0.1.3/dask_expr/_shuffle.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,14 +39,15 @@
     Prod,
     Size,
     Sum,
     Unique,
     ValueCounts,
 )
 from dask_expr._repartition import Repartition
+from dask_expr._util import LRU
 
 
 class Shuffle(Expr):
     """Abstract shuffle class
 
     Parameters
     ----------
@@ -74,14 +75,15 @@
         "options",
     ]
     _defaults = {
         "ignore_index": False,
         "backend": None,
         "options": None,
     }
+    _is_length_preserving = True
 
     def __str__(self):
         return f"Shuffle({self._name[-7:]})"
 
     def _node_label_args(self):
         return [self.frame, self.partitioning_index]
 
@@ -615,18 +617,20 @@
             index = partitioning_index(df[index], npartitions)
         else:
             index = partitioning_index(index, npartitions)
         return df.assign(**{name: index})
 
 
 class BaseSetIndexSortValues(Expr):
+    _is_length_preserving = True
+
     def _divisions(self):
         if self.user_divisions is not None:
             return self.user_divisions
-        divisions, mins, maxes, presorted = _calculate_divisions(
+        divisions, mins, maxes, presorted = _get_divisions(
             self.frame,
             self.other,
             self.npartitions,
             self.ascending,
             upsample=self.upsample,
         )
         if presorted:
@@ -678,15 +682,15 @@
         "npartitions": None,
         "upsample": 1.0,
     }
 
     def _divisions(self):
         if self.user_divisions is not None:
             return self.user_divisions
-        divisions, mins, maxes, presorted = _calculate_divisions(
+        divisions, mins, maxes, presorted = _get_divisions(
             self.frame,
             self.other,
             self.npartitions,
             self.ascending,
             upsample=self.upsample,
         )
         if presorted:
@@ -712,15 +716,15 @@
         if isinstance(self._other, Expr):
             return self._other
         return self.frame[self._other]
 
     def _lower(self):
         if self.user_divisions is None:
             divisions = self._divisions()
-            presorted = _calculate_divisions(
+            presorted = _get_divisions(
                 self.frame,
                 self.other,
                 self.npartitions,
                 self.ascending,
                 upsample=self.upsample,
             )[3]
 
@@ -789,15 +793,15 @@
 
     @property
     def _meta(self):
         return self.frame._meta
 
     def _lower(self):
         by = self.frame[self.by[0]]
-        divisions, _, _, presorted = _calculate_divisions(
+        divisions, _, _, presorted = _get_divisions(
             self.frame, by, self.npartitions, self.ascending, upsample=self.upsample
         )
         if presorted and self.npartitions == self.frame.npartitions:
             return SortValuesBlockwise(
                 self.frame, self.sort_function, self.sort_function_kwargs
             )
 
@@ -877,49 +881,54 @@
         return SortIndexBlockwise(index_set)
 
 
 class _SetPartitionsPreSetIndex(Blockwise):
     _parameters = ["frame", "new_divisions", "ascending", "na_position"]
     _defaults = {"ascending": True, "na_position": "last"}
     operation = staticmethod(set_partitions_pre)
+    _is_length_preserving = True
 
     @property
     def _meta(self):
         return self.frame._meta._constructor([0])
 
 
 class _SetIndexPost(Blockwise):
     _parameters = ["frame", "index_name", "drop", "set_name"]
+    _is_length_preserving = True
 
     def operation(self, df, index_name, drop, set_name):
         return df.set_index(set_name, drop=drop).rename_axis(index=index_name)
 
 
 class SortIndexBlockwise(Blockwise):
     _projection_passthrough = True
     _parameters = ["frame"]
     operation = M.sort_index
+    _is_length_preserving = True
 
 
 def sort_function(self, *args, **kwargs):
     sort_func = kwargs.pop("sort_function")
     sort_kwargs = kwargs.pop("sort_kwargs")
     return sort_func(*args, **kwargs, **sort_kwargs)
 
 
 class SortValuesBlockwise(Blockwise):
     _projection_passthrough = False
     _parameters = ["frame", "sort_function", "sort_kwargs"]
     operation = sort_function
     _keyword_only = ["sort_function", "sort_kwargs"]
+    _is_length_preserving = True
 
 
 class SetIndexBlockwise(Blockwise):
     _parameters = ["frame", "other", "drop", "new_divisions"]
     _keyword_only = ["drop", "new_divisions"]
+    _is_length_preserving = True
 
     def operation(self, df, *args, new_divisions, **kwargs):
         return df.set_index(*args, **kwargs)
 
     def _divisions(self):
         if self.new_divisions is None:
             return (None,) * (self.frame.npartitions + 1)
@@ -934,15 +943,35 @@
                 return
             return type(parent)(
                 type(self)(self.frame[columns], *self.operands[1:]),
                 parent.operand("columns"),
             )
 
 
-@functools.lru_cache  # noqa: B019
+divisions_lru = LRU(10)
+
+
+def _get_divisions(
+    frame,
+    other,
+    npartitions: int,
+    ascending: bool = True,
+    partition_size: float = 128e6,
+    upsample: float = 1.0,
+):
+    key = (other._name, npartitions, ascending, partition_size, upsample)
+    if key in divisions_lru:
+        return divisions_lru[key]
+    result = _calculate_divisions(
+        frame, other, npartitions, ascending, partition_size, upsample
+    )
+    divisions_lru[key] = result
+    return result
+
+
 def _calculate_divisions(
     frame,
     other,
     npartitions: int,
     ascending: bool = True,
     partition_size: float = 128e6,
     upsample: float = 1.0,
```

### Comparing `dask-expr-0.1.2/dask_expr/datasets.py` & `dask-expr-0.1.3/dask_expr/datasets.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         "freq": "1s",
         "partition_freq": "1d",
         "seed": None,
         "kwargs": {},
         "_partitions": None,
     }
 
-    @property
+    @functools.cached_property
     def _meta(self):
         dtypes = self.operand("dtypes")
         states = [0] * len(dtypes)
         return make_timeseries_part(
             "2000", "2000", dtypes, list(dtypes.keys()), "1H", states, self.kwargs
         ).iloc[:0]
 
@@ -55,14 +55,17 @@
             )
             for k in self.operand("dtypes")
         }
 
     def _filtered_task(self, index):
         full_divisions = self._divisions()
         column_states = [self.random_state[k][index] for k in self.operand("dtypes")]
+        if self.seed is not None and len(column_states) > 0:
+            # These will be the same anyway, so avoid serializing all of them
+            column_states = [column_states[0]]
         return (
             make_timeseries_part,
             full_divisions[index],
             full_divisions[index + 1],
             self.operand("dtypes"),
             self.columns,
             self.freq,
@@ -141,14 +144,16 @@
     object: make_string,
     "string": make_string,
     "category": make_categorical,
 }
 
 
 def make_timeseries_part(start, end, dtypes, columns, freq, state_data, kwargs):
+    if len(state_data) == 1:
+        state_data = state_data * len(dtypes)
     index = pd.date_range(start=start, end=end, freq=freq, name="timestamp")
     data = {}
     for i, (k, dt) in enumerate(dtypes.items()):
         state = np.random.RandomState(state_data[i])
         kws = {
             kk.rsplit("_", 1)[1]: v
             for kk, v in kwargs.items()
```

### Comparing `dask-expr-0.1.2/dask_expr/io/parquet.py` & `dask-expr-0.1.3/dask_expr/io/parquet.py`

 * *Files 3% similar despite different names*

```diff
@@ -412,14 +412,15 @@
         "filesystem": "fsspec",
         "engine": "pyarrow",
         "kwargs": None,
         "_partitions": None,
         "_series": False,
     }
     _pq_length_stats = None
+    _absorb_projections = True
 
     @property
     def engine(self):
         _engine = self.operand("engine")
         if isinstance(_engine, str):
             return get_engine(_engine)
         return _engine
@@ -428,65 +429,21 @@
     def columns(self):
         columns_operand = self.operand("columns")
         if columns_operand is None:
             return list(self._meta.columns)
         else:
             return _convert_to_list(columns_operand)
 
-    def _combine_similar(self, root: Expr):
-        # For ReadParquet, we can avoid redundant file-system
-        # access by aggregating multiple operations with different
-        # column projections into the same operation.
-        alike = self._find_similar_operations(root, ignore=["columns", "_series"])
-        if alike:
-            # We have other ReadParquet operations in the expression
-            # graph that can be combined with this one.
-
-            # Find the column-projection union needed to combine
-            # the qualified ReadParquet operations
-            columns = set()
-            rps = [self] + alike
-            for rp in rps:
-                if rp.operand("columns"):
-                    columns |= set(rp.operand("columns"))
-            columns = sorted(columns)
-
-            # Can bail if we are not changing columns or the "_series" operand
-            columns_operand = self.operand("columns")
-            if columns_operand == columns and (len(columns) > 1 or not self._series):
-                return
-
-            # Check if we have the operation we want elsewhere in the graph
-            for rp in rps:
-                if rp.operand("columns") == columns and not rp.operand("_series"):
-                    return (
-                        rp[columns_operand[0]] if self._series else rp[columns_operand]
-                    )
-
-            # Create the "combined" ReadParquet operation
-            subs = {"columns": columns}
-            if self._series:
-                subs["_series"] = False
-            new = self.substitute_parameters(subs)
-            return new[columns_operand[0]] if self._series else new[columns_operand]
-
-        return
-
     def _simplify_up(self, parent):
         if isinstance(parent, Index):
             # Column projection
             return self.substitute_parameters({"columns": [], "_series": False})
 
         if isinstance(parent, Projection):
-            # Column projection
-            parent_columns = parent.operand("columns")
-            substitutions = {"columns": _convert_to_list(parent_columns)}
-            if isinstance(parent_columns, (str, int)):
-                substitutions["_series"] = True
-            return self.substitute_parameters(substitutions)
+            return super()._simplify_up(parent)
 
         if isinstance(parent, Filter) and isinstance(
             parent.predicate, (LE, GE, LT, GT, EQ, NE, And, Or)
         ):
             # Predicate pushdown
             filters = _DNF.extract_pq_filters(self, parent.predicate)
             if filters:
```

### Comparing `dask-expr-0.1.2/dask_expr.egg-info/PKG-INFO` & `dask-expr-0.1.3/dask_expr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dask-expr
-Version: 0.1.2
+Version: 0.1.3
 Summary: High Level Expressions for Dask 
 Maintainer-email: Matthew Rocklin <mrocklin@gmail.com>
 License: BSD
 Project-URL: Source code, https://github.com/dask-contrib/dask-expr/
 Keywords: dask pandas
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `dask-expr-0.1.2/dask_expr.egg-info/SOURCES.txt` & `dask-expr-0.1.3/dask_expr.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 LICENSE.txt
 README.md
 pyproject.toml
 setup.cfg
 setup.py
+versioneer.py
 dask_expr/__init__.py
 dask_expr/_accessor.py
 dask_expr/_align.py
 dask_expr/_categorical.py
 dask_expr/_collection.py
 dask_expr/_concat.py
 dask_expr/_expr.py
 dask_expr/_groupby.py
 dask_expr/_merge.py
 dask_expr/_quantiles.py
 dask_expr/_reductions.py
 dask_expr/_repartition.py
 dask_expr/_shuffle.py
+dask_expr/_typing.py
 dask_expr/_util.py
 dask_expr/_version.py
 dask_expr/datasets.py
 dask_expr.egg-info/PKG-INFO
 dask_expr.egg-info/SOURCES.txt
 dask_expr.egg-info/dependency_links.txt
 dask_expr.egg-info/requires.txt
```

### Comparing `dask-expr-0.1.2/pyproject.toml` & `dask-expr-0.1.3/pyproject.toml`

 * *Files identical despite different names*

