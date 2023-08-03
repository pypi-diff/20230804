# Comparing `tmp/PyPartMC-0.4.0.tar.gz` & `tmp/PyPartMC-0.5.0-cp38-cp38-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyPartMC-0.4.0.tar", last modified: Tue Aug  1 23:25:44 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

