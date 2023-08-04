# Comparing `tmp/aws-cdk.aws-sagemaker-alpha-2.89.0a0.tar.gz` & `tmp/aws-cdk.aws-sagemaker-alpha-2.90.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/codebuild/output/src2022765760/src/packages/@aws-cdk/aws-sagemaker-alpha/dist/python/aws-cdk.aws-sagemaker-alpha-2.89.0a0.tar", last modified: Fri Jul 28 22:05:35 2023, max compression
+gzip compressed data, was "aws-cdk.aws-sagemaker-alpha-2.90.0a0.tar", last modified: Fri Aug  4 19:21:03 2023, max compression
```

## Comparing `aws-cdk.aws-sagemaker-alpha-2.89.0a0.tar` & `aws-cdk.aws-sagemaker-alpha-2.90.0a0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 22:05:35.000000 aws-cdk.aws-sagemaker-alpha-2.89.0a0/
--rw-r--r--   0 root         (0) root         (0)    11391 2023-07-28 22:05:24.000000 aws-cdk.aws-sagemaker-alpha-2.89.0a0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2023-07-28 22:05:24.000000 aws-cdk.aws-sagemaker-alpha-2.89.0a0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      113 2023-07-28 22:05:24.000000 aws-cdk.aws-sagemaker-alpha-2.89.0a0/NOTICE
--rw-r--r--   0 root         (0) root         (0)     9936 2023-07-28 22:05:35.000000 aws-cdk.aws-sagemaker-alpha-2.89.0a0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8931 2023-07-28 22:05:24.000000 aws-cdk.aws-sagemaker-alpha-2.89.0a0/README.md
--rw-r--r--   0 root         (0) root         (0)      234 2023-07-28 22:05:24.000000 aws-cdk.aws-sagemaker-alpha-2.89.0a0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-28 22:05:35.000000 aws-cdk.aws-sagemaker-alpha-2.89.0a0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1884 2023-07-28 22:05:24.000000 aws-cdk.aws-sagemaker-alpha-2.89.0a0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 22:05:35.000000 aws-cdk.aws-sagemaker-alpha-2.89.0a0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 22:05:35.000000 aws-cdk.aws-sagemaker-alpha-2.89.0a0/src/aws_cdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 22:05:35.000000 aws-cdk.aws-sagemaker-alpha-2.89.0a0/src/aws_cdk/aws_sagemaker_alpha/
--rw-r--r--   0 root         (0) root         (0)   240804 2023-07-28 22:05:24.000000 aws-cdk.aws-sagemaker-alpha-2.89.0a0/src/aws_cdk/aws_sagemaker_alpha/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 22:05:35.000000 aws-cdk.aws-sagemaker-alpha-2.89.0a0/src/aws_cdk/aws_sagemaker_alpha/_jsii/
--rw-r--r--   0 root         (0) root         (0)      445 2023-07-28 22:05:24.000000 aws-cdk.aws-sagemaker-alpha-2.89.0a0/src/aws_cdk/aws_sagemaker_alpha/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)    92185 2023-07-28 22:05:24.000000 aws-cdk.aws-sagemaker-alpha-2.89.0a0/src/aws_cdk/aws_sagemaker_alpha/_jsii/aws-sagemaker-alpha@2.89.0-alpha.0.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 22:05:24.000000 aws-cdk.aws-sagemaker-alpha-2.89.0a0/src/aws_cdk/aws_sagemaker_alpha/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 22:05:35.000000 aws-cdk.aws-sagemaker-alpha-2.89.0a0/src/aws_cdk.aws_sagemaker_alpha.egg-info/
--rw-r--r--   0 root         (0) root         (0)     9936 2023-07-28 22:05:35.000000 aws-cdk.aws-sagemaker-alpha-2.89.0a0/src/aws_cdk.aws_sagemaker_alpha.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      551 2023-07-28 22:05:35.000000 aws-cdk.aws-sagemaker-alpha-2.89.0a0/src/aws_cdk.aws_sagemaker_alpha.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 22:05:35.000000 aws-cdk.aws-sagemaker-alpha-2.89.0a0/src/aws_cdk.aws_sagemaker_alpha.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      104 2023-07-28 22:05:35.000000 aws-cdk.aws-sagemaker-alpha-2.89.0a0/src/aws_cdk.aws_sagemaker_alpha.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-07-28 22:05:35.000000 aws-cdk.aws-sagemaker-alpha-2.89.0a0/src/aws_cdk.aws_sagemaker_alpha.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 19:21:02.999359 aws-cdk.aws-sagemaker-alpha-2.90.0a0/
+-rw-r--r--   0 root         (0) root         (0)    11391 2023-08-04 19:20:48.000000 aws-cdk.aws-sagemaker-alpha-2.90.0a0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2023-08-04 19:20:48.000000 aws-cdk.aws-sagemaker-alpha-2.90.0a0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      113 2023-08-04 19:20:48.000000 aws-cdk.aws-sagemaker-alpha-2.90.0a0/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     9936 2023-08-04 19:21:02.999359 aws-cdk.aws-sagemaker-alpha-2.90.0a0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8931 2023-08-04 19:20:48.000000 aws-cdk.aws-sagemaker-alpha-2.90.0a0/README.md
+-rw-r--r--   0 root         (0) root         (0)      234 2023-08-04 19:20:48.000000 aws-cdk.aws-sagemaker-alpha-2.90.0a0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-04 19:21:02.999359 aws-cdk.aws-sagemaker-alpha-2.90.0a0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1884 2023-08-04 19:20:48.000000 aws-cdk.aws-sagemaker-alpha-2.90.0a0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 19:21:02.995359 aws-cdk.aws-sagemaker-alpha-2.90.0a0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 19:21:02.995359 aws-cdk.aws-sagemaker-alpha-2.90.0a0/src/aws_cdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 19:21:02.995359 aws-cdk.aws-sagemaker-alpha-2.90.0a0/src/aws_cdk/aws_sagemaker_alpha/
+-rw-r--r--   0 root         (0) root         (0)   241116 2023-08-04 19:20:48.000000 aws-cdk.aws-sagemaker-alpha-2.90.0a0/src/aws_cdk/aws_sagemaker_alpha/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 19:21:02.995359 aws-cdk.aws-sagemaker-alpha-2.90.0a0/src/aws_cdk/aws_sagemaker_alpha/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      445 2023-08-04 19:20:48.000000 aws-cdk.aws-sagemaker-alpha-2.90.0a0/src/aws_cdk/aws_sagemaker_alpha/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    92218 2023-08-04 19:20:48.000000 aws-cdk.aws-sagemaker-alpha-2.90.0a0/src/aws_cdk/aws_sagemaker_alpha/_jsii/aws-sagemaker-alpha@2.90.0-alpha.0.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 19:20:48.000000 aws-cdk.aws-sagemaker-alpha-2.90.0a0/src/aws_cdk/aws_sagemaker_alpha/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 19:21:02.995359 aws-cdk.aws-sagemaker-alpha-2.90.0a0/src/aws_cdk.aws_sagemaker_alpha.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     9936 2023-08-04 19:21:02.000000 aws-cdk.aws-sagemaker-alpha-2.90.0a0/src/aws_cdk.aws_sagemaker_alpha.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      551 2023-08-04 19:21:02.000000 aws-cdk.aws-sagemaker-alpha-2.90.0a0/src/aws_cdk.aws_sagemaker_alpha.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 19:21:02.000000 aws-cdk.aws-sagemaker-alpha-2.90.0a0/src/aws_cdk.aws_sagemaker_alpha.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      104 2023-08-04 19:21:02.000000 aws-cdk.aws-sagemaker-alpha-2.90.0a0/src/aws_cdk.aws_sagemaker_alpha.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-08-04 19:21:02.000000 aws-cdk.aws-sagemaker-alpha-2.90.0a0/src/aws_cdk.aws_sagemaker_alpha.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `aws-cdk.aws-sagemaker-alpha-2.89.0a0/LICENSE` & `aws-cdk.aws-sagemaker-alpha-2.90.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `aws-cdk.aws-sagemaker-alpha-2.89.0a0/PKG-INFO` & `aws-cdk.aws-sagemaker-alpha-2.90.0a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-cdk.aws-sagemaker-alpha
-Version: 2.89.0a0
+Version: 2.90.0a0
 Summary: The CDK Construct Library for AWS::SageMaker
 Home-page: https://github.com/aws/aws-cdk
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws/aws-cdk.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `aws-cdk.aws-sagemaker-alpha-2.89.0a0/README.md` & `aws-cdk.aws-sagemaker-alpha-2.90.0a0/README.md`

 * *Files identical despite different names*

### Comparing `aws-cdk.aws-sagemaker-alpha-2.89.0a0/setup.py` & `aws-cdk.aws-sagemaker-alpha-2.90.0a0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "aws-cdk.aws-sagemaker-alpha",
-    "version": "2.89.0.a0",
+    "version": "2.90.0.a0",
     "description": "The CDK Construct Library for AWS::SageMaker",
     "license": "Apache-2.0",
     "url": "https://github.com/aws/aws-cdk",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -22,25 +22,25 @@
     },
     "packages": [
         "aws_cdk.aws_sagemaker_alpha",
         "aws_cdk.aws_sagemaker_alpha._jsii"
     ],
     "package_data": {
         "aws_cdk.aws_sagemaker_alpha._jsii": [
-            "aws-sagemaker-alpha@2.89.0-alpha.0.jsii.tgz"
+            "aws-sagemaker-alpha@2.90.0-alpha.0.jsii.tgz"
         ],
         "aws_cdk.aws_sagemaker_alpha": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
-        "aws-cdk-lib==2.89.0",
+        "aws-cdk-lib==2.90.0",
         "constructs>=10.0.0, <11.0.0",
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

### Comparing `aws-cdk.aws-sagemaker-alpha-2.89.0a0/src/aws_cdk/aws_sagemaker_alpha/__init__.py` & `aws-cdk.aws-sagemaker-alpha-2.90.0a0/src/aws_cdk/aws_sagemaker_alpha/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -559,14 +559,15 @@
     def from_asset(
         cls,
         directory: builtins.str,
         *,
         asset_name: typing.Optional[builtins.str] = None,
         build_args: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
         build_secrets: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
+        build_ssh: typing.Optional[builtins.str] = None,
         cache_from: typing.Optional[typing.Sequence[typing.Union[_aws_cdk_aws_ecr_assets_ceddda9d.DockerCacheOption, typing.Dict[builtins.str, typing.Any]]]] = None,
         cache_to: typing.Optional[typing.Union[_aws_cdk_aws_ecr_assets_ceddda9d.DockerCacheOption, typing.Dict[builtins.str, typing.Any]]] = None,
         file: typing.Optional[builtins.str] = None,
         invalidation: typing.Optional[typing.Union[_aws_cdk_aws_ecr_assets_ceddda9d.DockerImageAssetInvalidationOptions, typing.Dict[builtins.str, typing.Any]]] = None,
         network_mode: typing.Optional[_aws_cdk_aws_ecr_assets_ceddda9d.NetworkMode] = None,
         outputs: typing.Optional[typing.Sequence[builtins.str]] = None,
         platform: typing.Optional[_aws_cdk_aws_ecr_assets_ceddda9d.Platform] = None,
@@ -578,14 +579,15 @@
     ) -> "ContainerImage":
         '''(experimental) Reference an image that's constructed directly from sources on disk.
 
         :param directory: The directory where the Dockerfile is stored.
         :param asset_name: Unique identifier of the docker image asset and its potential revisions. Required if using AppScopedStagingSynthesizer. Default: - no asset name
         :param build_args: Build args to pass to the ``docker build`` command. Since Docker build arguments are resolved before deployment, keys and values cannot refer to unresolved tokens (such as ``lambda.functionArn`` or ``queue.queueUrl``). Default: - no build args are passed
         :param build_secrets: Build secrets. Docker BuildKit must be enabled to use build secrets. Default: - no build secrets
+        :param build_ssh: SSH agent socket or keys to pass to the ``docker build`` command. Docker BuildKit must be enabled to use the ssh flag Default: - no --ssh flag
         :param cache_from: Cache from options to pass to the ``docker build`` command. Default: - no cache from options are passed to the build command
         :param cache_to: Cache to options to pass to the ``docker build`` command. Default: - no cache to options are passed to the build command
         :param file: Path to the Dockerfile (relative to the directory). Default: 'Dockerfile'
         :param invalidation: Options to control which parameters are used to invalidate the asset hash. Default: - hash all parameters
         :param network_mode: Networking mode for the RUN commands during build. Support docker API 1.25+. Default: - no networking mode specified (the default networking mode ``NetworkMode.DEFAULT`` will be used)
         :param outputs: Outputs to pass to the ``docker build`` command. Default: - no outputs are passed to the build command (default outputs are used)
         :param platform: Platform to build for. *Requires Docker Buildx*. Default: - no platform specified (the current machine architecture will be used)
@@ -600,14 +602,15 @@
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__9de8152b52ea9bc7ab7afc08793a9a98145196c9c9f1ff7cee2103ce1cfdb482)
             check_type(argname="argument directory", value=directory, expected_type=type_hints["directory"])
         options = _aws_cdk_aws_ecr_assets_ceddda9d.DockerImageAssetOptions(
             asset_name=asset_name,
             build_args=build_args,
             build_secrets=build_secrets,
+            build_ssh=build_ssh,
             cache_from=cache_from,
             cache_to=cache_to,
             file=file,
             invalidation=invalidation,
             network_mode=network_mode,
             outputs=outputs,
             platform=platform,
@@ -4697,14 +4700,15 @@
 
 def _typecheckingstub__9de8152b52ea9bc7ab7afc08793a9a98145196c9c9f1ff7cee2103ce1cfdb482(
     directory: builtins.str,
     *,
     asset_name: typing.Optional[builtins.str] = None,
     build_args: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
     build_secrets: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
+    build_ssh: typing.Optional[builtins.str] = None,
     cache_from: typing.Optional[typing.Sequence[typing.Union[_aws_cdk_aws_ecr_assets_ceddda9d.DockerCacheOption, typing.Dict[builtins.str, typing.Any]]]] = None,
     cache_to: typing.Optional[typing.Union[_aws_cdk_aws_ecr_assets_ceddda9d.DockerCacheOption, typing.Dict[builtins.str, typing.Any]]] = None,
     file: typing.Optional[builtins.str] = None,
     invalidation: typing.Optional[typing.Union[_aws_cdk_aws_ecr_assets_ceddda9d.DockerImageAssetInvalidationOptions, typing.Dict[builtins.str, typing.Any]]] = None,
     network_mode: typing.Optional[_aws_cdk_aws_ecr_assets_ceddda9d.NetworkMode] = None,
     outputs: typing.Optional[typing.Sequence[builtins.str]] = None,
     platform: typing.Optional[_aws_cdk_aws_ecr_assets_ceddda9d.Platform] = None,
```

### Comparing `aws-cdk.aws-sagemaker-alpha-2.89.0a0/src/aws_cdk.aws_sagemaker_alpha.egg-info/PKG-INFO` & `aws-cdk.aws-sagemaker-alpha-2.90.0a0/src/aws_cdk.aws_sagemaker_alpha.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-cdk.aws-sagemaker-alpha
-Version: 2.89.0a0
+Version: 2.90.0a0
 Summary: The CDK Construct Library for AWS::SageMaker
 Home-page: https://github.com/aws/aws-cdk
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws/aws-cdk.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `aws-cdk.aws-sagemaker-alpha-2.89.0a0/src/aws_cdk.aws_sagemaker_alpha.egg-info/SOURCES.txt` & `aws-cdk.aws-sagemaker-alpha-2.90.0a0/src/aws_cdk.aws_sagemaker_alpha.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 src/aws_cdk.aws_sagemaker_alpha.egg-info/SOURCES.txt
 src/aws_cdk.aws_sagemaker_alpha.egg-info/dependency_links.txt
 src/aws_cdk.aws_sagemaker_alpha.egg-info/requires.txt
 src/aws_cdk.aws_sagemaker_alpha.egg-info/top_level.txt
 src/aws_cdk/aws_sagemaker_alpha/__init__.py
 src/aws_cdk/aws_sagemaker_alpha/py.typed
 src/aws_cdk/aws_sagemaker_alpha/_jsii/__init__.py
-src/aws_cdk/aws_sagemaker_alpha/_jsii/aws-sagemaker-alpha@2.89.0-alpha.0.jsii.tgz
+src/aws_cdk/aws_sagemaker_alpha/_jsii/aws-sagemaker-alpha@2.90.0-alpha.0.jsii.tgz
```

