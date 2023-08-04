# Comparing `tmp/aws-cdk.aws-servicecatalogappregistry-alpha-2.9.0a0.tar.gz` & `tmp/aws-cdk.aws-servicecatalogappregistry-alpha-2.90.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/codebuild/output/src277428142/src/packages/individual-packages/aws-servicecatalogappregistry/dist/python/aws-cdk.aws-serviceca", last modified: Wed Jan 26 11:22:06 2022, max compression
+gzip compressed data, was "aws-cdk.aws-servicecatalogappregistry-alpha-2.90.0a0.tar", last modified: Fri Aug  4 19:21:01 2023, max compression
```

## Comparing `aws-cdk.aws-servicecatalogappregistry-alpha-2.9.0a0.tar` & `aws-cdk.aws-servicecatalogappregistry-alpha-2.90.0a0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 11:22:06.000000 aws-cdk.aws-servicecatalogappregistry-alpha-2.9.0a0/
--rw-r--r--   0 root         (0) root         (0)    11391 2022-01-26 11:22:01.000000 aws-cdk.aws-servicecatalogappregistry-alpha-2.9.0a0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2022-01-26 11:22:01.000000 aws-cdk.aws-servicecatalogappregistry-alpha-2.9.0a0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      113 2022-01-26 11:22:01.000000 aws-cdk.aws-servicecatalogappregistry-alpha-2.9.0a0/NOTICE
--rw-r--r--   0 root         (0) root         (0)     5341 2022-01-26 11:22:06.000000 aws-cdk.aws-servicecatalogappregistry-alpha-2.9.0a0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4337 2022-01-26 11:22:01.000000 aws-cdk.aws-servicecatalogappregistry-alpha-2.9.0a0/README.md
--rw-r--r--   0 root         (0) root         (0)      106 2022-01-26 11:22:01.000000 aws-cdk.aws-servicecatalogappregistry-alpha-2.9.0a0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2022-01-26 11:22:06.000000 aws-cdk.aws-servicecatalogappregistry-alpha-2.9.0a0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1921 2022-01-26 11:22:01.000000 aws-cdk.aws-servicecatalogappregistry-alpha-2.9.0a0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 11:22:06.000000 aws-cdk.aws-servicecatalogappregistry-alpha-2.9.0a0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 11:22:06.000000 aws-cdk.aws-servicecatalogappregistry-alpha-2.9.0a0/src/aws_cdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 11:22:06.000000 aws-cdk.aws-servicecatalogappregistry-alpha-2.9.0a0/src/aws_cdk/aws_servicecatalogappregistry_alpha/
--rw-r--r--   0 root         (0) root         (0)    23272 2022-01-26 11:22:01.000000 aws-cdk.aws-servicecatalogappregistry-alpha-2.9.0a0/src/aws_cdk/aws_servicecatalogappregistry_alpha/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 11:22:06.000000 aws-cdk.aws-servicecatalogappregistry-alpha-2.9.0a0/src/aws_cdk/aws_servicecatalogappregistry_alpha/_jsii/
--rw-r--r--   0 root         (0) root         (0)      441 2022-01-26 11:22:01.000000 aws-cdk.aws-servicecatalogappregistry-alpha-2.9.0a0/src/aws_cdk/aws_servicecatalogappregistry_alpha/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)    29601 2022-01-26 11:22:01.000000 aws-cdk.aws-servicecatalogappregistry-alpha-2.9.0a0/src/aws_cdk/aws_servicecatalogappregistry_alpha/_jsii/aws-servicecatalogappregistry-alpha@2.9.0-alpha.0.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2022-01-26 11:22:01.000000 aws-cdk.aws-servicecatalogappregistry-alpha-2.9.0a0/src/aws_cdk/aws_servicecatalogappregistry_alpha/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-26 11:22:06.000000 aws-cdk.aws-servicecatalogappregistry-alpha-2.9.0a0/src/aws_cdk.aws_servicecatalogappregistry_alpha.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5341 2022-01-26 11:22:06.000000 aws-cdk.aws-servicecatalogappregistry-alpha-2.9.0a0/src/aws_cdk.aws_servicecatalogappregistry_alpha.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      710 2022-01-26 11:22:06.000000 aws-cdk.aws-servicecatalogappregistry-alpha-2.9.0a0/src/aws_cdk.aws_servicecatalogappregistry_alpha.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-01-26 11:22:06.000000 aws-cdk.aws-servicecatalogappregistry-alpha-2.9.0a0/src/aws_cdk.aws_servicecatalogappregistry_alpha.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       92 2022-01-26 11:22:06.000000 aws-cdk.aws-servicecatalogappregistry-alpha-2.9.0a0/src/aws_cdk.aws_servicecatalogappregistry_alpha.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2022-01-26 11:22:06.000000 aws-cdk.aws-servicecatalogappregistry-alpha-2.9.0a0/src/aws_cdk.aws_servicecatalogappregistry_alpha.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 19:21:01.687368 aws-cdk.aws-servicecatalogappregistry-alpha-2.90.0a0/
+-rw-r--r--   0 root         (0) root         (0)    11391 2023-08-04 19:20:48.000000 aws-cdk.aws-servicecatalogappregistry-alpha-2.90.0a0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2023-08-04 19:20:48.000000 aws-cdk.aws-servicecatalogappregistry-alpha-2.90.0a0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      113 2023-08-04 19:20:48.000000 aws-cdk.aws-servicecatalogappregistry-alpha-2.90.0a0/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    14832 2023-08-04 19:21:01.683368 aws-cdk.aws-servicecatalogappregistry-alpha-2.90.0a0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    13795 2023-08-04 19:20:48.000000 aws-cdk.aws-servicecatalogappregistry-alpha-2.90.0a0/README.md
+-rw-r--r--   0 root         (0) root         (0)      234 2023-08-04 19:20:48.000000 aws-cdk.aws-servicecatalogappregistry-alpha-2.90.0a0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-04 19:21:01.687368 aws-cdk.aws-servicecatalogappregistry-alpha-2.90.0a0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1996 2023-08-04 19:20:48.000000 aws-cdk.aws-servicecatalogappregistry-alpha-2.90.0a0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 19:21:01.683368 aws-cdk.aws-servicecatalogappregistry-alpha-2.90.0a0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 19:21:01.683368 aws-cdk.aws-servicecatalogappregistry-alpha-2.90.0a0/src/aws_cdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 19:21:01.683368 aws-cdk.aws-servicecatalogappregistry-alpha-2.90.0a0/src/aws_cdk/aws_servicecatalogappregistry_alpha/
+-rw-r--r--   0 root         (0) root         (0)   177067 2023-08-04 19:20:48.000000 aws-cdk.aws-servicecatalogappregistry-alpha-2.90.0a0/src/aws_cdk/aws_servicecatalogappregistry_alpha/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 19:21:01.683368 aws-cdk.aws-servicecatalogappregistry-alpha-2.90.0a0/src/aws_cdk/aws_servicecatalogappregistry_alpha/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      477 2023-08-04 19:20:48.000000 aws-cdk.aws-servicecatalogappregistry-alpha-2.90.0a0/src/aws_cdk/aws_servicecatalogappregistry_alpha/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    74084 2023-08-04 19:20:48.000000 aws-cdk.aws-servicecatalogappregistry-alpha-2.90.0a0/src/aws_cdk/aws_servicecatalogappregistry_alpha/_jsii/aws-servicecatalogappregistry-alpha@2.90.0-alpha.0.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 19:20:48.000000 aws-cdk.aws-servicecatalogappregistry-alpha-2.90.0a0/src/aws_cdk/aws_servicecatalogappregistry_alpha/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 19:21:01.683368 aws-cdk.aws-servicecatalogappregistry-alpha-2.90.0a0/src/aws_cdk.aws_servicecatalogappregistry_alpha.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    14832 2023-08-04 19:21:01.000000 aws-cdk.aws-servicecatalogappregistry-alpha-2.90.0a0/src/aws_cdk.aws_servicecatalogappregistry_alpha.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      711 2023-08-04 19:21:01.000000 aws-cdk.aws-servicecatalogappregistry-alpha-2.90.0a0/src/aws_cdk.aws_servicecatalogappregistry_alpha.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 19:21:01.000000 aws-cdk.aws-servicecatalogappregistry-alpha-2.90.0a0/src/aws_cdk.aws_servicecatalogappregistry_alpha.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      104 2023-08-04 19:21:01.000000 aws-cdk.aws-servicecatalogappregistry-alpha-2.90.0a0/src/aws_cdk.aws_servicecatalogappregistry_alpha.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-08-04 19:21:01.000000 aws-cdk.aws-servicecatalogappregistry-alpha-2.90.0a0/src/aws_cdk.aws_servicecatalogappregistry_alpha.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `aws-cdk.aws-servicecatalogappregistry-alpha-2.9.0a0/LICENSE` & `aws-cdk.aws-servicecatalogappregistry-alpha-2.90.0a0/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -182,15 +182,15 @@
       replaced with your own identifying information. (Don't include
       the brackets!)  The text should be enclosed in the appropriate
       comment syntax for the file format. We also recommend that a
       file or class name and description of purpose be included on the
       same "printed page" as the copyright notice for easier
       identification within third-party archives.
 
-   Copyright 2018-2022 Amazon.com, Inc. or its affiliates. All Rights Reserved.
+   Copyright 2018-2023 Amazon.com, Inc. or its affiliates. All Rights Reserved.
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `aws-cdk.aws-servicecatalogappregistry-alpha-2.9.0a0/setup.py` & `aws-cdk.aws-servicecatalogappregistry-alpha-2.90.0a0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "aws-cdk.aws-servicecatalogappregistry-alpha",
-    "version": "2.9.0.a0",
+    "version": "2.90.0.a0",
     "description": "The CDK Construct Library for AWS::ServiceCatalogAppRegistry",
     "license": "Apache-2.0",
     "url": "https://github.com/aws/aws-cdk",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -22,41 +22,43 @@
     },
     "packages": [
         "aws_cdk.aws_servicecatalogappregistry_alpha",
         "aws_cdk.aws_servicecatalogappregistry_alpha._jsii"
     ],
     "package_data": {
         "aws_cdk.aws_servicecatalogappregistry_alpha._jsii": [
-            "aws-servicecatalogappregistry-alpha@2.9.0-alpha.0.jsii.tgz"
+            "aws-servicecatalogappregistry-alpha@2.90.0-alpha.0.jsii.tgz"
         ],
         "aws_cdk.aws_servicecatalogappregistry_alpha": [
             "py.typed"
         ]
     },
-    "python_requires": ">=3.6",
+    "python_requires": "~=3.7",
     "install_requires": [
-        "aws-cdk-lib>=2.9.0, <3.0.0",
+        "aws-cdk-lib==2.90.0",
         "constructs>=10.0.0, <11.0.0",
-        "jsii>=1.52.1, <2.0.0",
-        "publication>=0.0.3"
+        "jsii>=1.86.0, <2.0.0",
+        "publication>=0.0.3",
+        "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
         "Programming Language :: Python :: 3 :: Only",
-        "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Typing :: Typed",
         "Development Status :: 4 - Beta",
         "License :: OSI Approved",
         "Framework :: AWS CDK",
-        "Framework :: AWS CDK :: 1"
+        "Framework :: AWS CDK :: 2"
     ],
     "scripts": []
 }
 """
 )
 
 with open("README.md", encoding="utf8") as fp:
```

### Comparing `aws-cdk.aws-servicecatalogappregistry-alpha-2.9.0a0/src/aws_cdk.aws_servicecatalogappregistry_alpha.egg-info/SOURCES.txt` & `aws-cdk.aws-servicecatalogappregistry-alpha-2.90.0a0/src/aws_cdk.aws_servicecatalogappregistry_alpha.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 src/aws_cdk.aws_servicecatalogappregistry_alpha.egg-info/SOURCES.txt
 src/aws_cdk.aws_servicecatalogappregistry_alpha.egg-info/dependency_links.txt
 src/aws_cdk.aws_servicecatalogappregistry_alpha.egg-info/requires.txt
 src/aws_cdk.aws_servicecatalogappregistry_alpha.egg-info/top_level.txt
 src/aws_cdk/aws_servicecatalogappregistry_alpha/__init__.py
 src/aws_cdk/aws_servicecatalogappregistry_alpha/py.typed
 src/aws_cdk/aws_servicecatalogappregistry_alpha/_jsii/__init__.py
-src/aws_cdk/aws_servicecatalogappregistry_alpha/_jsii/aws-servicecatalogappregistry-alpha@2.9.0-alpha.0.jsii.tgz
+src/aws_cdk/aws_servicecatalogappregistry_alpha/_jsii/aws-servicecatalogappregistry-alpha@2.90.0-alpha.0.jsii.tgz
```

