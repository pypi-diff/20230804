# Comparing `tmp/rapidgzip-0.7.1.tar.gz` & `tmp/rapidgzip-0.8.0-pp39-pypy39_pp73-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rapidgzip-0.7.1.tar", last modified: Tue Aug  1 16:38:01 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

