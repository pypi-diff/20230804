# Comparing `tmp/aws-cdk.aws-codestar-alpha-2.9.0a0.tar.gz` & `tmp/aws_cdk.aws_codestar_alpha-2.90.0a0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/codebuild/output/src277428142/src/packages/individual-packages/aws-codestar/dist/python/aws-cdk.aws-codestar-alpha-2.9.0a0.tar", last modified: Wed Jan 26 11:22:04 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

