# Comparing `tmp/grobid_client_python-0.0.6.tar.gz` & `tmp/grobid_client_python-0.0.7-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grobid_client_python-0.0.6.tar", last modified: Wed Aug  2 13:06:12 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

