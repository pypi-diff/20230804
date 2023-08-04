# Comparing `tmp/mofmt-0.2.1-py3-none-any.whl.zip` & `tmp/mofmt-0.2.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 77271 bytes, number of entries: 26
--rw-r--r--  2.0 fat      845 b- defN 80-Jan-01 00:00 CHANGELOG.md
+Zip file size: 77340 bytes, number of entries: 26
+-rw-r--r--  2.0 fat      986 b- defN 80-Jan-01 00:00 CHANGELOG.md
 -rw-r--r--  2.0 fat        0 b- defN 80-Jan-01 00:00 mofmt/__init__.py
 -rw-r--r--  2.0 fat       35 b- defN 80-Jan-01 00:00 mofmt/__main__.py
 -rw-r--r--  2.0 fat       70 b- defN 80-Jan-01 00:00 mofmt/collecting/__init__.py
--rw-r--r--  2.0 fat     3823 b- defN 80-Jan-01 00:00 mofmt/collecting/collector.py
+-rw-r--r--  2.0 fat     3855 b- defN 80-Jan-01 00:00 mofmt/collecting/collector.py
 -rw-r--r--  2.0 fat      146 b- defN 80-Jan-01 00:00 mofmt/io/__init__.py
 -rw-r--r--  2.0 fat     1256 b- defN 80-Jan-01 00:00 mofmt/io/io.py
 -rw-r--r--  2.0 fat     1234 b- defN 80-Jan-01 00:00 mofmt/mofmt.py
 -rw-r--r--  2.0 fat      116 b- defN 80-Jan-01 00:00 mofmt/parsing/__init__.py
 -rw-r--r--  2.0 fat      171 b- defN 80-Jan-01 00:00 mofmt/parsing/generated/__init__.py
 -rw-r--r--  2.0 fat    41279 b- defN 80-Jan-01 00:00 mofmt/parsing/generated/Modelica.interp
 -rw-r--r--  2.0 fat   413159 b- defN 80-Jan-01 00:00 mofmt/parsing/generated/Modelica.py
@@ -16,13 +16,13 @@
 -rw-r--r--  2.0 fat    94541 b- defN 80-Jan-01 00:00 mofmt/parsing/generated/ModelicaLexer.py
 -rw-r--r--  2.0 fat     1997 b- defN 80-Jan-01 00:00 mofmt/parsing/generated/ModelicaLexer.tokens
 -rw-r--r--  2.0 fat    37712 b- defN 80-Jan-01 00:00 mofmt/parsing/generated/ModelicaListener.py
 -rw-r--r--  2.0 fat     8119 b- defN 80-Jan-01 00:00 mofmt/parsing/parser.py
 -rw-r--r--  2.0 fat     1037 b- defN 80-Jan-01 00:00 mofmt/parsing/parsing.py
 -rw-r--r--  2.0 fat       99 b- defN 80-Jan-01 00:00 mofmt/printing/__init__.py
 -rw-r--r--  2.0 fat     1641 b- defN 80-Jan-01 00:00 mofmt/printing/printing.py
--rw-r--r--  2.0 fat       42 b- defN 80-Jan-01 00:00 mofmt-0.2.1.dist-info/entry_points.txt
--rw-r--r--  2.0 fat     1090 b- defN 80-Jan-01 00:00 mofmt-0.2.1.dist-info/LICENSE
--rw-r--r--  2.0 fat     3738 b- defN 80-Jan-01 00:00 mofmt-0.2.1.dist-info/METADATA
--rw-r--r--  2.0 fat       88 b- defN 80-Jan-01 00:00 mofmt-0.2.1.dist-info/WHEEL
-?rw-r--r--  2.0 fat     2163 b- defN 16-Jan-01 00:00 mofmt-0.2.1.dist-info/RECORD
-26 files, 643878 bytes uncompressed, 73781 bytes compressed:  88.5%
+-rw-r--r--  2.0 fat       42 b- defN 80-Jan-01 00:00 mofmt-0.2.2.dist-info/entry_points.txt
+-rw-r--r--  2.0 fat     1090 b- defN 80-Jan-01 00:00 mofmt-0.2.2.dist-info/LICENSE
+-rw-r--r--  2.0 fat     3738 b- defN 80-Jan-01 00:00 mofmt-0.2.2.dist-info/METADATA
+-rw-r--r--  2.0 fat       88 b- defN 80-Jan-01 00:00 mofmt-0.2.2.dist-info/WHEEL
+?rw-r--r--  2.0 fat     2163 b- defN 16-Jan-01 00:00 mofmt-0.2.2.dist-info/RECORD
+26 files, 644051 bytes uncompressed, 73850 bytes compressed:  88.5%
```

## zipnote {}

```diff
@@ -57,23 +57,23 @@
 
 Filename: mofmt/printing/__init__.py
 Comment: 
 
 Filename: mofmt/printing/printing.py
 Comment: 
 
-Filename: mofmt-0.2.1.dist-info/entry_points.txt
+Filename: mofmt-0.2.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: mofmt-0.2.1.dist-info/LICENSE
+Filename: mofmt-0.2.2.dist-info/LICENSE
 Comment: 
 
-Filename: mofmt-0.2.1.dist-info/METADATA
+Filename: mofmt-0.2.2.dist-info/METADATA
 Comment: 
 
-Filename: mofmt-0.2.1.dist-info/WHEEL
+Filename: mofmt-0.2.2.dist-info/WHEEL
 Comment: 
 
-Filename: mofmt-0.2.1.dist-info/RECORD
+Filename: mofmt-0.2.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## CHANGELOG.md

```diff
@@ -1,12 +1,19 @@
 # Changelog
 
 All important changes will be described in this file. Or rather I will
 try to document them here.
 
+## [0.2.2] - 2023-08-04
+
+### Fixed
+
+- Fix issue with incorrect indentation when function call is breaked
+  inside wrapped expression
+
 ## [0.2.1] - 2023-07-06
 
 ### Fixed
 
 - Fix issue with additional blank lines when handling line comments
   between elements
```

## mofmt/collecting/collector.py

```diff
@@ -100,15 +100,15 @@
             self.wrapped = False
         self.add_marker(Marker(Marker.BLANK, "\n\n", "BLANK"))
 
     def add_linebreak(self) -> None:
         """Add a linebreak marker"""
         if self.markers[-1].typ >= Marker.BLANK:
             return
-        if self.wrapped:
+        if self.wrapped and self.markers[-1].val == ";":
             self.add_dedent()
             self.wrapped = False
         self.add_marker(Marker(Marker.LINEBREAK, "\n", "LINEBREAK"))
 
     def add_wrappoint(self) -> None:
         """Add a soft break marker"""
         if not self.wrapped:
```

## Comparing `mofmt-0.2.1.dist-info/LICENSE` & `mofmt-0.2.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mofmt-0.2.1.dist-info/METADATA` & `mofmt-0.2.2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mofmt
-Version: 0.2.1
+Version: 0.2.2
 Summary: Modelica Code Formatter
 Home-page: https://github.com/ErykMroczek/mofmt
 License: MIT
 Keywords: Modelica,automation,formatter
 Author: Eryk Mroczek
 Author-email: mroczek.eryk@gmail.com
 Requires-Python: >=3.9,<4.0
```

## Comparing `mofmt-0.2.1.dist-info/RECORD` & `mofmt-0.2.2.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-CHANGELOG.md,sha256=YOcP38Viar17QAWjhZfrsV2mxZzxRpcZXJRsHnHs3NU,845
+CHANGELOG.md,sha256=_8icj-FDldOUG6fbwDgC6jp-cX7z2GyuEVFzK6S42ak,986
 mofmt/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mofmt/__main__.py,sha256=qPwpG6FZCPK7S67iCLg2EP9-vOynvnhpG5Fq0lAkrvk,35
 mofmt/collecting/__init__.py,sha256=7NpwfO7DzFwMLRikvRoVmM8Mwxtiibybia562T3Sf8Q,70
-mofmt/collecting/collector.py,sha256=_qinhqiALRBuK47vBYUwH1IfcfuTVJEjf86ByWI6-_s,3823
+mofmt/collecting/collector.py,sha256=J0M46docBvHXWY_8fXd_6soy2nB9h5TrJyXXlwHJmvA,3855
 mofmt/io/__init__.py,sha256=Qm6ZTuyhoit16mnpNFdDpMmJhzOxpO799AXLFyLbRHY,146
 mofmt/io/io.py,sha256=RHjEhARszoVHzOELABj1ZPSz5vDJPF30CjcBgdDCjjE,1256
 mofmt/mofmt.py,sha256=JSyhOTCTFwFl96G1cZuKYGNiQcd-u3V-p3xOGUkmyeY,1234
 mofmt/parsing/__init__.py,sha256=N7fwkKpGH8UeVDGaXpNJbpTao74BzL36dK2adR5hP4E,116
 mofmt/parsing/generated/__init__.py,sha256=tQ2uERbsGYNWU8cq9dCK6p2yiW04Y3PTkXirUjdaILs,171
 mofmt/parsing/generated/Modelica.interp,sha256=4pKUOhSzpu4bSa1sL4SmDNzwGuxMIEkua0dRKCDuO5I,41279
 mofmt/parsing/generated/Modelica.py,sha256=CcD0uoQCRJ6G7X8W0eK8E0gmP7bsGHcngdelkcLAePc,413159
@@ -15,12 +15,12 @@
 mofmt/parsing/generated/ModelicaLexer.py,sha256=z-HBw-IlpnCqM9zEtDKsPMloS19xCX2_pRmXRf8WNIw,94541
 mofmt/parsing/generated/ModelicaLexer.tokens,sha256=e64qu0dk424gTRbkNgFfpVXVlMbxA2FsdqxFCXKCOXU,1997
 mofmt/parsing/generated/ModelicaListener.py,sha256=pFjsNbBVfgkX1V04Ldp-X0YcryPds0wExuh0bL6YqMo,37712
 mofmt/parsing/parser.py,sha256=Et4ELpqi3Nt_rp9q3TiqSClo60QgtPQJvzXTo6TsOPQ,8119
 mofmt/parsing/parsing.py,sha256=bZP3vAJUE8k1y67dU3KDsvePH0QaSMHbDYDQ82e9Ls8,1037
 mofmt/printing/__init__.py,sha256=0eOv6gLGz0I9DDcffafMIjC6Z0yJiWYP6Wvh7i1aXO8,99
 mofmt/printing/printing.py,sha256=IaLLhJUFUNhDDJeurbNORQd22gXIOBNxdtYyFoHxGjY,1641
-mofmt-0.2.1.dist-info/entry_points.txt,sha256=OX5RiOFxcysf3SizHLEHHf5n6MdMjFqsZp5QgfA4umM,42
-mofmt-0.2.1.dist-info/LICENSE,sha256=0CTm7r4VXiNrmaDn8y_CYz9u2qdocI8ugBpKtuF2x5g,1090
-mofmt-0.2.1.dist-info/METADATA,sha256=lkRJb_ElUL1yejM7uyBtEGMgiUV8sJIiIOIXrGJhD9A,3738
-mofmt-0.2.1.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
-mofmt-0.2.1.dist-info/RECORD,,
+mofmt-0.2.2.dist-info/entry_points.txt,sha256=OX5RiOFxcysf3SizHLEHHf5n6MdMjFqsZp5QgfA4umM,42
+mofmt-0.2.2.dist-info/LICENSE,sha256=0CTm7r4VXiNrmaDn8y_CYz9u2qdocI8ugBpKtuF2x5g,1090
+mofmt-0.2.2.dist-info/METADATA,sha256=ZXGVp2WZZPVRCjdX1W7EuFNGgXgThbfkaQn9N3upqkA,3738
+mofmt-0.2.2.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
+mofmt-0.2.2.dist-info/RECORD,,
```

