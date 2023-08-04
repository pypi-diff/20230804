# Comparing `tmp/aws-cdk.aws-kinesisfirehose-alpha-2.9.0a0.tar.gz` & `tmp/aws_cdk.aws_kinesisfirehose_alpha-2.90.0a0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/codebuild/output/src277428142/src/packages/individual-packages/aws-kinesisfirehose/dist/python/aws-cdk.aws-kinesisfirehose-alp", last modified: Wed Jan 26 11:22:05 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

