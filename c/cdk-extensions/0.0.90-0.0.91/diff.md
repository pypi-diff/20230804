# Comparing `tmp/cdk-extensions-0.0.90.tar.gz` & `tmp/cdk-extensions-0.0.91.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-extensions-0.0.90.tar", last modified: Wed Aug  2 18:25:25 2023, max compression
+gzip compressed data, was "cdk-extensions-0.0.91.tar", last modified: Fri Aug  4 13:37:46 2023, max compression
```

## Comparing `cdk-extensions-0.0.90.tar` & `cdk-extensions-0.0.91.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:25:25.290181 cdk-extensions-0.0.90/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-08-02 18:25:10.000000 cdk-extensions-0.0.90/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-02 18:25:10.000000 cdk-extensions-0.0.90/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4632 2023-08-02 18:25:25.290181 cdk-extensions-0.0.90/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-08-02 18:25:10.000000 cdk-extensions-0.0.90/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-08-02 18:25:10.000000 cdk-extensions-0.0.90/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 18:25:25.290181 cdk-extensions-0.0.90/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-08-02 18:25:10.000000 cdk-extensions-0.0.90/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:25:25.270179 cdk-extensions-0.0.90/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:25:25.274180 cdk-extensions-0.0.90/src/cdk_extensions/
--rw-r--r--   0 runner    (1001) docker     (123)     5012 2023-08-02 18:25:10.000000 cdk-extensions-0.0.90/src/cdk_extensions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:25:25.278180 cdk-extensions-0.0.90/src/cdk_extensions/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-08-02 18:25:10.000000 cdk-extensions-0.0.90/src/cdk_extensions/_jsii/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:25:25.278180 cdk-extensions-0.0.90/src/cdk_extensions/_jsii/bin/
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-08-02 18:25:10.000000 cdk-extensions-0.0.90/src/cdk_extensions/_jsii/bin/init-aws.sh
--rw-r--r--   0 runner    (1001) docker     (123)  1804207 2023-08-02 18:25:10.000000 cdk-extensions-0.0.90/src/cdk_extensions/_jsii/cdk-extensions@0.0.90.jsii.tgz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:25:25.278180 cdk-extensions-0.0.90/src/cdk_extensions/alerting/
--rw-r--r--   0 runner    (1001) docker     (123)   342439 2023-08-02 18:25:10.000000 cdk-extensions-0.0.90/src/cdk_extensions/alerting/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:25:25.282180 cdk-extensions-0.0.90/src/cdk_extensions/aps/
--rw-r--r--   0 runner    (1001) docker     (123)   277230 2023-08-02 18:25:10.000000 cdk-extensions-0.0.90/src/cdk_extensions/aps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:25:25.282180 cdk-extensions-0.0.90/src/cdk_extensions/asserts/
--rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-08-02 18:25:10.000000 cdk-extensions-0.0.90/src/cdk_extensions/asserts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:25:25.282180 cdk-extensions-0.0.90/src/cdk_extensions/athena/
--rw-r--r--   0 runner    (1001) docker     (123)   100087 2023-08-02 18:25:10.000000 cdk-extensions-0.0.90/src/cdk_extensions/athena/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:25:25.282180 cdk-extensions-0.0.90/src/cdk_extensions/core/
--rw-r--r--   0 runner    (1001) docker     (123)    20196 2023-08-02 18:25:10.000000 cdk-extensions-0.0.90/src/cdk_extensions/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:25:25.282180 cdk-extensions-0.0.90/src/cdk_extensions/ec2/
--rw-r--r--   0 runner    (1001) docker     (123)   702329 2023-08-02 18:25:10.000000 cdk-extensions-0.0.90/src/cdk_extensions/ec2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:25:25.282180 cdk-extensions-0.0.90/src/cdk_extensions/ec2_patterns/
--rw-r--r--   0 runner    (1001) docker     (123)   278700 2023-08-02 18:25:10.000000 cdk-extensions-0.0.90/src/cdk_extensions/ec2_patterns/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:25:25.282180 cdk-extensions-0.0.90/src/cdk_extensions/eks_patterns/
--rw-r--r--   0 runner    (1001) docker     (123)    96878 2023-08-02 18:25:10.000000 cdk-extensions-0.0.90/src/cdk_extensions/eks_patterns/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:25:25.282180 cdk-extensions-0.0.90/src/cdk_extensions/glue/
--rw-r--r--   0 runner    (1001) docker     (123)   507542 2023-08-02 18:25:10.000000 cdk-extensions-0.0.90/src/cdk_extensions/glue/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:25:25.282180 cdk-extensions-0.0.90/src/cdk_extensions/glue_tables/
--rw-r--r--   0 runner    (1001) docker     (123)   140877 2023-08-02 18:25:10.000000 cdk-extensions-0.0.90/src/cdk_extensions/glue_tables/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:25:25.282180 cdk-extensions-0.0.90/src/cdk_extensions/guardduty/
--rw-r--r--   0 runner    (1001) docker     (123)    60471 2023-08-02 18:25:10.000000 cdk-extensions-0.0.90/src/cdk_extensions/guardduty/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:25:25.286180 cdk-extensions-0.0.90/src/cdk_extensions/k8s_aws/
--rw-r--r--   0 runner    (1001) docker     (123)   692580 2023-08-02 18:25:10.000000 cdk-extensions-0.0.90/src/cdk_extensions/k8s_aws/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:25:25.286180 cdk-extensions-0.0.90/src/cdk_extensions/k8s_fargate/
--rw-r--r--   0 runner    (1001) docker     (123)    26236 2023-08-02 18:25:10.000000 cdk-extensions-0.0.90/src/cdk_extensions/k8s_fargate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:25:25.286180 cdk-extensions-0.0.90/src/cdk_extensions/kinesis_firehose/
--rw-r--r--   0 runner    (1001) docker     (123)   271406 2023-08-02 18:25:10.000000 cdk-extensions-0.0.90/src/cdk_extensions/kinesis_firehose/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:25:25.286180 cdk-extensions-0.0.90/src/cdk_extensions/lambda_/
--rw-r--r--   0 runner    (1001) docker     (123)    22981 2023-08-02 18:25:10.000000 cdk-extensions-0.0.90/src/cdk_extensions/lambda_/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:25:25.286180 cdk-extensions-0.0.90/src/cdk_extensions/networkmanager/
--rw-r--r--   0 runner    (1001) docker     (123)    40858 2023-08-02 18:25:10.000000 cdk-extensions-0.0.90/src/cdk_extensions/networkmanager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 18:25:10.000000 cdk-extensions-0.0.90/src/cdk_extensions/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:25:25.286180 cdk-extensions-0.0.90/src/cdk_extensions/ram/
--rw-r--r--   0 runner    (1001) docker     (123)    42369 2023-08-02 18:25:10.000000 cdk-extensions-0.0.90/src/cdk_extensions/ram/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:25:25.286180 cdk-extensions-0.0.90/src/cdk_extensions/ram_resources/
--rw-r--r--   0 runner    (1001) docker     (123)     5162 2023-08-02 18:25:10.000000 cdk-extensions-0.0.90/src/cdk_extensions/ram_resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:25:25.286180 cdk-extensions-0.0.90/src/cdk_extensions/rds/
--rw-r--r--   0 runner    (1001) docker     (123)    18474 2023-08-02 18:25:10.000000 cdk-extensions-0.0.90/src/cdk_extensions/rds/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:25:25.286180 cdk-extensions-0.0.90/src/cdk_extensions/resourcegroups/
--rw-r--r--   0 runner    (1001) docker     (123)    39153 2023-08-02 18:25:10.000000 cdk-extensions-0.0.90/src/cdk_extensions/resourcegroups/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:25:25.286180 cdk-extensions-0.0.90/src/cdk_extensions/route53/
--rw-r--r--   0 runner    (1001) docker     (123)    11199 2023-08-02 18:25:10.000000 cdk-extensions-0.0.90/src/cdk_extensions/route53/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:25:25.286180 cdk-extensions-0.0.90/src/cdk_extensions/s3_buckets/
--rw-r--r--   0 runner    (1001) docker     (123)   215599 2023-08-02 18:25:10.000000 cdk-extensions-0.0.90/src/cdk_extensions/s3_buckets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:25:25.286180 cdk-extensions-0.0.90/src/cdk_extensions/sso/
--rw-r--r--   0 runner    (1001) docker     (123)   130474 2023-08-02 18:25:10.000000 cdk-extensions-0.0.90/src/cdk_extensions/sso/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:25:25.290181 cdk-extensions-0.0.90/src/cdk_extensions/stacks/
--rw-r--r--   0 runner    (1001) docker     (123)    60527 2023-08-02 18:25:10.000000 cdk-extensions-0.0.90/src/cdk_extensions/stacks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:25:25.290181 cdk-extensions-0.0.90/src/cdk_extensions/stepfunctions/
--rw-r--r--   0 runner    (1001) docker     (123)    23021 2023-08-02 18:25:10.000000 cdk-extensions-0.0.90/src/cdk_extensions/stepfunctions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:25:25.278180 cdk-extensions-0.0.90/src/cdk_extensions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4632 2023-08-02 18:25:25.000000 cdk-extensions-0.0.90/src/cdk_extensions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-08-02 18:25:25.000000 cdk-extensions-0.0.90/src/cdk_extensions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 18:25:25.000000 cdk-extensions-0.0.90/src/cdk_extensions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-08-02 18:25:25.000000 cdk-extensions-0.0.90/src/cdk_extensions.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-02 18:25:25.000000 cdk-extensions-0.0.90/src/cdk_extensions.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:37:46.558490 cdk-extensions-0.0.91/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-08-04 13:37:28.000000 cdk-extensions-0.0.91/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-04 13:37:28.000000 cdk-extensions-0.0.91/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4632 2023-08-04 13:37:46.558490 cdk-extensions-0.0.91/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-08-04 13:37:28.000000 cdk-extensions-0.0.91/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-08-04 13:37:28.000000 cdk-extensions-0.0.91/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 13:37:46.558490 cdk-extensions-0.0.91/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-08-04 13:37:28.000000 cdk-extensions-0.0.91/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:37:46.542490 cdk-extensions-0.0.91/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:37:46.546490 cdk-extensions-0.0.91/src/cdk_extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)     5012 2023-08-04 13:37:28.000000 cdk-extensions-0.0.91/src/cdk_extensions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:37:46.546490 cdk-extensions-0.0.91/src/cdk_extensions/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-08-04 13:37:28.000000 cdk-extensions-0.0.91/src/cdk_extensions/_jsii/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:37:46.550490 cdk-extensions-0.0.91/src/cdk_extensions/_jsii/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-08-04 13:37:28.000000 cdk-extensions-0.0.91/src/cdk_extensions/_jsii/bin/init-aws.sh
+-rw-r--r--   0 runner    (1001) docker     (123)  1804207 2023-08-04 13:37:28.000000 cdk-extensions-0.0.91/src/cdk_extensions/_jsii/cdk-extensions@0.0.91.jsii.tgz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:37:46.550490 cdk-extensions-0.0.91/src/cdk_extensions/alerting/
+-rw-r--r--   0 runner    (1001) docker     (123)   342439 2023-08-04 13:37:28.000000 cdk-extensions-0.0.91/src/cdk_extensions/alerting/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:37:46.550490 cdk-extensions-0.0.91/src/cdk_extensions/aps/
+-rw-r--r--   0 runner    (1001) docker     (123)   277230 2023-08-04 13:37:28.000000 cdk-extensions-0.0.91/src/cdk_extensions/aps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:37:46.550490 cdk-extensions-0.0.91/src/cdk_extensions/asserts/
+-rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-08-04 13:37:28.000000 cdk-extensions-0.0.91/src/cdk_extensions/asserts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:37:46.550490 cdk-extensions-0.0.91/src/cdk_extensions/athena/
+-rw-r--r--   0 runner    (1001) docker     (123)   100087 2023-08-04 13:37:28.000000 cdk-extensions-0.0.91/src/cdk_extensions/athena/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:37:46.550490 cdk-extensions-0.0.91/src/cdk_extensions/core/
+-rw-r--r--   0 runner    (1001) docker     (123)    20196 2023-08-04 13:37:28.000000 cdk-extensions-0.0.91/src/cdk_extensions/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:37:46.550490 cdk-extensions-0.0.91/src/cdk_extensions/ec2/
+-rw-r--r--   0 runner    (1001) docker     (123)   702329 2023-08-04 13:37:28.000000 cdk-extensions-0.0.91/src/cdk_extensions/ec2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:37:46.550490 cdk-extensions-0.0.91/src/cdk_extensions/ec2_patterns/
+-rw-r--r--   0 runner    (1001) docker     (123)   278700 2023-08-04 13:37:28.000000 cdk-extensions-0.0.91/src/cdk_extensions/ec2_patterns/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:37:46.554490 cdk-extensions-0.0.91/src/cdk_extensions/eks_patterns/
+-rw-r--r--   0 runner    (1001) docker     (123)    96878 2023-08-04 13:37:28.000000 cdk-extensions-0.0.91/src/cdk_extensions/eks_patterns/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:37:46.554490 cdk-extensions-0.0.91/src/cdk_extensions/glue/
+-rw-r--r--   0 runner    (1001) docker     (123)   507542 2023-08-04 13:37:28.000000 cdk-extensions-0.0.91/src/cdk_extensions/glue/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:37:46.554490 cdk-extensions-0.0.91/src/cdk_extensions/glue_tables/
+-rw-r--r--   0 runner    (1001) docker     (123)   140877 2023-08-04 13:37:28.000000 cdk-extensions-0.0.91/src/cdk_extensions/glue_tables/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:37:46.554490 cdk-extensions-0.0.91/src/cdk_extensions/guardduty/
+-rw-r--r--   0 runner    (1001) docker     (123)    60471 2023-08-04 13:37:28.000000 cdk-extensions-0.0.91/src/cdk_extensions/guardduty/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:37:46.554490 cdk-extensions-0.0.91/src/cdk_extensions/k8s_aws/
+-rw-r--r--   0 runner    (1001) docker     (123)   692580 2023-08-04 13:37:28.000000 cdk-extensions-0.0.91/src/cdk_extensions/k8s_aws/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:37:46.554490 cdk-extensions-0.0.91/src/cdk_extensions/k8s_fargate/
+-rw-r--r--   0 runner    (1001) docker     (123)    26236 2023-08-04 13:37:28.000000 cdk-extensions-0.0.91/src/cdk_extensions/k8s_fargate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:37:46.554490 cdk-extensions-0.0.91/src/cdk_extensions/kinesis_firehose/
+-rw-r--r--   0 runner    (1001) docker     (123)   271406 2023-08-04 13:37:28.000000 cdk-extensions-0.0.91/src/cdk_extensions/kinesis_firehose/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:37:46.554490 cdk-extensions-0.0.91/src/cdk_extensions/lambda_/
+-rw-r--r--   0 runner    (1001) docker     (123)    22981 2023-08-04 13:37:28.000000 cdk-extensions-0.0.91/src/cdk_extensions/lambda_/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:37:46.558490 cdk-extensions-0.0.91/src/cdk_extensions/networkmanager/
+-rw-r--r--   0 runner    (1001) docker     (123)    40858 2023-08-04 13:37:28.000000 cdk-extensions-0.0.91/src/cdk_extensions/networkmanager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 13:37:28.000000 cdk-extensions-0.0.91/src/cdk_extensions/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:37:46.558490 cdk-extensions-0.0.91/src/cdk_extensions/ram/
+-rw-r--r--   0 runner    (1001) docker     (123)    42369 2023-08-04 13:37:28.000000 cdk-extensions-0.0.91/src/cdk_extensions/ram/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:37:46.558490 cdk-extensions-0.0.91/src/cdk_extensions/ram_resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     5162 2023-08-04 13:37:28.000000 cdk-extensions-0.0.91/src/cdk_extensions/ram_resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:37:46.558490 cdk-extensions-0.0.91/src/cdk_extensions/rds/
+-rw-r--r--   0 runner    (1001) docker     (123)    18474 2023-08-04 13:37:28.000000 cdk-extensions-0.0.91/src/cdk_extensions/rds/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:37:46.558490 cdk-extensions-0.0.91/src/cdk_extensions/resourcegroups/
+-rw-r--r--   0 runner    (1001) docker     (123)    39153 2023-08-04 13:37:28.000000 cdk-extensions-0.0.91/src/cdk_extensions/resourcegroups/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:37:46.558490 cdk-extensions-0.0.91/src/cdk_extensions/route53/
+-rw-r--r--   0 runner    (1001) docker     (123)    11199 2023-08-04 13:37:28.000000 cdk-extensions-0.0.91/src/cdk_extensions/route53/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:37:46.558490 cdk-extensions-0.0.91/src/cdk_extensions/s3_buckets/
+-rw-r--r--   0 runner    (1001) docker     (123)   215599 2023-08-04 13:37:28.000000 cdk-extensions-0.0.91/src/cdk_extensions/s3_buckets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:37:46.558490 cdk-extensions-0.0.91/src/cdk_extensions/sso/
+-rw-r--r--   0 runner    (1001) docker     (123)   130474 2023-08-04 13:37:28.000000 cdk-extensions-0.0.91/src/cdk_extensions/sso/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:37:46.558490 cdk-extensions-0.0.91/src/cdk_extensions/stacks/
+-rw-r--r--   0 runner    (1001) docker     (123)    60527 2023-08-04 13:37:28.000000 cdk-extensions-0.0.91/src/cdk_extensions/stacks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:37:46.558490 cdk-extensions-0.0.91/src/cdk_extensions/stepfunctions/
+-rw-r--r--   0 runner    (1001) docker     (123)    23021 2023-08-04 13:37:28.000000 cdk-extensions-0.0.91/src/cdk_extensions/stepfunctions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:37:46.546490 cdk-extensions-0.0.91/src/cdk_extensions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4632 2023-08-04 13:37:46.000000 cdk-extensions-0.0.91/src/cdk_extensions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-08-04 13:37:46.000000 cdk-extensions-0.0.91/src/cdk_extensions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 13:37:46.000000 cdk-extensions-0.0.91/src/cdk_extensions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-08-04 13:37:46.000000 cdk-extensions-0.0.91/src/cdk_extensions.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-04 13:37:46.000000 cdk-extensions-0.0.91/src/cdk_extensions.egg-info/top_level.txt
```

### Comparing `cdk-extensions-0.0.90/LICENSE` & `cdk-extensions-0.0.91/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.90/PKG-INFO` & `cdk-extensions-0.0.91/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-extensions
-Version: 0.0.90
+Version: 0.0.91
 Summary: cdk-extensions
 Home-page: https://github.com/vibe-io/cdk-extensions.git
 Author: Kevin Lucas<kevinluc08@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/vibe-io/cdk-extensions.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk-extensions-0.0.90/README.md` & `cdk-extensions-0.0.91/README.md`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.90/setup.py` & `cdk-extensions-0.0.91/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-extensions",
-    "version": "0.0.90",
+    "version": "0.0.91",
     "description": "cdk-extensions",
     "license": "Apache-2.0",
     "url": "https://github.com/vibe-io/cdk-extensions.git",
     "long_description_content_type": "text/markdown",
     "author": "Kevin Lucas<kevinluc08@gmail.com>",
     "bdist_wheel": {
         "universal": true
@@ -47,25 +47,25 @@
         "cdk_extensions.s3_buckets",
         "cdk_extensions.sso",
         "cdk_extensions.stacks",
         "cdk_extensions.stepfunctions"
     ],
     "package_data": {
         "cdk_extensions._jsii": [
-            "cdk-extensions@0.0.90.jsii.tgz"
+            "cdk-extensions@0.0.91.jsii.tgz"
         ],
         "cdk_extensions": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
         "aws-cdk-lib>=2.87.0, <3.0.0",
         "constructs>=10.0.5, <11.0.0",
-        "jsii>=1.86.0, <2.0.0",
+        "jsii>=1.86.1, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
```

### Comparing `cdk-extensions-0.0.90/src/cdk_extensions/__init__.py` & `cdk-extensions-0.0.91/src/cdk_extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.90/src/cdk_extensions/alerting/__init__.py` & `cdk-extensions-0.0.91/src/cdk_extensions/alerting/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.90/src/cdk_extensions/aps/__init__.py` & `cdk-extensions-0.0.91/src/cdk_extensions/aps/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.90/src/cdk_extensions/asserts/__init__.py` & `cdk-extensions-0.0.91/src/cdk_extensions/asserts/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.90/src/cdk_extensions/athena/__init__.py` & `cdk-extensions-0.0.91/src/cdk_extensions/athena/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.90/src/cdk_extensions/core/__init__.py` & `cdk-extensions-0.0.91/src/cdk_extensions/core/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.90/src/cdk_extensions/ec2/__init__.py` & `cdk-extensions-0.0.91/src/cdk_extensions/ec2/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.90/src/cdk_extensions/ec2_patterns/__init__.py` & `cdk-extensions-0.0.91/src/cdk_extensions/ec2_patterns/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.90/src/cdk_extensions/eks_patterns/__init__.py` & `cdk-extensions-0.0.91/src/cdk_extensions/eks_patterns/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.90/src/cdk_extensions/glue/__init__.py` & `cdk-extensions-0.0.91/src/cdk_extensions/glue/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.90/src/cdk_extensions/glue_tables/__init__.py` & `cdk-extensions-0.0.91/src/cdk_extensions/glue_tables/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.90/src/cdk_extensions/guardduty/__init__.py` & `cdk-extensions-0.0.91/src/cdk_extensions/guardduty/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.90/src/cdk_extensions/k8s_aws/__init__.py` & `cdk-extensions-0.0.91/src/cdk_extensions/k8s_aws/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.90/src/cdk_extensions/k8s_fargate/__init__.py` & `cdk-extensions-0.0.91/src/cdk_extensions/k8s_fargate/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.90/src/cdk_extensions/kinesis_firehose/__init__.py` & `cdk-extensions-0.0.91/src/cdk_extensions/kinesis_firehose/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.90/src/cdk_extensions/lambda_/__init__.py` & `cdk-extensions-0.0.91/src/cdk_extensions/lambda_/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.90/src/cdk_extensions/networkmanager/__init__.py` & `cdk-extensions-0.0.91/src/cdk_extensions/networkmanager/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.90/src/cdk_extensions/ram/__init__.py` & `cdk-extensions-0.0.91/src/cdk_extensions/ram/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.90/src/cdk_extensions/ram_resources/__init__.py` & `cdk-extensions-0.0.91/src/cdk_extensions/ram_resources/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.90/src/cdk_extensions/rds/__init__.py` & `cdk-extensions-0.0.91/src/cdk_extensions/rds/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.90/src/cdk_extensions/resourcegroups/__init__.py` & `cdk-extensions-0.0.91/src/cdk_extensions/resourcegroups/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.90/src/cdk_extensions/route53/__init__.py` & `cdk-extensions-0.0.91/src/cdk_extensions/route53/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.90/src/cdk_extensions/s3_buckets/__init__.py` & `cdk-extensions-0.0.91/src/cdk_extensions/s3_buckets/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.90/src/cdk_extensions/sso/__init__.py` & `cdk-extensions-0.0.91/src/cdk_extensions/sso/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.90/src/cdk_extensions/stacks/__init__.py` & `cdk-extensions-0.0.91/src/cdk_extensions/stacks/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.90/src/cdk_extensions/stepfunctions/__init__.py` & `cdk-extensions-0.0.91/src/cdk_extensions/stepfunctions/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.90/src/cdk_extensions.egg-info/PKG-INFO` & `cdk-extensions-0.0.91/src/cdk_extensions.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-extensions
-Version: 0.0.90
+Version: 0.0.91
 Summary: cdk-extensions
 Home-page: https://github.com/vibe-io/cdk-extensions.git
 Author: Kevin Lucas<kevinluc08@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/vibe-io/cdk-extensions.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk-extensions-0.0.90/src/cdk_extensions.egg-info/SOURCES.txt` & `cdk-extensions-0.0.91/src/cdk_extensions.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 src/cdk_extensions/py.typed
 src/cdk_extensions.egg-info/PKG-INFO
 src/cdk_extensions.egg-info/SOURCES.txt
 src/cdk_extensions.egg-info/dependency_links.txt
 src/cdk_extensions.egg-info/requires.txt
 src/cdk_extensions.egg-info/top_level.txt
 src/cdk_extensions/_jsii/__init__.py
-src/cdk_extensions/_jsii/cdk-extensions@0.0.90.jsii.tgz
+src/cdk_extensions/_jsii/cdk-extensions@0.0.91.jsii.tgz
 src/cdk_extensions/_jsii/bin/init-aws.sh
 src/cdk_extensions/alerting/__init__.py
 src/cdk_extensions/aps/__init__.py
 src/cdk_extensions/asserts/__init__.py
 src/cdk_extensions/athena/__init__.py
 src/cdk_extensions/core/__init__.py
 src/cdk_extensions/ec2/__init__.py
```

