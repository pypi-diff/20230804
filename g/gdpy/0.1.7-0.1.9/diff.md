# Comparing `tmp/gdpy-0.1.7.tar.gz` & `tmp/gdpy-0.1.9-py2.py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/gdpy-0.1.7.tar", last modified: Thu Mar 28 09:29:12 2019, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

