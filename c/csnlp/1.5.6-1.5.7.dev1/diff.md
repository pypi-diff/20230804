# Comparing `tmp/csnlp-1.5.6.tar.gz` & `tmp/csnlp-1.5.7.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csnlp-1.5.6.tar", last modified: Tue Jun 20 15:28:23 2023, max compression
+gzip compressed data, was "csnlp-1.5.7.dev1.tar", last modified: Fri Aug  4 17:08:37 2023, max compression
```

## Comparing `csnlp-1.5.6.tar` & `csnlp-1.5.7.dev1.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 15:28:23.141423 csnlp-1.5.6/
--rw-rw-rw-   0        0        0     1093 2022-11-02 20:11:46.000000 csnlp-1.5.6/LICENSE
--rw-rw-rw-   0        0        0     7065 2023-06-20 15:28:23.139434 csnlp-1.5.6/PKG-INFO
--rw-rw-rw-   0        0        0     6263 2023-06-20 12:25:01.000000 csnlp-1.5.6/README.md
--rw-rw-rw-   0        0        0     1155 2023-06-20 12:25:08.000000 csnlp-1.5.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-20 15:28:23.142065 csnlp-1.5.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-20 15:28:23.006753 csnlp-1.5.6/src/
-drwxrwxrwx   0        0        0        0 2023-06-20 15:28:23.029001 csnlp-1.5.6/src/csnlp/
--rw-rw-rw-   0        0        0      210 2023-04-04 11:47:09.000000 csnlp-1.5.6/src/csnlp/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-20 15:28:23.069034 csnlp-1.5.6/src/csnlp/core/
--rw-rw-rw-   0        0        0     3267 2023-01-02 20:43:22.000000 csnlp-1.5.6/src/csnlp/core/cache.py
--rw-rw-rw-   0        0        0     3186 2023-04-04 11:47:09.000000 csnlp-1.5.6/src/csnlp/core/data.py
--rw-rw-rw-   0        0        0     6057 2023-03-24 10:24:25.000000 csnlp-1.5.6/src/csnlp/core/debug.py
--rw-rw-rw-   0        0        0     2085 2023-02-16 10:35:36.000000 csnlp-1.5.6/src/csnlp/core/derivatives.py
--rw-rw-rw-   0        0        0     5241 2023-02-16 10:40:42.000000 csnlp-1.5.6/src/csnlp/core/scaling.py
--rw-rw-rw-   0        0        0     6426 2023-03-23 22:24:06.000000 csnlp-1.5.6/src/csnlp/core/solutions.py
-drwxrwxrwx   0        0        0        0 2023-06-20 15:28:23.077428 csnlp-1.5.6/src/csnlp/multistart/
--rw-rw-rw-   0        0        0      425 2023-03-20 12:01:22.000000 csnlp-1.5.6/src/csnlp/multistart/__init__.py
--rw-rw-rw-   0        0        0    15829 2023-06-20 15:25:08.000000 csnlp-1.5.6/src/csnlp/multistart/multistart_nlp.py
--rw-rw-rw-   0        0        0     3800 2023-06-20 15:25:49.000000 csnlp-1.5.6/src/csnlp/multistart/startpoints.py
-drwxrwxrwx   0        0        0        0 2023-06-20 15:28:23.091469 csnlp-1.5.6/src/csnlp/nlps/
--rw-rw-rw-   0        0        0    12297 2023-06-20 12:25:40.000000 csnlp-1.5.6/src/csnlp/nlps/constraints.py
--rw-rw-rw-   0        0        0     9068 2023-04-05 14:05:07.000000 csnlp-1.5.6/src/csnlp/nlps/nlp.py
--rw-rw-rw-   0        0        0     9584 2023-06-20 15:25:08.000000 csnlp-1.5.6/src/csnlp/nlps/objective.py
--rw-rw-rw-   0        0        0     2039 2023-03-25 14:04:48.000000 csnlp-1.5.6/src/csnlp/nlps/parameters.py
--rw-rw-rw-   0        0        0     2030 2023-03-25 14:01:54.000000 csnlp-1.5.6/src/csnlp/nlps/variables.py
-drwxrwxrwx   0        0        0        0 2023-06-20 15:28:23.103237 csnlp-1.5.6/src/csnlp/util/
--rw-rw-rw-   0        0        0     5231 2023-03-26 20:40:12.000000 csnlp-1.5.6/src/csnlp/util/docs.py
--rw-rw-rw-   0        0        0    11398 2023-03-25 13:36:29.000000 csnlp-1.5.6/src/csnlp/util/io.py
--rw-rw-rw-   0        0        0     5187 2023-04-05 14:05:07.000000 csnlp-1.5.6/src/csnlp/util/math.py
--rw-rw-rw-   0        0        0     3455 2023-03-24 17:58:30.000000 csnlp-1.5.6/src/csnlp/util/plot.py
-drwxrwxrwx   0        0        0        0 2023-06-20 15:28:23.117443 csnlp-1.5.6/src/csnlp/wrappers/
--rw-rw-rw-   0        0        0      294 2023-03-29 19:05:51.000000 csnlp-1.5.6/src/csnlp/wrappers/__init__.py
--rw-rw-rw-   0        0        0    16506 2023-03-25 14:29:46.000000 csnlp-1.5.6/src/csnlp/wrappers/mpc.py
--rw-rw-rw-   0        0        0     7474 2023-02-16 10:51:07.000000 csnlp-1.5.6/src/csnlp/wrappers/scaling.py
--rw-rw-rw-   0        0        0    16282 2023-04-04 11:47:09.000000 csnlp-1.5.6/src/csnlp/wrappers/sensitivity.py
--rw-rw-rw-   0        0        0     3644 2023-01-07 17:14:55.000000 csnlp-1.5.6/src/csnlp/wrappers/wrapper.py
-drwxrwxrwx   0        0        0        0 2023-06-20 15:28:23.044057 csnlp-1.5.6/src/csnlp.egg-info/
--rw-rw-rw-   0        0        0     7065 2023-06-20 15:28:22.000000 csnlp-1.5.6/src/csnlp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1015 2023-06-20 15:28:22.000000 csnlp-1.5.6/src/csnlp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 15:28:22.000000 csnlp-1.5.6/src/csnlp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       87 2023-06-20 15:28:22.000000 csnlp-1.5.6/src/csnlp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-20 15:28:22.000000 csnlp-1.5.6/src/csnlp.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-20 15:28:23.137180 csnlp-1.5.6/tests/
--rw-rw-rw-   0        0        0    13201 2023-03-29 19:49:44.000000 csnlp-1.5.6/tests/test_core.py
--rw-rw-rw-   0        0        0    10143 2023-06-20 15:25:49.000000 csnlp-1.5.6/tests/test_examples.py
--rw-rw-rw-   0        0        0     7610 2023-03-22 17:16:32.000000 csnlp-1.5.6/tests/test_multistart.py
--rw-rw-rw-   0        0        0    25071 2023-04-05 14:05:07.000000 csnlp-1.5.6/tests/test_nlps.py
--rw-rw-rw-   0        0        0    27440 2023-06-20 15:25:49.000000 csnlp-1.5.6/tests/test_quadrotor_mpc.py
--rw-rw-rw-   0        0        0     8151 2023-06-20 15:25:49.000000 csnlp-1.5.6/tests/test_util.py
--rw-rw-rw-   0        0        0    28699 2023-04-05 14:05:07.000000 csnlp-1.5.6/tests/test_wrappers.py
+drwxrwxrwx   0        0        0        0 2023-08-04 17:08:37.360389 csnlp-1.5.7.dev1/
+-rw-rw-rw-   0        0        0     1093 2022-11-02 20:11:46.000000 csnlp-1.5.7.dev1/LICENSE
+-rw-rw-rw-   0        0        0     7070 2023-08-04 17:08:37.359392 csnlp-1.5.7.dev1/PKG-INFO
+-rw-rw-rw-   0        0        0     6263 2023-06-20 12:25:01.000000 csnlp-1.5.7.dev1/README.md
+-rw-rw-rw-   0        0        0     1160 2023-08-04 17:07:57.000000 csnlp-1.5.7.dev1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-04 17:08:37.360389 csnlp-1.5.7.dev1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-04 17:08:37.228394 csnlp-1.5.7.dev1/src/
+drwxrwxrwx   0        0        0        0 2023-08-04 17:08:37.264389 csnlp-1.5.7.dev1/src/csnlp/
+-rw-rw-rw-   0        0        0      210 2023-04-04 11:47:09.000000 csnlp-1.5.7.dev1/src/csnlp/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-04 17:08:37.294389 csnlp-1.5.7.dev1/src/csnlp/core/
+-rw-rw-rw-   0        0        0     4311 2023-08-03 16:20:02.000000 csnlp-1.5.7.dev1/src/csnlp/core/cache.py
+-rw-rw-rw-   0        0        0     3196 2023-08-03 12:23:24.000000 csnlp-1.5.7.dev1/src/csnlp/core/data.py
+-rw-rw-rw-   0        0        0     5995 2023-08-03 12:22:22.000000 csnlp-1.5.7.dev1/src/csnlp/core/debug.py
+-rw-rw-rw-   0        0        0     2085 2023-02-16 10:35:36.000000 csnlp-1.5.7.dev1/src/csnlp/core/derivatives.py
+-rw-rw-rw-   0        0        0     5241 2023-02-16 10:40:42.000000 csnlp-1.5.7.dev1/src/csnlp/core/scaling.py
+-rw-rw-rw-   0        0        0     6494 2023-08-03 16:20:23.000000 csnlp-1.5.7.dev1/src/csnlp/core/solutions.py
+drwxrwxrwx   0        0        0        0 2023-08-04 17:08:37.299396 csnlp-1.5.7.dev1/src/csnlp/multistart/
+-rw-rw-rw-   0        0        0      425 2023-03-20 12:01:22.000000 csnlp-1.5.7.dev1/src/csnlp/multistart/__init__.py
+-rw-rw-rw-   0        0        0    15854 2023-08-04 17:07:57.000000 csnlp-1.5.7.dev1/src/csnlp/multistart/multistart_nlp.py
+-rw-rw-rw-   0        0        0     3649 2023-08-03 12:22:22.000000 csnlp-1.5.7.dev1/src/csnlp/multistart/startpoints.py
+drwxrwxrwx   0        0        0        0 2023-08-04 17:08:37.309391 csnlp-1.5.7.dev1/src/csnlp/nlps/
+-rw-rw-rw-   0        0        0    18203 2023-08-03 12:23:32.000000 csnlp-1.5.7.dev1/src/csnlp/nlps/constraints.py
+-rw-rw-rw-   0        0        0     9034 2023-08-03 12:22:22.000000 csnlp-1.5.7.dev1/src/csnlp/nlps/nlp.py
+-rw-rw-rw-   0        0        0    10220 2023-08-04 17:07:57.000000 csnlp-1.5.7.dev1/src/csnlp/nlps/objective.py
+-rw-rw-rw-   0        0        0     1991 2023-08-03 12:22:22.000000 csnlp-1.5.7.dev1/src/csnlp/nlps/parameters.py
+-rw-rw-rw-   0        0        0     1995 2023-08-03 12:22:22.000000 csnlp-1.5.7.dev1/src/csnlp/nlps/variables.py
+drwxrwxrwx   0        0        0        0 2023-08-04 17:08:37.319389 csnlp-1.5.7.dev1/src/csnlp/util/
+-rw-rw-rw-   0        0        0     5231 2023-03-26 20:40:12.000000 csnlp-1.5.7.dev1/src/csnlp/util/docs.py
+-rw-rw-rw-   0        0        0    10017 2023-08-03 12:22:29.000000 csnlp-1.5.7.dev1/src/csnlp/util/io.py
+-rw-rw-rw-   0        0        0     5187 2023-04-05 14:05:07.000000 csnlp-1.5.7.dev1/src/csnlp/util/math.py
+-rw-rw-rw-   0        0        0     3455 2023-03-24 17:58:30.000000 csnlp-1.5.7.dev1/src/csnlp/util/plot.py
+drwxrwxrwx   0        0        0        0 2023-08-04 17:08:37.343389 csnlp-1.5.7.dev1/src/csnlp/wrappers/
+-rw-rw-rw-   0        0        0      294 2023-03-29 19:05:51.000000 csnlp-1.5.7.dev1/src/csnlp/wrappers/__init__.py
+-rw-rw-rw-   0        0        0    16198 2023-08-04 17:07:57.000000 csnlp-1.5.7.dev1/src/csnlp/wrappers/mpc.py
+-rw-rw-rw-   0        0        0     7395 2023-08-03 12:22:22.000000 csnlp-1.5.7.dev1/src/csnlp/wrappers/scaling.py
+-rw-rw-rw-   0        0        0    16236 2023-08-03 12:22:26.000000 csnlp-1.5.7.dev1/src/csnlp/wrappers/sensitivity.py
+-rw-rw-rw-   0        0        0     3616 2023-08-03 12:22:22.000000 csnlp-1.5.7.dev1/src/csnlp/wrappers/wrapper.py
+drwxrwxrwx   0        0        0        0 2023-08-04 17:08:37.275389 csnlp-1.5.7.dev1/src/csnlp.egg-info/
+-rw-rw-rw-   0        0        0     7070 2023-08-04 17:08:37.000000 csnlp-1.5.7.dev1/src/csnlp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1015 2023-08-04 17:08:37.000000 csnlp-1.5.7.dev1/src/csnlp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-04 17:08:37.000000 csnlp-1.5.7.dev1/src/csnlp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       87 2023-08-04 17:08:37.000000 csnlp-1.5.7.dev1/src/csnlp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-08-04 17:08:37.000000 csnlp-1.5.7.dev1/src/csnlp.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-04 17:08:37.357389 csnlp-1.5.7.dev1/tests/
+-rw-rw-rw-   0        0        0    13935 2023-08-03 16:20:23.000000 csnlp-1.5.7.dev1/tests/test_core.py
+-rw-rw-rw-   0        0        0    10147 2023-08-03 16:20:23.000000 csnlp-1.5.7.dev1/tests/test_examples.py
+-rw-rw-rw-   0        0        0     7610 2023-03-22 17:16:32.000000 csnlp-1.5.7.dev1/tests/test_multistart.py
+-rw-rw-rw-   0        0        0    30843 2023-08-03 12:23:28.000000 csnlp-1.5.7.dev1/tests/test_nlps.py
+-rw-rw-rw-   0        0        0    27440 2023-06-28 09:25:26.000000 csnlp-1.5.7.dev1/tests/test_quadrotor_mpc.py
+-rw-rw-rw-   0        0        0     6959 2023-08-03 12:22:22.000000 csnlp-1.5.7.dev1/tests/test_util.py
+-rw-rw-rw-   0        0        0    28699 2023-07-29 07:14:15.000000 csnlp-1.5.7.dev1/tests/test_wrappers.py
```

### Comparing `csnlp-1.5.6/LICENSE` & `csnlp-1.5.7.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `csnlp-1.5.6/PKG-INFO` & `csnlp-1.5.7.dev1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csnlp
-Version: 1.5.6
+Version: 1.5.7.dev1
 Summary: Nonlinear Progamming with CasADi
 Author-email: Filippo Airaldi <filippoairaldi@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/FilippoAiraldi/casadi-nlp
 Project-URL: Bug Tracker, https://github.com/FilippoAiraldi/casadi-nlp/issues
 Keywords: nonlinear-optimization,casadi,sensitivity-analysis
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `csnlp-1.5.6/README.md` & `csnlp-1.5.7.dev1/README.md`

 * *Files identical despite different names*

### Comparing `csnlp-1.5.6/pyproject.toml` & `csnlp-1.5.7.dev1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "csnlp"
-version = "1.5.6"
+version = "1.5.7.dev1"
 authors = [
   { name="Filippo Airaldi", email="filippoairaldi@gmail.com" },
 ]
 description = "Nonlinear Progamming with CasADi"
 readme = "README.md"
 requires-python = ">=3.8"
 license = { text = "MIT" }
```

### Comparing `csnlp-1.5.6/src/csnlp/core/cache.py` & `csnlp-1.5.7.dev1/src/csnlp/core/cache.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,20 @@
 from functools import _lru_cache_wrapper, cached_property, wraps
-from typing import Callable, List
+from inspect import getmembers
+from typing import Any, Callable, List
+
+
+def _is_cached_property(c: Callable) -> bool:
+    """Returns True if the callable is a cached property."""
+    return isinstance(c, cached_property)
+
+
+def _is_lru_cache(c: Callable) -> bool:
+    """Returns True if the callable is a lru cache."""
+    return hasattr(c, "cache_info") or hasattr(c, "cache_clear")
 
 
 def invalidate_cache(*callables: Callable) -> Callable:
     """Decorator that allows to enhance a function or method with the ability, when
     called, to invalidate and clear the cached of some other target methods/properties.
     This is especially useful to reset the cache of a given cached method/property when
     another method makes changes to the underlying data, thus compromising the cached
@@ -32,17 +43,17 @@
         `functools._lru_cache_wrapper`.
     """
     if not callables:
         raise ValueError("No callables were passed for cache invalidation.")
     cached_properties: List[cached_property] = []
     lru_caches: List[_lru_cache_wrapper] = []
     for p in callables:
-        if isinstance(p, cached_property):
+        if _is_cached_property(p):
             cached_properties.append(p)
-        elif hasattr(p, "cache_clear"):
+        elif _is_lru_cache(p):
             lru_caches.append(p)  # type: ignore[arg-type]
         else:
             raise TypeError(
                 "Expected cached properties or lru wrappers; got "
                 f"{p.__class__.__name__} instead."
             )
 
@@ -88,7 +99,28 @@
             if invalidate_lru_caches is not None:
                 invalidate_lru_caches()
             return func(*args, **kwargs)
 
         return wrapper
 
     return decorating_function
+
+
+def invalidate_caches_of(obj: Any) -> None:
+    """
+    Similar to the decorator `invalidate_cache`, but clears the case of the given
+    object only once.
+
+    Parameters
+    ----------
+    obj : object
+        The object whose caches are to be cleared.
+    """
+    # basically do again what csnlp.core.cache.invalidate_cache does
+    for membername, member in getmembers(
+        type(obj), predicate=lambda m: _is_cached_property(m) or _is_lru_cache(m)
+    ):
+        if _is_cached_property(member):
+            if membername in obj.__dict__:
+                del obj.__dict__[membername]
+        elif _is_lru_cache(member):
+            getattr(obj, membername).cache_clear()
```

### Comparing `csnlp-1.5.6/src/csnlp/core/data.py` & `csnlp-1.5.7.dev1/src/csnlp/core/data.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from itertools import product
 from typing import Union
 
 import casadi as cs
 import numpy as np
+import numpy.typing as npt
 
 
 def array2cs(x: np.ndarray) -> Union[cs.SX, cs.MX]:
     """Converts numpy array `x` of scalar symbolic variable to a single symbolic
     instance. Opposite to `array2cs`. Note that all entries in `x` must have the same
     type, either SX or MX.
 
@@ -46,29 +47,29 @@
         raise ValueError("Can only convert 1D and 2D arrays to CasADi SX or MX.")
     m: Union[cs.SX, cs.MX] = cls(*shape)
     for idx in indices:
         m[idx] = x[idx]
     return m
 
 
-def cs2array(x: Union[cs.MX, cs.SX]) -> np.ndarray:
+def cs2array(x: Union[cs.MX, cs.SX]) -> npt.NDArray[np.object_]:
     """Converts casadi symbolic variable `x` to a numpy array of scalars. Opposite to
     `array2cs`.
 
     Inspired by
     https://bitbucket.org/rawlings-group/mpc-tools-casadi/src/master/mpctools/tools.py
 
     Parameters
     ----------
     x : casadi.SX or MX
         A symbolic variable (with multiple entries).
 
     Returns
     -------
-    np.ndarray
+    np array of cs.SX or MX
         The array containing the symbolic variable scalars.
     """
     if isinstance(x, np.ndarray):
         return x
     if isinstance(x, cs.DM):
         return x.full()
 
@@ -76,15 +77,17 @@
     y = np.empty(shape, object)
     indices = product(range(shape[0]), range(shape[1]))
     for idx in indices:
         y[idx] = x[idx]
     return y
 
 
-def find_index_in_vector(V: Union[cs.SX, cs.MX], a: Union[cs.SX, cs.MX]):
+def find_index_in_vector(
+    V: Union[cs.SX, cs.MX], a: Union[cs.SX, cs.MX]
+) -> npt.NDArray[np.int_]:
     """Finds the indices of `a` in `V`.
 
     Parameters
     ----------
     V : casadi.SX or MX
         The vector in which to search.
     a : casadi.SX or MX
@@ -96,18 +99,15 @@
         The indices of `a` in `V`.
 
     Raises
     ------
     ValueError
         Raises if `V` or `a` are not vectors.
     """
-    if not (V.is_vector() and a.is_vector()):
+    if not V.is_vector() or not a.is_vector():
         raise ValueError("`V` and `a` must be vectors.")
 
-    sp: cs.Sparsity = cs.jacobian(a, V).sparsity()
+    sp: cs.Sparsity = cs.jacobian_sparsity(a, V)
     idx = np.asarray(sp.get_crs()[1], int)
     if idx.size != a.numel():
-        raise RuntimeError(
-            "Invalid subset of target parameters (some were not found among the "
-            "original NLP parameters)."
-        )
+        raise RuntimeError("invalid subset: some entries of `a` were not found in `V`")
     return idx
```

### Comparing `csnlp-1.5.6/src/csnlp/core/debug.py` & `csnlp-1.5.7.dev1/src/csnlp/core/debug.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,14 @@
     NLP debug class for information about variables and constraints. In
     particular, it records information on
      - the decision variable `x`
      - the equality constraints `g`
      - the inequality constraints `h`
     """
 
-    __slots__ = ("_p_info", "_x_info", "_g_info", "_h_info")
     types = MappingProxyType(
         {
             "p": "Parameter",
             "x": "Decision variable",
             "g": "Equality constraint",
             "h": "Inequality constraint",
         }
```

### Comparing `csnlp-1.5.6/src/csnlp/core/derivatives.py` & `csnlp-1.5.7.dev1/src/csnlp/core/derivatives.py`

 * *Files identical despite different names*

### Comparing `csnlp-1.5.6/src/csnlp/core/scaling.py` & `csnlp-1.5.7.dev1/src/csnlp/core/scaling.py`

 * *Files identical despite different names*

### Comparing `csnlp-1.5.6/src/csnlp/core/solutions.py` & `csnlp-1.5.7.dev1/src/csnlp/core/solutions.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 @dataclass(frozen=True, repr=False, order=True)
 class Solution(Generic[SymType]):
     """Class containing information on the solution of an NLP solver's run."""
 
     f: float
     vars: Dict[str, SymType]
     vals: Dict[str, cs.DM]
+    dual_vars: Dict[str, SymType]
+    dual_vals: Dict[str, cs.DM]
     stats: Dict[str, Any]
     _get_value: partial  # Callable[[SymType, bool], Union[SymType, cs.DM]]
 
     @property
     def all_vars(self) -> SymType:
         """Gets all the variables of the solution in a vector."""
         return self._get_value.keywords["old"]
```

### Comparing `csnlp-1.5.6/src/csnlp/multistart/multistart_nlp.py` & `csnlp-1.5.7.dev1/src/csnlp/multistart/multistart_nlp.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,21 +28,14 @@
 
 
 def _n(sym_name: str, scenario: int) -> str:
     """Internal utility for the naming convention of i-scenario's symbols."""
     return f"{sym_name}__{scenario}"
 
 
-def _get_value(
-    x, sol: Solution[SymType], old: SymType, new: SymType, eval: bool = True
-) -> Union[SymType, cs.DM]:
-    """Internal utility for substituting numerical values in multinlp solutions."""
-    return sol._get_value(cs.substitute(x, old, new), eval=eval)
-
-
 def _chained_subevalf(
     expr: Union[SymType, np.ndarray],
     old_vars: Dict[str, SymType],
     new_vars: Dict[str, SymType],
     old_pars: Dict[str, SymType],
     new_pars: Dict[str, SymType],
     old_dual_vars: Optional[Dict[str, SymType]] = None,
@@ -56,15 +49,14 @@
     expr = subsevalf(expr, old_pars, new_pars, eval=False)
     return subsevalf(expr, old_dual_vars, new_dual_vars, eval=eval)
 
 
 class MultistartNlp(Nlp[SymType], Generic[SymType]):
     """Base class for NLP with multistarting."""
 
-    __slots__ = ("_starts",)
     is_multi: ClassVar[bool] = True
 
     def __init__(self, *args, starts: int, **kwargs) -> None:
         """Initializes the multistart NLP instance.
 
         Parameters
         ----------
@@ -129,16 +121,14 @@
 
 class StackedMultistartNlp(MultistartNlp[SymType], Generic[SymType]):
     """A class that models and solves an NLP from multiple starting initial guesses by
     automatically stacking the problem multiple independent times in the same,
     larger-scale NLP. This allows to solve the original problem multiple times via a
     single call to the solver."""
 
-    __slots__ = ("_stacked_nlp", "_fs")
-
     def __init__(self, *args, starts: int, **kwargs) -> None:
         # this class essentially is a facade that hides an internal nlp in which the
         # problem (variables, parameters, etc.) are duplicated by the requested number
         # of multiple starts. For this reason, all methods are overridden to create
         # multiples of these in the hidden nlp.
         super().__init__(*args, starts=starts, **kwargs)
         self._stacked_nlp = Nlp(*args, **kwargs)  # actual nlp
@@ -263,50 +253,70 @@
             }
         multi_sol = self._stacked_nlp.solve(pars, vals0)
         if return_stacked_sol:
             return multi_sol
 
         vars_ = self.variables
         pars_ = self.parameters
-        duals = self.dual_variables
+        duals_ = self.dual_variables
         old = cs.vertcat(
             self._x, self._lam_g, self._lam_h, self._lam_lbx, self._lam_ubx, self._p
         )
         fs = [float(multi_sol._get_value(f)) for f in self._fs]
 
         def get_ith_sol(idx: int) -> Solution[SymType]:
             vals = {n: multi_sol.vals[_n(n, idx)] for n in vars_.keys()}
+            dual_vals = {n: multi_sol.dual_vals[_n(n, idx)] for n in duals_.keys()}
             new = multi_sol._get_value(
                 _chained_subevalf(
                     old,
                     vars_,
                     self._vars_i(idx),
                     pars_,
                     self._pars_i(idx),
-                    duals,
+                    duals_,
                     self._dual_vars_i(idx),
                     False,
                 )
             )
             get_value = partial(subsevalf, old=old, new=new)
-            return Solution(fs[idx], vars_, vals, multi_sol.stats, get_value)
+            return Solution(
+                fs[idx], vars_, vals, duals_, dual_vals, multi_sol.stats, get_value
+            )
 
         if return_all_sols:
             return [get_ith_sol(i) for i in range(self._starts)]
         return get_ith_sol(np.argmin(fs).item())
 
     def __call__(self, *args, **kwargs):
         return self.solve_multi(*args, **kwargs)
 
+    def remove_variable_bounds(
+        self,
+        name: str,
+        direction: Literal["lb", "ub", "both"],
+        idx: Union[Tuple[int, int], List[Tuple[int, int]]] = None,
+    ) -> None:
+        idx = [idx] if isinstance(idx, tuple) else list(idx)
+        super().remove_variable_bounds(name, direction, idx)
+        for i in range(self._starts):
+            self._stacked_nlp.remove_variable_bounds(_n(name, i), direction, idx)
+
+    def remove_constraints(
+        self, name: str, idx: Union[Tuple[int, int], List[Tuple[int, int]]] = None
+    ) -> None:
+        idx = [idx] if isinstance(idx, tuple) else list(idx)
+        super().remove_constraints(name, idx)
+        for i in range(self._starts):
+            self._stacked_nlp.remove_constraints(_n(name, i), idx)
+
 
 class ParallelMultistartNlp(MultistartNlp[SymType], Generic[SymType]):
     """A class that solves an NLP via parallelization of the computations."""
 
-    __slots__ = ("_parallel", "_n_jobs")
-
     def __init__(
         self, *args, starts: int, n_jobs: Optional[int] = None, **kwargs
     ) -> None:
         """Initializes the multistart NLP instance.
 
         Parameters
         ----------
@@ -387,37 +397,21 @@
             ):
                 best_sol = sol
                 best_f = this_f
                 best_success = this_success
             self._failures += not this_success
         return self._process_solver_sol(best_sol)
 
-    def __getstate__(
-        self,
-        fullstate: bool = False,
-    ) -> Union[None, Dict[str, Any], Tuple[Optional[Dict[str, Any]], Dict[str, Any]]]:
+    def __getstate__(self, fullstate: bool = False) -> Dict[str, Any]:
         # joblib.Parallel cannot be pickled or deepcopied
         state = super().__getstate__(fullstate)
-        state[1].pop("_parallel", None)  # type: ignore[index]
+        state.pop("_parallel", None)
         return state
 
-    def __setstate__(
-        self,
-        state: Union[
-            None, Dict[str, Any], Tuple[Optional[Dict[str, Any]], Dict[str, Any]]
-        ],
-    ) -> None:
-        if isinstance(state, tuple) and len(state) == 2:
-            state, slotstate = state
-        else:
-            slotstate = None
+    def __setstate__(self, state: Optional[Dict[str, Any]]) -> None:
         if state is not None:
-            self.__dict__.update(state)  # type: ignore[arg-type]
-        if slotstate is not None:
-            for key, value in slotstate.items():
-                setattr(self, key, value)
-
+            self.__dict__.update(state)
         # re-initialized joblib.Parallel
         if not hasattr(self, "_n_jobs"):
             self._n_jobs = None
         self._parallel = Parallel(n_jobs=self._n_jobs)
         self.initialize_parallel()
```

### Comparing `csnlp-1.5.6/src/csnlp/multistart/startpoints.py` & `csnlp-1.5.7.dev1/src/csnlp/multistart/startpoints.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,16 +4,14 @@
 import numpy.typing as npt
 
 
 class RandomStartPoint:
     """Class containing all the information to guide the random generation of this
     point."""
 
-    __slots__ = ("method", "args", "kwargs")
-
     def __init__(self, method: str, *args: Any, **kwargs: Any) -> None:
         """Instantiates a `RandomStartPoint` object.
 
         Parameters
         ----------
         method : str
             Name of the method of `numpy.random.Generator` that must be used to generate
@@ -26,16 +24,14 @@
         self.kwargs = kwargs
 
 
 class RandomStartPoints:
     """Class that can be iterated to yield a set of random start points for a multistart
     NLP optimization problem."""
 
-    __slots__ = ("np_random", "multistarts", "points")
-
     def __init__(
         self,
         points: Dict[str, RandomStartPoint],
         multistarts: int,
         seed: Optional[int] = None,
     ) -> None:
         """Instantiates the generator of random start points for multistarting.
@@ -75,16 +71,14 @@
 
 
 class StructuredStartPoints:
     """Class that can be iterated to yield a set of structured (deterministic) start
     points for a multistart NLP optimization problem. The points are linearly spaced
     between upper- and lower-bounds."""
 
-    __slots__ = ("multistarts", "points")
-
     def __init__(
         self,
         points: Dict[str, StructuredStartPoint],
         multistarts: int,
     ) -> None:
         """Instantiates the generator of structured start points for multistarting.
```

### Comparing `csnlp-1.5.6/src/csnlp/nlps/constraints.py` & `csnlp-1.5.7.dev1/src/csnlp/nlps/constraints.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,37 +1,22 @@
-from typing import Dict, Literal, Tuple, TypeVar, Union
+from typing import Dict, List, Literal, Tuple, TypeVar, Union
 
 import casadi as cs
 import numpy as np
 import numpy.typing as npt
 
 from csnlp.core.cache import cached_property, invalidate_cache
 from csnlp.nlps.variables import HasVariables
 
 SymType = TypeVar("SymType", cs.SX, cs.MX)
 
 
 class HasConstraints(HasVariables[SymType]):
     """Class for creating and storing symbolic constraints for an NLP problem."""
 
-    __slots__ = (
-        "_dual_vars",
-        "_pars",
-        "_cons",
-        "_lbx",
-        "_ubx",
-        "_lam_lbx",
-        "_lam_ubx",
-        "_g",
-        "_lam_g",
-        "_h",
-        "_lam_h",
-        "_remove_redundant_x_bounds",
-    )
-
     def __init__(
         self,
         sym_type: Literal["SX", "MX"] = "SX",
         remove_redundant_x_bounds: bool = True,
     ) -> None:
         """Instantiate the class.
 
@@ -229,16 +214,16 @@
         mub: np.ma.MaskedArray = np.ma.masked_array(ub, np.ma.nomask)
         if self._remove_redundant_x_bounds:
             mlb.mask = lb == -np.inf
             mub.mask = ub == +np.inf
 
         self._lbx = np.ma.concatenate((self._lbx, mlb))
         self._ubx = np.ma.concatenate((self._ubx, mub))
-        self._lbx.fill_value = -np.inf
-        self._ubx.fill_value = +np.inf
+        np.ma.set_fill_value(self._lbx, -np.inf)
+        np.ma.set_fill_value(self._ubx, +np.inf)
 
         name_lam_lb = f"lam_lb_{name}"
         name_lam_ub = f"lam_ub_{name}"
         lam_lb = self._sym_type.sym(name_lam_lb, (~np.ma.getmaskarray(mlb)).sum())
         lam_ub = self._sym_type.sym(name_lam_ub, (~np.ma.getmaskarray(mub)).sum())
         self._dual_vars[name_lam_lb] = lam_lb
         self._dual_vars[name_lam_ub] = lam_ub
@@ -330,7 +315,147 @@
         name_lam = f"{lam[1:]}_{name}"
         lam_c = self._sym_type.sym(name_lam, shape[0] * shape[1])
         self._dual_vars[name_lam] = lam_c
 
         setattr(self, group, cs.veccat(getattr(self, group), expr))
         setattr(self, lam, cs.veccat(getattr(self, lam), lam_c))
         return (expr, lam_c, slack) if soft else (expr, lam_c)
+
+    @invalidate_cache(
+        nonmasked_lbx_idx, nonmasked_ubx_idx, h_lbx, h_ubx, lam, primal_dual
+    )
+    def remove_variable_bounds(
+        self,
+        name: str,
+        direction: Literal["lb", "ub", "both"],
+        idx: Union[Tuple[int, int], List[Tuple[int, int]]] = None,
+    ) -> None:
+        """Removes one or more lower and/or upper bounds from the given variable
+
+        Parameters
+        ----------
+        name : str
+            Name of the variable whose bounds must be modified
+        direction : {"lb", "ub", "both"}
+            Which bound to modify.
+        idx : tuple[int, int] or a list of, optional
+            A 2D index, or a list of 2D indices, of the variable entries whose
+            corresponding lower/upper bounds must be removed, i.e., set to -/+ inf. If
+            not provided, then all the bounds for that variable are removed.
+
+        Note
+        ----
+        This is a somewhat costly operation, so it is preferable to avoid creating
+        in the first place constraints that will need to be eliminated. Moreover, this
+        operation may compromise the results already obtained in, e.g., sensitivity
+        analysis, because it changes the underlying NLP problem and there is no way to
+        invalidate any user-arbitrary result obtained previously.
+        """
+        # sourcery skip: merge-comparisons
+        n_rows, n_cols = self._vars[name].shape
+        size = n_rows * n_cols
+        if idx is None:
+            idx_ = np.arange(size, dtype=int)
+        else:
+            # transform 2D indices to 1D (casadi column-wise)
+            if isinstance(idx, tuple):
+                idx = (idx,)
+            idx_ = np.asarray([i[0] + i[1] * n_rows for i in idx], int)
+
+        # add offset to skip variable created prior to the current
+        offset = 0
+        for n, other_var in self._vars.items():
+            if n == name:
+                break
+            offset += other_var.shape[0] * other_var.shape[1]
+        idx_ += offset
+
+        # set lbx and ubx to -/+ inf
+        if direction == "both" or direction == "lb":
+            self._lbx[idx_] = -np.inf
+        if direction == "both" or direction == "ub":
+            self._ubx[idx_] = +np.inf
+
+        if self._remove_redundant_x_bounds:
+            # update masks
+            lbx_mask = np.ma.getmaskarray(self._lbx)
+            ubx_mask = np.ma.getmaskarray(self._ubx)
+            lbx_mask[idx_] = ubx_mask[idx_] = True
+            self._lbx.mask = lbx_mask
+            self._ubx.mask = ubx_mask
+
+            # remove obsolete multipliers
+            directions = ("lb", "ub") if direction == "both" else (direction,)
+            for lb_or_ub in directions:
+                name_lam = f"lam_{lb_or_ub}_{name}"
+                bounds = getattr(self, f"_{lb_or_ub}x")[offset : offset + size]
+                mask = np.ma.getmaskarray(bounds)
+                new_lam = self._sym_type.sym(name_lam, (~mask).sum())
+
+                # replace in dict and re-create vector of lbx/ubx multipliers
+                self._dual_vars[name_lam] = new_lam
+                all_lams = [
+                    lam
+                    for n, lam in self._dual_vars.items()
+                    if n.startswith(f"lam_{lb_or_ub}")
+                ]
+                setattr(self, f"_lam_{lb_or_ub}x", cs.vvcat(all_lams))
+
+    @invalidate_cache(lam, primal_dual)
+    def remove_constraints(
+        self,
+        name: str,
+        idx: Union[Tuple[int, int], List[Tuple[int, int]]] = None,
+    ) -> None:
+        """Removes one or more (equality or inequality) constraints from the problem.
+
+        Parameters
+        ----------
+        name : str
+            Name of the constraint to be removed. The name will be used to identify if
+            the constraint is an inequality or an equality constraint.
+        idx : idx : tuple[int, int] or a list of, optional
+            A 2D index, or a list of 2D indices, of the constraint entries that
+            must be removed. If not provided, then the constraint is removed entirely.
+
+        Note
+        ----
+        This is a somewhat costly operation, so it is preferable to avoid creating
+        in the first place constraints that will need to be eliminated. Moreover, this
+        operation may compromise the results already obtained in, e.g., sensitivity
+        analysis, because it changes the underlying NLP problem and there is no way to
+        invalidate any user-arbitrary result obtained previously.
+        """
+        # sourcery skip: merge-comparisons
+        old_con = self._cons.pop(name)
+        group = "g" if f"lam_g_{name}" in self._dual_vars else "h"
+        this_name_lam = f"lam_{group}_{name}"
+        self._dual_vars.pop(this_name_lam)
+        if idx is not None:
+            # transform 2D indices to 1D (casadi column-wise) and keep only the
+            # remaining indices
+            n_rows = old_con.size1()
+            if isinstance(idx, tuple):
+                idx = (idx,)
+            idx_to_remove = {i[0] + i[1] * n_rows for i in idx}
+
+            # remove constraints and re-create corresponding multipliers
+            old_con = cs.vec(old_con)  # flatten the constraint - cannot do otherwise
+            idx_ = [i for i in range(old_con.size1()) if i not in idx_to_remove]
+            new_con = old_con[idx_]
+            self._cons[name] = new_con
+            self._dual_vars[this_name_lam] = self._sym_type.sym(
+                this_name_lam, new_con.size1()
+            )
+
+        # re-create constraints and multipliers vectors, and refresh the solver
+        new_cons = []
+        new_lams = []
+        for n, con in self._cons.items():
+            name_lam = f"lam_{group}_{n}"
+            if name_lam in self._dual_vars:
+                new_cons.append(con)
+                new_lams.append(self._dual_vars[name_lam])
+        setattr(self, f"_{group}", cs.vvcat(new_cons))
+        setattr(self, f"_lam_{group}", cs.vcat(new_lams))
+        if hasattr(self, "refresh_solver"):
+            self.refresh_solver()
```

### Comparing `csnlp-1.5.6/src/csnlp/nlps/nlp.py` & `csnlp-1.5.7.dev1/src/csnlp/nlps/nlp.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,14 @@
     optimization problem to yield a (possibly, sub-) optimal solution.
 
     This is a generic class in the sense that it does not solve a particular
     problem, but only offers the generic methods to build one (e.g., variables,
     constraints, objective, solver).
     """
 
-    __slots__ = ("id", "_debug")
     __ids: ClassVar[Iterator[int]] = count(0)
     is_multi: ClassVar[bool] = False
 
     def __init__(
         self,
         sym_type: Literal["SX", "MX"] = "SX",
         remove_redundant_x_bounds: bool = True,
```

### Comparing `csnlp-1.5.6/src/csnlp/nlps/objective.py` & `csnlp-1.5.7.dev1/src/csnlp/nlps/objective.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,24 +30,14 @@
     return sol
 
 
 class HasObjective(HasConstraints[SymType]):
     """Class for creating an NLP problem with parameters, variables, constraints and an
     objective."""
 
-    __slots__ = (
-        "name",
-        "_f",
-        "_solver",
-        "_solver_opts",
-        "_solver_type",
-        "_cache",
-        "_failures",
-    )
-
     def __init__(
         self,
         sym_type: Literal["SX", "MX"] = "SX",
         remove_redundant_x_bounds: bool = True,
         cache: Memory = None,
         name: Optional[str] = None,
     ) -> None:
@@ -239,19 +229,40 @@
             if vals0diff := self._vars.keys() - vals0.keys():
                 vals0.update({v: 0 for v in vals0diff})  # type: ignore[has-type]
             kwargs["x0"] = subsevalf(self._x, self._vars, vals0)
         return kwargs
 
     def _process_solver_sol(self, sol: Dict[str, Any]) -> Solution:
         """Internal utility to convert the solver sol dict to a Solution instance."""
+        # objective
+        f = float(sol["f"])
+
+        # primal variables and values
+        vars = self.variables
+        vals = {name: subsevalf(var, self._x, sol["x"]) for name, var in vars.items()}
+
+        # dual variables and values
         lam_lbx = -cs.fmin(sol["lam_x"], 0)[self.nonmasked_lbx_idx, :]
         lam_ubx = cs.fmax(sol["lam_x"], 0)[self.nonmasked_ubx_idx, :]
         lam_g = sol["lam_g"][: self.ng, :]
         lam_h = sol["lam_g"][self.ng :, :]
-        vars = self.variables
-        vals = {name: subsevalf(var, self._x, sol["x"]) for name, var in vars.items()}
+        dual_vars = self.dual_variables
+        dual_vals = {}
+        for n, var in dual_vars.items():
+            if n.startswith("lam_lb"):
+                dual_vals[n] = subsevalf(var, self._lam_lbx, lam_lbx)
+            elif n.startswith("lam_ub"):
+                dual_vals[n] = subsevalf(var, self._lam_ubx, lam_ubx)
+            elif n.startswith("lam_g"):
+                dual_vals[n] = subsevalf(var, self._lam_g, lam_g)
+            elif n.startswith("lam_h"):
+                dual_vals[n] = subsevalf(var, self._lam_h, lam_h)
+            else:
+                raise RuntimeError(f"unknown dual variable type {n}")
+
+        # get_value function
         old = cs.vertcat(
             self._x, self._lam_g, self._lam_h, self._lam_lbx, self._lam_ubx, self._p
         )
         new = cs.vertcat(sol["x"], lam_g, lam_h, lam_lbx, lam_ubx, sol["p"])
         get_value = partial(subsevalf, old=old, new=new)
-        return Solution(float(sol["f"]), vars, vals, sol["stats"], get_value)
+        return Solution(f, vars, vals, dual_vars, dual_vals, sol["stats"], get_value)
```

### Comparing `csnlp-1.5.6/src/csnlp/nlps/parameters.py` & `csnlp-1.5.7.dev1/src/csnlp/nlps/parameters.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,16 +4,14 @@
 
 SymType = TypeVar("SymType", cs.SX, cs.MX)
 
 
 class HasParameters(Generic[SymType]):
     """Class for creating and storing symbolic parameters of an NLP problem."""
 
-    __slots__ = ("_sym_type", "_pars", "_p")
-
     def __init__(self, sym_type: Literal["SX", "MX"] = "SX") -> None:
         """Instantiate the class.
 
         Parameters
         ----------
         sym_type : "SX" or "MX", optional
             The CasADi symbolic variable type to use in the NLP, by default "SX".
```

### Comparing `csnlp-1.5.6/src/csnlp/nlps/variables.py` & `csnlp-1.5.7.dev1/src/csnlp/nlps/variables.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,16 +6,14 @@
 
 SymType = TypeVar("SymType", cs.SX, cs.MX)
 
 
 class HasVariables(HasParameters[SymType]):
     """Class for creating and storing symbolic variables of an NLP problem."""
 
-    __slots__ = ("_vars", "_x")
-
     def __init__(self, sym_type: Literal["SX", "MX"] = "SX") -> None:
         """Instantiate the class.
 
         Parameters
         ----------
         sym_type : "SX" or "MX", optional
             The CasADi symbolic variable type to use in the NLP, by default "SX".
```

### Comparing `csnlp-1.5.6/src/csnlp/util/docs.py` & `csnlp-1.5.7.dev1/src/csnlp/util/docs.py`

 * *Files identical despite different names*

### Comparing `csnlp-1.5.6/src/csnlp/util/io.py` & `csnlp-1.5.7.dev1/src/csnlp/util/io.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,25 @@
 import pickle
-from copy import _reconstruct, deepcopy  # type: ignore[attr-defined]
-from functools import cached_property
-from inspect import getmembers
-from itertools import chain
+from copy import _reconstruct, deepcopy
 from os.path import splitext
 from pickletools import optimize
 from typing import (
     TYPE_CHECKING,
     Any,
     Callable,
     Dict,
-    Iterable,
     List,
     Literal,
     Optional,
-    Tuple,
     Type,
     TypeVar,
-    Union,
 )
 
+from csnlp.core.cache import invalidate_caches_of
+
 if TYPE_CHECKING:
     from scipy.io.matlab import mat_struct
 
 
 def is_casadi_object(obj: Any) -> bool:
     """Checks if the object belongs to the CasADi module.
 
@@ -61,34 +57,14 @@
     try:
         pickle.dumps(obj)
         return True
     except Exception:
         return False
 
 
-def _get_dict_state(
-    obj: "SupportsDeepcopyAndPickle",
-    attributes: Iterable[str],
-    fullstate: bool,
-    remove_None: bool,
-) -> Dict[str, Any]:
-    """Internal utility for SupportsDeepcopyAndPickle."""
-    state: Dict[str, Any] = {attr: getattr(obj, attr, None) for attr in attributes}
-    if not fullstate:
-        for attr in list(state.keys()):
-            val = state[attr]
-            if (
-                (remove_None and val is None)
-                or is_casadi_object(val)
-                or not is_pickleable(val)
-            ):
-                state.pop(attr, None)
-    return state
-
-
 T = TypeVar("T", bound="SupportsDeepcopyAndPickle")
 
 
 class SupportsDeepcopyAndPickle:
     """Class that defines a `__getstate__` that is compatible with both `deepcopy` and
     `pickle`, as well as any other operation that requires the instance's state.
 
@@ -108,52 +84,41 @@
         Returns
         -------
         `SupportsDeepcopyAndPickle` or its subclass
             A deepcopy of this instance.
         """
         new = deepcopy(self)
         if invalidate_caches:
-            # basically do again what csnlp.util.funcs.invalidate_cache does
-            for membername, member in getmembers(type(new)):
-                if hasattr(member, "cache_clear"):
-                    getattr(new, membername).cache_clear()
-                elif isinstance(member, cached_property):
-                    if membername in new.__dict__:
-                        del new.__dict__[membername]
+            invalidate_caches_of(new)
         return new
 
     def __deepcopy__(self: T, memo: Optional[Dict[int, List[Any]]] = None) -> T:
         """Returns a deepcopy of the object."""
         rv = self.__reduce_ex__(4)
         if isinstance(rv, str):
             return self
         assert len(rv) < 6 or rv[5] is None, "Unexpected reductor callable."
         # overwrite the filtered state with its full version
         fullstate = self.__getstate__(True)
         new_rv = (*rv[:2], fullstate, *rv[3:])
         return _reconstruct(self, memo, *new_rv)
 
-    def __getstate__(
-        self: T,
-        fullstate: bool = False,
-    ) -> Union[None, Dict[str, Any], Tuple[Optional[Dict[str, Any]], Dict[str, Any]]]:
+    def __getstate__(self: T, fullstate: bool = False) -> Optional[Dict[str, Any]]:
         """Returns the instance's state to be pickled/deepcopied."""
         # https://docs.python.org/3/library/pickle.html#pickle-inst
-        dictstate = (
-            _get_dict_state(self, self.__dict__.keys(), fullstate, False)
-            if hasattr(self, "__dict__") and self.__dict__.keys()
-            else None
-        )
-        slots = list(
-            chain.from_iterable(
-                getattr(cls, "__slots__", []) for cls in type(self).__mro__
-            )
-        )
-        slotstate = _get_dict_state(self, slots, fullstate, True) if slots else None
-        return (dictstate, slotstate) if slotstate is not None else dictstate
+        if not (hasattr(self, "__dict__") and self.__dict__.keys()):
+            return None
+        state = self.__dict__.copy()
+        if fullstate:
+            return state
+        state_items_copy = list(state.items())
+        for attr, val in state_items_copy:
+            if is_casadi_object(val) or not is_pickleable(val):
+                state.pop(attr, None)
+        return state
 
 
 _COMPRESSION_EXTS: Dict[str, Optional[str]] = {
     ".pkl": None,
     ".xz": "lzma",
     ".pbz2": "bz2",
     ".gz": "gzip",
@@ -197,17 +162,15 @@
     -------
     filename : str
         The complete name of the file where the data was written to.
     """
 
     actual_ext = splitext(filename)[1]
     if compression is None:
-        compression = _COMPRESSION_EXTS.get(  # type: ignore[assignment]
-            actual_ext, None
-        )
+        compression = _COMPRESSION_EXTS.get(actual_ext)
 
     open_fun: Callable
     compress_fun: Callable
     if compression is None:
         expected_ext = ".pkl"
         open_fun = open
         compress_fun = lambda o: o  # noqa E731
```

### Comparing `csnlp-1.5.6/src/csnlp/util/math.py` & `csnlp-1.5.7.dev1/src/csnlp/util/math.py`

 * *Files identical despite different names*

### Comparing `csnlp-1.5.6/src/csnlp/util/plot.py` & `csnlp-1.5.7.dev1/src/csnlp/util/plot.py`

 * *Files identical despite different names*

### Comparing `csnlp-1.5.6/src/csnlp/wrappers/mpc.py` & `csnlp-1.5.7.dev1/src/csnlp/wrappers/mpc.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,28 +22,14 @@
 
     References
     ----------
     [1] Rawlings, J.B., Mayne, D.Q. and Diehl, M., 2017. Model Predictive Control:
         theory, computation, and design (Vol. 2). Madison, WI: Nob Hill Publishing.
     """
 
-    __slots__ = (
-        "_is_multishooting",
-        "_prediction_horizon",
-        "_control_horizon",
-        "_input_spacing",
-        "_states",
-        "_initial_states",
-        "_actions",
-        "_actions_exp",
-        "_slacks",
-        "_disturbances",
-        "_dynamics",
-    )
-
     def __init__(
         self,
         nlp: Nlp[SymType],
         prediction_horizon: int,
         control_horizon: Optional[int] = None,
         input_spacing: int = 1,
         shooting: Literal["single", "multi"] = "multi",
@@ -234,16 +220,16 @@
         if self._is_multishooting:
             x = self.nlp.variable(name, (size, self._prediction_horizon + 1), lb, ub)[0]
             x0 = self.nlp.parameter(x0_name, (size, 1))
             self.nlp.constraint(x0_name, x[:, 0], "==", x0)
         else:
             if np.any(lb != -np.inf) or np.any(ub != +np.inf):
                 raise RuntimeError(
-                    "In single shooting, lower and upper state bounds can only"
-                    " be created after the dynamics have been set"
+                    "in single shooting, lower and upper state bounds can only be "
+                    "created after the dynamics have been set"
                 )
             x = None
             x0 = self.nlp.parameter(x0_name, (size, 1))
         self._states[name] = x
         self._initial_states[x0_name] = x0
         return x, x0
```

### Comparing `csnlp-1.5.6/src/csnlp/wrappers/scaling.py` & `csnlp-1.5.7.dev1/src/csnlp/wrappers/scaling.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,16 +14,14 @@
 
 class NlpScaling(NonRetroactiveWrapper[SymType]):
     """
     Wraps an NLP problem to facilitate the scaling of parameters and variables as well
     as the automatic scaling of expression (e.g., objective and constraints).
     """
 
-    __slots__ = ("scaler", "warns", "_svars", "_spars", "_uvars", "_upars")
-
     def __init__(self, nlp: Nlp[SymType], scaler: Scaler, warns: bool = True) -> None:
         """Initializes a scaling wrapper around an NLP instance.
 
         Parameters
         ----------
         nlp : Nlp[T]
             The NLP problem to be wrapped.
```

### Comparing `csnlp-1.5.6/src/csnlp/wrappers/sensitivity.py` & `csnlp-1.5.7.dev1/src/csnlp/wrappers/sensitivity.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,16 +25,14 @@
     ----------
     [1] Buskens, C. and Maurer, H. (2001). Sensitivity analysis and real-time
         optimization of parametric nonlinear programming problems. In M. Grotschel, S.O.
         Krumke, and J. Rambau (eds.), Online Optimization of Large Scale Systems, 3–16.
         Springer, Berlin, Heidelberg.
     """
 
-    __slots__ = ("include_barrier_term", "_p_idx_internal", "_tau")
-
     def __init__(
         self,
         nlp: Nlp[SymType],
         target_parameters: Optional[SymType] = None,
         include_barrier_term: bool = True,
     ) -> None:
         """Instantiates the wrapper for performing NLP sensitivities.
@@ -171,28 +169,31 @@
             "K-py": hojacobian(Kp, y)[..., 0],
         }
 
     @property
     def licq(self) -> SymType:
         """Gets the symbolic matrix for LICQ, defined as
         ```
-                    LICQ = [ dgdx^T, dhdx^T ]^T
+                    LICQ = [ dg dx, dh dx, dh_lbx dx, dh_ubx dx ]
         ```
         If the matrix is linear independent, then the NLP satisfies the Linear
         Independence Constraint Qualification.
 
-        Note:
-            1) the LICQ are computed for only the active inenquality constraints. Since
-               this is a symbolic representation, all are included, and it's up to the
-               user to eliminate the inactive.
-
-            2) lower and upper bound inequality constraints are not included in `h`
-               since they are by nature linear independent.
+        Note
+        -----
+        The LICQ is computed for only the active inenquality constraints. Since this is
+        a symbolic representation, all constraints are included, and it's up to the user
+        to eliminate the inactive ones.
         """
-        return cs.vertcat(self.jacobians["g-x"], self.jacobians["h-x"])
+        return cs.vertcat(
+            self.jacobians["g-x"],
+            self.jacobians["h-x"],
+            cs.jacobian(self.nlp.h_lbx, self.nlp.x),
+            cs.jacobian(self.nlp.h_ubx, self.nlp.x),
+        )
 
     def parametric_sensitivity(
         self,
         expr: SymType = None,
         solution: Optional[Solution[SymType]] = None,
         second_order: bool = False,
     ) -> Union[Tuple[SymType, Optional[SymType]], Tuple[cs.DM, Optional[cs.DM]]]:
```

### Comparing `csnlp-1.5.6/src/csnlp/wrappers/wrapper.py` & `csnlp-1.5.7.dev1/src/csnlp/wrappers/wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,16 +15,14 @@
     behavior of the original environment without touching the original code.
 
     The base class is retroactive, in the sense that it can be applied to any NLP
     instance that already defines variables, parameters, and/or objective. Use
     `NonRetroactiveWrapper` for wrappers that need to wrap an NLP before it is defined.
     """
 
-    __slots__ = ("nlp",)
-
     def __init__(self, nlp: Nlp[SymType]) -> None:
         """Wraps an NLP instance.
 
         Parameters
         ----------
         nlp : Nlp or subclass
             The NLP to wrap.
```

### Comparing `csnlp-1.5.6/src/csnlp.egg-info/PKG-INFO` & `csnlp-1.5.7.dev1/src/csnlp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csnlp
-Version: 1.5.6
+Version: 1.5.7.dev1
 Summary: Nonlinear Progamming with CasADi
 Author-email: Filippo Airaldi <filippoairaldi@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/FilippoAiraldi/casadi-nlp
 Project-URL: Bug Tracker, https://github.com/FilippoAiraldi/casadi-nlp/issues
 Keywords: nonlinear-optimization,casadi,sensitivity-analysis
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `csnlp-1.5.6/src/csnlp.egg-info/SOURCES.txt` & `csnlp-1.5.7.dev1/src/csnlp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `csnlp-1.5.6/tests/test_core.py` & `csnlp-1.5.7.dev1/tests/test_core.py`

 * *Files 5% similar despite different names*

```diff
@@ -222,32 +222,53 @@
         f = 0
         shape = (3, 4)
         V = {
             "x": (XX.sym("x", *shape), np.random.rand(*shape) * 10),
             "y": (XX.sym("y", *shape), np.random.rand(*shape) * 5),
             "z": (XX.sym("z"), np.random.rand() + 1),
         }
+        D = {
+            "dx": (XX.sym("dx", *shape), np.random.rand(*shape) * 10),
+            "dy": (XX.sym("dy", *shape), np.random.rand(*shape) * 5),
+            "dz": (XX.sym("dz"), np.random.rand() + 1),
+        }
         V_vec = cs.vertcat(*(cs.vec(v) for _, v in V.values()))
+        D_vec = cs.vertcat(*(cs.vec(d) for _, d in D.values()))
         V_struct = struct_X([entry(n, expr=s) for n, (s, _) in V.items()])
-        expr, expected_val = ((V["x"][i] / V["y"][i]) ** V["z"][i] for i in range(2))
+        D_struct = struct_X([entry(n, expr=s) for n, (s, _) in D.items()])
+
+        expr, expected_val = (
+            ((V["x"][i] + D["dx"][i]) / V["y"][i] / D["dy"][i])
+            ** (V["z"][i] - D["dz"][i])
+            for i in range(2)
+        )
 
-        vals = V_struct(V_vec)
-        get_value = partial(subsevalf, old=V_struct, new=vals)
+        all_vars = cs.vertcat(V_struct, D_struct)
+        all_vals = cs.vertcat(V_struct(V_vec), D_struct(D_vec))
+        get_value = partial(subsevalf, old=all_vars, new=all_vals)
         S = Solution(
-            f=f, vars=V_struct, vals=V_struct(V_vec), stats={}, _get_value=get_value
+            f=f,
+            vars=V_struct,
+            vals=V_struct(V_vec),
+            dual_vars=D_struct,
+            dual_vals=D_struct(V_vec),
+            stats={},
+            _get_value=get_value,
         )
         np.testing.assert_allclose(expected_val, S.value(expr))
 
     @parameterized.expand([(False,), (True,)])
     def test_solution__reports_success_and_barrier_properly(self, flag: bool):
         mu = np.abs(np.random.randn(10)).tolist()
         S = Solution(
             f=None,
             vars=None,
             vals=None,
+            dual_vars=None,
+            dual_vals=None,
             stats={"success": flag, "iterations": {"mu": mu}},
             _get_value=lambda x: x,
         )
         self.assertEqual(S.success, flag)
         self.assertEqual(S.barrier_parameter, mu[-1])
```

### Comparing `csnlp-1.5.6/tests/test_examples.py` & `csnlp-1.5.7.dev1/tests/test_examples.py`

 * *Files 2% similar despite different names*

```diff
@@ -136,24 +136,24 @@
 
     def test__rosenbrock(self):
         nlp = Nlp(sym_type=self.sym_type)
         x = nlp.variable("x", (2, 1))[0]
         r = nlp.parameter("r")
         f = (1 - x[0]) ** 2 + (x[1] - x[0] ** 2) ** 2
         nlp.minimize(f)
-        _, lam = nlp.constraint("con1", cs.sumsqr(x), "<=", r)
+        nlp.constraint("con1", cs.sumsqr(x), "<=", r)
         nlp.init_solver(OPTS)
         nlp = nlp.copy()
         r_values = np.linspace(1, 3, 25)
         f_values = []
         lam_values = []
         for r_value in r_values:
             sol = nlp.solve(pars={"r": r_value})
             f_values.append(sol.f)
-            lam_values.append(sol.value(lam))
+            lam_values.append(sol.dual_vals["lam_h_con1"])
         f_values = np.asarray(f_values).squeeze()
         lam_values = np.asarray(lam_values).squeeze()
         np.testing.assert_allclose(f_values, RESULTS["rosenbrock_f"])
         np.testing.assert_allclose(lam_values, RESULTS["rosenbrock_lam"])
 
     def test__sensitivity(self):
         def z1(x, lam, p):
```

### Comparing `csnlp-1.5.6/tests/test_multistart.py` & `csnlp-1.5.7.dev1/tests/test_multistart.py`

 * *Files identical despite different names*

### Comparing `csnlp-1.5.6/tests/test_nlps.py` & `csnlp-1.5.7.dev1/tests/test_nlps.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import pickle
 import unittest
+from itertools import product
 from typing import List, Union
 
 import casadi as cs
 import numpy as np
 from parameterized import parameterized, parameterized_class
 
 from csnlp import Nlp
@@ -582,10 +583,128 @@
         nlp.constraint("c2", g, "<=", p**2)
         nlp.init_solver(OPTS)
 
         nlp2 = pickle.loads(pickle.dumps(nlp))
 
         self.assertEqual(nlp.name, nlp2.name)
 
+    @parameterized.expand(product(("both", "lb", "ub"), (True, False)))
+    def test_remove_variable_bounds__remove_bounds_correctly(
+        self, direction: str, all_idx: bool
+    ):
+        shape = tuple(np.random.randint(3, 10, size=2))
+        lb = np.random.rand(*shape) - 3
+        ub = np.random.rand(*shape) + 3
+        if all_idx:
+            idx_to_remove = list(product(range(shape[0]), range(shape[1])))
+        else:
+            n_to_remove = np.random.randint(1, np.prod(shape) // 2)
+            idx_to_remove = np.random.randint((0, 0), shape, size=(n_to_remove, 2))
+
+        nlp = Nlp(sym_type=self.sym_type, remove_redundant_x_bounds=True)
+        u_size = np.prod(nlp.variable("u", (5, 2), ub=+1)[0].shape)  # to create noise
+        nlp.variable("x", shape, lb=lb, ub=ub)
+        nlp.variable("z", (7, 9), lb=+2, ub=+3)  # to create noise
+        nlp.remove_variable_bounds("x", direction, None if all_idx else idx_to_remove)
+
+        if direction in {"both", "lb"}:
+            lb_ = lb.copy()
+            lb_mask_ = np.full(lb.shape, False)
+            for i in idx_to_remove:
+                lb_[tuple(i)] = -np.inf
+                lb_mask_[tuple(i)] = True
+            exp_lb = nlp.lbx.data[u_size : u_size + np.prod(shape)]
+            exp_lb_mask = nlp.lbx.mask[u_size : u_size + np.prod(shape)]
+            np.testing.assert_array_equal(lb_.reshape(-1, order="F"), exp_lb)
+            np.testing.assert_array_equal(lb_mask_.reshape(-1, order="F"), exp_lb_mask)
+            self.assertTrue(
+                nlp.dual_variables["lam_lb_x"].size1() == (~exp_lb_mask).sum()
+            )
+            self.assertTrue(nlp.h_lbx.shape == nlp.lam_lbx.shape)
+        if direction in {"both", "ub"}:
+            ub_ = ub.copy()
+            ub_mask_ = np.full(ub.shape, False)
+            for i in idx_to_remove:
+                ub_[tuple(i)] = +np.inf
+                ub_mask_[tuple(i)] = True
+            exp_ub = nlp.ubx.data[u_size : u_size + np.prod(shape)]
+            exp_ub_mask = nlp.ubx.mask[u_size : u_size + np.prod(shape)]
+            np.testing.assert_array_equal(ub_.reshape(-1, order="F"), exp_ub)
+            np.testing.assert_array_equal(ub_mask_.reshape(-1, order="F"), exp_ub_mask)
+            self.assertTrue(
+                nlp.dual_variables["lam_ub_x"].size1() == (~exp_ub_mask).sum()
+            )
+            self.assertTrue(nlp.h_ubx.shape == nlp.lam_ubx.shape)
+
+    @parameterized.expand(product(("both", "g", "h"), (False, True)))
+    def test_remove_constraints__remove_bounds_correctly(
+        self, remove: str, all_idx: bool
+    ):
+        nlp = Nlp(sym_type=self.sym_type)
+        x = nlp.variable("x", tuple(np.random.randint(2, 5, size=2)))[0]
+        y = nlp.variable("y", tuple(np.random.randint(2, 5, size=2)))[0]
+        z = nlp.variable("z", tuple(np.random.randint(2, 5, size=2)))[0]  # noise
+        w = nlp.variable("w", tuple(np.random.randint(2, 5, size=2)))[0]  # noise
+        q = nlp.variable("q", tuple(np.random.randint(2, 5, size=2)))[0]  # noise
+        p = nlp.variable("p", tuple(np.random.randint(2, 5, size=2)))[0]  # noise
+        nlp.minimize(cs.sumsqr(cs.veccat(x, y, z, w, q, p)))
+        nlp.constraint("h0", z, ">=", 0.0)  # noise
+        nlp.constraint("h1", x, ">=", 1.0)
+        nlp.constraint("h2", q, ">=", 0.0)  # noise
+        nlp.constraint("g0", w, "==", 0.0)  # noise
+        nlp.constraint("g1", y, "==", 2.0)
+        nlp.constraint("g2", p, "==", 0.0)  # noise
+        nlp.init_solver(OPTS)
+
+        if all_idx:
+            idx_to_remove_h1 = idx_to_remove_g1 = None
+        else:
+            n_to_remove = np.random.randint(1, np.prod(x.shape) // 2)
+            idx_to_remove_h1 = np.unique(
+                np.random.randint((0, 0), x.shape, size=(n_to_remove, 2)), axis=0
+            )
+            n_to_remove = np.random.randint(1, np.prod(y.shape) // 2)
+            idx_to_remove_g1 = np.unique(
+                np.random.randint((0, 0), y.shape, size=(n_to_remove, 2)), axis=0
+            )
+        remove_h = remove in {"both", "h"}
+        remove_g = remove in {"both", "g"}
+        if remove_h:
+            nlp.remove_constraints("h1", idx_to_remove_h1)
+        if remove_g:
+            nlp.remove_constraints("g1", idx_to_remove_g1)
+
+        sol = nlp.solve()
+
+        expected_nh = cs.veccat(z, x, q).size1()
+        expected_ng = cs.veccat(w, y, p).size1()
+        expected_x = np.full(x.shape, 1.0)
+        expected_y = np.full(y.shape, 2.0)
+        if remove_h:
+            if all_idx:
+                expected_nh -= np.prod(x.shape)
+                expected_x.fill(0.0)
+            else:
+                expected_nh -= idx_to_remove_h1.shape[0]
+                for idx in idx_to_remove_h1:
+                    expected_x[idx[0], idx[1]] = 0.0
+        if remove_g:
+            if all_idx:
+                expected_ng -= np.prod(y.shape)
+                expected_y.fill(0.0)
+            else:
+                expected_ng -= idx_to_remove_g1.shape[0]
+                for idx in idx_to_remove_g1:
+                    expected_y[idx[0], idx[1]] = 0.0
+
+        self.assertEqual(nlp.nh, expected_nh)
+        self.assertEqual(nlp.ng, expected_ng)
+        np.testing.assert_allclose(sol.vals["z"], 0.0, atol=1e-4, rtol=1e-4)
+        np.testing.assert_allclose(sol.vals["x"], expected_x, atol=1e-4, rtol=1e-4)
+        np.testing.assert_allclose(sol.vals["q"], 0.0, atol=1e-4, rtol=1e-4)
+        np.testing.assert_allclose(sol.vals["w"], 0.0, atol=1e-4, rtol=1e-4)
+        np.testing.assert_allclose(sol.vals["y"], expected_y, atol=1e-4, rtol=1e-4)
+        np.testing.assert_allclose(sol.vals["p"], 0.0, atol=1e-4, rtol=1e-4)
+
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `csnlp-1.5.6/tests/test_quadrotor_mpc.py` & `csnlp-1.5.7.dev1/tests/test_quadrotor_mpc.py`

 * *Files identical despite different names*

### Comparing `csnlp-1.5.6/tests/test_util.py` & `csnlp-1.5.7.dev1/tests/test_util.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,37 +17,21 @@
 TMPFILENAME: str = ""
 
 
 class EmptyClass(io.SupportsDeepcopyAndPickle):
     ...
 
 
-class SlotsClass(EmptyClass):
-    __slots__ = ("x", "y", "sym1")
-
-    def __init__(self) -> None:
-        super().__init__()
-        self.x, self.y = 1, 2
-        self.sym1 = cs.SX.sym("x", 2, 1)
-
-
 class DictClass(EmptyClass):
     def __init__(self) -> None:
         super().__init__()
         self.z, self.w = 3, 4
         self.sym2 = cs.SX.sym("y", 3, 1)
 
 
-class SlotsAndDictClass(SlotsClass):
-    def __init__(self) -> None:
-        super().__init__()
-        self.z, self.w = 3, 4
-        self.sym2 = cs.SX.sym("y", 3, 1)
-
-
 class TestIo(unittest.TestCase):
     @parameterized.expand(
         [
             (5.0, False),
             (unittest.TestCase(), False),
             (cs.DM(5), True),
             (cs.SX.sym("x"), True),
@@ -96,46 +80,28 @@
             os.remove(TMPFILENAME)
         finally:
             return super().tearDown()
 
     @parameterized.expand([(False,), (True,)])
     def test_is_pickleable_and_deepcopy_able(self, copy: bool):
         ec = EmptyClass()
-        sc = SlotsClass()
         dc = DictClass()
-        sdc = SlotsAndDictClass()
         if copy:
             ec1 = ec.copy()
-            sc1 = sc.copy()
             dc1 = dc.copy()
-            sdc1 = sdc.copy()
         else:
             ec1 = pickle.loads(pickle.dumps(ec))
-            sc1 = pickle.loads(pickle.dumps(sc))
             dc1 = pickle.loads(pickle.dumps(dc))
-            sdc1 = pickle.loads(pickle.dumps(sdc))
         self.assertIsNot(ec, ec1)
-        self.assertIsNot(sc, sc1)
-        self.assertTupleEqual((sc.x, sc.y), (sc1.x, sc1.y))
         self.assertIsNot(dc, dc1)
         self.assertTupleEqual((dc.z, dc.w), (dc1.z, dc1.w))
-        self.assertIsNot(sdc, sdc1)
-        self.assertTupleEqual(
-            (sdc.x, sdc.y, sdc.z, sdc.w), (sdc1.x, sdc1.y, sdc1.z, sdc1.w)
-        )
         if copy:
-            self.assertTupleEqual(sc.sym1.shape, sc1.sym1.shape)
             self.assertTupleEqual(dc.sym2.shape, dc1.sym2.shape)
-            self.assertTupleEqual(
-                (sdc.sym1.shape, sdc.sym2.shape), (sdc1.sym1.shape, sdc1.sym2.shape)
-            )
         else:
-            self.assertFalse(hasattr(sc1, "sym1"))
             self.assertFalse(hasattr(dc1, "sym2"))
-            self.assertFalse(hasattr(sdc1, "sym1") or hasattr(sdc1, "sym2"))
 
 
 class TestMath(unittest.TestCase):
     def test_log(self):
         base = np.random.rand() * 10
         x = np.random.rand() * 10
         self.assertEqual(math.log(x), _math.log(x))
```

### Comparing `csnlp-1.5.6/tests/test_wrappers.py` & `csnlp-1.5.7.dev1/tests/test_wrappers.py`

 * *Files identical despite different names*

