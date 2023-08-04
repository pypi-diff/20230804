# Comparing `tmp/botocore-a-la-carte-entityresolution-1.31.18.tar.gz` & `tmp/botocore_a_la_carte_entityresolution-1.31.19-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-entityresolution-1.31.18.tar", last modified: Thu Aug  3 01:14:34 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

