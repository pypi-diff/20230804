# Comparing `tmp/garoupa-2.220128.1.tar.gz` & `tmp/garoupa-2.220128.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "garoupa-2.220128.1.tar", max compression
+gzip compressed data, was "garoupa-2.220128.2.tar", max compression
```

## Comparing `garoupa-2.220128.1.tar` & `garoupa-2.220128.2.tar`

### file list

```diff
@@ -1,48 +1,47 @@
--rw-r--r--   0        0        0    35149 2021-05-31 18:06:07.802081 garoupa-2.220128.1/LICENSE
--rw-r--r--   0        0        0    19401 2022-01-28 17:15:50.623365 garoupa-2.220128.1/README.md
--rw-r--r--   0        0        0     1329 2022-01-28 17:15:52.099382 garoupa-2.220128.1/pyproject.toml
--rw-r--r--   0        0        0     2745 2021-12-09 16:54:11.558083 garoupa-2.220128.1/src/garoupa/__init__.py
--rw-r--r--   0        0        0     1344 2021-12-07 15:26:14.247255 garoupa-2.220128.1/src/garoupa/algebra/__init__.py
--rw-r--r--   0        0        0     1063 2021-12-07 15:26:14.251256 garoupa-2.220128.1/src/garoupa/algebra/abs/__init__.py
--rw-r--r--   0        0        0     3122 2021-12-07 15:26:14.251256 garoupa-2.220128.1/src/garoupa/algebra/abs/element.py
--rw-r--r--   0        0        0     1210 2021-12-07 15:26:14.251256 garoupa-2.220128.1/src/garoupa/algebra/cyclic/__init__.py
--rw-r--r--   0        0        0     1604 2021-12-07 15:26:14.251256 garoupa-2.220128.1/src/garoupa/algebra/cyclic/nat.py
--rw-r--r--   0        0        0     1951 2021-12-07 15:26:14.251256 garoupa-2.220128.1/src/garoupa/algebra/cyclic/natm.py
--rw-r--r--   0        0        0     2049 2021-12-07 15:26:14.251256 garoupa-2.220128.1/src/garoupa/algebra/cyclic/z.py
--rw-r--r--   0        0        0     2006 2021-12-07 15:26:14.251256 garoupa-2.220128.1/src/garoupa/algebra/cyclic/zm.py
--rw-r--r--   0        0        0     1141 2021-12-07 15:26:14.255256 garoupa-2.220128.1/src/garoupa/algebra/dihedral/__init__.py
--rw-r--r--   0        0        0     4403 2021-12-07 15:26:14.255256 garoupa-2.220128.1/src/garoupa/algebra/dihedral/d.py
--rw-r--r--   0        0        0     1514 2021-12-07 15:26:14.255256 garoupa-2.220128.1/src/garoupa/algebra/dihedral/dr.py
--rw-r--r--   0        0        0     1510 2021-12-07 15:26:14.255256 garoupa-2.220128.1/src/garoupa/algebra/dihedral/ds.py
--rw-r--r--   0        0        0     3140 2021-12-07 15:26:14.255256 garoupa-2.220128.1/src/garoupa/algebra/math.py
--rw-r--r--   0        0        0     1159 2021-12-07 15:26:14.255256 garoupa-2.220128.1/src/garoupa/algebra/matrix/__init__.py
--rw-r--r--   0        0        0     4356 2021-12-12 20:50:17.715457 garoupa-2.220128.1/src/garoupa/algebra/matrix/aux.py
--rw-r--r--   0        0        0    10241 2021-12-07 15:26:14.255256 garoupa-2.220128.1/src/garoupa/algebra/matrix/group.py
--rw-r--r--   0        0        0     2094 2021-12-07 15:26:14.259256 garoupa-2.220128.1/src/garoupa/algebra/matrix/m.py
--rw-r--r--   0        0        0     2966 2021-12-07 15:26:14.259256 garoupa-2.220128.1/src/garoupa/algebra/matrix/m128bit.py
--rw-r--r--   0        0        0     2037 2021-12-07 15:26:14.259256 garoupa-2.220128.1/src/garoupa/algebra/matrix/m8bit.py
--rw-r--r--   0        0        0     2583 2021-12-07 15:26:14.259256 garoupa-2.220128.1/src/garoupa/algebra/matrix/mat.py
--rw-r--r--   0        0        0     1842 2021-12-07 15:26:14.259256 garoupa-2.220128.1/src/garoupa/algebra/matrix/mat128bit.py
--rw-r--r--   0        0        0     1999 2021-12-07 15:26:14.259256 garoupa-2.220128.1/src/garoupa/algebra/matrix/mat8bit.py
--rw-r--r--   0        0        0    10458 2021-12-07 15:26:14.259256 garoupa-2.220128.1/src/garoupa/algebra/npmath.py
--rw-r--r--   0        0        0     1145 2021-12-07 15:26:14.259256 garoupa-2.220128.1/src/garoupa/algebra/product/__init__.py
--rw-r--r--   0        0        0     7322 2021-12-07 15:26:14.259256 garoupa-2.220128.1/src/garoupa/algebra/product/product.py
--rw-r--r--   0        0        0     1644 2021-12-07 15:26:14.263256 garoupa-2.220128.1/src/garoupa/algebra/product/tuple.py
--rw-r--r--   0        0        0     1142 2021-12-07 15:26:14.263256 garoupa-2.220128.1/src/garoupa/algebra/symmetric/__init__.py
--rw-r--r--   0        0        0     1687 2021-12-07 15:26:14.263256 garoupa-2.220128.1/src/garoupa/algebra/symmetric/perm.py
--rw-r--r--   0        0        0     2093 2021-12-07 15:26:14.263256 garoupa-2.220128.1/src/garoupa/algebra/symmetric/s.py
--rw-r--r--   0        0        0     1142 2021-12-07 15:26:14.263256 garoupa-2.220128.1/src/garoupa/config.py
--rw-r--r--   0        0        0     3266 2021-12-07 15:26:14.263256 garoupa-2.220128.1/src/garoupa/groups.py
--rw-r--r--   0        0        0    21495 2021-12-25 01:19:02.966187 garoupa-2.220128.1/src/garoupa/hosh.py
--rw-r--r--   0        0        0     1100 2021-12-07 15:26:14.263256 garoupa-2.220128.1/src/garoupa/misc/__init__.py
--rw-r--r--   0        0        0    13921 2021-12-07 20:35:10.058113 garoupa-2.220128.1/src/garoupa/misc/colors.py
--rw-r--r--   0        0        0     5899 2021-12-07 15:26:14.267256 garoupa-2.220128.1/src/garoupa/misc/core.py
--rw-r--r--   0        0        0     1089 2021-12-07 15:26:14.267256 garoupa-2.220128.1/src/garoupa/misc/encoding/__init__.py
--rw-r--r--   0        0        0     9095 2021-12-07 15:26:14.267256 garoupa-2.220128.1/src/garoupa/misc/encoding/base.py
--rw-r--r--   0        0        0     3597 2021-12-07 15:26:14.267256 garoupa-2.220128.1/src/garoupa/misc/encoding/base777.py
--rw-r--r--   0        0        0     1456 2021-12-07 15:26:14.267256 garoupa-2.220128.1/src/garoupa/misc/exception.py
--rw-r--r--   0        0        0     1531 2021-12-07 15:26:14.267256 garoupa-2.220128.1/src/garoupa/misc/helper.py
--rw-r--r--   0        0        0     4727 2021-12-07 15:26:14.267256 garoupa-2.220128.1/src/garoupa/misc/identity.py
--rw-r--r--   0        0        0     4296 2021-12-07 15:26:14.267256 garoupa-2.220128.1/src/garoupa/misc/math.py
--rw-r--r--   0        0        0    21179 2022-01-28 17:16:08.181470 garoupa-2.220128.1/setup.py
--rw-r--r--   0        0        0    20269 2022-01-28 17:16:08.182440 garoupa-2.220128.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2022-08-11 20:05:58.000000 garoupa-2.220128.2/LICENSE
+-rw-r--r--   0        0        0    19550 2023-08-04 21:47:38.342338 garoupa-2.220128.2/README.md
+-rw-r--r--   0        0        0     1361 2023-08-04 21:47:42.606341 garoupa-2.220128.2/pyproject.toml
+-rw-r--r--   0        0        0     2745 2022-08-11 20:05:58.000000 garoupa-2.220128.2/src/garoupa/__init__.py
+-rw-r--r--   0        0        0     1344 2022-08-11 20:05:58.000000 garoupa-2.220128.2/src/garoupa/algebra/__init__.py
+-rw-r--r--   0        0        0     1063 2022-08-11 20:05:58.000000 garoupa-2.220128.2/src/garoupa/algebra/abs/__init__.py
+-rw-r--r--   0        0        0     3122 2022-08-11 20:05:58.000000 garoupa-2.220128.2/src/garoupa/algebra/abs/element.py
+-rw-r--r--   0        0        0     1210 2022-08-11 20:05:58.000000 garoupa-2.220128.2/src/garoupa/algebra/cyclic/__init__.py
+-rw-r--r--   0        0        0     1604 2022-08-11 20:05:58.000000 garoupa-2.220128.2/src/garoupa/algebra/cyclic/nat.py
+-rw-r--r--   0        0        0     1951 2022-08-11 20:05:58.000000 garoupa-2.220128.2/src/garoupa/algebra/cyclic/natm.py
+-rw-r--r--   0        0        0     2049 2022-08-11 20:05:58.000000 garoupa-2.220128.2/src/garoupa/algebra/cyclic/z.py
+-rw-r--r--   0        0        0     2006 2022-08-11 20:05:58.000000 garoupa-2.220128.2/src/garoupa/algebra/cyclic/zm.py
+-rw-r--r--   0        0        0     1141 2022-08-11 20:05:58.000000 garoupa-2.220128.2/src/garoupa/algebra/dihedral/__init__.py
+-rw-r--r--   0        0        0     4403 2022-08-11 20:05:58.000000 garoupa-2.220128.2/src/garoupa/algebra/dihedral/d.py
+-rw-r--r--   0        0        0     1514 2022-08-11 20:05:58.000000 garoupa-2.220128.2/src/garoupa/algebra/dihedral/dr.py
+-rw-r--r--   0        0        0     1510 2022-08-11 20:05:58.000000 garoupa-2.220128.2/src/garoupa/algebra/dihedral/ds.py
+-rw-r--r--   0        0        0     3140 2022-08-11 20:05:58.000000 garoupa-2.220128.2/src/garoupa/algebra/math.py
+-rw-r--r--   0        0        0     1159 2022-08-11 20:05:58.000000 garoupa-2.220128.2/src/garoupa/algebra/matrix/__init__.py
+-rw-r--r--   0        0        0     4356 2022-08-11 20:05:58.000000 garoupa-2.220128.2/src/garoupa/algebra/matrix/aux.py
+-rw-r--r--   0        0        0    10241 2022-08-11 20:05:58.000000 garoupa-2.220128.2/src/garoupa/algebra/matrix/group.py
+-rw-r--r--   0        0        0     2094 2022-08-11 20:05:58.000000 garoupa-2.220128.2/src/garoupa/algebra/matrix/m.py
+-rw-r--r--   0        0        0     2966 2022-08-11 20:05:58.000000 garoupa-2.220128.2/src/garoupa/algebra/matrix/m128bit.py
+-rw-r--r--   0        0        0     2037 2022-08-11 20:05:58.000000 garoupa-2.220128.2/src/garoupa/algebra/matrix/m8bit.py
+-rw-r--r--   0        0        0     2583 2022-08-11 20:05:58.000000 garoupa-2.220128.2/src/garoupa/algebra/matrix/mat.py
+-rw-r--r--   0        0        0     1842 2022-08-11 20:05:58.000000 garoupa-2.220128.2/src/garoupa/algebra/matrix/mat128bit.py
+-rw-r--r--   0        0        0     1999 2022-08-11 20:05:58.000000 garoupa-2.220128.2/src/garoupa/algebra/matrix/mat8bit.py
+-rw-r--r--   0        0        0    10458 2022-08-11 20:05:58.000000 garoupa-2.220128.2/src/garoupa/algebra/npmath.py
+-rw-r--r--   0        0        0     1145 2022-08-11 20:05:58.000000 garoupa-2.220128.2/src/garoupa/algebra/product/__init__.py
+-rw-r--r--   0        0        0     7322 2022-08-11 20:05:58.000000 garoupa-2.220128.2/src/garoupa/algebra/product/product.py
+-rw-r--r--   0        0        0     1644 2022-08-11 20:05:58.000000 garoupa-2.220128.2/src/garoupa/algebra/product/tuple.py
+-rw-r--r--   0        0        0     1142 2022-08-11 20:05:58.000000 garoupa-2.220128.2/src/garoupa/algebra/symmetric/__init__.py
+-rw-r--r--   0        0        0     1687 2022-08-11 20:05:58.000000 garoupa-2.220128.2/src/garoupa/algebra/symmetric/perm.py
+-rw-r--r--   0        0        0     2093 2022-08-11 20:05:58.000000 garoupa-2.220128.2/src/garoupa/algebra/symmetric/s.py
+-rw-r--r--   0        0        0     1142 2022-08-11 20:05:58.000000 garoupa-2.220128.2/src/garoupa/config.py
+-rw-r--r--   0        0        0     3266 2022-08-11 20:05:58.000000 garoupa-2.220128.2/src/garoupa/groups.py
+-rw-r--r--   0        0        0    21495 2022-08-11 20:05:58.000000 garoupa-2.220128.2/src/garoupa/hosh.py
+-rw-r--r--   0        0        0     1100 2022-08-11 20:05:58.000000 garoupa-2.220128.2/src/garoupa/misc/__init__.py
+-rw-r--r--   0        0        0    13921 2023-02-07 17:56:10.949052 garoupa-2.220128.2/src/garoupa/misc/colors.py
+-rw-r--r--   0        0        0     5899 2022-08-11 20:05:58.000000 garoupa-2.220128.2/src/garoupa/misc/core.py
+-rw-r--r--   0        0        0     1089 2022-08-11 20:05:58.000000 garoupa-2.220128.2/src/garoupa/misc/encoding/__init__.py
+-rw-r--r--   0        0        0     9095 2022-08-11 20:05:58.000000 garoupa-2.220128.2/src/garoupa/misc/encoding/base.py
+-rw-r--r--   0        0        0     3597 2022-08-11 20:05:58.000000 garoupa-2.220128.2/src/garoupa/misc/encoding/base777.py
+-rw-r--r--   0        0        0     1456 2022-08-11 20:05:58.000000 garoupa-2.220128.2/src/garoupa/misc/exception.py
+-rw-r--r--   0        0        0     1531 2022-08-11 20:05:58.000000 garoupa-2.220128.2/src/garoupa/misc/helper.py
+-rw-r--r--   0        0        0     4727 2022-08-11 20:05:58.000000 garoupa-2.220128.2/src/garoupa/misc/identity.py
+-rw-r--r--   0        0        0     4296 2022-08-11 20:05:58.000000 garoupa-2.220128.2/src/garoupa/misc/math.py
+-rw-r--r--   0        0        0    20516 1970-01-01 00:00:00.000000 garoupa-2.220128.2/PKG-INFO
```

### Comparing `garoupa-2.220128.1/LICENSE` & `garoupa-2.220128.2/LICENSE`

 * *Files identical despite different names*

### Comparing `garoupa-2.220128.1/README.md` & `garoupa-2.220128.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 </a>
 ![Python version](https://img.shields.io/badge/python-3.8%20%7C%203.9-blue.svg)
 [![license: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5501845.svg)](https://doi.org/10.5281/zenodo.5501845)
 [![arXiv](https://img.shields.io/badge/arXiv-2109.06028-b31b1b.svg?style=flat-square)](https://arxiv.org/abs/2109.06028)
 [![API documentation](https://img.shields.io/badge/doc-API%20%28auto%29-a0a0a0.svg)](https://davips.github.io/garoupa)
-
+[![Downloads](https://static.pepy.tech/badge/garoupa)](https://pepy.tech/project/garoupa)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/garoupa)
 
 # GaROUPa - Identification based on group theory
 The identification module of this library is evolving at its successor library [hosh (code)](https://github.com/davips/hosh) / [hosh (package)](https://pypi.org/project/hosh).
 The algebra module exists only here.
  
 
 
@@ -218,29 +219,29 @@
 
 ```python3
 
 # Operating over 5 sampled pairs.
 for a, b in islice(zip(G, G), 0, 5):
     print(a, "*", b, "=", a * b, sep="\t")
 """
-«[3, 0, 1, 2], 3, dr2»	*	«[1, 2, 0, 3], 3, dr2»	=	«[0, 1, 3, 2], 1, dr0»
-«[1, 3, 0, 2], 3, ds3»	*	«[1, 0, 3, 2], 2, ds1»	=	«[3, 1, 2, 0], 0, dr2»
-«[2, 3, 0, 1], 2, ds7»	*	«[1, 0, 2, 3], 0, ds1»	=	«[3, 2, 0, 1], 2, dr2»
-«[2, 0, 3, 1], 2, ds3»	*	«[0, 1, 3, 2], 0, dr5»	=	«[2, 0, 1, 3], 2, ds2»
-«[1, 2, 0, 3], 0, dr5»	*	«[2, 0, 1, 3], 3, ds6»	=	«[0, 1, 2, 3], 3, ds3»
+«[1, 3, 0, 2], 2, ds1»	*	«[2, 0, 3, 1], 0, dr3»	=	«[0, 1, 2, 3], 2, ds2»
+«[1, 2, 0, 3], 1, ds0»	*	«[2, 1, 0, 3], 0, ds4»	=	«[0, 2, 1, 3], 1, dr0»
+«[3, 2, 0, 1], 3, dr3»	*	«[0, 1, 3, 2], 0, dr5»	=	«[3, 2, 1, 0], 3, dr0»
+«[2, 0, 3, 1], 0, dr5»	*	«[1, 0, 3, 2], 1, dr0»	=	«[0, 2, 1, 3], 1, dr1»
+«[3, 2, 0, 1], 0, dr7»	*	«[3, 1, 0, 2], 2, dr3»	=	«[1, 2, 3, 0], 2, dr2»
 """
 ```
 
 ```python3
 
 # Operator ~ is another way of sampling.
 G = S(12)
 print(~G)
 """
-[10, 6, 5, 4, 9, 8, 1, 7, 0, 2, 3, 11]
+[9, 1, 10, 6, 4, 5, 8, 7, 2, 3, 0, 11]
 """
 ```
 
 ```python3
 
 # Manual element creation.
 last_perm_i = factorial(12) - 1
@@ -354,17 +355,17 @@
         f"{count}/{i}:".rjust(15, " "),
         f"  {G.bits} bits",
         f"\t~{100 * count / i} %",
         sep="",
     )
 """
            |M3%4| = 64:            2560/4096:  6.0 bits	62.5 %
-       |D8×D8×D8| = 4096:          843/10000:  12.0 bits	~8.43 %
-    |D8×D8×D8×D8| = 65536:         396/10000:  16.0 bits	~3.96 %
- |D8×D8×D8×D8×D8| = 1048576:       164/10000:  20.0 bits	~1.64 %
+       |D8×D8×D8| = 4096:          813/10000:  12.0 bits	~8.13 %
+    |D8×D8×D8×D8| = 65536:         378/10000:  16.0 bits	~3.78 %
+ |D8×D8×D8×D8×D8| = 1048576:       142/10000:  20.0 bits	~1.42 %
 """
 ```
 
 
 </p>
 </details>
 
@@ -447,15 +448,15 @@
     )
 # * -> [Explicit FOR due to autogeneration of README through eval]
 """
 21.376617194973697 bits   Pc: 0.004113533525298232  order: 2722720 D5×D7×D11×D13×D17
 --------------------------------------------------------------
 {(-1, 10): 9, (9, 20): 7, (19, 30): 9, (inf, inf): 75}
 
-bits: 21.38  Pc: 4.11e-03   a^<30=0: 25/100 = 2.50e-01 D5×D7×D11×D13×D17 0.125 28/01/2022 14:15:50
+bits: 21.38  Pc: 4.11e-03   a^<30=0: 25/100 = 2.50e-01 D5×D7×D11×D13×D17 0.125 04/08/2023 18:47:38
 """
 ```
 
 
 </p>
 </details>
```

#### html2text {}

```diff
@@ -3,17 +3,19 @@
 codecov.io/gh/davips/garoupa) [pypi] ![Python version](https://img.shields.io/
 badge/python-3.8%20%7C%203.9-blue.svg) [![license: GPL v3](https://
 img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-
 3.0) [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5501845.svg)](https://
 doi.org/10.5281/zenodo.5501845) [![arXiv](https://img.shields.io/badge/arXiv-
 2109.06028-b31b1b.svg?style=flat-square)](https://arxiv.org/abs/2109.06028) [!
 [API documentation](https://img.shields.io/badge/doc-API%20%28auto%29-
-a0a0a0.svg)](https://davips.github.io/garoupa) # GaROUPa - Identification based
-on group theory The identification module of this library is evolving at its
-successor library [hosh (code)](https://github.com/davips/hosh) / [hosh
+a0a0a0.svg)](https://davips.github.io/garoupa) [![Downloads](https://
+static.pepy.tech/badge/garoupa)](https://pepy.tech/project/garoupa) ![PyPI -
+Downloads](https://img.shields.io/pypi/dm/garoupa) # GaROUPa - Identification
+based on group theory The identification module of this library is evolving at
+its successor library [hosh (code)](https://github.com/davips/hosh) / [hosh
 (package)](https://pypi.org/project/hosh). The algebra module exists only here.
 GaROUPa solves the identification problem of multi-valued objects or sequences
 of events.
 This [Python library](https://pypi.org/project/garoupa) / [code](https://
 github.com/davips/garoupa) provides a reference implementation for the UT*.4
 specification presented [here](https://arxiv.org/abs/2109.06028). | ![fir0002
 flagstaffotos [at] gmail.com Canon 20D + Tamron 28-75mm f/2.8, GFDL 1.2 <http:/
@@ -127,22 +129,22 @@
 provided below. **Abstract algebra module**
 ```python3 from itertools import islice from math import factorial from
 garoupa.algebra.cyclic import Z from garoupa.algebra.dihedral import D from
 garoupa.algebra.symmetric import Perm from garoupa.algebra.symmetric import S #
 Direct product between: # symmetric group S4; # cyclic group Z5; and, #
 dihedral group D4. G = S(4) * Z(5) * D(4) print(G) """ S4ÃZ5ÃD4 """ ```
 ```python3 # Operating over 5 sampled pairs. for a, b in islice(zip(G, G), 0,
-5): print(a, "*", b, "=", a * b, sep="\t") """ Â«[3, 0, 1, 2], 3, dr2Â» * Â«[1,
-2, 0, 3], 3, dr2Â» = Â«[0, 1, 3, 2], 1, dr0Â» Â«[1, 3, 0, 2], 3, ds3Â» * Â«[1,
-0, 3, 2], 2, ds1Â» = Â«[3, 1, 2, 0], 0, dr2Â» Â«[2, 3, 0, 1], 2, ds7Â» * Â«[1,
-0, 2, 3], 0, ds1Â» = Â«[3, 2, 0, 1], 2, dr2Â» Â«[2, 0, 3, 1], 2, ds3Â» * Â«[0,
-1, 3, 2], 0, dr5Â» = Â«[2, 0, 1, 3], 2, ds2Â» Â«[1, 2, 0, 3], 0, dr5Â» * Â«[2,
-0, 1, 3], 3, ds6Â» = Â«[0, 1, 2, 3], 3, ds3Â» """ ``` ```python3 # Operator ~
-is another way of sampling. G = S(12) print(~G) """ [10, 6, 5, 4, 9, 8, 1, 7,
-0, 2, 3, 11] """ ``` ```python3 # Manual element creation. last_perm_i =
+5): print(a, "*", b, "=", a * b, sep="\t") """ Â«[1, 3, 0, 2], 2, ds1Â» * Â«[2,
+0, 3, 1], 0, dr3Â» = Â«[0, 1, 2, 3], 2, ds2Â» Â«[1, 2, 0, 3], 1, ds0Â» * Â«[2,
+1, 0, 3], 0, ds4Â» = Â«[0, 2, 1, 3], 1, dr0Â» Â«[3, 2, 0, 1], 3, dr3Â» * Â«[0,
+1, 3, 2], 0, dr5Â» = Â«[3, 2, 1, 0], 3, dr0Â» Â«[2, 0, 3, 1], 0, dr5Â» * Â«[1,
+0, 3, 2], 1, dr0Â» = Â«[0, 2, 1, 3], 1, dr1Â» Â«[3, 2, 0, 1], 0, dr7Â» * Â«[3,
+1, 0, 2], 2, dr3Â» = Â«[1, 2, 3, 0], 2, dr2Â» """ ``` ```python3 # Operator ~
+is another way of sampling. G = S(12) print(~G) """ [9, 1, 10, 6, 4, 5, 8, 7,
+2, 3, 0, 11] """ ``` ```python3 # Manual element creation. last_perm_i =
 factorial(12) - 1 a = Perm(i=last_perm_i, n=12) print("Last element of S35:",
 a) """ Last element of S35: [11, 10, 9, 8, 7, 6, 5, 4, 3, 2, 1, 0] """ ```
 ```python3 # Inverse element. Group S4. a = Perm(i=21, n=4) b = Perm(i=17, n=4)
 print(a, "*", ~a, "=", (a * ~a).i, "=", a * ~a, "= identity") """ [1, 3, 2, 0]
 * [3, 0, 2, 1] = 0 = [0, 1, 2, 3] = identity """ ``` ```python3 print(a, "*",
 b, "=", a * b) """ [1, 3, 2, 0] * [1, 2, 3, 0] = [3, 2, 0, 1] """ ```
 ```python3 print(a, "*", b, "*", ~b, "=", a * b * ~b, "= a") """ [1, 3, 2, 0] *
@@ -158,17 +160,17 @@
 |D8ÃD8| = 256: 12544/65536: 8.0 bits 19.140625 % """ ``` ```python3 # Z4!
 traverse(Z(4) * Z(3) * Z(2)) """ |Z4ÃZ3ÃZ2| = 24: 576/576: 4.584962500721157
 bits 100.0 % """ ``` ```python3 # M 3x3 %4 traverse(M(3, 4)) # Large groups
 (sampling is needed). Gs = [D(8) ^ 3, D(8) ^ 4, D(8) ^ 5] for G in Gs: i, count
 = 0, 0 for a, b in zip(G, G): if a * b == b * a: count += 1 if i >= 10_000:
 break i += 1 print( f"|{G}| = ".rjust(20, " "), f"{G.order}:".ljust(10, " "),
 f"{count}/{i}:".rjust(15, " "), f" {G.bits} bits", f"\t~{100 * count / i} %",
-sep="", ) """ |M3%4| = 64: 2560/4096: 6.0 bits 62.5 % |D8ÃD8ÃD8| = 4096: 843/
-10000: 12.0 bits ~8.43 % |D8ÃD8ÃD8ÃD8| = 65536: 396/10000: 16.0 bits ~3.96 %
-|D8ÃD8ÃD8ÃD8ÃD8| = 1048576: 164/10000: 20.0 bits ~1.64 % """ ```
+sep="", ) """ |M3%4| = 64: 2560/4096: 6.0 bits 62.5 % |D8ÃD8ÃD8| = 4096: 813/
+10000: 12.0 bits ~8.13 % |D8ÃD8ÃD8ÃD8| = 65536: 378/10000: 16.0 bits ~3.78 %
+|D8ÃD8ÃD8ÃD8ÃD8| = 1048576: 142/10000: 20.0 bits ~1.42 % """ ```
  **Detect identity after many repetitions**
 ```python3 import operator from datetime import datetime from functools import
 reduce from math import log, inf from sys import argv from
 garoupa.algebra.dihedral import D from garoupa.algebra.symmetric import S
 example = len(argv) == 1 or (not argv[1].isdecimal() and argv[1][0] not in
 ["p", "s", "d"]) primes = [5, 7, 11, 13, 17, 19, 23, 29, 31, 37, 41, 43, 47,
 53, 59, 61, 67, 71, 73, 79, 83, 89, 97, 101, 103, 107, 109, 113, 127, 131, 137,
@@ -203,15 +205,15 @@
 ( f"\nbits: {log(G.order, 2):.2f} Pc: {G.comm_degree or -1:.2e} a^<{limit}=0:
 {bad}/{tot} = {bad / tot:.2e}", G, G._pi_core(hist), datetime.now().strftime
 ("%d/%m/%Y %H:%M:%S"), flush=True, ) # * -> [Explicit FOR due to autogeneration
 of README through eval] """ 21.376617194973697 bits Pc: 0.004113533525298232
 order: 2722720 D5ÃD7ÃD11ÃD13ÃD17 ------------------------------------------
 -------------------- {(-1, 10): 9, (9, 20): 7, (19, 30): 9, (inf, inf): 75}
 bits: 21.38 Pc: 4.11e-03 a^<30=0: 25/100 = 2.50e-01 D5ÃD7ÃD11ÃD13ÃD17 0.125
-28/01/2022 14:15:50 """ ```
+04/08/2023 18:47:38 """ ```
  **Tendence of commutativity on Mn**
 ```python3 from itertools import chain from garoupa.algebra.matrix.m import M
 from garoupa.algebra.matrix.m8bit import M8bit def traverse(G): i, count =
 G.order, G.order for idx, a in enumerate(G.sorted()): for b in list(G.sorted())
 [idx + 1:]: if a * b == b * a: count += 2 i += 2 print(f"|{G}| = ".rjust(20, '
 '), f"{G.order}:".ljust(10, ' '), f"{count}/{i}:".rjust(15, ' '), f" {G.bits}
 bits", f"\t{100 * count / i} %", sep="") M1_4 = map(M, range(1, 5)) for G in
```

### Comparing `garoupa-2.220128.1/pyproject.toml` & `garoupa-2.220128.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "garoupa"
-version = "2.220128.1"
+version = "2.220128.2"
 description = "Predictable operable hash-based identifiers and abstract algebra groups"
 authors = ["davips <dpsabc@gmail.com>"]
 license = "GPL"
 readme = 'README.md'
 packages = [
     { include = "garoupa", from = "src" },
 ]
@@ -17,15 +17,15 @@
 experiments = ["bigfloat"]
 
 [tool.poetry.dependencies]
 python = ">=3.8"
 wheel = "^0.37.0"
 blake3 = "^0.2.0"
 colored = "1.4.2"
-ansi2html = "^1.6.0"
+ansi2html = "1.6.0"
 #hosh = { version = "^2.0.0", optional = true }  #  not implemented yet
 progress = { version = "^1.6", optional = true }
 pathos = { version = "^0.2.8", optional = true }
 # numpy = { version = "^1.21.2", optional = true }
 bigfloat = { version = "^0.4.0", optional = true }
 
 [tool.poetry.dev-dependencies]
@@ -33,18 +33,20 @@
 autoreadme = "^0.2102.20"
 pytest = "^6.2.5"
 pytest-cov = "^2.12.1"
 progress = "^1.6"
 pathos = "^0.2.8"
 #numpy = "^1.21.2"
 ipython = "^7.27.0"
-pypi-server = "^0.4.8"
 black = "^21.9b0"
 flake8 = "^4.0.1"
 
+[tool.poetry.group.dev.dependencies]
+numpy = "^1.24.2"
+
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 # 
 # [[tool.poetry.source]]
 # name = "dvpypi"
 # url = "http://localhost:8080/simple"
```

### Comparing `garoupa-2.220128.1/src/garoupa/__init__.py` & `garoupa-2.220128.2/src/garoupa/__init__.py`

 * *Files identical despite different names*

### Comparing `garoupa-2.220128.1/src/garoupa/algebra/__init__.py` & `garoupa-2.220128.2/src/garoupa/algebra/__init__.py`

 * *Files identical despite different names*

### Comparing `garoupa-2.220128.1/src/garoupa/algebra/abs/__init__.py` & `garoupa-2.220128.2/src/garoupa/algebra/abs/__init__.py`

 * *Files identical despite different names*

### Comparing `garoupa-2.220128.1/src/garoupa/algebra/abs/element.py` & `garoupa-2.220128.2/src/garoupa/algebra/abs/element.py`

 * *Files identical despite different names*

### Comparing `garoupa-2.220128.1/src/garoupa/algebra/cyclic/__init__.py` & `garoupa-2.220128.2/src/garoupa/algebra/cyclic/__init__.py`

 * *Files identical despite different names*

### Comparing `garoupa-2.220128.1/src/garoupa/algebra/cyclic/nat.py` & `garoupa-2.220128.2/src/garoupa/algebra/cyclic/nat.py`

 * *Files identical despite different names*

### Comparing `garoupa-2.220128.1/src/garoupa/algebra/cyclic/natm.py` & `garoupa-2.220128.2/src/garoupa/algebra/cyclic/natm.py`

 * *Files identical despite different names*

### Comparing `garoupa-2.220128.1/src/garoupa/algebra/cyclic/z.py` & `garoupa-2.220128.2/src/garoupa/algebra/cyclic/z.py`

 * *Files identical despite different names*

### Comparing `garoupa-2.220128.1/src/garoupa/algebra/cyclic/zm.py` & `garoupa-2.220128.2/src/garoupa/algebra/cyclic/zm.py`

 * *Files identical despite different names*

### Comparing `garoupa-2.220128.1/src/garoupa/algebra/dihedral/__init__.py` & `garoupa-2.220128.2/src/garoupa/algebra/dihedral/__init__.py`

 * *Files identical despite different names*

### Comparing `garoupa-2.220128.1/src/garoupa/algebra/dihedral/d.py` & `garoupa-2.220128.2/src/garoupa/algebra/dihedral/d.py`

 * *Files identical despite different names*

### Comparing `garoupa-2.220128.1/src/garoupa/algebra/dihedral/dr.py` & `garoupa-2.220128.2/src/garoupa/algebra/dihedral/dr.py`

 * *Files identical despite different names*

### Comparing `garoupa-2.220128.1/src/garoupa/algebra/dihedral/ds.py` & `garoupa-2.220128.2/src/garoupa/algebra/dihedral/ds.py`

 * *Files identical despite different names*

### Comparing `garoupa-2.220128.1/src/garoupa/algebra/math.py` & `garoupa-2.220128.2/src/garoupa/algebra/math.py`

 * *Files identical despite different names*

### Comparing `garoupa-2.220128.1/src/garoupa/algebra/matrix/__init__.py` & `garoupa-2.220128.2/src/garoupa/algebra/matrix/__init__.py`

 * *Files identical despite different names*

### Comparing `garoupa-2.220128.1/src/garoupa/algebra/matrix/aux.py` & `garoupa-2.220128.2/src/garoupa/algebra/matrix/aux.py`

 * *Files identical despite different names*

### Comparing `garoupa-2.220128.1/src/garoupa/algebra/matrix/group.py` & `garoupa-2.220128.2/src/garoupa/algebra/matrix/group.py`

 * *Files identical despite different names*

### Comparing `garoupa-2.220128.1/src/garoupa/algebra/matrix/m.py` & `garoupa-2.220128.2/src/garoupa/algebra/matrix/m.py`

 * *Files identical despite different names*

### Comparing `garoupa-2.220128.1/src/garoupa/algebra/matrix/m128bit.py` & `garoupa-2.220128.2/src/garoupa/algebra/matrix/m128bit.py`

 * *Files identical despite different names*

### Comparing `garoupa-2.220128.1/src/garoupa/algebra/matrix/m8bit.py` & `garoupa-2.220128.2/src/garoupa/algebra/matrix/m8bit.py`

 * *Files identical despite different names*

### Comparing `garoupa-2.220128.1/src/garoupa/algebra/matrix/mat.py` & `garoupa-2.220128.2/src/garoupa/algebra/matrix/mat.py`

 * *Files identical despite different names*

### Comparing `garoupa-2.220128.1/src/garoupa/algebra/matrix/mat128bit.py` & `garoupa-2.220128.2/src/garoupa/algebra/matrix/mat128bit.py`

 * *Files identical despite different names*

### Comparing `garoupa-2.220128.1/src/garoupa/algebra/matrix/mat8bit.py` & `garoupa-2.220128.2/src/garoupa/algebra/matrix/mat8bit.py`

 * *Files identical despite different names*

### Comparing `garoupa-2.220128.1/src/garoupa/algebra/npmath.py` & `garoupa-2.220128.2/src/garoupa/algebra/npmath.py`

 * *Files identical despite different names*

### Comparing `garoupa-2.220128.1/src/garoupa/algebra/product/__init__.py` & `garoupa-2.220128.2/src/garoupa/algebra/product/__init__.py`

 * *Files identical despite different names*

### Comparing `garoupa-2.220128.1/src/garoupa/algebra/product/product.py` & `garoupa-2.220128.2/src/garoupa/algebra/product/product.py`

 * *Files identical despite different names*

### Comparing `garoupa-2.220128.1/src/garoupa/algebra/product/tuple.py` & `garoupa-2.220128.2/src/garoupa/algebra/product/tuple.py`

 * *Files identical despite different names*

### Comparing `garoupa-2.220128.1/src/garoupa/algebra/symmetric/__init__.py` & `garoupa-2.220128.2/src/garoupa/algebra/symmetric/__init__.py`

 * *Files identical despite different names*

### Comparing `garoupa-2.220128.1/src/garoupa/algebra/symmetric/perm.py` & `garoupa-2.220128.2/src/garoupa/algebra/symmetric/perm.py`

 * *Files identical despite different names*

### Comparing `garoupa-2.220128.1/src/garoupa/algebra/symmetric/s.py` & `garoupa-2.220128.2/src/garoupa/algebra/symmetric/s.py`

 * *Files identical despite different names*

### Comparing `garoupa-2.220128.1/src/garoupa/config.py` & `garoupa-2.220128.2/src/garoupa/config.py`

 * *Files identical despite different names*

### Comparing `garoupa-2.220128.1/src/garoupa/groups.py` & `garoupa-2.220128.2/src/garoupa/groups.py`

 * *Files identical despite different names*

### Comparing `garoupa-2.220128.1/src/garoupa/hosh.py` & `garoupa-2.220128.2/src/garoupa/hosh.py`

 * *Files identical despite different names*

### Comparing `garoupa-2.220128.1/src/garoupa/misc/__init__.py` & `garoupa-2.220128.2/src/garoupa/misc/__init__.py`

 * *Files identical despite different names*

### Comparing `garoupa-2.220128.1/src/garoupa/misc/colors.py` & `garoupa-2.220128.2/src/garoupa/misc/colors.py`

 * *Files identical despite different names*

### Comparing `garoupa-2.220128.1/src/garoupa/misc/core.py` & `garoupa-2.220128.2/src/garoupa/misc/core.py`

 * *Files identical despite different names*

### Comparing `garoupa-2.220128.1/src/garoupa/misc/encoding/__init__.py` & `garoupa-2.220128.2/src/garoupa/misc/encoding/__init__.py`

 * *Files identical despite different names*

### Comparing `garoupa-2.220128.1/src/garoupa/misc/encoding/base.py` & `garoupa-2.220128.2/src/garoupa/misc/encoding/base.py`

 * *Files identical despite different names*

### Comparing `garoupa-2.220128.1/src/garoupa/misc/encoding/base777.py` & `garoupa-2.220128.2/src/garoupa/misc/encoding/base777.py`

 * *Files identical despite different names*

### Comparing `garoupa-2.220128.1/src/garoupa/misc/exception.py` & `garoupa-2.220128.2/src/garoupa/misc/exception.py`

 * *Files identical despite different names*

### Comparing `garoupa-2.220128.1/src/garoupa/misc/helper.py` & `garoupa-2.220128.2/src/garoupa/misc/helper.py`

 * *Files identical despite different names*

### Comparing `garoupa-2.220128.1/src/garoupa/misc/identity.py` & `garoupa-2.220128.2/src/garoupa/misc/identity.py`

 * *Files identical despite different names*

### Comparing `garoupa-2.220128.1/src/garoupa/misc/math.py` & `garoupa-2.220128.2/src/garoupa/misc/math.py`

 * *Files identical despite different names*

### Comparing `garoupa-2.220128.1/setup.py` & `garoupa-2.220128.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,51 +1,579 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: garoupa
+Version: 2.220128.2
+Summary: Predictable operable hash-based identifiers and abstract algebra groups
+License: GPL
+Author: davips
+Author-email: dpsabc@gmail.com
+Requires-Python: >=3.8
+Classifier: License :: Other/Proprietary License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: algebra
+Provides-Extra: experiments
+Provides-Extra: native
+Requires-Dist: ansi2html (==1.6.0)
+Requires-Dist: bigfloat (>=0.4.0,<0.5.0) ; extra == "experiments"
+Requires-Dist: blake3 (>=0.2.0,<0.3.0)
+Requires-Dist: colored (==1.4.2)
+Requires-Dist: pathos (>=0.2.8,<0.3.0) ; extra == "algebra"
+Requires-Dist: progress (>=1.6,<2.0) ; extra == "algebra"
+Requires-Dist: wheel (>=0.37.0,<0.38.0)
+Description-Content-Type: text/markdown
 
-package_dir = \
-{'': 'src'}
+![test](https://github.com/davips/garoupa/workflows/test/badge.svg)
+[![codecov](https://codecov.io/gh/davips/garoupa/branch/main/graph/badge.svg)](https://codecov.io/gh/davips/garoupa)
+<a href="https://pypi.org/project/garoupa">
+<img src="https://img.shields.io/pypi/v/garoupa.svg?label=release&color=blue&style=flat-square" alt="pypi">
+</a>
+![Python version](https://img.shields.io/badge/python-3.8%20%7C%203.9-blue.svg)
+[![license: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 
-packages = \
-['garoupa',
- 'garoupa.algebra',
- 'garoupa.algebra.abs',
- 'garoupa.algebra.cyclic',
- 'garoupa.algebra.dihedral',
- 'garoupa.algebra.matrix',
- 'garoupa.algebra.product',
- 'garoupa.algebra.symmetric',
- 'garoupa.misc',
- 'garoupa.misc.encoding']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['ansi2html>=1.6.0,<2.0.0',
- 'blake3>=0.2.0,<0.3.0',
- 'colored==1.4.2',
- 'wheel>=0.37.0,<0.38.0']
-
-extras_require = \
-{'algebra': ['progress>=1.6,<2.0', 'pathos>=0.2.8,<0.3.0'],
- 'experiments': ['bigfloat>=0.4.0,<0.5.0']}
-
-setup_kwargs = {
-    'name': 'garoupa',
-    'version': '2.220128.1',
-    'description': 'Predictable operable hash-based identifiers and abstract algebra groups',
-    'long_description': '![test](https://github.com/davips/garoupa/workflows/test/badge.svg)\n[![codecov](https://codecov.io/gh/davips/garoupa/branch/main/graph/badge.svg)](https://codecov.io/gh/davips/garoupa)\n<a href="https://pypi.org/project/garoupa">\n<img src="https://img.shields.io/pypi/v/garoupa.svg?label=release&color=blue&style=flat-square" alt="pypi">\n</a>\n![Python version](https://img.shields.io/badge/python-3.8%20%7C%203.9-blue.svg)\n[![license: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)\n\n[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5501845.svg)](https://doi.org/10.5281/zenodo.5501845)\n[![arXiv](https://img.shields.io/badge/arXiv-2109.06028-b31b1b.svg?style=flat-square)](https://arxiv.org/abs/2109.06028)\n[![API documentation](https://img.shields.io/badge/doc-API%20%28auto%29-a0a0a0.svg)](https://davips.github.io/garoupa)\n\n\n# GaROUPa - Identification based on group theory\nThe identification module of this library is evolving at its successor library [hosh (code)](https://github.com/davips/hosh) / [hosh (package)](https://pypi.org/project/hosh).\nThe algebra module exists only here.\n \n\n\nGaROUPa solves the identification problem of multi-valued objects or sequences of events.<br>This [Python library](https://pypi.org/project/garoupa) / [code](https://github.com/davips/garoupa) provides a reference implementation for the UT*.4 specification presented [here](https://arxiv.org/abs/2109.06028).  | ![fir0002  flagstaffotos [at] gmail.com Canon 20D + Tamron 28-75mm f/2.8, GFDL 1.2 &lt;http://www.gnu.org/licenses/old-licenses/fdl-1.2.html&gt;, via Wikimedia Commons](https://upload.wikimedia.org/wikipedia/commons/thumb/a/a7/Malabar_grouper_melb_aquarium.jpg/256px-Malabar_grouper_melb_aquarium.jpg)\n:-------------------------:|:-------------------------:\n\nWe adopt a novel paradigm to universally unique identification (UUID), making identifiers deterministic and predictable, \neven before an object is generated by a (possibly costly) process.   \nHere, data versioning and composition of processing steps are directly mapped as simple operations over identifiers.\nWe call each of the latter a Hosh, i.e., an identifier is an _**o**perable **h**a**sh**_.\n\nA complete implementation of the remaining ideas from the [paper](https://arxiv.org/abs/2109.06028) is provided in this\n[cacheable lazy dict](https://pypi.org/project/ldict/2.211016.3) which depends on GaROUPa and serves as an advanced usage example.\n<br>\nA more robust (entirely rewritten) version is available in the package [idict](https://pypi.org/project/idict).\n\n## Overview\nA product of identifiers produces a new identifier as shown below, where sequences of bytes (`b"..."`) are passed to simulate binary objects to be hashed.\n\n![img.png](https://raw.githubusercontent.com/davips/garoupa/main/examples/img.png) | New identifiers are easily <br> created from the identity <br> element `ø`. Also available as `identity` for people <br>or systems allergic to <br>utf-8 encoding.\n-------------------------|-------------------------\n\n![img_1.png](https://raw.githubusercontent.com/davips/garoupa/main/examples/img_1.png) | Operations can be reverted by the inverse of the identifier.\n-------------------------|-------------------------\n\n![img_2.png](https://raw.githubusercontent.com/davips/garoupa/main/examples/img_2.png) | Operations are associative. <br>They are order-sensitive by default, <br>in which case they are called _ordered_ ids.\n-------------------------|-------------------------\n\nHowever, order-insensitive (called _unordered_) and order-insensitive-among-themselves (called _hybrid_) identifiers are also available. | .\n-------------------------|-------------------------\n![img_3.png](https://raw.githubusercontent.com/davips/garoupa/main/examples/img_3.png) | .\n\nThis is how they affect each other: | .\n-------------------------|-------------------------\n![img_4.png](https://raw.githubusercontent.com/davips/garoupa/main/examples/img_4.png) | .\n\nThe chance of collision is determined by the number of possible identifiers of each type.\nSome versions are provided, e.g.: UT32.4, UT40.4 (default), UT64.4.\nThey can be easily implemented in other languages and are \nintended to be a specification on how to identify multi-valued objects and multi-step processes.\nUnordered ids use a very narrow range of the total number of identifiers.\nThis is not a problem as they are not very useful.\n\nOne use for unordered ids could be the embedding of authorship or other metadata into an object without worrying about the timing, since the resulting id will remain the same, no matter when the unordered id is operated with the id of the object under construction. | . \n-------------------------|-------------------------\n![img_5.png](https://raw.githubusercontent.com/davips/garoupa/main/examples/img_5.png) | . \n\nConversely, hybrid ids are excelent to represent values in a data structure like a map, \nsince the order is not relevant when the consumer process looks up for keys, not indexes.\nConverselly, a chain of a data processing functions usually implies one step is dependent on the result of the previous step.\nThis makes ordered ids the perfect fit to identify functions (and also their composition, as a consequence).\n\n### Relationships can also be represented\nHere is another possible use. ORCIDs are managed unique identifiers for researchers.\nThey can be directly used as digests to create operable identifiers.\nWe recommend the use of 40 digits to allow operations with SHA-1 hashes. \nThey are common in version control repositories among other uses.\n![img_orcid.png](https://raw.githubusercontent.com/davips/garoupa/main/examples/img_orcid.png)\n\nUnordered relationships are represented by hybrid ids.\nAutomatic transparent conversion between ORCID dashes by a hexdecimal character can be implemented in the future if needed.\n![img_orcid-comm.png](https://raw.githubusercontent.com/davips/garoupa/main/examples/img_orcid-comm.png)\n\n## More info\nAside from the [paper](https://arxiv.org/abs/2109.06028), [PyPI package](https://pypi.org/project/garoupa) \nand [GitHub repository](https://github.com/davips/garoupa), \none can find more information, at a higher level application perspective, \nin this presentation:\n![image](https://raw.githubusercontent.com/davips/garoupa/14cb45b888eb8a18ae093d200075c1a8a7e9cacb/examples/capa-slides-gdocs.png)\nA lower level perspective is provided in the [API documentation](https://davips.github.io/garoupa).\n\n## Python installation\n### from package\n```bash\n# Set up a virtualenv. \npython3 -m venv venv\nsource venv/bin/activate\n\n# Install from PyPI\npip install garoupa\n```\n\n### from source\n```bash\ngit clone https://github.com/davips/garoupa\ncd garoupa\npoetry install\n```\n\n### Examples\nSome usage examples.\n\n**Basic operations**\n<details>\n<p>\n\n```python3\nfrom garoupa import Hosh, ø  # ø is a shortcut for identity (AltGr+O in most keyboards)\n\n# Hoshes (operable hash-based elements) can be multiplied.\na = Hosh(content=b"Some large binary content...")\nb = Hosh(content=b"Some other binary content. Might be, e.g., an action or another large content.")\nc = a * b\nprint(f"{a} * {b} = {c}")\n"""\n8CG9so9N1nQ59uNO8HGYcZ4ExQW5Haw4mErvw8m8 * 7N-L-10JS-H5DN0-BXW2e5ENWFQFVWswyz39t8s9 = z3EgxfisgqbNXBd0eqDuFiaTblBLA5ZAUbvEZgOh\n"""\n```\n\n```python3\nprint(~b)\n# Multiplication can be reverted by the inverse hosh. Zero is the identity hosh.\nprint(f"{b} * {~b} = {b * ~b} = 0")\n"""\nQ6OjmYZSJ8pB3ogBVMKBOxVp-oZ80czvtUrSyTzS\n7N-L-10JS-H5DN0-BXW2e5ENWFQFVWswyz39t8s9 * Q6OjmYZSJ8pB3ogBVMKBOxVp-oZ80czvtUrSyTzS = 0000000000000000000000000000000000000000 = 0\n"""\n```\n\n```python3\n\nprint(f"{b} * {ø} = {b * ø} = b")\n"""\n7N-L-10JS-H5DN0-BXW2e5ENWFQFVWswyz39t8s9 * 0000000000000000000000000000000000000000 = 7N-L-10JS-H5DN0-BXW2e5ENWFQFVWswyz39t8s9 = b\n"""\n```\n\n```python3\n\nprint(f"{c} * {~b} = {c * ~b} = {a} = a")\n"""\nz3EgxfisgqbNXBd0eqDuFiaTblBLA5ZAUbvEZgOh * Q6OjmYZSJ8pB3ogBVMKBOxVp-oZ80czvtUrSyTzS = 8CG9so9N1nQ59uNO8HGYcZ4ExQW5Haw4mErvw8m8 = 8CG9so9N1nQ59uNO8HGYcZ4ExQW5Haw4mErvw8m8 = a\n"""\n```\n\n```python3\n\nprint(f"{~a} * {c} = {~a * c} = {b} = b")\n"""\nRNvSdLI-5RiBBGL8NekctiQofWUIeYvXFP3wvTFT * z3EgxfisgqbNXBd0eqDuFiaTblBLA5ZAUbvEZgOh = 7N-L-10JS-H5DN0-BXW2e5ENWFQFVWswyz39t8s9 = 7N-L-10JS-H5DN0-BXW2e5ENWFQFVWswyz39t8s9 = b\n"""\n```\n\n```python3\n\n# Division is shorthand for reversion.\nprint(f"{c} / {b} = {c / b} = a")\n"""\nz3EgxfisgqbNXBd0eqDuFiaTblBLA5ZAUbvEZgOh / 7N-L-10JS-H5DN0-BXW2e5ENWFQFVWswyz39t8s9 = 8CG9so9N1nQ59uNO8HGYcZ4ExQW5Haw4mErvw8m8 = a\n"""\n```\n\n```python3\n\n# Hosh multiplication is not expected to be commutative.\nprint(f"{a * b} != {b * a}")\n"""\nz3EgxfisgqbNXBd0eqDuFiaTblBLA5ZAUbvEZgOh != wwSd0LaGvuV0W-yEOfgB-yVBMlNLA5ZAUbvEZgOh\n"""\n```\n\n```python3\n\n# Hosh multiplication is associative.\nprint(f"{a * (b * c)} = {(a * b) * c}")\n"""\nRuTcC4ZIr0Y1QLzYmytPRc087a8cbbW9Nj-gXxAz = RuTcC4ZIr0Y1QLzYmytPRc087a8cbbW9Nj-gXxAz\n"""\n```\n\n\n</p>\n</details>\n\n### Examples (abstract algebra)\nAlthough not the focus of the library, GaROUPa hosts also some niceties for group theory experimentation.\nSome examples are provided below.\n\n**Abstract algebra module**\n<details>\n<p>\n\n```python3\nfrom itertools import islice\nfrom math import factorial\n\nfrom garoupa.algebra.cyclic import Z\nfrom garoupa.algebra.dihedral import D\nfrom garoupa.algebra.symmetric import Perm\nfrom garoupa.algebra.symmetric import S\n\n# Direct product between:\n#   symmetric group S4;\n#   cyclic group Z5; and,\n#   dihedral group D4.\nG = S(4) * Z(5) * D(4)\nprint(G)\n"""\nS4×Z5×D4\n"""\n```\n\n```python3\n\n# Operating over 5 sampled pairs.\nfor a, b in islice(zip(G, G), 0, 5):\n    print(a, "*", b, "=", a * b, sep="\\t")\n"""\n«[3, 0, 1, 2], 3, dr2»\t*\t«[1, 2, 0, 3], 3, dr2»\t=\t«[0, 1, 3, 2], 1, dr0»\n«[1, 3, 0, 2], 3, ds3»\t*\t«[1, 0, 3, 2], 2, ds1»\t=\t«[3, 1, 2, 0], 0, dr2»\n«[2, 3, 0, 1], 2, ds7»\t*\t«[1, 0, 2, 3], 0, ds1»\t=\t«[3, 2, 0, 1], 2, dr2»\n«[2, 0, 3, 1], 2, ds3»\t*\t«[0, 1, 3, 2], 0, dr5»\t=\t«[2, 0, 1, 3], 2, ds2»\n«[1, 2, 0, 3], 0, dr5»\t*\t«[2, 0, 1, 3], 3, ds6»\t=\t«[0, 1, 2, 3], 3, ds3»\n"""\n```\n\n```python3\n\n# Operator ~ is another way of sampling.\nG = S(12)\nprint(~G)\n"""\n[10, 6, 5, 4, 9, 8, 1, 7, 0, 2, 3, 11]\n"""\n```\n\n```python3\n\n# Manual element creation.\nlast_perm_i = factorial(12) - 1\na = Perm(i=last_perm_i, n=12)\nprint("Last element of S35:", a)\n"""\nLast element of S35: [11, 10, 9, 8, 7, 6, 5, 4, 3, 2, 1, 0]\n"""\n```\n\n```python3\n\n# Inverse element. Group S4.\na = Perm(i=21, n=4)\nb = Perm(i=17, n=4)\nprint(a, "*", ~a, "=", (a * ~a).i, "=", a * ~a, "= identity")\n"""\n[1, 3, 2, 0] * [3, 0, 2, 1] = 0 = [0, 1, 2, 3] = identity\n"""\n```\n\n```python3\n\nprint(a, "*", b, "=", a * b)\n"""\n[1, 3, 2, 0] * [1, 2, 3, 0] = [3, 2, 0, 1]\n"""\n```\n\n```python3\n\nprint(a, "*", b, "*", ~b, "=", a * b * ~b, "= a")\n"""\n[1, 3, 2, 0] * [1, 2, 3, 0] * [3, 0, 1, 2] = [1, 3, 2, 0] = a\n"""\n```\n\n\n</p>\n</details>\n\n**Commutativity degree of groups**\n<details>\n<p>\n\n```python3\n\nfrom garoupa.algebra.cyclic import Z\nfrom garoupa.algebra.dihedral import D\nfrom garoupa.algebra.matrix.m import M\n\n\ndef traverse(G):\n    i, count = G.order, G.order\n    for idx, a in enumerate(G.sorted()):\n        for b in list(G.sorted())[idx + 1 :]:\n            if a * b == b * a:\n                count += 2\n            i += 2\n    print(\n        f"|{G}| = ".rjust(20, " "),\n        f"{G.order}:".ljust(10, " "),\n        f"{count}/{i}:".rjust(15, " "),\n        f"  {G.bits} bits",\n        f"\\t{100 * count / i} %",\n        sep="",\n    )\n\n\n# Dihedral\ntraverse(D(8))\n"""\n             |D8| = 16:              112/256:  4.0 bits\t43.75 %\n"""\n```\n\n```python3\ntraverse(D(8) ^ 2)\n"""\n          |D8×D8| = 256:         12544/65536:  8.0 bits\t19.140625 %\n"""\n```\n\n```python3\n\n# Z4!\ntraverse(Z(4) * Z(3) * Z(2))\n"""\n       |Z4×Z3×Z2| = 24:              576/576:  4.584962500721157 bits\t100.0 %\n"""\n```\n\n```python3\n\n# M 3x3 %4\ntraverse(M(3, 4))\n\n# Large groups (sampling is needed).\nGs = [D(8) ^ 3, D(8) ^ 4, D(8) ^ 5]\nfor G in Gs:\n    i, count = 0, 0\n    for a, b in zip(G, G):\n        if a * b == b * a:\n            count += 1\n        if i >= 10_000:\n            break\n        i += 1\n    print(\n        f"|{G}| = ".rjust(20, " "),\n        f"{G.order}:".ljust(10, " "),\n        f"{count}/{i}:".rjust(15, " "),\n        f"  {G.bits} bits",\n        f"\\t~{100 * count / i} %",\n        sep="",\n    )\n"""\n           |M3%4| = 64:            2560/4096:  6.0 bits\t62.5 %\n       |D8×D8×D8| = 4096:          843/10000:  12.0 bits\t~8.43 %\n    |D8×D8×D8×D8| = 65536:         396/10000:  16.0 bits\t~3.96 %\n |D8×D8×D8×D8×D8| = 1048576:       164/10000:  20.0 bits\t~1.64 %\n"""\n```\n\n\n</p>\n</details>\n\n**Detect identity after many repetitions**\n<details>\n<p>\n\n```python3\n\nimport operator\nfrom datetime import datetime\nfrom functools import reduce\nfrom math import log, inf\nfrom sys import argv\n\nfrom garoupa.algebra.dihedral import D\nfrom garoupa.algebra.symmetric import S\n\nexample = len(argv) == 1 or (not argv[1].isdecimal() and argv[1][0] not in ["p", "s", "d"])\n\nprimes = [5, 7, 11, 13, 17, 19, 23, 29, 31, 37, 41, 43, 47, 53, 59, 61, 67, 71, 73, 79, 83, 89, 97, 101, 103, 107,\n          109, 113, 127, 131, 137, 139, 149, 151, 157, 163, 167, 173, 179, 181, 191, 193, 197, 199, 211, 223, 227, 229,\n          233, 239, 241, 251, 257, 263, 269, 271, 277, 281, 283, 293, 307, 311, 313, 317, 331, 337, 347, 349, 353, 359,\n          367, 373, 379, 383, 389, 397, 401, 409, 419, 421, 431, 433, 439, 443, 449, 457, 461, 463, 467, 479, 487, 491,\n          499, 503, 509, 521, 523, 541, 547, 557, 563, 569, 571, 577, 587, 593, 599, 601, 607, 613, 617, 619, 631, 641,\n          643, 647, 653, 659, 661, 673, 677, 683, 691, 701, 709, 719, 727, 733, 739, 743, 751, 757, 761, 769, 773, 787,\n          797, 809, 811, 821, 823, 827, 829, 839, 853, 857, 859, 863, 877, 881, 883, 887, 907, 911, 919, 929, 937, 941,\n          947, 953, 967, 971, 977, 983, 991, 997, 1009]\n\nif example:\n    limit, sample = 30, 100\n    lst = []  # See *.\n    for n in primes[:5]:\n        lst.append(D(n, seed=n))\n    G = reduce(operator.mul, lst)\nelse:\n    limit, sample = int(argv[2]), int(argv[3]) if len(argv) > 2 else 1_000_000_000_000\n    if argv[1] == "s25d":\n        G = S(25) * reduce(operator.mul, [D(n) for n in primes[:9]])\n    elif argv[1] == "s57":\n        G = S(57)\n    elif argv[1] == "p384":\n        G = reduce(operator.mul, [D(n) for n in primes[:51]])\n    elif argv[1] == "p64":\n        G = reduce(operator.mul, [D(n) for n in primes[:12]])\n    elif argv[1] == "p96":\n        G = reduce(operator.mul, [D(n) for n in primes[:16]])\n    elif argv[1] == "p128":\n        G = reduce(operator.mul, [D(n) for n in primes[:21]])\n    elif argv[1] == "p256":\n        G = reduce(operator.mul, [D(n) for n in primes[:37]])\n    elif argv[1] == "64":\n        G = reduce(operator.mul, [D(n) for n in range(5, 31, 2)])\n    elif argv[1] == "96":\n        G = reduce(operator.mul, [D(n) for n in range(5, 41, 2)])\n    elif argv[1] == "128":\n        G = reduce(operator.mul, [D(n) for n in range(5, 51, 2)])\n    else:\n        G = reduce(operator.mul, [D(n) for n in range(5, 86, 2)])\n\nprint(f"{G.bits} bits   Pc: {G.comm_degree}  order: {G.order} {G}", flush=True)\nprint("--------------------------------------------------------------", flush=True)\nfor hist in G.sampled_orders(sample=sample, limit=limit):\n    tot = sum(hist.values())\n    bad = 0  # See *.\n    for k, v in hist.items():\n        if k[0] <= limit:\n            bad += v\n    print(hist, flush=True)\n    hist = hist.copy()\n    if (inf, inf) in hist:\n        del hist[(inf, inf)]\n    hist = {int((k[0] + k[1]) / 2): v for k, v in hist.items()}\n    print(\n        f"\\nbits: {log(G.order, 2):.2f}  Pc: {G.comm_degree or -1:.2e}   a^<{limit}=0: {bad}/{tot} = {bad / tot:.2e}",\n        G,\n        G._pi_core(hist),\n        datetime.now().strftime("%d/%m/%Y %H:%M:%S"),\n        flush=True,\n    )\n# * -> [Explicit FOR due to autogeneration of README through eval]\n"""\n21.376617194973697 bits   Pc: 0.004113533525298232  order: 2722720 D5×D7×D11×D13×D17\n--------------------------------------------------------------\n{(-1, 10): 9, (9, 20): 7, (19, 30): 9, (inf, inf): 75}\n\nbits: 21.38  Pc: 4.11e-03   a^<30=0: 25/100 = 2.50e-01 D5×D7×D11×D13×D17 0.125 28/01/2022 14:15:50\n"""\n```\n\n\n</p>\n</details>\n\n**Tendence of commutativity on Mn**\n<details>\n<p>\n\n```python3\nfrom itertools import chain\n\nfrom garoupa.algebra.matrix.m import M\nfrom garoupa.algebra.matrix.m8bit import M8bit\n\n\ndef traverse(G):\n    i, count = G.order, G.order\n    for idx, a in enumerate(G.sorted()):\n        for b in list(G.sorted())[idx + 1:]:\n            if a * b == b * a:\n                count += 2\n            i += 2\n    print(f"|{G}| = ".rjust(20, \' \'),\n          f"{G.order}:".ljust(10, \' \'),\n          f"{count}/{i}:".rjust(15, \' \'), f"  {G.bits} bits",\n          f"\\t{100 * count / i} %", sep="")\n\n\nM1_4 = map(M, range(1, 5))\nfor G in chain(M1_4, [M8bit(), M(5)]):\n    traverse(G)\n# ...\nfor G in map(M, range(6, 11)):\n    i, count = 0, 0\n    for a, b in zip(G, G):\n        if a * b == b * a:\n            count += 1\n        i += 1\n        if i >= 1_000_000:\n            break\n    print(f"|{G}| = ".rjust(20, \' \'),\n          f"{G.order}:".ljust(10, \' \'),\n          f"{count}/{i}:".rjust(15, \' \'), f"  {G.bits} bits",\n          f"\\t~{100 * count / i} %", sep="")\n\n"""\n|M1| = 1:                        1/1:  0 bits\t100.0 %\n|M2| = 2:                        4/4:  1 bits\t100.0 %\n|M3| = 8:                      40/64:  3 bits\t62.5 %\n|M4| = 64:                 1024/4096:  6 bits\t25.0 %\n|M8bit| = 256:              14848/65536:  8 bits\t22.65625 %\n|M5| = 1024:           62464/1048576:  10 bits\t5.95703125 %\n|M6| = 32768:              286/32768:  15 bits\t0.872802734375 %\n|M7| = 2097152:          683/1000000:  21 bits\t0.0683 %\n|M8| = 268435456:         30/1000000:  28 bits\t0.003 %\n|M9| = 68719476736:        1/1000000:  36 bits\t0.0001 %\n|M10| = 35184372088832:     0/1000000:  45 bits\t0.0 %\n"""\n```\n</p>\n</details>\n\n**Groups benefit from methods from the module \'hosh\'**\n<details>\n<p>\n\n```python3\nfrom garoupa.algebra.matrix import M\n\nm = ~M(23)\nprint(repr(m.hosh))\n```\n<a href="https://github.com/davips/garoupa/blob/main/examples/7KDd8TiA3S11QTkUid2wy87DQIeGQ35vB1bsP5Y6DjZ.png">\n<img src="https://raw.githubusercontent.com/davips/garoupa/main/examples/7KDd8TiA3S11QTkUid2wy87DQIeGQ35vB1bsP5Y6DjZ.png" alt="Colored base-62 representation" width="380" height="18">\n</a>\n</p>\n</details>\n\n\n\n## Performance\nComputation time for the simple operations performed by GaROUPa can be considered negligible for most applications,\nsince the order of magnitude of creating and operating identifiers is around a few μs:\n![img_6.png](https://raw.githubusercontent.com/davips/garoupa/main/examples/img_6.png)\nOn the other hand, we estimate up to ~7x gains in speed when porting the core code to  _rust_.\nThe package [hosh](https://pypi.org/project/hosh) was a faster implementation of an earlier version of GaROUPa,\nIt will be updated to be fully compatible with current GaROUPa at major version `2.*.*`.\nAs the performance of garoupa seems already very high, an updated \'rust\' implementation might become unnecessary.\nSome parts of the algebra module need additional packages, they can be installed using:\n`poetry install -E full`\n\n## Grants\nThis work was partially supported by Fapesp under supervision of\nProf. André C. P. L. F. de Carvalho at CEPID-CeMEAI (Grants 2013/07375-0 – 2019/01735-0).\n',
-    'author': 'davips',
-    'author_email': 'dpsabc@gmail.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': None,
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'python_requires': '>=3.8',
-}
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5501845.svg)](https://doi.org/10.5281/zenodo.5501845)
+[![arXiv](https://img.shields.io/badge/arXiv-2109.06028-b31b1b.svg?style=flat-square)](https://arxiv.org/abs/2109.06028)
+[![API documentation](https://img.shields.io/badge/doc-API%20%28auto%29-a0a0a0.svg)](https://davips.github.io/garoupa)
+[![Downloads](https://static.pepy.tech/badge/garoupa)](https://pepy.tech/project/garoupa)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/garoupa)
 
+# GaROUPa - Identification based on group theory
+The identification module of this library is evolving at its successor library [hosh (code)](https://github.com/davips/hosh) / [hosh (package)](https://pypi.org/project/hosh).
+The algebra module exists only here.
+ 
+
+
+GaROUPa solves the identification problem of multi-valued objects or sequences of events.<br>This [Python library](https://pypi.org/project/garoupa) / [code](https://github.com/davips/garoupa) provides a reference implementation for the UT*.4 specification presented [here](https://arxiv.org/abs/2109.06028).  | ![fir0002  flagstaffotos [at] gmail.com Canon 20D + Tamron 28-75mm f/2.8, GFDL 1.2 &lt;http://www.gnu.org/licenses/old-licenses/fdl-1.2.html&gt;, via Wikimedia Commons](https://upload.wikimedia.org/wikipedia/commons/thumb/a/a7/Malabar_grouper_melb_aquarium.jpg/256px-Malabar_grouper_melb_aquarium.jpg)
+:-------------------------:|:-------------------------:
+
+We adopt a novel paradigm to universally unique identification (UUID), making identifiers deterministic and predictable, 
+even before an object is generated by a (possibly costly) process.   
+Here, data versioning and composition of processing steps are directly mapped as simple operations over identifiers.
+We call each of the latter a Hosh, i.e., an identifier is an _**o**perable **h**a**sh**_.
+
+A complete implementation of the remaining ideas from the [paper](https://arxiv.org/abs/2109.06028) is provided in this
+[cacheable lazy dict](https://pypi.org/project/ldict/2.211016.3) which depends on GaROUPa and serves as an advanced usage example.
+<br>
+A more robust (entirely rewritten) version is available in the package [idict](https://pypi.org/project/idict).
+
+## Overview
+A product of identifiers produces a new identifier as shown below, where sequences of bytes (`b"..."`) are passed to simulate binary objects to be hashed.
+
+![img.png](https://raw.githubusercontent.com/davips/garoupa/main/examples/img.png) | New identifiers are easily <br> created from the identity <br> element `ø`. Also available as `identity` for people <br>or systems allergic to <br>utf-8 encoding.
+-------------------------|-------------------------
+
+![img_1.png](https://raw.githubusercontent.com/davips/garoupa/main/examples/img_1.png) | Operations can be reverted by the inverse of the identifier.
+-------------------------|-------------------------
+
+![img_2.png](https://raw.githubusercontent.com/davips/garoupa/main/examples/img_2.png) | Operations are associative. <br>They are order-sensitive by default, <br>in which case they are called _ordered_ ids.
+-------------------------|-------------------------
+
+However, order-insensitive (called _unordered_) and order-insensitive-among-themselves (called _hybrid_) identifiers are also available. | .
+-------------------------|-------------------------
+![img_3.png](https://raw.githubusercontent.com/davips/garoupa/main/examples/img_3.png) | .
+
+This is how they affect each other: | .
+-------------------------|-------------------------
+![img_4.png](https://raw.githubusercontent.com/davips/garoupa/main/examples/img_4.png) | .
+
+The chance of collision is determined by the number of possible identifiers of each type.
+Some versions are provided, e.g.: UT32.4, UT40.4 (default), UT64.4.
+They can be easily implemented in other languages and are 
+intended to be a specification on how to identify multi-valued objects and multi-step processes.
+Unordered ids use a very narrow range of the total number of identifiers.
+This is not a problem as they are not very useful.
+
+One use for unordered ids could be the embedding of authorship or other metadata into an object without worrying about the timing, since the resulting id will remain the same, no matter when the unordered id is operated with the id of the object under construction. | . 
+-------------------------|-------------------------
+![img_5.png](https://raw.githubusercontent.com/davips/garoupa/main/examples/img_5.png) | . 
+
+Conversely, hybrid ids are excelent to represent values in a data structure like a map, 
+since the order is not relevant when the consumer process looks up for keys, not indexes.
+Converselly, a chain of a data processing functions usually implies one step is dependent on the result of the previous step.
+This makes ordered ids the perfect fit to identify functions (and also their composition, as a consequence).
+
+### Relationships can also be represented
+Here is another possible use. ORCIDs are managed unique identifiers for researchers.
+They can be directly used as digests to create operable identifiers.
+We recommend the use of 40 digits to allow operations with SHA-1 hashes. 
+They are common in version control repositories among other uses.
+![img_orcid.png](https://raw.githubusercontent.com/davips/garoupa/main/examples/img_orcid.png)
+
+Unordered relationships are represented by hybrid ids.
+Automatic transparent conversion between ORCID dashes by a hexdecimal character can be implemented in the future if needed.
+![img_orcid-comm.png](https://raw.githubusercontent.com/davips/garoupa/main/examples/img_orcid-comm.png)
+
+## More info
+Aside from the [paper](https://arxiv.org/abs/2109.06028), [PyPI package](https://pypi.org/project/garoupa) 
+and [GitHub repository](https://github.com/davips/garoupa), 
+one can find more information, at a higher level application perspective, 
+in this presentation:
+![image](https://raw.githubusercontent.com/davips/garoupa/14cb45b888eb8a18ae093d200075c1a8a7e9cacb/examples/capa-slides-gdocs.png)
+A lower level perspective is provided in the [API documentation](https://davips.github.io/garoupa).
+
+## Python installation
+### from package
+```bash
+# Set up a virtualenv. 
+python3 -m venv venv
+source venv/bin/activate
+
+# Install from PyPI
+pip install garoupa
+```
+
+### from source
+```bash
+git clone https://github.com/davips/garoupa
+cd garoupa
+poetry install
+```
+
+### Examples
+Some usage examples.
+
+**Basic operations**
+<details>
+<p>
+
+```python3
+from garoupa import Hosh, ø  # ø is a shortcut for identity (AltGr+O in most keyboards)
+
+# Hoshes (operable hash-based elements) can be multiplied.
+a = Hosh(content=b"Some large binary content...")
+b = Hosh(content=b"Some other binary content. Might be, e.g., an action or another large content.")
+c = a * b
+print(f"{a} * {b} = {c}")
+"""
+8CG9so9N1nQ59uNO8HGYcZ4ExQW5Haw4mErvw8m8 * 7N-L-10JS-H5DN0-BXW2e5ENWFQFVWswyz39t8s9 = z3EgxfisgqbNXBd0eqDuFiaTblBLA5ZAUbvEZgOh
+"""
+```
+
+```python3
+print(~b)
+# Multiplication can be reverted by the inverse hosh. Zero is the identity hosh.
+print(f"{b} * {~b} = {b * ~b} = 0")
+"""
+Q6OjmYZSJ8pB3ogBVMKBOxVp-oZ80czvtUrSyTzS
+7N-L-10JS-H5DN0-BXW2e5ENWFQFVWswyz39t8s9 * Q6OjmYZSJ8pB3ogBVMKBOxVp-oZ80czvtUrSyTzS = 0000000000000000000000000000000000000000 = 0
+"""
+```
+
+```python3
+
+print(f"{b} * {ø} = {b * ø} = b")
+"""
+7N-L-10JS-H5DN0-BXW2e5ENWFQFVWswyz39t8s9 * 0000000000000000000000000000000000000000 = 7N-L-10JS-H5DN0-BXW2e5ENWFQFVWswyz39t8s9 = b
+"""
+```
+
+```python3
+
+print(f"{c} * {~b} = {c * ~b} = {a} = a")
+"""
+z3EgxfisgqbNXBd0eqDuFiaTblBLA5ZAUbvEZgOh * Q6OjmYZSJ8pB3ogBVMKBOxVp-oZ80czvtUrSyTzS = 8CG9so9N1nQ59uNO8HGYcZ4ExQW5Haw4mErvw8m8 = 8CG9so9N1nQ59uNO8HGYcZ4ExQW5Haw4mErvw8m8 = a
+"""
+```
+
+```python3
+
+print(f"{~a} * {c} = {~a * c} = {b} = b")
+"""
+RNvSdLI-5RiBBGL8NekctiQofWUIeYvXFP3wvTFT * z3EgxfisgqbNXBd0eqDuFiaTblBLA5ZAUbvEZgOh = 7N-L-10JS-H5DN0-BXW2e5ENWFQFVWswyz39t8s9 = 7N-L-10JS-H5DN0-BXW2e5ENWFQFVWswyz39t8s9 = b
+"""
+```
+
+```python3
+
+# Division is shorthand for reversion.
+print(f"{c} / {b} = {c / b} = a")
+"""
+z3EgxfisgqbNXBd0eqDuFiaTblBLA5ZAUbvEZgOh / 7N-L-10JS-H5DN0-BXW2e5ENWFQFVWswyz39t8s9 = 8CG9so9N1nQ59uNO8HGYcZ4ExQW5Haw4mErvw8m8 = a
+"""
+```
+
+```python3
+
+# Hosh multiplication is not expected to be commutative.
+print(f"{a * b} != {b * a}")
+"""
+z3EgxfisgqbNXBd0eqDuFiaTblBLA5ZAUbvEZgOh != wwSd0LaGvuV0W-yEOfgB-yVBMlNLA5ZAUbvEZgOh
+"""
+```
+
+```python3
+
+# Hosh multiplication is associative.
+print(f"{a * (b * c)} = {(a * b) * c}")
+"""
+RuTcC4ZIr0Y1QLzYmytPRc087a8cbbW9Nj-gXxAz = RuTcC4ZIr0Y1QLzYmytPRc087a8cbbW9Nj-gXxAz
+"""
+```
+
+
+</p>
+</details>
+
+### Examples (abstract algebra)
+Although not the focus of the library, GaROUPa hosts also some niceties for group theory experimentation.
+Some examples are provided below.
+
+**Abstract algebra module**
+<details>
+<p>
+
+```python3
+from itertools import islice
+from math import factorial
+
+from garoupa.algebra.cyclic import Z
+from garoupa.algebra.dihedral import D
+from garoupa.algebra.symmetric import Perm
+from garoupa.algebra.symmetric import S
+
+# Direct product between:
+#   symmetric group S4;
+#   cyclic group Z5; and,
+#   dihedral group D4.
+G = S(4) * Z(5) * D(4)
+print(G)
+"""
+S4×Z5×D4
+"""
+```
+
+```python3
+
+# Operating over 5 sampled pairs.
+for a, b in islice(zip(G, G), 0, 5):
+    print(a, "*", b, "=", a * b, sep="\t")
+"""
+«[1, 3, 0, 2], 2, ds1»	*	«[2, 0, 3, 1], 0, dr3»	=	«[0, 1, 2, 3], 2, ds2»
+«[1, 2, 0, 3], 1, ds0»	*	«[2, 1, 0, 3], 0, ds4»	=	«[0, 2, 1, 3], 1, dr0»
+«[3, 2, 0, 1], 3, dr3»	*	«[0, 1, 3, 2], 0, dr5»	=	«[3, 2, 1, 0], 3, dr0»
+«[2, 0, 3, 1], 0, dr5»	*	«[1, 0, 3, 2], 1, dr0»	=	«[0, 2, 1, 3], 1, dr1»
+«[3, 2, 0, 1], 0, dr7»	*	«[3, 1, 0, 2], 2, dr3»	=	«[1, 2, 3, 0], 2, dr2»
+"""
+```
+
+```python3
+
+# Operator ~ is another way of sampling.
+G = S(12)
+print(~G)
+"""
+[9, 1, 10, 6, 4, 5, 8, 7, 2, 3, 0, 11]
+"""
+```
+
+```python3
+
+# Manual element creation.
+last_perm_i = factorial(12) - 1
+a = Perm(i=last_perm_i, n=12)
+print("Last element of S35:", a)
+"""
+Last element of S35: [11, 10, 9, 8, 7, 6, 5, 4, 3, 2, 1, 0]
+"""
+```
+
+```python3
+
+# Inverse element. Group S4.
+a = Perm(i=21, n=4)
+b = Perm(i=17, n=4)
+print(a, "*", ~a, "=", (a * ~a).i, "=", a * ~a, "= identity")
+"""
+[1, 3, 2, 0] * [3, 0, 2, 1] = 0 = [0, 1, 2, 3] = identity
+"""
+```
+
+```python3
+
+print(a, "*", b, "=", a * b)
+"""
+[1, 3, 2, 0] * [1, 2, 3, 0] = [3, 2, 0, 1]
+"""
+```
+
+```python3
+
+print(a, "*", b, "*", ~b, "=", a * b * ~b, "= a")
+"""
+[1, 3, 2, 0] * [1, 2, 3, 0] * [3, 0, 1, 2] = [1, 3, 2, 0] = a
+"""
+```
+
+
+</p>
+</details>
+
+**Commutativity degree of groups**
+<details>
+<p>
+
+```python3
+
+from garoupa.algebra.cyclic import Z
+from garoupa.algebra.dihedral import D
+from garoupa.algebra.matrix.m import M
+
+
+def traverse(G):
+    i, count = G.order, G.order
+    for idx, a in enumerate(G.sorted()):
+        for b in list(G.sorted())[idx + 1 :]:
+            if a * b == b * a:
+                count += 2
+            i += 2
+    print(
+        f"|{G}| = ".rjust(20, " "),
+        f"{G.order}:".ljust(10, " "),
+        f"{count}/{i}:".rjust(15, " "),
+        f"  {G.bits} bits",
+        f"\t{100 * count / i} %",
+        sep="",
+    )
+
+
+# Dihedral
+traverse(D(8))
+"""
+             |D8| = 16:              112/256:  4.0 bits	43.75 %
+"""
+```
+
+```python3
+traverse(D(8) ^ 2)
+"""
+          |D8×D8| = 256:         12544/65536:  8.0 bits	19.140625 %
+"""
+```
+
+```python3
+
+# Z4!
+traverse(Z(4) * Z(3) * Z(2))
+"""
+       |Z4×Z3×Z2| = 24:              576/576:  4.584962500721157 bits	100.0 %
+"""
+```
+
+```python3
+
+# M 3x3 %4
+traverse(M(3, 4))
+
+# Large groups (sampling is needed).
+Gs = [D(8) ^ 3, D(8) ^ 4, D(8) ^ 5]
+for G in Gs:
+    i, count = 0, 0
+    for a, b in zip(G, G):
+        if a * b == b * a:
+            count += 1
+        if i >= 10_000:
+            break
+        i += 1
+    print(
+        f"|{G}| = ".rjust(20, " "),
+        f"{G.order}:".ljust(10, " "),
+        f"{count}/{i}:".rjust(15, " "),
+        f"  {G.bits} bits",
+        f"\t~{100 * count / i} %",
+        sep="",
+    )
+"""
+           |M3%4| = 64:            2560/4096:  6.0 bits	62.5 %
+       |D8×D8×D8| = 4096:          813/10000:  12.0 bits	~8.13 %
+    |D8×D8×D8×D8| = 65536:         378/10000:  16.0 bits	~3.78 %
+ |D8×D8×D8×D8×D8| = 1048576:       142/10000:  20.0 bits	~1.42 %
+"""
+```
+
+
+</p>
+</details>
+
+**Detect identity after many repetitions**
+<details>
+<p>
+
+```python3
+
+import operator
+from datetime import datetime
+from functools import reduce
+from math import log, inf
+from sys import argv
+
+from garoupa.algebra.dihedral import D
+from garoupa.algebra.symmetric import S
+
+example = len(argv) == 1 or (not argv[1].isdecimal() and argv[1][0] not in ["p", "s", "d"])
+
+primes = [5, 7, 11, 13, 17, 19, 23, 29, 31, 37, 41, 43, 47, 53, 59, 61, 67, 71, 73, 79, 83, 89, 97, 101, 103, 107,
+          109, 113, 127, 131, 137, 139, 149, 151, 157, 163, 167, 173, 179, 181, 191, 193, 197, 199, 211, 223, 227, 229,
+          233, 239, 241, 251, 257, 263, 269, 271, 277, 281, 283, 293, 307, 311, 313, 317, 331, 337, 347, 349, 353, 359,
+          367, 373, 379, 383, 389, 397, 401, 409, 419, 421, 431, 433, 439, 443, 449, 457, 461, 463, 467, 479, 487, 491,
+          499, 503, 509, 521, 523, 541, 547, 557, 563, 569, 571, 577, 587, 593, 599, 601, 607, 613, 617, 619, 631, 641,
+          643, 647, 653, 659, 661, 673, 677, 683, 691, 701, 709, 719, 727, 733, 739, 743, 751, 757, 761, 769, 773, 787,
+          797, 809, 811, 821, 823, 827, 829, 839, 853, 857, 859, 863, 877, 881, 883, 887, 907, 911, 919, 929, 937, 941,
+          947, 953, 967, 971, 977, 983, 991, 997, 1009]
+
+if example:
+    limit, sample = 30, 100
+    lst = []  # See *.
+    for n in primes[:5]:
+        lst.append(D(n, seed=n))
+    G = reduce(operator.mul, lst)
+else:
+    limit, sample = int(argv[2]), int(argv[3]) if len(argv) > 2 else 1_000_000_000_000
+    if argv[1] == "s25d":
+        G = S(25) * reduce(operator.mul, [D(n) for n in primes[:9]])
+    elif argv[1] == "s57":
+        G = S(57)
+    elif argv[1] == "p384":
+        G = reduce(operator.mul, [D(n) for n in primes[:51]])
+    elif argv[1] == "p64":
+        G = reduce(operator.mul, [D(n) for n in primes[:12]])
+    elif argv[1] == "p96":
+        G = reduce(operator.mul, [D(n) for n in primes[:16]])
+    elif argv[1] == "p128":
+        G = reduce(operator.mul, [D(n) for n in primes[:21]])
+    elif argv[1] == "p256":
+        G = reduce(operator.mul, [D(n) for n in primes[:37]])
+    elif argv[1] == "64":
+        G = reduce(operator.mul, [D(n) for n in range(5, 31, 2)])
+    elif argv[1] == "96":
+        G = reduce(operator.mul, [D(n) for n in range(5, 41, 2)])
+    elif argv[1] == "128":
+        G = reduce(operator.mul, [D(n) for n in range(5, 51, 2)])
+    else:
+        G = reduce(operator.mul, [D(n) for n in range(5, 86, 2)])
+
+print(f"{G.bits} bits   Pc: {G.comm_degree}  order: {G.order} {G}", flush=True)
+print("--------------------------------------------------------------", flush=True)
+for hist in G.sampled_orders(sample=sample, limit=limit):
+    tot = sum(hist.values())
+    bad = 0  # See *.
+    for k, v in hist.items():
+        if k[0] <= limit:
+            bad += v
+    print(hist, flush=True)
+    hist = hist.copy()
+    if (inf, inf) in hist:
+        del hist[(inf, inf)]
+    hist = {int((k[0] + k[1]) / 2): v for k, v in hist.items()}
+    print(
+        f"\nbits: {log(G.order, 2):.2f}  Pc: {G.comm_degree or -1:.2e}   a^<{limit}=0: {bad}/{tot} = {bad / tot:.2e}",
+        G,
+        G._pi_core(hist),
+        datetime.now().strftime("%d/%m/%Y %H:%M:%S"),
+        flush=True,
+    )
+# * -> [Explicit FOR due to autogeneration of README through eval]
+"""
+21.376617194973697 bits   Pc: 0.004113533525298232  order: 2722720 D5×D7×D11×D13×D17
+--------------------------------------------------------------
+{(-1, 10): 9, (9, 20): 7, (19, 30): 9, (inf, inf): 75}
+
+bits: 21.38  Pc: 4.11e-03   a^<30=0: 25/100 = 2.50e-01 D5×D7×D11×D13×D17 0.125 04/08/2023 18:47:38
+"""
+```
+
+
+</p>
+</details>
+
+**Tendence of commutativity on Mn**
+<details>
+<p>
+
+```python3
+from itertools import chain
+
+from garoupa.algebra.matrix.m import M
+from garoupa.algebra.matrix.m8bit import M8bit
+
+
+def traverse(G):
+    i, count = G.order, G.order
+    for idx, a in enumerate(G.sorted()):
+        for b in list(G.sorted())[idx + 1:]:
+            if a * b == b * a:
+                count += 2
+            i += 2
+    print(f"|{G}| = ".rjust(20, ' '),
+          f"{G.order}:".ljust(10, ' '),
+          f"{count}/{i}:".rjust(15, ' '), f"  {G.bits} bits",
+          f"\t{100 * count / i} %", sep="")
+
+
+M1_4 = map(M, range(1, 5))
+for G in chain(M1_4, [M8bit(), M(5)]):
+    traverse(G)
+# ...
+for G in map(M, range(6, 11)):
+    i, count = 0, 0
+    for a, b in zip(G, G):
+        if a * b == b * a:
+            count += 1
+        i += 1
+        if i >= 1_000_000:
+            break
+    print(f"|{G}| = ".rjust(20, ' '),
+          f"{G.order}:".ljust(10, ' '),
+          f"{count}/{i}:".rjust(15, ' '), f"  {G.bits} bits",
+          f"\t~{100 * count / i} %", sep="")
+
+"""
+|M1| = 1:                        1/1:  0 bits	100.0 %
+|M2| = 2:                        4/4:  1 bits	100.0 %
+|M3| = 8:                      40/64:  3 bits	62.5 %
+|M4| = 64:                 1024/4096:  6 bits	25.0 %
+|M8bit| = 256:              14848/65536:  8 bits	22.65625 %
+|M5| = 1024:           62464/1048576:  10 bits	5.95703125 %
+|M6| = 32768:              286/32768:  15 bits	0.872802734375 %
+|M7| = 2097152:          683/1000000:  21 bits	0.0683 %
+|M8| = 268435456:         30/1000000:  28 bits	0.003 %
+|M9| = 68719476736:        1/1000000:  36 bits	0.0001 %
+|M10| = 35184372088832:     0/1000000:  45 bits	0.0 %
+"""
+```
+</p>
+</details>
+
+**Groups benefit from methods from the module 'hosh'**
+<details>
+<p>
+
+```python3
+from garoupa.algebra.matrix import M
+
+m = ~M(23)
+print(repr(m.hosh))
+```
+<a href="https://github.com/davips/garoupa/blob/main/examples/7KDd8TiA3S11QTkUid2wy87DQIeGQ35vB1bsP5Y6DjZ.png">
+<img src="https://raw.githubusercontent.com/davips/garoupa/main/examples/7KDd8TiA3S11QTkUid2wy87DQIeGQ35vB1bsP5Y6DjZ.png" alt="Colored base-62 representation" width="380" height="18">
+</a>
+</p>
+</details>
+
+
+
+## Performance
+Computation time for the simple operations performed by GaROUPa can be considered negligible for most applications,
+since the order of magnitude of creating and operating identifiers is around a few μs:
+![img_6.png](https://raw.githubusercontent.com/davips/garoupa/main/examples/img_6.png)
+On the other hand, we estimate up to ~7x gains in speed when porting the core code to  _rust_.
+The package [hosh](https://pypi.org/project/hosh) was a faster implementation of an earlier version of GaROUPa,
+It will be updated to be fully compatible with current GaROUPa at major version `2.*.*`.
+As the performance of garoupa seems already very high, an updated 'rust' implementation might become unnecessary.
+Some parts of the algebra module need additional packages, they can be installed using:
+`poetry install -E full`
+
+## Grants
+This work was partially supported by Fapesp under supervision of
+Prof. André C. P. L. F. de Carvalho at CEPID-CeMEAI (Grants 2013/07375-0 – 2019/01735-0).
 
-setup(**setup_kwargs)
```

#### html2text {}

```diff
@@ -1,273 +1,260 @@
-# -*- coding: utf-8 -*- from setuptools import setup package_dir = \ {'':
-'src'} packages = \ ['garoupa', 'garoupa.algebra', 'garoupa.algebra.abs',
-'garoupa.algebra.cyclic', 'garoupa.algebra.dihedral', 'garoupa.algebra.matrix',
-'garoupa.algebra.product', 'garoupa.algebra.symmetric', 'garoupa.misc',
-'garoupa.misc.encoding'] package_data = \ {'': ['*']} install_requires = \
-['ansi2html>=1.6.0,<2.0.0', 'blake3>=0.2.0,<0.3.0', 'colored==1.4.2',
-'wheel>=0.37.0,<0.38.0'] extras_require = \ {'algebra': ['progress>=1.6,<2.0',
-'pathos>=0.2.8,<0.3.0'], 'experiments': ['bigfloat>=0.4.0,<0.5.0']}
-setup_kwargs = { 'name': 'garoupa', 'version': '2.220128.1', 'description':
-'Predictable operable hash-based identifiers and abstract algebra groups',
-'long_description': '![test](https://github.com/davips/garoupa/workflows/test/
-badge.svg)\n[![codecov](https://codecov.io/gh/davips/garoupa/branch/main/graph/
-badge.svg)](https://codecov.io/gh/davips/garoupa)\n\n[pypi]\n\n![Python
-version](https://img.shields.io/badge/python-3.8%20%7C%203.9-blue.svg)\n[!
-[license: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https:/
-/www.gnu.org/licenses/gpl-3.0)\n\n[![DOI](https://zenodo.org/badge/DOI/10.5281/
-zenodo.5501845.svg)](https://doi.org/10.5281/zenodo.5501845)\n[![arXiv](https:/
-/img.shields.io/badge/arXiv-2109.06028-b31b1b.svg?style=flat-square)](https://
-arxiv.org/abs/2109.06028)\n[![API documentation](https://img.shields.io/badge/
-doc-API%20%28auto%29-a0a0a0.svg)](https://davips.github.io/garoupa)\n\n\n#
-GaROUPa - Identification based on group theory\nThe identification module of
-this library is evolving at its successor library [hosh (code)](https://
-github.com/davips/hosh) / [hosh (package)](https://pypi.org/project/hosh).\nThe
-algebra module exists only here.\n \n\n\nGaROUPa solves the identification
-problem of multi-valued objects or sequences of events.
+Metadata-Version: 2.1 Name: garoupa Version: 2.220128.2 Summary: Predictable
+operable hash-based identifiers and abstract algebra groups License: GPL
+Author: davips Author-email: dpsabc@gmail.com Requires-Python: >=3.8
+Classifier: License :: Other/Proprietary License Classifier: Programming
+Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: algebra Provides-Extra: experiments Provides-Extra: native
+Requires-Dist: ansi2html (==1.6.0) Requires-Dist: bigfloat (>=0.4.0,<0.5.0) ;
+extra == "experiments" Requires-Dist: blake3 (>=0.2.0,<0.3.0) Requires-Dist:
+colored (==1.4.2) Requires-Dist: pathos (>=0.2.8,<0.3.0) ; extra == "algebra"
+Requires-Dist: progress (>=1.6,<2.0) ; extra == "algebra" Requires-Dist: wheel
+(>=0.37.0,<0.38.0) Description-Content-Type: text/markdown ![test](https://
+github.com/davips/garoupa/workflows/test/badge.svg) [![codecov](https://
+codecov.io/gh/davips/garoupa/branch/main/graph/badge.svg)](https://codecov.io/
+gh/davips/garoupa) [pypi] ![Python version](https://img.shields.io/badge/
+python-3.8%20%7C%203.9-blue.svg) [![license: GPL v3](https://img.shields.io/
+badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0) [![DOI]
+(https://zenodo.org/badge/DOI/10.5281/zenodo.5501845.svg)](https://doi.org/
+10.5281/zenodo.5501845) [![arXiv](https://img.shields.io/badge/arXiv-
+2109.06028-b31b1b.svg?style=flat-square)](https://arxiv.org/abs/2109.06028) [!
+[API documentation](https://img.shields.io/badge/doc-API%20%28auto%29-
+a0a0a0.svg)](https://davips.github.io/garoupa) [![Downloads](https://
+static.pepy.tech/badge/garoupa)](https://pepy.tech/project/garoupa) ![PyPI -
+Downloads](https://img.shields.io/pypi/dm/garoupa) # GaROUPa - Identification
+based on group theory The identification module of this library is evolving at
+its successor library [hosh (code)](https://github.com/davips/hosh) / [hosh
+(package)](https://pypi.org/project/hosh). The algebra module exists only here.
+GaROUPa solves the identification problem of multi-valued objects or sequences
+of events.
 This [Python library](https://pypi.org/project/garoupa) / [code](https://
 github.com/davips/garoupa) provides a reference implementation for the UT*.4
 specification presented [here](https://arxiv.org/abs/2109.06028). | ![fir0002
 flagstaffotos [at] gmail.com Canon 20D + Tamron 28-75mm f/2.8, GFDL 1.2 <http:/
 /www.gnu.org/licenses/old-licenses/fdl-1.2.html>, via Wikimedia Commons](https:
 //upload.wikimedia.org/wikipedia/commons/thumb/a/a7/
-Malabar_grouper_melb_aquarium.jpg/256px-Malabar_grouper_melb_aquarium.jpg)\n:--
------------------------:|:-------------------------:\n\nWe adopt a novel
-paradigm to universally unique identification (UUID), making identifiers
-deterministic and predictable, \neven before an object is generated by a
-(possibly costly) process. \nHere, data versioning and composition of
-processing steps are directly mapped as simple operations over identifiers.\nWe
-call each of the latter a Hosh, i.e., an identifier is an _**o**perable
-**h**a**sh**_.\n\nA complete implementation of the remaining ideas from the
-[paper](https://arxiv.org/abs/2109.06028) is provided in this\n[cacheable lazy
-dict](https://pypi.org/project/ldict/2.211016.3) which depends on GaROUPa and
-serves as an advanced usage example.\n
-\nA more robust (entirely rewritten) version is available in the package
-[idict](https://pypi.org/project/idict).\n\n## Overview\nA product of
-identifiers produces a new identifier as shown below, where sequences of bytes
-(`b"..."`) are passed to simulate binary objects to be hashed.\n\n![img.png]
-(https://raw.githubusercontent.com/davips/garoupa/main/examples/img.png) | New
+Malabar_grouper_melb_aquarium.jpg/256px-Malabar_grouper_melb_aquarium.jpg) :---
+----------------------:|:-------------------------: We adopt a novel paradigm
+to universally unique identification (UUID), making identifiers deterministic
+and predictable, even before an object is generated by a (possibly costly)
+process. Here, data versioning and composition of processing steps are directly
+mapped as simple operations over identifiers. We call each of the latter a
+Hosh, i.e., an identifier is an _**o**perable **h**a**sh**_. A complete
+implementation of the remaining ideas from the [paper](https://arxiv.org/abs/
+2109.06028) is provided in this [cacheable lazy dict](https://pypi.org/project/
+ldict/2.211016.3) which depends on GaROUPa and serves as an advanced usage
+example.
+A more robust (entirely rewritten) version is available in the package [idict]
+(https://pypi.org/project/idict). ## Overview A product of identifiers produces
+a new identifier as shown below, where sequences of bytes (`b"..."`) are passed
+to simulate binary objects to be hashed. ![img.png](https://
+raw.githubusercontent.com/davips/garoupa/main/examples/img.png) | New
 identifiers are easily
 created from the identity
 element `Ã¸`. Also available as `identity` for people
 or systems allergic to
-utf-8 encoding.\n-------------------------|-------------------------\n\n!
+utf-8 encoding. -------------------------|------------------------- !
 [img_1.png](https://raw.githubusercontent.com/davips/garoupa/main/examples/
-img_1.png) | Operations can be reverted by the inverse of the identifier.\n----
----------------------|-------------------------\n\n![img_2.png](https://
+img_1.png) | Operations can be reverted by the inverse of the identifier. -----
+--------------------|------------------------- ![img_2.png](https://
 raw.githubusercontent.com/davips/garoupa/main/examples/img_2.png) | Operations
 are associative.
 They are order-sensitive by default,
-in which case they are called _ordered_ ids.\n-------------------------|-------
-------------------\n\nHowever, order-insensitive (called _unordered_) and
-order-insensitive-among-themselves (called _hybrid_) identifiers are also
-available. | .\n-------------------------|-------------------------\n!
-[img_3.png](https://raw.githubusercontent.com/davips/garoupa/main/examples/
-img_3.png) | .\n\nThis is how they affect each other: | .\n--------------------
------|-------------------------\n![img_4.png](https://
-raw.githubusercontent.com/davips/garoupa/main/examples/img_4.png) | .\n\nThe
-chance of collision is determined by the number of possible identifiers of each
-type.\nSome versions are provided, e.g.: UT32.4, UT40.4 (default),
-UT64.4.\nThey can be easily implemented in other languages and are \nintended
-to be a specification on how to identify multi-valued objects and multi-step
-processes.\nUnordered ids use a very narrow range of the total number of
-identifiers.\nThis is not a problem as they are not very useful.\n\nOne use for
+in which case they are called _ordered_ ids. -------------------------|--------
+----------------- However, order-insensitive (called _unordered_) and order-
+insensitive-among-themselves (called _hybrid_) identifiers are also available.
+| . -------------------------|------------------------- ![img_3.png](https://
+raw.githubusercontent.com/davips/garoupa/main/examples/img_3.png) | . This is
+how they affect each other: | . -------------------------|---------------------
+---- ![img_4.png](https://raw.githubusercontent.com/davips/garoupa/main/
+examples/img_4.png) | . The chance of collision is determined by the number of
+possible identifiers of each type. Some versions are provided, e.g.: UT32.4,
+UT40.4 (default), UT64.4. They can be easily implemented in other languages and
+are intended to be a specification on how to identify multi-valued objects and
+multi-step processes. Unordered ids use a very narrow range of the total number
+of identifiers. This is not a problem as they are not very useful. One use for
 unordered ids could be the embedding of authorship or other metadata into an
 object without worrying about the timing, since the resulting id will remain
 the same, no matter when the unordered id is operated with the id of the object
-under construction. | . \n-------------------------|-------------------------
-\n![img_5.png](https://raw.githubusercontent.com/davips/garoupa/main/examples/
-img_5.png) | . \n\nConversely, hybrid ids are excelent to represent values in a
-data structure like a map, \nsince the order is not relevant when the consumer
-process looks up for keys, not indexes.\nConverselly, a chain of a data
+under construction. | . -------------------------|------------------------- !
+[img_5.png](https://raw.githubusercontent.com/davips/garoupa/main/examples/
+img_5.png) | . Conversely, hybrid ids are excelent to represent values in a
+data structure like a map, since the order is not relevant when the consumer
+process looks up for keys, not indexes. Converselly, a chain of a data
 processing functions usually implies one step is dependent on the result of the
-previous step.\nThis makes ordered ids the perfect fit to identify functions
-(and also their composition, as a consequence).\n\n### Relationships can also
-be represented\nHere is another possible use. ORCIDs are managed unique
-identifiers for researchers.\nThey can be directly used as digests to create
-operable identifiers.\nWe recommend the use of 40 digits to allow operations
-with SHA-1 hashes. \nThey are common in version control repositories among
-other uses.\n![img_orcid.png](https://raw.githubusercontent.com/davips/garoupa/
-main/examples/img_orcid.png)\n\nUnordered relationships are represented by
-hybrid ids.\nAutomatic transparent conversion between ORCID dashes by a
-hexdecimal character can be implemented in the future if needed.\n![img_orcid-
-comm.png](https://raw.githubusercontent.com/davips/garoupa/main/examples/
-img_orcid-comm.png)\n\n## More info\nAside from the [paper](https://arxiv.org/
-abs/2109.06028), [PyPI package](https://pypi.org/project/garoupa) \nand [GitHub
-repository](https://github.com/davips/garoupa), \none can find more
-information, at a higher level application perspective, \nin this presentation:
-\n![image](https://raw.githubusercontent.com/davips/garoupa/
-14cb45b888eb8a18ae093d200075c1a8a7e9cacb/examples/capa-slides-gdocs.png)\nA
+previous step. This makes ordered ids the perfect fit to identify functions
+(and also their composition, as a consequence). ### Relationships can also be
+represented Here is another possible use. ORCIDs are managed unique identifiers
+for researchers. They can be directly used as digests to create operable
+identifiers. We recommend the use of 40 digits to allow operations with SHA-
+1 hashes. They are common in version control repositories among other uses. !
+[img_orcid.png](https://raw.githubusercontent.com/davips/garoupa/main/examples/
+img_orcid.png) Unordered relationships are represented by hybrid ids. Automatic
+transparent conversion between ORCID dashes by a hexdecimal character can be
+implemented in the future if needed. ![img_orcid-comm.png](https://
+raw.githubusercontent.com/davips/garoupa/main/examples/img_orcid-comm.png) ##
+More info Aside from the [paper](https://arxiv.org/abs/2109.06028), [PyPI
+package](https://pypi.org/project/garoupa) and [GitHub repository](https://
+github.com/davips/garoupa), one can find more information, at a higher level
+application perspective, in this presentation: ![image](https://
+raw.githubusercontent.com/davips/garoupa/
+14cb45b888eb8a18ae093d200075c1a8a7e9cacb/examples/capa-slides-gdocs.png) A
 lower level perspective is provided in the [API documentation](https://
-davips.github.io/garoupa).\n\n## Python installation\n### from
-package\n```bash\n# Set up a virtualenv. \npython3 -m venv venv\nsource venv/
-bin/activate\n\n# Install from PyPI\npip install garoupa\n```\n\n### from
-source\n```bash\ngit clone https://github.com/davips/garoupa\ncd
-garoupa\npoetry install\n```\n\n### Examples\nSome usage examples.\n\n**Basic
-operations**\n\n
-\n\n```python3\nfrom garoupa import Hosh, Ã¸ # Ã¸ is a shortcut for identity
-(AltGr+O in most keyboards)\n\n# Hoshes (operable hash-based elements) can be
-multiplied.\na = Hosh(content=b"Some large binary content...")\nb = Hosh
+davips.github.io/garoupa). ## Python installation ### from package ```bash #
+Set up a virtualenv. python3 -m venv venv source venv/bin/activate # Install
+from PyPI pip install garoupa ``` ### from source ```bash git clone https://
+github.com/davips/garoupa cd garoupa poetry install ``` ### Examples Some usage
+examples. **Basic operations**
+```python3 from garoupa import Hosh, Ã¸ # Ã¸ is a shortcut for identity
+(AltGr+O in most keyboards) # Hoshes (operable hash-based elements) can be
+multiplied. a = Hosh(content=b"Some large binary content...") b = Hosh
 (content=b"Some other binary content. Might be, e.g., an action or another
-large content.")\nc = a * b\nprint(f"{a} * {b} =
-{c}")\n"""\n8CG9so9N1nQ59uNO8HGYcZ4ExQW5Haw4mErvw8m8 * 7N-L-10JS-H5DN0-
-BXW2e5ENWFQFVWswyz39t8s9 =
-z3EgxfisgqbNXBd0eqDuFiaTblBLA5ZAUbvEZgOh\n"""\n```\n\n```python3\nprint(~b)\n#
-Multiplication can be reverted by the inverse hosh. Zero is the identity
-hosh.\nprint(f"{b} * {~b} = {b * ~b} = 0")\n"""\nQ6OjmYZSJ8pB3ogBVMKBOxVp-
-oZ80czvtUrSyTzS\n7N-L-10JS-H5DN0-BXW2e5ENWFQFVWswyz39t8s9 *
-Q6OjmYZSJ8pB3ogBVMKBOxVp-oZ80czvtUrSyTzS =
-0000000000000000000000000000000000000000 = 0\n"""\n```\n\n```python3\n\nprint
-(f"{b} * {Ã¸} = {b * Ã¸} = b")\n"""\n7N-L-10JS-H5DN0-BXW2e5ENWFQFVWswyz39t8s9 *
+large content.") c = a * b print(f"{a} * {b} = {c}") """
+8CG9so9N1nQ59uNO8HGYcZ4ExQW5Haw4mErvw8m8 * 7N-L-10JS-H5DN0-
+BXW2e5ENWFQFVWswyz39t8s9 = z3EgxfisgqbNXBd0eqDuFiaTblBLA5ZAUbvEZgOh """ ```
+```python3 print(~b) # Multiplication can be reverted by the inverse hosh. Zero
+is the identity hosh. print(f"{b} * {~b} = {b * ~b} = 0") """
+Q6OjmYZSJ8pB3ogBVMKBOxVp-oZ80czvtUrSyTzS 7N-L-10JS-H5DN0-
+BXW2e5ENWFQFVWswyz39t8s9 * Q6OjmYZSJ8pB3ogBVMKBOxVp-oZ80czvtUrSyTzS =
+0000000000000000000000000000000000000000 = 0 """ ``` ```python3 print(f"{b} *
+{Ã¸} = {b * Ã¸} = b") """ 7N-L-10JS-H5DN0-BXW2e5ENWFQFVWswyz39t8s9 *
 0000000000000000000000000000000000000000 = 7N-L-10JS-H5DN0-
-BXW2e5ENWFQFVWswyz39t8s9 = b\n"""\n```\n\n```python3\n\nprint(f"{c} * {~b} = {c
-* ~b} = {a} = a")\n"""\nz3EgxfisgqbNXBd0eqDuFiaTblBLA5ZAUbvEZgOh *
+BXW2e5ENWFQFVWswyz39t8s9 = b """ ``` ```python3 print(f"{c} * {~b} = {c * ~b} =
+{a} = a") """ z3EgxfisgqbNXBd0eqDuFiaTblBLA5ZAUbvEZgOh *
 Q6OjmYZSJ8pB3ogBVMKBOxVp-oZ80czvtUrSyTzS =
 8CG9so9N1nQ59uNO8HGYcZ4ExQW5Haw4mErvw8m8 =
-8CG9so9N1nQ59uNO8HGYcZ4ExQW5Haw4mErvw8m8 = a\n"""\n```\n\n```python3\n\nprint
-(f"{~a} * {c} = {~a * c} = {b} = b")\n"""\nRNvSdLI-
-5RiBBGL8NekctiQofWUIeYvXFP3wvTFT * z3EgxfisgqbNXBd0eqDuFiaTblBLA5ZAUbvEZgOh =
-7N-L-10JS-H5DN0-BXW2e5ENWFQFVWswyz39t8s9 = 7N-L-10JS-H5DN0-
-BXW2e5ENWFQFVWswyz39t8s9 = b\n"""\n```\n\n```python3\n\n# Division is shorthand
-for reversion.\nprint(f"{c} / {b} = {c / b} =
-a")\n"""\nz3EgxfisgqbNXBd0eqDuFiaTblBLA5ZAUbvEZgOh / 7N-L-10JS-H5DN0-
-BXW2e5ENWFQFVWswyz39t8s9 = 8CG9so9N1nQ59uNO8HGYcZ4ExQW5Haw4mErvw8m8 =
-a\n"""\n```\n\n```python3\n\n# Hosh multiplication is not expected to be
-commutative.\nprint(f"{a * b} != {b *
-a}")\n"""\nz3EgxfisgqbNXBd0eqDuFiaTblBLA5ZAUbvEZgOh != wwSd0LaGvuV0W-yEOfgB-
-yVBMlNLA5ZAUbvEZgOh\n"""\n```\n\n```python3\n\n# Hosh multiplication is
-associative.\nprint(f"{a * (b * c)} = {(a * b) *
-c}")\n"""\nRuTcC4ZIr0Y1QLzYmytPRc087a8cbbW9Nj-gXxAz =
-RuTcC4ZIr0Y1QLzYmytPRc087a8cbbW9Nj-gXxAz\n"""\n```\n\n\n
-\n\n\n### Examples (abstract algebra)\nAlthough not the focus of the library,
-GaROUPa hosts also some niceties for group theory experimentation.\nSome
-examples are provided below.\n\n**Abstract algebra module**\n\n
-\n\n```python3\nfrom itertools import islice\nfrom math import
-factorial\n\nfrom garoupa.algebra.cyclic import Z\nfrom
-garoupa.algebra.dihedral import D\nfrom garoupa.algebra.symmetric import
-Perm\nfrom garoupa.algebra.symmetric import S\n\n# Direct product between:\n#
-symmetric group S4;\n# cyclic group Z5; and,\n# dihedral group D4.\nG = S(4) *
-Z(5) * D(4)\nprint(G)\n"""\nS4ÃZ5ÃD4\n"""\n```\n\n```python3\n\n# Operating
-over 5 sampled pairs.\nfor a, b in islice(zip(G, G), 0, 5):\n print(a, "*", b,
-"=", a * b, sep="\\t")\n"""\nÂ«[3, 0, 1, 2], 3, dr2Â»\t*\tÂ«[1, 2, 0, 3], 3,
-dr2Â»\t=\tÂ«[0, 1, 3, 2], 1, dr0Â»\nÂ«[1, 3, 0, 2], 3, ds3Â»\t*\tÂ«[1, 0, 3,
-2], 2, ds1Â»\t=\tÂ«[3, 1, 2, 0], 0, dr2Â»\nÂ«[2, 3, 0, 1], 2, ds7Â»\t*\tÂ«[1,
-0, 2, 3], 0, ds1Â»\t=\tÂ«[3, 2, 0, 1], 2, dr2Â»\nÂ«[2, 0, 3, 1], 2,
-ds3Â»\t*\tÂ«[0, 1, 3, 2], 0, dr5Â»\t=\tÂ«[2, 0, 1, 3], 2, ds2Â»\nÂ«[1, 2, 0,
-3], 0, dr5Â»\t*\tÂ«[2, 0, 1, 3], 3, ds6Â»\t=\tÂ«[0, 1, 2, 3], 3,
-ds3Â»\n"""\n```\n\n```python3\n\n# Operator ~ is another way of sampling.\nG =
-S(12)\nprint(~G)\n"""\n[10, 6, 5, 4, 9, 8, 1, 7, 0, 2, 3,
-11]\n"""\n```\n\n```python3\n\n# Manual element creation.\nlast_perm_i =
-factorial(12) - 1\na = Perm(i=last_perm_i, n=12)\nprint("Last element of S35:",
-a)\n"""\nLast element of S35: [11, 10, 9, 8, 7, 6, 5, 4, 3, 2, 1,
-0]\n"""\n```\n\n```python3\n\n# Inverse element. Group S4.\na = Perm(i=21,
-n=4)\nb = Perm(i=17, n=4)\nprint(a, "*", ~a, "=", (a * ~a).i, "=", a * ~a, "=
-identity")\n"""\n[1, 3, 2, 0] * [3, 0, 2, 1] = 0 = [0, 1, 2, 3] =
-identity\n"""\n```\n\n```python3\n\nprint(a, "*", b, "=", a * b)\n"""\n[1, 3,
-2, 0] * [1, 2, 3, 0] = [3, 2, 0, 1]\n"""\n```\n\n```python3\n\nprint(a, "*", b,
-"*", ~b, "=", a * b * ~b, "= a")\n"""\n[1, 3, 2, 0] * [1, 2, 3, 0] * [3, 0, 1,
-2] = [1, 3, 2, 0] = a\n"""\n```\n\n\n
-\n\n\n**Commutativity degree of groups**\n\n
-\n\n```python3\n\nfrom garoupa.algebra.cyclic import Z\nfrom
-garoupa.algebra.dihedral import D\nfrom garoupa.algebra.matrix.m import
-M\n\n\ndef traverse(G):\n i, count = G.order, G.order\n for idx, a in enumerate
-(G.sorted()):\n for b in list(G.sorted())[idx + 1 :]:\n if a * b == b * a:\n
-count += 2\n i += 2\n print(\n f"|{G}| = ".rjust(20, " "),\n f"{G.order}:
-".ljust(10, " "),\n f"{count}/{i}:".rjust(15, " "),\n f" {G.bits} bits",\n
-f"\\t{100 * count / i} %",\n sep="",\n )\n\n\n# Dihedral\ntraverse(D(8))\n"""\n
-|D8| = 16: 112/256: 4.0 bits\t43.75 %\n"""\n```\n\n```python3\ntraverse(D(8) ^
-2)\n"""\n |D8ÃD8| = 256: 12544/65536: 8.0 bits\t19.140625
-%\n"""\n```\n\n```python3\n\n# Z4!\ntraverse(Z(4) * Z(3) * Z(2))\n"""\n
-|Z4ÃZ3ÃZ2| = 24: 576/576: 4.584962500721157 bits\t100.0
-%\n"""\n```\n\n```python3\n\n# M 3x3 %4\ntraverse(M(3, 4))\n\n# Large groups
-(sampling is needed).\nGs = [D(8) ^ 3, D(8) ^ 4, D(8) ^ 5]\nfor G in Gs:\n i,
-count = 0, 0\n for a, b in zip(G, G):\n if a * b == b * a:\n count += 1\n if i
->= 10_000:\n break\n i += 1\n print(\n f"|{G}| = ".rjust(20, " "),\n f"
-{G.order}:".ljust(10, " "),\n f"{count}/{i}:".rjust(15, " "),\n f" {G.bits}
-bits",\n f"\\t~{100 * count / i} %",\n sep="",\n )\n"""\n |M3%4| = 64: 2560/
-4096: 6.0 bits\t62.5 %\n |D8ÃD8ÃD8| = 4096: 843/10000: 12.0 bits\t~8.43 %\n
-|D8ÃD8ÃD8ÃD8| = 65536: 396/10000: 16.0 bits\t~3.96 %\n |D8ÃD8ÃD8ÃD8ÃD8|
-= 1048576: 164/10000: 20.0 bits\t~1.64 %\n"""\n```\n\n\n
-\n\n\n**Detect identity after many repetitions**\n\n
-\n\n```python3\n\nimport operator\nfrom datetime import datetime\nfrom
-functools import reduce\nfrom math import log, inf\nfrom sys import
-argv\n\nfrom garoupa.algebra.dihedral import D\nfrom garoupa.algebra.symmetric
-import S\n\nexample = len(argv) == 1 or (not argv[1].isdecimal() and argv[1][0]
-not in ["p", "s", "d"])\n\nprimes = [5, 7, 11, 13, 17, 19, 23, 29, 31, 37, 41,
-43, 47, 53, 59, 61, 67, 71, 73, 79, 83, 89, 97, 101, 103, 107,\n 109, 113, 127,
-131, 137, 139, 149, 151, 157, 163, 167, 173, 179, 181, 191, 193, 197, 199, 211,
-223, 227, 229,\n 233, 239, 241, 251, 257, 263, 269, 271, 277, 281, 283, 293,
-307, 311, 313, 317, 331, 337, 347, 349, 353, 359,\n 367, 373, 379, 383, 389,
-397, 401, 409, 419, 421, 431, 433, 439, 443, 449, 457, 461, 463, 467, 479, 487,
-491,\n 499, 503, 509, 521, 523, 541, 547, 557, 563, 569, 571, 577, 587, 593,
-599, 601, 607, 613, 617, 619, 631, 641,\n 643, 647, 653, 659, 661, 673, 677,
-683, 691, 701, 709, 719, 727, 733, 739, 743, 751, 757, 761, 769, 773, 787,\n
-797, 809, 811, 821, 823, 827, 829, 839, 853, 857, 859, 863, 877, 881, 883, 887,
-907, 911, 919, 929, 937, 941,\n 947, 953, 967, 971, 977, 983, 991, 997,
-1009]\n\nif example:\n limit, sample = 30, 100\n lst = [] # See *.\n for n in
-primes[:5]:\n lst.append(D(n, seed=n))\n G = reduce(operator.mul, lst)\nelse:\n
-limit, sample = int(argv[2]), int(argv[3]) if len(argv) > 2 else
-1_000_000_000_000\n if argv[1] == "s25d":\n G = S(25) * reduce(operator.mul, [D
-(n) for n in primes[:9]])\n elif argv[1] == "s57":\n G = S(57)\n elif argv[1]
-== "p384":\n G = reduce(operator.mul, [D(n) for n in primes[:51]])\n elif argv
-[1] == "p64":\n G = reduce(operator.mul, [D(n) for n in primes[:12]])\n elif
-argv[1] == "p96":\n G = reduce(operator.mul, [D(n) for n in primes[:16]])\n
-elif argv[1] == "p128":\n G = reduce(operator.mul, [D(n) for n in primes[:
-21]])\n elif argv[1] == "p256":\n G = reduce(operator.mul, [D(n) for n in
-primes[:37]])\n elif argv[1] == "64":\n G = reduce(operator.mul, [D(n) for n in
-range(5, 31, 2)])\n elif argv[1] == "96":\n G = reduce(operator.mul, [D(n) for
-n in range(5, 41, 2)])\n elif argv[1] == "128":\n G = reduce(operator.mul, [D
-(n) for n in range(5, 51, 2)])\n else:\n G = reduce(operator.mul, [D(n) for n
-in range(5, 86, 2)])\n\nprint(f"{G.bits} bits Pc: {G.comm_degree} order:
-{G.order} {G}", flush=True)\nprint("-------------------------------------------
--------------------", flush=True)\nfor hist in G.sampled_orders(sample=sample,
-limit=limit):\n tot = sum(hist.values())\n bad = 0 # See *.\n for k, v in
-hist.items():\n if k[0] <= limit:\n bad += v\n print(hist, flush=True)\n hist =
-hist.copy()\n if (inf, inf) in hist:\n del hist[(inf, inf)]\n hist = {int((k[0]
-+ k[1]) / 2): v for k, v in hist.items()}\n print(\n f"\\nbits: {log(G.order,
-2):.2f} Pc: {G.comm_degree or -1:.2e} a^<{limit}=0: {bad}/{tot} = {bad /
-tot:.2e}",\n G,\n G._pi_core(hist),\n datetime.now().strftime("%d/%m/%Y %H:%M:
-%S"),\n flush=True,\n )\n# * -> [Explicit FOR due to autogeneration of README
-through eval]\n"""\n21.376617194973697 bits Pc: 0.004113533525298232 order:
-2722720 D5ÃD7ÃD11ÃD13ÃD17\n------------------------------------------------
---------------\n{(-1, 10): 9, (9, 20): 7, (19, 30): 9, (inf, inf): 75}\n\nbits:
-21.38 Pc: 4.11e-03 a^<30=0: 25/100 = 2.50e-01 D5ÃD7ÃD11ÃD13ÃD17 0.125 28/
-01/2022 14:15:50\n"""\n```\n\n\n
-\n\n\n**Tendence of commutativity on Mn**\n\n
-\n\n```python3\nfrom itertools import chain\n\nfrom garoupa.algebra.matrix.m
-import M\nfrom garoupa.algebra.matrix.m8bit import M8bit\n\n\ndef traverse(G):
-\n i, count = G.order, G.order\n for idx, a in enumerate(G.sorted()):\n for b
-in list(G.sorted())[idx + 1:]:\n if a * b == b * a:\n count += 2\n i += 2\n
-print(f"|{G}| = ".rjust(20, \' \'),\n f"{G.order}:".ljust(10, \' \'),\n f"
-{count}/{i}:".rjust(15, \' \'), f" {G.bits} bits",\n f"\\t{100 * count / i} %",
-sep="")\n\n\nM1_4 = map(M, range(1, 5))\nfor G in chain(M1_4, [M8bit(), M(5)]):
-\n traverse(G)\n# ...\nfor G in map(M, range(6, 11)):\n i, count = 0, 0\n for
-a, b in zip(G, G):\n if a * b == b * a:\n count += 1\n i += 1\n if i >=
-1_000_000:\n break\n print(f"|{G}| = ".rjust(20, \' \'),\n f"{G.order}:".ljust
-(10, \' \'),\n f"{count}/{i}:".rjust(15, \' \'), f" {G.bits} bits",\n f"\\t~
-{100 * count / i} %", sep="")\n\n"""\n|M1| = 1: 1/1: 0 bits\t100.0 %\n|M2| = 2:
-4/4: 1 bits\t100.0 %\n|M3| = 8: 40/64: 3 bits\t62.5 %\n|M4| = 64: 1024/4096: 6
-bits\t25.0 %\n|M8bit| = 256: 14848/65536: 8 bits\t22.65625 %\n|M5| = 1024:
-62464/1048576: 10 bits\t5.95703125 %\n|M6| = 32768: 286/32768: 15
-bits\t0.872802734375 %\n|M7| = 2097152: 683/1000000: 21 bits\t0.0683 %\n|M8| =
-268435456: 30/1000000: 28 bits\t0.003 %\n|M9| = 68719476736: 1/1000000: 36
-bits\t0.0001 %\n|M10| = 35184372088832: 0/1000000: 45 bits\t0.0 %\n"""\n```\n
-\n\n\n**Groups benefit from methods from the module \'hosh\'**\n\n
-\n\n```python3\nfrom garoupa.algebra.matrix import M\n\nm = ~M(23)\nprint(repr
-(m.hosh))\n```\n\n[Colored_base-62_representation]\n\n
-\n\n\n\n\n## Performance\nComputation time for the simple operations performed
-by GaROUPa can be considered negligible for most applications,\nsince the order
-of magnitude of creating and operating identifiers is around a few Î¼s:\n!
+8CG9so9N1nQ59uNO8HGYcZ4ExQW5Haw4mErvw8m8 = a """ ``` ```python3 print(f"{~a} *
+{c} = {~a * c} = {b} = b") """ RNvSdLI-5RiBBGL8NekctiQofWUIeYvXFP3wvTFT *
+z3EgxfisgqbNXBd0eqDuFiaTblBLA5ZAUbvEZgOh = 7N-L-10JS-H5DN0-
+BXW2e5ENWFQFVWswyz39t8s9 = 7N-L-10JS-H5DN0-BXW2e5ENWFQFVWswyz39t8s9 = b """ ```
+```python3 # Division is shorthand for reversion. print(f"{c} / {b} = {c / b} =
+a") """ z3EgxfisgqbNXBd0eqDuFiaTblBLA5ZAUbvEZgOh / 7N-L-10JS-H5DN0-
+BXW2e5ENWFQFVWswyz39t8s9 = 8CG9so9N1nQ59uNO8HGYcZ4ExQW5Haw4mErvw8m8 = a """ ```
+```python3 # Hosh multiplication is not expected to be commutative. print(f"{a
+* b} != {b * a}") """ z3EgxfisgqbNXBd0eqDuFiaTblBLA5ZAUbvEZgOh !=
+wwSd0LaGvuV0W-yEOfgB-yVBMlNLA5ZAUbvEZgOh """ ``` ```python3 # Hosh
+multiplication is associative. print(f"{a * (b * c)} = {(a * b) * c}") """
+RuTcC4ZIr0Y1QLzYmytPRc087a8cbbW9Nj-gXxAz = RuTcC4ZIr0Y1QLzYmytPRc087a8cbbW9Nj-
+gXxAz """ ```
+ ### Examples (abstract algebra) Although not the focus of the library, GaROUPa
+hosts also some niceties for group theory experimentation. Some examples are
+provided below. **Abstract algebra module**
+```python3 from itertools import islice from math import factorial from
+garoupa.algebra.cyclic import Z from garoupa.algebra.dihedral import D from
+garoupa.algebra.symmetric import Perm from garoupa.algebra.symmetric import S #
+Direct product between: # symmetric group S4; # cyclic group Z5; and, #
+dihedral group D4. G = S(4) * Z(5) * D(4) print(G) """ S4ÃZ5ÃD4 """ ```
+```python3 # Operating over 5 sampled pairs. for a, b in islice(zip(G, G), 0,
+5): print(a, "*", b, "=", a * b, sep="\t") """ Â«[1, 3, 0, 2], 2, ds1Â» * Â«[2,
+0, 3, 1], 0, dr3Â» = Â«[0, 1, 2, 3], 2, ds2Â» Â«[1, 2, 0, 3], 1, ds0Â» * Â«[2,
+1, 0, 3], 0, ds4Â» = Â«[0, 2, 1, 3], 1, dr0Â» Â«[3, 2, 0, 1], 3, dr3Â» * Â«[0,
+1, 3, 2], 0, dr5Â» = Â«[3, 2, 1, 0], 3, dr0Â» Â«[2, 0, 3, 1], 0, dr5Â» * Â«[1,
+0, 3, 2], 1, dr0Â» = Â«[0, 2, 1, 3], 1, dr1Â» Â«[3, 2, 0, 1], 0, dr7Â» * Â«[3,
+1, 0, 2], 2, dr3Â» = Â«[1, 2, 3, 0], 2, dr2Â» """ ``` ```python3 # Operator ~
+is another way of sampling. G = S(12) print(~G) """ [9, 1, 10, 6, 4, 5, 8, 7,
+2, 3, 0, 11] """ ``` ```python3 # Manual element creation. last_perm_i =
+factorial(12) - 1 a = Perm(i=last_perm_i, n=12) print("Last element of S35:",
+a) """ Last element of S35: [11, 10, 9, 8, 7, 6, 5, 4, 3, 2, 1, 0] """ ```
+```python3 # Inverse element. Group S4. a = Perm(i=21, n=4) b = Perm(i=17, n=4)
+print(a, "*", ~a, "=", (a * ~a).i, "=", a * ~a, "= identity") """ [1, 3, 2, 0]
+* [3, 0, 2, 1] = 0 = [0, 1, 2, 3] = identity """ ``` ```python3 print(a, "*",
+b, "=", a * b) """ [1, 3, 2, 0] * [1, 2, 3, 0] = [3, 2, 0, 1] """ ```
+```python3 print(a, "*", b, "*", ~b, "=", a * b * ~b, "= a") """ [1, 3, 2, 0] *
+[1, 2, 3, 0] * [3, 0, 1, 2] = [1, 3, 2, 0] = a """ ```
+ **Commutativity degree of groups**
+```python3 from garoupa.algebra.cyclic import Z from garoupa.algebra.dihedral
+import D from garoupa.algebra.matrix.m import M def traverse(G): i, count =
+G.order, G.order for idx, a in enumerate(G.sorted()): for b in list(G.sorted())
+[idx + 1 :]: if a * b == b * a: count += 2 i += 2 print( f"|{G}| = ".rjust(20,
+" "), f"{G.order}:".ljust(10, " "), f"{count}/{i}:".rjust(15, " "), f" {G.bits}
+bits", f"\t{100 * count / i} %", sep="", ) # Dihedral traverse(D(8)) """ |D8| =
+16: 112/256: 4.0 bits 43.75 % """ ``` ```python3 traverse(D(8) ^ 2) """
+|D8ÃD8| = 256: 12544/65536: 8.0 bits 19.140625 % """ ``` ```python3 # Z4!
+traverse(Z(4) * Z(3) * Z(2)) """ |Z4ÃZ3ÃZ2| = 24: 576/576: 4.584962500721157
+bits 100.0 % """ ``` ```python3 # M 3x3 %4 traverse(M(3, 4)) # Large groups
+(sampling is needed). Gs = [D(8) ^ 3, D(8) ^ 4, D(8) ^ 5] for G in Gs: i, count
+= 0, 0 for a, b in zip(G, G): if a * b == b * a: count += 1 if i >= 10_000:
+break i += 1 print( f"|{G}| = ".rjust(20, " "), f"{G.order}:".ljust(10, " "),
+f"{count}/{i}:".rjust(15, " "), f" {G.bits} bits", f"\t~{100 * count / i} %",
+sep="", ) """ |M3%4| = 64: 2560/4096: 6.0 bits 62.5 % |D8ÃD8ÃD8| = 4096: 813/
+10000: 12.0 bits ~8.13 % |D8ÃD8ÃD8ÃD8| = 65536: 378/10000: 16.0 bits ~3.78 %
+|D8ÃD8ÃD8ÃD8ÃD8| = 1048576: 142/10000: 20.0 bits ~1.42 % """ ```
+ **Detect identity after many repetitions**
+```python3 import operator from datetime import datetime from functools import
+reduce from math import log, inf from sys import argv from
+garoupa.algebra.dihedral import D from garoupa.algebra.symmetric import S
+example = len(argv) == 1 or (not argv[1].isdecimal() and argv[1][0] not in
+["p", "s", "d"]) primes = [5, 7, 11, 13, 17, 19, 23, 29, 31, 37, 41, 43, 47,
+53, 59, 61, 67, 71, 73, 79, 83, 89, 97, 101, 103, 107, 109, 113, 127, 131, 137,
+139, 149, 151, 157, 163, 167, 173, 179, 181, 191, 193, 197, 199, 211, 223, 227,
+229, 233, 239, 241, 251, 257, 263, 269, 271, 277, 281, 283, 293, 307, 311, 313,
+317, 331, 337, 347, 349, 353, 359, 367, 373, 379, 383, 389, 397, 401, 409, 419,
+421, 431, 433, 439, 443, 449, 457, 461, 463, 467, 479, 487, 491, 499, 503, 509,
+521, 523, 541, 547, 557, 563, 569, 571, 577, 587, 593, 599, 601, 607, 613, 617,
+619, 631, 641, 643, 647, 653, 659, 661, 673, 677, 683, 691, 701, 709, 719, 727,
+733, 739, 743, 751, 757, 761, 769, 773, 787, 797, 809, 811, 821, 823, 827, 829,
+839, 853, 857, 859, 863, 877, 881, 883, 887, 907, 911, 919, 929, 937, 941, 947,
+953, 967, 971, 977, 983, 991, 997, 1009] if example: limit, sample = 30, 100
+lst = [] # See *. for n in primes[:5]: lst.append(D(n, seed=n)) G = reduce
+(operator.mul, lst) else: limit, sample = int(argv[2]), int(argv[3]) if len
+(argv) > 2 else 1_000_000_000_000 if argv[1] == "s25d": G = S(25) * reduce
+(operator.mul, [D(n) for n in primes[:9]]) elif argv[1] == "s57": G = S(57)
+elif argv[1] == "p384": G = reduce(operator.mul, [D(n) for n in primes[:51]])
+elif argv[1] == "p64": G = reduce(operator.mul, [D(n) for n in primes[:12]])
+elif argv[1] == "p96": G = reduce(operator.mul, [D(n) for n in primes[:16]])
+elif argv[1] == "p128": G = reduce(operator.mul, [D(n) for n in primes[:21]])
+elif argv[1] == "p256": G = reduce(operator.mul, [D(n) for n in primes[:37]])
+elif argv[1] == "64": G = reduce(operator.mul, [D(n) for n in range(5, 31, 2)])
+elif argv[1] == "96": G = reduce(operator.mul, [D(n) for n in range(5, 41, 2)])
+elif argv[1] == "128": G = reduce(operator.mul, [D(n) for n in range(5, 51,
+2)]) else: G = reduce(operator.mul, [D(n) for n in range(5, 86, 2)]) print(f"
+{G.bits} bits Pc: {G.comm_degree} order: {G.order} {G}", flush=True) print("---
+-----------------------------------------------------------", flush=True) for
+hist in G.sampled_orders(sample=sample, limit=limit): tot = sum(hist.values())
+bad = 0 # See *. for k, v in hist.items(): if k[0] <= limit: bad += v print
+(hist, flush=True) hist = hist.copy() if (inf, inf) in hist: del hist[(inf,
+inf)] hist = {int((k[0] + k[1]) / 2): v for k, v in hist.items()} print
+( f"\nbits: {log(G.order, 2):.2f} Pc: {G.comm_degree or -1:.2e} a^<{limit}=0:
+{bad}/{tot} = {bad / tot:.2e}", G, G._pi_core(hist), datetime.now().strftime
+("%d/%m/%Y %H:%M:%S"), flush=True, ) # * -> [Explicit FOR due to autogeneration
+of README through eval] """ 21.376617194973697 bits Pc: 0.004113533525298232
+order: 2722720 D5ÃD7ÃD11ÃD13ÃD17 ------------------------------------------
+-------------------- {(-1, 10): 9, (9, 20): 7, (19, 30): 9, (inf, inf): 75}
+bits: 21.38 Pc: 4.11e-03 a^<30=0: 25/100 = 2.50e-01 D5ÃD7ÃD11ÃD13ÃD17 0.125
+04/08/2023 18:47:38 """ ```
+ **Tendence of commutativity on Mn**
+```python3 from itertools import chain from garoupa.algebra.matrix.m import M
+from garoupa.algebra.matrix.m8bit import M8bit def traverse(G): i, count =
+G.order, G.order for idx, a in enumerate(G.sorted()): for b in list(G.sorted())
+[idx + 1:]: if a * b == b * a: count += 2 i += 2 print(f"|{G}| = ".rjust(20, '
+'), f"{G.order}:".ljust(10, ' '), f"{count}/{i}:".rjust(15, ' '), f" {G.bits}
+bits", f"\t{100 * count / i} %", sep="") M1_4 = map(M, range(1, 5)) for G in
+chain(M1_4, [M8bit(), M(5)]): traverse(G) # ... for G in map(M, range(6, 11)):
+i, count = 0, 0 for a, b in zip(G, G): if a * b == b * a: count += 1 i += 1 if
+i >= 1_000_000: break print(f"|{G}| = ".rjust(20, ' '), f"{G.order}:".ljust(10,
+' '), f"{count}/{i}:".rjust(15, ' '), f" {G.bits} bits", f"\t~{100 * count / i}
+%", sep="") """ |M1| = 1: 1/1: 0 bits 100.0 % |M2| = 2: 4/4: 1 bits 100.0 %
+|M3| = 8: 40/64: 3 bits 62.5 % |M4| = 64: 1024/4096: 6 bits 25.0 % |M8bit| =
+256: 14848/65536: 8 bits 22.65625 % |M5| = 1024: 62464/1048576: 10 bits
+5.95703125 % |M6| = 32768: 286/32768: 15 bits 0.872802734375 % |M7| = 2097152:
+683/1000000: 21 bits 0.0683 % |M8| = 268435456: 30/1000000: 28 bits 0.003 %
+|M9| = 68719476736: 1/1000000: 36 bits 0.0001 % |M10| = 35184372088832: 0/
+1000000: 45 bits 0.0 % """ ```
+ **Groups benefit from methods from the module 'hosh'**
+```python3 from garoupa.algebra.matrix import M m = ~M(23) print(repr(m.hosh))
+``` [Colored_base-62_representation]
+ ## Performance Computation time for the simple operations performed by GaROUPa
+can be considered negligible for most applications, since the order of
+magnitude of creating and operating identifiers is around a few Î¼s: !
 [img_6.png](https://raw.githubusercontent.com/davips/garoupa/main/examples/
-img_6.png)\nOn the other hand, we estimate up to ~7x gains in speed when
-porting the core code to _rust_.\nThe package [hosh](https://pypi.org/project/
-hosh) was a faster implementation of an earlier version of GaROUPa,\nIt will be
-updated to be fully compatible with current GaROUPa at major version
-`2.*.*`.\nAs the performance of garoupa seems already very high, an updated
-\'rust\' implementation might become unnecessary.\nSome parts of the algebra
-module need additional packages, they can be installed using:\n`poetry install
--E full`\n\n## Grants\nThis work was partially supported by Fapesp under
-supervision of\nProf. AndrÃ© C. P. L. F. de Carvalho at CEPID-CeMEAI (Grants
-2013/07375-0 â 2019/01735-0).\n', 'author': 'davips', 'author_email':
-'dpsabc@gmail.com', 'maintainer': None, 'maintainer_email': None, 'url': None,
-'package_dir': package_dir, 'packages': packages, 'package_data': package_data,
-'install_requires': install_requires, 'extras_require': extras_require,
-'python_requires': '>=3.8', } setup(**setup_kwargs)
+img_6.png) On the other hand, we estimate up to ~7x gains in speed when porting
+the core code to _rust_. The package [hosh](https://pypi.org/project/hosh) was
+a faster implementation of an earlier version of GaROUPa, It will be updated to
+be fully compatible with current GaROUPa at major version `2.*.*`. As the
+performance of garoupa seems already very high, an updated 'rust'
+implementation might become unnecessary. Some parts of the algebra module need
+additional packages, they can be installed using: `poetry install -E full` ##
+Grants This work was partially supported by Fapesp under supervision of Prof.
+AndrÃ© C. P. L. F. de Carvalho at CEPID-CeMEAI (Grants 2013/07375-0 â 2019/
+01735-0).
```

