# Comparing `tmp/rapids_singlecell-0.7.2.tar.gz` & `tmp/rapids_singlecell-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rapids_singlecell-0.7.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "rapids_singlecell-0.7.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `rapids_singlecell-0.7.2.tar` & `rapids_singlecell-0.7.5.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     1070 2023-06-24 21:46:06.256052 rapids_singlecell-0.7.2/LICENSE
--rw-r--r--   0        0        0     5987 2023-06-24 21:46:06.256052 rapids_singlecell-0.7.2/README.md
--rw-r--r--   0        0        0     1062 2023-06-24 21:46:06.552057 rapids_singlecell-0.7.2/pyproject.toml
--rwxr-xr-x   0        0        0      132 2023-06-24 21:46:06.552057 rapids_singlecell-0.7.2/rapids_singlecell/__init__.py
--rw-r--r--   0        0        0    24992 2023-06-24 21:46:06.552057 rapids_singlecell-0.7.2/rapids_singlecell/cunnData/__init__.py
--rw-r--r--   0        0        0      334 2023-06-24 21:46:06.552057 rapids_singlecell-0.7.2/rapids_singlecell/cunnData_funcs/__init__.py
--rw-r--r--   0        0        0    36773 2023-06-24 21:46:06.552057 rapids_singlecell-0.7.2/rapids_singlecell/cunnData_funcs/_hvg.py
--rw-r--r--   0        0        0    14581 2023-06-24 21:46:06.552057 rapids_singlecell-0.7.2/rapids_singlecell/cunnData_funcs/_normalize.py
--rw-r--r--   0        0        0     4544 2023-06-24 21:46:06.552057 rapids_singlecell-0.7.2/rapids_singlecell/cunnData_funcs/_pca.py
--rw-r--r--   0        0        0     2783 2023-06-24 21:46:06.552057 rapids_singlecell-0.7.2/rapids_singlecell/cunnData_funcs/_plotting.py
--rw-r--r--   0        0        0     4795 2023-06-24 21:46:06.552057 rapids_singlecell-0.7.2/rapids_singlecell/cunnData_funcs/_regress_out.py
--rw-r--r--   0        0        0     1459 2023-06-24 21:46:06.552057 rapids_singlecell-0.7.2/rapids_singlecell/cunnData_funcs/_scale.py
--rw-r--r--   0        0        0    18267 2023-06-24 21:46:06.552057 rapids_singlecell-0.7.2/rapids_singlecell/cunnData_funcs/_simple.py
--rw-r--r--   0        0        0     3351 2023-06-24 21:46:06.552057 rapids_singlecell-0.7.2/rapids_singlecell/cunnData_funcs/_utils.py
--rw-r--r--   0        0        0       29 2023-06-24 21:46:06.552057 rapids_singlecell-0.7.2/rapids_singlecell/dcg.py
--rw-r--r--   0        0        0       68 2023-06-24 21:46:06.552057 rapids_singlecell-0.7.2/rapids_singlecell/decoupler_gpu/__init__.py
--rw-r--r--   0        0        0     4609 2023-06-24 21:46:06.552057 rapids_singlecell-0.7.2/rapids_singlecell/decoupler_gpu/_method_mlm.py
--rw-r--r--   0        0        0     6349 2023-06-24 21:46:06.552057 rapids_singlecell-0.7.2/rapids_singlecell/decoupler_gpu/_method_wsum.py
--rw-r--r--   0        0        0       27 2023-06-24 21:46:06.552057 rapids_singlecell-0.7.2/rapids_singlecell/gr.py
--rw-r--r--   0        0        0       91 2023-06-24 21:46:06.552057 rapids_singlecell-0.7.2/rapids_singlecell/pl.py
--rw-r--r--   0        0        0       30 2023-06-24 21:46:06.552057 rapids_singlecell-0.7.2/rapids_singlecell/pp.py
--rw-r--r--   0        0        0      340 2023-06-24 21:46:06.552057 rapids_singlecell-0.7.2/rapids_singlecell/scanpy_gpu/__init__.py
--rw-r--r--   0        0        0     5680 2023-06-24 21:46:06.552057 rapids_singlecell-0.7.2/rapids_singlecell/scanpy_gpu/_clustering.py
--rw-r--r--   0        0        0     3429 2023-06-24 21:46:06.552057 rapids_singlecell-0.7.2/rapids_singlecell/scanpy_gpu/_diffmap.py
--rw-r--r--   0        0        0     4040 2023-06-24 21:46:06.552057 rapids_singlecell-0.7.2/rapids_singlecell/scanpy_gpu/_draw_graph.py
--rw-r--r--   0        0        0     5154 2023-06-24 21:46:06.552057 rapids_singlecell-0.7.2/rapids_singlecell/scanpy_gpu/_embedding_density.py
--rw-r--r--   0        0        0    12177 2023-06-24 21:46:06.552057 rapids_singlecell-0.7.2/rapids_singlecell/scanpy_gpu/_harmonpy_gpu.py
--rw-r--r--   0        0        0     1729 2023-06-24 21:46:06.552057 rapids_singlecell-0.7.2/rapids_singlecell/scanpy_gpu/_harmony_integrate.py
--rw-r--r--   0        0        0     2425 2023-06-24 21:46:06.552057 rapids_singlecell-0.7.2/rapids_singlecell/scanpy_gpu/_pymde.py
--rw-r--r--   0        0        0     7928 2023-06-24 21:46:06.552057 rapids_singlecell-0.7.2/rapids_singlecell/scanpy_gpu/_rank_gene_groups.py
--rw-r--r--   0        0        0     3241 2023-06-24 21:46:06.552057 rapids_singlecell-0.7.2/rapids_singlecell/scanpy_gpu/_tsne.py
--rw-r--r--   0        0        0       68 2023-06-24 21:46:06.552057 rapids_singlecell-0.7.2/rapids_singlecell/squidpy_gpu/__init__.py
--rw-r--r--   0        0        0     6012 2023-06-24 21:46:06.552057 rapids_singlecell-0.7.2/rapids_singlecell/squidpy_gpu/_autocorr.py
--rw-r--r--   0        0        0     6467 2023-06-24 21:46:06.552057 rapids_singlecell-0.7.2/rapids_singlecell/squidpy_gpu/_gearysc.py
--rw-r--r--   0        0        0    29539 2023-06-24 21:46:06.556057 rapids_singlecell-0.7.2/rapids_singlecell/squidpy_gpu/_ligrec.py
--rw-r--r--   0        0        0     6325 2023-06-24 21:46:06.556057 rapids_singlecell-0.7.2/rapids_singlecell/squidpy_gpu/_moransi.py
--rw-r--r--   0        0        0     6227 2023-06-24 21:46:06.556057 rapids_singlecell-0.7.2/rapids_singlecell/squidpy_gpu/_utils.py
--rw-r--r--   0        0        0       26 2023-06-24 21:46:06.560057 rapids_singlecell-0.7.2/rapids_singlecell/tl.py
--rw-r--r--   0        0        0     6794 1970-01-01 00:00:00.000000 rapids_singlecell-0.7.2/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-08-04 12:29:40.898790 rapids_singlecell-0.7.5/LICENSE
+-rw-r--r--   0        0        0     4066 2023-08-04 12:29:40.898790 rapids_singlecell-0.7.5/README.md
+-rw-r--r--   0        0        0     2217 2023-08-04 12:29:41.158795 rapids_singlecell-0.7.5/pyproject.toml
+-rwxr-xr-x   0        0        0       67 2023-08-04 12:29:41.158795 rapids_singlecell-0.7.5/rapids_singlecell/__init__.py
+-rw-r--r--   0        0        0    25070 2023-08-04 12:29:41.158795 rapids_singlecell-0.7.5/rapids_singlecell/cunnData/__init__.py
+-rw-r--r--   0        0        0      339 2023-08-04 12:29:41.158795 rapids_singlecell-0.7.5/rapids_singlecell/cunnData_funcs/__init__.py
+-rw-r--r--   0        0        0    36761 2023-08-04 12:29:41.158795 rapids_singlecell-0.7.5/rapids_singlecell/cunnData_funcs/_hvg.py
+-rw-r--r--   0        0        0    14597 2023-08-04 12:29:41.158795 rapids_singlecell-0.7.5/rapids_singlecell/cunnData_funcs/_normalize.py
+-rw-r--r--   0        0        0    11457 2023-08-04 12:29:41.158795 rapids_singlecell-0.7.5/rapids_singlecell/cunnData_funcs/_pca.py
+-rw-r--r--   0        0        0     2754 2023-08-04 12:29:41.158795 rapids_singlecell-0.7.5/rapids_singlecell/cunnData_funcs/_plotting.py
+-rw-r--r--   0        0        0     4758 2023-08-04 12:29:41.158795 rapids_singlecell-0.7.5/rapids_singlecell/cunnData_funcs/_regress_out.py
+-rw-r--r--   0        0        0     1477 2023-08-04 12:29:41.158795 rapids_singlecell-0.7.5/rapids_singlecell/cunnData_funcs/_scale.py
+-rw-r--r--   0        0        0    18244 2023-08-04 12:29:41.158795 rapids_singlecell-0.7.5/rapids_singlecell/cunnData_funcs/_simple.py
+-rw-r--r--   0        0        0     3352 2023-08-04 12:29:41.158795 rapids_singlecell-0.7.5/rapids_singlecell/cunnData_funcs/_utils.py
+-rw-r--r--   0        0        0       29 2023-08-04 12:29:41.158795 rapids_singlecell-0.7.5/rapids_singlecell/dcg.py
+-rw-r--r--   0        0        0       68 2023-08-04 12:29:41.158795 rapids_singlecell-0.7.5/rapids_singlecell/decoupler_gpu/__init__.py
+-rw-r--r--   0        0        0     4581 2023-08-04 12:29:41.158795 rapids_singlecell-0.7.5/rapids_singlecell/decoupler_gpu/_method_mlm.py
+-rw-r--r--   0        0        0     6334 2023-08-04 12:29:41.158795 rapids_singlecell-0.7.5/rapids_singlecell/decoupler_gpu/_method_wsum.py
+-rw-r--r--   0        0        0       27 2023-08-04 12:29:41.158795 rapids_singlecell-0.7.5/rapids_singlecell/gr.py
+-rw-r--r--   0        0        0       40 2023-08-04 12:29:41.158795 rapids_singlecell-0.7.5/rapids_singlecell/pl.py
+-rw-r--r--   0        0        0       30 2023-08-04 12:29:41.158795 rapids_singlecell-0.7.5/rapids_singlecell/pp.py
+-rw-r--r--   0        0        0      357 2023-08-04 12:29:41.158795 rapids_singlecell-0.7.5/rapids_singlecell/scanpy_gpu/__init__.py
+-rw-r--r--   0        0        0     5644 2023-08-04 12:29:41.158795 rapids_singlecell-0.7.5/rapids_singlecell/scanpy_gpu/_clustering.py
+-rw-r--r--   0        0        0     3425 2023-08-04 12:29:41.158795 rapids_singlecell-0.7.5/rapids_singlecell/scanpy_gpu/_diffmap.py
+-rw-r--r--   0        0        0     4039 2023-08-04 12:29:41.158795 rapids_singlecell-0.7.5/rapids_singlecell/scanpy_gpu/_draw_graph.py
+-rw-r--r--   0        0        0     5166 2023-08-04 12:29:41.158795 rapids_singlecell-0.7.5/rapids_singlecell/scanpy_gpu/_embedding_density.py
+-rw-r--r--   0        0        0    12158 2023-08-04 12:29:41.158795 rapids_singlecell-0.7.5/rapids_singlecell/scanpy_gpu/_harmonpy_gpu.py
+-rw-r--r--   0        0        0     1729 2023-08-04 12:29:41.158795 rapids_singlecell-0.7.5/rapids_singlecell/scanpy_gpu/_harmony_integrate.py
+-rw-r--r--   0        0        0     2440 2023-08-04 12:29:41.158795 rapids_singlecell-0.7.5/rapids_singlecell/scanpy_gpu/_pymde.py
+-rw-r--r--   0        0        0     7921 2023-08-04 12:29:41.158795 rapids_singlecell-0.7.5/rapids_singlecell/scanpy_gpu/_rank_gene_groups.py
+-rw-r--r--   0        0        0     3214 2023-08-04 12:29:41.158795 rapids_singlecell-0.7.5/rapids_singlecell/scanpy_gpu/_tsne.py
+-rw-r--r--   0        0        0       68 2023-08-04 12:29:41.158795 rapids_singlecell-0.7.5/rapids_singlecell/squidpy_gpu/__init__.py
+-rw-r--r--   0        0        0     5994 2023-08-04 12:29:41.158795 rapids_singlecell-0.7.5/rapids_singlecell/squidpy_gpu/_autocorr.py
+-rw-r--r--   0        0        0     6467 2023-08-04 12:29:41.158795 rapids_singlecell-0.7.5/rapids_singlecell/squidpy_gpu/_gearysc.py
+-rw-r--r--   0        0        0    29549 2023-08-04 12:29:41.158795 rapids_singlecell-0.7.5/rapids_singlecell/squidpy_gpu/_ligrec.py
+-rw-r--r--   0        0        0     6326 2023-08-04 12:29:41.158795 rapids_singlecell-0.7.5/rapids_singlecell/squidpy_gpu/_moransi.py
+-rw-r--r--   0        0        0     6230 2023-08-04 12:29:41.158795 rapids_singlecell-0.7.5/rapids_singlecell/squidpy_gpu/_utils.py
+-rw-r--r--   0        0        0       26 2023-08-04 12:29:41.162795 rapids_singlecell-0.7.5/rapids_singlecell/tl.py
+-rw-r--r--   0        0        0     5342 1970-01-01 00:00:00.000000 rapids_singlecell-0.7.5/PKG-INFO
```

### Comparing `rapids_singlecell-0.7.2/LICENSE` & `rapids_singlecell-0.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.7.2/rapids_singlecell/cunnData/__init__.py` & `rapids_singlecell-0.7.5/rapids_singlecell/cunnData/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,38 +1,35 @@
+import warnings
+from collections import OrderedDict
+from itertools import repeat
+from typing import Any, List, Mapping, MutableMapping, Optional, Union
+
+import anndata
 import cupy as cp
 import cupyx as cpx
-from anndata import AnnData
-from anndata._core.index import _normalize_indices
-import anndata
-
 import numpy as np
 import pandas as pd
-from scipy import sparse
-from collections import OrderedDict
-from typing import Any, Union, Optional, Mapping, MutableMapping, List
-from pandas.api.types import infer_dtype, is_string_dtype
-from itertools import repeat
-import warnings
-
+from anndata import AnnData
+from anndata._core.index import _normalize_indices
+from cupyx.scipy.sparse import issparse as issparse_gpu
 from natsort import natsorted
-
+from pandas.api.types import infer_dtype, is_string_dtype
+from scipy import sparse
 from scipy.sparse import issparse as issparse_cpu
-from cupyx.scipy.sparse import issparse as issparse_gpu
 
 
 class Layer_Mapping(dict):
-    """
-    Dictonary subclass for layers handeling in cunnData
-    """
+    """Dictonary subclass for layers handeling in cunnData"""
 
     def __init__(self, shape=None):
         super().__init__({})
         self.shape = shape
 
     def update_shape(self, shape):
+        """Updates Shape for Layers"""
         self.shape = shape
 
     def __setitem__(self, key, item):
         if self.shape == item.shape:
             if issparse_gpu(item):
                 item = item.astype(cp.float32)
             elif isinstance(item, cp.ndarray):
@@ -47,61 +44,60 @@
                     raise ValueError(
                         "Cupy only supports Sparse Matrices with `.nnz`"
                         "with less than 2**31-1 for the int32 indptr"
                     )
             super().__setitem__(key, item)
         else:
             raise ValueError(
-                f"Shape of {key} {item.shape} does not match :attr:`.X` {self.shape}"
+                f"Shape of {key} {item.shape} does not match `.X` {self.shape}"
             )
 
 
 class obsm_Mapping(dict):
-    """
-    Dictonary subclass for obsm handeling in cunnData
-    """
+    """Dictonary subclass for obsm handeling in cunnData"""
 
     def __init__(self, shape=None):
         super().__init__({})
         self.shape = shape
 
     def update_shape(self, shape):
+        """Updates Shape for obsm"""
         self.shape = shape
 
     def __setitem__(self, key, item):
         if self.shape == item.shape[0]:
             super().__setitem__(key, item)
         else:
-            raise ValueError(f"Shape of {key} does not match :attr:`.n_obs`")
+            raise ValueError(f"Shape of {key} does not match `.n_obs`")
 
 
 class varm_Mapping(dict):
-    """
-    Dictonary subclass for obsm handeling in cunnData
-    """
+    """Dictonary subclass for obsm handeling in cunnData"""
 
     def __init__(self, shape=None):
         super().__init__({})
         self.shape = shape
 
     def update_shape(self, shape):
+        """Updates Shape for varm"""
         self.shape = shape
 
     def __setitem__(self, key, item):
         if self.shape == item.shape[0]:
             super().__setitem__(key, item)
         else:
-            raise ValueError(f"Shape of {key} does not match :attr:`.n_vars`")
+            raise ValueError(f"Shape of {key} does not match `.n_vars`")
 
 
 class cunnData:
-    """
+    """\
     The cunnData objects can be used as an AnnData replacement for the inital preprocessing
     of single cell Datasets. It replaces some of the most common preprocessing steps within
     scanpy for annData objects.
+
     It can be initalized with a preexisting annData object or with a countmatrix and seperate
     Dataframes for var and obs. Index of var will be used as gene_names. Initalization with an
     AnnData object is advised.
     """
 
     def __init__(
         self,
@@ -306,16 +302,17 @@
 
     @uns.deleter
     def uns(self):
         self.uns = OrderedDict()
 
     @property
     def layers(self):
-        """\
+        """
         Dictionary-like object with values of the same dimensions as :attr:`.X`.
+
         Layers in cunnData are inspired by AnnData.
 
         Return the layer named `"unspliced"`::
             adata.layers["unspliced"]
         Create or replace the `"spliced"` layer::
             adata.layers["spliced"] = ...
         Assign the 10th column of layer `"spliced"` to the variable a::
@@ -325,28 +322,30 @@
         Return layers’ names::
             adata.layers.keys()
         """
         return self._layers
 
     @property
     def obsm(self):
-        """\
+        """
         Multi-dimensional annotation of observations
         (mutable structured :class:`~numpy.ndarray`).
+
         Stores for each key a two or higher-dimensional :class:`~numpy.ndarray`
         of length :attr:`n_obs`.
         Is sliced with `data` and `obs` but behaves otherwise like a :term:`mapping`.
         """
         return self._obsm
 
     @property
     def varm(self):
         """\
         Multi-dimensional annotation of variables/features
         (mutable structured :class:`~numpy.ndarray`).
+
         Stores for each key a two or higher-dimensional :class:`~numpy.ndarray`
         of length :attr:`n_vars`.
         Is sliced with `data` and `var` but behaves otherwise like a :term:`mapping`.
         """
         return self._varm
 
     @property
@@ -528,30 +527,30 @@
             return self.layers[layer]
         else:
             return self.X
 
     def obs_vector(self, k: str, *, layer: Optional[str] = None):
         """\
         Convenience function for returning a 1 dimensional ndarray of values
-        from :attr:`X`, :attr:`layers`\\ `[k]`, or :attr:`obs`.
+        from :attr:`.X`, :attr:`.layers`\\ `[k]`, or :attr:`.obs`.
 
         Made for convenience, not performance.
         Intentionally permissive about arguments, for easy iterative use.
 
         Params
         ------
         k
-            Key to use. Should be in :attr:`var_names` or :attr:`obs`\\ `.columns`.
+            Key to use. Should be in :attr:`.var_names` or :attr:`.obs`\\ `.columns`.
         layer
-            What layer values should be returned from. If `None`, :attr:`X` is used.
+            What layer values should be returned from. If `None`, :attr:`.X` is used.
 
         Returns
         -------
         A one dimensional nd array, with values for each obs in the same order
-        as :attr:`obs_names`.
+        as :attr:`.obs_names`.
         """
         if layer == "X":
             if "X" in self.layers:
                 pass
             else:
                 warnings.warn(
                     "In a future version of AnnData, access to `.X` by passing"
@@ -560,30 +559,30 @@
                 )
                 layer = None
         return _get_vector(self, k, "obs", "var", layer=layer)
 
     def var_vector(self, k, *, layer: Optional[str] = None):
         """\
         Convenience function for returning a 1 dimensional ndarray of values
-        from :attr:`X`, :attr:`layers`\\ `[k]`, or :attr:`var`.
+        from :attr:`.X`, :attr:`.layers`\\ `[k]`, or :attr:`.var`.
 
         Made for convenience, not performance. Intentionally permissive about
         arguments, for easy iterative use.
 
         Params
         ------
         k
-            Key to use. Should be in :attr:`obs_names` or :attr:`var`\\ `.columns`.
+            Key to use. Should be in :attr:`.obs_names` or :attr:`.var`\\ `.columns`.
         layer
-            What layer values should be returned from. If `None`, :attr:`X` is used.
+            What layer values should be returned from. If `None`, :attr:`.X` is used.
 
         Returns
         -------
         A one dimensional nd array, with values for each var in the same order
-        as :attr:`var_names`.
+        as :attr:`.var_names`.
         """
         if layer == "X":
             if "X" in self.layers:
                 pass
             else:
                 warnings.warn(
                     "In a future version of AnnData, access to `.X` by passing "
@@ -593,32 +592,32 @@
                 layer = None
         return _get_vector(self, k, "var", "obs", layer=layer)
 
     def __repr__(self) -> str:
         return self._gen_repr(self.n_obs, self.n_vars)
 
     def obs_keys(self) -> List[str]:
-        """List keys of observation annotation :attr:`obs`."""
+        """List keys of observation annotation :attr:`.obs`."""
         return self._obs.keys().tolist()
 
     def var_keys(self) -> List[str]:
-        """List keys of variable annotation :attr:`var`."""
+        """List keys of variable annotation :attr:`.var`."""
         return self._var.keys().tolist()
 
     def obsm_keys(self) -> List[str]:
-        """List keys of observation annotation :attr:`obsm`."""
+        """List keys of observation annotation :attr:`.obsm`."""
         return list(self._obsm.keys())
 
     def varm_keys(self) -> List[str]:
-        """List keys of variable annotation :attr:`varm`."""
+        """List keys of variable annotation :attr:`.varm`."""
         return list(self._varm.keys())
 
     def uns_keys(self) -> List[str]:
         """List keys of unstructured annotation."""
-        return sorted(list(self._uns.keys()))
+        return sorted(self._uns.keys())
 
     def to_AnnData(self):
         """
         Takes the cunnData object and creates an AnnData object
 
         Returns
         -------
```

### Comparing `rapids_singlecell-0.7.2/rapids_singlecell/cunnData_funcs/_hvg.py` & `rapids_singlecell-0.7.5/rapids_singlecell/cunnData_funcs/_hvg.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-import cupy as cp
-import cupyx as cpx
-import numpy as np
-import pandas as pd
 import math
 import warnings
 from typing import Optional
 
-from ..cunnData import cunnData
+import cupy as cp
+import numpy as np
+import pandas as pd
+
+from rapids_singlecell.cunnData import cunnData
+
 from ._utils import _check_nonnegative_integers, _get_mean_var
 
 
 def highly_variable_genes(
     cudata: cunnData,
     layer: str = None,
     min_mean: float = 0.0125,
@@ -199,23 +200,23 @@
                 idxs = np.concatenate((thr, thr_2))
                 hvg = hvg.loc[np.argsort(idxs)]
                 df.append(hvg)
 
             df = pd.concat(df, axis=0)
             df["highly_variable"] = df["highly_variable"].astype(int)
             df = df.groupby("gene").agg(
-                dict(
-                    means=np.nanmean,
-                    dispersions=np.nanmean,
-                    dispersions_norm=np.nanmean,
-                    highly_variable=np.nansum,
-                )
+                {
+                    "means": np.nanmean,
+                    "dispersions": np.nanmean,
+                    "dispersions_norm": np.nanmean,
+                    "highly_variable": np.nansum,
+                }
             )
             df.rename(
-                columns=dict(highly_variable="highly_variable_nbatches"), inplace=True
+                columns={"highly_variable": "highly_variable_nbatches"}, inplace=True
             )
             df["highly_variable_intersection"] = df["highly_variable_nbatches"] == len(
                 batches
             )
             if n_top_genes is not None:
                 # sort genes by how often they selected as hvg within each batch and
                 # break ties with normalized dispersion across batches
@@ -265,19 +266,20 @@
     max_disp=np.inf,
     n_top_genes=None,
     flavor="seurat",
     n_bins=20,
 ):
     """\
         See `highly_variable_genes`.
-        Returns
-        -------
-        A DataFrame that contains the columns
-        `highly_variable`, `means`, `dispersions`, and `dispersions_norm`.
-        """
+
+    Returns
+    -------
+    A DataFrame that contains the columns
+    `highly_variable`, `means`, `dispersions`, and `dispersions_norm`.
+    """
     if flavor == "seurat":
         X = X.expm1()
     mean, var = _get_mean_var(X, axis=1)
     mean[mean == 0] = 1e-12
     disp = var / mean
     if flavor == "seurat":  # logarithmized mean as in Seurat
         disp[disp == 0] = np.nan
@@ -293,15 +295,15 @@
         disp_grouped = df.groupby("mean_bin")["dispersions"]
         disp_mean_bin = disp_grouped.mean()
         disp_std_bin = disp_grouped.std(ddof=1)
         # retrieve those genes that have nan std, these are the ones where
         # only a single gene fell in the bin and implicitly set them to have
         # a normalized disperion of 1
         one_gene_per_bin = disp_std_bin.isnull()
-        gen_indices = np.where(one_gene_per_bin[df["mean_bin"].values])[0].tolist()
+        np.where(one_gene_per_bin[df["mean_bin"].values])[0].tolist()
 
         # Circumvent pandas 0.23 bug. Both sides of the assignment have dtype==float32,
         # but there’s still a dtype error without “.value”.
         disp_std_bin[one_gene_per_bin.values] = disp_mean_bin[
             one_gene_per_bin.values
         ].values
         disp_mean_bin[one_gene_per_bin.values] = 0
@@ -364,14 +366,15 @@
     batch_key: Optional[str] = None,
     span: float = 0.3,
     check_values=True,
 ):
     """\
     See `highly_variable_genes`.
     For further implementation details see https://www.overleaf.com/read/ckptrbgzzzpg
+
     Returns
     -------
     updates `.var` with the following fields:
     highly_variable : bool
         boolean indicator of highly-variable genes.
     **means**
         means per gene.
@@ -659,22 +662,22 @@
     ranks_residual_var = ranks_residual_var.get()
     ranks_masked_array = np.ma.masked_invalid(ranks_residual_var)
     # Median rank across batches, ignoring batches in which gene was not selected
     medianrank_residual_var = np.ma.median(ranks_masked_array, axis=0).filled(np.nan)
     means, variances = _get_mean_var(X, axis=1)
     means, variances = means.get(), variances.get()
     df = pd.DataFrame.from_dict(
-        dict(
-            means=means,
-            variances=variances,
-            residual_variances=cp.mean(residual_gene_vars, axis=0).get(),
-            highly_variable_rank=medianrank_residual_var,
-            highly_variable_nbatches=highly_variable_nbatches.astype(np.int64),
-            highly_variable_intersection=highly_variable_nbatches == n_batches,
-        )
+        {
+            "means": means,
+            "variances": variances,
+            "residual_variances": cp.mean(residual_gene_vars, axis=0).get(),
+            "highly_variable_rank": medianrank_residual_var,
+            "highly_variable_nbatches": highly_variable_nbatches.astype(np.int64),
+            "highly_variable_intersection": highly_variable_nbatches == n_batches,
+        }
     )
     df = df.set_index(cudata.var_names)
     df.sort_values(
         ["highly_variable_nbatches", "highly_variable_rank"],
         ascending=[False, True],
         na_position="last",
         inplace=True,
@@ -711,14 +714,15 @@
     """
     Rank and select genes based on the enrichment of zero counts.
     Enrichment is considered by comparing data to a Poisson count model.
     This is based on M3Drop: https://github.com/tallulandrews/M3Drop
     The method accounts for library size internally, a raw count matrix should be provided.
     Instead of Z-test, enrichment of zeros is quantified by posterior
     probabilites from a binomial model, computed through sampling.
+
     Parameters
     ----------
     cudata
         cunnData object (with sparse X matrix).
     layer
         If provided, use `adata.layers[layer]` for expression values instead of `adata.X`.
     n_top_genes
@@ -729,14 +733,15 @@
     batch_key
         key in adata.obs that contains batch info. If None, do not use batch info.
         Defatult: ``None``.
     minibatch_size
         Size of temporary matrix for incremental calculation. Larger is faster but
         requires more RAM or GPU memory. (The default should be fine unless
         there are hundreds of millions cells or millions of genes.)
+
     Returns
     -------
     Depending on `inplace` returns calculated metrics (:class:`~pd.DataFrame`) or
     updates `.var` with the following fields
     highly_variable : bool
         boolean indicator of highly-variable genes
     **observed_fraction_zeros**
@@ -746,15 +751,14 @@
     prob_zero_enrichment : float
         Probability of zero enrichment, median across batches in the case of multiple batches
     prob_zero_enrichment_rank : float
         Rank of the gene according to probability of zero enrichment, median rank in the case of multiple batches
     prob_zero_enriched_nbatches : int
         If batch_key is given, this denotes in how many batches genes are detected as zero enriched
     """
-
     try:
         import torch
     except ImportError:
         raise ImportError("Please install pytorch package via `pip install pytorch")
     if n_top_genes is None:
         n_top_genes = 2000
         warnings.warn(
```

### Comparing `rapids_singlecell-0.7.2/rapids_singlecell/cunnData_funcs/_normalize.py` & `rapids_singlecell-0.7.5/rapids_singlecell/cunnData_funcs/_normalize.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,16 @@
-import cupy as cp
-import cupyx as cpx
 import math
 import warnings
 from typing import Optional
 
-from ..cunnData import cunnData
+import cupy as cp
+import cupyx as cpx
+
+from rapids_singlecell.cunnData import cunnData
+
 from ._utils import _check_nonnegative_integers
 
 
 def normalize_total(
     cudata: cunnData, target_sum: int, layer: Optional[str] = None, inplace: bool = True
 ) -> Optional[cpx.scipy.sparse.csr_matrix]:
     """
@@ -96,15 +98,15 @@
         layer
             Layer to normalize instead of `X`. If `None`, `X` is normalized.
 
         copy
             Whether to return a copy or update `cudata`.
 
     Returns
-    ----------
+    -------
             The resulting sparse matrix after applying the natural logarithm of one plus the input matrix. \
             If `copy` is set to True, returns the new sparse matrix. Otherwise, updates the `cudata` object \
             in-place and returns None.
 
     """
     X = cudata.layers[layer] if layer is not None else cudata.X
     X = X.log1p()
@@ -306,29 +308,28 @@
             and return a warning if non-integers are found. Otherwise, proceed without checking. Setting this to False can speed up code for large datasets.
         layer
             Layer to use as input instead of X. If None, X is used.
         inplace
             If True, update cunnData with results. Otherwise, return results. See below for details of what is returned.
 
     Returns
-    ----------
+    -------
         If `inplace=True`, `cudata.X` or the selected layer in `cudata.layers` is updated with the normalized values. \
         If `inplace=False` the normalized matrix is returned.
 
     """
-
     X = cudata.layers[layer] if layer is not None else cudata.X
 
     if check_values and not _check_nonnegative_integers(X):
         warnings.warn(
             "`flavor='pearson_residuals'` expects raw count data, but non-integers were found.",
             UserWarning,
         )
     computed_on = layer if layer else "cudata.X"
-    settings_dict = dict(theta=theta, clip=clip, computed_on=computed_on)
+    settings_dict = {"theta": theta, "clip": clip, "computed_on": computed_on}
     if theta <= 0:
         raise ValueError("Pearson residuals require theta > 0")
     if clip is None:
         n = X.shape[0]
         clip = cp.sqrt(n, dtype=cp.float32)
     if clip < 0:
         raise ValueError("Pearson residuals require `clip>=0` or `clip=None`.")
@@ -420,15 +421,15 @@
                 clip,
                 theta,
                 residuals.shape[0],
                 residuals.shape[1],
             ),
         )
 
-    if inplace == True:
+    if inplace is True:
         cudata.uns["pearson_residuals_normalization"] = settings_dict
         if layer:
             cudata.layers[layer] = residuals
         else:
             cudata.X = residuals
     else:
         return residuals
```

### Comparing `rapids_singlecell-0.7.2/rapids_singlecell/cunnData_funcs/_plotting.py` & `rapids_singlecell-0.7.5/rapids_singlecell/cunnData_funcs/_plotting.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,13 @@
-from ..cunnData import cunnData
+import os
 
-import numpy as np
-import pandas as pd
-import seaborn as sns
 import matplotlib.pyplot as plt
-import os
+import seaborn as sns
+
+from rapids_singlecell.cunnData import cunnData
 
 
 def scatter(
     cudata: cunnData,
     x: str,
     y: str,
     color: str = None,
@@ -17,15 +16,15 @@
     dpi: int = 300,
 ) -> None:
     """
     Violin plot.
     Wraps :func:`seaborn.scatterplot` for :class:`~rapids_singlecell.cunnData.cunnData`. This plotting function so far is really basic and doesnt include all the features form :func:`scanpy.pl.scatter`.
 
     Parameters
-    ---------
+    ----------
     cudata
         cunnData object
     x
         Keys for accessing variables of fields of `.obs`.
     y
         Keys for accessing variables of fields of `.obs`.
     save
@@ -34,15 +33,15 @@
         if you want to display the plot
     dpi
         The resolution in dots per inch for save
 
 
     """
     fig, ax = plt.subplots()
-    if color == None:
+    if color is None:
         sns.scatterplot(data=cudata.obs, x=x, y=y, s=2, color="grey", edgecolor="grey")
     else:
         sns.scatterplot(data=cudata.obs, x=x, y=y, s=2, hue=color)
 
     if save:
         os.makedirs("./figures/", exist_ok=True)
         fig_path = "./figures/" + save
@@ -61,15 +60,15 @@
     dpi: int = 300,
 ):
     """
     Violin plot.
     Wraps :func:`seaborn.violinplot` for :class:`~rapids_singlecell.cunnData.cunnData`. This plotting function so far is really basic and doesnt include all the features form :func:`scanpy.pl.violin`.
 
     Parameters
-    ---------
+    ----------
         cudata
             cunnData object
         key
             Keys for accessing variables of fields of `.obs`.
         groupby
             The key of the observation grouping to consider.(e.g batches)
         size
@@ -78,22 +77,22 @@
             file name to save plot as in ./figures
         show
             if you want to display the plot
         dpi
             The resolution in dots per inch for save
 
     Returns
-    ------
+    -------
     nothing
 
     """
     fig, ax = plt.subplots()
-    ax = sns.violinplot(data=cudata.obs, y=key, scale="width", x=groupby, inner=None)
+    sns.violinplot(data=cudata.obs, y=key, scale="width", x=groupby, inner=None)
     if size:
-        ax = sns.stripplot(
+        sns.stripplot(
             data=cudata.obs,
             y=key,
             x=groupby,
             color="k",
             size=size,
             dodge=True,
             jitter=True,
```

### Comparing `rapids_singlecell-0.7.2/rapids_singlecell/cunnData_funcs/_regress_out.py` & `rapids_singlecell-0.7.5/rapids_singlecell/cunnData_funcs/_regress_out.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
+import math
+from typing import Literal, Optional, Union
+
 import cupy as cp
 import cupyx as cpx
 from cuml.linear_model import LinearRegression
+
 from rapids_singlecell.cunnData import cunnData
-from typing import Literal, Union, Optional
-from ..cunnData import cunnData
-import math
 
 
 def regress_out(
     cudata: cunnData,
     keys: Union[str, list],
     layer: Optional[str] = None,
     inplace: bool = True,
@@ -43,28 +44,27 @@
             Print debugging information
 
     Returns
     -------
     Returns a corrected copy or  updates `cudata` with a corrected version of the \
     original `cudata.X` and `cudata.layers['layer']`, depending on `inplace`.
     """
-
     if batchsize != "all" and type(batchsize) not in [int, type(None)]:
         raise ValueError("batchsize must be `int`, `None` or `'all'`")
 
     X = cudata.layers[layer] if layer is not None else cudata.X
 
     if cpx.scipy.sparse.issparse(X) and not cpx.scipy.sparse.isspmatrix_csc(X):
         X = X.tocsc()
 
     dim_regressor = 2
     if type(keys) is list:
         dim_regressor = len(keys) + 1
 
-    regressors = cp.ones((X.shape[0] * dim_regressor)).reshape(
+    regressors = cp.ones(X.shape[0] * dim_regressor).reshape(
         (X.shape[0], dim_regressor), order="F"
     )
     if dim_regressor == 2:
         regressors[:, 1] = cp.array(cudata.obs[keys]).ravel()
     else:
         for i in range(dim_regressor - 1):
             regressors[:, i + 1] = cp.array(cudata.obs[keys[i]]).ravel()
@@ -99,15 +99,15 @@
                 lr.fit(regressors, arr_batch, convert_dtype=True)
                 outputs[:, start_idx:stop_idx] = arr_batch - lr.predict(regressors)
     else:
         if X.shape[0] < 100000 and cpx.scipy.sparse.issparse(X):
             X = X.todense()
         for i in range(X.shape[1]):
             if verbose and i % 500 == 0:
-                print("Regressed %s out of %s" % (i, X.shape[1]))
+                print(f"Regressed {i} out of {X.shape[1]}")
 
             y = X[:, i]
             outputs[:, i] = _regress_out_chunk(regressors, y)
 
     if inplace:
         if layer:
             cudata.layers[layer] = outputs
@@ -117,20 +117,22 @@
         return outputs
 
 
 def _regress_out_chunk(X, y):
     """
     Performs a data_cunk.shape[1] number of local linear regressions,
     replacing the data in the original chunk w/ the regressed result.
+
     Parameters
     ----------
     X : cupy.ndarray of shape (n_cells, 3)
         Matrix of regressors
     y : cupy.sparse.spmatrix of shape (n_cells,)
         Sparse matrix containing a single column of the cellxgene matrix
+
     Returns
     -------
     dense_mat : cupy.ndarray of shape (n_cells,)
         Adjusted column
     """
     if cpx.scipy.sparse.issparse(y):
         y = y.todense()
```

### Comparing `rapids_singlecell-0.7.2/rapids_singlecell/cunnData_funcs/_scale.py` & `rapids_singlecell-0.7.5/rapids_singlecell/cunnData_funcs/_scale.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,13 @@
-import cupy as cp
-from ..cunnData import cunnData
 from typing import Optional
 
+import cupy as cp
+
+from rapids_singlecell.cunnData import cunnData
+
 
 def scale(
     cudata: cunnData,
     max_value: Optional[int] = None,
     layer: Optional[str] = None,
     inplace: bool = True,
 ) -> Optional[cp.ndarray]:
```

### Comparing `rapids_singlecell-0.7.2/rapids_singlecell/cunnData_funcs/_simple.py` & `rapids_singlecell-0.7.5/rapids_singlecell/cunnData_funcs/_simple.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
+import math
+from typing import Union
+
 import cupy as cp
 import cupyx as cpx
-import math
 import numpy as np
-import pandas as pd
-import math
-from ..cunnData import cunnData
-from typing import Union
+
+from rapids_singlecell.cunnData import cunnData
 
 _sparse_qc_kernel_csc = cp.RawKernel(
     r"""
     extern "C" __global__
     void caluclate_qc_csc(const int *indptr,const int *index,const float *data,
                                         float* sums_cells, float* sums_genes,
                                         int* cell_ex, int* gene_ex,
@@ -209,15 +209,14 @@
                 E.g. 'n_cells_by_counts'. Number of cells this expression is measured in.
             `mean_{expr_type}`
                 E.g. "mean_counts". Mean expression over all cells.
             `pct_dropout_by_{expr_type}`
                 E.g. 'pct_dropout_by_counts'. Percentage of cells this feature does not appear in.
 
     """
-
     X = cudata.X
     sums_cells = cp.zeros(X.shape[0], dtype=cp.float32)
     sums_genes = cp.zeros(X.shape[1], dtype=cp.float32)
     cell_ex = cp.zeros(X.shape[0], dtype=cp.int32)
     gene_ex = cp.zeros(X.shape[1], dtype=cp.int32)
     if cpx.scipy.sparse.issparse(X):
         if cpx.scipy.sparse.isspmatrix_csr(X):
@@ -400,15 +399,14 @@
             Print number of discarded genes
 
     Returns
     -------
         a filtered :class:`~rapids_singlecell.cunnData.cunnData` object inplace
 
     """
-
     if qc_var in cudata.var.keys():
         if min_count is not None and max_count is not None:
             thr = np.where(
                 (cudata.var[qc_var] <= max_count) & (min_count <= cudata.var[qc_var])
             )[0]
         elif min_count is not None:
             thr = np.where(cudata.var[qc_var] >= min_count)[0]
@@ -425,15 +423,15 @@
     elif qc_var in [
         "n_cells_by_counts",
         "total_counts",
         "mean_counts",
         "pct_dropout_by_counts",
     ]:
         print(
-            f"Running `calculate_qc_metrics` for 'n_cells_by_counts','total_counts','mean_counts' or 'pct_dropout_by_counts'"
+            "Running `calculate_qc_metrics` for 'n_cells_by_counts','total_counts','mean_counts' or 'pct_dropout_by_counts'"
         )
         calculate_qc_metrics(cudata=cudata, log1p=False)
         if min_count is not None and max_count is not None:
             thr = np.where(
                 (cudata.var[qc_var] <= max_count) & (min_count <= cudata.var[qc_var])
             )[0]
         elif min_count is not None:
@@ -444,15 +442,15 @@
         if verbose:
             print(
                 f"filtered out {cudata.var.shape[0]-thr.shape[0]} genes based on {qc_var}"
             )
 
         cudata._inplace_subset_var(thr)
     else:
-        print(f"please check qc_var")
+        print("please check qc_var")
 
 
 def filter_cells(
     cudata: cunnData,
     qc_var: str,
     min_count: float = None,
     max_count: float = None,
@@ -489,48 +487,48 @@
                 (cudata.obs[qc_var] < max_count) & (min_count < cudata.obs[qc_var])
             )[0]
         elif min_count is not None:
             inter = np.where(cudata.obs[qc_var] > min_count)[0]
         elif max_count is not None:
             inter = np.where(cudata.obs[qc_var] < max_count)[0]
         else:
-            print(f"Please specify a cutoff to filter against")
+            print("Please specify a cutoff to filter against")
         if verbose:
             print(f"filtered out {cudata.obs.shape[0]-inter.shape[0]} cells")
         cudata._inplace_subset_obs(inter)
     elif qc_var in ["n_genes_by_counts", "total_counts"]:
         print(
-            f"Running `calculate_qc_metrics` for 'n_cells_by_counts' or 'total_counts'"
+            "Running `calculate_qc_metrics` for 'n_cells_by_counts' or 'total_counts'"
         )
         calculate_qc_metrics(cudata, log1p=False)
         inter = np.array
         if min_count is not None and max_count is not None:
             inter = np.where(
                 (cudata.obs[qc_var] < max_count) & (min_count < cudata.obs[qc_var])
             )[0]
         elif min_count is not None:
             inter = np.where(cudata.obs[qc_var] > min_count)[0]
         elif max_count is not None:
             inter = np.where(cudata.obs[qc_var] < max_count)[0]
         else:
-            print(f"Please specify a cutoff to filter against")
+            print("Please specify a cutoff to filter against")
         if verbose:
             print(f"filtered out {cudata.obs.shape[0]-inter.shape[0]} cells")
         cudata._inplace_subset_obs(inter)
     else:
-        print(f"Please check qc_var.")
+        print("Please check qc_var.")
 
 
 def filter_highly_variable(cudata: cunnData) -> None:
     """
     Filters the :class:`~rapids_singlecell.cunnData.cunnData` object for highly_variable genes. Run highly_varible_genes first.
 
     Returns
     -------
         updates :class:`~rapids_singlecell.cunnData.cunnData` object to only contain highly variable genes.
 
     """
     if "highly_variable" in cudata.var.keys():
-        thr = np.where(cudata.var["highly_variable"] == True)[0]
+        thr = np.where(cudata.var["highly_variable"] is True)[0]
         cudata._inplace_subset_var(thr)
     else:
-        print(f"Please calculate highly variable genes first")
+        print("Please calculate highly variable genes first")
```

### Comparing `rapids_singlecell-0.7.2/rapids_singlecell/cunnData_funcs/_utils.py` & `rapids_singlecell-0.7.5/rapids_singlecell/cunnData_funcs/_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
+import math
+
 import cupy as cp
 import cupyx as cpx
 from cupyx.scipy.sparse import issparse
-import math
 
 _get_mean_var_major = cp.RawKernel(
     r"""
     extern "C" __global__
     void caluclate_meanvar_major(const int *indptr,const int *index,const float *data,
                         double* means,double* vars,
                         int major, int minor) {
```

### Comparing `rapids_singlecell-0.7.2/rapids_singlecell/decoupler_gpu/_method_mlm.py` & `rapids_singlecell-0.7.5/rapids_singlecell/decoupler_gpu/_method_mlm.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,22 @@
+from typing import Optional, Union
+
+import cupy as cp
 import numpy as np
 import pandas as pd
-import cupy as cp
-
-from decoupler.pre import extract, match, rename_net, get_net_mat, filt_min_n
-
 from anndata import AnnData
+from decoupler.pre import extract, filt_min_n, get_net_mat, match, rename_net
 from scipy import stats
-
 from tqdm import tqdm
-from typing import Union, Optional
 
 
 def fit_mlm(X, y, inv, df):
     X = cp.ascontiguousarray(X)
-    n_samples = y.shape[1]
-    n_fsets = X.shape[1]
+    y.shape[1]
+    X.shape[1]
     coef, sse, _, _ = cp.linalg.lstsq(X, y, rcond=-1)
     if len(sse) == 0:
         raise ValueError(
             """Couldn\'t fit a multivariate linear model. This can happen because there are more sources
         (covariates) than unique targets (samples), or because the network\'s matrix rank is smaller than the number of
         sources."""
         )
@@ -104,29 +102,28 @@
         Updates `adata` with the following fields.
 
             **estimate** : DataFrame
                 MLM scores. Stored in `.obsm['mlm_estimate']` if `mat` is AnnData.
             **pvals** : DataFrame
                 Obtained p-values. Stored in `.obsm['mlm_pvals']` if `mat` is AnnData.
     """
-
     # Extract sparse matrix and array of genes
     m, r, c = extract(mat, use_raw=use_raw, verbose=verbose)
 
     # Transform net
     net = rename_net(net, source=source, target=target, weight=weight)
     net = filt_min_n(c, net, min_n=min_n)
     sources, targets, net = get_net_mat(net)
 
     # Match arrays
     net = match(c, targets, net)
 
     if verbose:
         print(
-            "Running mlm on mat with {0} samples and {1} targets for {2} sources.".format(
+            "Running mlm on mat with {} samples and {} targets for {} sources.".format(
                 m.shape[0], len(c), net.shape[1]
             )
         )
 
     # Run MLM
     estimate, pvals = mlm(m, net, batch_size=batch_size, verbose=verbose)
```

### Comparing `rapids_singlecell-0.7.2/rapids_singlecell/decoupler_gpu/_method_wsum.py` & `rapids_singlecell-0.7.5/rapids_singlecell/decoupler_gpu/_method_wsum.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,16 @@
+from typing import Optional, Union
+
+import cupy as cp
 import numpy as np
 import pandas as pd
-import cupy as cp
-
-from decoupler.pre import extract, match, rename_net, get_net_mat, filt_min_n
-
 from anndata import AnnData
+from decoupler.pre import extract, filt_min_n, get_net_mat, match, rename_net
 from tqdm import tqdm
 
-from typing import Union, Optional
-
 
 def run_perm(estimate, mat, net, idxs, times, seed):
     mat = cp.ascontiguousarray(mat)
     cp.random.seed(seed)
     # Init null distirbution
     null_dst = cp.zeros((mat.shape[0], net.shape[1], times), dtype=np.float32)
     pvals = cp.zeros((mat.shape[0], net.shape[1]), dtype=np.float32)
@@ -47,15 +45,15 @@
 def wsum(mat, net, times, batch_size, seed, verbose):
     # Get number of batches
     n_samples = mat.shape[0]
     n_features, n_fsets = net.shape
     n_batches = int(np.ceil(n_samples / batch_size))
 
     if verbose:
-        print("Infering activities on {0} batches.".format(n_batches))
+        print(f"Infering activities on {n_batches} batches.")
 
     # Init empty acts
     estimate = np.zeros((n_samples, n_fsets), dtype=np.float32)
     if times > 1:
         norm = np.zeros((n_samples, n_fsets), dtype=np.float32)
         corr = np.zeros((n_samples, n_fsets), dtype=np.float32)
         pvals = np.zeros((n_samples, n_fsets), dtype=np.float32)
@@ -135,28 +133,27 @@
             **norm**: DataFrame
                 Normalized WSUM scores. Stored in `.obsm['wsum_norm']` if `mat` is AnnData.
             **corr** : DataFrame
                 Corrected WSUM scores. Stored in `.obsm['wsum_corr']` if `mat` is AnnData.
             **pvals** : DataFrame
                 Obtained p-values. Stored in `.obsm['wsum_pvals']` if `mat` is AnnData.
     """
-
     # Extract sparse matrix and array of genes
     m, r, c = extract(mat, use_raw=use_raw, verbose=verbose)
     # Transform net
     net = rename_net(net, source=source, target=target, weight=weight)
     net = filt_min_n(c, net, min_n=min_n)
     sources, targets, net = get_net_mat(net)
 
     # Match arrays
     net = match(c, targets, net)
 
     if verbose:
         print(
-            "Running wsum on mat with {0} samples and {1} targets for {2} sources.".format(
+            "Running wsum on mat with {} samples and {} targets for {} sources.".format(
                 m.shape[0], len(c), net.shape[1]
             )
         )
 
     # Run WSUM
     estimate, norm, corr, pvals = wsum(m, net, times, batch_size, seed, verbose)
```

### Comparing `rapids_singlecell-0.7.2/rapids_singlecell/scanpy_gpu/_clustering.py` & `rapids_singlecell-0.7.5/rapids_singlecell/scanpy_gpu/_clustering.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,19 @@
-import cupy as cp
+from typing import Optional
+
 import cudf
+import numpy as np
+import pandas as pd
+from anndata import AnnData
 from cugraph import Graph
 from cugraph import leiden as culeiden
 from cugraph import louvain as culouvain
-import numpy as np
-import pandas as pd
 from cuml.cluster import KMeans
-
-from anndata import AnnData
-
-from typing import Optional
 from natsort import natsorted
 
-import warnings
-
 
 def leiden(
     adata: AnnData,
     resolution: float = 1.0,
     n_iterations: int = 100,
     use_weights: bool = True,
     neighbors_key: Optional[int] = None,
@@ -79,18 +75,18 @@
 
     adata.obs[key_added] = pd.Categorical(
         values=groups.astype("U"),
         categories=natsorted(map(str, np.unique(groups))),
     )
     # store information on the clustering parameters
     adata.uns["leiden"] = {}
-    adata.uns["leiden"]["params"] = dict(
-        resolution=resolution,
-        n_iterations=n_iterations,
-    )
+    adata.uns["leiden"]["params"] = {
+        "resolution": resolution,
+        "n_iterations": n_iterations,
+    }
 
 
 def louvain(
     adata: AnnData,
     resolution: float = 1.0,
     n_iterations: int = 100,
     use_weights: bool = True,
@@ -156,15 +152,15 @@
     )
 
     adata.obs[key_added] = pd.Categorical(
         values=groups.astype("U"),
         categories=natsorted(map(str, np.unique(groups))),
     )
     adata.uns["louvain"] = {}
-    adata.uns["louvain"]["params"] = dict(resolution=resolution)
+    adata.uns["louvain"]["params"] = {"resolution": resolution}
 
 
 def kmeans(
     adata: AnnData,
     n_clusters: int = 8,
     key_added: str = "kmeans",
     random_state: float = 42,
@@ -180,15 +176,14 @@
             Number of clusters to compute
 
         random_state: float (default: 42)
             if you want results to be the same when you restart Python, select a
             state.
 
     """
-
     kmeans_out = KMeans(n_clusters=n_clusters, random_state=random_state).fit(
         adata.obsm["X_pca"]
     )
     groups = kmeans_out.labels_.astype(str)
 
     adata.obs[key_added] = pd.Categorical(
         values=groups.astype("U"),
```

### Comparing `rapids_singlecell-0.7.2/rapids_singlecell/scanpy_gpu/_diffmap.py` & `rapids_singlecell-0.7.5/rapids_singlecell/scanpy_gpu/_diffmap.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
+import cupy as cp
+import cupyx as cpx
+import cupyx.scipy.sparse
+import cupyx.scipy.sparse.linalg
 from anndata import AnnData
 from scipy.sparse import issparse
-import cupyx.scipy.sparse.linalg
-import cupyx.scipy.sparse
-import cupyx as cpx
-import cupy as cp
 
 
 def diffmap(
     adata: AnnData,
     n_comps: int = 15,
     neighbors_key: str = None,
     sort: str = "decrease",
@@ -33,25 +33,24 @@
             If specified, diffmap looks at `.obsp['neighbors_key_ connectivities']` for neighbors connectivities
         sort
             Leave as is for the same behavior as sc.tl.diffmap
         density_normalize
             Leave as is for the same behavior as sc.tl.diffmap
 
     Returns
-    ----------
+    -------
         updates `adata` with the following fields.
 
             `X_diffmap` : :class:`numpy.ndarray` (`adata.obsm`)
                 Diffusion map representation of data, which is the right eigen basis of
                 the transition matrix with eigenvectors as columns.
             `diffmap_evals` : :class:`numpy.ndarray` (`adata.uns`)
                 Array of size (number of eigen vectors).
                 Eigenvalues of transition matrix.
     """
-
     if neighbors_key:
         connectivities = adata.obsp[neighbors_key + "_connectivities"]
     else:
         connectivities = adata.obsp["connectivities"]
     if issparse(connectivities):
         W = cpx.scipy.sparse.csr_matrix(connectivities, dtype=cp.float32)
     else:
```

### Comparing `rapids_singlecell-0.7.2/rapids_singlecell/scanpy_gpu/_draw_graph.py` & `rapids_singlecell-0.7.5/rapids_singlecell/scanpy_gpu/_draw_graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-from anndata import AnnData
+from typing import Union
+
 import cudf
 import cugraph
-import numpy as np
 import cupy as cp
-from typing import Union
+import numpy as np
+from anndata import AnnData
 
 
 def draw_graph(
     adata: AnnData, init_pos: Union[str, bool, None] = None, max_iter: int = 500
 ) -> None:
     """
     Force-directed graph drawing with cugraph's implementation of Force Atlas 2.
@@ -27,21 +28,20 @@
             Force Atlas algorithm. When specified the algorithm will terminate
             after no more than the specified number of iterations.
             No error occurs when the algorithm terminates in this manner.
             Good short-term quality can be achieved with 50-100 iterations.
             Above 1000 iterations is discouraged.
 
     Returns
-    ----------
+    -------
         updates `adata` with the following fields.
 
             X_draw_graph_layout_fa : `adata.obsm`
                 Coordinates of graph layout.
     """
-
     from cugraph.layout import force_atlas2
 
     # Adjacency graph
     adjacency = adata.obsp["connectivities"]
     offsets = cudf.Series(adjacency.indptr)
     indices = cudf.Series(adjacency.indices)
     g = cugraph.Graph()
@@ -100,10 +100,10 @@
         scaling_ratio=2.0,
         strong_gravity_mode=False,
         gravity=1.0,
     )
     positions = cp.vstack((positions["x"].to_cupy(), positions["y"].to_cupy())).T
     layout = "fa"
     adata.uns["draw_graph"] = {}
-    adata.uns["draw_graph"]["params"] = dict(layout=layout, random_state=0)
+    adata.uns["draw_graph"]["params"] = {"layout": layout, "random_state": 0}
     key_added = f"X_draw_graph_{layout}"
     adata.obsm[key_added] = positions.get()  # Format output
```

### Comparing `rapids_singlecell-0.7.2/rapids_singlecell/scanpy_gpu/_embedding_density.py` & `rapids_singlecell-0.7.5/rapids_singlecell/scanpy_gpu/_embedding_density.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from anndata import AnnData
 import cupy as cp
 import numpy as np
+from anndata import AnnData
 
 
 def embedding_density(
     adata: AnnData,
     basis: str = "umap",
     groupby=None,
     key_added=None,
@@ -37,14 +37,15 @@
             are calculated per category.
         key_added
             Name of the `.obs` covariate that will be added with the density
             estimates.
         components
             The embedding dimensions over which the density should be calculated.
             This is limited to two components.
+
     Returns
     -------
     Updates `adata.obs` with an additional field specified by the `key_added` \
     parameter. This parameter defaults to `[basis]_density_[groupby]`, where \
     `[basis]` is one of `umap`, `diffmap`, `pca`, `tsne`, or `draw_graph_fa` \
     and `[groupby]` denotes the parameter input.
 
@@ -118,17 +119,18 @@
 
     # Reduce diffmap components for labeling
     # Note: plot_scatter takes care of correcting diffmap components
     #       for plotting automatically
     if basis != "diffmap":
         components += 1
 
-    adata.uns[f"{density_covariate}_params"] = dict(
-        covariate=groupby, components=components.tolist()
-    )
+    adata.uns[f"{density_covariate}_params"] = {
+        "covariate": groupby,
+        "components": components.tolist(),
+    }
 
 
 def _calc_density(x: cp.ndarray, y: cp.ndarray):
     """\
     Calculates the density of points in 2 dimensions.
     """
     from cuml.neighbors import KernelDensity
```

### Comparing `rapids_singlecell-0.7.2/rapids_singlecell/scanpy_gpu/_harmonpy_gpu.py` & `rapids_singlecell-0.7.5/rapids_singlecell/scanpy_gpu/_harmonpy_gpu.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,20 +12,20 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
-import pandas as pd
-import numpy as np
-import cupy as cp
+import logging
 
+import cupy as cp
+import numpy as np
+import pandas as pd
 from cuml import KMeans
-import logging
 
 # create logger
 logger = logging.getLogger("harmonypy_gpu")
 logger.setLevel(logging.DEBUG)
 ch = logging.StreamHandler()
 ch.setLevel(logging.DEBUG)
 formatter = logging.Formatter("%(asctime)s - %(name)s - %(levelname)s - %(message)s")
@@ -52,15 +52,14 @@
     plot_convergence=False,
     verbose=True,
     reference_values=None,
     cluster_prior=None,
     random_state=0,
 ):
     """Run Harmony."""
-
     # theta = None
     # lamb = None
     # sigma = 0.1
     # nclust = None
     # tau = 0
     # block_size = 0.05
     # epsilon_cluster = 1e-5
@@ -139,15 +138,15 @@
         lamb_mat,
         verbose,
     )
 
     return ho
 
 
-class Harmony(object):
+class Harmony:
     def __init__(
         self,
         Z,
         Phi,
         Phi_moe,
         Pr_b,
         sigma,
@@ -207,15 +206,15 @@
         self.O = cp.zeros((self.K, self.B))
         self.E = cp.zeros((self.K, self.B))
         self.W = cp.zeros((self.B + 1, self.d))
         self.Phi_Rk = cp.zeros((self.B + 1, self.N))
 
     def init_cluster(self):
         # Start with cluster centroids
-        kmeans_obj = KMeans(n_clusters=self.K, init="k-means++").fit(self.Z_cos.T)
+        kmeans_obj = KMeans(n_clusters=self.K, init="k-means||").fit(self.Z_cos.T)
         self.Y = kmeans_obj.cluster_centers_.T
         # (1) Normalize
         self.Y = self.Y / cp.linalg.norm(self.Y, ord=2, axis=0)
         # (2) Assign cluster probabilities
         self.dist_mat = 2 * (1 - cp.dot(self.Y.T, self.Z_cos))
         self.R = -self.dist_mat
         self.R = self.R / self.sigma[:, None]
@@ -245,15 +244,15 @@
         self.objective_kmeans_entropy.append(_entropy)
         self.objective_kmeans_cross.append(_cross_entropy)
 
     def harmonize(self, iter_harmony=10, verbose=True):
         converged = False
         for i in range(1, iter_harmony + 1):
             if verbose:
-                logger.info("Iteration {} of {}".format(i, iter_harmony))
+                logger.info(f"Iteration {i} of {iter_harmony}")
             # STEP 1: Clustering
             self.cluster()
             # STEP 2: Regress out covariates
             # self.moe_correct_ridge()
             self.Z_cos, self.Z_corr, self.W, self.Phi_Rk = moe_correct_ridge(
                 self.Z_orig,
                 self.Z_cos,
```

### Comparing `rapids_singlecell-0.7.2/rapids_singlecell/scanpy_gpu/_harmony_integrate.py` & `rapids_singlecell-0.7.5/rapids_singlecell/scanpy_gpu/_harmony_integrate.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.7.2/rapids_singlecell/scanpy_gpu/_pymde.py` & `rapids_singlecell-0.7.5/rapids_singlecell/scanpy_gpu/_pymde.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-from anndata import AnnData
-from typing import Optional, Literal
+from typing import Literal, Optional
+
 import pandas as pd
+from anndata import AnnData
 
 
 def mde(
     adata: AnnData,
     device: Optional[Literal["cpu", "cuda"]] = None,
     n_neighbors: int = 15,
     n_pcs: int = None,
@@ -42,38 +43,38 @@
         The appropriateness of use of visualization of high-dimensional spaces in single-
         cell omics remains an open research questions. See:
         Chari, Tara, Joeyta Banerjee, and Lior Pachter. "The specious art of single-cell genomics." bioRxiv (2021).
         If you use this function in your research please cite:
         Agrawal, Akshay, Alnur Ali, and Stephen Boyd. "Minimum-distortion embedding." arXiv preprint arXiv:2103.02559 (2021).
     """
     try:
-        import torch
         import pymde
+        import torch
     except ImportError:
         raise ImportError("Please install pymde package via `pip install pymde`")
 
-    if use_rep == None:
+    if use_rep is None:
         data = adata.obsm["X_pca"]
     else:
         data = adata.obsm[use_rep]
 
     if isinstance(data, pd.DataFrame):
         data = data.values
     if n_pcs is not None:
         data = data[:, :n_pcs]
 
     device = "cpu" if not torch.cuda.is_available() else "cuda"
-    _kwargs = dict(
-        embedding_dim=2,
-        constraint=pymde.Standardized(),
-        repulsive_fraction=0.7,
-        verbose=False,
-        device=device,
-        n_neighbors=n_neighbors,
-    )
+    _kwargs = {
+        "embedding_dim": 2,
+        "constraint": pymde.Standardized(),
+        "repulsive_fraction": 0.7,
+        "verbose": False,
+        "device": device,
+        "n_neighbors": n_neighbors,
+    }
     _kwargs.update(kwargs)
 
     emb = pymde.preserve_neighbors(data, **_kwargs).embed(verbose=_kwargs["verbose"])
 
     if isinstance(emb, torch.Tensor):
         emb = emb.cpu().numpy()
         torch.cuda.empty_cache()
```

### Comparing `rapids_singlecell-0.7.2/rapids_singlecell/scanpy_gpu/_rank_gene_groups.py` & `rapids_singlecell-0.7.5/rapids_singlecell/scanpy_gpu/_rank_gene_groups.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
+from typing import Iterable, Literal, Union
+
 import cupy as cp
-from anndata import AnnData
 import numpy as np
 import pandas as pd
-import warnings
-from typing import Iterable, Union, Optional, Literal
+from anndata import AnnData
 
 
 def _select_groups(labels, groups_order_subset="all"):
     groups_order = labels.cat.categories
     groups_masks = np.zeros(
         (len(labels.cat.categories), len(labels.cat.codes)), dtype=bool
     )
@@ -71,15 +71,15 @@
         n_genes
             The number of genes that appear in the returned tables.
             Defaults to all genes.
         layer
             Key from `adata.layers` whose value will be used to perform tests on.
 
     Returns
-    --------
+    -------
         Updates `adata` with the following fields.
 
             **names** : structured `np.ndarray` (`.uns['rank_genes_groups']`)
                 Structured array to be indexed by group id storing the gene
                 names. Ordered according to scores.
 
             **scores** : structured `np.ndarray` (`.uns['rank_genes_groups']`)
@@ -89,19 +89,18 @@
 
             **pvals** : structured `np.ndarray` (`.uns['rank_genes_groups']`)
                 p-values.
 
             **pvals_adj** : structured `np.ndarray` (`.uns['rank_genes_groups']`)
                 Corrected p-values.
     """
-
     #### Wherever we see "adata.obs[groupby], we should just replace w/ the groups"
 
     # for clarity, rename variable
-    if groups == "all" or groups == None:
+    if groups == "all" or groups is None:
         groups_order = "all"
     elif isinstance(groups, (str, int)):
         raise ValueError("Specify a sequence of groups")
     else:
         groups_order = list(groups)
         if isinstance(groups_order[0], int):
             groups_order = [str(n) for n in groups_order]
@@ -112,34 +111,34 @@
         cats = labels.cat.categories.tolist()
         raise ValueError(
             f"reference = {reference} needs to be one of groupby = {cats}."
         )
 
     groups_order, groups_masks = _select_groups(labels, groups_order)
 
-    if layer and use_raw == True:
+    if layer and use_raw is True:
         raise ValueError("Cannot specify `layer` and have `use_raw=True`.")
     elif layer:
         X = adata.layers[layer]
         var_names = adata.var_names
-    elif use_raw == None and adata.raw:
+    elif use_raw is None and adata.raw:
         print("defaulting to using `.raw`")
         X = adata.raw.X
         var_names = adata.raw.var_names
-    elif use_raw == True:
+    elif use_raw is True:
         X = adata.raw.X
         var_names = adata.raw.var_names
     else:
         X = adata.X
         var_names = adata.var_names
 
     # for clarity, rename variable
     n_genes_user = n_genes
     # make sure indices are not OoB in case there are less genes than n_genes
-    if n_genes == None or n_genes_user > X.shape[1]:
+    if n_genes is None or n_genes_user > X.shape[1]:
         n_genes_user = X.shape[1]
     # in the following, n_genes is simply another name for the total number of genes
 
     n_groups = groups_masks.shape[0]
     ns = np.zeros(n_groups, dtype=int)
     for imask, mask in enumerate(groups_masks):
         ns[imask] = np.where(mask)[0].size
@@ -174,15 +173,15 @@
 
     clf = LogisticRegression(**kwds)
     clf.fit(X, grouping_logreg)
     scores_all = cp.array(clf.coef_)
 
     if len(groups_order) == scores_all.shape[1]:
         scores_all = scores_all.T
-    for igroup, group in enumerate(groups_order):
+    for igroup, _group in enumerate(groups_order):
         if len(groups_order) <= 2:  # binary logistic regression
             scores = scores_all[0]
         else:
             scores = scores_all[igroup]
 
         partition = cp.argpartition(scores, -n_genes_user)[-n_genes_user:]
         partial_indices = cp.argsort(scores[partition])[::-1]
@@ -193,21 +192,24 @@
             break
 
     groups_order_save = [str(g) for g in groups_order]
     if len(groups) == 2:
         groups_order_save = [groups_order_save[0]]
 
     scores = np.rec.fromarrays(
-        [n for n in rankings_gene_scores],
+        list(rankings_gene_scores),
         dtype=[(rn, "float32") for rn in groups_order_save],
     )
 
     names = np.rec.fromarrays(
-        [n for n in rankings_gene_names],
+        list(rankings_gene_names),
         dtype=[(rn, "U50") for rn in groups_order_save],
     )
     adata.uns["rank_genes_groups"] = {}
-    adata.uns["rank_genes_groups"]["params"] = dict(
-        groupby=groupby, method="logreg", reference=refname, use_raw=use_raw
-    )
+    adata.uns["rank_genes_groups"]["params"] = {
+        "groupby": groupby,
+        "method": "logreg",
+        "reference": refname,
+        "use_raw": use_raw,
+    }
     adata.uns["rank_genes_groups"]["scores"] = scores
     adata.uns["rank_genes_groups"]["names"] = names
```

### Comparing `rapids_singlecell-0.7.2/rapids_singlecell/scanpy_gpu/_tsne.py` & `rapids_singlecell-0.7.5/rapids_singlecell/scanpy_gpu/_tsne.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from anndata import AnnData
 from cuml.manifold import TSNE
-from typing import Optional
 
 
 def tsne(
     adata: AnnData,
     n_pcs: int = None,
     use_rep: str = None,
     perplexity: int = 30,
@@ -13,15 +12,15 @@
     method: str = "barnes_hut",
     metric: str = "euclidean",
 ) -> None:
     """
     Performs t-distributed stochastic neighborhood embedding (tSNE) using cuML libraray.
 
     Parameters
-    ---------
+    ----------
         adata
             Annotated data matrix.
         n_pcs
             use this many PCs
         use_rep
             use this obsm keys (defaults to `X_pca`)
         perplexity
@@ -50,15 +49,15 @@
     Returns
     -------
         Updates `adata` with the following fields.
 
             **X_tsne** : `np.ndarray` (`adata.obs`, dtype `float`)
                 tSNE coordinates of data.
     """
-    if use_rep == None:
+    if use_rep is None:
         data = adata.obsm["X_pca"]
     else:
         data = adata.obsm[use_rep]
     if n_pcs is not None:
         data = data[:, :n_pcs]
     adata.obsm["X_tsne"] = TSNE(
         perplexity=perplexity,
```

### Comparing `rapids_singlecell-0.7.2/rapids_singlecell/squidpy_gpu/_autocorr.py` & `rapids_singlecell-0.7.5/rapids_singlecell/squidpy_gpu/_autocorr.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
-from anndata import AnnData
-import pandas as pd
-import numpy as np
 from typing import (
-    TYPE_CHECKING,
     Literal,  # < 3.8
+    Optional,
     Sequence,
     Union,
-    Optional,
 )
-from scipy import sparse
+
 import cupy as cp
 import cupyx as cpx
-from ._moransi import _morans_I_cupy
+import numpy as np
+import pandas as pd
+from anndata import AnnData
+from scipy import sparse
+from statsmodels.stats.multitest import multipletests
+
 from ._gearysc import _gearys_C_cupy
+from ._moransi import _morans_I_cupy
 from ._utils import _p_value_calc
-from statsmodels.stats.multitest import multipletests
 
 
 def spatial_autocorr(
     adata: AnnData,
     connectivity_key: str = "spatial_connectivities",
     genes: Union[str, Sequence[str], None] = None,
     mode: Literal["moran", "geary"] = "moran",
@@ -72,15 +73,14 @@
             If True, return the results as a DataFrame instead of storing them in `adata.uns`, by default False.
 
     Returns
     -------
             DataFrame containing the autocorrelation scores, p-values, and corrected p-values for each gene. \
             If `copy` is False, the results are stored in `adata.uns` and None is returned.
     """
-
     if genes is None:
         if "highly_variable" in adata.var:
             genes = adata[:, adata.var["highly_variable"]].var_names.values
         else:
             genes = adata.var_names.values
     if isinstance(genes, str):
         genes = [genes]
```

### Comparing `rapids_singlecell-0.7.2/rapids_singlecell/squidpy_gpu/_gearysc.py` & `rapids_singlecell-0.7.5/rapids_singlecell/squidpy_gpu/_gearysc.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-import cupy as cp
-import cupyx as cpx
 import math
 
+import cupy as cp
+import cupyx as cpx
 
 kernel_gearys_C_num_dense = r"""
 extern "C" __global__ void gearys_C_num_dense(const float* data,
 const int* adj_matrix_row_ptr, const int* adj_matrix_col_ind, const float* adj_matrix_data,
 float* num, int n_samples, int n_features) {
     int f = blockIdx.x * blockDim.x + threadIdx.x;
     int i = blockIdx.y * blockDim.y + threadIdx.y;
```

### Comparing `rapids_singlecell-0.7.2/rapids_singlecell/squidpy_gpu/_ligrec.py` & `rapids_singlecell-0.7.5/rapids_singlecell/squidpy_gpu/_ligrec.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,26 +1,27 @@
-import cupy as cp
-import numpy as np
-import pandas as pd
-from scipy.sparse import csc_matrix, issparse
-from cupyx.scipy.sparse import issparse as cpissparse
-import cupyx as cpx
 import math
-from anndata import AnnData
 from itertools import product
 from typing import (
-    Union,
+    Iterable,
     Literal,
+    Mapping,
     Optional,
     Sequence,
-    Mapping,
-    Iterable,
+    Union,
 )
-from ._utils import _create_sparse_df, _assert_categorical_obs
 
+import cupy as cp
+import cupyx as cpx
+import numpy as np
+import pandas as pd
+from anndata import AnnData
+from cupyx.scipy.sparse import issparse as cpissparse
+from scipy.sparse import csc_matrix, issparse
+
+from ._utils import _assert_categorical_obs, _create_sparse_df
 
 SOURCE = "source"
 TARGET = "target"
 
 
 def _get_interactions(
     interactions_params={},
@@ -150,18 +151,18 @@
 
     Parameters
     ----------
         adata
             Annotated data object.
 
         cluster_key
-            Key in :attr:`anndata.AnnData.obs` where clustering is stored.
+            Key in :attr:`~anndata.AnnData.obs` where clustering is stored.
 
         clusters
-            Clusters from :attr:`anndata.AnnData.obs` `['{cluster_key}']`. \
+            Clusters from :attr:`~anndata.AnnData.obs` `['{cluster_key}']`. \
             Can be specified either as a sequence of :class:`tuple` or just a \
             sequence of cluster names, in which case all combinations \
             considered.
 
         interactions
             Interaction to test. The type can be one of:
                 * :class:`pandas.DataFrame` - must contain at least 2 columns named `source` and `target`.
@@ -192,25 +193,25 @@
                 * `interactions` - correct interactions by performing FDR correction across the clusters.
                 * `clusters` - correct clusters by performing FDR correction across the interactions.
 
         alpha
             Significance level for FDR correction. Only used when `corr_method != None`.
 
         use_raw
-            Whether to access :attr:`anndata.AnnData.raw`
+            Whether to access :attr:`~anndata.AnnData.raw`
 
         copy
             If `True`, return the result, otherwise save it to the `adata` object.
 
         key_added
-            Key in :attr:`anndata.AnnData.uns` where the result is stored if copy = False. \
+            Key in :attr:`~anndata.AnnData.uns` where the result is stored if copy = False. \
             If None, '{cluster_key}_ligrec' will be used.
 
         gene_symbols
-            Key in :attr:`anndata.AnnData.var` to use instead of :attr:`anndata.AnnData.var_names`.
+            Key in :attr:`~anndata.AnnData.var` to use instead of :attr:`~anndata.AnnData.var_names`.
 
         n_perms
             Number of permutations for the permutation test.
 
         interactions_params
             Keyword arguments for :func:`omnipath.interactions.import_intercell_network()` defining the \
             interactions. These datasets from [Türei et al., 2016] are used by default: \
@@ -230,15 +231,15 @@
         * `means` -
             :class:`pandas.DataFrame` containing the mean expression.
         * `pvalues` -
             :class:`pandas.DataFrame` containing the possibly corrected p-values.
         * `metadata` -
             :class:`pandas.DataFrame` containing interaction metadata.
     Otherwise, modifies the adata object with the following key:
-        * :attr:`anndata.AnnData.uns` `['{key_added}']` -
+        * :attr:`~anndata.AnnData.uns` `['{key_added}']` -
             the above mentioned dict.
     NaN p-values mark combinations for which the mean expression of one of the \
     interacting components was 0 or it didnt pass the threshold percentage of \
     cells being expressed within a given cluster.
 
     """
     # Get and Check interactions
@@ -692,15 +693,15 @@
         int(math.ceil(n_cls) / block[1]),
     )
     total_counts = total_counts.astype(cp.float32)
     res = cp.zeros(
         (len(interactions_), len(interaction_clusters)), dtype=np.float32, order="C"
     )
     if cpissparse(data_cp):
-        for i in range(n_perms):
+        for _i in range(n_perms):
             cp.random.shuffle(clustering_use)
             g = cp.zeros((data_cp.shape[1], n_cls), dtype=cp.float32, order="C")
             mean_kernel_sparse(
                 grid_sparse,
                 block_sparse,
                 (
                     data_cp.indptr,
@@ -730,15 +731,15 @@
                     g,
                     len(interactions_),
                     len(interaction_clusters),
                     n_cls,
                 ),
             )
     else:
-        for i in range(n_perms):
+        for _i in range(n_perms):
             cp.random.shuffle(clustering_use)
             g = cp.zeros((data_cp.shape[1], n_cls), dtype=cp.float32, order="C")
             mean_kernel(
                 grid_shuffle,
                 block,
                 (data_cp, clustering_use, g, data_cp.shape[0], data_cp.shape[1], n_cls),
             )
```

### Comparing `rapids_singlecell-0.7.2/rapids_singlecell/squidpy_gpu/_moransi.py` & `rapids_singlecell-0.7.5/rapids_singlecell/squidpy_gpu/_moransi.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
+import math
+
 import cupy as cp
 import cupyx as cpx
-import math
 
 kernel_morans_I_num_dense = r"""
 extern "C" __global__
 void morans_I_num_dense(const float* data_centered, const int* adj_matrix_row_ptr, const int* adj_matrix_col_ind,
 const float* adj_matrix_data, float* num, int n_samples, int n_features) {
     int f = blockIdx.x * blockDim.x + threadIdx.x;
     int i = blockIdx.y * blockDim.y + threadIdx.y;
```

### Comparing `rapids_singlecell-0.7.2/rapids_singlecell/squidpy_gpu/_utils.py` & `rapids_singlecell-0.7.5/rapids_singlecell/squidpy_gpu/_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,37 +1,40 @@
-import numpy as np
 from typing import (
     TYPE_CHECKING,
     Any,
     Dict,
     Union,
 )
-from scipy import stats
-from scipy.sparse import spmatrix, issparse
+
+import numpy as np
 import pandas as pd
 from pandas.api.types import infer_dtype, is_categorical_dtype
+from scipy import stats
+from scipy.sparse import issparse, spmatrix
 
 
 ### Taken from squidpy: https://github.com/scverse/squidpy/blob/main/squidpy/gr/_ppatterns.py
 def _p_value_calc(
     score: np.ndarray,
     sims: Union[np.ndarray, None],
     weights: Union[spmatrix, np.ndarray],
     params: Dict[str, Any],
 ):
     """
     Handle p-value calculation for spatial autocorrelation function.
+
     Parameters
     ----------
     score
         (n_features,).
     sims
         (n_simulations, n_features).
     params
         Object to store relevant function parameters.
+
     Returns
     -------
     pval_norm
         p-value under normality assumption
     pval_sim
         p-values based on permutations
     pval_z_sim
```

