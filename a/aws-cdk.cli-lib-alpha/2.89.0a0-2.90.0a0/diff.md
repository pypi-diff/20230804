# Comparing `tmp/aws-cdk.cli-lib-alpha-2.89.0a0.tar.gz` & `tmp/aws-cdk.cli-lib-alpha-2.90.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/codebuild/output/src2022765760/src/packages/@aws-cdk/cli-lib-alpha/dist/python/aws-cdk.cli-lib-alpha-2.89.0a0.tar", last modified: Fri Jul 28 22:05:13 2023, max compression
+gzip compressed data, was "aws-cdk.cli-lib-alpha-2.90.0a0.tar", last modified: Fri Aug  4 19:20:38 2023, max compression
```

## Comparing `aws-cdk.cli-lib-alpha-2.89.0a0.tar` & `aws-cdk.cli-lib-alpha-2.90.0a0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 22:05:13.000000 aws-cdk.cli-lib-alpha-2.89.0a0/
--rw-r--r--   0 root         (0) root         (0)    11391 2023-07-28 22:05:04.000000 aws-cdk.cli-lib-alpha-2.89.0a0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2023-07-28 22:05:08.000000 aws-cdk.cli-lib-alpha-2.89.0a0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      726 2023-07-28 22:05:06.000000 aws-cdk.cli-lib-alpha-2.89.0a0/NOTICE
--rw-r--r--   0 root         (0) root         (0)     4306 2023-07-28 22:05:13.000000 aws-cdk.cli-lib-alpha-2.89.0a0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3319 2023-07-28 22:05:08.000000 aws-cdk.cli-lib-alpha-2.89.0a0/README.md
--rw-r--r--   0 root         (0) root         (0)      234 2023-07-28 22:05:08.000000 aws-cdk.cli-lib-alpha-2.89.0a0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-28 22:05:13.000000 aws-cdk.cli-lib-alpha-2.89.0a0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1766 2023-07-28 22:05:08.000000 aws-cdk.cli-lib-alpha-2.89.0a0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 22:05:13.000000 aws-cdk.cli-lib-alpha-2.89.0a0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 22:05:13.000000 aws-cdk.cli-lib-alpha-2.89.0a0/src/aws_cdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 22:05:13.000000 aws-cdk.cli-lib-alpha-2.89.0a0/src/aws_cdk/cli_lib_alpha/
--rw-r--r--   0 root         (0) root         (0)   256641 2023-07-28 22:05:08.000000 aws-cdk.cli-lib-alpha-2.89.0a0/src/aws_cdk/cli_lib_alpha/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 22:05:13.000000 aws-cdk.cli-lib-alpha-2.89.0a0/src/aws_cdk/cli_lib_alpha/_jsii/
--rw-r--r--   0 root         (0) root         (0)      387 2023-07-28 22:05:08.000000 aws-cdk.cli-lib-alpha-2.89.0a0/src/aws_cdk/cli_lib_alpha/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)  4402330 2023-07-28 22:05:04.000000 aws-cdk.cli-lib-alpha-2.89.0a0/src/aws_cdk/cli_lib_alpha/_jsii/cli-lib-alpha@2.89.0-alpha.0.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 22:05:08.000000 aws-cdk.cli-lib-alpha-2.89.0a0/src/aws_cdk/cli_lib_alpha/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 22:05:13.000000 aws-cdk.cli-lib-alpha-2.89.0a0/src/aws_cdk.cli_lib_alpha.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4306 2023-07-28 22:05:13.000000 aws-cdk.cli-lib-alpha-2.89.0a0/src/aws_cdk.cli_lib_alpha.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      491 2023-07-28 22:05:13.000000 aws-cdk.cli-lib-alpha-2.89.0a0/src/aws_cdk.cli_lib_alpha.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 22:05:13.000000 aws-cdk.cli-lib-alpha-2.89.0a0/src/aws_cdk.cli_lib_alpha.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       57 2023-07-28 22:05:13.000000 aws-cdk.cli-lib-alpha-2.89.0a0/src/aws_cdk.cli_lib_alpha.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-07-28 22:05:13.000000 aws-cdk.cli-lib-alpha-2.89.0a0/src/aws_cdk.cli_lib_alpha.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 19:20:38.283482 aws-cdk.cli-lib-alpha-2.90.0a0/
+-rw-r--r--   0 root         (0) root         (0)    11391 2023-08-04 19:20:25.000000 aws-cdk.cli-lib-alpha-2.90.0a0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2023-08-04 19:20:27.000000 aws-cdk.cli-lib-alpha-2.90.0a0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      726 2023-08-04 19:20:26.000000 aws-cdk.cli-lib-alpha-2.90.0a0/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     4306 2023-08-04 19:20:38.283482 aws-cdk.cli-lib-alpha-2.90.0a0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3319 2023-08-04 19:20:27.000000 aws-cdk.cli-lib-alpha-2.90.0a0/README.md
+-rw-r--r--   0 root         (0) root         (0)      234 2023-08-04 19:20:27.000000 aws-cdk.cli-lib-alpha-2.90.0a0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-04 19:20:38.283482 aws-cdk.cli-lib-alpha-2.90.0a0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1766 2023-08-04 19:20:27.000000 aws-cdk.cli-lib-alpha-2.90.0a0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 19:20:38.279482 aws-cdk.cli-lib-alpha-2.90.0a0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 19:20:38.279482 aws-cdk.cli-lib-alpha-2.90.0a0/src/aws_cdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 19:20:38.279482 aws-cdk.cli-lib-alpha-2.90.0a0/src/aws_cdk/cli_lib_alpha/
+-rw-r--r--   0 root         (0) root         (0)   256641 2023-08-04 19:20:27.000000 aws-cdk.cli-lib-alpha-2.90.0a0/src/aws_cdk/cli_lib_alpha/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 19:20:38.279482 aws-cdk.cli-lib-alpha-2.90.0a0/src/aws_cdk/cli_lib_alpha/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      387 2023-08-04 19:20:27.000000 aws-cdk.cli-lib-alpha-2.90.0a0/src/aws_cdk/cli_lib_alpha/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)  4405518 2023-08-04 19:20:25.000000 aws-cdk.cli-lib-alpha-2.90.0a0/src/aws_cdk/cli_lib_alpha/_jsii/cli-lib-alpha@2.90.0-alpha.0.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 19:20:27.000000 aws-cdk.cli-lib-alpha-2.90.0a0/src/aws_cdk/cli_lib_alpha/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 19:20:38.279482 aws-cdk.cli-lib-alpha-2.90.0a0/src/aws_cdk.cli_lib_alpha.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4306 2023-08-04 19:20:38.000000 aws-cdk.cli-lib-alpha-2.90.0a0/src/aws_cdk.cli_lib_alpha.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      491 2023-08-04 19:20:38.000000 aws-cdk.cli-lib-alpha-2.90.0a0/src/aws_cdk.cli_lib_alpha.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 19:20:38.000000 aws-cdk.cli-lib-alpha-2.90.0a0/src/aws_cdk.cli_lib_alpha.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       57 2023-08-04 19:20:38.000000 aws-cdk.cli-lib-alpha-2.90.0a0/src/aws_cdk.cli_lib_alpha.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-08-04 19:20:38.000000 aws-cdk.cli-lib-alpha-2.90.0a0/src/aws_cdk.cli_lib_alpha.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `aws-cdk.cli-lib-alpha-2.89.0a0/LICENSE` & `aws-cdk.cli-lib-alpha-2.90.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `aws-cdk.cli-lib-alpha-2.89.0a0/NOTICE` & `aws-cdk.cli-lib-alpha-2.90.0a0/NOTICE`

 * *Files identical despite different names*

### Comparing `aws-cdk.cli-lib-alpha-2.89.0a0/PKG-INFO` & `aws-cdk.cli-lib-alpha-2.90.0a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-cdk.cli-lib-alpha
-Version: 2.89.0a0
+Version: 2.90.0a0
 Summary: AWS CDK Programmatic CLI library
 Home-page: https://github.com/aws/aws-cdk
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws/aws-cdk.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `aws-cdk.cli-lib-alpha-2.89.0a0/README.md` & `aws-cdk.cli-lib-alpha-2.90.0a0/README.md`

 * *Files identical despite different names*

### Comparing `aws-cdk.cli-lib-alpha-2.89.0a0/setup.py` & `aws-cdk.cli-lib-alpha-2.90.0a0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "aws-cdk.cli-lib-alpha",
-    "version": "2.89.0.a0",
+    "version": "2.90.0.a0",
     "description": "AWS CDK Programmatic CLI library",
     "license": "Apache-2.0",
     "url": "https://github.com/aws/aws-cdk",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -22,23 +22,23 @@
     },
     "packages": [
         "aws_cdk.cli_lib_alpha",
         "aws_cdk.cli_lib_alpha._jsii"
     ],
     "package_data": {
         "aws_cdk.cli_lib_alpha._jsii": [
-            "cli-lib-alpha@2.89.0-alpha.0.jsii.tgz"
+            "cli-lib-alpha@2.90.0-alpha.0.jsii.tgz"
         ],
         "aws_cdk.cli_lib_alpha": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
-        "jsii>=1.85.0, <2.0.0",
+        "jsii>=1.86.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
```

### Comparing `aws-cdk.cli-lib-alpha-2.89.0a0/src/aws_cdk/cli_lib_alpha/__init__.py` & `aws-cdk.cli-lib-alpha-2.90.0a0/src/aws_cdk/cli_lib_alpha/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-cdk.cli-lib-alpha-2.89.0a0/src/aws_cdk.cli_lib_alpha.egg-info/PKG-INFO` & `aws-cdk.cli-lib-alpha-2.90.0a0/src/aws_cdk.cli_lib_alpha.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-cdk.cli-lib-alpha
-Version: 2.89.0a0
+Version: 2.90.0a0
 Summary: AWS CDK Programmatic CLI library
 Home-page: https://github.com/aws/aws-cdk
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws/aws-cdk.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

