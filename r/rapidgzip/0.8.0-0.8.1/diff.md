# Comparing `tmp/rapidgzip-0.8.0.tar.gz` & `tmp/rapidgzip-0.8.1-pp39-pypy39_pp73-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rapidgzip-0.8.0.tar", last modified: Thu Aug  3 22:37:21 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

