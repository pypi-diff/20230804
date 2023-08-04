# Comparing `tmp/hyperelastic-0.5.0.tar.gz` & `tmp/hyperelastic-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyperelastic-0.5.0.tar", last modified: Sun Jul  9 20:19:17 2023, max compression
+gzip compressed data, was "hyperelastic-0.6.0.tar", last modified: Fri Aug  4 12:36:05 2023, max compression
```

## Comparing `hyperelastic-0.5.0.tar` & `hyperelastic-0.6.0.tar`

### file list

```diff
@@ -1,40 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 20:19:17.615776 hyperelastic-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-09 20:19:06.000000 hyperelastic-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    50628 2023-07-09 20:19:17.615776 hyperelastic-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8745 2023-07-09 20:19:06.000000 hyperelastic-0.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-07-09 20:19:06.000000 hyperelastic-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 20:19:17.615776 hyperelastic-0.5.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 20:19:17.607776 hyperelastic-0.5.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 20:19:17.611775 hyperelastic-0.5.0/src/hyperelastic/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-09 20:19:06.000000 hyperelastic-0.5.0/src/hyperelastic/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-09 20:19:06.000000 hyperelastic-0.5.0/src/hyperelastic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 20:19:17.611775 hyperelastic-0.5.0/src/hyperelastic/frameworks/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-09 20:19:06.000000 hyperelastic-0.5.0/src/hyperelastic/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8932 2023-07-09 20:19:06.000000 hyperelastic-0.5.0/src/hyperelastic/frameworks/_invariants.py
--rw-r--r--   0 runner    (1001) docker     (123)     6610 2023-07-09 20:19:06.000000 hyperelastic-0.5.0/src/hyperelastic/frameworks/_stretches.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 20:19:17.611775 hyperelastic-0.5.0/src/hyperelastic/math/
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-09 20:19:06.000000 hyperelastic-0.5.0/src/hyperelastic/math/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27544 2023-07-09 20:19:06.000000 hyperelastic-0.5.0/src/hyperelastic/math/_voigt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 20:19:17.611775 hyperelastic-0.5.0/src/hyperelastic/models/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-09 20:19:06.000000 hyperelastic-0.5.0/src/hyperelastic/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 20:19:17.615776 hyperelastic-0.5.0/src/hyperelastic/models/invariants/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-09 20:19:06.000000 hyperelastic-0.5.0/src/hyperelastic/models/invariants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-07-09 20:19:06.000000 hyperelastic-0.5.0/src/hyperelastic/models/invariants/_third_order_deformation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 20:19:17.615776 hyperelastic-0.5.0/src/hyperelastic/models/stretches/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-09 20:19:06.000000 hyperelastic-0.5.0/src/hyperelastic/models/stretches/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-09 20:19:06.000000 hyperelastic-0.5.0/src/hyperelastic/models/stretches/_ogden.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 20:19:17.615776 hyperelastic-0.5.0/src/hyperelastic/spaces/
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-09 20:19:06.000000 hyperelastic-0.5.0/src/hyperelastic/spaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-07-09 20:19:06.000000 hyperelastic-0.5.0/src/hyperelastic/spaces/_deformation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-07-09 20:19:06.000000 hyperelastic-0.5.0/src/hyperelastic/spaces/_dilatational.py
--rw-r--r--   0 runner    (1001) docker     (123)     8027 2023-07-09 20:19:06.000000 hyperelastic-0.5.0/src/hyperelastic/spaces/_distortional.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 20:19:17.611775 hyperelastic-0.5.0/src/hyperelastic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    50628 2023-07-09 20:19:17.000000 hyperelastic-0.5.0/src/hyperelastic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-07-09 20:19:17.000000 hyperelastic-0.5.0/src/hyperelastic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 20:19:17.000000 hyperelastic-0.5.0/src/hyperelastic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-09 20:19:17.000000 hyperelastic-0.5.0/src/hyperelastic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-09 20:19:17.000000 hyperelastic-0.5.0/src/hyperelastic.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 20:19:17.615776 hyperelastic-0.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-07-09 20:19:06.000000 hyperelastic-0.5.0/tests/test_math.py
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-07-09 20:19:06.000000 hyperelastic-0.5.0/tests/test_space.py
--rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-07-09 20:19:06.000000 hyperelastic-0.5.0/tests/test_sympy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:36:05.002768 hyperelastic-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-08-04 12:35:53.000000 hyperelastic-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    50628 2023-08-04 12:36:05.002768 hyperelastic-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8745 2023-08-04 12:35:53.000000 hyperelastic-0.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-08-04 12:35:53.000000 hyperelastic-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:36:05.002768 hyperelastic-0.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:36:04.994768 hyperelastic-0.6.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:36:04.998768 hyperelastic-0.6.0/src/hyperelastic/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-04 12:35:53.000000 hyperelastic-0.6.0/src/hyperelastic/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-08-04 12:35:53.000000 hyperelastic-0.6.0/src/hyperelastic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:36:04.998768 hyperelastic-0.6.0/src/hyperelastic/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-08-04 12:35:53.000000 hyperelastic-0.6.0/src/hyperelastic/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5564 2023-08-04 12:35:53.000000 hyperelastic-0.6.0/src/hyperelastic/frameworks/_generalized.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8932 2023-08-04 12:35:53.000000 hyperelastic-0.6.0/src/hyperelastic/frameworks/_invariants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6610 2023-08-04 12:35:53.000000 hyperelastic-0.6.0/src/hyperelastic/frameworks/_stretches.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:36:04.998768 hyperelastic-0.6.0/src/hyperelastic/lab/
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-08-04 12:35:53.000000 hyperelastic-0.6.0/src/hyperelastic/lab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-08-04 12:35:53.000000 hyperelastic-0.6.0/src/hyperelastic/lab/_curve_fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-08-04 12:35:53.000000 hyperelastic-0.6.0/src/hyperelastic/lab/_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-08-04 12:35:53.000000 hyperelastic-0.6.0/src/hyperelastic/lab/_load_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-08-04 12:35:53.000000 hyperelastic-0.6.0/src/hyperelastic/lab/_optimize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-08-04 12:35:53.000000 hyperelastic-0.6.0/src/hyperelastic/lab/_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-08-04 12:35:53.000000 hyperelastic-0.6.0/src/hyperelastic/lab/_simulation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:36:04.998768 hyperelastic-0.6.0/src/hyperelastic/math/
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-08-04 12:35:53.000000 hyperelastic-0.6.0/src/hyperelastic/math/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27544 2023-08-04 12:35:53.000000 hyperelastic-0.6.0/src/hyperelastic/math/_voigt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:36:04.998768 hyperelastic-0.6.0/src/hyperelastic/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-08-04 12:35:53.000000 hyperelastic-0.6.0/src/hyperelastic/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:36:04.998768 hyperelastic-0.6.0/src/hyperelastic/models/generalized/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-08-04 12:35:53.000000 hyperelastic-0.6.0/src/hyperelastic/models/generalized/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-08-04 12:35:53.000000 hyperelastic-0.6.0/src/hyperelastic/models/generalized/_stretch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:36:04.998768 hyperelastic-0.6.0/src/hyperelastic/models/invariants/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-08-04 12:35:53.000000 hyperelastic-0.6.0/src/hyperelastic/models/invariants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-08-04 12:35:53.000000 hyperelastic-0.6.0/src/hyperelastic/models/invariants/_third_order_deformation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:36:04.998768 hyperelastic-0.6.0/src/hyperelastic/models/stretches/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-08-04 12:35:53.000000 hyperelastic-0.6.0/src/hyperelastic/models/stretches/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9260 2023-08-04 12:35:53.000000 hyperelastic-0.6.0/src/hyperelastic/models/stretches/_generalized_invariants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-08-04 12:35:53.000000 hyperelastic-0.6.0/src/hyperelastic/models/stretches/_ogden.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:36:05.002768 hyperelastic-0.6.0/src/hyperelastic/spaces/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-08-04 12:35:53.000000 hyperelastic-0.6.0/src/hyperelastic/spaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-08-04 12:35:53.000000 hyperelastic-0.6.0/src/hyperelastic/spaces/_deformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-08-04 12:35:53.000000 hyperelastic-0.6.0/src/hyperelastic/spaces/_dilatational.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8027 2023-08-04 12:35:53.000000 hyperelastic-0.6.0/src/hyperelastic/spaces/_distortional.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:36:04.998768 hyperelastic-0.6.0/src/hyperelastic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    50628 2023-08-04 12:36:04.000000 hyperelastic-0.6.0/src/hyperelastic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-08-04 12:36:04.000000 hyperelastic-0.6.0/src/hyperelastic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:36:04.000000 hyperelastic-0.6.0/src/hyperelastic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-04 12:36:04.000000 hyperelastic-0.6.0/src/hyperelastic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-04 12:36:04.000000 hyperelastic-0.6.0/src/hyperelastic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:36:05.002768 hyperelastic-0.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-08-04 12:35:53.000000 hyperelastic-0.6.0/tests/test_generalized.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-08-04 12:35:53.000000 hyperelastic-0.6.0/tests/test_lab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-08-04 12:35:53.000000 hyperelastic-0.6.0/tests/test_math.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-08-04 12:35:53.000000 hyperelastic-0.6.0/tests/test_space.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-08-04 12:35:53.000000 hyperelastic-0.6.0/tests/test_sympy.py
```

### Comparing `hyperelastic-0.5.0/LICENSE` & `hyperelastic-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hyperelastic-0.5.0/PKG-INFO` & `hyperelastic-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyperelastic
-Version: 0.5.0
+Version: 0.6.0
 Summary: Constitutive hyperelastic material formulations for FElupe
 Author: Andreas Dutzler
 Author-email: a.dutzler@gmail.com
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `hyperelastic-0.5.0/README.md` & `hyperelastic-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `hyperelastic-0.5.0/pyproject.toml` & `hyperelastic-0.6.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,16 @@
   "Topic :: Scientific/Engineering :: Mathematics",
   "Topic :: Utilities"
 ]
 dynamic = ["version"]
 requires-python = ">=3.7"
 dependencies = [
   "numpy",
+  "scipy",
+  "matplotlib",
 ]
 
 [project.optional-dependencies]
 test = [
     "felupe",
     "sympy",
 ]
```

### Comparing `hyperelastic-0.5.0/src/hyperelastic/__init__.py` & `hyperelastic-0.6.0/src/hyperelastic/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,23 @@
-from . import frameworks, math, models, spaces
+from . import frameworks, lab, math, models, spaces
 from .__about__ import __version__
+from .frameworks import GeneralizedInvariants as GeneralizedInvariantsFramework
 from .frameworks import Invariants as InvariantsFramework
 from .frameworks import Stretches as StretchesFramework
 from .spaces import Deformation as DeformationSpace
 from .spaces import Dilatational as DilatationalSpace
 from .spaces import Distortional as DistortionalSpace
 
 __all__ = [
+    "lab",
     "spaces",
     "frameworks",
     "math",
     "models",
     "__version__",
     "DistortionalSpace",
     "DilatationalSpace",
     "DeformationSpace",
     "InvariantsFramework",
     "StretchesFramework",
+    "GeneralizedInvariantsFramework",
 ]
```

### Comparing `hyperelastic-0.5.0/src/hyperelastic/frameworks/_invariants.py` & `hyperelastic-0.6.0/src/hyperelastic/frameworks/_invariants.py`

 * *Files identical despite different names*

### Comparing `hyperelastic-0.5.0/src/hyperelastic/frameworks/_stretches.py` & `hyperelastic-0.6.0/src/hyperelastic/frameworks/_stretches.py`

 * *Files identical despite different names*

### Comparing `hyperelastic-0.5.0/src/hyperelastic/math/_voigt.py` & `hyperelastic-0.6.0/src/hyperelastic/math/_voigt.py`

 * *Files identical despite different names*

### Comparing `hyperelastic-0.5.0/src/hyperelastic/models/invariants/_third_order_deformation.py` & `hyperelastic-0.6.0/src/hyperelastic/models/invariants/_third_order_deformation.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,25 +33,28 @@
 
         \frac{\partial^2 \psi}{\partial I_1~\partial I_2} &=
             \sum_{i \ge 1, j \ge 1} C_{ij}~i~(I_1 - 3)^{i-1}~j~(I_2 - 3)^{j-1}
 
 
     """
 
-    def __init__(self, C10=0, C01=0, C11=0, C20=0, C30=0):
+    def __init__(self, C10=0, C01=0, C11=0, C20=0, C30=0, strain=False):
         """Initialize the Third Order Deformation material formulation with its
         parameters.
         """
 
         self.C10 = C10
         self.C01 = C01
         self.C11 = C11
         self.C20 = C20
         self.C30 = C30
 
+        # value of invariants at the undeformed state
+        self.undeformed = 0 if strain else 3
+
     def gradient(self, I1, I2, I3, statevars):
         """The gradient as the partial derivative of the strain energy function w.r.t.
         the invariants."""
 
         dWdI1 = None
         dWdI2 = None
         dWdI3 = None
@@ -65,22 +68,22 @@
         if self.C10 != 0:
             dWdI1 += self.C10
 
         if self.C01 != 0:
             dWdI2 += self.C01
 
         if self.C11 != 0:
-            dWdI1 += self.C11 * (I2 - 3)
-            dWdI2 += self.C11 * (I1 - 3)
+            dWdI1 += self.C11 * (I2 - self.undeformed)
+            dWdI2 += self.C11 * (I1 - self.undeformed)
 
         if self.C20 != 0:
-            dWdI1 += self.C20 * 2 * (I1 - 3)
+            dWdI1 += self.C20 * 2 * (I1 - self.undeformed)
 
         if self.C30 != 0:
-            dWdI1 += self.C30 * 3 * (I1 - 3) ** 2
+            dWdI1 += self.C30 * 3 * (I1 - self.undeformed) ** 2
 
         return dWdI1, dWdI2, dWdI3, statevars
 
     def hessian(self, I1, I2, I3, statevars):
         """The hessian as the second partial derivatives of the strain energy function
         w.r.t. the invariants."""
 
@@ -88,13 +91,13 @@
         d2WdI2I2 = None
         d2WdI3I3 = None
         d2WdI1I2 = None
         d2WdI2I3 = None
         d2WdI1I3 = None
 
         if self.C20 != 0 or self.C30 != 0:
-            d2WdI1I1 = self.C20 * 2 + self.C30 * 6 * (I1 - 3)
+            d2WdI1I1 = self.C20 * 2 + self.C30 * 6 * (I1 - self.undeformed)
 
         if self.C11 != 0:
             d2WdI1I2 = self.C11
 
         return d2WdI1I1, d2WdI2I2, d2WdI3I3, d2WdI1I2, d2WdI2I3, d2WdI1I3
```

### Comparing `hyperelastic-0.5.0/src/hyperelastic/spaces/_deformation.py` & `hyperelastic-0.6.0/src/hyperelastic/spaces/_deformation.py`

 * *Files identical despite different names*

### Comparing `hyperelastic-0.5.0/src/hyperelastic/spaces/_dilatational.py` & `hyperelastic-0.6.0/src/hyperelastic/spaces/_dilatational.py`

 * *Files identical despite different names*

### Comparing `hyperelastic-0.5.0/src/hyperelastic/spaces/_distortional.py` & `hyperelastic-0.6.0/src/hyperelastic/spaces/_distortional.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import numpy as np
 
 from ..math import astensor, asvoigt, cdya, cdya_ik, ddot, det, dya, eye, inv, transpose
 
 
 class Distortional:
     r"""The distortional (part of the deformation) space is a partial deformation with
-    constant volume. For a given deformation map :math:`\boldsymbol{x}(\boldsymbol{x})`
+    constant volume. For a given deformation map :math:`\boldsymbol{x}(\boldsymbol{X})`
     and its deformation gradient :math:`\boldsymbol{F}`, the distortional part of the
     deformation gradient :math:`\hat{\boldsymbol{F}}` is obtained by a multiplicative
     (consecutive) split into a volume-changing (dilatational) and a constant-volume
     (distortional) part of the deformation gradient. Due to the fact that the
     dilatational part is proportional to the unit tensor, the order of these partial
     deformations is not unique.
```

### Comparing `hyperelastic-0.5.0/src/hyperelastic.egg-info/PKG-INFO` & `hyperelastic-0.6.0/src/hyperelastic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyperelastic
-Version: 0.5.0
+Version: 0.6.0
 Summary: Constitutive hyperelastic material formulations for FElupe
 Author: Andreas Dutzler
 Author-email: a.dutzler@gmail.com
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `hyperelastic-0.5.0/src/hyperelastic.egg-info/SOURCES.txt` & `hyperelastic-0.6.0/src/hyperelastic.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -5,23 +5,36 @@
 src/hyperelastic/__init__.py
 src/hyperelastic.egg-info/PKG-INFO
 src/hyperelastic.egg-info/SOURCES.txt
 src/hyperelastic.egg-info/dependency_links.txt
 src/hyperelastic.egg-info/requires.txt
 src/hyperelastic.egg-info/top_level.txt
 src/hyperelastic/frameworks/__init__.py
+src/hyperelastic/frameworks/_generalized.py
 src/hyperelastic/frameworks/_invariants.py
 src/hyperelastic/frameworks/_stretches.py
+src/hyperelastic/lab/__init__.py
+src/hyperelastic/lab/_curve_fit.py
+src/hyperelastic/lab/_experiment.py
+src/hyperelastic/lab/_load_case.py
+src/hyperelastic/lab/_optimize.py
+src/hyperelastic/lab/_plotting.py
+src/hyperelastic/lab/_simulation.py
 src/hyperelastic/math/__init__.py
 src/hyperelastic/math/_voigt.py
 src/hyperelastic/models/__init__.py
+src/hyperelastic/models/generalized/__init__.py
+src/hyperelastic/models/generalized/_stretch.py
 src/hyperelastic/models/invariants/__init__.py
 src/hyperelastic/models/invariants/_third_order_deformation.py
 src/hyperelastic/models/stretches/__init__.py
+src/hyperelastic/models/stretches/_generalized_invariants.py
 src/hyperelastic/models/stretches/_ogden.py
 src/hyperelastic/spaces/__init__.py
 src/hyperelastic/spaces/_deformation.py
 src/hyperelastic/spaces/_dilatational.py
 src/hyperelastic/spaces/_distortional.py
+tests/test_generalized.py
+tests/test_lab.py
 tests/test_math.py
 tests/test_space.py
 tests/test_sympy.py
```

### Comparing `hyperelastic-0.5.0/tests/test_math.py` & `hyperelastic-0.6.0/tests/test_math.py`

 * *Files identical despite different names*

### Comparing `hyperelastic-0.5.0/tests/test_space.py` & `hyperelastic-0.6.0/tests/test_space.py`

 * *Files 17% similar despite different names*

```diff
@@ -28,14 +28,34 @@
     model = hel.models.invariants.ThirdOrderDeformation(
         C10=0.4, C01=0.1, C11=0.02, C20=-0.05, C30=0.01
     )
     umat = hel.DistortionalSpace(hel.InvariantsFramework(model))
     fea(umat).evaluate(verbose=2)
 
 
+def test_distortional_generalized_strain_invariants():
+    tod = hel.models.invariants.ThirdOrderDeformation(
+        C10=0.4, C01=0.1, C20=0.1, strain=True
+    )
+    fun = hel.models.generalized.strain
+    framework = hel.GeneralizedInvariantsFramework(tod, fun=fun, exponent=1.4)
+    umat = hel.DistortionalSpace(framework)
+    fea(umat).evaluate(verbose=2)
+
+
+def test_distortional_generalized_deformation_invariants():
+    tod = hel.models.invariants.ThirdOrderDeformation(
+        C10=0.4, C01=0.1, C20=0.1, strain=False
+    )
+    fun = hel.models.generalized.deformation
+    framework = hel.GeneralizedInvariantsFramework(tod, fun=fun, exponent=1.4)
+    umat = hel.DistortionalSpace(framework)
+    fea(umat).evaluate(verbose=2)
+
+
 def test_dilatational_invariants():
     model = hel.models.invariants.ThirdOrderDeformation(C10=0.5)
     umat = hel.DilatationalSpace(hel.InvariantsFramework(model))
     fea(umat).evaluate(verbose=2)
 
 
 def test_deformation_invariants():
@@ -47,7 +67,9 @@
 
 
 if __name__ == "__main__":
     test_distortional_stretches()
     test_distortional_invariants()
     test_dilatational_invariants()
     test_deformation_invariants()
+    test_distortional_generalized_strain_invariants()
+    test_distortional_generalized_deformation_invariants()
```

### Comparing `hyperelastic-0.5.0/tests/test_sympy.py` & `hyperelastic-0.6.0/tests/test_sympy.py`

 * *Files identical despite different names*

