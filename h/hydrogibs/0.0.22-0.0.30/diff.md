# Comparing `tmp/hydrogibs-0.0.22.tar.gz` & `tmp/hydrogibs-0.0.30-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hydrogibs-0.0.22.tar", last modified: Wed Jul  5 07:21:45 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

