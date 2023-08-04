# Comparing `tmp/proto_clip_toolkit-0.1.tar.gz` & `tmp/proto_clip_toolkit-0.1.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proto_clip_toolkit-0.1.tar", last modified: Fri Jul  7 05:28:11 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

