# Comparing `tmp/django_bread-1.0.4.tar.gz` & `tmp/django_bread-1.0.5-py2.py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_bread-1.0.4.tar", last modified: Thu Mar 24 14:53:45 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

