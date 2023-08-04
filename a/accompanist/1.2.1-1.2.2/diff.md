# Comparing `tmp/accompanist-1.2.1-py3-none-any.whl.zip` & `tmp/accompanist-1.2.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,25 +1,25 @@
-Zip file size: 50383 bytes, number of entries: 23
+Zip file size: 50381 bytes, number of entries: 23
 -rw-r--r--  2.0 unx        0 b- defN 23-May-18 15:07 accompanist/__init__.py
 -rw-r--r--  2.0 unx     8831 b- defN 23-Aug-04 15:41 accompanist/cmd_hear.py
 -rw-r--r--  2.0 unx     1970 b- defN 23-Jul-14 12:07 accompanist/cmd_init.py
 -rw-r--r--  2.0 unx     8499 b- defN 23-Aug-04 15:55 accompanist/cmd_listen.py
 -rw-r--r--  2.0 unx     3637 b- defN 23-Jun-13 14:46 accompanist/cmd_play.py
 -rw-r--r--  2.0 unx      973 b- defN 23-Jul-22 08:32 accompanist/main.py
 -rw-r--r--  2.0 unx     3128 b- defN 23-Aug-04 15:54 accompanist/utility.py
--rw-r--r--  2.0 unx       18 b- defN 23-Aug-04 12:34 accompanist/version.py
+-rw-r--r--  2.0 unx       18 b- defN 23-Aug-04 16:59 accompanist/version.py
 -rw-r--r--  2.0 unx        0 b- defN 23-May-18 15:10 accompanist/report/__init__.py
 -rw-r--r--  2.0 unx     4302 b- defN 23-May-20 15:45 accompanist/report/draw_histgram.py
 -rw-r--r--  2.0 unx     5259 b- defN 23-Jun-15 13:41 accompanist/report/draw_pie_chart.py
 -rw-r--r--  2.0 unx     3562 b- defN 23-May-20 14:16 accompanist/report/draw_table.py
 -rw-r--r--  2.0 unx     1597 b- defN 23-Aug-01 14:58 accompanist/report/write_comment.py
 -rw-r--r--  2.0 unx     1503 b- defN 23-May-21 16:45 accompanist/report/write_front_cover.py
 -rw-r--r--  2.0 unx     3905 b- defN 23-Jun-09 15:09 accompanist/report/write_header_footer.py
 -rw-r--r--  2.0 unx    19193 b- defN 23-Mar-26 08:39 accompanist/resource/logo_trans.png
 -rw-r--r--  2.0 unx     6761 b- defN 23-Mar-26 08:25 accompanist/resource/logo_trans_small.png
--rw-r--r--  2.0 unx     1063 b- defN 23-Aug-04 16:54 accompanist-1.2.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     8820 b- defN 23-Aug-04 16:54 accompanist-1.2.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Aug-04 16:54 accompanist-1.2.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       53 b- defN 23-Aug-04 16:54 accompanist-1.2.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       31 b- defN 23-Aug-04 16:54 accompanist-1.2.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1970 b- defN 23-Aug-04 16:54 accompanist-1.2.1.dist-info/RECORD
-23 files, 85167 bytes uncompressed, 47159 bytes compressed:  44.6%
+-rw-r--r--  2.0 unx     1063 b- defN 23-Aug-04 17:05 accompanist-1.2.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     8810 b- defN 23-Aug-04 17:05 accompanist-1.2.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Aug-04 17:05 accompanist-1.2.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       53 b- defN 23-Aug-04 17:05 accompanist-1.2.2.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       31 b- defN 23-Aug-04 17:05 accompanist-1.2.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1970 b- defN 23-Aug-04 17:05 accompanist-1.2.2.dist-info/RECORD
+23 files, 85157 bytes uncompressed, 47157 bytes compressed:  44.6%
```

## zipnote {}

```diff
@@ -45,26 +45,26 @@
 
 Filename: accompanist/resource/logo_trans.png
 Comment: 
 
 Filename: accompanist/resource/logo_trans_small.png
 Comment: 
 
-Filename: accompanist-1.2.1.dist-info/LICENSE
+Filename: accompanist-1.2.2.dist-info/LICENSE
 Comment: 
 
-Filename: accompanist-1.2.1.dist-info/METADATA
+Filename: accompanist-1.2.2.dist-info/METADATA
 Comment: 
 
-Filename: accompanist-1.2.1.dist-info/WHEEL
+Filename: accompanist-1.2.2.dist-info/WHEEL
 Comment: 
 
-Filename: accompanist-1.2.1.dist-info/entry_points.txt
+Filename: accompanist-1.2.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: accompanist-1.2.1.dist-info/top_level.txt
+Filename: accompanist-1.2.2.dist-info/top_level.txt
 Comment: 
 
-Filename: accompanist-1.2.1.dist-info/RECORD
+Filename: accompanist-1.2.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## accompanist/version.py

```diff
@@ -1 +1 @@
-VERSION = "1.2.1"
+VERSION = "1.2.2"
```

## Comparing `accompanist-1.2.1.dist-info/LICENSE` & `accompanist-1.2.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `accompanist-1.2.1.dist-info/METADATA` & `accompanist-1.2.2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: accompanist
-Version: 1.2.1
+Version: 1.2.2
 Summary: Analysis AWS WAF logs and generate a report
 Author: itsuki
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: click (>=8.1.3)
 Requires-Dist: boto3 (>=1.26.126)
@@ -94,15 +94,15 @@
 ```
 
 # 🌱 How to use
 
 ## Convenient usage
 
 - The "listen" or "hear" with `--json_log`  or `-j`  option can be help to investigate the detail of WAF logs.
-    - [Important] Please handle it with care as sometimes it includes sensitive data.
+    - [Important] Please handle it with care as it includes sensitive data.
     - If you want to confirm a specific access of log, you should re-run "play" with the option and open a json file generated in the current directory.
 - The report color is customizable for when you run "play" with the option, `--color` or `-d` .
 
 ## Precaution
 
 - This tool works with AWS WAFv2 and does not support v1.
 - For AWS Managed Rules, you need to append "AWS" to the prefix, or the histogram works wrong.
```

## Comparing `accompanist-1.2.1.dist-info/RECORD` & `accompanist-1.2.2.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 accompanist/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 accompanist/cmd_hear.py,sha256=DAaG9o4WIkg49o6T8Fd7Jina2_CyIb-TJjbwJx45DwQ,8831
 accompanist/cmd_init.py,sha256=Ca1bNzvhOkcQNcX91JSh3myt2INCVzECcHfFE6wxPys,1970
 accompanist/cmd_listen.py,sha256=u3vsOBDCCxxO2i7sBfkQBkdYGOV-zPJUb1Y2A7oqTIQ,8499
 accompanist/cmd_play.py,sha256=FEyWOz-GBnC5kwA2aComfiDXsybBpf5q8aicV8RYdg8,3637
 accompanist/main.py,sha256=7LyT6KyNbWQ1kobWNwl3tu0_NuwxFRHBNPPbhMRwOFg,973
 accompanist/utility.py,sha256=G9t5MDjmNzSEMkFF-USu3xI90CnPKOVBWKVVvU92KF0,3128
-accompanist/version.py,sha256=QEOrN0FLYbf9G_JHQ21m2esKHMbgVGkm_l_9cpxloj4,18
+accompanist/version.py,sha256=x8lFhSdfuHMCmwSRoPODpZk4iXik5ChlGTaTfg8coBc,18
 accompanist/report/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 accompanist/report/draw_histgram.py,sha256=cYxzjROtITo98QL6M8O98EXKlvM78E-WfE9thsPbzEE,4302
 accompanist/report/draw_pie_chart.py,sha256=xxDRhpxwKWKukWwNPbM8HBkr3_EygquJ9mmw0M9_RKM,5259
 accompanist/report/draw_table.py,sha256=YZ9PpGS6sLaEgYsqL2Jj5yR7_ng1ywrLEozSlyfnNGQ,3562
 accompanist/report/write_comment.py,sha256=cJ7QgdDnU6PAJqPlYAHbH7TgZAYsTQsTy6QNVF4I9mg,1597
 accompanist/report/write_front_cover.py,sha256=lwRs7u17v7NbuoDVS-9TsH0PX0a1WQk-NEzbK3-ez10,1503
 accompanist/report/write_header_footer.py,sha256=uUt-bnbp7T4ktYXVu68WupBOVDsQFXtqPQOx2mq0P30,3905
 accompanist/resource/logo_trans.png,sha256=IbkfTLMa9qzSifN32YocbOdpDRecelHA7k8cLrBVK_4,19193
 accompanist/resource/logo_trans_small.png,sha256=SS9AlZGL3Ce-6BbD4EW5rbn7zuDcje7HkEXW_lHE2zs,6761
-accompanist-1.2.1.dist-info/LICENSE,sha256=EHImwl3uAjnXzz33MkVgnfcyDByFp0t6O-H4QaGLs4M,1063
-accompanist-1.2.1.dist-info/METADATA,sha256=dB1f7osiyF88oMLfHJDks3n-PQg07RQI_dovDEOyJ3g,8820
-accompanist-1.2.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-accompanist-1.2.1.dist-info/entry_points.txt,sha256=gLZwXDl7kf85kYQ1HNQZSxCe81vLub8Eb8wWqrThDeM,53
-accompanist-1.2.1.dist-info/top_level.txt,sha256=vUeFtOUVsBOaqJK8b1z7iVPvaRhz3jGN4Uw79o1o9Ck,31
-accompanist-1.2.1.dist-info/RECORD,,
+accompanist-1.2.2.dist-info/LICENSE,sha256=EHImwl3uAjnXzz33MkVgnfcyDByFp0t6O-H4QaGLs4M,1063
+accompanist-1.2.2.dist-info/METADATA,sha256=G2aM3UqO7AODN_obOz8AFCpLJXVq__gam_FDkMaqdc4,8810
+accompanist-1.2.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+accompanist-1.2.2.dist-info/entry_points.txt,sha256=gLZwXDl7kf85kYQ1HNQZSxCe81vLub8Eb8wWqrThDeM,53
+accompanist-1.2.2.dist-info/top_level.txt,sha256=vUeFtOUVsBOaqJK8b1z7iVPvaRhz3jGN4Uw79o1o9Ck,31
+accompanist-1.2.2.dist-info/RECORD,,
```

