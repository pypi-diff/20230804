# Comparing `tmp/padic-0.2.2.1.tar.gz` & `tmp/padic-0.2.3.tar.gz`

## Comparing `padic-0.2.2.1.tar` & `padic-0.2.3.tar`

### file list

```diff
@@ -1,10 +1,12 @@
--rw-r--r--   0        0        0     5868 2020-02-02 00:00:00.000000 padic-0.2.2.1/2.2.1/padic-0.2.1-py3-none-any.whl
--rw-r--r--   0        0        0     5069 2020-02-02 00:00:00.000000 padic-0.2.2.1/2.2.1/padic-0.2.1.tar.gz
--rw-r--r--   0        0        0     5871 2020-02-02 00:00:00.000000 padic-0.2.2.1/2.2.2/padic-0.2.2-py3-none-any.whl
--rw-r--r--   0        0        0     5072 2020-02-02 00:00:00.000000 padic-0.2.2.1/2.2.2/padic-0.2.2.tar.gz
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 padic-0.2.2.1/src/padic/__init__.py
--rw-r--r--   0        0        0    13882 2020-02-02 00:00:00.000000 padic-0.2.2.1/src/padic/padic.py
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 padic-0.2.2.1/LICENSE.txt
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 padic-0.2.2.1/README.md
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 padic-0.2.2.1/pyproject.toml
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 padic-0.2.2.1/PKG-INFO
+-rw-r--r--   0        0        0     5895 2020-02-02 00:00:00.000000 padic-0.2.3/0.2.2.1/padic-0.2.2.1-py3-none-any.whl
+-rw-r--r--   0        0        0    21573 2020-02-02 00:00:00.000000 padic-0.2.3/0.2.2.1/padic-0.2.2.1.tar.gz
+-rw-r--r--   0        0        0     5868 2020-02-02 00:00:00.000000 padic-0.2.3/2.2.1/padic-0.2.1-py3-none-any.whl
+-rw-r--r--   0        0        0     5069 2020-02-02 00:00:00.000000 padic-0.2.3/2.2.1/padic-0.2.1.tar.gz
+-rw-r--r--   0        0        0     5871 2020-02-02 00:00:00.000000 padic-0.2.3/2.2.2/padic-0.2.2-py3-none-any.whl
+-rw-r--r--   0        0        0     5072 2020-02-02 00:00:00.000000 padic-0.2.3/2.2.2/padic-0.2.2.tar.gz
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 padic-0.2.3/src/padic/__init__.py
+-rw-r--r--   0        0        0    15793 2020-02-02 00:00:00.000000 padic-0.2.3/src/padic/padic.py
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 padic-0.2.3/LICENSE.txt
+-rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 padic-0.2.3/README.md
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 padic-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 padic-0.2.3/PKG-INFO
```

### Comparing `padic-0.2.2.1/2.2.1/padic-0.2.1-py3-none-any.whl` & `padic-0.2.3/2.2.1/padic-0.2.1-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `padic-0.2.2.1/2.2.1/padic-0.2.1.tar.gz` & `padic-0.2.3/2.2.1/padic-0.2.1.tar.gz`

 * *Files identical despite different names*

### Comparing `padic-0.2.2.1/2.2.2/padic-0.2.2-py3-none-any.whl` & `padic-0.2.3/2.2.2/padic-0.2.2-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `padic-0.2.2.1/2.2.2/padic-0.2.2.tar.gz` & `padic-0.2.3/2.2.2/padic-0.2.2.tar.gz`

 * *Files identical despite different names*

### Comparing `padic-0.2.2.1/src/padic/padic.py` & `padic-0.2.3/src/padic/padic.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,65 +1,69 @@
+# Version 0.2.3
 from __future__ import annotations
 from typing import Callable
 from numpy import base_repr
 from numpy.polynomial import Polynomial
 from functools import lru_cache
 import sys
 
 sys.setrecursionlimit(2000)
 
 
 class Padic:
-    # numbers are compared modulo p**PRECISION. Doesn't affect precision of computations.
+    # Numbers are compared modulo p**PRECISION. Doesn't affect precision of computations.
     PRECISION: int = 32
 
-    # default precision for integer to Padic conversion. Please note that this may affect
-    # some arithmetic operations and other functions as for example x: Padic *= 7 converts
-    # 7 to Padic before performing the multiplication
+    # Default precision for integer to Padic conversion.
+    # This also may affect precision of some arithmetic operations.
     INTEGER_PRECISION: int = 64
 
-    # default value of p used in some functions for convenience so that one doesn't have to
+    # Default value of p used in some functions for convenience so that one doesn't have to
     # keep inputting same prime over and over again. Can be set by set_prime function. Ignored
     # if None.
     DEFAULT_PRIME: int | None = None
 
+    # Determines how many digits before period (on left) of a number will be displayed by default.
+    # If set to None displays all of them. Should be non-negative.
+    DISPLAY_PRECISION: int | None = None
+
     # Represents p-adic number as an interval p^v*s + O(p^N)
-    def __init__(self, N: int, v: int, s: int, p: int | None = None):
+    def __init__(self, N: int, v: int, s: int, p: int | None = None) -> None:
         if p is None:
             p = Padic.DEFAULT_PRIME
         # Assumes p is prime
         # Assumes s _|_ p or s == 0
         if v >= N:
             s = 0
         if s == 0:
             v = N
         self.N: int = N
         self.v: int = v
-        self.s: int = s % p**(N - v)
+        self.s: int = s % p ** (N - v)
         self.p: int = p
 
     def __abs__(self) -> int | float:
-        return self.p**(-self.v)
+        return self.p ** (-self.v)
 
     def __eq__(self, other: Padic | int) -> bool:
         diff = self - other
         return diff.v >= Padic.PRECISION or diff.v == diff.N
 
     def __add__(self, other: Padic | int | float) -> Padic:
         if isinstance(other, float) and other == 0.0:
             return self
         if isinstance(other, Padic) and self.p == other.p:
             v_diff = self.v - other.v
             if v_diff > 0:
-                return Padic(min(self.N, other.N), other.v, (self.p**v_diff)*self.s + other.s, self.p)
+                return Padic(min(self.N, other.N), other.v, (self.p ** v_diff) * self.s + other.s, self.p)
             if v_diff < 0:
-                return Padic(min(self.N, other.N), self.v, self.s + (self.p**(-v_diff))*other.s, self.p)
+                return Padic(min(self.N, other.N), self.v, self.s + (self.p ** (-v_diff)) * other.s, self.p)
             return Padic.from_int(self.s + other.s, self.p, min(self.N, other.N), self.v)
         if isinstance(other, int):
-            return self + Padic.from_int(other, self.p)
+            return self + Padic.from_int(other, self.p, self.N)
         else:
             raise RuntimeError(f"Can't add {str(self)} to {str(other)}")
 
     # This may look weird. That's a bypass to make class work with evaluation of numpy polynomials
     def __radd__(self, other: int | float) -> Padic:
         if isinstance(other, float) and other == 0.0:
             return self
@@ -74,96 +78,124 @@
     def __rsub__(self, other: int) -> Padic:
         return -(self - other)
 
     def __mul__(self, other: Padic | int | float) -> Padic:
         if isinstance(other, float) and other == 1.0:
             return self
         if isinstance(other, Padic) and self.p == other.p:
-            return Padic(min(self.v + other.N, other.s + self.N), self.v + other.v, self.s * other.s, self.p)
+            return Padic(min(self.v + other.N, other.v + self.N), self.v + other.v, self.s * other.s, self.p)
         if isinstance(other, int):
-            return self * Padic.from_int(other, self.p)
+            return self * Padic.from_int(other, self.p, self.N + Padic.val(other, self.p) - Padic.val(self))
         else:
-            raise RuntimeError(f"Can't multiply {str(self)} with {str(other)}")
+            raise RuntimeError(f"Can't multiply {self} with {other}")
 
     # This may look weird. That's a bypass to make class work with evaluation of numpy polynomials
     def __rmul__(self, other: int | float) -> Padic:
         if isinstance(other, float) and other == 1.0:
             return self
         return self * other
 
     def __truediv__(self, other: Padic | int) -> Padic:
         if isinstance(other, Padic) and self.p == other.p:
             N = min(self.v + other.N - 2 * other.v, self.N - other.v)
             v = self.v - other.v
-            s = self.s * pow(other.s, -1, self.p**N)
+            s = self.s * pow(other.s, -1, self.p ** (N - v))
             return Padic(N, v, s, self.p)
         if isinstance(other, int):
-            return self / Padic.from_int(other, self.p)
+            return self / Padic.from_int(other, self.p, self.N + Padic.val(other, self.p) - Padic.val(self))
         else:
-            raise RuntimeError(f"Can't divide {str(self)} by {str(other)}")
+            raise RuntimeError(f"Can't divide {self} by {other}")
 
     def __rtruediv__(self, other: int) -> Padic:
-        return Padic.from_int(other, self.p) / self
+        return Padic.from_int(other, self.p, self.N + Padic.val(other, self.p) - Padic.val(self)) / self
 
     def __mod__(self, other: Padic | int) -> Padic:
         if Padic.val(self) >= Padic.val(other, self.p):
             return Padic(max(Padic.INTEGER_PRECISION, self.N), max(Padic.INTEGER_PRECISION, self.N), 0, self.p)
-        return Padic.from_int(other.s % self.p**(Padic.val(other, self.p) - Padic.val(self)),
+        return Padic.from_int(self.s % self.p ** (min(Padic.val(other, self.p) - Padic.val(self), self.N)),
                               self.p, max(Padic.INTEGER_PRECISION, self.N), Padic.val(self))
 
     def __rmod__(self, other: int) -> Padic:
-        return Padic.from_int(other, self.p) % self
+        return Padic.from_int(other, self.p, self.v) % self
 
     def __floordiv__(self, other: Padic | int) -> Padic:
-        return (self - self % other)/other
+        return (self - self % other) / other
 
     def __rfloordiv__(self, other: int) -> Padic:
-        return Padic.from_int(other, self.p) // self
+        return (other - other % self) / self
 
     def __str__(self) -> str:
         if self.p > 31:
             return f"{self.p}-adic + O({self.p}^{self.N})"
         out = base_repr(self.s, self.p)
         if self.v >= 0:
-            return out + ''.join(['0']*self.v) + f' + O({self.p}^{self.N})'
+            if Padic.DISPLAY_PRECISION is None:
+                return out + ''.join(['0'] * self.v) + f' + O({self.p}^{self.N})'
+            num = out + ''.join(['0'] * self.v)
+            # Space is a workaround space cuz now (08.2023) 3-year-old bug causes pycharm not to
+            # print ... if at the start of the string...
+            return ((" ..." if Padic.DISPLAY_PRECISION < len(num) else "") +
+                    num[-Padic.DISPLAY_PRECISION:] + f' + O({self.p}^{self.N})')
         else:
-            return out[:self.v] + '.' + out[self.v:] + f' + O({self.p}^{self.N})'
+            if Padic.DISPLAY_PRECISION is None:
+                return out[:self.v] + '.' + out[self.v:] + f' + O({self.p}^{self.N})'
+            num = out[:self.v]
+            # Same comment as above.
+            return ((" ..." if Padic.DISPLAY_PRECISION < len(num) else "") +
+                    num[-Padic.DISPLAY_PRECISION:] + '.' + out[self.v:] + f' + O({self.p}^{self.N})')
+
+    def __repr__(self) -> str:
+        return str(self)
+
+    def __format__(self, format_spec: str) -> str:
+        if format_spec[0] == '.':
+            digits = int(format_spec[1:])
+            prev, Padic.DISPLAY_PRECISION = Padic.DISPLAY_PRECISION, digits
+            out = str(self)
+            Padic.DISPLAY_PRECISION = prev
+            return out
+        if format_spec in ['exact', 'all', 'a', '.None']:
+            prev, Padic.DISPLAY_PRECISION = Padic.DISPLAY_PRECISION, None
+            out = str(self)
+            Padic.DISPLAY_PRECISION = prev
+            return out
+        return str(self)
 
     # Currently works for integer powers only. This may change in the future.
     # Modulo argument is for now ignored.
-    def __pow__(self, power: int, modulo=None):
+    def __pow__(self, power: int, modulo=None) -> Padic:
         assert isinstance(power, int)
         if power == 0:
-            return Padic.from_int(1, self.p)
+            return Padic.from_int(1, self.p, max(Padic.INTEGER_PRECISION, self.N))
         if power == 1:
             return Padic(self.N, self.v, self.s, self.p)
         if power == -1:
-            return 1/self
-        return self**(power//2) * self**(power//2) * self**(power % 2)
+            return 1 / self
+        return self ** (power // 2) * self ** (power // 2) * self ** (power % 2)
 
     def __lshift__(self, other: int) -> Padic:
         assert isinstance(other, int)
-        return self.p**other * self
+        return self.p ** other * self
 
     def __rshift__(self, other: int) -> Padic:
         assert isinstance(other, int)
-        return self//self.p**other
+        return self // self.p ** other
 
     # Warning! Center isn't necessarily an integer!
     def center(self) -> int | float:
         return self.s * (self.p ** self.v)
 
     @staticmethod
     # No default prime on purpose.
     def val(n: Padic | int, p: int | None = None) -> int:
         if isinstance(n, Padic) and (n.p == p or p is None):
             return n.v
         if isinstance(n, int) and p is not None:
             if n == 0:
-                return 10**9 + 1
+                return 10 ** 9 + 1
             out = 0
             while n % p == 0:
                 out += 1
                 n //= p
             return out
         raise RuntimeError("Valuation undefined for " + str(n), type(n))
 
@@ -228,20 +260,16 @@
     def from_frac(a: int, b: int, p: int | None = None, N: int = None) -> Padic:
         if p is None:
             p = Padic.DEFAULT_PRIME
         if N is None:
             N = Padic.INTEGER_PRECISION
         return Padic.from_int(a, p, N) / Padic.from_int(b, p, N)
 
-    @staticmethod
-    def set_prime(p: int):
-        Padic.DEFAULT_PRIME = p
-
 
-def gcd(a: int, b: int):
+def gcd(a: int, b: int) -> int:
     if b == 0:
         return a
     return gcd(b, a % b)
 
 
 class Rational:
     def __init__(self, p, q):
@@ -264,15 +292,17 @@
     def __neg__(self):
         return Rational(-self.num, self.den)
 
     def __str__(self):
         return str(self.num) + "/" + str(self.den)
 
 
-def series(a: Callable[[int], int | Rational | Padic], n: int, z='p'):  # To be changed
+def series(a: Callable[[int], int | Rational | Padic], n: int, z='p') -> \
+                                    Callable[[int | Rational], Rational] \
+                                    | Callable[[int | Padic, int | None], Padic]:
     def u1(x: int | Rational):
         if isinstance(x, int):
             x = Rational(x, 1)
         out = Rational(0, 1)
         for k in range(n, -1, -1):
             out *= x
             out += a(k)
@@ -298,56 +328,56 @@
     return n * factorial(n - 1) if n else 1
 
 
 @lru_cache(maxsize=1000)
 def binomial_coeff(a: Padic | int, b: int, p: int | None = None) -> Padic:
     if p is None:
         p = a.p
-    return Padic.from_int(1, p) if b == 0 else binomial_coeff(a, b - 1)/b * (a-b + 1)
+    return Padic.from_int(1, p) if b == 0 else binomial_coeff(a, b - 1) / b * (a - b + 1)
 
 
 # Convergent for x = 1 + O(p)
-def log(x: int | Padic, p: int | None = None, N=100):
+def log(x: int | Padic, p: int | None = None, N: int = 100) -> Padic:
     if p is None:
         p = x.p
-    return -series(lambda n: Padic.from_frac(1, n, p) if n != 0 else Padic.from_int(0, 2), N)(1-x)
+    return -series(lambda n: Padic.from_frac(1, n, p) if n != 0 else Padic.from_int(0, 2), N)(1 - x)
 
 
 # Convergent for |x|_p < p^{-1/{p-1}}
-def exp(x: int | Padic, p: int | None = None, N=100):
+def exp(x: int | Padic, p: int | None = None, N: int = 100) -> Padic:
     if p is None:
         p = x.p
     return series(lambda n: Padic.from_frac(1, factorial(n), p), N)(x)
 
 
 # Convergent for |x|_p < p^{-1/{p-1}}
-def sin(x: int | Padic, p: int | None = None, N=100):
+def sin(x: int | Padic, p: int | None = None, N: int = 100) -> Padic:
     if p is None:
         p = x.p
     return series(lambda n: Padic.from_frac(1, factorial(n), p) * (-1) ** ((n - 1) // 2) if n % 2 else 0, N)(x)
 
 
 # Convergent for |x|_p < p^{-1/{p-1}}
-def cos(x: int | Padic, p: int | None = None, N=100):
+def cos(x: int | Padic, p: int | None = None, N: int = 100) -> Padic:
     if p is None:
         p = x.p
     return series(lambda n: Padic.from_frac(1, factorial(n), p) * (-1) ** ((n + 1) // 2) if (n - 1) % 2 else 0, N)(x)
 
 
 # Convergence radius dependent on p and a
-def binomial(x: int | Padic, a: int | Padic, p: int | None = None, N=100):
+def binomial(x: int | Padic, a: int | Padic, p: int | None = None, N: int = 100) -> Padic:
     if p is None:
         p = x.p
-    return series(lambda n: binomial_coeff(a, n, p), N)(1-x)
+    return series(lambda n: binomial_coeff(a, n, p), N)(1 - x)
 
 
 # Finds approximate root of a polynomial
 # or doesn't.
 # Currently checks for roots in Z_p only.
-def find_approx_root(poly: Polynomial, p: int | None = None, depth: int = 5):
+def find_approx_root(poly: Polynomial, p: int | None = None, depth: int = 5) -> Padic:
     der = poly.deriv()
 
     def check_path(x, i):
         v1 = Padic.val(poly(x), p)
         v2 = Padic.val(der(x), p)
         return 1 if v1 > 2 * v2 else 2 if v1 <= i else 0
 
@@ -357,15 +387,15 @@
     current_paths = [Padic.from_int(0, p)]
     ppow = 1
     for i in range(depth):
         previous_paths = current_paths
         current_paths = []
         for path in previous_paths:
             for k in range(p):
-                current_paths.append(path + k*ppow)
+                current_paths.append(path + k * ppow)
         for path in current_paths:
             res = check_path(path, i)
             if res == 1:
                 return path
             if res == 2:
                 current_paths.remove(path)
         ppow *= p
@@ -373,19 +403,19 @@
 
 
 # Calculates polynomial root closest to a given approximate root
 # In case no root is given returns arbitrary root or raises NoRoot exception.
 # Doesn't verify correctness of given approximate root.
 # Note that in fact GHL (Generalised Hensel Lemma) for polynomial roots is used
 # Currently checks for roots in Z_p only
-def hensel(poly: Polynomial, approx: Padic | int | None = None, p: int | None = None, N=100):
+def hensel(poly: Polynomial, approx: Padic | int | None = None, p: int | None = None, N: int = 100) -> Padic:
     if p is None:
         p = approx.p
     if approx is None:
         approx = find_approx_root(poly)
     if isinstance(approx, int):
         approx = Padic.from_int(approx, p)
     der = poly.deriv()
     out = approx
     for _ in range(N):
-        out -= poly(out)/der(out)
+        out -= poly(out) / der(out)
     return out
```

### Comparing `padic-0.2.2.1/LICENSE.txt` & `padic-0.2.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `padic-0.2.2.1/pyproject.toml` & `padic-0.2.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "padic"
-version = "0.2.2.1"
+version = "0.2.3"
 authors = [
   { name="MRaczuk", email="mraczuk@gmail.com" },
 ]
 description = "Package implementing p-adic numbers"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

